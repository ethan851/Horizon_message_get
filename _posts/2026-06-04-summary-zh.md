---
layout: default
title: "Horizon Summary: 2026-06-04 (ZH)"
date: 2026-06-04
lang: zh
---

> From 28 items, 13 important content pieces were selected

---

1. [美国计划拆除大西洋洋流监测系统](#item-1) ⭐️ 9.0/10
2. [Elixir v1.20 引入渐进类型系统](#item-2) ⭐️ 9.0/10
3. [Google 发布 Gemma 4 12B：无编码器多模态模型](#item-3) ⭐️ 9.0/10
4. [Let's Encrypt 计划通过默克尔树实现后量子证书](#item-4) ⭐️ 9.0/10
5. [优步将员工 AI 工具月支出上限设为 1500 美元](#item-5) ⭐️ 8.0/10
6. [DaVinci Resolve 21 发布，新增照片管理和 AI 工具](#item-6) ⭐️ 8.0/10
7. [乐鑫发布 ESP32-S31：内置 SIMD 指令的 RISC-V SoC](#item-7) ⭐️ 8.0/10
8. [数学家警告 AI 快速发展](#item-8) ⭐️ 8.0/10
9. [原始 PlayStation 架构深度分析](#item-9) ⭐️ 8.0/10
10. [谷歌允许网站退出 AI 搜索结果](#item-10) ⭐️ 8.0/10
11. [千问向第三方智能体和技能全面开放平台](#item-11) ⭐️ 8.0/10
12. [HTTP/2 Bomb 远程击垮主流服务器](#item-12) ⭐️ 8.0/10
13. [奥特曼：OpenAI 内部最高用户月消耗约 1000 亿 token](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [美国计划拆除大西洋洋流监测系统](https://e360.yale.edu/digest/trump-ooi-amoc) ⭐️ 9.0/10

美国政府计划拆除自 2004 年起在 26.5°N 监测大西洋经向翻转环流（AMOC）的 RAPID 阵列。尽管有越来越多的证据表明 AMOC 因气候变化面临崩溃风险，这一决定仍被提出。 AMOC 的崩溃将对全球气候产生灾难性影响，而失去持续监测将使早期预警能力丧失。此举凸显了气候科学资金与其他国家优先事项之间的持续矛盾。 与重大国防项目相比，RAPID 阵列是一个相对廉价的系统，但它为理解 AMOC 行为提供了关键数据。近期研究表明，AMOC 正处于 1600 多年来的最弱状态，可能正接近临界点。

hackernews · rguiscard · Jun 4, 00:44 · [社区讨论](https://news.ycombinator.com/item?id=48392232)

**背景**: 大西洋经向翻转环流（AMOC）是一个将暖水向北输送、冷水向南输送的洋流系统，在调节全球气候中起着至关重要的作用。位于 26.5°N 的 RAPID 阵列自 2004 年以来持续提供 AMOC 的观测数据，使科学家能够追踪其强度和变化。没有这样的监测，检测突变或即将发生的崩溃将变得更加困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Atlantic_meridional_overturning_circulation">Atlantic meridional overturning circulation - Wikipedia</a></li>
<li><a href="https://oceanservice.noaa.gov/facts/amoc.html">What is the Atlantic Meridional Overturning Circulation (AMOC)?</a></li>
<li><a href="https://www.theguardian.com/environment/2026/apr/15/critical-atlantic-current-significantly-more-likely-to-collapse-than-thought">Critical Atlantic current significantly more likely to collapse than thought | Oceans | The Guardian</a></li>
<li><a href="https://climate.metoffice.cloud/amoc.html">AMOC | Climate Dashboard</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC10590665/">From theory to RAPID AMOC observations: a personal voyage of...</a></li>

</ul>
</details>

**社区讨论**: 评论对削减气候监测同时大规模投资 F-35 等军事项目表示失望，指出 RAPID 阵列相对低廉的成本。一些用户强调报道中的政治倾向，另一些则强调连续数据对气候建模的重要性。

**标签**: `#climate science`, `#oceanography`, `#policy`, `#research funding`, `#AMOC`

---

<a id="item-2"></a>
## [Elixir v1.20 引入渐进类型系统](https://elixir-lang.org/blog/2026/06/03/elixir-v1-20-0-released/) ⭐️ 9.0/10

Elixir v1.20 于 2026 年 6 月 3 日发布，引入了渐进类型作为核心特性，允许开发者可选地添加静态类型注解，同时未注解的代码保持动态类型。 这标志着 Elixir 的重大演进，满足了函数式编程社区对静态类型的长期需求，并可能吸引那些偏好类型安全但又不愿牺牲语言动态灵活性的开发者。 该渐进类型系统基于 Jeremy Siek 和 Walid Taha 的研究，已集成到编译器中，并在必要时通过运行时检查提供健全的类型系统。

hackernews · cloud8421 · Jun 3, 19:02 · [社区讨论](https://news.ycombinator.com/item?id=48388324)

**背景**: 渐进类型是一种允许在同一语言中混合静态和动态类型的类型系统，能够逐步添加类型注解以提高安全性，而无需完全重写。Elixir 此前依赖 Dialyzer 进行类型推断，但新系统提供了更深入的集成和健全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gradual_typing">Gradual typing</a></li>
<li><a href="https://jsiek.github.io/home/WhatIsGradualTyping.html">What is Gradual Typing | Jeremy Siek</a></li>

</ul>
</details>

**社区讨论**: 社区评论中既有兴奋也有怀疑，一些开发者欢迎向类型化迈进，而另一些则质疑与 Dialyzer 的“成功类型”方法相比的性能权衡。关于渐进类型能否达到完全静态系统的效率，存在争论。

**标签**: `#Elixir`, `#gradual typing`, `#functional programming`, `#language design`, `#type systems`

---

<a id="item-3"></a>
## [Google 发布 Gemma 4 12B：无编码器多模态模型](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemma-4-12b/) ⭐️ 9.0/10

Google DeepMind 发布了 Gemma 4 12B，这是一款紧凑型无编码器多模态模型，无需单独的视觉编码器即可通过语言模型主干直接处理视觉和音频输入。 这种设计显著缩小了模型体积并降低了硬件要求，使强大的多模态 AI 能够在配备 16GB RAM 的消费级笔记本上运行，从而普及了先进 AI 能力的访问。 该模型用仅包含单次矩阵乘法、位置嵌入和归一化的轻量级嵌入模块取代了传统的视觉编码器，总参数量仅为 3500 万。该模型以 Apache 2.0 许可证发布。

hackernews · rvz · Jun 3, 16:04 · [社区讨论](https://news.ycombinator.com/item?id=48385906)

**背景**: 传统的多模态大语言模型（LLM）依赖单独的视觉编码器（如 5.5 亿参数的 SigLIP）和音频编码器（3 亿参数）来处理非文本输入。这些编码器增加了大量计算开销。Gemma 4 12B 的无编码器架构将原始视觉和音频令牌直接送入 LLM 主干，大幅提升了效率，无需云端依赖即可在消费级硬件上进行本地推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/06/03/google-deepmind-releases-gemma-4-12b-an-encoder-free-multimodal-model-with-native-audio-that-runs-on-a-16-gb-laptop/">Google DeepMind Releases Gemma 4 12B: An Encoder - Free ...</a></li>
<li><a href="https://dev.to/gilles_hamelink_ea9ff7d93/unlocking-3d-understanding-the-rise-of-encoder-free-multimodal-models-b03">"Unlocking 3D Understanding: The Rise of Encoder - Free Multimodal ..."</a></li>

</ul>
</details>

**社区讨论**: 社区成员测试了 Q4 量化版本，报告结果不错，但注意到偶尔会出现语法错误，例如多余的括号或逗号。一些人对无编码器设计表示好奇，质疑这是否真正消除了编码。其他人称赞这是面向平价硬件的理想小模型方案，同时有用户质疑 Google 发布开源模型的商业动机。

**标签**: `#AI`, `#multimodal`, `#machine learning`, `#Gemma`, `#open source`

---

<a id="item-4"></a>
## [Let's Encrypt 计划通过默克尔树实现后量子证书](https://letsencrypt.org/2026/06/03/pq-certs) ⭐️ 9.0/10

Let's Encrypt 宣布计划采用基于默克尔树证书（MTC）的后量子证书，为量子计算时代做准备。该公告于 2026 年 6 月 3 日发布。 作为发行量最大的证书颁发机构，Let's Encrypt 向后量子密码学的过渡为整个互联网的安全基础设施树立了关键先例。此举应对了量子计算机破解当前公钥密码学的迫在眉睫的威胁，即所谓的“Q-Day”。 默克尔树证书是一种新的证书格式，集成了公开日志记录，以减少大量后量子签名和短寿命证书的开销。这一过渡涉及对 X.509 证书和证书透明度（Certificate Transparency）的重大变更，预计将是一个复杂的项目。

hackernews · SGran · Jun 3, 15:06 · [社区讨论](https://news.ycombinator.com/item?id=48385114)

**背景**: 后量子密码学（PQC）是指设计用于抵御量子计算机攻击的算法，量子计算机可以使用秀尔算法破解广泛使用的 RSA 和 ECDSA 等算法。NIST 在 2024 年发布了首批 PQC 标准。默克尔树证书（MTC）是一种提议的格式，它将证书颁发与公开日志记录相结合，旨在减少 TLS 握手中大型 PQC 签名的性能影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography</a></li>
<li><a href="https://www.ietf.org/archive/id/draft-davidben-tls-merkle-tree-certs-09.html">Merkle Tree Certificates</a></li>
<li><a href="https://blog.cloudflare.com/bootstrap-mtc/">Keeping the Internet fast and secure: introducing Merkle Tree Certificates</a></li>

</ul>
</details>

**社区讨论**: 社区成员表达了兴奋与担忧：有人指出我们正生活在‘科幻未来’中，另一个人则强调了替代数十年经过实战检验的基础设施所面临的挑战。一位开发者指出了当前证书透明度的局限性，并介绍了一个现有的 MTC 兼容实现 Cordon。还有用户询问 ed25519 签名的量子抗性。

**标签**: `#post-quantum cryptography`, `#Let's Encrypt`, `#Merkle Tree`, `#certificate transparency`, `#PKI`

---

<a id="item-5"></a>
## [优步将员工 AI 工具月支出上限设为 1500 美元](https://simonwillison.net/2026/Jun/3/uber-caps-usage/#atom-everything) ⭐️ 8.0/10

优步对每位员工每款 AI 编码工具实施了每月 1500 美元（约合 10800 元人民币）的代币支出上限，原因是员工大量使用 Claude Code 和 Cursor 等智能编码代理工具，导致公司 2026 年 AI 预算在四个月内超支。 这揭示了随着 AI 编码代理迅速普及，企业在成本管理上面临的实际挑战——设置支出上限可能成为普遍做法。同时，它也提供了一个衡量这些工具生产力价值的基准——约占工程师中位薪酬的 11%。 该上限按工具单独计算，因此同时使用 Cursor 和 Claude Code 的工程师每月合计最多可花费 3000 美元。个人订阅者目前受益于补贴计划，类似使用量仅需约 100 美元/月，但优步等大型企业无法享受此类计划。

rss · Simon Willison · Jun 3, 12:01 · [社区讨论](https://news.ycombinator.com/item?id=48383056)

**背景**: 像 Claude Code 和 Cursor 这样的 AI 编码代理是能够自主编辑代码、运行命令并协助开发者的工具。它们消耗大语言模型（LLM）的代币，成本随使用量增加。优步的 2026 年 AI 预算制定于 2025 年，当时尚未预见到此类工具的爆发式流行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社区讨论**: 社区评论在争论 AI 编码是一时热潮还是持续趋势，有评论指出企业已为每席位支付数千美元。其他人质疑轻量模型是否足够，并认为大模型在处理重大变更时仍需人工监督。一些评论强调应考虑工程师的全成本（包括办公空间、保险等）而不仅是薪资。

**标签**: `#AI`, `#cost management`, `#enterprise`, `#coding agents`, `#productivity`

---

<a id="item-6"></a>
## [DaVinci Resolve 21 发布，新增照片管理和 AI 工具](https://www.blackmagicdesign.com/products/davinciresolve/whatsnew) ⭐️ 8.0/10

Blackmagic Design 发布了 DaVinci Resolve 21，这是一个重要更新，引入了全新的照片管理和编辑模块，增强了动态图形工具，并提供了多项 AI 功能，如物体移除和人脸识别。 此次发布显著扩展了 DaVinci Resolve 在视频制作之外的功能，进入了照片管理领域，有可能挑战像 Lightroom 和 Affinity Photo 这样的专业工具。同时，它为缺乏强大照片编辑选项的 Linux 用户提供了一个极具吸引力的替代方案。 此次更新包括对 Fusion 动态图形的全面改造，新增了 Fusion 模板，DaVinci Neural Engine 现在支持 ‘Ultra Beauty’ 和 ‘Surface Tracking’ 等 AI 功能。照片管理模块支持导入、整理和编辑 RAW 照片，并可使用调色工具。

hackernews · pentagrama · Jun 3, 14:18 · [社区讨论](https://news.ycombinator.com/item?id=48384482)

**背景**: DaVinci Resolve 是由 Blackmagic Design 开发的专业非线性视频编辑和调色应用。它历来专注于视频后期制作，但第 21 版首次大规模扩展到照片编辑领域。DaVinci Neural Engine 是一个机器学习系统，为软件中的各种 AI 辅助功能提供支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DaVinci_Resolve">DaVinci Resolve - Wikipedia</a></li>
<li><a href="https://www.blackmagicdesign.com/products/davinciresolve/whatsnew">DaVinci Resolve – What’s New | Blackmagic Design</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极，用户称赞照片管理功能可能成为 Linux 照片编辑的变革者。一些人对大量 AI 功能的营销感到厌倦，但承认它们在编辑工作流程中的实际好处。

**标签**: `#davinci-resolve`, `#video-editing`, `#blackmagic-design`, `#photo-management`, `#ai`

---

<a id="item-7"></a>
## [乐鑫发布 ESP32-S31：内置 SIMD 指令的 RISC-V SoC](https://www.espressif.com/en/products/socs/esp32-s31) ⭐️ 8.0/10

乐鑫科技发布了 ESP32-S31，一款主频高达 320 MHz 的双核 RISC-V 微控制器，内置 SIMD 指令，支持无需专有工具链的 Rust 嵌入式开发。 这款芯片允许通过 `rustup target add riscv32imac-unknown-none-elf` 使用标准 Rust 工具链，降低了对专有 SDK 的依赖。同时为低成本物联网设备带来 SIMD 能力，扩展了性能可能性。 ESP32-S31 具备 60 个 GPIO，一个类似于树莓派 Pico PIO 的 Bitscrambler 外设，用于灵活的数据转换，专为需要多协议连接和丰富人机界面的高级物联网应用设计。

hackernews · volemo · Jun 3, 16:10 · [社区讨论](https://news.ycombinator.com/item?id=48385965)

**背景**: RISC-V 是一种开源指令集架构，支持自定义扩展。SIMD（单指令多数据）允许一条指令并行处理多个数据点，提升音频/视频处理等任务的性能。此前乐鑫的 ESP32 芯片使用 Tensilica Xtensa 内核，转向 RISC-V 为开源工具链打开了更多可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.espressif.com/en/products/socs/esp32-s31">ESP32-S31 Dual-Core RISC-V + Multi-Protocol SoC | Espressif Systems</a></li>
<li><a href="https://en.wikipedia.org/wiki/Single_instruction,_multiple_data">Single instruction , multiple data - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/ESP32-S2">ESP32-S2</a></li>

</ul>
</details>

**社区讨论**: 社区对 SIMD 指令和 Rust 支持表现出极大热情，有评论者指出 RISC-V 内核使得编译变得像 `rustup target add` 一样简单。也有讨论关于命名混乱的问题，许多芯片尽管架构不同都叫“ESP32”，还有评论提到 Bitscrambler 外设与 PIO 的相似性。

**标签**: `#ESP32`, `#RISC-V`, `#Embedded Systems`, `#Espressif`, `#Rust`

---

<a id="item-8"></a>
## [数学家警告 AI 快速发展](https://www.science.org/content/article/mathematicians-issue-warning-ai-rapidly-gains-ground) ⭐️ 8.0/10

数学家们就人工智能在数学研究中的快速发展发出正式警告，表达了对归属、验证以及该领域潜在颠覆性影响的担忧。 这一警告意义重大，因为其来自数学界的权威声音，突出了对 AI 影响研究诚信及人类在该领域角色的深层担忧。 警告关注 AI 生成和验证证明的能力，可能使人类数学家边缘化。社区讨论揭示了广泛的观点，从对无关紧要的恐惧到与过去技术颠覆的比较。

hackernews · pseudolus · Jun 3, 10:05 · [社区讨论](https://news.ycombinator.com/item?id=48382052)

**背景**: 人工智能，尤其是大型语言模型，在科学研究中应用日益广泛。在数学领域，AI 已被用于证明定理和发现模式，引发了关于人类直觉和严格验证作用的疑问。

**社区讨论**: 评论显示出复杂情绪：一些人将其与受 AI 影响的艺术家和作者相类比，另一些人指出 AI 适用于实际问题，还有少数人担心未来人类在数学过程中变得无关紧要。

**标签**: `#AI`, `#mathematics`, `#research ethics`, `#machine learning`

---

<a id="item-9"></a>
## [原始 PlayStation 架构深度分析](https://www.copetti.org/writings/consoles/playstation/) ⭐️ 8.0/10

Rodrigo Copetti 对原始 PlayStation 硬件的实用分析在 Hacker News 上被重新分享，详细介绍了 CPU、内存映射和图形系统，并附有注解图和说明。 这份全面的资源帮助复古开发者、模拟器作者和爱好者理解 PS1 的独特设计约束和创新，这对于经典游戏的精确模拟和保存至关重要。 PlayStation 使用 33.8688 MHz 的 32 位 MIPS R3000A CPU，配备几何变换引擎（GTE）进行 3D 向量数学运算，其内存映射包含一个 1 KB 的暂存区，映射到数据缓存上供开发者快速访问。

hackernews · gregsadetsky · Jun 3, 10:24 · [社区讨论](https://news.ycombinator.com/item?id=48382142)

**背景**: 原始 PlayStation 于 1994 年发布，是普及 3D 游戏的代表性主机。其架构将定制 CPU、GPU 和声音处理器集成在一块主板上，并采用内存映射技术实现高效数据访问。了解这些细节对于模拟和自制软件开发至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.copetti.org/writings/consoles/playstation/">PlayStation Architecture | A Practical Analysis</a></li>
<li><a href="https://psx-spx.consoledev.net/memorymap/">Memory Map - PlayStation Specifications - psx-spx</a></li>
<li><a href="https://en.wikipedia.org/wiki/PlayStation_technical_specifications">PlayStation technical specifications - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了技术轶事，包括《合金装备》中的一个技巧，通过将指针与地址标志进行 OR 操作来编码炸弹放置位置。其他人则称赞了网站的设计，并询问使用 JavaScript 或 WebAssembly 的 PS1 网页模拟器推荐。

**标签**: `#PlayStation`, `#console architecture`, `#retro gaming`, `#hardware`, `#computer engineering`

---

<a id="item-10"></a>
## [谷歌允许网站退出 AI 搜索结果](https://9to5google.com/2026/06/02/google-ai-mode-overviews-opt-out/) ⭐️ 8.0/10

谷歌在 Search Console 中新增了一个开关，允许网站所有者选择退出 AI Overviews 和 AI Mode 的展示，且不影响其常规搜索结果排名和 Discover 信息流的显示。该功能目前在英国测试，随后将向全球推广。 这一政策变化赋予了发布者对谷歌 AI 功能如何使用其内容前所未有的控制权，解决了长期存在的对 AI 摘要导致流量流失和不准确性的担忧。它为在搜索生态系统中平衡 AI 创新与网站所有者权利树立了先例。 退出选项适用于 AI Overviews、AI Mode 以及 Discover 中的 AI Overviews，而常规搜索结果和 Discover 信息流不受影响。谷歌同时还推出了 Search Console 中的生成式 AI 搜索统计数据，帮助网站所有者追踪展示量和性能。

telegram · zaihuapd · Jun 3, 12:00

**背景**: AI Overviews 是谷歌搜索的一项功能，可生成 AI 驱动的搜索结果摘要，但因不准确和减少网站点击率而受到批评。Google Discover 是一个个性化内容信息流，根据用户兴趣推荐文章。Search Console 是一个免费工具，供网站管理员监控和优化其网站在谷歌搜索中的表现。此次退出选项是在英国监管机构施压和发布者抱怨 AI 生成内容导致流量下降后推出的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://9to5google.com/2026/06/02/google-ai-mode-overviews-opt-out/">Google will let websites opt-out of AI Mode & Overviews in Search</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_AI_Overviews">Google AI Overviews</a></li>
<li><a href="https://the-decoder.com/google-lets-sites-opt-out-of-ai-search-results-knowing-most-have-nowhere-else-to-go/">Google lets sites opt out of AI search results, knowing most have nowhere else to go</a></li>

</ul>
</details>

**标签**: `#Google`, `#AI Search`, `#Search Console`, `#SEO`, `#AI Overviews`

---

<a id="item-11"></a>
## [千问向第三方智能体和技能全面开放平台](https://www.stcn.com/article/detail/3941333.html) ⭐️ 8.0/10

千问应用宣布向第三方智能体（Agent）和技能（Skill）全面开放，允许企业在平台上运营自己的品牌智能体。首批测试企业包括瑞幸、肯德基、东方航空等。 这一举措标志着阿里巴巴在构建 AI 智能体生态系统方面的战略推进，类似于 OpenAI 的 GPT 商店，为企业广泛采用和定制提供了可能。这将加速各行各业的企业 AI 集成。 平台开放覆盖了智能体（Agent）和技能（Skill）两类，企业可部署针对自身服务定制的品牌智能体。首批企业来自餐饮、航空等行业。

telegram · zaihuapd · Jun 3, 12:15

**背景**: AI 智能体是使用大语言模型和外部工具自主执行复杂任务的程序。技能（Skill）是可复用的能力定义，规定了 AI 在特定工作流中的行为。千问（又称通义千问）是阿里云的大语言模型系列。向第三方开发者开放平台紧跟了构建平台化 AI 生态系统的趋势，类似于 OpenAI 的 GPTs。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/insights/enterprise-ai-agents">Enterprise AI Agents: Beyond Productivity | IBM</a></li>
<li><a href="https://www.youmaximize.com/blog/the-ai-skills-vault-how-to-build-reusable-ai-skills-for-video-saas-and-design-workflows">The AI Skills Vault: How to Build Reusable AI Skills for... | YouMaximize</a></li>

</ul>
</details>

**标签**: `#AI`, `#enterprise AI`, `#Qianwen`, `#agents`, `#platform opening`

---

<a id="item-12"></a>
## [HTTP/2 Bomb 远程击垮主流服务器](https://blog.calif.io/p/codex-discovered-a-hidden-http2-bomb) ⭐️ 8.0/10

研究人员披露了一种名为 HTTP/2 Bomb 的新型拒绝服务攻击，它利用 HPACK 压缩放大和类似 Slowloris 的连接占用技术耗尽服务器内存，影响 NGINX、Apache HTTPD、Microsoft IIS、Envoy 和 Cloudflare Pingora 的默认 HTTP/2 配置。 该攻击至关重要，因为它能通过 100 Mbps 家用网络在数秒内使数十万网站瘫痪，且多款主流服务器尚未修复，构成广泛的远程拒绝服务威胁。 单个客户端可在约 20 秒内占用 Apache httpd 或 Envoy 的 32 GB 内存；NGINX 已在 1.29.8+ 中修复，Apache 在 mod_http2 v2.0.41 中修复，而 IIS、Envoy 和 Pingora 目前尚无补丁。

telegram · zaihuapd · Jun 3, 15:00

**背景**: HPACK 是 HTTP/2 中使用的头部压缩方案，可将小输入放大为大量解压数据；Slowloris 是一种经典 DoS 攻击，通过缓慢保持大量连接来耗尽服务器资源。HTTP/2 Bomb 将两者结合：压缩炸弹快速分配内存，而连接保持阻止内存释放，从而导致内存迅速耗尽。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cyberinsider.com/new-http-2-bomb-attack-can-exhaust-server-memory-in-seconds/">New “HTTP/2 Bomb” attack can exhaust server memory in seconds | CyberInsider</a></li>
<li><a href="https://thehackernews.com/2026/06/new-http2-bomb-vulnerability-allows.html">New HTTP/2 Bomb Vulnerability Allows Remote DoS on NGINX, Apache, IIS, Envoy & Cloudflare</a></li>
<li><a href="https://www.securityweek.com/http-2-bomb-exploit-knocks-web-servers-offline-in-seconds/">'HTTP/2 Bomb' Exploit Knocks Web Servers Offline in Seconds - SecurityWeek</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#HTTP/2`, `#denial-of-service`, `#web server`

---

<a id="item-13"></a>
## [奥特曼：OpenAI 内部最高用户月消耗约 1000 亿 token](https://www.businessinsider.com/sam-altman-openai-top-token-spender-ai-costs-issue-2026-6) ⭐️ 8.0/10

Sam Altman 在企业活动上透露，OpenAI 内部最高用户每月消耗约 1000 亿个 token，外部用户消耗更多。他还提到，6 年半前最高用户每月只消耗 10 万个 token，当时可能已是全球领先水平，而如今这仅是全球平均水平。 这一披露凸显了 AI 模型使用规模的大幅增长以及随之而来的成本压力，将影响整个行业的定价策略和模型效率改进。它揭示了大规模部署先进 AI 的经济挑战——成本已成为一个“巨大问题”，OpenAI 正在积极应对。 Altman 提到 OpenAI 内部有鼓励高 token 使用的文化，但 AI 成本压力正在升高。他指出，2026 年初成本问题还很少被提起（可能是口误或未来指代，根据上下文指现在），现在已经成了“巨大问题”，公司正改进模型以用更低支出提供更多价值。

telegram · zaihuapd · Jun 4, 02:31

**背景**: 在 OpenAI 的 GPT 系列等 AI 模型中，token 是文本处理的基本单元，短可以是一个字符，长可以是一个单词，模型按 token 数量收费。从每月 10 万 token 到 1000 亿 token 的剧增，反映了 AI 采用的指数级增长以及对更高效架构的需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/ai-tokens-explained/">What Are AI Tokens ? The Language and Currency... | NVIDIA Blog</a></li>
<li><a href="https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them">What are tokens and how to count them? | OpenAI Help Center</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI costs`, `#token usage`, `#scaling AI`

---