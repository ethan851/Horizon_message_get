---
layout: default
title: "Horizon Summary: 2026-05-24 (EN)"
date: 2026-05-24
lang: en
---

> From 20 items, 7 important content pieces were selected

---

1. [Deep Learning Optimization from Hardware Up](#item-1) ⭐️ 9.0/10
2. [Anthropic's Project Glasswing: AI Finds Over 10,000 High-Severity Vulnerabilities](#item-2) ⭐️ 9.0/10
3. [Apple open-sources corecrypto with formal proofs for PQ algorithms](#item-3) ⭐️ 9.0/10
4. [Microsoft Reveals OpenAI's $11.5 Billion Quarterly Loss](#item-4) ⭐️ 9.0/10
5. [80386 Microcode Disassembled](#item-5) ⭐️ 8.0/10
6. [Microsoft Widely Rolls Out Claude Code Internally](#item-6) ⭐️ 8.0/10
7. [China Proposes Fines on Futu, Tiger Brokers](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Deep Learning Optimization from Hardware Up](https://horace.io/brrr_intro.html) ⭐️ 9.0/10

A deep dive blog post by Horace He (2022) explains how to dramatically accelerate deep learning by understanding GPU architecture, memory hierarchy, and kernel fusion, achieving speedups by orders of magnitude. This guide empowers ML engineers and researchers to write highly efficient GPU code, directly impacting model training and inference costs. It also frames key industry debates, such as NVIDIA's sustained lead and the challenge of performance portability across different backends. The post covers techniques like roofline analysis, kernel fusion (merging multiple GPU kernels to reduce memory traffic), and using fused operations (e.g., x.cos().cos() is faster than two separate cos calls due to lazy evaluation and fusion). It demonstrates that in the time Python does one FLOP, an A100 GPU executes 9.75 million FLOPS.

hackernews · tosh · May 23, 11:50 · [Discussion](https://news.ycombinator.com/item?id=48246889)

**Background**: GPU kernel fusion is a key optimization that merges multiple small kernels into one, reducing memory bandwidth usage and launch overhead. Modern GPUs like NVIDIA's A100 have massive parallelism and high memory bandwidth, but achieving peak performance requires understanding the memory hierarchy and compute-to-memory ratio. Hardware-aware optimization, including kernel fusion and memory access patterns, is essential for efficient deep learning inference and training.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/kernel-fusion">Kernel Fusion in GPU Computing</a></li>
<li><a href="https://docs.nvidia.com/deeplearning/performance/dl-performance-gpu-background/index.html">GPU Performance Background User's Guide - NVIDIA Docs</a></li>
<li><a href="https://arxiv.org/pdf/1809.05476">Hardware-Aware Machine Learning: Modeling and ...</a></li>

</ul>
</details>

**Discussion**: Commenters praised the post as a classic, highlighting its clear explanation of NVIDIA's technological lead via sustained exponential growth in TFLOPs and bandwidth. Others noted the lack of portable performance advice, with models behaving differently across runtimes and hardware. A technical query about x.cos().cos() sparked discussion on kernel fusion.

**Tags**: `#deep learning`, `#GPU optimization`, `#ML systems`, `#performance engineering`

---

<a id="item-2"></a>
## [Anthropic's Project Glasswing: AI Finds Over 10,000 High-Severity Vulnerabilities](https://www.anthropic.com/research/glasswing-initial-update) ⭐️ 9.0/10

Anthropic announced initial results from Project Glasswing, where its Claude Mythos Preview model discovered over ten thousand high-severity vulnerabilities in critical open source software within one month, with a 90.6% true positive rate on reviewed findings. This breakthrough dramatically accelerates vulnerability discovery, shifting the bottleneck from finding to fixing, and pressures the industry to shorten patch cycles to keep pace with AI-driven discovery. The AI model scanned thousands of open source projects, identifying 6,202 high/critical vulnerabilities; of 1,752 reviewed, 90.6% were true positives. Partners like Cloudflare reported a ten-fold increase in discovery rate.

telegram · zaihuapd · May 23, 03:16

**Background**: Project Glasswing is Anthropic's research initiative to use AI for defensive cybersecurity, focusing on securing critical software. The Claude Mythos Preview model is Anthropic's most powerful model, used here for vulnerability discovery. Open source software underpins most modern systems, making its security crucial.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing: Securing critical software for the AI era</a></li>
<li><a href="https://www.anthropic.com/project/glasswing">Project Glasswing \ Anthropic</a></li>
<li><a href="https://cloud.google.com/blog/products/ai-machine-learning/claude-mythos-preview-on-vertex-ai">Claude Mythos Preview on Vertex AI | Google Cloud Blog</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cybersecurity`, `#vulnerability discovery`, `#open source`, `#Anthropic`

---

<a id="item-3"></a>
## [Apple open-sources corecrypto with formal proofs for PQ algorithms](https://security.apple.com/blog/formal-verification-corecrypto/) ⭐️ 9.0/10

On May 22, 2025, Apple open-sourced its corecrypto library, including implementations of post-quantum algorithms ML-KEM and ML-DSA, and provided end-to-end formal verification proofs that the C and ARM64 assembly code exactly matches the NIST standards. This is a groundbreaking step because corecrypto powers encryption on over 2.5 billion active Apple devices, and formal verification of post-quantum algorithms at this scale sets a new bar for cryptographic software assurance. Apple also released its custom verification tools and Isabelle/HOL theory libraries for independent evaluation, covering the entire chain from high-level specifications to optimized assembly.

telegram · zaihuapd · May 23, 04:49

**Background**: Post-quantum cryptography (PQC) is designed to resist attacks from future quantum computers. ML-KEM (formerly Kyber) is a NIST-standardized key encapsulation mechanism, and ML-DSA (formerly Dilithium) is a digital signature algorithm. Formal verification uses mathematical proofs to confirm that code correctly implements its specification, eliminating entire classes of bugs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kyber">ML - KEM - Wikipedia</a></li>
<li><a href="https://nochat.io/lp/post-quantum-encryption-messaging">Post - Quantum Encryption Messaging — ML - KEM & AES-256 | NoChat</a></li>

</ul>
</details>

**Tags**: `#cryptography`, `#post-quantum`, `#formal verification`, `#Apple`, `#open source`

---

<a id="item-4"></a>
## [Microsoft Reveals OpenAI's $11.5 Billion Quarterly Loss](https://t.me/zaihuapd/41537) ⭐️ 9.0/10

Microsoft's latest earnings report disclosed a $3.1 billion reduction in net income attributable to its equity method investment in OpenAI, implying that OpenAI incurred a staggering $11.5 billion net loss in a single quarter. This disclosure underscores the extreme capital intensity of cutting-edge AI development, as OpenAI's quarterly loss nearly triples its total revenue of $4.3 billion in the first half of 2024, potentially affecting investor sentiment and industry expectations. Based on Microsoft's ~27% ownership stake, OpenAI's net loss was calculated at ~$11.5 billion; using a pre-tax figure and actual stake of 32.5%, the loss could exceed $12 billion. Microsoft has invested $11.6 billion of its $13 billion committed investment in OpenAI.

telegram · zaihuapd · May 23, 07:40

**Background**: Under the equity method, an investor records its share of the investee's profits or losses. OpenAI's massive loss reflects its high burn rate—the rate at which a company spends cash—in developing and operating large AI models. Despite generating $4.3 billion in revenue in the first half of 2024, OpenAI's expenses far outpace its income, typical for AI startups racing to build and scale advanced systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Equity_(finance)">Equity (finance) - Wikipedia</a></li>
<li><a href="https://www.investopedia.com/terms/b/burnrate.asp">Understanding Burn Rate: Definition, Types, and Calculation Examples</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Microsoft`, `#AI`, `#finance`, `#earnings`

---

<a id="item-5"></a>
## [80386 Microcode Disassembled](https://www.reenigne.org/blog/80386-microcode-disassembled/) ⭐️ 8.0/10

The microcode ROM of the Intel 80386 CPU has been successfully disassembled by reenigne, revealing the low-level micro-operations and instruction sequencing. This reverse engineering effort provides unprecedented insight into the internal workings of the classic 80386 processor, enabling projects like open-source clones that use original microcode and advancing retrocomputing understanding. The 80386 always executes a micro-op for every instruction, unlike earlier or modern CPUs, and the disassembly revealed potential unused code in the microcode ROM. The specific CPU revision is important because microcode changed over its 22-year production run.

hackernews · nand2mario · May 23, 12:11 · [Discussion](https://news.ycombinator.com/item?id=48247004)

**Background**: Microcode is a low-level layer that translates machine instructions into hardware control signals. In complex CPUs like the 80386, microcode defines the internal sequencing of micro-operations. Disassembling microcode involves extracting the ROM contents and decoding them, a process that requires deep reverse engineering skills.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microcode">Microcode</a></li>
<li><a href="https://www.reenigne.org/blog/80386-microcode-disassembled/">80386 microcode disassembled « Reenigne blog</a></li>

</ul>
</details>

**Discussion**: Commenters emphasize the importance of knowing the exact CPU revision and discuss methods to extract microcode from die images. They also reference related projects like z386, which builds an open-source 80386 around original microcode.

**Tags**: `#microcode`, `#reverse engineering`, `#80386`, `#CPU architecture`, `#retrocomputing`

---

<a id="item-6"></a>
## [Microsoft Widely Rolls Out Claude Code Internally](https://t.me/zaihuapd/41535) ⭐️ 8.0/10

Microsoft is broadly rolling out Anthropic's Claude Code to its engineering teams, requiring engineers to test it alongside GitHub Copilot and encouraging non-technical employees to use it for prototyping. This move signals Microsoft's strategic openness to competing AI tools, potentially reshaping the AI-assisted coding market and validating Claude Code's maturity outside of Anthropic's own ecosystem. The rollout covers Microsoft's CoreAI team and the Experiences & Devices division responsible for Windows, Microsoft 365, and Outlook. Engineers must provide comparative feedback on both Claude Code and GitHub Copilot.

telegram · zaihuapd · May 23, 06:05

**Background**: Claude Code is an AI coding agent developed by Anthropic that integrates with IDEs and terminals to assist with software development. While Microsoft owns GitHub Copilot, this internal adoption of a competitor's tool highlights a pragmatic approach to leveraging the best available AI coding assistants.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#Claude Code`, `#AI coding`, `#GitHub Copilot`, `#software development`

---

<a id="item-7"></a>
## [China Proposes Fines on Futu, Tiger Brokers](https://t.me/zaihuapd/41539) ⭐️ 8.0/10

Chinese regulators proposed fines of 18.5 billion yuan on Futu Holdings and 4.11 billion yuan on Tiger Brokers' subsidiaries for unauthorized securities, fund sales, and futures operations in mainland China. This action signals tightening regulatory oversight of cross-border securities operations, potentially impacting the business models of offshore brokerages serving mainland Chinese clients. Futu's founder and CEO Li Hua faces a personal fine of 1.25 million yuan. The fines are preliminary and subject to further procedures and final decisions.

telegram · zaihuapd · May 23, 10:58

**Background**: In China, conducting securities, public fund sales, and futures business requires approval from the China Securities Regulatory Commission (CSRC). Foreign brokerages operating without these licenses are considered illegal. The CSRC has previously warned against unauthorized cross-border securities activities. This enforcement demonstrates a serious commitment to regulating such practices.

<details><summary>References</summary>
<ul>
<li><a href="https://m.jiemian.com/article/14471841.html">m.jiemian.com/article/14471841.html</a></li>
<li><a href="https://t.me/xhqcankao/29533">风向旗参考快讯 – Telegram</a></li>
<li><a href="https://finance.sina.cn/2023-01-06/detail-imxzfiqm8946390.d.html">finance.sina.cn/2023-01-06/detail-imxzfiqm8946390.d.html</a></li>

</ul>
</details>

**Tags**: `#fintech`, `#regulation`, `#China`, `#securities`

---