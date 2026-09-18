---
layout: page
title: AI+脑科学
description: 本页面介绍我们在人工智能与脑科学交叉方向的研究。
lang: zh-CN
alternate_url: /ai_brain
permalink: /zh/ai-brain/
---

## 概览

我们开展人工智能与脑科学的交叉研究：一方面借助 AI 加深对大脑的理解，另一方面把脑科学中的机制用于改进人工智能与脑健康。

<figure>
    <p align="center">
        <img src="/img/ai_brain/ai_brain_overview.png" width="500" alt="AI 与脑科学研究概览">
    </p>
</figure>

### 类脑人工智能

- **脉冲神经网络**：我们致力于缩小脉冲神经网络与传统人工神经网络之间的性能差距。SeqSNN 利用脉冲神经元处理时序信息的高效性，在多个时间序列预测基准上以更低能耗获得相当或更优的效果 [Lv et al., ICML 2024][^1]。CPG-PE 借鉴大脑中央模式发生器，在时序预测、自然语言处理和图像分类任务中提升了脉冲神经网络性能 [Lv et al., NeurIPS 2024 Spotlight][^2]。
- **类脑网络架构**：CircuitNet 模拟神经回路中的前馈、反馈和侧向连接，在函数逼近、强化学习、图像分类及时间序列预测任务中展现出通用性 [Wang et al., ICML 2023][^3]。2026 年，我们进一步提出基于 Kuramoto 振荡同步的相位编码 KoPE，以提升视觉模型的训练、参数和数据效率 [Xiao et al., ICML 2026][^4]。
- **类脑算法**：我们通过变分贝叶斯框架统一描述习惯性与目标导向行为 [Han et al., Nature Communications 2024][^5]，并系统研究扩散规划器的关键设计 [Lu et al., ICLR 2025 Spotlight][^6]。

<p align="center"><img src="/img/ai_brain/CPG_SNN.png" width="500" alt="CPG-PE 脉冲神经网络"></p>

### 脑机接口

