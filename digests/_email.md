2026-06-29 新增 8 篇，已按顶会/高赞优先排序

---

## 方向一：VPR / 视觉位置识别 / 视觉地理定位（2 篇）

### 1. **Unifying UAV Cross-View Geo-Localization via 3D Geometric Perception**

作者：Haoyuan Li, Wen Yang, Fang Xu, Hong Tan, Haijian Zhang, Shengyang Li, Gui-Song Xia

arXiv:[2604.01747](https://arxiv.org/abs/2604.01747)(2026-04-02)

`[热度:未知]`

提出几何感知的无人机地理定位框架，使用 VGGT 从多视角无人机图像重建 3D 场景并渲染 BEV 对齐卫星图，统一地点检索与姿态估计两个子任务；同步发布重标注 University-1652 数据集。

---

### 2. **Scale-Aware UAV-to-Satellite Cross-View Geo-Localization: A Semantic Geometric Approach**

作者：Yibin Ye, Shuo Chen, Kun Wang, Xiaokai Song, Jisheng Dang, Qifeng Yu, Xichao Teng, Zhang Li

arXiv:[2603.07535](https://arxiv.org/abs/2603.07535)(2026-03-08)

`[热度:未知]`

以小型车辆为语义锚点从单目无人机图像恢复绝对真实尺度，配合解耦立体投影模型解决无人机图像尺度不确定性问题，在 DenseUAV 和 UAV-VisLoc 数据集上显著提升未知尺度下的跨视图定位鲁棒性。

---

## 方向二：Agent 做检索 / Agentic RAG（2 篇）

### 3. **CriticSearch: Fine-Grained Credit Assignment for Search Agents via a Retrospective Critic**

作者：Yaocheng Zhang, Haohuan Huang, Zijun Song, Yuanheng Zhu, Qichao Zhang, Zijie Zhao, Dongbin Zhao

arXiv:[2511.12159](https://arxiv.org/abs/2511.12159)(2025-11-15)

`[热度:未知]`

引入事后批评（retrospective critic）机制，在完整轨迹可见时对每个工具调用 turn 给出密集的过程级反馈，为 RL 训练搜索 Agent 提供细粒度信用分配，多跳推理任务上收敛更快、准确率更高。

---

### 4. **AI-SearchPlanner: Modular Agentic Search via Pareto-Optimal Multi-Objective Reinforcement Learning**

作者：Lang Mei, Zhihan Yang, Chong Chen

arXiv:[2508.20368](https://arxiv.org/abs/2508.20368)(2025-08-28)

`[热度:未知]`

将搜索规划从 QA 模型中解耦，提出即插即用的搜索规划模块，利用双重奖励对齐与 Pareto 多目标优化训练，辅助各类冻结 QA 模型实现更高效检索，显著提升多跳检索性能。

---

## 方向三：Agent 做图像检索（1 篇）

### 5. **Chain-of-Thought Re-ranking for Image Retrieval Tasks**

作者：Shangrong Wu, Yanghong Zhou, Yang Chen, Feng Zhang, P. Y. Mok

arXiv:[2509.14746](https://arxiv.org/abs/2509.14746)(2025-09-18)

`[GitHub: freshfish15/CoTRR]`

提出 CoTRR，利用 MLLM 链式思维推理进行列表级图像重排序，设计图像评估 prompt 支持全局比较与可解释决策，覆盖文本-图像检索、组合图像检索和对话式图像检索三类任务。

---

## 方向四：Agent 做细粒度检索 / 组合图像检索（3 篇）

### 6. **QuRe: Query-Relevant Retrieval through Hard Negative Sampling in Composed Image Retrieval**

作者：Jaehyun Kwak, Ramahdani Muhammad Izaaz Inhar, Se-Young Yun, Sung-Ju Lee

arXiv:[2507.12416](https://arxiv.org/abs/2507.12416)(2025-07-16,ICML 2025)

`[ICML 2025]`

指出 CIR 对比学习中假负例问题，引入奖励模型目标和硬负例采样策略，有效过滤假负例，在 FashionIQ 和 CIRR 上超越 SOTA，已收录 ICML 2025。

---

### 7. **A Sanity Check on Composed Image Retrieval**

作者：Yikun Liu, Jiangchao Yao, Weidi Xie, Yanfeng Wang

arXiv:[2604.12904](https://arxiv.org/abs/2604.12904)(2026-04-14)

`[热度:未知]`

揭示现有 CIR benchmark 的不确定查询问题，提出 FISD benchmark 精确控制六维评估维度，并设计自动多轮 agentic 评估框架探究现有模型潜力上限。

---

### 8. **MCoT-RE: Multi-Faceted Chain-of-Thought and Re-Ranking for Training-Free Zero-Shot Composed Image Retrieval**

作者：Jeong-Woo Park, Seong-Whan Lee

arXiv:[2507.12819](https://arxiv.org/abs/2507.12819)(2025-07-17)

`[热度:未知]`

无需训练的零样本 CIR 框架，利用 MLLM 多面向 CoT 生成修改聚焦描述（过滤候选）与视觉-文本整合描述（重排序），在 FashionIQ R@10 和 CIRR R@1 上分别提升 6.24% 和 8.58%。
