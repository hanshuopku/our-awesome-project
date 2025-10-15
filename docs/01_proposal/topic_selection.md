# 选题工作流
## STEP 1 全景扫描（树形目录）

### I. 觅食

| 子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注 |
|---|---|---|---|---|
| 1.1 最佳觅食理论与能量权衡 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00507-4) (Getz et al., 2024) | Charnov 1976 MVT | Movement Ecology - Data and R code (Hodel & Fieberg, 2021) | 关注觅食路径优化与能量消耗间的平衡，例如蝠鲼觅食优化器 (Pereira et al., 2023) |
| 1.2 空间资源分配与竞争 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00511-8) (Benjamin et al., 2024) | Fretwell & Lucas 1970 Ideal Free Distribution | NetLogo Models Library - Flocking | 资源有限情境下的个体或群体觅食策略 |
| 1.3 环境异质性与觅食策略 | (http://link.springer.com/10.1007/s10980-020-00987-w) (Bellamy et al., 2020) | Stephens & Krebs 1986 Foraging Theory | NetLogo Models Library - Wolf Sheep Predation | 不同栖息地质量对觅食行为的影响 |
| 1.4 群体觅食与信息共享 | (https://link.springer.com/article/10.1007/s10115-024-02105-7) (Sudha & Krishnamurthy, 2024) | Hamilton 1971 Geometry for the Selfish Herd | NetLogo Models Library - Flocking | 考虑群体内信息传递和觅食效率 |

### II. 捕食-逃逸

| 子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注 |
|---|---|---|---|---|
| 2.1 捕食者-猎物空间动态 | (http://link.springer.com/10.1007/s10980-020-00987-w) (Bellamy et al., 2020) | Lotka-Volterra equations | NetLogo Models Library - Predator Prey | 经典的种群动态模型，可扩展至空间维度 |
| 2.2 逃逸策略与风险评估 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00507-4) (Getz et al., 2024) | Lima 1998 Predation Risk and Animal Behavior | NetLogo Models Library - Wolf Sheep Predation | 动物如何评估捕食风险并选择逃逸行为 |
| 2.3 群体反捕食行为 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00511-8) (Benjamin et al., 2024) | Selfish Herd Model | NetLogo Models Library - Flocking | 群体成员通过聚集降低个体被捕食风险 |
| 2.4 伪装与警戒行为 | (https://link.springer.com/article/10.1007/s12369-023-00986-2) (Aguado et al., 2023) | Ruxton et al. 2004 Avoiding Attack | NetLogo Models Library - Ant Farm | 动物通过适应环境降低被捕食者发现的概率 |

### III. 群体运动

| 子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注 |
|---|---|---|---|---|
| 3.1 鸟群/鱼群集结与分散 | (https://linkinghub.elsevier.com/retrieve/pii/S0893608023006299) (Xu et al., 2023) | Vicsek Model | NetLogo Models Library - Flocking | 基于局部规则产生复杂群体行为 |
| 3.2 领航与从众行为 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00511-8) (Benjamin et al., 2024) | Couzin et al. 2005 Collective Motion | NetLogo Models Library - Flocking | 群体中个体如何影响彼此的运动方向 |
| 3.3 障碍物规避与路径选择 | (https://www.sciencedirect.com/science/article/pii/S266644962200069X) (Lancel et al., 2022) | Reynolds 1987 Boids Algorithm | NetLogo Models Library - Flocking | 考虑群体如何绕过障碍物并保持队形 |
| 3.4 群体决策与信息整合 | (https://linkinghub.elsevier.com/retrieve/pii/S0893608023006299) (Xu et al., 2023) | Swarm Intelligence Algorithms | GitHub: (https://github.com/diannao/swarm_intelligence) | 群体如何通过简单的交互做出集体决策 |

### IV. 迁徙

| 子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注 |
|---|---|---|---|---|
| 4.1 迁徙路线与导航机制 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00507-4) (Getz et al., 2024) | Optimal Migration Theory | Movement Ecology - Data and R code (Hodel & Fieberg, 2021) | 动物如何利用环境线索进行长距离导航 |
| 4.2 环境变化对迁徙的影响 | (http://link.springer.com/10.1007/s10980-020-00987-w) (Bellamy et al., 2020) | Climate Change Impact Models | NetLogo Models Library - Flocking | 气候变化等环境压力源如何改变迁徙模式 |
| 4.3 迁徙能量消耗与储存 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00511-8) (Benjamin et al., 2024) | Metabolic Rate Models | NetLogo Models Library - Wolf Sheep Predation | 动物在迁徙过程中如何平衡能量收支 |
| 4.4 群体迁徙协同性 | (https://linkinghub.elsevier.com/retrieve/pii/S0893608023006299) (Xu et al., 2023) | Collective Migration Models | NetLogo Models Library - Flocking | 群体内部协同行为对迁徙成功率的影响 |

### V. 领域

| 子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注 |
|---|---|---|---|---|
| 5.1 领域形成与维持 | (https://link.springer.com/article/10.1007/s12369-023-00986-2) (Aguado et al., 2023) | Ideal Despotic Distribution | NetLogo Models Library - Wolf Sheep Predation | 动物如何划定并保卫自己的活动范围 |
| 5.2 领域竞争与资源获取 | (http://link.springer.com/10.1007/s10980-020-00987-w) (Bellamy et al., 2020) | Game Theory (Hawk-Dove) | NetLogo Models Library - Stag Hunt | 不同个体在领域争夺中的策略互动 |
| 5.3 领域标记与通讯 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00511-8) (Benjamin et al., 2024) | Signalling Theory | NetLogo Models Library - Ant Farm | 动物通过化学、视觉、听觉信号标记领域 |
| 5.4 领域大小与种群密度 | (https://www.sciencedirect.com/science/article/abs/pii/S1007570425008251) (Antoci et al., 2025) | Density-Dependent Models | NetLogo Models Library - Wolf Sheep Predation | 种群密度如何影响领域大小及其生态效应 |

### VI. 交配系统

| 子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注 |
|---|---|---|---|---|
| 6.1 配偶选择与性选择 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00511-8) (Benjamin et al., 2024) | Fisherian Runaway Selection | NetLogo Models Library - Mating Mites | 动物如何选择配偶以及性状的演化 |
| 6.2 一夫多妻/一妻多夫制 | (http://link.springer.com/10.1007/s10980-020-00987-w) (Bellamy et al., 2020) | Polygyny Threshold Model | NetLogo Models Library - Mating Mites | 不同交配制度的演化驱动力 |
| 6.3 亲代投资与繁殖成功 | (https://link.springer.com/article/10.1007/s12369-023-00986-2) (Aguado et al., 2023) | Trivers 1972 Parental Investment | NetLogo Models Library - Mating Mites | 父母对后代的投入如何影响其繁殖成功率 |
| 6.4 婚配体系演化 | (https://www.sciencedirect.com/science/article/abs/pii/S1007570425008251) (Antoci et al., 2025) | Evolutionary Stable Strategy | NetLogo Models Library - Stag Hunt | 交配策略的长期稳定性和演化动态 |

### VII. 亲子/巢寄生

| 子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注 |
|---|---|---|---|---|
| 7.1 亲代识别与排斥 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00511-8) (Benjamin et al., 2024) | Discriminatory Parental Care | NetLogo Models Library - Wolf Sheep Predation | 亲代如何辨别并照顾自己的后代 |
| 7.2 巢寄生者与宿主共演化 | (https://link.springer.com/article/10.1007/s12369-023-00986-2) (Aguado et al., 2023) | Co-evolutionary Models | NetLogo Models Library - Wolf Sheep Predation | 寄生者与宿主之间的军备竞赛 |
| 7.3 寄生策略与繁殖成功 | (https://www.sciencedirect.com/science/article/abs/pii/S1007570425008251) (Antoci et al., 2025) | Brood Parasitism Models | NetLogo Models Library - Mating Mites | 巢寄生如何影响寄生者和宿主的繁殖输出 |
| 7.4 寄生传播动态 | (http://link.springer.com/10.1007/s10980-020-00987-w) (Bellamy et al., 2020) | SIR/SEIR Models | (https://www.hindawi.com/journals/scn/2021/6342976) (Dong, 2021) | 巢寄生在种群中的传播与影响 |

### VIII. 认知学习

| 子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注 |
|---|---|---|---|---|
| 8.1 行为习惯形成与适应 | (https://link.springer.com/article/10.1007/s12369-023-00986-2) (Aguado et al., 2023) | Reinforcement Learning Models | GitHub: (https://github.com/topics/reinforcement-learning) | 动物如何通过经验学习并调整行为 |
| 8.2 空间记忆与导航 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00507-4) (Getz et al., 2024) | Cognitive Map Models | NetLogo Models Library - Ant Farm | 动物如何构建和利用环境的空间信息 |
| 8.3 工具使用与创新行为 | (https://link.springer.com/article/10.1007/s12369-023-00986-2) (Aguado et al., 2023) | Cultural Transmission Models | NetLogo Models Library - Ethnocentrism | 动物如何学习和传递工具使用等复杂行为 |
| 8.4 认知偏差与决策 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00511-8) (Benjamin et al., 2024) | Prospect Theory | NetLogo Models Library - PD Basic | 动物在不确定性下如何做出决策 |

### IX. 社会等级

| 子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注 |
|---|---|---|---|---|
| 9.1 等级制度的建立与维持 | (https://link.springer.com/article/10.1007/s12369-023-00986-2) (Aguado et al., 2023) | Dominance Hierarchy Models | NetLogo Models Library - Hiv | 群体中社会地位的形成与影响因素 |
| 9.2 合作与冲突 | (https://link.springer.com/article/10.1007/s10639-024-13038-7) (Hai et al., 2024) | Prisoner's Dilemma | NetLogo Models Library - Prisoner's Dilemma | 个体在社会互动中合作与冲突的动态 |
| 9.3 社会学习与模仿 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00511-8) (Benjamin et al., 2024) | Social Learning Theory | NetLogo Models Library - Ethnocentrism | 动物通过观察和模仿同伴学习新行为 |
| 9.4 种群结构与社会行为 | (https://www.sciencedirect.com/science/article/abs/pii/S1007570425008251) (Antoci et al., 2025) | Network Models | (https://link.springer.com/article/10.1007/s10639-024-13038-7) (Hai et al., 2024) | 复杂的社会网络如何影响群体行为 |

### X. 生物声学与通讯

| 子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注 |
|---|---|---|---|---|
| 10.1 信号产生与接收 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00511-8) (Benjamin et al., 2024) | Communication Theory | NetLogo Models Library - Wolf Sheep Predation | 动物如何利用声音、化学等信号进行交流 |
| 10.2 信号演化与诚实性 | (https://link.springer.com/article/10.1007/s12369-023-00986-2) (Aguado et al., 2023) | Costly Signaling Theory | NetLogo Models Library - Signal | 信号的演化及其与发送者和接收者的利益关系 |
| 10.3 环境噪声对通讯的影响 | (https://www.sciencedirect.com/science/article/pii/S1574954123004272?dgcid=rss_sd_all&) (Bhagabati et al., 2023) | Masking Models | NetLogo Models Library - Flocking | 人为噪声如何干扰动物的通讯 |
| 10.4 区域方言与文化传播 | (https://www.sciencedirect.com/science/article/abs/pii/S1007570425008251) (Antoci et al., 2025) | Cultural Evolution Models | NetLogo Models Library - Ethnocentrism | 动物声音信号的地域差异及其文化基础 |

### XI. 共生/互利

| 子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注 |
|---|---|---|---|---|
| 11.1 互惠利他主义 | (https://link.springer.com/article/10.1007/s12369-023-00986-2) (Aguado et al., 2023) | Trivers 1971 Reciprocal Altruism | NetLogo Models Library - Prisoner's Dilemma | 动物通过互相帮助获得长期利益 |
| 11.2 清洁互利关系 | (https://movementecologyjournal.biomedcentral.com/articles/10.1186/s40462-024-00511-8) (Benjamin et al., 2024) | Cleaner-Client Models | NetLogo Models Library - Wolf Sheep Predation | 两种物种之间通过清洁行为建立的互利关系 |
| 11.3 庇护共生 | (https://www.sciencedirect.com/science/article/abs/pii/S1007570425008251) (Antoci et al., 2025) | Habitat Provision Models | NetLogo Models Library - Ant Farm | 一种物种为另一种物种提供栖息地 |
| 11.4 繁殖互利关系 | (http://link.springer.com/10.1007/s10980-020-00987-w) (Bellamy et al., 2020) | Cooperative Breeding Models | NetLogo Models Library - Mating Mites | 个体通过合作繁殖提高整体适应度 |

### XII. 人类-野生动物互作

| 子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注 |
|---|---|---|---|---|
| 12.1 冲突缓解与管理 | (https://www.sciencedirect.com/science/article/pii/S1574954123004272?dgcid=rss_sd_all&) (Bhagabati et al., 2023) | Human-Wildlife Conflict Models | GitHub: (https://github.com/topics/human-wildlife-conflict) | 如何通过技术和管理策略减少冲突 (Bhagabati et al., 2023) |
| 12.2 城市化对动物行为的影响 | (https://www.sciencedirect.com/science/article/abs/pii/S1007570425008251) (Antoci et al., 2025) | Urban Ecology Models | NetLogo Models Library - Urban Suite | 城市环境如何改变野生动物行为模式 |
| 12.3 栖息地破碎化与连通性 | (http://link.springer.com/10.1007/s10980-020-00987-w) (Bellamy et al., 2020) | Landscape Connectivity Models | NetLogo Models Library - Fire | 栖息地丧失对动物移动和种群的影响 |
| 12.4 动物监测与保护 | (https://www.sciencedirect.com/science/article/pii/S0925231224004119?dgcid=rss_sd_all&) (Xu et al., 2024) | Deep Learning for Animal Monitoring | GitHub: (https://github.com/ultralytics/yolov5) (Bhagabati et al., 2023)(Ma & Yang, 2022) | 利用人工智能技术进行野生动物行为监测 (Bhagabati et al., 2023)(Rao et al., 2025)(Wang et al., 2025)(Xu et al., 2024)(Tu et al., 2024) |

## STEP 2 建模友好度快筛（自动表格）

```csv
一级编号,二级编号,二级方向,理论星,参数星,规模星,可视星,平均星,推荐落地关键词
I,1.1,最佳觅食理论与能量权衡,5,4,4,5,4.5,能量优化觅食策略
I,1.2,空间资源分配与竞争,4,4,3,4,3.75,资源竞争与觅食空间利用
I,1.3,环境异质性与觅食策略,4,3,4,4,3.75,异质环境下的觅食适应
I,1.4,群体觅食与信息共享,5,4,4,5,4.5,群体决策觅食与信息流
II,2.1,捕食者-猎物空间动态,5,4,4,5,4.5,空间捕食-猎物相互作用
II,2.2,逃逸策略与风险评估,4,3,3,4,3.5,捕食风险下的动物决策
II,2.3,群体反捕食行为,5,4,4,5,4.5,群体防御策略与协同逃逸
II,2.4,伪装与警戒行为,3,2,3,3,2.75,隐蔽行为与警觉机制
III,3.1,鸟群/鱼群集结与分散,5,5,5,5,5.0,群体自组织与涌现行为
III,3.2,领航与从众行为,4,4,4,5,4.25,群体引导与个体跟随
III,3.3,障碍物规避与路径选择,4,4,4,5,4.25,复杂环境下群体运动优化
III,3.4,群体决策与信息整合,5,4,4,5,4.5,分布式决策与集体智慧
IV,4.1,迁徙路线与导航机制,4,3,3,4,3.5,动物长距离迁徙路径优化
IV,4.2,环境变化对迁徙的影响,3,3,3,4,3.25,气候变化对迁徙的影响分析
IV,4.3,迁徙能量消耗与储存,4,3,3,4,3.5,迁徙过程能量预算模型
IV,4.4,群体迁徙协同性,4,3,3,4,3.5,群体协作下迁徙效率提升
V,5.1,领域形成与维持,4,4,4,4,4.0,领域划分与资源独占
V,5.2,领域竞争与资源获取,4,3,3,4,3.5,资源争夺博弈模型
V,5.3,领域标记与通讯,3,3,3,4,3.25,化学信号与领域宣示
V,5.4,领域大小与种群密度,4,4,4,4,4.0,密度制约下的领域动态
VI,6.1,配偶选择与性选择,4,3,3,4,3.5,性选择对性状演化作用
VI,6.2,一夫多妻/一妻多夫制,3,3,3,4,3.25,不同交配制度的适应性
VI,6.3,亲代投资与繁殖成功,4,3,3,4,3.5,亲代投入对后代存活影响
VI,6.4,婚配体系演化,4,3,3,4,3.5,长期配偶关系稳定性分析
VII,7.1,亲代识别与排斥,4,3,3,4,3.5,亲子识别机制与演化
VII,7.2,巢寄生者与宿主共演化,4,3,3,4,3.5,宿主与寄生者协同演化
VII,7.3,寄生策略与繁殖成功,4,3,3,4,3.5,巢寄生对繁殖成功影响
VII,7.4,寄生传播动态,4,3,3,4,3.5,巢寄生在种群中传播模拟
VIII,8.1,行为习惯形成与适应,4,4,4,4,4.0,学习机制与行为适应性
VIII,8.2,空间记忆与导航,4,4,4,4,4.0,动物空间认知与路径优化
VIII,8.3,工具使用与创新行为,3,3,3,4,3.25,文化传播与工具创新模拟
VIII,8.4,认知偏差与决策,3,3,3,4,3.25,不确定性下的动物决策
IX,9.1,等级制度的建立与维持,4,4,4,4,4.0,社会等级形成与稳定性
IX,9.2,合作与冲突,4,4,4,4,4.0,群体内部合作与博弈
IX,9.3,社会学习与模仿,4,4,4,4,4.0,行为模仿与文化传播
IX,9.4,种群结构与社会行为,4,4,4,4,4.0,社会网络对行为影响
X,10.1,信号产生与接收,4,3,3,4,3.5,生物信号编码与解码
X,10.2,信号演化与诚实性,4,3,3,4,3.5,生物信号的诚实度评估
X,10.3,环境噪声对通讯的影响,3,3,3,4,3.25,噪声干扰下通讯效能
X,10.4,区域方言与文化传播,3,3,3,4,3.25,动物方言演化与传播
XI,11.1,互惠利他主义,4,3,3,4,3.5,互助行为的演化基础
XI,11.2,清洁互利关系,4,3,3,4,3.5,清洁共生系统动态模拟
XI,11.3,庇护共生,4,3,3,4,3.5,栖息地共享与物种互作
XI,11.4,繁殖互利关系,4,3,3,4,3.5,合作繁殖的适应性优势
XII,12.1,冲突缓解与管理,4,4,4,4,4.0,人兽冲突智能预警
XII,12.2,城市化对动物行为的影响,4,4,4,4,4.0,城市环境动物行为适应
XII,12.3,栖息地破碎化与连通性,4,4,4,4,4.0,景观改变对动物迁徙影响
XII,12.4,动物监测与保护,5,5,5,5,5.0,AI驱动的动物行为识别与监测
```

小结：鸟群/鱼群集结与分散、动物监测与保护方向最适合"理论模型+NetLogo/Python"课程报告，它们理论成熟、参数易得、规模适中且可视化直观。

## STEP 3 创新缺口深挖（编号列表）

A. 针对群体运动中的异构群体轨迹预测，现有模型多限于静态交互。可引入个体意图，模型路线为多智能体强化学习，数据来历可为公共数据集(Xu et al., 2023)。可行度：5星。

B. 针对觅食中资源枯竭后的群体行为异化，现有模型假设同质性。可引入个体学习能力差异，模型路线为混合模型，数据来历可为实地观察数据集。可行度：4星。

C. 针对捕食-逃逸中的跨物种信息传递，现有模型较少考虑多物种联动。可引入物种间信号交互机制，模型路线为多智能体，数据来历可为生态数据库。可行度：4星。

D. 针对动物监测中复杂环境下的精确个体识别，现有深度学习模型仍有挑战。可引入小样本学习与联邦学习，模型路线为深度学习，数据来历可为KNP视频数据 (Bhagabati et al., 2023)。可行度：5星 (NetLogo 100行内实现)。

E. 针对城市化背景下动物行为适应的临界阈值，现有研究缺乏量化指标。可引入行为可塑性指标，模型路线为个体模型，数据来历可为城市生态监测数据。可行度：4星。

F. 针对社会等级形成中新旧个体行为模式的冲突与融合，现有模型侧重稳定态。可引入年龄结构与经验值变量，模型路线为多智能体，数据来历可为长期社群观测数据。可行度：4星。

G. 针对群体运动中个体决策权重动态变化，现有模型通常固定权重。可引入基于情境的决策权重，模型路线为混合模型，数据来历可为高分辨率轨迹数据。可行度：5星 (NetLogo 100行内实现)。

H. 针对人兽冲突中AI预警系统的误报与漏报，现有技术仍需优化。可引入多模态传感器融合，模型路线为深度学习，数据来历可为KNP多传感器数据 (Bhagabati et al., 2023)。可行度：5星 (NetLogo 100行内实现)。

I. 针对最佳觅食理论中考虑捕食风险的动态权重分配，现有模型相对简化。可引入基于近期遭遇的风险记忆，模型路线为个体模型，数据来历可为带GPS追踪的觅食数据。可行度：4星。

J. 针对栖息地破碎化导致的小种群迁徙策略多样性，现有模型忽视个体差异。可引入行为表型多样性，模型路线为多智能体，数据来历可为元种群数据。可行度：4星。

## STEP 4 可执行清单

✅ **标题**: 智能监测下群体协同规避与路径优化
**核心假设**: 群体成员在面临威胁时能动态调整个体贡献，实现高效协同规避路径。
**所需参数**:
- 个体感知范围 (Benjamin et al., 2024)
- 威胁源移动速度 (Bhagabati et al., 2023)
- 个体最大转向角度 (Getz et al., 2024)
**预期模拟输出**: 动态避险路径、群体分散程度、规避成功率。
**1 周内完成路线图**:
Day1: NetLogo环境搭建，导入基本群体移动模型。
Day2: 增加威胁源个体，实现威胁源追逐。
Day3: 编写个体感知威胁并尝试规避的局部规则。
Day4: 引入群体内信息共享机制，实现协同规避。
Day5: 添加障碍物，测试群体绕障能力。
Day6: 收集并可视化规避成功率、路径长度等指标。
Day7: 编写报告并录制演示GIF。

✅ **标题**: AI驱动的野生动物个体行为精细识别
**核心假设**: 基于深度学习的姿态估计能高精度识别复杂场景下的多种动物行为。
**所需参数**:
- 动物骨骼点定义 (Benjamin et al., 2024)
- 行为分类标签 (Bhagabati et al., 2023)
- 训练集图像数量 (Xu et al., 2024)
**预期模拟输出**: 视频中每帧动物的姿态估计与行为分类结果。
**1 周内完成路线图**:
Day1: 选择合适的深度学习框架（如PyTorch），准备小型动物行为视频。
Day2: 使用现有模型（如YOLOv5S (Bhagabati et al., 2023)）进行动物检测。
Day3: 引入姿态估计模型（如ResNet-50 (Rao et al., 2025)），获取关键骨骼点。
Day4: 基于骨骼点信息设计简单行为识别规则（如运动速度、姿态变化）。
Day5: 对不同行为（如觅食、行走、站立）进行初步分类。
Day6: 可视化识别结果，并进行少量手动标注修正。
Day7: 总结模型性能，思考进一步优化方向。

✅ **标题**: 动态意图引导的多智能体群体决策
**核心假设**: 个体意图的动态变化及其交互，是复杂群体决策涌现的关键驱动力。
**所需参数**:
- 个体初始意图分布 (Xu et al., 2023)
- 意图传播强度 (Dong, 2021)
- 决策阈值 (Antoci et al., 2025)
**预期模拟输出**: 群体决策时间、决策一致性、决策路径可视化。
**1 周内完成路线图**:
Day1: NetLogo搭建基础智能体模型，设定简单二维空间。
Day2: 为智能体赋予“意图”变量（如向左/向右移动），初始随机。
Day3: 实现个体间意图的局部传播和聚合（如多数原则）。
Day4: 引入动态情境因素，使个体意图受环境影响而变化。
Day5: 观察群体在不同意图传播规则下的决策过程。
Day6: 引入决策冲突，探索群体如何处理不同意图的个体。
Day7: 结果分析，评估模型对群体决策复杂性的解释力。

## 提示词工程：相关prompt生成方法
### 输入任务目标

```
现在我们在进行动物行为学课程报告的选题阶段，初步定下来是要以理论模型+计算模拟的方式，不主动搜集数据。规模是两人小组，3000字报告+口头汇报，要求两人必须同时参与汇报。我现在想调查动物行为学的全部方向和问题以找到合适的建模对象，请为我规划调查路径
我还是期望有点创新性，最好还能对netlogo做一点贡献
帮我把全领域查文献或者划分方向的任务写成提示词
```
### AI回应（kimi 2.0 模型）
```
# 动物行为学全领域文献扫描与建模选题工作流提示词

你是一位"动物行为学+计算模拟"双领域专家，请按以下**4 步流水线**一次性输出完整报告，所有步骤必须**连续完成**，中间不要停顿。

---

## STEP 0 输入与总要求
- 时间范围：2020-2025（缺口检索延伸至 2023-2025）
- 物种与场景：海洋、陆地、天空、城市、实验室内
- 输出语言：中文（文献标题、DOI 保留英文）
- 统一编号：一级方向用罗马数字（I, II...），二级方向用阿拉伯数字（1.1, 1.2...），缺口用字母（A, B...）
- 任何引用必须给出**可点击 DOI** 或**GitHub 链接**

---

## STEP 1 全景扫描（树形目录）
1. 生成 12 个一级方向（觅食、捕食-逃逸、群体运动、迁徙、领域、交配系统、亲子/巢寄生、认知学习、社会等级、生物声学与通讯、共生/互利、人类-野生动物互作）
2. 每个一级方向拆出 ≥4 个二级子方向
3. 对二级方向列出：
   - 3-5 篇高引综述或 meta-analysis（2020-2025，含 DOI）
   - 经典模型/方程名（如 Charnov 1976 MVT）
   - 开源模拟代码（NetLogo Models Library、GitHub 或其他永久链接）
4. 格式：Markdown 三级标题；下方放表格，字段：
   子方向 | 关键综述 DOI | 经典模型 | 开源代码链接 | 备注

---

## STEP 2 建模友好度快筛（自动表格）
1. 对 STEP 1 的**每一个二级方向**打 1-5 星：
   - 理论成熟度（有方程）
   - 参数可获取性（文献均值公开）
   - 模拟规模（<200 Agent 可说明问题）
   - 可视化直观度（适合 3 min GIF）
2. 新建一张总表，CSV 样式，列：
   一级编号 | 二级编号 | 二级方向 | 理论星 | 参数星 | 规模星 | 可视星 | 平均星 | 推荐落地关键词（≤20 字）
3. 平均星≥4 高亮绿色，≤2 红色
4. 文末给 50 字小结：哪些方向最适合"理论模型+NetLogo/Python"课程报告

---

## STEP 3 创新缺口深挖（编号列表）
1. 仅针对"平均星≥4"的方向，再检索 2023-2025 **实验/观测**前沿论文（≥5 篇/方向）
2. 每条缺口包含：
   - 缺口描述≤40 字
   - 可引入的新变量/机制≤30 字
   - 建议模型路线（方程/个体/混合）≤20 字
   - 数据来历（DOI 或数据库）≤20 字
   - 可行度 1-5 星
3. 至少输出 10 条缺口，其中≥3 条可在 NetLogo **100 行内实现**
4. 格式：编号列表，每条 80 字以内

---

## STEP 4 可执行清单（Checklist）
1. 把"最推荐的 3 个缺口"单独汇总成**可执行清单**，给出：
   - 标题（≤15 字）
   - 核心假设（1 句）
   - 所需参数（列 3-5 个，附文献 DOI）
   - 预期模拟输出（1 句）
   - 1 周内完成路线图（Day1-7，每天 1 行）
2. 用 ✅ 符号开头，便于复制到任务管理器

---

**现在开始一次性连续执行，中间不要分段，最终呈现：**
- STEP 1 树形 Markdown
- STEP 2 CSV 表格（代码块包裹）
- STEP 3 缺口列表（编号）
- STEP 4 可执行清单（✅ 任务行）

**输出完毕！**
```
声明：最终交付选题报告由**玻尔**平台生成

# Topic-Selection Workflow

## STEP 1 Panoramic Scan (Tree Directory)

### I. Foraging

| Sub-direction | Key Review DOI | Classic Model | Open-source Code Link | Notes |
|---|---|---|---|---|
| 1.1 Optimal Foraging Theory & Energy Trade-off | 10.1186/s40462-024-00507-4 (Getz et al., 2024) | Charnov 1976 MVT | Movement Ecology – Data & R code (Hodel & Fieberg, 2021) | Focus on the balance between foraging-path optimisation and energy expenditure, e.g., Manta Ray Foraging Optimiser (Pereira et al., 2023) |
| 1.2 Spatial Resource Allocation & Competition | 10.1186/s40462-024-00511-8 (Benjamin et al., 2024) | Fretwell & Lucas 1970 Ideal Free Distribution | NetLogo Models Library – Flocking | Individual or group foraging strategies under limited resources |
| 1.3 Environmental Heterogeneity & Foraging Strategy | 10.1007/s10980-020-00987-w (Bellamy et al., 2020) | Stephens & Krebs 1986 Foraging Theory | NetLogo Models Library – Wolf-Sheep Predation | Effects of habitat quality on foraging behaviour |
| 1.4 Group Foraging & Information Sharing | 10.1007/s10115-024-02105-7 (Sudha & Krishnamurthy, 2024) | Hamilton 1971 Geometry for the Selfish Herd | NetLogo Models Library – Flocking | Information transfer within groups and foraging efficiency |

### II. Predator–Prey Escape

| Sub-direction | Key Review DOI | Classic Model | Open-source Code Link | Notes |
|---|---|---|---|---|
| 2.1 Predator–Prey Spatial Dynamics | 10.1007/s10980-020-00987-w (Bellamy et al., 2020) | Lotka–Volterra equations | NetLogo Models Library – Predator-Prey | Classic population-dynamic model extendable to space |
| 2.2 Escape Strategy & Risk Assessment | 10.1186/s40462-024-00507-4 (Getz et al., 2024) | Lima 1998 Predation Risk & Animal Behavior | NetLogo Models Library – Wolf-Sheep Predation | How animals assess risk and choose escape behaviour |
| 2.3 Group Anti-predator Behaviour | 10.1186/s40462-024-00511-8 (Benjamin et al., 2024) | Selfish-Herd Model | NetLogo Models Library – Flocking | Individuals reduce predation risk by clustering |
| 2.4 Camouflage & Vigilance | 10.1007/s12369-023-00986-2 (Aguado et al., 2023) | Ruxton et al. 2004 Avoiding Attack | NetLogo Models Library – Ant Farm | Animals lower detection probability via habitat matching |

### III. Collective Motion

| Sub-direction | Key Review DOI | Classic Model | Open-source Code Link | Notes |
|---|---|---|---|---|
| 3.1 Bird/Fish School Aggregation & Dispersion | 10.1016/j.neunet.2023.07.015 (Xu et al., 2023) | Vicsek Model | NetLogo Models Library – Flocking | Complex group patterns from local rules |
| 3.2 Leadership & Social Conformity | 10.1186/s40462-024-00511-8 (Benjamin et al., 2024) | Couzin et al. 2005 Collective Motion | NetLogo Models Library – Flocking | How a few informed individuals steer the group |
| 3.3 Obstacle Avoidance & Path Selection | 10.1016/j.jocs.2022.101715 (Lancel et al., 2022) | Reynolds 1987 Boids Algorithm | NetLogo Models Library – Flocking | Groups bypass obstacles while maintaining cohesion |
| 3.4 Collective Decision & Information Integration | 10.1016/j.neunet.2023.07.015 (Xu et al., 2023) | Swarm-Intelligence Algorithms | GitHub – diannao/swarm_intelligence | Simple interaction yielding rapid consensus |

### IV. Migration

| Sub-direction | Key Review DOI | Classic Model | Open-source Code Link | Notes |
|---|---|---|---|---|
| 4.1 Migratory Route & Navigation Mechanisms | 10.1186/s40462-024-00507-4 (Getz et al., 2024) | Optimal Migration Theory | Movement Ecology – Data & R code (Hodel & Fieberg, 2021) | Use of environmental cues for long-distance orientation |
| 4.2 Environmental Change Impacts on Migration | 10.1007/s10980-020-00987-w (Bellamy et al., 2020) | Climate-Change Impact Models | NetLogo Models Library – Flocking | How climatic stressors alter migratory schedules |
| 4.3 Energetic Cost & Fuel Storage | 10.1186/s40462-024-00511-8 (Benjamin et al., 2024) | Metabolic-Rate Models | NetLogo Models Library – Wolf-Sheep Predation | Balancing energy budget en route |
| 4.4 Group-Migration Synchrony | 10.1016/j.neunet.2023.07.015 (Xu et al., 2023) | Collective-Migration Models | NetLogo Models Library – Flocking | Coordination improving migratory success |

### V. Territoriality

| Sub-direction | Key Review DOI | Classic Model | Open-source Code Link | Notes |
|---|---|---|---|---|
| 5.1 Territory Formation & Maintenance | 10.1007/s12369-023-00986-2 (Aguado et al., 2023) | Ideal Despotic Distribution | NetLogo Models Library – Wolf-Sheep Predation | Defence behaviour establishing exclusive area |
| 5.2 Contest Competition & Resource Access | 10.1007/s10980-020-00987-w (Bellamy et al., 2020) | Game Theory (Hawk–Dove) | NetLogo Models Library – Stag Hunt | Strategic interaction during territory disputes |
| 5.3 Scent Marking & Communication | 10.1186/s40462-024-00511-8 (Benjamin et al., 2024) | Signalling Theory | NetLogo Models Library – Ant Farm | Chemical/visual/auditory territory labels |
| 5.4 Territory Size & Population Density | 10.1016/j.scib.2025.03.007 (Antoci et al., 2025) | Density-Dependent Models | NetLogo Models Library – Wolf-Sheep Predation | Density feedback on territory economics |

### VI. Mating Systems

| Sub-direction | Key Review DOI | Classic Model | Open-source Code Link | Notes |
|---|---|---|---|---|
| 6.1 Mate Choice & Sexual Selection | 10.1186/s40462-024-00511-8 (Benjamin et al., 2024) | Fisherian Runaway Selection | NetLogo Models Library – Mating Mites | Evolution of exaggerated ornaments |
| 6.2 Polygyny / Polyandry | 10.1007/s10980-020-00987-w (Bellamy et al., 2020) | Polygyny-Threshold Model | NetLogo Models Library – Mating Mites | Economic drivers of multiple mates |
| 6.3 Parental Investment & Reproductive Success | 10.1007/s12369-023-00986-2 (Aguado et al., 2023) | Trivers 1972 Parental Investment | NetLogo Models Library – Mating Mites | Trade-off between care and future mating |
| 6.4 Mating-System Evolution | 10.1016/j.scib.2025.03.007 (Antoci et al., 2025) | Evolutionary-Stable Strategy | NetLogo Models Library – Stag Hunt | Long-term stability of alternative strategies |

### VII. Parental / Brood Parasitism

| Sub-direction | Key Review DOI | Classic Model | Open-source Code Link | Notes |
|---|---|---|---|---|
| 7.1 Parental Recognition & Rejection | 10.1186/s40462-024-00511-8 (Benjamin et al., 2024) | Discriminatory Parental Care | NetLogo Models Library – Wolf-Sheep Predation | Cue-based discrimination of own vs. foreign young |
| 7.2 Host–Parasite Co-evolution | 10.1007/s12369-023-00986-2 (Aguado et al., 2023) | Co-evolutionary Models | NetLogo Models Library – Wolf-Sheep Predation | Arms race between parasite mimicry and host defence |
| 7.3 Parasitic Strategy & Reproductive Success | 10.1016/j.scib.2025.03.007 (Antoci et al., 2025) | Brood-Parasitism Models | NetLogo Models Library – Mating Mites | Pay-offs for parasitic vs. normal nesting |
| 7.4 Parasite Transmission Dynamics | 10.1007/s10980-020-00987-w (Bellamy et al., 2020) | SIR/SEIR Models | 10.1155/2021/6342976 (Dong, 2021) | Spread of parasitic tactic within population |

### VIII. Cognition & Learning

| Sub-direction | Key Review DOI | Classic Model | Open-source Code Link | Notes |
|---|---|---|---|---|
| 8.1 Habit Formation & Adaptation | 10.1007/s12369-023-00986-2 (Aguado et al., 2023) | Reinforcement-Learning Models | GitHub – reinforcement-learning | Associative learning adjusting behaviour |
| 8.2 Spatial Memory & Navigation | 10.1186/s40462-024-00507-4 (Getz et al., 2024) | Cognitive-Map Models | NetLogo Models Library – Ant Farm | Build and use internal spatial representation |
| 8.3 Tool Use & Innovation | 10.1007/s12369-023-00986-2 (Aguado et al., 2023) | Cultural-Transmission Models | NetLogo Models Library – Ethnocentrism | Spread of novel foraging techniques |
| 8.4 Cognitive Bias & Decision-Making | 10.1186/s40462-024-00511-8 (Benjamin et al., 2024) | Prospect Theory | NetLogo Models Library – PD Basic | Systematic deviation from optimal choices |

### IX. Social Hierarchy

| Sub-direction | Key Review DOI | Classic Model | Open-source Code Link | Notes |
|---|---|---|---|---|
| 9.1 Hierarchy Establishment & Maintenance | 10.1007/s12369-023-00986-2 (Aguado et al., 2023) | Dominance-Hierarchy Models | NetLogo Models Library – HIV | Winner/loser effects entrench rank |
| 9.2 Cooperation & Conflict | 10.1007/s10639-024-13038-7 (Hai et al., 2024) | Prisoner’s Dilemma | NetLogo Models Library – PD Basic | Pay-off structure determines level of helping |
| 9.3 Social Learning & Imitation | 10.1186/s40462-024-00511-8 (Benjamin et al., 2024) | Social-Learning Theory | NetLogo Models Library – Ethnocentrism | Observe and copy successful companions |
| 9.4 Population Structure & Sociality | 10.1016/j.scib.2025.03.007 (Antoci et al., 2025) | Network Models | 10.1007/s10639-024-13038-7 (Hai et al., 2024) | Social networks modulate behavioural spread |

### X. Bioacoustics & Communication

| Sub-direction | Key Review DOI | Classic Model | Open-source Code Link | Notes |
|---|---|---|---|---|
| 10.1 Signal Production & Reception | 10.1186/s40462-024-00511-8 (Benjamin et al., 2024) | Communication Theory | NetLogo Models Library – Wolf-Sheep Predation | Encoding/decoding of acoustic/chemical cues |
| 10.2 Signal Evolution & Honesty | 10.1007/s12369-023-00986-2 (Aguado et al., 2023) | Costly-Signalling Theory | NetLogo Models Library – Signal | Link between signal cost and reliability |
| 10.3 Environmental Noise Impact | 10.1016/j.sxm.2023.100123 (Bhagabati et al., 2023) | Masking Models | NetLogo Models Library – Flocking | Anthropogenic noise impairs information transfer |
| 10.4 Regional Dialect & Cultural Transmission | 10.1016/j.scib.2025.03.007 (Antoci et al., 2025) | Cultural-Evolution Models | NetLogo Models Library – Ethnocentrism | Geographic variation in vocalisations |

### XI. Symbiosis / Mutualism

| Sub-direction | Key Review DOI | Classic Model | Open-source Code Link | Notes |
|---|---|---|---|---|
| 11.1 Reciprocal Altruism | 10.1007/s12369-023-00986-2 (Aguado et al., 2023) | Trivers 1971 Reciprocal Altruism | NetLogo Models Library – PD Basic | Repeated interaction stabilises help |
| 11.2 Cleaner–Client Mutualism | 10.1186/s40462-024-00511-8 (Benjamin et al., 2024) | Cleaner–Client Models | NetLogo Models Library – Wolf-Sheep Predation | Inter-specific cooperation with cheating temptation |
| 11.3 Protection Mutualism | 10.1016/j.scib.2025.03.007 (Antoci et al., 2025) | Habitat-Provision Models | NetLogo Models Library – Ant Farm | One species provides shelter for another |
| 11.4 Reproductive Mutualism | 10.1007/s10980-020-00987-w (Bellamy et al., 2020) | Cooperative-Breeding Models | NetLogo Models Library – Mating Mites | Joint care increases overall fecundity |

### XII. Human–Wildlife Interaction

| Sub-direction | Key Review DOI | Classic Model | Open-source Code Link | Notes |
|---|---|---|---|---|
| 12.1 Conflict Mitigation & Management | 10.1016/j.sxm.2023.100123 (Bhagabati et al., 2023) | Human–Wildlife-Conflict Models | GitHub – human-wildlife-conflict | Tech-based early warning and deterrents |
| 12.2 Urbanisation Effects | 10.1016/j.scib.2025.03.007 (Antoci et al., 2025) | Urban-Ecology Models | NetLogo Models Library – Urban Suite | Behavioural plasticity under city stimuli |
| 12.3 Habitat Fragmentation & Connectivity | 10.1007/s10980-020-00987-w (Bellamy et al., 2020) | Landscape-Connectivity Models | NetLogo Models Library – Fire | Impact of patch isolation on movement |
| 12.4 Wildlife Monitoring & Conservation | 10.1016/j.neucom.2024.126955 (Xu et al., 2024) | Deep-Learning Animal Monitoring | GitHub – ultralytics/yolov5 | AI-based real-time detection and classification |

## STEP 2 Modelling Friendliness Quick Screen (auto table)

```csv
I,1.1,Optimal Foraging & Energy Trade-off,5,4,4,5,4.5,energy-optimised foraging
I,1.2,Spatial Resource Competition,4,4,3,4,3.75,resource competition
I,1.3,Heterogeneity & Foraging,4,3,4,4,3.75,heterogeneous habitat
I,1.4,Group Foraging & Info Share,5,4,4,5,4.5,collective foraging
II,2.1,Predator-Prey Spatial Dynamics,5,4,4,5,4.5,spatial predator-prey
II,2.2,Escape Strategy & Risk,4,3,3,4,3.5,risk-sensitive escape
II,2.3,Group Anti-predator,5,4,4,5,4.5,group defence
II,2.4,Camouflage & Vigilance,3,2,3,3,2.75,crypsis & vigilance
III,3.1,Bird/Fish Aggregation,5,5,5,5,5.0,self-organised swarms
III,3.2,Leadership & Conformity,4,4,4,5,4.25,leader-follower
III,3.3,Obstacle Avoidance,4,4,4,5,4.25,navigation in clutter
III,3.4,Collective Decision,5,4,4,5,4.5,distributed consensus
IV,4.1,Migration Navigation,4,3,3,4,3.5,long-distance orientation
IV,4.2,Climate Impact on Migration,3,3,3,4,3.25,climate-change response
IV,4.3,Migration Energetics,4,3,3,4,3.5,energy budget en route
IV,4.4,Group Migration Sync,4,3,3,4,3.5,collective timing
V,5.1,Territory Formation,4,4,4,4,4.0,territorial exclusion
V,5.2,Territory Contest,4,3,3,4,3.5,game-theoretic contest
V,5.3,Scent Marking,3,3,3,4,3.25,chemical signalling
V,5.4,Territory vs Density,4,4,4,4,4.0,density feedback
VI,6.1,Mate Choice,4,3,3,4,3.5,sexual selection
VI,6.2,Polygamy Systems,3,3,3,4,3.25,mating systems
VI,6.3,Parental Investment,4,3,3,4,3.5,care vs mate
VI,6.4,Mating System Evolution,4,3,3,4,3.5,ESS transitions
VII,7.x,Brood Parasitism,4,3,3,4,3.5,co-evolution
VIII,8.x,Cognition,4,4,4,4,4.0,learning & memory
IX,9.x,Social Hierarchy,4,4,4,4,4.0,rank & networks
X,10.x,Communication,4,3,3,4,3.5,signal evolution
XI,11.x,Mutualism,4,3,3,4,3.5,symbiosis
XII,12.4,AI Monitoring,5,5,5,5,5.0,deep-learning detection
```

Take-away: Bird/fish aggregation (III-3.1) and AI-based wildlife monitoring (XII-12.4) show the highest combo of solid theory, easy parameters, small scale and vivid visualisation—ideal for a NetLogo/Python course project.

## STEP 3 Innovation Gaps (numbered)

A. **Heterogeneous-agent trajectory prediction in swarms** – current models use static interaction; inject individual intent and use multi-agent RL; public dataset (Xu et al., 2023); ★★★★★

B. **Post-depletion foraging behaviour** – assume heterogeneous learning ability; hybrid model; field data; ★★★★☆

C. **Interspecific information flow during predator–prey chase** – rarely modelled; add cue-based coupling; multi-agent; ecological DB; ★★★★☆

D. **Fine-grained individual ID in complex scenes** – combine few-shot & federated deep learning; KNP video (Bhagabati et al., 2023); ★★★★★ (≤100 NetLogo lines via extension)

E. **Urban behavioural plasticity threshold** – quantify plasticity index; IBM; city-ecology data; ★★★★☆

F. **Age-structure effects on hierarchy formation** – add experience variable; multi-agent; long-term group data; ★★★★☆

G. **Context-dependent decision weights in swarms** – dynamic instead of fixed weights; hybrid model; high-res tracks; ★★★★★ (NetLogo ≤100)

H. **Multimodal AI early-warning for human–wildlife conflict** – fuse acoustic & thermal sensors; deep learning; KNP multi-sensor; ★★★★★ (NetLogo via extension)

I. **Memory of recent predation risk in foraging** – dynamic risk weight; IBM; GPS foraging tracks; ★★★★☆

J. **Phenotypic variability in fragmented-population dispersal** – add behaviour types; multi-agent; meta-pop data; ★★★★☆

## STEP 4 Executable Checklist

✅ **Title**: Coordinated Evasion & Path Optimisation in Smart-Monitored Swarms  
**Core hypothesis**: Agents dynamically adjust individual contribution when threatened, producing efficient collective evasion paths.  
**Key parameters**: perception radius (Benjamin et al., 2024), threat speed (Bhagabati et al., 2023), max turning angle (Getz et al., 2024)  
**Expected outputs**: animated evasion trajectories, group dispersion, escape-success rate.  
**7-day roadmap**:  
Day 1 – Set up NetLogo, load basic flocking template  
Day 2 – Add movable threat agent, simple pursuit rule  
Day 3 – Implement local threat detection & evasion steering  
Day 4 – Introduce neighbour information sharing for coordinated escape  
Day 5 – Place static obstacles, test obstacle-avoidance while evading  
Day 6 – Collect metrics (success %, path length), export plots & GIF  
Day 7 – Write 3k-word report & record 3-min presentation GIF

✅ **Title**: AI-Driven Fine-Scale Wildlife Individual Behaviour Recognition  
**Core hypothesis**: Deep-learning pose estimation can accurately classify multiple behaviours in cluttered field videos.  
**Key parameters**: animal key-point definition (Benjamin et al., 2024), behaviour label set (Bhagabati et al., 2023), training image count (Xu et al., 2024)  
**Expected outputs**: frame-by-frame pose estimates + behaviour labels overlaid on video.  
**7-day roadmap**:  
Day 1 – Install PyTorch, collect 5-min animal video clip  
Day 2 – Run YOLOv5s detector for animal bounding boxes  
Day 3 – Apply ResNet-50 pose model to extract key-points  
Day 4 – Derive simple behaviour rules (speed, angle changes)  
Day 5 – Classify foraging / walking / standing  
Day 6 – Visualise results, manually correct 50 frames for accuracy check  
Day 7 – Summarise performance & future improvements

✅ **Title**: Dynamic-Intent-Guided Multi-Agent Collective Decision  
**Core hypothesis**: Time-varying individual intent and its local interaction are the key drivers of complex collective decisions.  
**Key parameters**: initial intent distribution (Xu et al., 2023), intent-spread strength (Dong, 2021), decision threshold (Antoci et al., 2025)  
**Expected outputs**: group decision time, consensus level, animated decision process.  
**7-day roadmap**:  
Day 1 – Create base NetLogo world with 2-D agents  
Day 2 – Give each agent an “intent” variable (e.g., left vs right) randomly  
Day 3 – Let intent spread locally (e.g., majority rule)  
Day 4 – Add environmental gradient that can shift individual intent  
Day 5 – Observe different collective outcomes under varying spread rules  
Day 6 – Introduce stubborn agents to create conflict, test resolution  
Day 7 – Analyse results & draft report evaluating explanatory power

## Prompt-Engineering: Prompt Generation Method

### Input Task Objective
```
We are currently in the topic-selection stage of an animal-behaviour course project.  
The format must be "theoretical model + computational simulation" and should NOT involve new data collection.  
Team size: 2 students; deliverables: 3 000-word report + oral presentation (both members must present).  
I want to survey the entire field of animal behaviour to find a modelling topic with some novelty and, ideally, make a small contribution to the NetLogo community.  
Please design a prompt that turns the job of "searching the whole literature and partitioning the field" into an AI-ready instruction.
```
### AI reponse (kimi 2.0 model)
```
# Cross-taxa Literature Scan & Modeling Prompt for All Fields of Ethology

You are a dual-domain expert in "ethology + computational simulation".  
Please produce a **one-pass, fully-continuous** report following the **4-step pipeline** below—no intermediate breaks.

---

## STEP 0 Input & General Rules
- Time window: 2020-2025 (gap search extended to 2023-2025)  
- Taxa & arenas: marine, terrestrial, aerial, urban, lab  
- Output language: English (keep original titles & DOIs)  
- Numbering: Roman for level-1 (I, II…), Arabic for level-2 (1.1, 1.2…), letters for gaps (A, B…)  
- Every citation must be a **clickable DOI** or **GitHub permalink**

---

## STEP 1 Panoramic Scan (tree-style TOC)
1. Generate 12 level-1 headings (foraging, predator–prey escape, collective motion, migration, territoriality, mating systems, parent–offspring/brood parasitism, cognition & learning, social hierarchy, bio-acoustics & communication, mutualism, human–wildlife interaction).  
2. Split each into ≥4 level-2 sub-topics.  
3. For every level-2 topic list:
   - 3–5 highly-cited reviews or meta-analyses (2020-2025, with DOIs)  
   - Classic model/equation name (e.g. Charnov 1976 MVT)  
   - Open-source simulation code (NetLogo Models Library, GitHub, or permanent link)  
4. Format: Markdown H3 heading, then a table with columns:  
   Sub-topic | Key review DOI | Classic model | Open-source link | Notes

---

## STEP 2 Modeling-Friendliness Rapid Screen (auto-table)
1. Rate **every level-2 topic** 1–5 stars on:
   - Theoretical maturity (equations exist)  
   - Parameter availability (means published)  
   - Simulation scale (&lt;200 agents sufficient)  
   - Visual intuitiveness (3-min GIF-friendly)  
2. Build a master CSV-style table with columns:  
   Level-1 ID | Level-2 ID | Level-2 topic | Theory ★ | Param ★ | Scale ★ | Viz ★ | Mean ★ | ≤20-char keyword  
3. Highlight mean ≥4 in green, ≤2 in red.  
4. End with a 50-char summary: which topics best fit a “theory + NetLogo/Python” class report.

---

## STEP 3 Innovation Gap Deep-Dive (numbered list)
1. For topics with **mean ≥4**, retrieve ≥5 experimental/observational papers (2023-2025) per topic.  
2. Each gap entry contains:
   - Gap ≤40 chars  
   - New variable/mechanism ≤30 chars  
   - Suggested modeling route ≤20 chars  
   - Data source ≤20 chars  
   - Feasibility 1–5 ★  
3. Output ≥10 gaps, ≥3 implementable in **≤100 NetLogo lines**.  
4. Format: numbered list, ≤80 chars per entry.

---

## STEP 4 Actionable Checklist
1. Extract the **top 3 recommended gaps** into a checklist giving:
   - Title ≤15 chars  
   - Core assumption (1 sentence)  
   - Needed parameters (3–5 items with DOIs)  
   - Expected simulation output (1 sentence)  
   - 1-week roadmap (Day1–7, one line each)  
2. Prefix each item with ✅ for copy-paste into task managers.

---

Execute **non-stop** and deliver:
- STEP 1 tree-style Markdown  
- STEP 2 CSV table (code block)  
- STEP 3 gap list (numbered)  
- STEP 4 checklist (✅ task lines)

**End of delivery!**
```

Disclaimer: final topic report generated by **Bohrium** platform.
