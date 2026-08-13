---
layout: default
title: "Horizon Summary: 2026-08-13 (ZH)"
date: 2026-08-13
lang: zh
---

> From 32 items, 10 important content pieces were selected

---

1. [DeepSeek V4 Pro 0813 发布：高性价比的 MoE 大模型](#item-1) ⭐️ 9.0/10
2. [Tailscale 将数据库损坏追溯到 16 年前的 SQLite WAL-Reset Bug](#item-2) ⭐️ 9.0/10
3. [Qwen 3.8-Max：2.4 万亿参数开源模型发布](#item-3) ⭐️ 9.0/10
4. [Zed 推出 Delta，支持实时多人协作 AI 智能体对话](#item-4) ⭐️ 8.0/10
5. [xAI 发布 Grok 4.6：1753 ELO 的平价前沿模型](#item-5) ⭐️ 8.0/10
6. [uBlock Origin 放弃屏蔽 Facebook 广告，指责其反用户手段](#item-6) ⭐️ 8.0/10
7. [为什么小尺寸 JPEG 在 Chrome 和 Firefox 中显示不同](#item-7) ⭐️ 8.0/10
8. [Grok 4.6 在 Artificial Analysis 智能指数中得 61 分](#item-8) ⭐️ 8.0/10
9. [AI 是否正在淘汰软件工程的中层？](#item-9) ⭐️ 8.0/10
10. [微信发布资源高效的 WeLM 大语言模型家族](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [DeepSeek V4 Pro 0813 发布：高性价比的 MoE 大模型](https://openrouter.ai/deepseek/deepseek-v4-pro-0813) ⭐️ 9.0/10

DeepSeek 发布了 DeepSeek-V4 Pro（版本 0813），这是一个预览版混合专家（MoE）模型，总参数量达 1.6 万亿，激活参数为 490 亿。它支持 100 万 token 的上下文长度，并已在 OpenRouter 上线，输入价格为每百万 token 0.435 美元，输出价格为每百万 token 0.87 美元。 这一发布意义重大，因为 DeepSeek 继续以远低于专有系统的成本提供性能可与之匹敌的开源权重模型。此次发布可能会加快开发者对 DeepSeek 模型的采用，并加剧 AI API 提供商之间的价格竞争。 该模型是 DeepSeek-V4 系列的预览版本，采用混合专家（MoE）架构，每次推理仅激活 1.6 万亿参数中的 490 亿。它支持 100 万 token 的上下文长度，适合长文档处理和复杂推理任务。

hackernews · explosion-s · Aug 12, 16:04 · [社区讨论](https://news.ycombinator.com/item?id=49274600)

**背景**: DeepSeek 是一家成立于 2023 年的中国 AI 公司，由对冲基金 High-Flyer 资助，以其开源权重的大语言模型（如 V3 和 R1）而闻名。其混合专家（MoE）方法大幅降低了训练和推理成本，2025 年 1 月 R1 发布时曾引发全球对 AI 经济学的重新评估。尽管该公司因开源和高效而受到称赞，但其模型也因数据收集和审查合规问题而受到关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/DeepSeek-V4-Pro · Hugging Face</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-pro">DeepSeek V4 Pro - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>

</ul>
</details>

**社区讨论**: Hacker News 用户总体持正面态度，有用户实测后称赞该模型的性能和低成本。有用户批评链接指向 OpenRouter 而非官方文档或基准测试，也有人将其与 Claude 和 Kimi 等模型在每任务成本上做对比，认为 DeepSeek 适合只想快速完成任务的场景。

**标签**: `#AI`, `#DeepSeek`, `#LLM`, `#model release`, `#Hacker News`

---

<a id="item-2"></a>
## [Tailscale 将数据库损坏追溯到 16 年前的 SQLite WAL-Reset Bug](https://tailscale.com/blog/sqlite-wal-reset-bug) ⭐️ 9.0/10

Tailscale 发布技术文章，详述如何追踪到一个隐蔽的数据库损坏问题，最终定位为 SQLite WAL-Reset 逻辑中一个存在 16 年的数据竞争。SQLite 已在 3.51.3 版本中修复此 Bug，Tailscale 还资助了一个开源 VFS shim 来协助隔离问题。 该发现意义重大，因为 SQLite 是全球使用最广泛的嵌入式数据库之一，而此 Bug 潜伏多年且极难复现。Tailscale 与 SQLite 团队的协作以及资助调试工具的做法，为企业反哺开源基础设施树立了范例。 这个 Bug 是 WAL 子系统中一个时序窗口极窄的数据竞争，自 2010 年起就存在。Tailscale 给其 SQLite 驱动打了补丁，在写事务与 WAL 重置重叠时输出告警日志，SQLite 官方则在 3.51.3 版本中完成修复。

hackernews · ropbear · Aug 12, 14:22 · [社区讨论](https://news.ycombinator.com/item?id=49272832)

**背景**: SQLite 是一种广泛嵌入使用的轻量级关系型数据库，采用预写式日志（WAL）机制来提升并发读写性能。VFS（虚拟文件系统）层是 SQLite 与操作系统之间的抽象接口，而 VFS shim 是插入其中的插件，可用于调试、校验或插桩。此次 Bug 的根源是写事务与 WAL 重置之间的数据竞争，在特定时序下可能导致数据库文件损坏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tailscale.com/blog/sqlite-wal-reset-bug">How Tailscale helped find the SQLite WAL-Reset bug</a></li>
<li><a href="https://antithesis.com/blog/2026/wal-reset-bug/">Breaking the WAL | Antithesis</a></li>
<li><a href="https://sqlite.org/vfs.html">The SQLite OS Interface or "VFS"</a></li>

</ul>
</details>

**社区讨论**: 评论区普遍称赞 Tailscale 写下了详尽的技术复盘，并为开源调试工具提供资金支持，也欣赏 SQLite 团队对 Bug 的官方解释。有读者希望了解为何要如此频繁地执行 checkpoint，还有人指出即便有海量测试，某些 Bug 仍可能长期潜伏。

**标签**: `#SQLite`, `#Tailscale`, `#Database Corruption`, `#Bug Analysis`, `#Open Source`

---

<a id="item-3"></a>
## [Qwen 3.8-Max：2.4 万亿参数开源模型发布](https://t.me/zaihuapd/43151) ⭐️ 9.0/10

Qwen 发布了 Qwen 3.8-Max，这是一个拥有 2.4 万亿参数的混合专家模型，其中活跃参数为 950 亿，这标志着 Max 级别模型权重首次开源。下周该模型将在 Hugging Face 上线。 这是 Qwen 首次开源 Max 级模型，让 AI 社区获得了可与 Opus、Fable 等专有系统媲美的能力。这向着前沿大型语言模型的普及迈出了重要一步，但服务于如此庞大的模型仍具挑战。 开源权重版本基于 Qwen 3.5 架构，支持编码、智能体工作和长期任务等，但不具备官方 Max 版本的视觉输入和默认 100 万上下文长度。模型以 BF16 和 FP8 格式发布，完整的 BF16 无损版本大约需要 4.9TB 内存，而 1 比特量化版本仅需 397GB。

telegram · zaihuapd · Aug 12, 16:13

**背景**: 混合专家（MoE）是一种只对每个令牌激活部分参数的架构，使模型能够扩展到万亿参数而无需成比例增加计算成本。FP8 量化通过以更低精度存储权重来减小模型大小和内存占用，使大型模型更易部署。Qwen 是阿里巴巴的开源大语言模型系列；以往的 Max 级模型均为闭源，因此此次发布对社区来说是显著的转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://rcrtech.com/semiconductor-news/llms-quantization-fp8-fp4-int8/">LLMs and quantization: FP8, FP4, and INT8 explained</a></li>

</ul>
</details>

**社区讨论**: 评论者对于 1 比特量化版本（397GB）能在消费级硬件上带来接近 Opus 4.5 的性能感到惊叹，但也指出完整 BF16 模型体积庞大（约 4.9TB），服务成本可能很高，有用户表示其 API 价格是 Grok 4.6 的两倍。其他人指出，开源权重模型缺少视觉支持和 100 万上下文，并且许可协议限制超过 5000 万美元收入的公司对外提供服务，这与 Kimi k3 的条款类似。

**标签**: `#AI`, `#LLM`, `#Qwen`, `#Open Source`, `#Model Release`

---

<a id="item-4"></a>
## [Zed 推出 Delta，支持实时多人协作 AI 智能体对话](https://zed.dev/blog/introducing-delta) ⭐️ 8.0/10

Zed 宣布推出 Delta 功能，支持实时协同的多人 AI 智能体对话，并可在对话中内联评论。该功能将智能体对话视为一种文档，用户可以直接在对话线程内进行评论。 Delta 可能改变团队与 AI 智能体协作的方式，让结对调试、辅导新人以及设计讨论都能在编辑器内完成。它延续了 Zed 的押注：实时协作与 AI 辅助工作流将在多人编程环境中融合。 该发布与 DeltaDB 紧密相关，后者是一套操作级版本控制系统，其愿景是将 IDE 变成人机协作的工作空间，让人类与 AI 智能体跨时间尺度共同工作。对话内联评论让用户可以标注产生代码的推理过程，不过该功能似乎主要面向 AI 智能体高频参与的工作流。

hackernews · khy · Aug 12, 18:19 · [社区讨论](https://news.ycombinator.com/item?id=49276574)

**背景**: Zed 是一款以速度著称的高性能多人代码编辑器，并内置 AI 智能体。Zed 团队一直在推动一种工作流：开发者和 AI 智能体之间的对话被视为软件的真正来源，而 DeltaDB 为这种对话提供操作级版本控制。Delta 看起来是在这一理念之上构建的多人协作界面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zed.dev/blog/introducing-deltadb">Software Is Made Between Commits — Zed's Blog</a></li>
<li><a href="https://shapeof.com/archives/2025/8/deltadb_from_zed.html">DeltaDB From Zed (the Code Editor) - shapeof.com</a></li>
<li><a href="https://github.com/zed-industries/zed">GitHub - zed -industries/ zed : Code at the speed of thought – Zed is...</a></li>

</ul>
</details>

**社区讨论**: HN 评论者反应不一：有人认为多人编程没有必要，因为编程本质上是单人活动；也有人不喜欢阅读冗长且可能漏掉边界情况的 AI 总结。更积极的看法认为它有助于辅导新人和审计 PR 的产生过程；同时还有不少人抱怨公告页面低对比度的设计。

**标签**: `#Zed`, `#collaborative coding`, `#AI agents`, `#editor`, `#real-time collaboration`

---

<a id="item-5"></a>
## [xAI 发布 Grok 4.6：1753 ELO 的平价前沿模型](https://x.ai/news/grok-4-6) ⭐️ 8.0/10

xAI 于 2026 年 8 月 7 日发布了 Grok 4.6，这是一个 1.5 万亿参数的前沿模型，基于与 Grok 4.5 相同的 V9 基础架构，但显著改进了监督微调和强化学习。该模型的 API 价格约为竞争对手前沿模型的一半，据报道 ELO 评分达到 1753。 Grok 4.6 通过提供比 GPT-5.6-Sol 和 Claude 4.8/5 更便宜且性能更高的替代方案，加剧了前沿 AI 市场的竞争。这可能迫使竞争对手调整定价，并让基于 Grok 的智能体对开发者和企业更具吸引力。 该版本复用了 1.5T V9 基础架构，而不是从头进行预训练，性能提升主要来自改进的 SFT 和 RL。一些 API 用户报告称，xAI 现在会在所有 Grok 4.6 请求中注入默认系统提示，这可能会覆盖用户关于讨论系统提示的指令。

hackernews · iLuddite · Aug 12, 15:32 · [社区讨论](https://news.ycombinator.com/item?id=49274027)

**背景**: Grok 是埃隆·马斯克旗下 xAI 开发的大语言模型和聊天机器人，于 2023 年 11 月上线。它与 X 社交网络集成，并提供 iOS、Android 及特斯拉 Optimus 机器人版本。xAI 在 2026 年 2 月被 SpaceX 收购后以 SpaceXAI 名义运营，已发布多个 Grok 模型家族，包括开源 Grok-1，并建造了 Colossus 超级计算机来支持训练和推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://kie.ai/blog/what-is-grok-4-6">What Is Grok 4.6? xAI's 1.5T-Param Model Explained</a></li>
<li><a href="https://www.basenor.com/blogs/news/xai-launches-grok-4-6-1753-elo-half-the-price-of-rival-frontier-models">xAI Launches Grok 4.6: 1753 ELO, Half the Price of Rival Frontier Models</a></li>
<li><a href="https://en.wikipedia.org/wiki/XAI_(company)">XAI (company)</a></li>

</ul>
</details>

**社区讨论**: 评论区对 Grok 4.6 的基准成绩和定价总体持积极态度，有人称其具有'Fable 级智能'，在多数基准上超过 GPT-5.6-Sol。但也有人担心默认系统提示会干扰用户指令，还有人质疑多个实验室在两个月内发布'Fable 级'模型，可能意味着基准测试作弊而非真实进步。

**标签**: `#Grok`, `#xAI`, `#AI`, `#LLM`, `#model release`

---

<a id="item-6"></a>
## [uBlock Origin 放弃屏蔽 Facebook 广告，指责其反用户手段](https://digitalescapetools.com/2026/08/ublock-origin-stops-chasing-facebook-ads.html) ⭐️ 8.0/10

uBlock Origin 正式停止与 Facebook 广告的对抗。开发团队成员在 uBlock Origin 子版块宣布，项目不再追逐 Facebook 不断更新的反广告屏蔽技术，并称 Facebook 是“令人厌恶的反用户网站”。 这是广告屏蔽军备竞赛中的一个标志性时刻，表明即使是广受欢迎的开源广告屏蔽器也无法与 Facebook 的工程资源抗衡。依赖 uBlock Origin 的用户今后将在 Facebook 上看到更多广告，其他广告屏蔽项目未来也可能面临类似抉择。 该项目将保留现有的 Facebook 过滤列表，但不再在 Facebook 找到新的规避方法时更新它们。Facebook 使用混淆广告元素、将广告混入普通帖子等技术，使基于过滤器的屏蔽几乎无法持续维护。

hackernews · Markoff · Aug 12, 11:28 · [社区讨论](https://news.ycombinator.com/item?id=49270726)

**背景**: uBlock Origin 是一款广泛使用的开源浏览器扩展，通过社区维护的过滤列表来屏蔽广告和追踪器。Facebook 依赖广告收入，并在反广告屏蔽技术上投入了大量资源，包括更改广告在 HTML 中的标识特征，以及让广告与普通帖子使用同样的服务器加载。由于基于过滤器的屏蔽器必须不断适应这些变化，维护 Facebook 过滤列表对 uBlock Origin 的小团队来说成了一场永无止境、耗费大量精力的战斗。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.neowin.net/news/facebook-ads-are-so-hard-to-block-that-ublock-origin-stopped-filtering-them/">Facebook ads are so hard to block that uBlock Origin stopped filtering them - Neowin</a></li>
<li><a href="https://piunikaweb.com/2026/08/10/ublock-origin-facebook-ads-not-blocking/">Seeing ads on Facebook even with uBlock Origin? Here's why - PiunikaWeb</a></li>
<li><a href="https://www.techspot.com/news/65906-facebook-has-figured-out-how-circumvent-ad-blockers.html">Facebook has figured out how to circumvent ad blockers | TechSpot</a></li>

</ul>
</details>

**社区讨论**: 评论者大多支持这一决定，认为这是对有限开发时间的合理利用。有人预测军备竞赛的下一步将是基于计算机视觉的广告检测，直接在屏幕上广告元素上画矩形；也有人质疑，把广告强推给屏蔽广告的用户，对 Facebook 来说是否真的能赚钱。

**标签**: `#adblocking`, `#privacy`, `#facebook`, `#ublock-origin`, `#arms-race`

---

<a id="item-7"></a>
## [为什么小尺寸 JPEG 在 Chrome 和 Firefox 中显示不同](https://guillaumetech.github.io/posts/jpg-scaling-chrome/) ⭐️ 8.0/10

一篇技术文章解释了 Chrome 和 Firefox 在缩小小型 JPEG 图片时会产生肉眼可见的差异，并指出了两个浏览器图像缩放管线中的根本原因。Chrome 的输出往往更模糊，而 Firefox 的输出更锐利，但容易出现振铃伪影。 这对准备图标和小尺寸图片的 Web 开发者很重要，因为同一文件在不同浏览器中看起来会有明显差异。选择合适的图片分辨率和格式对于保持一致的渲染质量至关重要。 差异部分来自 Chrome 和 Firefox 使用不同的缩小滤波器——Chrome 偏好更平滑（更模糊）的输出，而 Firefox 使用更锐利的内核，可能产生振铃效应。当图片缩小到非常小的尺寸时，JPEG 色度子采样还会进一步放大色彩伪影。

hackernews · gutechh · Aug 12, 14:00 · [社区讨论](https://news.ycombinator.com/item?id=49272549)

**背景**: 浏览器渲染管线会在将图片绘制到屏幕前进行缩放。JPEG 压缩采用色度子采样，以低于亮度的分辨率存储颜色信息；当高分辨率图片被缩小到很小的尺寸时，这些子采样的颜色细节会与浏览器的缩放算法相互作用。不同的缩放算法（如 box、bilinear、bicubic 或 Lanczos）在清晰度和伪影之间各有取舍，这就是为什么相同的 JPEG 在 Chrome 和 Firefox 中显示效果不同的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Image_scaling">Image scaling - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Chroma_subsampling">Chroma subsampling - Wikipedia</a></li>
<li><a href="https://developer.chrome.com/docs/chromium/renderingng-architecture">RenderingNG architecture | Chromium | Chrome for Developers</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论指出，PNG 图标也会受到影响，Chrome 更模糊的缩放曾在 Electron 应用中破坏图标。评论者建议使用与显示尺寸相匹配的图片分辨率，还有人链接到 Firefox 的一个 bug，涉及实现低倍率解压来解决该问题。

**标签**: `#JPEG`, `#browser rendering`, `#image scaling`, `#Chrome`, `#Firefox`

---

<a id="item-8"></a>
## [Grok 4.6 在 Artificial Analysis 智能指数中得 61 分](https://artificialanalysis.ai/articles/grok-4-6-benchmarks-and-analysis) ⭐️ 8.0/10

SpaceXAI 发布了面向编程、智能体任务和知识工作的前沿模型 Grok 4.6，该模型在 Artificial Analysis 智能指数中获得了 61 分。该分数反映了模型在最新综合基准评估中的表现。 在 Artificial Analysis 智能指数中获得 61 分，使 Grok 4.6 跻身于争夺编程和智能体工作负载领先地位的前沿大语言模型之列。社区的高度关注和基准讨论之所以重要，是因为开发者越来越根据实际可用性、定价和模型多样性来选择模型，而不仅仅是看原始分数。 Artificial Analysis 智能指数是一个综合基准，汇总了数学、科学、编码和推理等九项具有挑战性的评估。搜索结果还指出，Grok 4.6 的缓存读取定价从 Grok 4.5 的 0.30 美元几乎翻倍至 0.50 美元，这可能会明显影响高频编码会话的成本。

hackernews · wertyk · Aug 12, 16:54 · [社区讨论](https://news.ycombinator.com/item?id=49275385)

**背景**: Artificial Analysis 智能指数旨在通过将多个高难度基准合并为一个模型级分数，提供对 AI 能力的整体衡量；v4.1 版本将更大权重转向智能体工作负载。Grok 4.6 是 SpaceXAI 的前沿模型，相比 Grok 4.5 进行了更长的补充训练，使用了经过筛选的模型生成数据、高质量的工程数据，以及改进的优化器和训练方案。这一背景有助于理解为何该基准结果会与其他前沿模型进行比较，并与实际使用体验一起被讨论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index</a></li>
<li><a href="https://x.ai/news/grok-4-6">Introducing Grok 4.6 | SpaceXAI</a></li>
<li><a href="https://artificialanalysis.ai/models/grok-4-6">Grok 4.6 (high) Intelligence, Performance & Price Analysis</a></li>

</ul>
</details>

**社区讨论**: 评论区总体持正面态度，有人说 Grok“沟通更好”且比 Claude Code 更快，也有人称赞 Cursor 捆绑 Grok 4.5/4.6 的定价很有性价比。一些用户重视 Grok 作为独立“模型家族”的价值，指出其与 Anthropic 和 Gemini 存在实用的行为差异。也有用户担忧缓存读取价格几乎翻倍，从每批 0.30 美元涨至 0.50 美元，可能对重度编程使用产生成本影响。

**标签**: `#AI`, `#LLM`, `#Benchmark`, `#Grok`, `#Artificial Analysis`

---

<a id="item-9"></a>
## [AI 是否正在淘汰软件工程的中层？](https://blog.florianherrengt.com/ai-removing-middle-class-software-engineering.html) ⭐️ 8.0/10

一篇博客文章认为，AI 助手正通过让资深工程师跳过将编码任务交给中级工程师的传统交接，从而“淘汰软件工程的中层”。文章警告说，这种动态会同时放大好的和差的工程实践，可能使中级工程师变得可有可无。 这一点很重要，因为它触及了一个及时且广泛争论的问题：AI 对科技行业就业的影响，尤其是对中级工程师的需求。该讨论对职业规划、招聘策略以及 AI 时代工程团队的组织方式都有影响。 文章用“StackOverflow 工程师的自动化”来描述高级开发者现在可以直接编写以往需要外包的代码。它还声称，“糟糕的”工程师可以借助 AI 将他们的负面影响在组织内放大十倍。

hackernews · florianherrengt · Aug 12, 13:20 · [社区讨论](https://news.ycombinator.com/item?id=49271994)

**背景**: 在软件团队中，常见的工作流程是高级工程师编写规格说明或 Jira 工单，中级工程师负责实现。基于 LLM 的 AI 编码工具现在让高级工程师可以自己生成这些代码，从而减少了对交接的需求。这一讨论触及了 AI 推动科技行业岗位替代的广泛担忧，以及所谓的“K 型经济”——部分劳动者受益，而另一些则被甩在后面。

**社区讨论**: 评论者大多积极参与且观点不一：一些人认为工程师绝不应将批判性思维外包给 LLM，另一些人则指出几十年来技术一直在重构劳动力市场，将“K 型经济”视为更广泛的趋势。一位评论者强调“糟糕的”工程师现在可以放大其负面影响，另一位则将其视为“StackOverflow 工程师”的自然自动化。

**标签**: `#AI`, `#software engineering`, `#career impact`, `#LLM`, `#productivity`

---

<a id="item-10"></a>
## [微信发布资源高效的 WeLM 大语言模型家族](https://x.com/Weixin_WeChat/status/2087509298310209718) ⭐️ 8.0/10

微信团队发布了 WeLM 通用大语言模型系列，以极致的资源效率为核心。其中 WeLM-80B（3B 激活参数）已应用于微信 AI 智能体小微，而采用 MoE 架构的 WeLM-617B（23B 激活参数）正在研发中。 此次发布意义重大，因为资源高效的大语言模型能够在微信海量用户场景中规模化落地，大幅降低算力与能耗成本。这也体现了行业从单纯追求参数量向注重实际部署效率的转变。 WeLM-80B 采用稀疏激活机制（每次推理仅激活 80B 参数中的 3B），已支持对话、搜索、微信原生功能及小程序服务。研发中的 WeLM-617B 基于混合专家（MoE）架构，仅激活 23B 参数，面向小程序智能开发与“微信小微”小工具生成等复杂任务。

telegram · zaihuapd · Aug 12, 13:58

**背景**: WeLM 是微信 AI 团队自研的 NLP 大规模语言模型系列，支持零样本与少样本场景下的对话、阅读理解、翻译、改写等多种任务。MoE（混合专家）架构通过门控网络为每个输入动态选择专门的子模型，使模型容量增大而计算成本不成比例增长。稀疏激活机制则仅对每轮输入的部分参数进行计算，降低显存占用与能耗。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.tencent.com/developer/article/2235231">WeLM 微 信 自研NLP 大 规 模 语 言 模 型 -腾讯云开发者社区-腾讯云</a></li>
<li><a href="https://www.d1ev.com/newsflash/310245">微 信 AI助手“小 微 ”升级！ WeLM 大 模 型 赋能800...</a></li>
<li><a href="https://zilliz.com.cn/blog/what-is-mixture-of-experts">深度解读混合专家模型（MoE）：算法、演变与原理 - Zilliz 向量数据库</a></li>

</ul>
</details>

**标签**: `#大语言模型`, `#微信`, `#AI`, `#资源效率`, `#MoE`

---