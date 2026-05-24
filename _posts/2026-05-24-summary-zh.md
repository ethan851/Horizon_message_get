---
layout: default
title: "Horizon Summary: 2026-05-24 (ZH)"
date: 2026-05-24
lang: zh
---

> From 20 items, 7 important content pieces were selected

---

1. [从硬件底层优化深度学习性能](#item-1) ⭐️ 9.0/10
2. [Anthropic Project Glasswing：AI 发现逾万高危漏洞](#item-2) ⭐️ 9.0/10
3. [苹果开源 corecrypto，附形式化证明量子安全算法](#item-3) ⭐️ 9.0/10
4. [微软披露 OpenAI 单季度亏损 115 亿美元](#item-4) ⭐️ 9.0/10
5. [80386 微码被反汇编](#item-5) ⭐️ 8.0/10
6. [微软内部大规模推广 Claude Code](#item-6) ⭐️ 8.0/10
7. [中国证监会拟对富途与老虎证券处以巨额罚款](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [从硬件底层优化深度学习性能](https://horace.io/brrr_intro.html) ⭐️ 9.0/10

一篇由 Horace He 撰写的深度技术博客（2022 年）详细解释了如何通过理解 GPU 架构、内存层次结构和内核融合来大幅加速深度学习，实现数量级的性能提升。 该指南使机器学习工程师和研究人员能够编写高效的 GPU 代码，直接影响模型训练和推理成本。它还勾勒了关键行业辩论，如 NVIDIA 的持续领先地位以及跨不同后端的性能可移植性挑战。 该文章涵盖了屋顶线分析、内核融合（合并多个 GPU 内核以减少内存流量）以及使用融合操作（例如，x.cos().cos()比两次单独 cos 调用更快，因为惰性求值和融合）。它展示了在 Python 执行一个 FLOP 的时间内，A100 GPU 可以执行 975 万次 FLOPS。

hackernews · tosh · May 23, 11:50 · [社区讨论](https://news.ycombinator.com/item?id=48246889)

**背景**: GPU 内核融合是一种关键优化技术，它将多个小内核合并为一个，减少内存带宽使用和启动开销。现代 GPU（如 NVIDIA A100）具有巨大的并行性和高内存带宽，但实现峰值性能需要理解内存层次结构和计算与内存比率。硬件感知的优化，包括内核融合和内存访问模式，对于高效的深度学习推理和训练至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/kernel-fusion">Kernel Fusion in GPU Computing</a></li>
<li><a href="https://docs.nvidia.com/deeplearning/performance/dl-performance-gpu-background/index.html">GPU Performance Background User's Guide - NVIDIA Docs</a></li>
<li><a href="https://arxiv.org/pdf/1809.05476">Hardware-Aware Machine Learning: Modeling and ...</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞这篇文章是经典之作，强调了它对 NVIDIA 通过 TFLOP 和带宽的持续指数级增长保持技术领先的清晰解释。其他人则指出缺乏可移植的性能建议，不同运行时和硬件上模型行为各异。关于 x.cos().cos()的技术问题引发了关于内核融合的讨论。

**标签**: `#deep learning`, `#GPU optimization`, `#ML systems`, `#performance engineering`

---

<a id="item-2"></a>
## [Anthropic Project Glasswing：AI 发现逾万高危漏洞](https://www.anthropic.com/research/glasswing-initial-update) ⭐️ 9.0/10

Anthropic 公布了 Project Glasswing 的初期成果，其 Claude Mythos Preview 模型在一个月内从关键开源软件中发现逾万高危严重漏洞，审查后的真阳性率达 90.6%。 这一突破极大加速了漏洞发现，将瓶颈从发现转向修复，并促使行业缩短补丁周期以跟上 AI 驱动的发现速度。 该 AI 模型扫描了数千个开源项目，识别出 6202 个高危/严重漏洞；在经审查的 1752 个中，90.6%为真阳性。Cloudflare 等合作伙伴报告发现速率提高十倍。

telegram · zaihuapd · May 23, 03:16

**背景**: Project Glasswing 是 Anthropic 的一项研究计划，旨在利用 AI 进行防御性网络安全，专注于保护关键软件。Claude Mythos Preview 模型是 Anthropic 最强大的模型，在此用于漏洞发现。开源软件支撑着大多数现代系统，其安全性至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing: Securing critical software for the AI era</a></li>
<li><a href="https://www.anthropic.com/project/glasswing">Project Glasswing \ Anthropic</a></li>
<li><a href="https://cloud.google.com/blog/products/ai-machine-learning/claude-mythos-preview-on-vertex-ai">Claude Mythos Preview on Vertex AI | Google Cloud Blog</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#vulnerability discovery`, `#open source`, `#Anthropic`

---

<a id="item-3"></a>
## [苹果开源 corecrypto，附形式化证明量子安全算法](https://security.apple.com/blog/formal-verification-corecrypto/) ⭐️ 9.0/10

2025 年 5 月 22 日，苹果开源了 corecrypto 密码库，其中包括后量子算法 ML-KEM 和 ML-DSA 的实现，并提供了端到端的形式化验证证明，确保 C 代码和 ARM64 汇编与 NIST 标准严格一致。 这是开创性的一步，因为 corecrypto 为超过 25 亿台活跃苹果设备提供加密运算，而如此大规模地对后量子算法进行形式化验证，为加密软件保障树立了新标杆。 苹果还公开了其定制验证工具和 Isabelle/HOL 理论库供独立评估，覆盖了从高级规范到优化汇编的完整链条。

telegram · zaihuapd · May 23, 04:49

**背景**: 后量子密码学（PQC）旨在抵御未来量子计算机的攻击。ML-KEM（原 Kyber）是一种 NIST 标准化的密钥封装机制，ML-DSA（原 Dilithium）是一种数字签名算法。形式化验证利用数学证明来确认代码正确实现了其规范，从而消除整类错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kyber">ML - KEM - Wikipedia</a></li>
<li><a href="https://nochat.io/lp/post-quantum-encryption-messaging">Post - Quantum Encryption Messaging — ML - KEM & AES-256 | NoChat</a></li>

</ul>
</details>

**标签**: `#cryptography`, `#post-quantum`, `#formal verification`, `#Apple`, `#open source`

---

<a id="item-4"></a>
## [微软披露 OpenAI 单季度亏损 115 亿美元](https://t.me/zaihuapd/41537) ⭐️ 9.0/10

微软最新财报显示，其对 OpenAI 的权益法投资导致净利润减少 31 亿美元，这意味着 OpenAI 单季度净亏损高达 115 亿美元。 这一披露凸显了前沿 AI 开发的极高资本消耗，OpenAI 单季度亏损几乎是其 2024 年上半年总收入 43 亿美元的三倍，可能影响投资者情绪和行业预期。 基于微软持有约 27%的股权，OpenAI 净亏损约为 115 亿美元；若按税前损失和实际持股比例 32.5%计算，亏损可能超过 120 亿美元。微软已向 OpenAI 投入 116 亿美元，占其 130 亿美元承诺投资的绝大部分。

telegram · zaihuapd · May 23, 07:40

**背景**: 权益法下，投资者按其持股比例确认被投资方的损益。OpenAI 的巨额亏损反映了其在开发和运行大型 AI 模型时的高烧钱率——即公司消耗现金的速度。尽管 2024 年上半年创造了 43 亿美元营收，OpenAI 的支出远超收入，这是 AI 初创公司在竞相构建和扩展先进系统时的典型现象。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Equity_(finance)">Equity (finance) - Wikipedia</a></li>
<li><a href="https://www.investopedia.com/terms/b/burnrate.asp">Understanding Burn Rate: Definition, Types, and Calculation Examples</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Microsoft`, `#AI`, `#finance`, `#earnings`

---

<a id="item-5"></a>
## [80386 微码被反汇编](https://www.reenigne.org/blog/80386-microcode-disassembled/) ⭐️ 8.0/10

Intel 80386 CPU 的微码 ROM 已被 reenigne 成功反汇编，揭示了底层的微操作和指令序列。 这一逆向工程工作为了解经典 80386 处理器的内部工作原理提供了前所未有的视角，推动了使用原始微码的开源克隆项目，并加深了对复古计算的理解。 与早期或现代 CPU 不同，80386 对每条指令始终执行一个微操作，反汇编还发现微码 ROM 中可能存在未使用的代码。具体的 CPU 版本很重要，因为微码在其 22 年的生产周期中发生了变化。

hackernews · nand2mario · May 23, 12:11 · [社区讨论](https://news.ycombinator.com/item?id=48247004)

**背景**: 微码是一个将机器指令翻译为硬件控制信号的底层层。在像 80386 这样的复杂 CPU 中，微码定义了微操作的内部序列。反汇编微码需要提取 ROM 内容并解码，这一过程需要深厚的逆向工程技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microcode">Microcode</a></li>
<li><a href="https://www.reenigne.org/blog/80386-microcode-disassembled/">80386 microcode disassembled « Reenigne blog</a></li>

</ul>
</details>

**社区讨论**: 评论者强调知道确切 CPU 版本的重要性，并讨论从芯片图像中提取微码的方法。他们还提到了相关项目如 z386，该项目围绕原始微码构建开源 80386。

**标签**: `#microcode`, `#reverse engineering`, `#80386`, `#CPU architecture`, `#retrocomputing`

---

<a id="item-6"></a>
## [微软内部大规模推广 Claude Code](https://t.me/zaihuapd/41535) ⭐️ 8.0/10

微软正在其工程团队中广泛推广 Anthropic 的 Claude Code，要求工程师同时测试 Claude Code 和 GitHub Copilot，并鼓励非技术员工使用它进行原型设计。 此举表明微软对竞争性 AI 工具的战略开放态度，可能重塑 AI 辅助编程市场，并验证了 Claude Code 在 Anthropic 生态系统外的成熟度。 推广范围涵盖微软的 CoreAI 团队以及负责 Windows、Microsoft 365 和 Outlook 的体验与设备部门。工程师需要同时使用 Claude Code 和 GitHub Copilot 并提供对比反馈。

telegram · zaihuapd · May 23, 06:05

**背景**: Claude Code 是 Anthropic 开发的 AI 编程代理，可集成到 IDE 和终端中辅助软件开发。尽管微软拥有 GitHub Copilot，但内部采用竞争对手的工具凸显了其利用最佳 AI 编程助手的务实态度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#Claude Code`, `#AI coding`, `#GitHub Copilot`, `#software development`

---

<a id="item-7"></a>
## [中国证监会拟对富途与老虎证券处以巨额罚款](https://t.me/zaihuapd/41539) ⭐️ 8.0/10

中国证监会拟对富途控股处以 18.5 亿元罚款，对老虎证券子公司罚没约 4.11 亿元，因其未经批准在内地开展证券、基金销售和期货业务。 此举表明中国加强对跨境证券业务的监管力度，可能影响服务内地客户的境外券商的商业模式。 富途创始人兼首席执行官李华个人拟被罚款 125 万元。罚款仍需经过后续程序并等待最终决定。

telegram · zaihuapd · May 23, 10:58

**背景**: 在中国，从事证券、公募基金销售和期货业务需要获得中国证监会批准。境外证券公司若未取得相应牌照，不得在内地开展相关业务。中国证监会此前已多次警示跨境证券业务的合规风险。此次处罚表明监管层对这类行为的严厉打击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.jiemian.com/article/14471841.html">m.jiemian.com/article/14471841.html</a></li>
<li><a href="https://t.me/xhqcankao/29533">风向旗参考快讯 – Telegram</a></li>
<li><a href="https://finance.sina.cn/2023-01-06/detail-imxzfiqm8946390.d.html">finance.sina.cn/2023-01-06/detail-imxzfiqm8946390.d.html</a></li>

</ul>
</details>

**标签**: `#fintech`, `#regulation`, `#China`, `#securities`

---