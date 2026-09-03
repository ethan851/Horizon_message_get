---
layout: default
title: "Horizon Summary: 2026-09-03 (ZH)"
date: 2026-09-03
lang: zh
---

> From 30 items, 7 important content pieces were selected

---

1. [谷歌发布 Gemini 3.8 Flash 与 3.8 Flash Cyber 模型](#item-1) ⭐️ 9.0/10
2. [Meta 推出 Muse Spark 1.3：以低成本实现接近 SOTA 的性能](#item-2) ⭐️ 8.0/10
3. [谷歌避免广告技术业务被强制拆分](#item-3) ⭐️ 8.0/10
4. [报告：三个内容农场生成 21.5 万个“最佳软件”页面，被 Perplexity 引用](#item-4) ⭐️ 8.0/10
5. [Paint.NET 借助 Claude 重写 Direct2D，初步支持 WINE 运行](#item-5) ⭐️ 8.0/10
6. [阿里发布 Qwen3.8-Max-0902，CodeArena 编程榜 1691 分夺冠](#item-6) ⭐️ 8.0/10
7. [xAI 发布 Grok 4.6，强化长时间运行智能体任务](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [谷歌发布 Gemini 3.8 Flash 与 3.8 Flash Cyber 模型](https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/) ⭐️ 9.0/10

谷歌发布了 Gemini 3.8 Flash 和 Gemini 3.8 Flash Cyber。3.8 Flash 在多项基准测试中名列前茅，能以极低成本快速生成 HTML 和 JavaScript；Cyber 版本则定位为谷歌在漏洞检测与自动修复方面最强的新一代网络安全模型，通过新的 Fairwind 计划向可信防御者提供。 此次发布扩充了谷歌 Flash 系列低成本、低延迟模型，也体现了当前 AI 行业所期望的快速迭代节奏。由于 Gemini 3.8 Flash 在智能水平评分上接近更大规模的旗舰模型，它可能让开发者、初创企业和媒体分析任务以更低成本获得强大的 AI 能力。 据 Artificial Analysis 数据，Gemini 3.8 Flash 的智能评分为 59，与 Opus 5 medium 相同；社区测试显示，一次生成约耗时 13 秒、花费约 1.8 美分。Cyber 版本取代了此前的 3.5 版，起初仅向“可信防御者”提供而非公众；还有社区成员指出，低思考强度设置下的表现可能相比 3.7 有所回退。

hackernews · bratao · Sep 2, 15:12 · [社区讨论](https://news.ycombinator.com/item?id=49537553)

**背景**: Gemini 是 Google DeepMind 的大规模多模态 AI 模型系列，分为 Ultra、Pro、Flash 等不同层级。Flash 系列主打速度、效率和低成本，同时保留较强的推理与编程能力，因此常用于 agentic 和高并发应用。本次发布延续了谷歌快速更新的节奏——3.8 Flash 是其六周内发布的第三款 Flash 模型——同时还推出了面向漏洞识别、补丁生成等防御性安全场景的 Cyber 专用版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/3-8-flash-and-3-8-flash-cyber/">Introducing Gemini 3.8 Flash and 3.8 Flash Cyber</a></li>
<li><a href="https://arstechnica.com/ai/2026/09/google-releases-gemini-3-8-flash-its-third-flash-model-in-six-weeks/">Google releases Gemini 3.8 Flash, its third Flash model in six weeks - Ars Technica</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论总体积极但带保留。Simon Willison 特别称赞了模型的速度和出色的 HTML/JavaScript 生成能力，并分享了一个 1.8 美分的示例；其他用户报告它在 DeepSwe 上超过了 Opus 5，jampa 则认可其行程规划与文档解析质量。也有人提出了注意事项：Willison 观察到 3.8 在低思考强度设置下的表现可能相比 3.7 回退，并有多位评论者指出 Gemini Flash 原生支持音频/视频输入仍是相对 OpenAI 和 Anthropic 旗舰模型的优势。

**标签**: `#AI`, `#Google Gemini`, `#Machine Learning`, `#Benchmarks`, `#Product Launch`

---

<a id="item-2"></a>
## [Meta 推出 Muse Spark 1.3：以低成本实现接近 SOTA 的性能](https://developer.meta.com/ai/models/muse-spark/) ⭐️ 8.0/10

Meta 发布了 Muse Spark 1.3，这是由 Meta Superintelligence Labs（MSL）打造的 Muse 系列 LLM 的最新版本。它公布了接近前沿的成绩，例如 DeepSWE 得分 75.4，而且单次示例查询只需几美分。 这一发布表明，接近 SOTA 的模型质量不再必然伴随高端定价，先进的编码辅助对预算有限的开发者来说也更易获得。它带来的竞争压力很可能会推动整个行业的模型价格下降。 Muse Spark 1.3 针对长周期编码工作流进行了优化：它会跟踪上下文和先前结果，能够处理杂乱或相互矛盾的输入，并以更少的不必要交互生成更干净的输出。它的“contributor”特殊定价档位明确表示，Meta 可以用用户数据训练模型，以换取更低价格。

hackernews · bvaldivielso · Sep 2, 19:35 · [社区讨论](https://news.ycombinator.com/item?id=49541256)

**背景**: Muse Spark 是 Meta 通过 Meta Superintelligence Labs（MSL）开发的大型语言模型系列。SOTA（State-of-the-Art，最先进水平）指在特定时间点、特定任务或基准测试中已报告的最佳性能，因此“接近 SOTA”意味着该模型接近顶级结果，但不一定在每个基准上都领先。日常的 LLM 用途（如代码生成和工具调用）不仅看原始质量，也看成本和延迟，因此低价且接近 SOTA 的模型会受到关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Muse_Spark">Muse Spark - Wikipedia</a></li>
<li><a href="https://developer.meta.com/ai/models/muse-spark/">Muse Spark 1.3 | Meta</a></li>
<li><a href="https://research.meta.ai/blog/introducing-muse-spark-1-3">Introducing Muse Spark 1.3 | Meta AI Research</a></li>

</ul>
</details>

**社区讨论**: 评论区整体非常正面：Simon Willison 提到 Muse Spark 1.3 用约 4.2 美分、38 秒生成了比 1.2 版本更好的 SVG。还有人强调其 DeepSWE 得分 75.4 是目前所见最佳成绩，并预测竞争会推动价格下降。一些用户指出它不是前沿模型，但仍认为它在日常工作中很有价值，并对 Meta 明确的“contributor”数据训练权衡表示赞赏。

**标签**: `#AI`, `#Meta`, `#LLM`, `#machine learning`, `#model release`

---

<a id="item-3"></a>
## [谷歌避免广告技术业务被强制拆分](https://www.nytimes.com/2026/09/02/technology/google-ad-tech-remedies.html) ⭐️ 8.0/10

美国法院拒绝强制谷歌出售其广告技术业务，尽管谷歌此前已被认定在该市场拥有非法垄断地位。这一决定使谷歌避免了被拆分，分析师指出该广告技术部门仅占 Alphabet 利润不到 1%。 这项裁决意义重大，因为它为美国反垄断补救措施在重塑大型科技公司权力方面划定了界限。它影响谷歌母公司 Alphabet 以及整个数字广告行业——该行业长期担忧谷歌对广告工具的掌控。 该广告技术业务去年带来约 300 亿美元收入，约占 Alphabet 总收入的 8%，但分析师估计其贡献的利润不到 1%。该部门收入已连续 16 个季度下滑，法院仍可能施加行为性补救措施，而非结构性拆分。

hackernews · donohoe · Sep 2, 14:46 · [社区讨论](https://news.ycombinator.com/item?id=49537131)

**背景**: 该案源于美国司法部对谷歌的诉讼，指控谷歌垄断了出版商和广告主买卖在线展示广告所使用的工具。联邦法官已裁定谷歌存在非法垄断，补救阶段旨在决定采取何种处罚或结构性变更以恢复竞争。广告技术（ad tech）指的是实现数字广告自动化买卖的软件和平台，通过广告交易平台和广告服务器将广告主与网站发布商连接起来。分析师指出，谷歌的广告技术业务在其整体利润中占比很小，因此与搜索和云业务相比，对该公司的未来影响相对有限。

**社区讨论**: 评论者大多持怀疑态度，质疑在垄断认定之后，仅仅承诺停止滥用行为是否算得上充分的补救措施。有人提出了替代方案，例如让拆分公司像合并公司一样容易，或对垄断企业累进征税以促使它们自行拆分。还有人深入分析财务数据，或提到谷歌因 YouTube 和解而捐赠 2200 万美元等细枝末节。

**标签**: `#google`, `#antitrust`, `#adtech`, `#monopoly`, `#regulation`

---

<a id="item-4"></a>
## [报告：三个内容农场生成 21.5 万个“最佳软件”页面，被 Perplexity 引用](https://trellner.com/reports/manufactured-sources-behind-ai-recommendations/) ⭐️ 8.0/10

Trellner 的一份报告发现，三个网站批量生成了 215,128 个“最佳软件”页面，这些页面很可能使用了 AI 生成内容，并且如今被 Perplexity 在其回答中频繁引用。这揭示了 AI 制造的内容正日益污染 AI 驱动的搜索推荐。 这一点很重要，因为像 Perplexity 这样的 AI 搜索引擎本应筛选可靠来源，但它们显然信任了低质量的内容农场，从而降低了 AI 生成答案的可信度。这凸显了一个日益严重的反馈循环：AI 生成内容与 AI 搜索引擎相互强化彼此的缺陷，影响到依赖这些工具做决策的用户。 该报告专门针对“最佳软件”类的搜索查询，展示了算法优化和人为制造的页面如何被 Perplexity 的引用机制当作权威来源。这些发现与社区用户反映的情况一致：AI 答案中引用的许多对比页面，要么由被比较的公司自己托管，要么是 AI 生成的“答案引擎优化”玩法。

hackernews · jakobgreenfeld · Sep 2, 13:59 · [社区讨论](https://news.ycombinator.com/item?id=49536375)

**背景**: Perplexity AI 是一个搜索引擎，它使用大型语言模型和实时网络搜索来综合答案，并引用其信息来源。与此同时，内容农场是批量生产低质量、SEO 优化文章的组织；大约从 2022 年起，许多内容农场开始使用生成式 AI 工具来以极低成本制造这类内容。当这两种趋势相遇时，AI 搜索引擎最终可能会引用大量机器生成的页面，把它们当作可靠、权威的来源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Perplexity_AI">Perplexity AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Content_farm">Content farm</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对 AI 搜索的可靠性表示担忧。有用户指出，LLM 倾向于偏好自己生成的段落而非人类撰写的内容；还有人举例说，LLM 曾自信地推荐一个根本不存在的场所。一位 Perplexity 用户表示，其结果变得很快但却是“垃圾”；其他人则指出，模型缺乏对来源的怀疑，常常引用由利益相关的公司托管的 AI 生成对比页面。

**标签**: `#AI-generated content`, `#search quality`, `#Perplexity`, `#content farms`, `#LLM bias`

---

<a id="item-5"></a>
## [Paint.NET 借助 Claude 重写 Direct2D，初步支持 WINE 运行](https://simonwillison.net/2026/Sep/2/rick-brewster/) ⭐️ 8.0/10

Paint.NET 作者 Rick Brewster 宣布，Paint.NET 现在可以通过一个内部、从零开始、采用洁净室方式逆向重写的 Direct2D 实现运行在 WINE 上，启动时加 /wine 参数即可启用。这个约 18 万行的模块 PaintDotNet.Windows.Direct2D1.Managed.dll 主要由 Anthropic 的 Claude 编写。 这是 AI 辅助软件工程的一个重要里程碑：一个大型语言模型帮助生成了 18 万行复杂代码，攻克了长期阻碍 Paint.NET 在 WINE 上运行的兼容性问题。它也为 Paint.NET 用户通过 WINE 在 Linux 上运行程序提供了路径，同时引发了人们对几乎未经审查的“vibe coding（氛围编程）”代码风险的讨论。 Brewster 表示，这段代码属于“vibe coding”，即没有经过彻底审查，属于“信我没错”（trust me bro）的风格，因为 18 万行代码实在无法逐行人工检查。他不得不“盯”着 Claude 处理 COM 资源管理（例如一开始漏掉了对引用计数对象调用 AddRef），并纠正一些糟糕的设计决策，但 Claude 在逆向推导 Direct2D 内置特效库公式方面表现出色。

rss · Simon Willison · Sep 2, 05:50

**背景**: Direct2D 是微软为 Windows 提供的硬件加速、即时模式二维图形 API，Paint.NET 依赖它进行渲染。WINE 是一个开源兼容层，能让 Windows 应用程序在 Linux 等类 Unix 操作系统上运行，但它的 Direct2D 实现一直不完整，无法满足 Paint.NET 的需求。洁净室逆向工程是一种通过观察外部行为重建设计、而不复制原始实现的方法，以避免侵犯版权。Claude 是一种 AI 编程助手，可以根据自然语言提示生成大量代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Direct2D">Direct2D - Wikipedia</a></li>
<li><a href="https://www.winehq.org/">WineHQ - Run Windows applications on Linux, BSD, Solaris and macOS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Clean-room_design">Clean - room design - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Paint.NET`, `#WINE`, `#Direct2D`, `#AI coding`, `#Claude`

---

<a id="item-6"></a>
## [阿里发布 Qwen3.8-Max-0902，CodeArena 编程榜 1691 分夺冠](https://mp.weixin.qq.com/s/BfKRXMAR5ykD58LDkBftLg) ⭐️ 8.0/10

阿里巴巴发布了 Qwen3.8-Max-0902，这是通义千问大模型的新版本。该模型在 CodeArena 前端编程总榜上以 1691 分夺冠，比旧版本提升 22 分。 登顶 CodeArena 表明阿里旗舰模型具备很强的编程能力，也让 AI 编程助手赛道的竞争更加激烈。其 API 定价为每百万输入 tokens 2 美元、每百万输出 tokens 6 美元，远低于榜单第二名（20 美元）和第三名（12 美元）的模型，可能对竞争对手形成价格压力。 据了解，该模型拥有 2.4 万亿参数和 100 万（1M）token 的上下文长度。目前新版本已在千问 AI 平台上线，并接入千问办公、Qoder 与千问 APP。

telegram · zaihuapd · Sep 2, 06:05

**背景**: CodeArena 是一个用于评估自主编程智能体的交互式基准测试，这类智能体能够规划、编写、调试和执行代码来解决编程问题；它还致力于解决现有基准测试中的数据污染等问题。Qwen 是阿里巴巴推出的大语言模型系列，由通义（Tongyi）大模型团队开发，广泛应用于自然语言理解、文本生成和多模态数据处理等场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.alphaxiv.org/benchmarks/monash-university/codearena">CodeArena | alphaXiv</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://medium.com/@huguosuo/codearena-a-dynamic-benchmark-for-evaluating-autonomous-coding-agents-501eec40758b">CodeArena : A Dynamic Benchmark for Evaluating... | Medium</a></li>

</ul>
</details>

**标签**: `#AI`, `#Qwen`, `#CodeArena`, `#LLM`, `#Alibaba`

---

<a id="item-7"></a>
## [xAI 发布 Grok 4.6，强化长时间运行智能体任务](https://t.me/zaihuapd/43559) ⭐️ 8.0/10

xAI 于 2026 年 8 月 12 日发布 Grok 4.6，在 Grok 4.5 的基础上强化了长时间运行的智能体、交互和视觉任务。该模型在综合九项基准的 Artificial Analysis 智能指数上与 GPT-5.6 Sol 持平，并已在 Cursor、Grok Build 及 API 上线。 本次发布表明 xAI 正加大对智能体 AI 的投入，即模型需要长时间执行多步骤任务，而非只回答单次提示。在 Cursor 等工具中上线并采用有竞争力的定价，可能让先进的智能体模型更容易被开发者与企业使用，从而加剧 AI 模型市场的竞争。 定价为每百万输入 token 2 美元、每百万输出 token 6 美元，同时提供双倍价格的快速版本。该模型已在 Cursor、Grok Build 和 API 上线，原文还提到 Grok 中首周有相关活动，但具体细节在来源中被截断。

telegram · zaihuapd · Sep 2, 08:10

**背景**: Artificial Analysis 智能指数是一个综合基准评分，用于衡量语言模型在推理、编码、知识、指令遵循、科学推理和多步任务完成等方面的能力。长时间运行的智能体任务是指自主的多步骤智能体工作流，运行时间从几分钟到数小时甚至数天，需要超越单次函数调用的基础设施。Grok Build 是 xAI 的可扩展编码智能体，支持 CLI、交互式或 headless 会话。理解这些概念有助于理解 Grok 4.6 在基准测试中持平以及聚焦智能体的意义。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index v4.1.1 | Artificial Analysis</a></li>
<li><a href="https://docs.x.ai/build/overview">Grok Build : SpaceXAI's Coding Agent | SpaceXAI Docs</a></li>
<li><a href="https://www.openlegion.ai/en/learn/ai-agent-long-running-tasks">AI Agent Long Running Tasks : Queues, Checkpoints... | OpenLegion</a></li>

</ul>
</details>

**标签**: `#AI`, `#Grok`, `#xAI`, `#Language Models`, `#Benchmarks`

---