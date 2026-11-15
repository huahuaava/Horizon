---
layout: default
title: "Horizon Summary: 2026-11-15 (ZH)"
date: 2026-11-15
lang: zh
---

> 从 120 条内容中筛选出 4 条重要资讯。

---

**科技新闻**
1. [理解现代大语言模型中的位置编码](#item-tech-news-1) ⭐️ 8.0/10
2. [SpaceX 成功在第 15 次飞行中捕获 Starship 级](#item-tech-news-2) ⭐️ 8.0/10
3. [递归自我改进延伸至前沿预训练，801-30B-A3B-Base 模型开源](#item-tech-news-3) ⭐️ 8.0/10
4. [higurashi-ai 发布 Haru-4B 开源多语种全双工语音模型](#item-tech-news-4) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [理解现代大语言模型中的位置编码](https://magazine.sebastianraschka.com/p/understanding-positional-embeddings) ⭐️ 8.0/10

本文深入分析了现代大语言模型中位置 embeddings 的实现方式与实际应用。文章为开发者提供了关于模型如何处理序列中词元相对与绝对位置的技术解析。相关讨论指出了纯粹从实现层面理解的局限性。

hackernews · vismit2000 · 11月15日 12:14 · [社区讨论](https://news.ycombinator.com/item?id=50506376)

**「背景」** 由于 Transformer 架构本身对输入词元的顺序不敏感，大语言模型必须借助位置编码来注入序列的顺序信息，以便正确理解上下文关系。

**「社区讨论」** 有评论指出，仅从代码实现来理解位置编码是不够的，深入理解需要借助群论视角，将旋转位置编码等方法视为群表示来进行参数化和微分。

**标签**: `#artificial intelligence`, `#machine learning`, `#natural language processing`, `#large language models`

---

<a id="item-tech-news-2"></a>
### [SpaceX 成功在第 15 次飞行中捕获 Starship 级](https://www.spacex.com/launches/starship-flight-15) ⭐️ 8.0/10

SpaceX 在 Starship 的第 15 次飞行中成功完成了对火箭上升级的捕获。这一成就标志着向完全可重复使用轨道发射系统迈出了重要一步。

hackernews · ls612 · 11月14日 21:22 · [社区讨论](https://news.ycombinator.com/item?id=50500963)

**「背景」** Starship 是 SpaceX 开发的下一代重型运载火箭系统，旨在实现完全可重复使用，以大幅降低发射成本并提高发射频率。

**「影响」** 成功捕获上升级为实现高频次、低成本的轨道飞行奠定了硬件基础，若后续热防护及复飞验证顺利，将彻底改变航天发射的经济性。

**「社区讨论」** 评论者指出，这是自航天飞机以来首次成功演示可重复使用的火箭上升级，其历史意义重大。不过，社区成员也指出后续仍需验证热防护系统的表现以及多次重复飞行的可行性。

**标签**: `#aerospace`, `#hardware`, `#engineering`, `#systems`

---

<a id="item-tech-news-3"></a>
### [递归自我改进延伸至前沿预训练，801-30B-A3B-Base 模型开源](https://www.reddit.com/r/LocalLLaMA/comments/1xwt3ri/paper_no_second_run_does_rsi_stop_at_frontier/) ⭐️ 8.0/10

研究人员将递归自我改进（RSI）首次应用到从头开始的前沿预训练中，通过将不可重复的完整过程分解为更小的反馈循环来克服成本与评估障碍。由此产生的 801-30B-A3B-Base 是一个 30B-A3B 混合专家（MoE）基础模型，由新团队在三个月内使用 11.8 万亿个 Token 从头训练完成。该模型现已开源，在基础模型阶段表现优于 Qwen3-30B-A3B 和 Nemotron-3.5-Lightning-30B-A3B，并在仅经过轻量级 SFT（60 亿 Token，无 RL）后在四个代理基准测试中创下同类模型最高平均分。

reddit · r/LocalLlama · /u/pmttyji · 11月15日 11:21

**「背景」** 此前公开的递归自我改进工作主要集中在后训练阶段，该阶段依赖于现有的基础模型、可控的 GPU 试错成本以及可验证的分数，而前沿预训练则因耗资巨大且过程不可重复而难以直接应用自我改进。

**「影响」** 开发人员和研究机构现在可以获取 801-30B-A3B-Base 模型及其轻量级 SFT 数据集，从而能够利用在预训练阶段引入递归自我改进的基础模型进行进一步研究或下游应用开发。

**标签**: `#artificial intelligence`, `#machine learning`, `#large language models`, `#pre-training`, `#recursive self-improvement`

---

<a id="item-tech-news-4"></a>
### [higurashi-ai 发布 Haru-4B 开源多语种全双工语音模型](https://www.reddit.com/r/LocalLLaMA/comments/1xww5o2/higurashiaiharu4b_hugging_face/) ⭐️ 8.0/10

higurashi-ai 发布了 Haru-4B，这是一款低延迟、多语种的全双工连续语音对话基础模型，适用于研究用途。该模型在单一语言模型流中原生支持每秒 7.5 帧的全双工处理，每 133 毫秒同时接收用户音频帧并生成音频与文本帧。它通过 MeanFlow 采样直接从隐藏状态生成 64 维连续音频潜在表示，无需离散音频标记或单独的音频 Transformer。支持英语、西班牙语、葡萄牙语、德语、法语、中文、日语、俄语和韩语九种语言，并可通过文本卡片设定角色、参考音频剪辑控制声音。

reddit · r/LocalLlama · /u/pmttyji · 11月15日 13:58

**「背景」** 传统的对话模型通常采用分段式的“先听后说”轮流交互模式，在实时性和自然双向交互方面存在局限。全双工语音对话技术旨在让模型能够像人类打电话一样同时进行倾听和发言。

**「影响」** 研究人员和开发者现在可以利用这一开源的 4B 基础模型，构建具备低延迟、原生双向对话以及多语种支持的实时语音交互应用。

**标签**: `#artificial intelligence`, `#machine learning`, `#spoken dialogue models`, `#open source`, `#audio generation`

---