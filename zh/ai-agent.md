---
layout: page
title: AI+智能体
description: 本页面介绍我们在大语言模型智能体方向的研究。
lang: zh-CN
alternate_url: /llm_agent
permalink: /zh/ai-agent/
---

## 概览

我们以自然语言作为接口，让大语言模型连接多种 AI 模型，共同完成复杂任务。系统由一个作为控制器的大语言模型和多个作为执行器的专家模型组成，工作流包括四个阶段：

- **任务规划**：理解用户意图，并把请求拆分为可执行任务。
- **模型选择**：根据任务及模型描述选择合适的专家模型。
- **任务执行**：调用所选模型并收集结果。
- **回答生成**：整合各模型输出，形成最终回答。

<p align="center"><img src="/img/agent/overview.jpg" width="500" alt="HuggingGPT 智能体框架"></p>

## 开源项目

项目代码位于 [microsoft/JARVIS](https://github.com/microsoft/JARVIS)。JARVIS 致力于探索通用人工智能，并向研究社区开放前沿成果。

## 研究主题

### 工具使用与任务自动化

HuggingGPT 建立了由大语言模型进行任务规划、专家模型选择、任务执行和结果整合的控制器架构 [Shen et al., NeurIPS 2023][^8]。TaskBench 提供面向任务自动化与规划的大规模基准 [Shen et al., NeurIPS 2024][^9]；EasyTool 则把冗长工具文档压缩为智能体更容易理解和使用的简洁指令 [Yuan et al., NAACL 2025][^1]。相应代码和数据均在 [JARVIS](https://github.com/microsoft/JARVIS) 中维护。

### 智能体学习、记忆与多智能体生成

EvoAgent 通过进化操作自动生成多智能体系统 [Yuan et al., NAACL 2025][^2]。近期的记忆增强智能体结合在线与离线策略优化，使经验既能支持稳定学习，又能保持持续探索 [Liu et al., ICLR 2026][^3]。

### 垂直领域智能体

我们研究把智能体的推理和记忆扎根于专业工作流。Trade in Minutes! 构建理性驱动的量化金融交易智能体系统 [Song et al., ICLR 2026][^6]；AgentCF++ 通过双层记忆和群体共享记忆，建模推荐场景中的跨领域偏好与流行度影响 [Liu et al., SIGIR 2025][^7]。

### 计算机操作智能体与评测

WeaveBench 面向长程真实任务，要求智能体协同使用图形界面、终端、代码编辑器、浏览器和外部工具 [Li et al., EMNLP 2026][^4]。MedCUA-Bench 将这一方向扩展到临床工作流和纯截图交互 [Yu et al., EMNLP 2026 Findings][^5]。二者共同评估智能体能否完成端到端工作流，而不只是孤立动作。

JARVIS 还支持 Azure OpenAI 与 GPT-4；LangChain 中提供了轻量级 [HuggingGPT 实现](https://github.com/langchain-ai/langchain/tree/master/libs/experimental/langchain_experimental/autonomous_agents/hugginggpt)。

## 参考文献

[^1]: [Siyu Yuan et al. EASYTOOL: Enhancing LLM-based Agents with Concise Tool Instruction. NAACL 2025.](https://openreview.net/forum?id=B9pxstB1tB)
[^2]: [Siyu Yuan et al. EvoAgent: Towards Automatic Multi-Agent Generation via Evolutionary Algorithms. NAACL 2025.](https://openreview.net/forum?id=QPRpTAxPJM)
[^3]: [Zeyuan Liu et al. Exploratory Memory-Augmented LLM Agent via Hybrid On- and Off-Policy Optimization. ICLR 2026.](https://openreview.net/forum?id=UOzxviKVFO)
[^4]: [Wanli Li et al. WeaveBench: A Long-Horizon, Real-World Benchmark for Computer-Use Agents with Hybrid Interfaces. EMNLP 2026.](https://arxiv.org/abs/2606.09426)
[^5]: [Jia Yu et al. MedCUA-Bench: A Screenshot-Only Benchmark for Clinical Computer-Use Agents. EMNLP 2026 Findings.](https://openreview.net/forum?id=gC1m98w7cq)
[^6]: [Zifan Song et al. Trade in Minutes! Rationality-Driven Agentic System for Quantitative Financial Trading. ICLR 2026.](https://openreview.net/forum?id=ROEwZAxqyS)
[^7]: [Jiahao Liu et al. AgentCF++: Memory-enhanced LLM-based Agents for Popularity-aware Cross-domain Recommendations. SIGIR 2025.](https://arxiv.org/abs/2502.13843)
[^8]: [Yongliang Shen et al. HuggingGPT: Solving AI Tasks with ChatGPT and its Friends in Hugging Face. NeurIPS 2023.](https://arxiv.org/abs/2303.17580)
[^9]: [Yongliang Shen et al. TaskBench: Benchmarking Large Language Models for Task Automation. NeurIPS 2024.](https://openreview.net/forum?id=bAxUA5r3Ss)