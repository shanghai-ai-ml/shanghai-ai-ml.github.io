---
layout: page
title: AI + Brain
description: This page introduces our research works about AI and Brain.
---

We work on the interdisciplinary research between AI and the brain, with the goal of using AI to enhance our understanding of the brain and applying these insights to improve both AI and brain health.

![The overview of two researcb direction!](/img/ai_brain_overview.png "AI + Brain Research Overview")

## Brain-inspired AI

- **Spiking neural networks**: We aim to make the performance of spiking neural networks to be competitive to their ANN counterparts.
  - we proposed a framework for SNNs in time-series forecasting tasks, leveraging the efficiency of spiking neurons in processing temporal information, which can achieve comparable or superior results to traditional time-series forecasting methods on diverse benchmarks with much less energy consumption [Lv et al., ICML 2024][1].
  - We proposed a novel position encoding (PE) technique for SNNs, termed CPG-PE, by drawing inspiration from the central pattern generators (CPGs) in the human brain, which produce rhythmic patterned outputs without requiring rhythmic inputs. Extensive experiments across various domains, including time-series forecasting, natural language processing, and image classification, show that SNNs with CPG-PE outperform their conventional counterparts [Lv et al., arXiv 2024][2].

- **brain-inspired neural networks**: We design new neural network architectures by mimicking the biological neural networks, aiming to improve the learning/parameter efficiency of ANNs.
  - We proposed a new type of neural network inspired by the architectures of neuronal circuits, namely Circuit Neural Network (CircuitNet). Compared with traditional feed-forward networks, CircuitNet has the ability to model more types of neuron connections such as feed-back and lateral motifs. Experiments have demonstrated that CircuitNet can outperform popular neural network architectures in function approximation, reinforcement learning, image classification, and time series forecasting tasks [Wang et al., ICML 2023][3].
  
- **brain-inspired algorithms**: We design new algorithms to mimic the complex behaviors of human, aiming to understand the mechanism of human decision-making.
  - We introduce a theoretical framework using variational Bayesian theory, incorporating a Bayesian "intention" variable. Habitual behavior depends on the prior distribution of intention, computed from sensory context without goal-specification. In contrast, goal-directed behavior relies on the goal-conditioned, posterior distribution of intention, inferred through variational free energy minimization. Our work suggests a fresh perspective on the neural mechanisms of habits and goals, shedding light on future research in decision-making [Han et al., Nature Communications 2024][4].

## Brain-computer Interface



## Embodied AI


## Reference

[1]: Changze Lv, Yansen Wang, Dongqi Han, Xiaoqing Zheng, Xuanjing Huang, Dongsheng Li. Efficient and Effective Time-Series Forecasting with Spiking Neural Networks. ICML 2024. <https://arxiv.org/abs/2402.01533>

[2]: Changze Lv, Dongqi Han, Yansen Wang, Xiaoqing Zheng, Xuanjing Huang, Dongsheng Li. Advancing Spiking Neural Networks for Sequential Modeling with Central Pattern Generators. arXiv 2024. <https://arxiv.org/abs/2405.14362>

[3]: Yansen Wang, Xinyang Jiang, Kan Ren, Caihua Shan, Xufang Luo, Dongqi Han, Kaitao Song, Yifei Shen, Dongsheng Li. CircuitNet: A Generic Neural Network to Realize Universal Circuit Motif Modeling. ICML 2023. <https://proceedings.mlr.press/v202/wang23k.html>

[4]: Dongqi Han, Kenji Doya, Dongsheng Li, Jun Tani. Synergizing habits and goals with variational Bayes. Nature Communications, volume 15, Article number: 4461 (2024). <https://www.nature.com/articles/s41467-024-48577-7>
