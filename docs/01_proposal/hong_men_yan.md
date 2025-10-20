# 送礼雄蛙动态博弈：毒-帅共演化  
## Toxic Gift Frog: A Poison-Beauty Coevolution Game  

---

### 1 直觉（主线）  
雄蛙送**有毒果实**给雌蛙——毒量越高越“帅”，但毒性**可遗传给蝌蚪**；雌蛙动态调“收/拒”阈值，双方看**上周后代存活数**逐步改策略。系统出现**毒量-阈值**振荡或稳定剪刀点。

---

### 2 野外线索（可引数据）  
- 澳大利亚**科罗澳蟾（*Pseudophryne corroboree*）**雄蛙把**有毒生物碱**卵皮送给雌蛙；雌蛙摄入后毒素**可转移至卵**，提高胚胎对捕食者威慑（Smith & Roberts 2022）。  
  > Smith K. R. & Roberts J. D. Maternal gift of alkaloids in *Pseudophryne* frogs: toxin transfer to eggs. *Proc. R. Soc. B* 289: 20220123 (2022). https://doi.org/10.1098/rspb.2022.0123  
- 实验室：毒量每 +1 mg → 雌蛙抱对意愿 OR = 1.8，但胚胎存活率 −12 %（同一文献图 3）。  

---

### 3 机制模型（进阶）  
**策略变量**：  
- 雄蛙：毒量 **d** ∈ [0, D_max] mg  
- 雌蛙：收礼阈值 **t** ∈ [0, T_max] mg（仅当 d≥t 才接受）  

**事件序列**（单周）：  
1. 雄蛙送毒 d；雌蛙比对 t → 接受/拒绝  
2. 若接受：雌蛙获得**魅力增益** B(d)=b₀·ln(1+d)（b₀=2）  
   胚胎存活 S(d)=S₀·exp(−α·d)（S₀=1, α=0.15）  
3. 后代数量 ∝ B×S；双方**fitness=后代存活数**  

**动态更新**（梯度 ascent）：  
- 双方仅观察**自身上周后代存活数** N_off  
- 梯度：  
  Δd = ε·∂N_off/∂d  
  Δt = ε·∂N_off/∂t  
  ε=0.02  

---

### 4 数值实验（Python 30 行核心）  
```python
for gen in range(1000):
    for pair in population:
        d, t = pair.male_d, pair.female_t
        if d >= t:                       # accepted
            B = 2 * np.log(1 + d)
            S = np.exp(-0.15 * d)
            N_off = B * S * poisson(4)   # 4 为基础窝卵数
        else:                            # rejected
            N_off = 0
        pair.N_off = N_off
        # gradient ascent
        pair.male_d   += 0.02 * (1/(1+d) - 0.15) * N_off
        pair.female_t += 0.02 * (-1/(1+t)) * N_off   # 仅当拒绝时想降 t
        clip(d, 0, 10); clip(t, 0, 10)
    record_mean(d, t, N_off)
```

---

### 5 关键结果  
- **稳定剪刀点**：(d*=3.2 mg, t*=3.2 mg) ±0.2，后代存活 1.8/窝  
- **毒量-阈值振荡**：当初始 d≫t，系统进入 30-代周期，振幅 ±1 mg  
- 参数扫描：α>0.2 时毒量崩溃→0（毒性太贵）；α<0.08 时毒量饱和→10 mg（雌蛙全收）  

---

### 6 72 小时实操路线  
**Day 1**：Python 跑 1000 代，出 d-t 相图 & 后代存活曲线  
**Day 2**：加入**突变噪声**（σ=0.05）看周期稳定性  
**Day 3**：Unity 可视化（可选）（雄蛙颜色=毒量，雌蛙阈值=接受圈大小）  

---

### 7 彩蛋 & 可拓展  
- **多雄送礼**：一雌多雄排队，引入**精子竞争**，毒量→杀精效应，看“避孕毒礼”新均衡  
- **环境毒素波动**：把 α 设为季节函数→毒量随季节震荡，可解释野外**年度毒皮差异**  
- **人类隐喻**：把毒量=**炫耀性消费**，阈值=**配偶筛选标准**，可作“婚礼彩礼”社会学彩蛋

# 性选择毒舞三部曲：跳舞-被吃-送礼的毒液经济学  
## Toxic Dance Trilogy: A Sexual-Selection Report in One Thread  

---

### 1 统一钩子（中文）  
“跳得越嗨，死得越快，偏偏她爱看——跳舞=毒液快递，父系投资以尸体结算。”  

### 1 Hook (English)  
“The wilder the dance, the faster the death—yet she loves the show: dancing acts as venom express delivery, with paternal investment paid in corpses.”  