- **脑电信号基础模型**：我们提出面向跨数据集脑电预训练的统一拓扑和 MMM 框架 [Yi et al., NeurIPS 2023][^7]。NeuroLM 将脑电信号视作一种“外语”，利用大语言模型实现多任务脑电理解 [Jiang et al., ICLR 2025][^8]。
- **脑电应用**：STATENet 面向真实大规模新生儿脑电数据，在时间、空间和模型层面共同建模癫痫发作 [Li et al., SMC 2023][^9]；SimSort 利用大规模电生理仿真推动数据驱动的神经尖峰分类 [Zhang et al., NeurIPS 2025][^10]。
- **PhysioPro**：我们的生理数据深度学习框架汇集了多项脑电研究，代码见 [microsoft/PhysioPro](https://github.com/microsoft/PhysioPro)。该代码库不可用于临床诊疗。

<p align="center"><img src="/img/ai_brain/NeuroLM_model.png" width="500" alt="NeuroLM 模型"></p>

### 具身智能与决策

面对目标开放、状态动态且训练阶段未曾出现的任务，我们研究能够灵活规划和行动的智能体。DOG 面向开放目标生成动态计划；Habi 则把性能强但推理较慢的扩散规划器“习惯化”为快速决策模型，在标准离线强化学习基准上实现 800 Hz 以上的决策频率 [Lu et al., ICML 2025][^11]。

<p align="center"><img src="/img/ai_brain/habi_overview.png" width="500" alt="Habi 扩散规划框架"></p>

## 近期研究（2025-2026）

### 神经形态与类脑学习

近期研究从时间结构、神经动力学和生物同步机制三个层面推进类脑模型。我们为脉冲 Transformer 提出相对位置编码 [Lv et al., NeurIPS 2025 Spotlight][^12]，并提出无需传统反向传播的在线伪零阶神经形态训练方法 [Xiao et al., ICLR 2026][^13]。在非脉冲模型上，KoPE 利用 Kuramoto 振荡同步提升视觉模型的训练、参数和数据效率 [Xiao et al., ICML 2026][^4]。我们还研究持续学习中保持网络可塑性的架构机制 [Koeppe et al., ICML 2026][^14]，以及能够切换神经编码策略、平衡计算代价与性能的稳定超线性网络 [Wang et al., ICML 2026][^15]。

### 神经数据与人类行为理解

我们把计算模型与神经及行为数据结合。SimSort 基于大规模电生理仿真构建数据驱动的神经尖峰分类框架 [Zhang et al., NeurIPS 2025][^10]；EgoBrain 协同建模第一视角视觉观察与认知信号，用于理解人类行为 [Lin et al., ICLR 2026][^16]。

### 自适应决策

在扩散规划研究的基础上，我们利用能量函数进行自监督动作门控，提升扩散规划器的动作质量与效率 [Lu et al., ICML 2026][^17]，进一步连接灵活的目标导向规划与高效自适应行为。

## 参考文献

[^1]: [Changze Lv et al. Efficient and Effective Time-Series Forecasting with Spiking Neural Networks. ICML 2024.](https://arxiv.org/abs/2402.01533)
[^2]: [Changze Lv et al. Advancing Spiking Neural Networks for Sequential Modeling with Central Pattern Generators. NeurIPS 2024 Spotlight.](https://arxiv.org/abs/2405.14362)
[^3]: [Yansen Wang et al. CircuitNet: A Generic Neural Network to Realize Universal Circuit Motif Modeling. ICML 2023.](https://proceedings.mlr.press/v202/wang23k.html)
[^4]: [Mingqing Xiao et al. Kuramoto Oscillatory Phase Encoding: Neuro-inspired Synchronization for Improved Learning Efficiency. ICML 2026.](https://openreview.net/forum?id=1rSqVUl7l3)
[^5]: [Dongqi Han et al. Synergizing habits and goals with variational Bayes. Nature Communications 2024.](https://www.nature.com/articles/s41467-024-48577-7)
[^6]: [Haofei Lu et al. What Makes a Good Diffusion Planner for Decision Making? ICLR 2025 Spotlight.](https://openreview.net/forum?id=7BQkXXM8Fy)
[^7]: [Ke Yi et al. Learning Topology-Agnostic EEG Representations with Geometry-Aware Modeling. NeurIPS 2023.](https://proceedings.neurips.cc/paper_files/paper/2023/hash/a8c893712cb7858e49631fb03c941f8d-Abstract-Conference.html)
[^8]: [Weibang Jiang et al. NeuroLM: A Universal Multi-task Foundation Model for Bridging the Gap between Language and EEG Signals. ICLR 2025.](https://openreview.net/forum?id=Io9yFt7XH7)
[^9]: [Ziyue Li et al. Protecting the Future: Neonatal Seizure Detection with Spatial-Temporal Modeling. IEEE SMC 2023.](https://arxiv.org/abs/2307.05382)
[^10]: [Yimu Zhang et al. SimSort: A Data-Driven Framework for Spike Sorting by Large-Scale Electrophysiology Simulation. NeurIPS 2025.](https://openreview.net/forum?id=IwjkwtkPGb)
[^11]: [Haofei Lu et al. Habitizing Diffusion Planning for Efficient and Effective Decision Making. ICML 2025.](https://arxiv.org/abs/2502.06401)

[^12]: [Changze Lv et al. Toward Relative Positional Encoding in Spiking Transformers. NeurIPS 2025 Spotlight.](https://openreview.net/forum?id=MDWJlTWZHH)
[^13]: [Mingqing Xiao et al. Online Pseudo-Zeroth-Order Training of Neuromorphic Spiking Neural Networks. ICLR 2026.](https://openreview.net/forum?id=6ZietpbPoB)
[^14]: [Niklas Koeppe et al. Mitigating Plasticity Loss through Architectural Design in Continual Learning. ICML 2026.](https://openreview.net/forum?id=pAhGjPOlwy)
[^15]: [Haoyu Albert Wang et al. Stabilized Supralinear Networks Learn to Switch Coding Strategies Balancing Cost and Performance. ICML 2026.](https://openreview.net/forum?id=fPX6A4us61)
[^16]: [Nie Lin et al. EgoBrain: Synergizing Minds and Eyes For Human Action Understanding. ICLR 2026.](https://openreview.net/forum?id=DGcoJINQ7P)
[^17]: [Yuan Lu et al. Improving Diffusion Planners by Self-Supervised Action Gating with Energies. ICML 2026.](https://openreview.net/forum?id=tLW4Tc7Zn9)