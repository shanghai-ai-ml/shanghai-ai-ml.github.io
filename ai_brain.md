---
layout: page
title: AI+Brain
description: This page introduces our research works about AI and Brain.
---

## Overview

We work on the interdisciplinary research between AI and the brain, with the goal of using AI to enhance our understanding of the brain and applying these insights to improve both AI and brain health.


<figure>
    <p align="center">
        <img src="/img/ai_brain/ai_brain_overview.png" width="500">
    </p>
</figure>

### Brain-inspired AI

- **Spiking neural networks**: We aim to make the performance of spiking neural networks to be competitive to their ANN counterparts.
  - we proposed a framework for SNNs in time-series forecasting tasks, leveraging the efficiency of spiking neurons in processing temporal information, which can achieve comparable or superior results to traditional time-series forecasting methods on diverse benchmarks with much less energy consumption [Lv et al., ICML 2024][^1].
    <div id="image-table" align="center">
        <table>
    	    <tr>
        	    <td style="padding:5px">
            	    <img src="/img/ai_brain/SeqSNN_overview.png" height="160">
          	    </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/SeqSNN_result_energy.png" height="160">
                </td>
            </tr>
        </table>
    </div>
  - We proposed a novel position encoding (PE) technique for SNNs, termed CPG-PE, by drawing inspiration from the central pattern generators (CPGs) in the human brain, which produce rhythmic patterned outputs without requiring rhythmic inputs. Extensive experiments across various domains, including time-series forecasting, natural language processing, and image classification, show that SNNs with CPG-PE outperform their conventional counterparts [Lv et al., NeurIPS 2024][^2].
    <div id="image-table" align="center">
        <table>
    	    <tr>
        	    <td style="padding:5px">
            	    <img src="/img/ai_brain/CPG.png" height="125">
          	    </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/CPG_SNN.png" height="125">
                </td>
            </tr>
        </table>
    </div>
- **brain-inspired neural networks**: We design new neural network architectures by mimicking the biological neural networks, aiming to improve the learning/parameter efficiency of ANNs.
  - We proposed a new type of neural network inspired by the architectures of neuronal circuits, namely Circuit Neural Network (CircuitNet). Compared with traditional feed-forward networks, CircuitNet has the ability to model more types of neuron connections such as feed-back and lateral motifs. Experiments have demonstrated that CircuitNet can outperform popular neural network architectures in function approximation, reinforcement learning, image classification, and time series forecasting tasks [Wang et al., ICML 2023][^3].
    <div id="image-table" align="center">
        <table>
    	    <tr>
        	    <td style="padding:5px">
            	    <img src="/img/ai_brain/CircuitNet_overview.png" height="130">
          	    </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/CircuitNet_ts_acc.png" height="130">
                </td>
            </tr>
        </table>
    </div>
- **brain-inspired algorithms**: We design new algorithms to mimic the complex behaviors of human, aiming to understand the mechanism of human decision-making.
  - We introduce a theoretical framework using variational Bayesian theory, incorporating a Bayesian "intention" variable. Habitual behavior depends on the prior distribution of intention, computed from sensory context without goal-specification. In contrast, goal-directed behavior relies on the goal-conditioned, posterior distribution of intention, inferred through variational free energy minimization. Our work suggests a fresh perspective on the neural mechanisms of habits and goals, shedding light on future research in decision-making [Han et al., Nature Communications 2024][^4].
    <div id="image-table" align="center">
        <table>
    	    <tr>
        	    <td style="padding:5px">
            	    <img src="/img/ai_brain/NC_figure_1.png" height="200">
          	    </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/NC_figure_2.png" height="200">
                </td>
            </tr>
        </table>
    </div>
  - Signal delay occurs when there is a lag between an agent’s perception of the environment and its corresponding actions. We formalize delayed-observation Markov decision processes (DOMDP) by extending the standard MDP framework to incorporate signal delays. Next, we elucidate the challenges posed by the presence of signal delay in DRL, showing that trivial DRL algorithms and generic methods for partially observable tasks suffer greatly from delays. Lastly, we propose effective strategies to overcome these challenges [Wang et al., ICLR 2024 Spotlight][^5]. Project repository: <https://github.com/microsoft/Addressing-signal-delay-in-deep-RL>.

    <div id="image-table" align="center">
        <table>
    	    <tr>
        	    <td style="padding:5px">
            	    <img src="/img/ai_brain/DRLwD_overview.png" height="125">
          	    </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/DRLwD_method.png" height="125">
                </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/DRLwD_result.png" height="125">
                </td>
            </tr>
        </table>
    </div>

