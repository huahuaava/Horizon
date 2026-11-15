---
layout: default
title: "Horizon Summary: 2026-11-15 (EN)"
date: 2026-11-15
lang: en
---

> From 120 items, 4 important content pieces were selected

---

**Technology News**
1. [Understanding Positional Embeddings in Modern LLMs](#item-tech-news-1) ⭐️ 8.0/10
2. [SpaceX successfully catches Starship upper stage during Flight 15](#item-tech-news-2) ⭐️ 8.0/10
3. [Applying Recursive Self-Improvement to Frontier Pre-training From Scratch](#item-tech-news-3) ⭐️ 8.0/10
4. [Haru-4B Open-Source Full-Duplex Spoken Dialogue Model Released](#item-tech-news-4) ⭐️ 8.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [Understanding Positional Embeddings in Modern LLMs](https://magazine.sebastianraschka.com/p/understanding-positional-embeddings) ⭐️ 8.0/10

Sebastian Raschka published a technical analysis examining how positional embeddings are implemented and utilized in modern large language models. The piece breaks down the specific mechanisms used to inject sequence order information into transformer architectures. No specific software versions, benchmarks, or availability conditions were announced alongside the article.

hackernews · vismit2000 · Nov 15, 12:14 · [Discussion](https://news.ycombinator.com/item?id=50506376)

**「Background」** Because the self-attention mechanism in transformer models is inherently permutation-invariant, models require positional embeddings to process the order of tokens in a sequence.

**「Community Discussion」** A commenter argued that fully understanding positional embeddings requires looking beyond software implementation to underlying group theory, noting that rotary positional embeddings specifically represent the translation group.

**Tags**: `#artificial intelligence`, `#machine learning`, `#natural language processing`, `#large language models`

---

<a id="item-tech-news-2"></a>
### [SpaceX successfully catches Starship upper stage during Flight 15](https://www.spacex.com/launches/starship-flight-15) ⭐️ 8.0/10

SpaceX successfully caught the Starship upper stage during the Flight 15 test, marking the first demonstration of a reusable rocket upper stage system since the Space Shuttle. The maneuver was captured on video and verified via mission broadcasts. It advances the development toward fully reusable orbital launch systems.

hackernews · ls612 · Nov 14, 21:22 · [Discussion](https://news.ycombinator.com/item?id=50500963)

**「Background」** Developing a reusable orbital-class rocket requires safely recovering major flight hardware components, such as boosters and upper stages, to minimize expensive manufacturing and refurbishment cycles between launches.

**「Impact」** Achieving upper-stage reusability lays the groundwork for drastically lowering orbital payload costs and increasing launch cadences once refurbishment and reliability are proven at scale.

**「Community Discussion」** Commenters acknowledged the historic significance of catching a rocket upper stage for the first time since the Space Shuttle era, while noting that durability and heat shield performance remain critical factors for future operational reflights.

**Tags**: `#aerospace`, `#hardware`, `#engineering`, `#systems`

---

<a id="item-tech-news-3"></a>
### [Applying Recursive Self-Improvement to Frontier Pre-training From Scratch](https://www.reddit.com/r/LocalLLaMA/comments/1xwt3ri/paper_no_second_run_does_rsi_stop_at_frontier/) ⭐️ 8.0/10

Researchers have applied recursive self-improvement \(RSI\) to frontier pre-training from scratch by decomposing the unrepeatable process into smaller feedback loops, resulting in the release of 801-30B-A3B-Base. The model is a 30B-A3B Mixture-of-Experts trained on 11.8 trillion tokens over three months. As a base model, it outperforms Qwen3-30B-A3B and Nemotron-3.5-Lightning-30B-A3B while trailing Qwen3.5-35B-A3B, and it achieves the highest average on four agentic benchmarks against fully post-trained models when using a lightweight 6B-token SFT.

reddit · r/LocalLlama · /u/pmttyji · Nov 15, 11:21

**「Background」** Public work on recursive self-improvement for large language models has historically focused on post-training, which builds on an existing base model and benefits from repeatable trials and verifiable scores. Pre-training from scratch, by contrast, consumes hundreds of thousands of GPU-hours over months, lacks an immediate single verification score, and involves an entire production system rather than just a standalone model.

**「Impact」** Developers and researchers can utilize the open-sourced 801-30B-A3B-Base model, its SFT dataset, and the accompanying research paper to examine how RSI techniques can be adapted for foundational pre-training.

**Tags**: `#artificial intelligence`, `#machine learning`, `#large language models`, `#pre-training`, `#recursive self-improvement`

---

<a id="item-tech-news-4"></a>
### [Haru-4B Open-Source Full-Duplex Spoken Dialogue Model Released](https://www.reddit.com/r/LocalLLaMA/comments/1xww5o2/higurashiaiharu4b_hugging_face/) ⭐️ 8.0/10

Higurashi-AI has released Haru-4B, a pretrained multilingual, full-duplex continuous spoken dialogue foundation model designed for research. The model processes audio natively at 7.5 Hz, allowing it to listen and speak simultaneously by generating one frame of audio and text every 133 ms. It combines user audio, model audio, and text into a single language model stream using a 64-dimensional latent per frame and a MeanFlow sampling MLP head. Additionally, it supports English, Spanish, Portuguese, German, French, Chinese, Japanese, Russian, and Korean, with character and voice control managed via text cards and reference clips.

reddit · r/LocalLlama · /u/pmttyji · Nov 15, 13:58

**「Background」** Traditional conversational AI systems typically rely on a pipeline architecture that separates speech-to-text, text generation, and text-to-speech, which introduces latency and prevents simultaneous listening and speaking. Recent advancements in speech-language models have focused on native audio tokenization and continuous representations to enable more natural, low-latency conversational interactions.

**「Impact」** Researchers and developers working on open-source conversational AI can now experiment with a native full-duplex foundation model that eliminates traditional turn-taking delays and separate audio transformers.

**Tags**: `#artificial intelligence`, `#machine learning`, `#spoken dialogue models`, `#open source`, `#audio generation`

---