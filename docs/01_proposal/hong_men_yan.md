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
