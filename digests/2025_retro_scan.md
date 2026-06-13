# 2025 年四方向论文回溯扫描

> 检索日期：2026-06-13。覆盖 2025-01 至 2025-12，共收录 38 篇。
> 来源：Hugging Face Papers、arXiv、Google Scholar、Semantic Scholar、GitHub。
> 排序：顶会/顶刊录用 > 高赞 > 其他；同类内按发表时间降序。

---

## 方向一：VPR（Visual Place Recognition / 视觉位置识别 / 图像地理定位）

**UGNA-VPR: A Novel Training Paradigm for Visual Place Recognition Based on Uncertainty-Guided NeRF Augmentation**
Yehui Shen et al.
[2503.21338](https://arxiv.org/abs/2503.21338) (2025-03, CVPR 2025)
`[CVPR 2025]`
提出基于不确定性引导 NeRF 增强的 VPR 训练范式，通过自监督不确定性估计网络识别高不确定性场景，将其位姿输入 NeRF 合成新视角图像补充训练集，提升模型在多方向行驶和稀疏特征场景中的识别精度，在三个数据集上以三种 VPR 骨干网络进行了验证。
**归属方向：方向一 · VPR**

---

**SelaVPR++: Towards Seamless Adaptation of Foundation Models for Efficient Place Recognition**
Feng Lu et al.
[2502.16601](https://arxiv.org/abs/2502.16601) (2025-02, T-PAMI 2025)
`[T-PAMI 2025]`
提出轻量级多尺度卷积适配器（MultiConv Adapter），在冻结基础视觉模型骨干的基础上微调中间特征，同时用紧凑二值特征做初步检索、高维浮点特征做重排，无需局部特征匹配，大幅降低训练显存占用和检索延迟，在多个 VPR 基准上取得领先性能。
**归属方向：方向一 · VPR**

---

**Focus on Local: Finding Reliable Discriminative Regions for Visual Place Recognition**
Changwei Wang et al.
[2504.09881](https://arxiv.org/abs/2504.09881) (2025-04, AAAI 2025)
`[AAAI 2025]`
提出 FoL 框架，设计提取-聚合空间对齐损失（SAL）和前背景对比增强损失（CEL），显式建模可靠判别局部区域；同步提升 VPR 检索与重排性能，在多个 VPR 基准上以更高计算效率超越现有两阶段方法。
**归属方向：方向一 · VPR**

---

**SAGE: Spatial-visual Adaptive Graph Exploration for Efficient Visual Place Recognition**
Shunpeng Chen et al.
[2509.25723](https://arxiv.org/abs/2509.25723) (2025-09, ICLR 2026 录用)
`[ICLR 2026 录用]`
提出统一 VPR 训练流水线，通过轻量级 Soft Probing 模块学习块描述符的残差权重，在线重建融合地理邻近性与视觉相似性的地理-视觉图以优化候选邻域，联合提升局部特征聚合与困难样本挖掘，以冻结 DINOv2 骨干在八个多样化 VPR 基准上实现新 SOTA。
**归属方向：方向一 · VPR**

---

**GeoRanker: Distance-Aware Ranking for Worldwide Image Geolocalization**
Pengyue Jia et al.
[2505.13731](https://arxiv.org/abs/2505.13731) (2025-05)
`[HF▲2]`
提出 GeoRanker 距离感知排名框架，利用大型视觉-语言模型对查询-候选图像对进行联合编码，引入多阶距离损失同时对绝对距离和相对距离进行监督，使模型能推理候选集内的空间结构关系；构建 GeoRanking 数据集，在 IM2GPS3K 和 YFCC4K 上取得最优结果。
**归属方向：方向一 · VPR**

---

**GeoVLM: Improving Automated Vehicle Geolocalisation Using Vision-Language Matching**
Barkin Dagda et al.
[2505.13669](https://arxiv.org/abs/2505.13669) (2025-05)
利用视觉-语言模型对卫星-地面跨视角匹配进行零样本重排，借助 VLM 生成可解释的跨视角语言描述来提升匹配精度和可解释性；在 VIGOR、University-1652、Cross-View United Kingdom 等数据集上改善了跨视角地理定位性能。
**归属方向：方向一 · VPR**

---

**MMS-VPR: Multimodal Street-Level Visual Place Recognition Dataset and Benchmark**
Yiwei Ou et al.
[2505.12254](https://arxiv.org/abs/2505.12254) (2025-05)
`[HF▲1]`
提出 MMS-VPR 大规模多模态街道级视觉位置识别数据集，包含成都商业区 207 个地点的 78,575 张标注图像与 2,512 段视频，配有精确 GPS 坐标、时间戳和文本元数据；数据集形成含 125 条边的空间图，支持结构感知的位置识别研究。
**归属方向：方向一 · VPR**

---

**Visual Re-Ranking with Non-Visual Side Information (GCSA)**
Gustav Hanning et al.
[2504.11134](https://arxiv.org/abs/2504.11134) (2025-04)
提出广义上下文相似度聚合（GCSA），基于图神经网络在视觉描述符之外额外融合 WiFi/蓝牙信号强度或数据库图像位姿等非视觉侧信息进行 VPR 重排，利用亲和向量实现异构多模态输入的统一编码，在室内外大规模数据集上提升定位性能。
**归属方向：方向一 · VPR**

---

**To Match or Not to Match: Revisiting Image Matching for Reliable Visual Place Recognition**
Davide Sferrazza et al.
[2504.06116](https://arxiv.org/abs/2504.06116) (2025-04)
重新审视图像匹配在 VPR 重排中的必要性，通过实验证明现代 VPR 检索系统在已高度饱和的数据集上应用重排反而会降低性能，提出将内点匹配数量作为置信度指标以预测重排是否有益。
**归属方向：方向一 · VPR**

---

**Recognition through Reasoning: Reinforcing Image Geo-localization with Large Vision-Language Models (GLOBE)**
Ling Li et al.
[2506.14674](https://arxiv.org/abs/2506.14674) (2025-06)
构建基于多样社交媒体图像的推理导向地理定位数据集 MP16-Reason，提出 GLOBE 框架通过任务专属奖励联合增强可定位性评估、视觉线索推理和定位精度，在多样视觉场景上超越现有开源大型视觉-语言模型。
**归属方向：方向一 · VPR**

---

**R-SCoRe: Revisiting Scene Coordinate Regression for Robust Large-Scale Visual Localization**
Xudong Jiang et al.
[2501.01421](https://arxiv.org/abs/2501.01421) (2025-01)
`[HF▲2]`
提出利用协可见性图与深度调整重投影损失改进大规模场景坐标回归（SCR）视觉定位方法，通过协可见性图辅助全局编码与数据增强，在 Aachen Day-Night 等大规模数据集上以更小地图规模实现更高定位精度。
**归属方向：方向一 · VPR / 图像定位**

---

## 方向二：Agent 做检索（Agentic Retrieval / LLM-Agent RAG / Search Agent）

**ZeroSearch: Incentivize the Search Capability of LLMs without Searching**
Hao Sun et al.
[2505.04588](https://arxiv.org/abs/2505.04588) (2025-05)
`[HF▲66]`
提出 ZeroSearch 强化学习框架，通过轻量级 SFT 预热和课程式 rollout 策略在模拟检索环境中训练 LLM 的搜索能力，完全无需调用真实搜索引擎 API；在多尺寸 LLM 和多类 RL 算法上验证有效性，大幅降低训练成本。
**归属方向：方向二 · Agent 做检索**

---

**Search-R1: Training LLMs to Reason and Leverage Search Engines with Reinforcement Learning**
Bowen Jin et al.
[2503.09516](https://arxiv.org/abs/2503.09516) (2025-03)
`[HF▲40]`
通过强化学习（支持 PPO/GRPO/REINFORCE 等）训练 LLM 在多步推理过程中自动生成多轮搜索查询并利用检索结果，引入检索词遮蔽策略实现稳定训练；在七个问答数据集上比各类 RAG 基线分别提升 20%（Qwen2.5-3B）和 41%（Qwen2.5-7B）。
**归属方向：方向二 · Agent 做检索**

---

**RAVine: Reality-Aligned Evaluation for Agentic Search**
Yilong Xu et al.
[2507.16725](https://arxiv.org/abs/2507.16725) (2025-07)
`[HF▲31]`
提出 RAVine 现实对齐的 Agentic Search 评估框架，专注于含多个问题点的复杂查询、精确可溯源标注以及对迭代检索过程效率的量化，弥补了现有评估集在查询复杂度和过程评估指标上的不足。
**归属方向：方向二 · Agent 做检索**

---

**Agentic Reasoning: Reasoning LLMs with Tools for the Deep Research**
Junde Wu et al.
[2502.04644](https://arxiv.org/abs/2502.04644) (2025-02)
`[HF▲4]`
提出 Agentic Reasoning 框架，整合网络搜索 Agent、代码执行 Agent 和思维导图 Agent（构建结构化知识图追踪逻辑关系），通过 Agent 间协作动态获取实时信息并进行多步逻辑推导；在 GPQA 和深度研究任务上超越现有 RAG 系统及闭源大模型。
**归属方向：方向二 · Agent 做检索**

---

**From Web Search towards Agentic Deep Research: Incentivizing Search with Reasoning Agents**
Weizhi Zhang et al.
[2506.18959](https://arxiv.org/abs/2506.18959) (2025-06)
`[HF▲5]`
梳理从静态关键词搜索引擎到 LLM 驱动的 Agentic Deep Research 范式的演进路径，引入测试时扩展律量化计算深度对检索推理能力的影响，综述 OpenAI Deep Research 等工业产品及开源实现，并整理相关资源库。
**归属方向：方向二 · Agent 做检索**

---

**Agentic Retrieval-Augmented Generation: A Survey on Agentic RAG**
Aditi Singh et al.
[2501.09136](https://arxiv.org/abs/2501.09136) (2025-01)
`[HF▲3]`
系统综述将自主 AI 智能体嵌入 RAG 流水线的 Agentic RAG 范式，覆盖反思、规划、工具调用和多智能体协作四种设计模式，梳理架构分类与在医疗、金融、教育等领域的应用，提供该领域首份全面综述。
**归属方向：方向二 · Agent 做检索**

---

**ManuSearch: Democratizing Deep Search in Large Language Models with a Transparent and Open Multi-Agent Framework**
Lisheng Huang et al.
[2505.18105](https://arxiv.org/abs/2505.18105) (2025-05)
提出 ManuSearch 透明开源多智能体深度搜索框架，由方案规划 Agent（迭代子查询生成）、互联网搜索 Agent（实时网络检索）和网页阅读 Agent（关键证据提取）三部分协作完成复杂推理；发布 ORION 基准，在英中两语言上超越闭源系统。
**归属方向：方向二 · Agent 做检索**

---

**Agent-UniRAG: A Trainable Open-Source LLM Agent Framework for Unified Retrieval-Augmented Generation Systems**
Hoang Pham et al.
[2505.22571](https://arxiv.org/abs/2505.22571) (2025-05)
提出 Agent-UniRAG 可训练 LLM Agent 框架，在同一端到端架构中统一处理单跳和多跳 RAG 任务，根据输入复杂度逐步决策检索步骤；发布合成训练数据集 SynAgent-RAG 支持 Llama-3-8B 等小型开源模型，在多个 RAG 基准上取得与大模型相当的性能。
**归属方向：方向二 · Agent 做检索**

---

**A Comprehensive Survey on Reinforcement Learning-based Agentic Search**
Minhua Lin et al.
[2510.16724](https://arxiv.org/abs/2510.16724) (2025-10)
提供 RL 驱动 Agentic Search 领域首篇全面综述，沿功能角色（RL 的目标）、优化策略（RL 的使用方式）和优化范围三维度梳理代表性方法，总结评测协议和应用场景，讨论构建可靠可扩展 RL 驱动搜索系统面临的开放挑战。
**归属方向：方向二 · Agent 做检索**

---

**Interact-RAG: Reason and Interact with the Corpus, Beyond Black-Box Retrieval**
Yulong Hui et al.
[2510.27566](https://arxiv.org/abs/2510.27566) (2025-10)
`[HF▲1]`
提出 Interact-RAG 范式，通过语料交互引擎（Corpus Interaction Engine）赋予 LLM Agent 对检索过程的细粒度操作原语，突破黑盒查询局限；结合推理增强工作流和监督微调+强化学习的端到端 Agent 训练，在六个基准上取得领先性能。
**归属方向：方向二 · Agent 做检索**

---

**TeaRAG: A Token-Efficient Agentic Retrieval-Augmented Generation Framework**
Chao Zhang et al.
[2511.05385](https://arxiv.org/abs/2511.05385) (2025-11)
`[HF▲1]`
提出 TeaRAG Token 高效 Agentic RAG 框架，通过语义检索结合知识关联图（Personalized PageRank）压缩每次检索的 Token 数量，并通过迭代过程感知 DPO（IP-DPO）减少多余推理步骤；在六个数据集上使 Llama3-8B 精确匹配提升约4%、输出 Token 减少约61%。
**归属方向：方向二 · Agent 做检索**

---

**ReSeek: A Self-Correcting Framework for Search Agents with Instructive Rewards**
Shiyu Li et al.
[2510.00568](https://arxiv.org/abs/2510.00568) (2025-10)
提出 ReSeek 自纠错框架，为搜索 Agent 设计密集奖励函数（包含正确性奖励和效用奖励），在知识密集型任务中通过 JUDGE 动作触发动态错误恢复与重规划；在 FictionalHot 基准上取得任务成功率和路径忠实度的提升。
**归属方向：方向二 · Agent 做检索**

---

## 方向三：Agent 做图像检索（Agentic Image Retrieval / Multimodal Retrieval Agent / CIR）

**MMSearch-R1: Incentivizing LMMs to Search**
Jinming Wu et al.
[2506.20670](https://arxiv.org/abs/2506.20670) (2025-06)
`[HF▲65]`
提出首个端到端强化学习框架，使大型多模态模型（LMM）在真实互联网环境中按需执行多轮图像与文本搜索；通过搜索惩罚结合结果奖励设计搜索行为塑造机制，构建多模态搜索 VQA 数据集，在知识密集型 VQA 任务上超越同规模 RAG 基线并减少超30%搜索调用次数。
**归属方向：方向三 · Agent 做图像检索**

---

**SQUARE: Semantic Query-Augmented Fusion and Efficient Batch Reranking for Training-free Zero-Shot Composed Image Retrieval**
Ren-Di Wu et al.
[2509.26330](https://arxiv.org/abs/2509.26330) (2025-09)
`[HF▲2]`
提出 SQUARE 两阶段无训练零样本 CIR 框架，第一阶段通过语义查询增强融合（SQAF）利用 MLLM 丰富查询嵌入，第二阶段通过高效批量重排（EBR）在候选集中进行跨模态视觉-语义联合推理；在 CIRR、FashionIQ 等基准的零样本 CIR 任务上取得新最优性能。
**归属方向：方向三 · Agent 做图像检索 / CIR**

---

**IDMR: Towards Instance-Driven Precise Visual Correspondence in Multimodal Retrieval**
Bangwei Liu et al.
[2504.00954](https://arxiv.org/abs/2504.00954) (2025-04)
`[HF▲2]`
提出实例驱动多模态图像检索（IDMR）任务，要求模型在跨上下文图像中定位与查询图像同一实例的图像，同时满足文本场景描述；利用目标跟踪和第一视角视频数据构建 IDMR-bench，提出跨域合成方法生成55.7万条训练样本，MLLM 检索模型在零样本评测上取得最优性能。
**归属方向：方向三 · Agent 做图像检索**

---

**A Comprehensive Survey on Composed Image Retrieval**
Xuemeng Song et al.
[2502.18495](https://arxiv.org/abs/2502.18495) (2025-02)
综述120余篇 ACM TOIS、SIGIR、CVPR 等顶级会议和期刊中的组合图像检索（CIR）研究，建立涵盖监督 CIR 和零样本 CIR 的精细化分类体系，比较各方法在 FashionIQ、CIRR、CIRCO 等标准基准上的实验结果，并讨论属性导向 CIR、对话式 CIR 及未来方向。
**归属方向：方向三 · Agent 做图像检索 / CIR**

---

**Generative Giants, Retrieval Weaklings: Why do Multimodal Large Language Models Fail at Multimodal Retrieval?**
Hengyi Feng et al.
[2512.19115](https://arxiv.org/abs/2512.19115) (2025-12)
利用稀疏自编码器分析揭示 MLLM 在多模态检索中表现不佳的两个根本原因：表示空间中文本语义主导导致视觉信息被压制、以及嵌入同质化削弱判别能力，为改进 MLLM 判别式检索提供可操作的诊断工具和理论依据。
**归属方向：方向三 · Agent 做图像检索**

---

**Patho-AgenticRAG: Towards Multimodal Agentic Retrieval-Augmented Generation for Pathology VLMs via Reinforcement Learning**
Wenchuan Zhang et al.
[2508.02258](https://arxiv.org/abs/2508.02258) (2025-08)
`[HF▲1]`
提出病理学领域多模态 Agentic RAG 框架，基于病理教材的页面级图文嵌入实现联合文本-图像搜索与推理，通过任务分解与多轮搜索交互处理复杂病理诊断 VQA；在多项复杂病理任务上显著超越单轮 RAG 基线。
**归属方向：方向三 · Agent 做图像检索**

---

## 方向四：Agent 做细粒度检索（Agentic Fine-Grained Retrieval / Fine-Grained Image Retrieval with LLM）

**Llama Nemoretriever Colembed: Top-Performing Text-Image Retrieval Model**
Mengyao Xu et al. (NVIDIA)
[2507.05513](https://arxiv.org/abs/2507.05513) (2025-07)
`[HF▲1 | ViDoRe V1 & V2 榜首]`
基于 NVIDIA Eagle2 视觉-语言模型，将因果注意力替换为双向注意力并集成 ColBERT 式晚期交互机制，在共享嵌入空间中实现细粒度多模态检索；3B 模型在 ViDoRe V1（NDCG@5=91.0）和 ViDoRe V2（63.5）均位列排行榜第一（截至 2025-06-27）。
**归属方向：方向四 · Agent 做细粒度检索**

---

**Composed Object Retrieval (COR): Object-level Retrieval via Composed Expressions**
Tong Wang et al.
[2508.04424](https://arxiv.org/abs/2508.04424) (2025-08)
`[HF▲1]`
提出 Composed Object Retrieval（COR）新任务，将 CIR 从图像级匹配延伸至对象级检索与分割，要求系统根据参考对象与修改文本的组合表达定位特定目标；构建 COR127K 大规模基准（127,166 条三元组，408 类别），并提出集成参考区域编码与区域级对比学习的 CORE 模型。
**归属方向：方向四 · Agent 做细粒度检索**

---

**SETR: A Two-Stage Semantic-Enhanced Framework for Zero-Shot Composed Image Retrieval**
Yuqi Xiao et al.
[2509.26012](https://arxiv.org/abs/2509.26012) (2025-09)
提出 SETR 两阶段语义增强零样本 CIR 框架：粗检索阶段通过交集驱动策略过滤参考图像与修改文本之间无关视觉干扰，细粒度重排阶段使用 LoRA 微调的多模态 LLM 进行二元语义相关性判断；在 CIRR 上 Recall@1 最高提升15.15个百分点。
**归属方向：方向四 · Agent 做细粒度检索**

---

**DetailFusion: A Dual-branch Framework with Detail Enhancement for Composed Image Retrieval**
Yuxin Yang et al.
[2505.17796](https://arxiv.org/abs/2505.17796) (2025-05)
提出 DetailFusion 双分支框架，利用图像编辑数据集中的原子级细节变化先验，设计细节导向推理分支与自适应特征合成器，动态融合全局与细粒度特征；在 CIRR 和 FashionIQ 数据集上取得最优性能，并验证了细节增强的跨域适应性。
**归属方向：方向四 · Agent 做细粒度检索**

---

**FineCIR: Explicit Parsing of Fine-Grained Modification Semantics for Composed Image Retrieval**
Zixu Li et al.
[2503.21309](https://arxiv.org/abs/2503.21309) (2025-03)
提出 FineCIR 框架，通过显式解析 CIR 修改文本中的细粒度语义并与视觉实体精准对齐，以减少粗粒度文本带来的歧义；构建 Fine-FashionIQ 和 Fine-CIRR 两个细粒度 CIR 注释数据集，在细粒度和传统 CIR 基准（FashionIQ、CIRR）上均超越现有方法。
**归属方向：方向四 · Agent 做细粒度检索**

---

**Rethinking Vision Transformer for Large-Scale Fine-Grained Image Retrieval (EET)**
Xin Jiang et al.
[2504.16691](https://arxiv.org/abs/2504.16691) (2025-04)
提出 EET 高效有效细粒度大规模图像检索框架，通过内容感知 Token 剪枝模块在 ViT 各阶段渐进去除低判别性 Token 以降低计算量，采用判别性知识蒸馏和判别区域引导策略；在 NABirds 等6个细粒度数据集上 ViT-Small 推理延迟降低42.7%、16位哈希检索性能提升5.15%。
**归属方向：方向四 · Agent 做细粒度检索**

---

**Benchmarking Large Vision-Language Models on Fine-Grained Image Tasks (FG-BMK)**
Hong-Tao Yu et al.
[2504.14988](https://arxiv.org/abs/2504.14988) (2025-04)
构建含101万道问题、33万张图像的大规模细粒度评测基准 FG-BMK，从人类导向和机器导向两个视角系统评估12个代表性 LVLM 在语义识别与细粒度特征表示上的能力，揭示训练范式、模态对齐方式、扰动鲁棒性和细粒度类别推理对任务性能的关键影响。
**归属方向：方向四 · Agent 做细粒度检索**

---

**good4cir: Generating Detailed Synthetic Captions for Composed Image Retrieval**
Pranavi Kolouju et al.
[2503.17871](https://arxiv.org/abs/2503.17871) (2025-03)
提出 good4cir 结构化流水线，利用 VLM 为 CIR 生成高质量细粒度合成注释：从查询图像提取精细对象描述、为目标图像生成可比较描述、再合成捕捉图像间有意义变换的文本指令，减少幻觉并增强修改多样性，可提升多领域 CIR 模型检索精度。
**归属方向：方向四 · Agent 做细粒度检索**

---

**Category-level Text-to-Image Retrieval Improved: Bridging the Domain Gap with Diffusion Models and Vision Encoders**
Faizan Farooq Khan et al.
[2509.00177](https://arxiv.org/abs/2509.00177) (2025-09)
提出两步方法改善类别级文本到图像检索：首先使用生成式扩散模型将文本查询转换为视觉查询，再通过视觉模型聚合多图像表示，弥合跨域检索中的文本-图像语义鸿沟；在 DFMM-Compose 等文本-图像检索基准上超越纯 CLIP 方法。
**归属方向：方向四 · Agent 做细粒度检索**
