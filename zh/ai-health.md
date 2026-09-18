---
layout: page
title: AI+医疗健康
description: 本页面介绍我们在人工智能与医疗健康方向的研究。
lang: zh-CN
alternate_url: /ai_health
permalink: /zh/ai-health/
---

## 概览

我们把前沿机器学习技术用于真实医疗问题，希望提升医生和医学研究人员的工作效率。研究涵盖 AI 辅助言语治疗、药物发现、医学影像与临床智能体。

### AI 辅助言语治疗

高鼻音评估直接影响唇腭裂患者后续的手术和言语治疗方案。我们利用大规模通用语音数据预训练自动语音识别模型，再在低资源唇腭裂数据上微调，从而提升自动评估的泛化能力 [Song et al., INTERSPEECH 2022][^1]。我们还提出端到端的 MPA 方法，通过掩码预训练缓解词和音素对齐误差 [Liang et al., INTERSPEECH 2023][^2]。

### AI 药物发现

我们研究药物组合与分子生成。针对三阴性乳腺癌，团队利用 AI 和多组学数据发现诱导细胞焦亡的药物组合 [Ouyang et al., Nature Communications 2024][^3]；针对多目标三维分子生成，我们提出无需额外训练的条件扩散方法 [Han et al., ICLR 2024][^4]。

<p align="center"><img src="/img/health/mudm.png" width="500" alt="多目标分子扩散模型"></p>

### AI、生物学与治疗系统

近期研究从分子生成进一步拓展到生物表征学习与实验设计。我们分离单细胞表征中的因果因素，以支持可控反事实生成 [Gao et al., Nature Communications 2025][^10]；“实验室闭环”框架把机器学习预测与湿实验反馈连接起来，用于设计脑靶向递送系统 [Qiu et al., Cell Biomaterials 2025][^11]；Omni-DNA 则统一支持基因组序列理解、长上下文建模和文本注释 [Li et al., NeurIPS 2025][^12]。

### 医学影像基础模型

UniMedI 以诊断报告作为共同语义空间，为二维和三维医学影像学习统一表示 [He et al., ECCV 2024][^5]。我们还发布 Med-VTAB，用 168 万张医学影像系统评估视觉任务适配方法 [Mo et al., 2024][^6]。

<p align="center"><img src="/img/health/unimedi.png" width="500" alt="UniMedI 医学影像预训练框架"></p>

### 精准诊断与可信临床 AI

在神经系统疾病诊断方面，我们联合适配单模态基础模型，整合多模态证据进行阿尔茨海默病诊断 [Gu et al., ICLR 2026][^7]；COME 框架引入协同元知识，处理跨中心痴呆病因诊断中的数据异质性 [Du et al., TMI 2026][^13]。在精准肿瘤学方面，疾病中心视觉语言基础模型融合病理视觉证据和领域知识，用于肾癌分析 [Tao et al., Nature Communications 2026][^8]。我们还揭示了医疗记录遗忘如何导致临床 AI 的算法不公平，并研究相应缓解方法 [Chen et al., Nature Communications 2026][^14]。

### 临床计算机操作智能体

真实临床工作流需要智能体操作现有软件，而不只是输出预测标签。MedCUA-Bench 面向仅使用屏幕截图的计算机操作智能体，评估其在临床任务中的视觉交互、长程执行与关键工作流能力 [Yu et al., EMNLP 2026 Findings][^9]。

## 参考文献

[^1]: [Kaitao Song et al. Improving Hypernasality Estimation with Automatic Speech Recognition in Cleft Palate Speech. INTERSPEECH 2022.](https://arxiv.org/abs/2208.05122)
[^2]: [Yukang Liang et al. End-to-End Word-Level Pronunciation Assessment with MASK Pre-training. INTERSPEECH 2023.](https://arxiv.org/abs/2306.02682)
[^3]: [Boshu Ouyang et al. AI-powered omics-based drug pair discovery for pyroptosis therapy targeting triple-negative breast cancer. Nature Communications 2024.](https://www.nature.com/articles/s41467-024-51980-9)
[^4]: [Xu Han et al. Training-free Multi-objective Diffusion Model for 3D Molecule Generation. ICLR 2024.](https://openreview.net/forum?id=X41c4uB4k0)
[^5]: [Xiaoxuan He et al. Unified Medical Image Pre-training in Language-Guided Common Semantic Space. ECCV 2024.](https://arxiv.org/abs/2311.14851)
[^6]: [Shentong Mo et al. A Large-scale Medical Visual Task Adaptation Benchmark.](https://arxiv.org/abs/2404.12876)
[^7]: [Wentao Gu et al. Joint Adaptation of Uni-modal Foundation Models for Multi-modal Alzheimer's Disease Diagnosis. ICLR 2026.](https://openreview.net/forum?id=gPTjQxC74G)
[^8]: [Yuhui Tao et al. A disease-centric vision-language foundation model for precision oncology in kidney cancer. Nature Communications 2026.](https://www.nature.com/articles/s41467-026-74175-w)
[^9]: [Jia Yu et al. MedCUA-Bench: A Screenshot-Only Benchmark for Clinical Computer-Use Agents. EMNLP 2026 Findings.](https://openreview.net/forum?id=gC1m98w7cq)

[^10]: [Yicheng Gao et al. Causal disentanglement for single-cell representations and controllable counterfactual generation. Nature Communications 2025.](https://www.nature.com/articles/s41467-025-62008-1)
[^11]: [Qiujun Qiu et al. Lab-in-the-loop Machine Learning for Brain-Targeting Delivery System Design. Cell Biomaterials 2025.](https://www.sciencedirect.com/science/article/pii/S3050562325001217)
[^12]: [Zehui Li et al. Omni-DNA: A Genomic Model Supporting Sequence Understanding, Long-context, and Textual Annotation. NeurIPS 2025.](https://openreview.net/forum?id=qfP6IDxOrA)
[^13]: [Siyuan Du et al. Dementia Etiology Diagnosis via Collaborative Meta Knowledge Enhancement. IEEE Transactions on Medical Imaging 2026.](https://arxiv.org/abs/2607.22770)
[^14]: [Yixuan Chen et al. Mitigating algorithmic unfairness arising from forgetfulness of medical records in clinical artificial intelligence. Nature Communications 2026.](https://www.nature.com/articles/s41467-026-72601-7)