# 恋爱脑：颜值零相关与审美进化博弈

## 钩子
雄性毒羽鸟靠吃毒果让羽毛更艳，却把毒性遗传给雏鸟；雌性越挑“帅哥”，家族寿命越短。  
如果“长得帅”对后代质量零相关甚至负相关，功能派择偶突变为何没有崩溃这种“恋爱脑”审美？我们提出**颜值-零相关陷阱**(ZRL Trap)，用博弈论+可学习雌性+遗传算法，量化“审美净化”的动态红线。

## 核心问题
- 是否存在临界漂移速度σ*，让务实策略永远入侵失败？  
- 能否用AI雌性实时演化择偶网络，主动“净化”糟糕审美？  
- 给出可计算的搜索-误配红线β，预测极端信号何时被锁死或释放？

## 模型框架
| 基因座 | 等位基因 | 效应 |
|--------|----------|------|
| S      | S(帅/渣), s(普通) | 雄性信号；零生存收益，轻微捕食风险 |
| P      | P(颜控), p(务实) | 雌性偏好；p需支付搜索成本C_s探测隐藏质量Q |
| Q      | Q(+20 %幼体存活), q(无) | 不可直接观测，仅p型雌性可花费C_s探测 |

动态红线条件：β = (S频率) × (C_s / 繁殖窗口) &gt; 1 时，p突变无法固定。

## 审美漂移
- 雌性偏好强度α每世代加入随机游走Δα ~ N(0, σ_α)
- σ_α越大，颜控越易漂移到“极端审美”，进一步拉高S频率，反向强化红线

## AI净化实验
- 遗传算法演化雌性神经网络：输入=雄性信号、可见成本、带噪Q值；输出=接受/拒绝
- 适应度=一生繁殖输出×幼体存活
- 并行深度学习预测器实时评估“若全网转向务实”的期望fitness，触发净化相变
- 预期出现150代周期的“净化-再污染”循环；降低C_s可缩短至40代，提供干预破口

## 预期发现
- σ* ≈ 2×Q突变出现率，审美漂移超此速即永恒ZRL
- AI实验将显示：只要搜索成本不可降，恋爱脑即无法被自然选择“卸载”
- 首次给出可计算红线β与漂移-功能比δ，为极端性选择提供动态阈值

## 下一步扩展
- 多模信号(色+声)升高搜索维度，检验净化难度指数上升
- 荧光标记Q的小鼠/果蝇实验演化，实测降低C_s后红线是否下移


# Love-Brain: Zero-Related Looks and the Evolutionary Game of Aesthetics

## Hook
Male toxic-plume birds eat poisonous berries to brighten their feathers, then pass the toxin to their chicks. Females that prefer the handsomest males shorten family lifespan. If “being handsome” has zero—or even negative—effects on offspring quality, why hasn’t natural selection crashed this “love-brain” aesthetic? We introduce the **Zero-Relatedness Look (ZRL) Trap** and combine game theory, learnable females, and genetic algorithms to quantify the dynamic red line for “aesthetic purification.”

## Core Questions
- Is there a critical drift rate σ* that forever prevents pragmatic preference alleles from invading?
- Can AI-evolved females actively “purify” bad taste in real time?
- We provide the first computable search-mismatch threshold β to predict when extreme signals are locked in or released.

## Model Framework
| Locus | Alleles | Effect |
|-------|---------|--------|
| S     | S (sexy/zero-benefit), s (plain) | Male signal; zero survival gain, slight predation risk |
| P     | P (aesthetic), p (pragmatic) | Female preference; p pays search cost C_s to probe hidden quality Q |
| Q     | Q (+20 % juvenile survival), q (null) | Not directly observable; only p-type females can detect it at cost C_s |

Dynamic red-line condition: β = (S frequency) × (C_s / reproductive window) &gt; 1 ⇒ p mutant cannot invade.

## Aesthetic Drift
- Female preference strength α undergoes random walk Δα ~ N(0, σ_α) each generation
- Larger σ_α drives preference into extreme regions, boosting S frequency and reinforcing the red line

## AI Purification Experiment
- Evolve female mating networks with genetic algorithms: inputs = male signal, visible cost, noisy Q value; output = accept/reject
- Fitness = lifetime reproductive output × offspring survival
- Parallel deep-learning predictor estimates expected fitness under a global pragmatic switch; triggers a purification transition when mean_net &gt; mean_aesthetic
- Expect 150-generation cycles of “purge–re-contamination”; reducing C_s shortens cycles to ~40 generations, offering an intervention lever

## Expected Findings
- σ* ≈ 2 × Q-mutation arrival rate; drift above this speed eternalizes ZRL
- AI simulations will show: as long as search costs cannot be reduced, natural selection cannot uninstall the love-brain
- First computable red-line β and drift-to-function ratio δ provide a dynamic threshold theory for extreme sexual selection

## Next Steps
- Multi-modal signals (color + song) raise search dimensionality; test whether purification difficulty increases exponentially
- Experimental evolution in mice or fruit flies with fluorescent Q labels; measure whether lowering C_s shifts the predicted red line
