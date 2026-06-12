> 📌 本封为一次性整理的《2025 关键论文清单》(相关工作梳理 / 答辩准备),非每日新论文摘报。

# 2025 年关键论文清单：VPR、VLM 地点识别与 Agentic 检索

> **用途说明**：本文档为本科毕业论文相关工作梳理与答辩准备整理的论文清单，时间覆盖 2023 末 ~ 2026 初（重点在 2024–2025 年），围绕「用 VLM 生成文本描述做 VPR 检索 + agentic 校验（verifier / OCRAgent）+ divide-and-conquer 零训练 UTM cell 分类」三条研究主线收录关键论文。链接均已核实；被引数如无法通过检索工具直接读取，标注「未知」。

---

## 线 1：VPR / 视觉位置识别 SOTA 方法

涵盖聚合策略创新、Foundation Model 微调适配和新基准，包含本工作所用的 backbone 与主要对标 baseline。

---

### 1.1 **MixVPR: Feature Mixing for Visual Place Recognition**

- **第一作者**：Amar Ali-bey
- **年份**：2023
- **Venue**：WACV 2023（IEEE/CVF Winter Conference on Applications of Computer Vision，A 类会议）
- **被引数**：未知
- **链接**：[arXiv:2303.02190](https://arxiv.org/abs/2303.02190)，WACV 2023
- **与本毕设关系**：全 MLP 特征混合聚合，将预训练 backbone 的全局特征图经 row-wise 和 channel-wise mixing 聚合为全局描述子；是本工作 Pitts30k / Pitts250k 实验中的经典 baseline，AnyLoc、BoQ 等后续工作均与其对比。

---

### 1.2 **EigenPlaces: Training Viewpoint Robust Models for Visual Place Recognition**

- **第一作者**：Gabriele Berton
- **年份**：2023
- **Venue**：ICCV 2023（IEEE/CVF International Conference on Computer Vision，CCF-A 顶会）
- **被引数**：约 39（来源：搜索引擎摘要自 Semantic Scholar，截至检索日期，待核实）
- **链接**：[arXiv:2308.10832](https://arxiv.org/abs/2308.10832)，ICCV 2023
- **与本毕设关系**：以地理聚类方式构建训练集，使模型对视点变化鲁棒；是 Pitts250k 标准对标 baseline 之一，本工作在 Pitts 数据集上须引用并对比。

---

### 1.3 **AnyLoc: Towards Universal Visual Place Recognition**

- **第一作者**：Nikhil Varma Keetha
- **年份**：2023
- **Venue**：RA-L 2023（IEEE Robotics and Automation Letters，SCI 一区顶刊）
- **被引数**：未知（2024–2025 年多篇顶会论文广泛引用）
- **链接**：[arXiv:2308.00688](https://arxiv.org/abs/2308.00688)，RA-L 2023
- **与本毕设关系**：**本工作直接使用的 backbone**。AnyLoc 以 DINOv2 特征 + VLAD 聚合实现零训练通用 VPR，覆盖 12 个多样化数据集；是本工作的起点与核心依赖方法，答辩须详细介绍。

---

### 1.4 **Optimal Transport Aggregation for Visual Place Recognition (SALAD)**

- **第一作者**：Sergio Izquierdo
- **年份**：2024
- **Venue**：CVPR 2024（IEEE/CVF Conference on Computer Vision and Pattern Recognition，CCF-A 顶会）
- **被引数**：未知
- **链接**：[arXiv:2311.15937](https://arxiv.org/abs/2311.15937)，CVPR 2024
- **与本毕设关系**：用 Sinkhorn 最优传输将 NetVLAD 的软分配重构为 OT 问题，引入 dustbin cluster 过滤无效特征，并微调 DINOv2；是本工作 Pitts 数据集上的重要对标方法，聚合设计可参考借鉴。

---

### 1.5 **BoQ: A Place is Worth a Bag of Learnable Queries**

- **第一作者**：Amar Ali-Bey
- **年份**：2024
- **Venue**：CVPR 2024（CCF-A 顶会）
- **被引数**：未知
- **链接**：[arXiv:2405.07364](https://arxiv.org/abs/2405.07364)，CVPR 2024
- **与本毕设关系**：一组可学习全局查询通过跨注意力机制探测输入特征，在 14 个 VPR 基准上超越 MixVPR、EigenPlaces 等；本工作重要对标 baseline，Pitts250k-test 上须引用其指标。

---

### 1.6 **CricaVPR: Cross-image Correlation-aware Representation Learning for Visual Place Recognition**

- **第一作者**：Feng Lu
- **年份**：2024
- **Venue**：CVPR 2024（CCF-A 顶会）
- **被引数**：未知
- **链接**：[arXiv:2402.19231](https://arxiv.org/abs/2402.19231)，CVPR 2024
- **与本毕设关系**：批内跨图像注意力机制 + 多尺度卷积高效适配 Foundation Model 做 VPR，性能显著领先；本工作在 Pitts 系列上的重要对标方法，可与本工作零训练方案比较性能差距。

---

### 1.7 **SelaVPR++: Towards Seamless Adaptation of Foundation Models for Efficient Place Recognition**

- **第一作者**：Feng Lu
- **年份**：2025
- **Venue**：arXiv 预印本（2025 年 2 月，待投顶会）
- **被引数**：未知
- **链接**：[arXiv:2502.16601](https://arxiv.org/abs/2502.16601)，arXiv 2025
- **与本毕设关系**：参数高效适配 + 轻量多尺度卷积 + 紧凑二进制特征 + 优化重排序，兼顾精度与效率；代表 2025 年 Foundation Model 适配 VPR 的前沿，可作为本工作性能上界参照。

---

### 1.8 **SuperPlace: The Renaissance of Classical Feature Aggregation for Visual Place Recognition in the Era of Foundation Models**

- **第一作者**：Bingxi Liu
- **年份**：2025
- **Venue**：arXiv 预印本（2025 年 6 月）
- **被引数**：未知
- **链接**：[arXiv:2506.13073](https://arxiv.org/abs/2506.13073)，arXiv 2025
- **与本毕设关系**：重拾 GeM / NetVLAD 等经典聚合与 Foundation Model 结合，SuperPlace-NVL-FT2 登上 MSLS Challenge 榜首；为本工作提供 2025 年最新 SOTA 性能上界，答辩定位用。

---

## 线 2：语言 / 文本 / VLM 驱动的地点识别与地理定位

与本毕设创新点**最直接相关**，用于界定「用 VLM 文本描述做 VPR」的创新边界，确认本工作的独特贡献。

---

### 2.1 **LVLM-empowered Multi-modal Representation Learning for Visual Place Recognition**

- **第一作者**：Teng Wang
- **年份**：2024
- **Venue**：arXiv 预印本（2024 年 7 月，未见顶会收录记录）
- **被引数**：未知
- **链接**：[arXiv:2407.06730](https://arxiv.org/abs/2407.06730)，arXiv 2024
- **与本毕设关系**：⚠️ **创新边界最关键论文**。该文提出 LVL3M-VPR，以 LVLM 生成场景文本描述并与图像特征多模态融合用于 VPR，与本毕设核心思路高度相近。**答辩时必须明确说明差异**：本工作额外引入 agentic verifier 二次确认、OCRAgent 读招牌文字、divide-and-conquer UTM cell 零训练分类，聚焦 Pitts30k / Pitts250k 城市大规模场景，而非单纯多模态特征融合。

---

### 2.2 **Context-Based Visual-Language Place Recognition**

- **第一作者**：Soojin Woo
- **年份**：2024
- **Venue**：arXiv 预印本（2024 年 10 月）
- **被引数**：未知
- **链接**：[arXiv:2410.19341](https://arxiv.org/abs/2410.19341)，arXiv 2024
- **与本毕设关系**：以零样本语言驱动语义分割生成像素级语义描述符用于 VPR，无需额外训练；与本工作「零训练」思路相近，但未使用 VLM 生成自然语言文本描述，是本工作界定创新边界的参照论文。

---

### 2.3 **Image-based Geo-localization for Robotics: Are Black-box Vision-Language Models there yet?**

- **第一作者**：Sania Waheed
- **年份**：2025
- **Venue**：arXiv 预印本（2025 年 1 月）
- **被引数**：未知
- **链接**：[arXiv:2501.16947](https://arxiv.org/abs/2501.16947)，arXiv 2025
- **与本毕设关系**：系统评估黑盒 VLM 作为独立零样本地理定位系统的能力与局限，揭示 VLM 单独做 VPR 时的不稳定性；为本工作「VLM 辅助检索而非单独定位」设计选择提供实验依据。

---

### 2.4 **Bridging Text and Vision: A Multi-View Text-Vision Registration Approach for Cross-Modal Place Recognition (Text4VPR)**

- **第一作者**：Tianyi Shang
- **年份**：2025
- **Venue**：arXiv 预印本（2025 年 2 月）
- **被引数**：未知
- **链接**：[arXiv:2502.14195](https://arxiv.org/abs/2502.14195)，arXiv 2025
- **与本毕设关系**：⚠️ **创新边界论文**。冻结 T5 文本嵌入 + Sinkhorn 最优传输实现文本描述到图像的跨模态 VPR（Street360Loc 数据集）。与本工作均采用自然语言描述检索图像，但本工作针对 Pitts 城市场景并引入 agentic 校验，创新边界答辩中需对照说明。

---

### 2.5 **TextInPlace: Indoor Visual Place Recognition in Repetitive Structures with Scene Text Spotting and Verification**

- **第一作者**：Huaqi Tao
- **年份**：2025
- **Venue**：IEEE（arXiv:2503.06501，IEEE Xplore 已收录，具体会议/期刊待核实）
- **被引数**：未知
- **链接**：[arXiv:2503.06501](https://arxiv.org/abs/2503.06501)，IEEE 2025
- **与本毕设关系**：⚠️ **OCRAgent 创新边界论文**。双分支架构集成 Scene Text Spotting（STS）做室内重复场景 VPR 的文字验证，与本工作 OCRAgent 读招牌文字思路**最为接近**。差异：本工作面向**室外城市**（Pitts）大规模场景，以 VLM 生成自然语言描述为第一阶段，OCR 为 agentic 第二阶段校验，答辩须明确指出此区别。

---

### 2.6 **VLM-Guided Visual Place Recognition for Planet-Scale Geo-Localization**

- **第一作者**：Sania Waheed
- **年份**：2025
- **Venue**：arXiv 预印本（2025 年 7 月）
- **被引数**：未知
- **链接**：[arXiv:2507.17455](https://arxiv.org/abs/2507.17455)，arXiv 2025
- **与本毕设关系**：VLM 生成初始坐标估计作为先验，再用 VPR 方法在受限搜索空间精细检索；混合 VLM + 检索架构与本工作思路高度一致，但本工作额外引入 agentic verifier + OCR 校验环节。

---

### 2.7 **Scale, Don't Fine-tune: Guiding Multimodal LLMs for Efficient Visual Place Recognition at Test-Time**

- **第一作者**：Jintao Cheng
- **年份**：2025
- **Venue**：arXiv 预印本（2025 年 9 月）
- **被引数**：未知
- **链接**：[arXiv:2509.02129](https://arxiv.org/abs/2509.02129)，arXiv 2025
- **与本毕设关系**：Test-Time Scaling + Uncertainty-Aware Self-Consistency（UASC），无需微调直接用 MLLM 做 VPR 相似度打分，效率提升 210×；与本工作均利用 MLLM 能力，但本工作侧重 VLM 生成描述后检索而非直接相似度打分，设计路线不同。

---

### 2.8 **LaVPR: Benchmarking Language and Vision for Place Recognition**

- **第一作者**：Ofer Idan
- **年份**：2026
- **Venue**：arXiv 预印本（2026 年 2 月）
- **被引数**：未知
- **链接**：[arXiv:2602.03253](https://arxiv.org/abs/2602.03253)，arXiv 2026
- **与本毕设关系**：为现有 VPR 数据集配套超 65 万条自然语言描述，建立语言 + 视觉联合 VPR 大规模 benchmark；直接为本工作的文本描述检索方向提供 benchmark 参照，可引用以佐证本方向在学界的研究价值。

---

## 线 3：Agentic 检索 / LLM-agent 检索

对应本工作的 verifier 二次确认 / OCRAgent 多步骤校验思路，以及 divide-and-conquer agentic 推理框架。

---

### 3.1 **Agentic Information Retrieval**

- **第一作者**：Weinan Zhang
- **年份**：2024
- **Venue**：arXiv 预印本（2024 年 10 月）
- **被引数**：未知
- **链接**：[arXiv:2410.09713](https://arxiv.org/abs/2410.09713)，arXiv 2024
- **与本毕设关系**：系统梳理 LLM 驱动的 Agentic IR 范式——规划、工具调用、多步推理；为本工作 agentic verifier 框架提供理论基础与概念定义，答辩引用以定位本工作在 IR+Agent 交叉领域的位置。

---

### 3.2 **Agentic Retrieval-Augmented Generation: A Survey on Agentic RAG**

- **第一作者**：Aditi Singh
- **年份**：2025
- **Venue**：arXiv 预印本（2025 年 1 月）
- **被引数**：未知
- **链接**：[arXiv:2501.09136](https://arxiv.org/abs/2501.09136)，arXiv 2025
- **与本毕设关系**：综合综述 Agentic RAG——自主检索、动态规划与上下文理解；本工作的 verifier + OCRAgent 可视为面向 VPR 场景的特化 Agentic RAG，引用本综述可为答辩提供完整的相关工作叙事框架。

---

### 3.3 **Multimodal Reasoning Agent for Zero-Shot Composed Image Retrieval**

- **第一作者**：Rong-Cheng Tu
- **年份**：2025
- **Venue**：arXiv 预印本（2025 年 5 月）
- **被引数**：未知
- **链接**：[arXiv:2505.19952](https://arxiv.org/abs/2505.19952)，arXiv 2025
- **与本毕设关系**：多模态推理 agent（MRA）直接用未标注图像构建三元组、绕过文本中间表示做零样本组合图像检索；与本工作 verifier agent 对候选结果做多步推理校验的思路相近，是方法借鉴的直接来源。

---

### 3.4 **XR: Cross-Modal Agents for Composed Image Retrieval**

- **第一作者**：Zhongyu Yang
- **年份**：2026
- **Venue**：arXiv 预印本（2026 年 1 月，HuggingFace 8 upvotes）
- **被引数**：未知
- **链接**：[arXiv:2601.14245](https://arxiv.org/abs/2601.14245)，arXiv 2026
- **与本毕设关系**：多 agent 框架分工做生成、过滤与验证，实现跨模态组合图像检索；其「专用 verification agent」子模块与本工作 verifier 二次确认设计高度相近，方法借鉴价值最高。

---

### 3.5 **DeepImageSearch: Benchmarking Multimodal Agents for Context-Aware Image Retrieval in Visual Histories**

- **第一作者**：Chenlong Deng
- **年份**：2026
- **Venue**：arXiv 预印本（2026 年 2 月，HuggingFace 59 upvotes）
- **被引数**：未知
- **链接**：[arXiv:2602.10809](https://arxiv.org/abs/2602.10809)，arXiv 2026
- **与本毕设关系**：针对视觉历史流中上下文感知图像检索建立 agentic benchmark，提出模块化 agent + 双记忆系统做多步推理；与本工作 divide-and-conquer + agentic 检索框架在整体结构上最为相近，可用于答辩时说明多步 agentic 检索的合理性。

---

### 3.6 **MC-Search: Evaluating and Enhancing Multimodal Agentic Search with Structured Long Reasoning Chains**

- **第一作者**：Xuying Ning
- **年份**：2026
- **Venue**：arXiv 预印本（2026 年 3 月）
- **被引数**：未知
- **链接**：[arXiv:2603.00873](https://arxiv.org/abs/2603.00873)，arXiv 2026
- **与本毕设关系**：首个针对 agentic 多模态检索增强生成的 benchmark，强调长链推理与步骤级评估（含 verification 步骤）；为本工作 verifier 二次确认设计提供 benchmark 层面的支撑，可引用以说明 verification 在 agentic 检索中的重要性。

---

### 3.7 **Learning to Retrieve from Agent Trajectories**

- **第一作者**：Yuqi Zhou
- **年份**：2026
- **Venue**：arXiv 预印本（2026 年 4 月，HuggingFace 71 upvotes）
- **被引数**：未知
- **链接**：[arXiv:2604.04949](https://arxiv.org/abs/2604.04949)，arXiv 2026
- **与本毕设关系**：从多步 agent 交互轨迹中挖掘监督信号训练检索模型，结合相关强度加权优化；对本工作 agentic verifier 如何与检索阶段协同优化有直接方法启发，也是 2026 年该方向热度最高论文之一。

---

*检索时间：2026 年 6 月。主要数据源：HuggingFace Papers（upvote 作为热度信号）、arXiv、Google Scholar（搜索摘要）、Semantic Scholar（API 限速 403，被引数多数标注「未知」）。所有 arXiv 链接均为已核实的真实链接。如有被引数或 venue 标注不准确，请以 Semantic Scholar / Google Scholar 实时查询结果为准。*