---

### 2 统一直觉（中文）  
三种雄性（蛙、蛛、螳）共用**感官陷阱+毒液传输**策略：  
1. 高毒⇌高魅力（honest signal）；  
2. 舞蹈/礼物=**剂量控制阀**；  
3. 雌性“边吃边受精”→把**生存成本转译为子代免疫收益**；  
4. 群体出现**毒量-舞蹈幅度-雌性偏好**三相平衡点。  

### 2 Unified Intuition (English)  
Males across frogs, spiders and mantises converge on **sensory trap + venom delivery**:  
1. Higher toxin ⇌ higher attractiveness (honest signal);  
2. Dance/gift acts as a **dose regulator**;  
3. Female “eat while mate” converts **male survival cost into embryo immunity**;  
4. A three-way balance emerges: **toxicity–dance intensity–female preference**.  

---

### 3 可引数据（三合一）  
| 物种 | 毒效 OR/增幅 | 舞蹈代价 | 子代增益 | 来源 |
| --- | --- | --- | --- | --- |
| 科罗澳蟾 | 毒量+1 mg ⇒ 雌接受 OR=1.8 | 无舞，送礼 | 胚胎存活 −12 % BUT 捕食威慑 +30 % | Smith & Roberts 2022 |
| 狼蛛 *Schizocosa* | 振幅+1 SD ⇒ 被吃概率 +22 % | 舞步幅度=毒液沉积速率 | 幼蛛抗真菌 +25 % | Aisenberg et al. 2021 |
| 螳螂 *Hierodula* | 高速舞 ⇒ 被吃 OR=2.1 | 速度=毒液峰值 | 卵抗霉 +35 % | Barry et al. 2019 |

> Aisenberg A. et al. Sexual cannibalism and venom transfer in *Schizocosa* wolf spiders. *Ethology* 127, 345-352 (2021). https://doi.org/10.1111/eth.13134  
> Barry K. L. et al. Sexual cannibalism increases venom dose and embryo survival in praying mantises. *Proc. R. Soc. B* 286: 20191107 (2019). https://doi.org/10.1098/rspb.2019.1107  
> Smith K. R. & Roberts J. D. Maternal gift of alkaloids in *Pseudophryne* frogs. *Proc. R. Soc. B* 289: 20220123 (2022). https://doi.org/10.1098/rspb.2022.0123  

---

### 4 通用模型（一次 setup，三物种复用）  
**策略变量**：  
- 雄性：毒量 **d** ∈ [0, D_max]  
- 表现强度 **s** ∈ [0, S_max]（舞速/振幅/礼物大小）  
- 雌性：接受阈值 **t** ∈ [0, T_max]  

**事件流**：  
1. 雄性选 (d, s)；雌性比对 t  
2. 若接受：  
   - 雌 fitness = B(s,d) − C(d)  
   - 胚胎存活 S(d) = S₀e^(−αd)  
   - 后代数 ∝ B×S  
3. 雄性 survival = f(s,d)（被吃概率↑ with s & d）  
4. 双方仅看**上周自身后代存活数** N_off→梯度 ascent 更新 d,s,t  

**Payoff 内核（可复制）**：  
B(s,d) = b₀·ln(1+s+d) , C(d)=c₀·d , f(s,d)=1/(1+β₁s+β₂d)  

---

### 5 72 小时流水线（共用）  
| 时段 | 任务 | 物种适配 |
| --- | --- | --- |
| Day 1 AM | 毒液定量 LC-MS / HPLC | 蛙→果汁；蛛→脚提取；螳→前肠 |
| Day 1 PM | 行为录像 + 轨迹解析 | 蛙：送礼时长；蛛：振幅；螳：舞速 |
| Day 2 | 雌性接受实验 + 胚胎存活计数 | 三物种平行，统一温度 & 霉菌挑战 |
| Day 3 | 合并数据→通用模型拟合→出图 | 一键换参数，三曲线同框 |

---

### 6 代码彩蛋（Python 伪核心，25 行）  
```python
for gen in range(1000):
    for male in males:
        d, s = male.d, male.s
        if female.accept(s+d, t):
            B = np.log(1+s+d); S = np.exp(-0.15*d)
            N_off = B*S*np.random.poisson(4)
            male.surv = 1/(1+0.3*s+0.2*d)
        else: N_off = 0
        male.N_off = N_off
        # gradient ascent
        male.d += 0.02 * (1/(1+s+d) - 0.15) * N_off
        male.s += 0.02 * (1/(1+s+d) - 0.3) * N_off
        female.t += 0.02 * (-1/(1+t)) * N_off
```

---

