# 健忘鸟：记忆长度与邻居数量对群体协调的影响

## Hook
欧洲椋鸟可在 0.15 s 内完成数千只同步转弯（视频 https://www.youtube.com/watch?v=_p8SKdY7V8Q，0:25 处），单只短时视觉记忆仅约 3–5 帧。记忆如此短促，群体如何保持协调？我们利用“健忘鸟”模型系统扫描记忆长度 m 与邻居数量 K，重点监测掉队频率、个体角色分化、路线碎片化指数和转向响应时间，量化“健忘”对集群行为的综合效应。

## 模型与方法
- 个体运动：N 只自推进粒子，速度恒为 v₀=1 BL/s，方向单位向量 u_i；时间步长 Δt=0.04 s  
- 邻居选择：Euclidean 距离最近的 K 个个体  
- FIFO 记忆：个体维护长度 m 的队列 Q_i，存储邻居方向；超长者弹出队首  
- 方差惩罚：计算队列方向散布 σ²=1−|⟨exp(iθ_j)⟩|；若 σ²&gt;σ_c=0.26，随机采纳 Q_i 中一条方向，否则取平均方向并加高斯噪声 η=0.1 rad  

观测变量：
- 掉队频率 P_out：每 50 帧统计一次，距群体质心 &gt;5 BL 的个体比例平均值  
- 个体角色分化 I_i：记录每次转向扰动后 Δθ_j(t+1) 对 θ_i(t) 的偏导，归一化得影响度，计算分布峰度 κ  
- 路线碎片化指数 F=|ΔR|/ΣL_i，ΔR 为质心位移，ΣL_i 为总轨迹长  
- 转向响应时间 τ：中心 5 % 个体瞬时 90° 偏转，至 95 % 个体完成 50 % 偏转所需时间  

参数扫描：m∈[1,15]，K∈[1,15]，N=500，ρ=2 BL⁻²；每组 30 次重复，报告均值 ± 标准误

## 预期发现
- 掉队频率 P_out 随 m 减小而升高，预计 m≤3 时 P_out&gt;15 %，m≥7 后趋平  
- 角色分化峰度 κ 在 m 中等（4–6）时最大，预示“领航-跟随”结构最清晰；m 过小则方向随机，κ 下降  
- 路线碎片化指数 F 与 τ 呈正相关，二者均在 m≈4 出现拐点，验证“记忆门槛”假说  
- 综合四维响应面，可定位最佳协调区（m≥6, K≥5）与高风险散群区（m≤3, K≤3）

## 讨论
- 异质记忆：引入 20 % 幼鸟（m=1）观测 P_out 与 κ 变化，评估幼鸟是否成为掉队源  
- 三维视野锥：加入水平 240°、垂直 120° 限制，检验密林条件下临界 m 是否上移  
- 城市疏散：将方向替换为出口选择向量，同样四指标可测短视频式信息更新对人群逃生效率的影响


# Forgetful Birds: How Memory Length and Neighbor Number Shape Collective Coordination

## Hook
European starlings execute thousand-bird turns in 0.15 s (video: https://www.youtube.com/watch?v=_p8SKdY7V8Q, 0:25), yet single-bird visual memory lasts only 3–5 frames. How is such rapid coordination possible with such short memory? We probe this with "forgetful birds"—agents whose memory is a FIFO queue of length m—while tracking four key metrics: straying frequency, individual role differentiation, route fragmentation, and turn-response time.

## Model & Methods
- Self-propelled particles in 3-D, constant speed v₀ = 1 BL s⁻¹, time step Δt = 0.04 s  
- K-nearest-neighbor interaction (Euclidean distance)  
- FIFO memory: each bird keeps the latest m headings from its neighbors; older entries are discarded  
- Variance penalty: compute spread σ² = 1 − |⟨exp(i θⱼ)⟩|. If σ² &gt; σ_c = 0.26 rad², the bird randomly picks one stored heading; otherwise it adopts the mean heading plus Gaussian noise η = 0.1 rad  

Observables
- Straying frequency P_out: fraction of birds &gt; 5 BL from the flock centroid, averaged every 50 frames  
- Individual influence κ: perturb Δθ = 90° on 5 % of birds, compute ∂θⱼ(t+1)/∂θᵢ(t), normalize to obtain influence Iᵢ; report kurtosis κ of the I-distribution  
- Route fragmentation F = |ΔR| / Σ Lᵢ (ΔR: flock displacement; Σ Lᵢ: total path length)  
- Turn-response time τ: time for 95 % of birds to reach 50 % of the imposed 90° turn  

Parameter sweep: m ∈ [1, 15], K ∈ [1, 15], N = 500, ρ = 2 BL⁻²; 30 runs per grid point, mean ± s.e.m. reported.

## Expected Findings
- P_out increases sharply for m ≤ 3 and saturates for m ≥ 7  
- Kurtosis κ peaks at intermediate m (4–6), indicating strongest leader–follower structure  
- F and τ are positively correlated and both exhibit a knee near m ≈ 4, supporting a memory-limited coordination threshold  
- Combined 4-D response surface will map "safe coordination" (m ≥ 6, K ≥ 5) versus "fragmentation risk" (m ≤ 3, K ≤ 3) regions

## Discussion
- Heterogeneous memory: introduce 20 % juvenile birds (m = 1) and quantify their impact on P_out and κ  
- 3-D visual cone: restrict horizontal FOV to 240° and vertical to 120° to test whether dense woodland elevates the critical m  
- Urban evacuation: reinterpret heading as exit-choice vector; the same four metrics can quantify how short-memory, social-media-like updates impair human evacuation efficiency
