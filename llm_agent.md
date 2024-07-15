---
layout: page
title: AI+Agent
description: This page introduces our research works about LLM-based Agents.
---

## Overview
In this project, we leverage natural Language as an interface for LLMs to connect numerous AI models for solving complicated AI tasks! We introduce a collaborative system that consists of **an LLM as the controller** and **numerous expert models as collaborative executors** (e.g., from HuggingFace Hub). The workflow of our system consists of four stages:
+ **Task Planning**: Using ChatGPT to analyze the requests of users to understand their intention, and disassemble them into possible solvable tasks.
+ **Model Selection**: To solve the planned tasks, ChatGPT selects expert models hosted on Hugging Face based on their descriptions.
+ **Task Execution**: Invokes and executes each selected model, and return the results to ChatGPT.
+ **Response Generation**: Finally, using ChatGPT to integrate the prediction of all models, and generate responses.

<p align="center"><img src="./img/agent/overview.jpg" width = "500"></p>

## Open-source Project
The source code of this project can be found by [https://github.com/microsoft/JARVIS](https://github.com/microsoft/JARVIS). The mission of JARVIS is to explore artificial general intelligence (AGI) and deliver cutting-edge research to the whole community.

## What's New

+  [2024.01.15] We release Easytool for easier tool usage.
   + The code and datasets are available at [EasyTool](https://github.com/microsoft/JARVIS/tree/main/easytool).
   + The paper is available at [EasyTool: Enhancing LLM-based Agents with Concise Tool Instruction](https://arxiv.org/abs/2401.06201).
+  [2023.11.30] We release TaskBench for evaluating task automation capability of LLMs.
   + The code and datasets are avaliable at [TaskBench](https://github.com/microsoft/JARVIS/tree/main/taskbench).
   + The paper is avaliable at [TaskBench: Benchmarking Large Language Models for Task Automation](https://arxiv.org/abs/2311.18760).
+  [2023.07.24] We released a light langchain version of Jarvis. See <a href="https://github.com/langchain-ai/langchain/tree/master/libs/experimental/langchain_experimental/autonomous_agents/hugginggpt">here</a>.
+  [2023.04.16] Jarvis now supports the OpenAI service on the Azure platform and the GPT-4 model.


## Reference
If you find this work useful in your method, you can cite the paper as below:
>
    @inproceedings{shen2023hugginggpt,
      author = {Shen, Yongliang and Song, Kaitao and Tan, Xu and Li, Dongsheng and Lu, Weiming and Zhuang, Yueting},
      booktitle = {Advances in Neural Information Processing Systems},
      title = {HuggingGPT: Solving AI Tasks with ChatGPT and its Friends in HuggingFace},
      year = {2023}
    }

>
    @article{shen2023taskbench,
      title   = {TaskBench: Benchmarking Large Language Models for Task Automation},
      author  = {Shen, Yongliang and Song, Kaitao and Tan, Xu and Zhang, Wenqi and Ren, Kan and Yuan, Siyu and Lu, Weiming and Li, Dongsheng and Zhuang, Yueting},
      journal = {arXiv preprint arXiv:2311.18760},
      year    = {2023}
    }

>
    @article{chen2023learning,
      title   = {Learning to teach large language models logical reasoning},
      author  = {Meiqi Chen, Yubo Ma, Kaitao Song, Yixin Cao, Yan Zhang, Dongsheng Li},
      journal = {arXiv preprint arXiv:2310.09158},
      year    = {2023}
    }
    
>
    @article{yuan2024easytool,
      title   = {EASYTOOL: Enhancing LLM-based Agents with Concise Tool Instruction},
      author  = {Siyu Yuan and Kaitao Song and Jiangjie Chen and Xu Tan and Yongliang Shen and Ren Kan and Dongsheng Li and Deqing Yang},
      journal = {arXiv preprint arXiv:2401.06201},
      year    = {2024}
    }

>
    @article{shen2024large,
      title={Large language models empowered autonomous edge AI for connected intelligence},
      author={Shen, Yifei and Shao, Jiawei and Zhang, Xinjie and Lin, Zehong and Pan, Hao and Li, Dongsheng and Zhang, Jun and Letaief, Khaled B},
      journal={IEEE Communications Magazine},
      year={2024},
      publisher={IEEE}
    }

>
    @article{yuan2024evoagent,
      title   = {EvoAgent: Towards Automatic Multi-Agent Generation via Evolutionary Algorithms},
      author  = {Siyu Yuan, Kaitao Song, Jiangjie Chen, Xu Tan, Dongsheng Li, Deqing Yang},
      journal = {arXiv preprint arXiv:2406.14228},
      year    = {2024}
    }

>
    @article{wu2024planning,
      title   = {Can Graph Learning Improve Task Planning?},
      author  = {Xixi Wu, Yifei Shen, Caihua Shan, Kaitao Song, Siwei Wang, Bohang Zhang, Jiarui Feng, Hong Cheng, Wei Chen, Yun Xiong, Dongsheng Li},
      journal = {arXiv preprint arXiv:2405.19119},
      year    = {2024}
    }
