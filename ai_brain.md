---
layout: page
title: AI + Brain
description: This page introduces our research works about AI and Brain.
---

We work on the interdisciplinary research between AI and the brain, with the goal of using AI to enhance our understanding of the brain and applying these insights to improve both AI and brain health.


<figure>
    <p align="center">
        <img src="/img/ai_brain/ai_brain_overview.png" width="500">
    </p>
</figure>

## Brain-inspired AI

- **Spiking neural networks**: We aim to make the performance of spiking neural networks to be competitive to their ANN counterparts.
  - we proposed a framework for SNNs in time-series forecasting tasks, leveraging the efficiency of spiking neurons in processing temporal information, which can achieve comparable or superior results to traditional time-series forecasting methods on diverse benchmarks with much less energy consumption [Lv et al., ICML 2024][1].
    <figure>
        <p align="center">
            <img src="/img/ai_brain/SeqSNN_overview.png" height="125">
            <img src="/img/ai_brain/SeqSNN_result_energy.png" height="125">
        </p>
    </figure>
  - We proposed a novel position encoding (PE) technique for SNNs, termed CPG-PE, by drawing inspiration from the central pattern generators (CPGs) in the human brain, which produce rhythmic patterned outputs without requiring rhythmic inputs. Extensive experiments across various domains, including time-series forecasting, natural language processing, and image classification, show that SNNs with CPG-PE outperform their conventional counterparts [Lv et al., arXiv 2024][2].

- **brain-inspired neural networks**: We design new neural network architectures by mimicking the biological neural networks, aiming to improve the learning/parameter efficiency of ANNs.
  - We proposed a new type of neural network inspired by the architectures of neuronal circuits, namely Circuit Neural Network (CircuitNet). Compared with traditional feed-forward networks, CircuitNet has the ability to model more types of neuron connections such as feed-back and lateral motifs. Experiments have demonstrated that CircuitNet can outperform popular neural network architectures in function approximation, reinforcement learning, image classification, and time series forecasting tasks [Wang et al., ICML 2023][3].
  
- **brain-inspired algorithms**: We design new algorithms to mimic the complex behaviors of human, aiming to understand the mechanism of human decision-making.
  - We introduce a theoretical framework using variational Bayesian theory, incorporating a Bayesian "intention" variable. Habitual behavior depends on the prior distribution of intention, computed from sensory context without goal-specification. In contrast, goal-directed behavior relies on the goal-conditioned, posterior distribution of intention, inferred through variational free energy minimization. Our work suggests a fresh perspective on the neural mechanisms of habits and goals, shedding light on future research in decision-making [Han et al., Nature Communications 2024][4].
  - Signal delay occurs when there is a lag between an agent’s perception of the environment and its corresponding actions. We formalize delayed-observation Markov decision processes (DOMDP) by extending the standard MDP framework to incorporate signal delays. Next, we elucidate the challenges posed by the presence of signal delay in DRL, showing that trivial DRL algorithms and generic methods for partially observable tasks suffer greatly from delays. Lastly, we propose effective strategies to overcome these challenges [Wang et al., ICLR 2024 Spotlight][5].

## Brain-computer Interface

- **EEG Signal Processing**: We develop pretraining techniques for EEG signals, aiming to better understand EEG signals from large-scale unlabeled data.
  - We proposed one of earliest EEG foundation model, which can consistently improve the performance of EEG-related downstream tasks. To break boundaries between different EEG resources and facilitate cross-dataset EEG pre-training, we propose to map all kinds of channel selections to a unified topology. We further introduce MMM, a pre-training framework with Multi-dimensional position encoding, Multi-level channel hierarchy, and Multi-stage pre-training strategy built on the unified topology to obtain topology-agnostic representations [Yi et al., NeurIPS 2023][6].

- **EEG-based Applications**: We improve the performance of EEG-based BCI applications by combing EEG foundation models and advanced machine learning techniques.
  - We improve the performance of neonatal seizure detection by proposing a deep learning framework, namely STATENet, to address the exclusive challenges with exquisite designs at the temporal, spatial and model levels. The experiments over the real-world large-scale neonatal EEG dataset illustrate that our framework achieves significantly better seizure detection performance [Li et al., SMC 2023][7].

- **The PhysioPro Project**: PhysioPro is a deep learning framework for physiological data processing and understanding, which contains most of our EEG related work <https://github.com/microsoft/PhysioPro>. Note that this code should not be used in clinical settings to influence treatment decisions.

## Embodied AI

- **Open-ended Tasks Solving**: A major challenge in embodied agents is task open-endedness. In practice, robots often need to perform tasks with novel goals that are multifaceted, dynamic, lack a definitive "end-state", and were not encountered during training. To tackle this problem, this paper introduces *Diffusion for Open-ended Goals* (DOG), a novel framework designed to enable embodied AI to plan and act flexibly and dynamically for open-ended task goals [Wang et al., NeurIPS Workshop 2023][8]. 

## Reference

[1]: Changze Lv, Yansen Wang, Dongqi Han, Xiaoqing Zheng, Xuanjing Huang, Dongsheng Li. Efficient and Effective Time-Series Forecasting with Spiking Neural Networks. ICML 2024. <https://arxiv.org/abs/2402.01533>

[2]: Changze Lv, Dongqi Han, Yansen Wang, Xiaoqing Zheng, Xuanjing Huang, Dongsheng Li. Advancing Spiking Neural Networks for Sequential Modeling with Central Pattern Generators. arXiv 2024. <https://arxiv.org/abs/2405.14362>

[3]: Yansen Wang, Xinyang Jiang, Kan Ren, Caihua Shan, Xufang Luo, Dongqi Han, Kaitao Song, Yifei Shen, Dongsheng Li. CircuitNet: A Generic Neural Network to Realize Universal Circuit Motif Modeling. ICML 2023. <https://proceedings.mlr.press/v202/wang23k.html>

[4]: Dongqi Han, Kenji Doya, Dongsheng Li, Jun Tani. Synergizing habits and goals with variational Bayes. Nature Communications, volume 15, Article number: 4461 (2024). <https://www.nature.com/articles/s41467-024-48577-7>

[5]: Wei Wang, Dongqi Han, Xufang Luo, Dongsheng Li. Addressing Signal Delay in Deep Reinforcement Learning. ICLR 2024 spotlight. <https://openreview.net/forum?id=Z8UfDs4J46>

[6]: Ke Yi, Yansen Wang, Kan Ren, Dongsheng Li. Learning Topology-Agnostic EEG Representations with Geometry-Aware Modeling. NeurIPS 2023. <https://proceedings.neurips.cc/paper_files/paper/2023/hash/a8c893712cb7858e49631fb03c941f8d-Abstract-Conference.html>

[7]: Ziyue Li, Yuchen Fang, You Li, Kan Ren, Yansen Wang, Xufang Luo, Juanyong Duan, Congrui Huang, Dongsheng Li, Lili Qiu. Protecting the Future: Neonatal Seizure Detection with Spatial-Temporal Modeling. IEEE SMC 2023. <https://arxiv.org/abs/2307.05382>

[8]: William Wei Wang, Dongqi Han, Xufang Luo, Yifei Shen, Charles Ling, Boyu Wang, Dongsheng Li. Toward Open-ended Embodied Tasks Solving. Second Agent Learning in Open-Endedness Workshop, NeurIPS 2023. <https://arxiv.org/abs/2312.05822>