### Brain-computer Interface

- **EEG Signal Processing**: We develop pretraining techniques for EEG signals, aiming to better understand EEG signals from large-scale unlabeled data.
  - We proposed one of earliest EEG foundation model, which can consistently improve the performance of EEG-related downstream tasks. To break boundaries between different EEG resources and facilitate cross-dataset EEG pre-training, we propose to map all kinds of channel selections to a unified topology. We further introduce MMM, a pre-training framework with Multi-dimensional position encoding, Multi-level channel hierarchy, and Multi-stage pre-training strategy built on the unified topology to obtain topology-agnostic representations [Yi et al., NeurIPS 2023][^6].
    <div id="image-table" align="center">
        <table>
    	    <tr>
        	    <td style="padding:5px">
            	    <img src="/img/ai_brain/MMM_overview.png" height="150">
          	    </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/MMM_result.png" height="150">
                </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/MMM_reconstruct.png" height="150">
                </td>
            </tr>
        </table>
    </div>

  - We proposed NeuroLM, the first multi-task foundation model that leverages the capabilities of Large Language Models (LLMs) by regarding EEG signals as a foreign language, endowing the model with multi-task learning and inference capabilities. The largest variant NeuroLM-XL has record-breaking 1.7B parameters for EEG signal processing, and is pre-trained on a large-scale corpus comprising approximately 25,000-hour EEG data. When evaluated on six diverse downstream datasets, NeuroLM showcases the huge potential of this multi-task learning paradigm [Jiang et al., arXiv 2024][^9].
    <div id="image-table" align="center">
        <table>
    	    <tr>
        	    <td style="padding:5px">
            	    <img src="/img/ai_brain/NeuroLM_model.png" height="200">
          	    </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/NeuroLM_result.png" height="200">
                </td>
            </tr>
        </table>
    </div>
- **EEG-based Applications**: We improve the performance of EEG-based BCI applications by combing EEG foundation models and advanced machine learning techniques.
  - We improve the performance of neonatal seizure detection by proposing a deep learning framework, namely STATENet, to address the exclusive challenges with exquisite designs at the temporal, spatial and model levels. The experiments over the real-world large-scale neonatal EEG dataset illustrate that our framework achieves significantly better seizure detection performance [Li et al., SMC 2023][^7].
    <div id="image-table" align="center">
        <table>
    	    <tr>
        	    <td style="padding:5px">
            	    <img src="/img/ai_brain/StateNet_motivation_1.png" height="150">
          	    </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/StateNet_motivation_2.png" height="150">
                </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/StateNet_result.png" height="150">
                </td>
            </tr>
        </table>
    </div>
- **The PhysioPro Project**: PhysioPro is a deep learning framework for physiological data processing and understanding, which contains most of our EEG related work <https://github.com/microsoft/PhysioPro>.
> **_NOTE:_** This code base should not be used in clinical settings.

### Embodied AI

- **Open-ended Tasks Solving**: A major challenge in embodied agents is task open-endedness. In practice, robots often need to perform tasks with novel goals that are multifaceted, dynamic, lack a definitive "end-state", and were not encountered during training. To tackle this problem, this paper introduces *Diffusion for Open-ended Goals* (DOG), a novel framework designed to enable embodied AI to plan and act flexibly and dynamically for open-ended task goals [Wang et al., NeurIPS Workshop 2023][^8].
    <div id="image-table" align="center">
        <table>
    	    <tr>
        	    <td style="padding:5px">
            	    <img src="/img/ai_brain/DOG_1.png" height="180">
          	    </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/DOG_2.png" height="180">
                </td>
            </tr>
        </table>
    </div>

- **More Effective Diffusion Planner**: In this work, we address this issue through systematic empirical experiments on diffusion planning in an offline reinforcement learning (RL) setting, providing practical insights into the essential components of diffusion planning. We trained and evaluated over 6,000 diffusion models, identifying the critical components such as guided sampling, network architecture, action generation and planning strategy. We revealed that some design choices opposite to the common practice in previous work in diffusion planning actually lead to better performance, e.g., unconditional sampling with selection can be better than guided sampling and Transformer outperforms U-Net as denoising network. Based on these insights, we suggest a simple yet strong diffusion planning baseline that achieves state-of-the-art results on standard offline RL benchmarks [Lu et al., ICLR 2025 (Spotlight)][^10].

    <div id="image-table" align="center">
        <table>
    	    <tr>
        	    <td style="padding:5px">
            	    <img src="/img/ai_brain/dv_overview.png" height="180">
          	    </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/dv_result.png" height="180">
                </td>
            </tr>
        </table>
    </div>

