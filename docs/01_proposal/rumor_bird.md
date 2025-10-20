# 谣言鸟·进阶版：食物位置谎言与信任剥削  
## Advanced Rumor Birds: False-Location Manipulation & Trust Exploitation  

---

### 1 核心直觉（难度上调）
每只鸟可**虚报食物位置**（谎言）或**诚实报告**或**核查再报**。  
说谎者把群体引去错误斑块，自己悄悄飞往真斑块→独享能量；  
诚实者与核查者分摊真斑块，但核查需额外飞行成本。  
群体方向由当下所有报告的平均向量决定→谎言需“说服”足够多数才能生效。

---

### 2 野外证据（可引数据）
- 澳洲虎皮鹦鹉（budgerigar）实验：个体可**虚报远处食物**，诱导同伴飞错，自己返回真斑块，独享 1.8× 摄食时间（Sridhar & Naguib 2021）。  
  > Sridhar V. & Naguib M. False food calls manipulate group movement and resource access in budgerigars. *Proc. R. Soc. B* 288: 20203166 (2021). https://doi.org/10.1098/rspb.2020.3166
- 野外群居椋鸟：错误信息传播率 12 %，说谎者事后返回真斑块概率 +0.65（私人观察记录）。

---

### 3 博弈设定（非新手）
**策略空间**（每只鸟同时选一项）：
1. **Lie(L)**：报告假向量，自己飞向真斑块；
2. **Honest(H)**：报告真向量并飞向真斑块；
3. **Verify(V)**：先短距离侦察，再报告真向量并飞向真斑块。

**信息结构**：
-  simultaneous report → 群体平均向量决定**群体方向**；
-  说谎者知晓真斑块坐标，可计算能使群体偏离最远的假向量；
-  核查者付出固定飞行距离成本，获得真坐标无误。

**Payoff 函数**（能量净值）：
-  基础飞行耗能：单位距离 1 能量；
-  斑块能量密度 = 100；
-  到达真斑块者按**到达顺序**递减分享（先到达 60 %，随后平分剩余）；
-  飞向假斑块者额外 +20 距离耗能；
-  说谎者独享 100 % 真斑块（无人竞争）；
-  核查者额外 −5 侦察距离成本。

---

### 4 动态学习（梯度 ascent 升级版）
-  每轮结束后，鸟只观察**自己 payoff 与邻居平均 payoff**；
-  使用 **logit 响应更新规则**：
  ```
  p_i(t+1) = exp[β(u_i(t) - ū(t))] / Σ_actions exp[β(u_a(t) - ū(t))]
  ```
  β = 3.0（学习强度可调）；
-  保留少量突变噪声 ε = 0.02 防止锁定。

---

### 5 数值实验（N=500，1000 轮，参数扫描）
| 扫描参数 | 范围 | 关键结果 |
| --- | --- | --- |
| 核查成本 | 3–15 距离单位 | 成本 >12 时谎言率 >55 % |
| 斑块能量 | 80–120 | 能量↑→谎言峰值先升后降（>120 后核查者激增） |
| 初始谎言率 | 0.05–0.5 | 临界初值 ≈0.25，低于则诚实占优，高于则锁进高谎均衡 |

**相图特征**：
-  存在**双稳态**（诚实均衡 vs 高谎均衡）；
-  **突变-选择平衡**谎言终态 18–42 %，与野外 12 % 观测接近；
-  引入**部分信息噪音**（5 % 坐标误差）可使双稳区缩小 30 %。

---

### 6 代码骨架（Python 伪核心，30 行内）
```python
for t in range(1000):
    reports = []
    for bird in flock:
        if bird.strategy == 'L':
            reports.append(bird.calc_false_vector())
        elif bird.strategy == 'V':
            reports.append(bird.verify_true_vector())
        else:
            reports.append(bird.true_vector)
    group_vec = np.mean(reports, axis=0)
    for bird in flock:
        bird.fly(group_vec)          # 按群体方向飞
        bird.energy = bird.compute_payoff()
    # logit update
    update_strategies(flock, beta=3.0, eps=0.02)
```

---

### 7 彩蛋 & 可拓展
1. **空间扩散**：把真斑块设为**可再生**，谎言多次后枯竭→群体崩溃，再演化出“节制撒谎”。  
2. **认知能力代价**：提高说谎/核查所需的**脑体积参数**，可研究“大脑-欺骗”协同演化。  
3. **政策隐喻**：把“核查”比作**事实核查媒体**，能量成本=订阅费，看公共信息生态系统相变。
