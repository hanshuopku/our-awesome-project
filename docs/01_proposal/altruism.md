# 裸利他第一秒：无外挂利他突变如何逃过瞬时清洗  

---

### 路线 1　突变–漂变走廊  
**钩子**  
在最残酷的负选择面前，只要突变够勤快，利他也能靠“买彩票”活下来。  

**核心疑问**  
裸利他（s = −Δc）在小种群且持续突变条件下，能否靠中性漂变反复“冲关”，累积到后续机制可接管频率？  

**模型骨架**  
1. Moran 过程 + 往返突变：A→a 速率 0，a→A 速率 μ  
2. 解析逃穿概率：φ_esc ≈ 1 − exp(−2μ/s · ln N)  
3. τ-leap 随机模拟：10⁵ 条 trajectory，N = 50–500，s = 0.01–0.05  

**可观测**  
- f_esc：A ≥ 5 % 至少一次的运行比例  
- T_esc：首次突破 5 % 的世代数  

**实验系统**  
酵母微种群（N = 100）+ 人工“利他”SUC2 分泌构建（耗 ATP）+ Bar-seq 每 6 h 读数。  

**关键预测**  
μ* ≈ s / ln N 是临界突变率；N = 100、s = 0.02 时 μ* ≈ 2×10⁻⁵，背景突变率可比。  

---
### Route 1 Mutation–Drift Corridor  
**Hook**  
Even under lethal selection, a lottery ticket called "recurrent mutation" can keep altruism alive.  

**Core Question**  
Can a naked altruistic allele (s = −Δc) in a small population repeatedly breach the 5 % threshold by drift alone, buying time for later mechanisms?  

**Model Skeleton**  
1. Moran process with recurrent mutation (a → A at rate μ; A → a at rate 0)  
2. Analytical escape probability: φ_esc ≈ 1 − exp(−2μ/s · ln N)  
3. τ-leap simulations: 10⁵ trajectories, N = 50–500, s = 0.01–0.05  

**Observables**  
- f_esc: fraction of runs where A ≥ 5 % at least once  
- T_esc: generations to first exceed 5 %  

**Empirical System**  
Yeast micro-populations (N = 100) carrying a synthetic "altruistic" SUC2 secretion construct (costs ATP) read by Bar-seq every 6 h.  

**Key Prediction**  
Critical mutation rate μ* ≈ s / ln N; for N = 100 and s = 0.02, μ* ≈ 2×10⁻⁵, comparable to background mutation rate.  

---

### 路线 2　背景选择掩体  
**钩子**  
利他位点本身有害，却恰好搭上一列高适应度的“ genomic 列车”。  

**核心疑问**  
若 A 与高背景适应度座 B 紧密连锁，背景优势能否暂时掩盖 Δc，让 A 活到重组剥离日？  

**模型骨架**  
SLiM 单染色体模型：B 座（+s_bg）与 A 座（−Δc）重组率 r，参数扫 s_bg ∈ [0.01,0.1]，r ∈ [0,0.1]  

**可观测**  
- T_10：A 达 10 % 所需世代  
- R_strip：重组剥离导致 A 骤降的事件率  

**实验系统**  
大肠杆菌：将“利他”氨苄酶分泌质粒（cost 3 %）插入不同 rpoB 有益背景（+8 %），用 IS10 控制 r。  

**关键预测**  
r < 10⁻³ 且 s_bg > 2Δc 时 T_10 延 10 倍；连锁半衰期 t½ ≈ ln 2 / (r·s_bg)  

---
### Route 2 Background-Selection Shield  
**Hook**  
The altruistic site is bad, but it hitch-hikes on a high-fitness genomic train.  

**Core Question**  
Can a linked beneficial background temporarily mask the cost of A until recombination unhooks it?  

**Model Skeleton**  
SLiM single-chromosome: background locus B (+s_bg) tightly linked (r) to altruistic locus A (−Δc); sweep s_bg ∈ [0.01,0.1], r ∈ [0,0.1]  

**Observables**  
- T_10: generations for A to reach 10 % frequency  
- R_strip: rate of recombination-induced crashes  

**Empirical System**  
E. coli: insert "altruistic" ampicillinase plasmid (cost 3 %) into chromosomes carrying different rpoB beneficial alleles (+8 %); control r with engineered IS10.  

**Key Prediction**  
When r < 10⁻³ and s_bg > 2Δc, T_10 increases ten-fold; linkage half-life t½ ≈ ln 2 / (r·s_bg).  

---

### 路线 3　表型延迟暴露  
**钩子**  
先生长以“自私”身份复制几代，再亮身份——时间换空间。  

**核心疑问**  
发育或阈值延迟能否让 A 频率在沉默期突破临界？  