- **More Effecient Generative Planner**: Diffusion models have shown great promise in decision-making, also known as diffusion planning. However, the slow inference speeds limit their potential for broader real-world applications. Here, we introduce Habi, a general framework that transforms powerful but slow diffusion planning models into fast decision-making models, which mimics the cognitive process in the brain that costly goal-directed behavior gradually transitions to efficient habitual behavior with repetitive practice. Even using a laptop CPU, the habitized model can achieve an average 800+ Hz decision-making frequency (faster than previous diffusion planners by orders of magnitude) on standard offline reinforcement learning benchmarks D4RL, while maintaining comparable or even higher performance compared to its corresponding diffusion planner. [Lu et al., arXiv 2025][^11].

    <div id="image-table" align="center">
        <table>
    	    <tr>
        	    <td style="padding:5px">
            	    <img src="/img/ai_brain/habi_overview.png" height="180">
          	    </td>
                <td style="padding:5px">
                	<img src="/img/ai_brain/habi_result.png" height="180">
                </td>
            </tr>
        </table>
    </div>




## Reference

[^1]: [Changze Lv, Yansen Wang, Dongqi Han, Xiaoqing Zheng, Xuanjing Huang, Dongsheng Li. Efficient and Effective Time-Series Forecasting with Spiking Neural Networks. ICML 2024.](https://arxiv.org/abs/2402.01533)

[^2]: [Changze Lv, Dongqi Han, Yansen Wang, Xiaoqing Zheng, Xuanjing Huang, Dongsheng Li. Advancing Spiking Neural Networks for Sequential Modeling with Central Pattern Generators. NeurIPS 2024. (Spotlight)](https://arxiv.org/abs/2405.14362)

[^3]: [Yansen Wang, Xinyang Jiang, Kan Ren, Caihua Shan, Xufang Luo, Dongqi Han, Kaitao Song, Yifei Shen, Dongsheng Li. CircuitNet: A Generic Neural Network to Realize Universal Circuit Motif Modeling. ICML 2023.](https://proceedings.mlr.press/v202/wang23k.html)

[^4]: [Dongqi Han, Kenji Doya, Dongsheng Li, Jun Tani. Synergizing habits and goals with variational Bayes. Nature Communications, volume 15, Article number: 4461 (2024).](https://www.nature.com/articles/s41467-024-48577-7)

[^5]: [Wei Wang, Dongqi Han, Xufang Luo, Dongsheng Li. Addressing Signal Delay in Deep Reinforcement Learning. ICLR 2024. (Spotlight)](https://openreview.net/forum?id=Z8UfDs4J46)

[^6]: [Ke Yi, Yansen Wang, Kan Ren, Dongsheng Li. Learning Topology-Agnostic EEG Representations with Geometry-Aware Modeling. NeurIPS 2023.](https://proceedings.neurips.cc/paper_files/paper/2023/hash/a8c893712cb7858e49631fb03c941f8d-Abstract-Conference.html)

[^7]: [Ziyue Li, Yuchen Fang, You Li, Kan Ren, Yansen Wang, Xufang Luo, Juanyong Duan, Congrui Huang, Dongsheng Li, Lili Qiu. Protecting the Future: Neonatal Seizure Detection with Spatial-Temporal Modeling. IEEE SMC 2023.](https://arxiv.org/abs/2307.05382)

[^8]: [William Wei Wang, Dongqi Han, Xufang Luo, Yifei Shen, Charles Ling, Boyu Wang, Dongsheng Li. Toward Open-ended Embodied Tasks Solving. Second Agent Learning in Open-Endedness Workshop, NeurIPS 2023.](https://arxiv.org/abs/2312.05822)

[^9]: [Wei-Bang Jiang, Yansen Wang, Bao-Liang Lu, Dongsheng Li. NeuroLM: A Universal Multi-task Foundation Model for Bridging the Gap between Language and EEG Signals, arXiv:2409.00101 2024.](https://arxiv.org/abs/2409.00101)

[^10]: [Haofei Lu, Dongqi Han, Yifei Shen, Dongsheng Li. What Makes a Good Diffusion Planner for Decision Making? ICLR 2025 (Spotlight)](https://openreview.net/forum?id=7BQkXXM8Fy)

[^11]: [Haofei Lu, Yifei Shen, Dongsheng Li, Junliang Xing, Dongqi Han. Habitizing Diffusion Planning for Efficient and Effective Decision Making. arXiv:2502.06401](https://arxiv.org/abs/2502.06401)
