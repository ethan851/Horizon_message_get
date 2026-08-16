---
layout: default
title: "Horizon Summary: 2026-08-16 (EN)"
date: 2026-08-16
lang: en
---

> From 19 items, 3 important content pieces were selected

---

1. [AI's Edge Over Mathematicians: Memory and Persistence, Not Reasoning](#item-1) ⭐️ 8.0/10
2. [Codex Auto-Research Speeds Up Kernel by 232x](#item-2) ⭐️ 8.0/10
3. [Tencent Negotiates to Acquire Manus, Oust Meta as Top Shareholder](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [AI's Edge Over Mathematicians: Memory and Persistence, Not Reasoning](https://davidepiffer.com/p/ai-isnt-outthinking-mathematicians) ⭐️ 8.0/10

A new essay by Davide Piffer argues that AI's advantage over human mathematicians stems from a vastly larger working memory and tireless persistence, not from superior reasoning ability. The piece reframes AI's mathematical achievements as an outcome of scale and endurance. This reframing challenges common assumptions about AI's cognitive abilities, suggesting that memory capacity and persistence may matter more than reasoning algorithms. It influences how researchers and the public evaluate AI progress in mathematics and other knowledge work. The essay contrasts AI's large context window with the limited working memory of humans, and notes that AI never tires or gets discouraged. Community discussants add that AI can systematically record and reuse negative results, with projects like theoremdb.org exploring this idea.

hackernews · rzk · Aug 15, 18:13 · [Discussion](https://news.ycombinator.com/item?id=49312845)

**Background**: Working memory is the limited information a person can actively hold and manipulate at one time, while an LLM's context window is the amount of text it can 'remember' when generating output. Modern LLMs have context windows that can span thousands of pages, vastly exceeding human working memory capacity. The essay builds on this contrast to argue that AI's mathematical successes may be explained by memory scale and persistent search, rather than deeper reasoning.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/context-window">What is a context window? - IBM</a></li>
<li><a href="https://arxiv.org/html/2504.15965v2">From Human Memory to AI Memory: A Survey on Memory Mechanisms ...</a></li>
<li><a href="https://www.illumio.com/blog/the-limits-of-working-memory-human-brains-vs-ai-models">The Limits of Working Memory: Human Brains vs. AI Models</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed and extended the argument: some saw intelligence as 'out-remembering' others, while others emphasized AI's ability to brute-force search without fatigue. A few pointed to related work on augmenting long-term memory or publishing negative results, though one commenter felt the point was fairly obvious.

**Tags**: `#AI`, `#mathematics`, `#working memory`, `#cognition`, `#LLM`

---

<a id="item-2"></a>
## [Codex Auto-Research Speeds Up Kernel by 232x](https://sankalp.bearblog.dev/autoresearch/) ⭐️ 8.0/10

A developer used OpenAI's Codex to autonomously research and optimize a GPU kernel, achieving a 232x speedup. The work demonstrates a fully automated 'modify-verify-retain' loop for performance engineering. This result highlights the potential of LLM agents to tackle complex, low-level optimization tasks that typically require deep expert knowledge. It also fuels discussion about the reliability of such optimizations, especially when models overfit to benchmark inputs. The optimization was performed through an iterative agent loop that modifies code, verifies correctness, and retains or discards changes. Community members noted that in a related competition, 8 out of 10 AI-optimized top solutions failed on out-of-distribution inputs, while expert-guided solutions remained robust.

hackernews · tosh · Aug 15, 11:00 · [Discussion](https://news.ycombinator.com/item?id=49309549)

**Background**: CUDA kernels are functions that run on NVIDIA GPUs in parallel, and optimizing them is a notorious challenge in high-performance computing. Codex is an AI agent from OpenAI that can autonomously edit and test code, and 'auto-research' refers to a self-directed loop where the agent repeatedly improves and verifies its own changes. The codex-autoresearch skill implements such a workflow for Codex CLI and similar tools.

<details><summary>References</summary>
<ul>
<li><a href="https://modal.com/gpu-glossary/device-software/kernel">What is a CUDA Kernel ? | GPU Glossary</a></li>
<li><a href="https://github.com/leo-lilinxiao/codex-autoresearch/blob/main/docs/EXAMPLES.md">codex -autoresearch/docs/EXAMPLES.md at main...</a></li>

</ul>
</details>

**Discussion**: Comments express both enthusiasm and caution. One user's experience with a video codec repository showed promise, but another warned that many benchmark-winning AI solutions were brittle on unseen inputs. Another commenter appreciated the human-written style, and one wondered whether GPU kernel code is particularly well-represented in training data.

**Tags**: `#AI-assisted development`, `#kernel optimization`, `#CUDA`, `#LLM agents`, `#performance engineering`

---

<a id="item-3"></a>
## [Tencent Negotiates to Acquire Manus, Oust Meta as Top Shareholder](https://t.me/zaihuapd/43205) ⭐️ 8.0/10

Tencent is in talks to acquire AI startup Manus and become its largest shareholder by buying back Meta's stake for at least $2 billion, with backing from original investors ZhenFund and HSG. Beijing had previously asked Meta to unwind its $2 billion acquisition of Manus. This deal would reshape competitive dynamics in AI, transferring a prominent AI startup from Meta to Tencent and giving Tencent strategic control. It also highlights how regulatory pressures in China can influence global tech M&A. The deal is valued at no less than $2 billion, and Tencent will partner with Manus's original investors, including ZhenFund and HSG. Neither Tencent, Manus, Meta, nor the two investment firms has responded to requests for comment; the news was first reported by the Financial Times and cited by Reuters.

telegram · zaihuapd · Aug 15, 08:05

**Background**: Manus is an autonomous AI agent developed by Butterfly Effect, a company founded in China and based in Singapore, and is designed to perform complex real-world tasks such as research, data processing, and web navigation. In December 2025, Meta announced it would acquire Manus in a deal reportedly valued between $2 and $3 billion, but Chinese regulators later asked Meta to unwind the acquisition.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_AI">Manus AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus (AI agent) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Tencent`, `#Meta`, `#acquisition`, `#Manus`

---