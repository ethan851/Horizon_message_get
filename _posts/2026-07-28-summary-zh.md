---
layout: default
title: "Horizon Summary: 2026-07-28 (ZH)"
date: 2026-07-28
lang: zh
---

> From 25 items, 9 important content pieces were selected

---

1. [月之暗面发布开源权重模型 Kimi K3，参数达 2.8 万亿](#item-1) ⭐️ 9.0/10
2. [Fastjson 1.x 发现无需 gadget 的高危 RCE 漏洞](#item-2) ⭐️ 9.0/10
3. [Anthropic 澄清对开放权重 AI 模型的立场](#item-3) ⭐️ 8.0/10
4. [法官驳回谷歌利用 DMCA 禁止爬取搜索结果](#item-4) ⭐️ 8.0/10
5. [Libsm64 将超级马里奥 64 转变为可复用的游戏库](#item-5) ⭐️ 8.0/10
6. [谷歌 CEO 预告 Gemini 4，称其为最雄心勃勃的预训练项目](#item-6) ⭐️ 8.0/10
7. [中方驳美方拟制裁中国 AI 企业：模型蒸馏是通用技术](#item-7) ⭐️ 8.0/10
8. [中芯国际测试国产首台 DUV 光刻机](#item-8) ⭐️ 8.0/10
9. [月之暗面将开源 Kimi-K3，全球首个 3T 级前沿模型](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [月之暗面发布开源权重模型 Kimi K3，参数达 2.8 万亿](https://t.me/zaihuapd/42793) ⭐️ 9.0/10

月之暗面发布了 Kimi K3，这是首个参数规模达 2.8 万亿的开源权重模型，在前端代码竞技场中以 1679 分超越 Claude Fable 5，跃居第一。 Kimi K3 的开源权重发布和顶尖基准表现，为大型语言模型设立了新标准，尤其在前端代码生成领域，其新颖的 Kimi Delta Attention 架构可能影响未来模型设计。 Kimi K3 采用名为 Kimi Linear 的混合线性注意力架构，其中 Kimi Delta Attention 与全局注意力的比例为 3:1，KV 缓存使用量减少高达 75%，并支持 100 万 token 的上下文窗口。

telegram · zaihuapd · Jul 27, 06:27

**背景**: 大型语言模型通常使用全注意力机制，在长上下文场景下计算成本高昂。Kimi Delta Attention 通过逐通道衰减控制扩展了 Gated DeltaNet，实现了高效的线性注意力。2.8 万亿的参数规模使 K3 成为迄今为止最大的开源权重模型之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2510.26692">[2510.26692] Kimi Linear: An Expressive, Efficient Attention ... GitHub - MoonshotAI/Kimi-Linear GitHub - hwilner/kimi-delta-attention: Educational ... Linear Attention: Kimi Delta Attention | Jianyu Huang Kimi Delta Attention - Papers with Code Kimi Linear: An Expressive, Efficient Attention Architecture Kimi K3 Technical Advancements Explained - nextbigfuture.com</a></li>
<li><a href="https://x.com/arena/status/2077824029126504525">Arena.ai on X: "Big news: Kimi-K3 by @Kimi_Moonshot is now #1 in the Frontend Code Arena with 1679 pts, surpassing Claude Fable 5. This is a 17-place jump from Kimi-k2.6 (#18 -> #1). In Frontend, Kimi-K3 ranked #1 in 6 of 7 domains: Brand & Marketing, Reference-Based Design, Data & Analytics, Consumer Product, Simulations, and Content Creation Tools, landing #2 only in Gaming behind Fable 5. The full model weights will be released by July 27. Congrats to the @Kimi_Moonshot team on this major milestone!" / X</a></li>
<li><a href="https://aitoolhunt.co/blog/kimi-k3-benchmarks-frontend-code-arena-2026">Kimi K3 Benchmarks: Frontend Leap and Review Verdicts (2026) | AIToolHunt</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#open-source`, `#benchmark`

---

<a id="item-2"></a>
## [Fastjson 1.x 发现无需 gadget 的高危 RCE 漏洞](https://t.me/zaihuapd/42797) ⭐️ 9.0/10

安全研究人员 Kirill Firsov 披露了 Fastjson 1.2.68 至 1.2.83 版本中存在高危远程代码执行漏洞。该漏洞无需 gadget 链，也无需开启 autoType 支持，可在 JDK 8、17 和 21 上利用。 该漏洞极其严重，因为它绕过了传统的反序列化防护（无需 gadget 和 autoType），影响大量 Java 应用。由于 Fastjson 1.x 已停止维护，用户必须升级到 Fastjson2 才能保持安全。 该漏洞影响 Fastjson 1.2.68 至 1.2.83 版本，可在多个 JDK 版本上利用，无需 classpath gadget 或 autoType。官方已于 2024 年 10 月停止维护 Fastjson 1.x，极不可能发布补丁。

telegram · zaihuapd · Jul 27, 10:31

**背景**: Fastjson 是 Java 中常用的 JSON 库，常用于序列化/反序列化。在 Java 反序列化中，“gadget 链”是一系列类，在反序列化时可导致任意代码执行。“autoType”是 Fastjson 的一个特性，允许在 JSON 中指定类型信息，攻击者可能滥用。此漏洞的特殊之处在于它既不依赖 gadget 链也不依赖 autoType，使得利用更加容易。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/alibaba/fastjson/wiki/enable_autotype">enable_autotype · alibaba/fastjson Wiki · GitHub</a></li>

</ul>
</details>

**标签**: `#安全`, `#漏洞`, `#Fastjson`, `#RCE`, `#高危`

---

<a id="item-3"></a>
## [Anthropic 澄清对开放权重 AI 模型的立场](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic 发布声明，否认主张禁止开放权重模型，但呼吁对所有足够强大的模型（包括开放和封闭模型）进行强制性安全测试。 作为领先的 AI 实验室，Anthropic 的立场影响了关于 AI 监管和开源开发的辩论，批评者指责其偏向有利于自身商业模式的监管俘获。 该声明是在社区强烈反对后发布的，澄清 Anthropic 不支持禁令，但同时也支持限制对华芯片销售和打击走私等措施，一些人认为这与其反禁令立场相矛盾。

hackernews · surprisetalk · Jul 27, 22:03 · [社区讨论](https://news.ycombinator.com/item?id=49076057)

**背景**: 开放权重模型是指核心组件公开发布的 AI 模型，任何人都可以下载、检查、修改和运行。它们是开源 AI 生态系统的关键部分，使得更广泛的使用成为可能，但也因潜在滥用而引发安全担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍持批评态度，许多人指责 Anthropic 通过繁重的测试要求倡导事实上的禁令。评论者还指出前后矛盾之处，例如支持硬件禁令同时否认支持软件禁令，并认为该立场背后有商业动机。

**标签**: `#open-weights`, `#AI safety`, `#regulation`, `#Anthropic`, `#AI ethics`

---

<a id="item-4"></a>
## [法官驳回谷歌利用 DMCA 禁止爬取搜索结果](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

一名美国法官裁定，谷歌不能利用《数字千年版权法》（DMCA）阻止第三方服务爬取其公开的搜索结果，这标志着一个重要的法律先例。 该裁决维护了爬取公开数据的合法性，对竞争、透明度以及 SEO 分析等工具至关重要。它也凸显了谷歌自身的讽刺之处——它建立在爬取网络的基础上，却试图阻止他人这样做。 该案件涉及谷歌起诉 SerpAPI（一种爬取谷歌搜索结果的服務）。法官驳回了谷歌关于爬取行为构成 DMCA 下版权侵权的论点，指出搜索结果是事实的汇编，不具备足够的创造性来获得版权保护。

hackernews · cdrnsf · Jul 27, 18:15 · [社区讨论](https://news.ycombinator.com/item?id=49073513)

**背景**: 《数字千年版权法》包含反规避条款，禁止绕过保护版权作品的技术措施。谷歌试图主张爬取其搜索结果违反了这些条款，但法院不同意，因为数据本身不受版权保护。该裁决强化了一个观点：在美国，只要不违反其他法律，爬取公开可访问的数据通常是合法的。

**社区讨论**: 评论表达了对谷歌取消廉价 API 的不满，用户指出他们依赖第三方爬虫作为替代方案。一些人指出谷歌自身的讽刺之处——它建立在爬取网络的基础上——却利用 DMCA 阻止爬虫。其他人则强调了社会效益，例如检测广告欺诈行为。

**标签**: `#scraping`, `#DMCA`, `#Google`, `#copyright`, `#legal`

---

<a id="item-5"></a>
## [Libsm64 将超级马里奥 64 转变为可复用的游戏库](https://github.com/libsm64/libsm64) ⭐️ 8.0/10

libsm64 是一个逆向工程库，它提取了《超级马里奥 64》的角色和物理特性，使得马里奥可以在《半条命 2》等外部游戏引擎中作为可玩角色使用。 该项目实现了创造性的跨游戏混搭，展示了一种实用的、非区块链的互操作性方法，而这正是元宇宙所承诺的。开发者现在可以轻松地将马里奥集成到自己的项目中，无需从头实现他复杂的移动机制。 该库提供了定义在 libsm64.h 中的最小 API，客户端只需包含该头文件并链接共享库。社区成员已经创建了诸如《半条命 2》中的马里奥等演示，并维护了一个使用 libsm64 的项目精选列表。

hackernews · klaussilveira · Jul 27, 10:04 · [社区讨论](https://news.ycombinator.com/item?id=49067352)

**背景**: 《超级马里奥 64》是 1996 年为任天堂 64 发布的平台游戏，以其标志性角色马里奥和精确的 3D 移动机制而闻名。libsm64 逆向工程了原始游戏的可执行文件，将角色的动画、物理和控制逻辑提取为独立的 C 语言库，并可以编译到多个平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/libsm64/libsm64">GitHub - libsm64/libsm64: Mario 64 as a library for use in external game engines · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区成员对此充满热情，称该库令人难以置信，是无需炒作即可实现的元宇宙。有人分享了马里奥在《半条命 2》中的演示视频，一条评论开玩笑地建议将“马里奥 64 作为服务出售”，同时安抚任天堂不要起诉。另一位用户指向了一个包含有趣项目的 awesome-libsm64 列表。

**标签**: `#reverse engineering`, `#game development`, `#interoperability`, `#retro gaming`, `#libraries`

---

<a id="item-6"></a>
## [谷歌 CEO 预告 Gemini 4，称其为最雄心勃勃的预训练项目](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 8.0/10

谷歌 CEO Sundar Pichai 在 Alphabet 2026 年第二季度财报电话会议上宣布，下一代大语言模型 Gemini 4 已投入预训练，这是该公司迄今为止最具雄心的项目，计划于 2026 年底发布。 这表明谷歌致力于通过构建更大的基础模型来保持 AI 前沿的领导地位，直接影响与 OpenAI 和 Anthropic 等竞争对手的竞争格局。 Pichai 强调，谷歌将优先将算力分配给前沿 AGI 研究，以确保 Gemini 4 发布时仍处于最前沿。Gemini 3.x Flash 系列将继续以近乎每月一次的频率更新，重点提升智能编码能力。

telegram · zaihuapd · Jul 27, 04:06

**背景**: 预训练是大语言模型在针对特定任务进行微调之前，从海量文本语料库中学习广泛语言理解的基础阶段。AGI（通用人工智能）指的是在几乎所有任务上匹配或超越人类认知能力的假设性 AI。谷歌的 Gemini 系列是其旗舰多模态 AI 模型家族，直接与 OpenAI 的 GPT 系列等竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sapien.io/blog/fine-tuning-vs-pre-training-key-differences-for-language-models">Fine-Tuning vs. Pre-Training: Their Impact on Language Models</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artificial_general_intelligence">Artificial general intelligence - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI`, `#Google`, `#Gemini`, `#Large Language Model`, `#Pretraining`

---

<a id="item-7"></a>
## [中方驳美方拟制裁中国 AI 企业：模型蒸馏是通用技术](https://www.mofcom.gov.cn/syxwfb/art/2026/art_7f1622463a7c48ef9fad600ce0ef702f.html) ⭐️ 8.0/10

中国商务部正式驳斥美方因所谓“蒸馏”美国 AI 模型而调查并制裁中国 AI 企业的威胁，称相关指控毫无根据。 这一争端凸显了中美科技紧张局势的升级，可能扰乱全球 AI 研究合作，因为模型蒸馏是包括美国企业在内的全球公司广泛使用的技术。 商务部指出，近 200 家美国初创企业已呼吁政府不要限制访问中国开源模型，并警告如果中方利益受到实质性损害，将采取必要措施维护中国企业合法权益。

telegram · zaihuapd · Jul 27, 11:01

**背景**: 模型蒸馏是一种机器学习技术，较小的“学生”模型从较大的“教师”模型中学习，常用于创建高效的 AI 系统。该技术在 AI 行业中被广泛采用，以提高性能并降低计算成本。美国近期担忧中国企业可能利用蒸馏复制美国专有 AI 模型，从而发出制裁威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://www.cnbc.com/2026/07/25/hat-is-distillation-and-why-is-everyone-so-obsessed-with-it-this-week.html">From Silicon Valley to DC, the tech world is suddenly obsessed with one concept in AI: Distillation</a></li>
<li><a href="https://labelbox.com/guides/model-distillation/">What is Model Distillation?</a></li>

</ul>
</details>

**标签**: `#AI`, `#model distillation`, `#trade sanctions`, `#China`, `#US`

---

<a id="item-8"></a>
## [中芯国际测试国产首台 DUV 光刻机](https://t.me/zaihuapd/42800) ⭐️ 8.0/10

中芯国际正在试运行上海初创公司宇量昇研发的中国首台国产先进深紫外（DUV）光刻机，目标实现 28 纳米生产，并可能通过多重图形化工艺达到 7 纳米，计划在 2027 年前实现量产。 这标志着中国在半导体自主化进程中迈出了重要一步，减少了对 ASML 的 DUV 设备的依赖，并绕过了美国对 EUV 光刻机的出口限制。然而，该设备仍处于早期阶段，在良率和规模化方面面临挑战。 该光刻机采用 193nm 氟化氩（ArF）激光技术，与 ASML 的 Twinscan 系列类似，大部分零部件已实现国产化，但仍依赖部分进口。中芯国际正尝试通过多重图形化技术达到 7 纳米，甚至以较低良率挑战 5 纳米。

telegram · zaihuapd · Jul 27, 14:10

**背景**: 深紫外（DUV）光刻技术利用深紫外光谱（如 193nm 波长）的光在硅片上绘制电路图案，用于芯片制造。多重图形化光刻使用多个光掩模来获得比单次曝光更精细的图案，这是在没有极紫外（EUV）工具的情况下生产 7 纳米等先进节点的关键。美国限制了 ASML 的 EUV 设备对华销售，因此国产 DUV 的发展对中国先进芯片目标至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DUV_lithography">DUV lithography</a></li>
<li><a href="https://eureka.patsnap.com/article/duv-lithography-explained-how-193nm-arf-lasers-enable-7nm-nodes">DUV Lithography Explained: How 193nm ArF Lasers Enable 7nm...</a></li>
<li><a href="https://eureka.patsnap.com/article/multi-patterning-lithography-why-do-we-need-multiple-masks">Multi - Patterning Lithography : Why Do We Need Multiple Masks?</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#lithography`, `#SMIC`, `#DUV`, `#China tech`

---

<a id="item-9"></a>
## [月之暗面将开源 Kimi-K3，全球首个 3T 级前沿模型](https://t.me/zaihuapd/42802) ⭐️ 8.0/10

月之暗面宣布将开源 Kimi-K3，这是一个基于全新 Kimi Delta 注意力机制和注意力残差架构的 2.8 万亿参数模型，权重预计于 2026 年 7 月 27 日在 Hugging Face 发布。 作为首个开源 3T 级模型，Kimi-K3 将开源大语言模型的规模推向新前沿，有望加速长程编程、知识工作和复杂推理领域的研究，让更多人能够使用尖端 AI 能力。 Kimi-K3 拥有 100 万 token 的上下文窗口、原生视觉能力以及工具调用和多步规划等智能体能力，这些均由其 Kimi Delta 注意力机制和注意力残差架构实现。权重将在公告约一年后，即 2026 年 7 月发布。

telegram · zaihuapd · Jul 27, 15:15

**背景**: 大语言模型是具有数十亿参数的神经网络，参数量通常与能力相关。开源大语言模型，如 Meta 的 Llama 或 Mistral，允许研究人员和开发者检查、修改并在自己的硬件上运行模型。Kimi Delta 注意力机制是一种线性注意力机制，支持高效的长上下文处理；而注意力残差则用可学习的、依赖输入的方式聚合前层输出，替代了标准的残差连接，提升了表示质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/kimi-delta-attention">Kimi Delta Attention : Delta ‐Rule Linear Mechanism</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>

</ul>
</details>

**标签**: `#AI`, `#open-source`, `#large language model`, `#Kimi-K3`, `#Moonshot AI`

---