**模型骨架**  
阈值模型：个体出生后 τ 代内不表达利他；τ ~ Poisson(τ_mean)；有效选择 s_eff = −Δc · P(已表达)  

**可观测**  
- τ*：使 A ≥ 5 % 的最小延迟  
- ε：提前表达误差率  

**实验系统**  
斑马鱼：用激素诱导启动子驱动 cecropin，调控诱导时机，CRISPR barcode 追踪 lineage。  

**关键预测**  
τ* ≈ 1 / s；ε > 5 % 则延迟收益全失。  

---
### Route 3 Phenotypic Delay  
**Hook**  
Born selfish, turn altruist later—trade time for frequency.  

**Core Question**  
Can developmental or environmentally gated delay let A rise silently before the cost appears?  

**Model Skeleton**  
Threshold model: individuals express altruism only after τ ~ Poisson(τ_mean) generations; effective selection s_eff = −Δc · P(expressed)  

**Observables**  
- τ*: minimum delay for A to exceed 5 %  
- ε: premature-expression error rate  

**Empirical System**  
Zebrafish carrying mifepristone-inducible cecropin transgene; induction timing controlled by water-borne dose, lineage tracked with CRISPR barcodes.  

**Key Prediction**  
τ* ≈ 1 / s; premature rate ε > 5 % cancels the escape benefit.  

---

### 路线 4　随机肥尾收益  
**钩子**  
同一行为多数时候吃亏，偶尔天降横财——肥尾让少数 lineage 一夜暴富。  

**核心疑问**  
在随机灾难/大奖环境下，负期望但正肥尾能否使 A 存活？  

**模型骨架**  
分支过程：每代成本 −Δc；灾难时收益 B ~ Pareto(α, B_min)，概率 p_disaster  

**可观测**  
- P_surv(α, Δc)：存活且频率 > 5 % 概率  
- T_burst：条件爆发时间  

**实验系统**  
线虫：利他者分泌甘油（耗 5 % 适合度），干旱事件幂律间隔；微流控湿度随机切换。  

**关键预测**  
尾指数 α < 2 时 P_surv 与 Δc 无关且 > 1 %；逃生条件：α < 1 + Δc / B_min  

---
### Route 4 Fat-Tail Random Returns  
**Hook**  
Mostly you lose, but rarely the sky falls—fat-tail winds make a few lineages jackpot-rich.  

**Core Question**  
In random environments with rare but large benefits, can a negative-mean altruistic strategy survive via lineage-level jackpot events?  

**Model Skeleton**  
Branching process: cost −Δc per generation; catastrophe benefit B ~ Pareto(α, B_min) with probability p_disaster  

**Observables**  
- P_surv(α, Δc): survival AND frequency > 5 %  
- T_burst: conditional time to explosive growth  

**Empirical System**  
C. elegans: altruistic individuals secrete glycerol (costs 5 % fecundity); desiccation events follow power-law intervals in micro-fluidic humidity chambers.  

**Key Prediction**  
Tail index α < 2 yields P_surv independent of Δc and > 1 %; first analytical "fat-tail escape" condition: α < 1 + Δc / B_min.  

---

### 路线 5　亲代–子代黏附  
**钩子**  
无需识别，子代就留在出生地——第一秒自动生成亲缘簇，r > 0 立生效。  

**核心疑问**  
空间黏附 alone 能否在无量化识别下保护裸利他？  

**模型骨架**  
连续空间 Moran：子代投放半径 σ_d 内；计算局部 r 随 σ_d 衰减  

**可观测**  
- r vs σ_d 曲线  
- T_cluster：利他斑块被自私入侵的平均时间  

**实验系统**  
水蚤：成体携卵，释放距离由流速控制；无人机成像测簇寿命。  

**关键预测**  
σ_d* ≈ 0.3 × 平均邻距；黏附不等式 σ_d < σ_d* 是裸利他存活的**充分最小条件**。  

---
### Route 5 Parent–Offspring Adhesion  
**Hook**  
No green beard, no recognition—just stay at home and kin clustering appears for free.  

**Core Question**  
Can limited offspring dispersal alone generate sufficiently high local relatedness to protect a naked altruistic allele?  

**Model Skeleton**  
Continuous-space Moran: offspring dispersed within Gaussian σ_d from parent; compute local r vs σ_d  

**Observables**  
- r vs σ_d decay curve  
- T_cluster: average lifetime of altruistic patch before selfish invasion  

**Empirical System**  
Daphnia magna: neonates remain in maternal brood pouch; release distance manipulated by flow velocity in 1 m linear tanks, drone imaging records cluster dissolution.  

**Key Prediction**  
σ_d* ≈ 0.3 × mean inter-individual distance; adhesion inequality σ_d < σ_d* is the minimal sufficient condition for naked altruism survival.
