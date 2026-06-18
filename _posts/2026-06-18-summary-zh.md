---
layout: default
title: "Horizon Summary: 2026-06-18 (ZH)"
date: 2026-06-18
lang: zh
---

> From 36 items, 11 important content pieces were selected

---

1. [RFC 10008 定义新的 HTTP QUERY 方法](#item-1) ⭐️ 9.0/10
2. [GLM-5.2：MIT 许可下的领先开放权重 LLM](#item-2) ⭐️ 9.0/10
3. [Lore：面向游戏开发的可扩展开源版本控制系统](#item-3) ⭐️ 8.0/10
4. [美国推迟将 DeepSeek 列入黑名单，新增百余家中国公司为风险企业](#item-4) ⭐️ 8.0/10
5. [美国科学与政治信任崩塌，研究人员外流](#item-5) ⭐️ 8.0/10
6. [乐购因博通定价将 4 万个服务器工作负载迁离 VMware](#item-6) ⭐️ 8.0/10
7. [GLM-5.2 在 Artificial Analysis 开放权重模型中居首](#item-7) ⭐️ 8.0/10
8. [Charity Majors: AI 让代码生成变得免费且可抛弃](#item-8) ⭐️ 8.0/10
9. [中国将科创板第五套标准扩展至人工智能与硬科技](#item-9) ⭐️ 8.0/10
10. [Anthropic 企业 AI 市场份额首次超越 OpenAI](#item-10) ⭐️ 8.0/10
11. [微软借助 OpenAI 模型在中国拓展 AI 业务](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [RFC 10008 定义新的 HTTP QUERY 方法](https://www.rfc-editor.org/info/rfc10008/) ⭐️ 9.0/10

RFC 10008 定义了一种新的 HTTP QUERY 方法，允许发送安全且幂等的请求并携带请求体，将此前通过 GET 发送请求体（非标准做法）的模式正式规范化。 这一标准化为 API 中的复杂查询提供了清晰的解决方案，改善了缓存语义，减少了在非修改操作中对 POST 的依赖，可能简化 Web 架构并优化开发者工作流。 QUERY 方法是安全且幂等的，但缓存其响应时需要将请求体纳入缓存键，这可能导致缓存键无界，给中间件带来实际挑战。

hackernews · schappim · Jun 17, 10:51 · [社区讨论](https://news.ycombinator.com/item?id=48568502)

**背景**: HTTP GET 请求设计用于安全、幂等地获取数据，且不携带请求体。然而，对于复杂查询（如大型 JSON 过滤器），开发者经常通过 GET 发送请求体，这违反了 HTTP 规范并导致互操作性问题。新的 QUERY 方法通过提供标准、安全的方式来发送带体的查询，从而解决了这一问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://httpwg.org/http-extensions/draft-ietf-httpbis-safe-method-w-body.html">The HTTP QUERY Method</a></li>
<li><a href="https://horovits.medium.com/http-s-new-method-for-data-apis-http-query-1ff71e6f73f3">HTTP ‘s New Method For Data APIs: HTTP QUERY | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区评论中，有人关注 QUERY 方法在 HTML 表单中的支持，也有人对包含大请求体的缓存表示担忧。部分开发者表示已在实践中使用 GET 带体，另一些人则质疑将请求体纳入缓存键的可行性。

**标签**: `#HTTP`, `#RFC`, `#web protocol`, `#API design`, `#caching`

---

<a id="item-2"></a>
## [GLM-5.2：MIT 许可下的领先开放权重 LLM](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai 于 2026 年 6 月 16 日以 MIT 许可发布了 GLM-5.2，这是一个 7530 亿参数的混合专家模型，拥有 100 万 token 的上下文窗口，在开放权重模型中取得了 Artificial Analysis 智能指数的最高分。 此次发布提供了一个与专有模型相媲美的最先进开放权重 LLM，凭借宽松的许可促进了 AI 社区的创新和可访问性，支持广泛使用和定制。 GLM-5.2 在总共 7530 亿参数中激活 40 个专家，每个任务消耗的输出 token 多于同类模型，且仅支持文本输入；它在 Code Arena WebDev 排行榜上仅次于 Claude Fable 5 位列第二。

rss · Simon Willison · Jun 17, 23:58

**背景**: 混合专家（MoE）是一种架构，每个 token 仅激活部分参数，从而在高效推理的同时实现大模型。开放权重模型公开发布训练好的参数权重，允许微调和部署，这与 GPT-5.5 等完全封闭的模型不同。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://codingscape.com/blog/llms-with-largest-context-windows">LLMs with largest context windows</a></li>

</ul>
</details>

**社区讨论**: 文章强调了强烈的关注和独立基准测试证实 GLM-5.2 的领先性能，但也有评论指出其 token 消耗高于其他开放权重模型。

**标签**: `#AI`, `#LLM`, `#open-weights`, `#MoE`, `#GLM-5.2`

---

<a id="item-3"></a>
## [Lore：面向游戏开发的可扩展开源版本控制系统](https://lore.org/) ⭐️ 8.0/10

Epic Games 开源了 Lore，这是一个为处理大型二进制资产和扩展到大型团队而设计的下一代版本控制系统，主要面向游戏开发和其他以媒体为中心的项目。 Lore 为游戏开发领域提供了 Perforce（当前主流版本控制系统）的可行开源替代方案，解决了 Git 在处理非文本文件时的不足。它可能降低游戏工作室的成本和供应商锁定，同时改善纹理、3D 模型等资源的协作。 Lore 针对代码与大型二进制资产混合的项目进行了优化，支持文件锁定以实现独占编辑，由 Epic Games 维护并直接集成到 Unreal Engine 5 中。它旨在实现数据和团队前所未有的可扩展性。

hackernews · regnerba · Jun 17, 14:30 · [社区讨论](https://news.ycombinator.com/item?id=48571081)

**背景**: 版本控制系统（如 Git）擅长处理文本文件，但难以应对游戏开发中常见的纹理、音频和 3D 模型等大型二进制文件。Perforce 凭借对大型文件、文件锁定和权限的强大支持，一直是游戏行业的事实标准，但它是专有软件且管理复杂。Lore 旨在作为开源、可扩展的替代方案填补这一空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/EpicGames/lore">Lore is a next-generation, open source revision control system</a></li>
<li><a href="https://lore.org/">Lore | Next-Generation Open Source Version Control - Lore</a></li>
<li><a href="https://dev.epicgames.com/documentation/unreal-engine/lore-version-control-in-unreal-engine?lang=en-US">Lore Version Control in Unreal Engine - Epic Dev</a></li>

</ul>
</details>

**社区讨论**: HN 社区普遍认为 Lore 是游戏开发领域 Perforce 急需的挑战者，并注意到它在 Unreal Engine 工作流程中的潜力。一些评论者指出 Git 的用户界面不友好，而 Perforce 虽然艺术家熟悉但已显老旧。整体情绪积极，人们对一个能解决实际痛点、又无意取代通用代码 Git 的开源方案感到兴奋。

**标签**: `#version control`, `#game development`, `#open source`, `#scalability`, `#perforce alternative`

---

<a id="item-4"></a>
## [美国推迟将 DeepSeek 列入黑名单，新增百余家中国公司为风险企业](https://www.reuters.com/world/china/us-holds-off-blacklisting-chinas-deepseek-more-than-100-firms-deemed-security-2026-06-17/) ⭐️ 8.0/10

据报道，美国决定推迟将中国人工智能公司 DeepSeek 列入贸易黑名单，但已将超过 100 家其他中国企业列入安全风险清单。 这一决定凸显了中美技术脱钩的持续进行，以及监管国家安全风险与保持对竞争性人工智能技术准入之间的微妙平衡。DeepSeek 模型的开发者和用户可能面临未来准入的不确定性。 DeepSeek 因其先进且成本效益高的人工智能模型而受到关注，这些模型使用了出口受限的 NVIDIA GPU 进行训练。该公司目前仍在观察名单中，但未被列入实体清单（Entity List），后者将禁止美国向其出口。

hackernews · giuliomagnifico · Jun 17, 03:55 · [社区讨论](https://news.ycombinator.com/item?id=48565498)

**背景**: DeepSeek 是一家成立于 2023 年的中国人工智能初创公司，以远低于竞争对手（如 OpenAI 的 GPT-4）的成本开发了 DeepSeek-R1 等大型语言模型而闻名。其模型是开放权重的，并在受出口限制的较弱芯片上训练，挑战了美国在人工智能领域的主导地位。美国一直在收紧对华先进人工智能芯片的出口管制，以防止军事用途并保持技术优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>
<li><a href="https://www.deepseek.com/en/">DeepSeek</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了多种观点：一些人称赞 DeepSeek 的实惠和编码能力（例如在 VSCode 中使用），而另一些人则批评美国政策为保护主义且适得其反，并将其与中国防火墙相类比。少数人指出实体清单并未完全禁止贸易，且中国 AI 公司除了已经受限的 NVIDIA GPU 外，对美国商品依赖甚少。

**标签**: `#geopolitics`, `#AI regulation`, `#DeepSeek`, `#US-China trade`, `#technology policy`

---

<a id="item-5"></a>
## [美国科学与政治信任崩塌，研究人员外流](https://www.scientificamerican.com/article/americas-compact-between-science-and-politics-is-broken/) ⭐️ 8.0/10

这场危机威胁到美国在研究创新领域的领先地位，因为优秀科学家和学生正在离开美国或放弃学术界，削弱了国家的科学事业。 文章强调前所未有的政治干预，例如禁止提及多样性、公平和包容（DEI）的拨款，以及资金被随意取消或延迟发放。

hackernews · presspot · Jun 17, 09:54 · [社区讨论](https://news.ycombinator.com/item?id=48568058)

**背景**: 美国科学事业长期基于一种契约：科学家在不受政治干预的情况下追求知识，而政府以跨党派广泛支持提供研究资金。但近年来，科学日益政治化，气候变化和新冠疫情等问题受到党派攻击，如今拨款直接受干预，削弱了传统信任。

**社区讨论**: 评论者分享个人经历：一位研究人员的妻子操作罕见的光阱显微镜，因科研混乱而移居国外；教授们报告资金枯竭、签证限制阻碍外籍研究生；某些领域的氛围从谨慎乐观转为明显紧张，许多资深科学家都在准备备用计划。

**标签**: `#science policy`, `#research funding`, `#academia`, `#US politics`, `#immigration`

---

<a id="item-6"></a>
## [乐购因博通定价将 4 万个服务器工作负载迁离 VMware](https://arstechnica.com/information-technology/2026/06/tesco-moving-40000-server-workloads-off-vmware-amid-broadcoms-abusive-conduct/) ⭐️ 8.0/10

英国最大连锁超市乐购（Tesco）宣布，为应对博通收购 VMware 后激进的定价和削减支持的做法，正在将 4 万个服务器工作负载迁离 VMware。 一家大型企业的如此大规模迁移，标志着 VMware 在虚拟化市场的主导地位正受到严重侵蚀，可能加速 Proxmox 等替代平台的应用，并迫使博通重新审视其策略。 乐购的新虚拟化软件尚未公布名称，且与现有 Veeam 和 Zerto 备份工具不兼容，给迁移中的数据安全带来挑战。该公司是博通收购后涨价导致重新考虑 VMware 的众多客户之一。

hackernews · Bender · Jun 17, 21:00 · [社区讨论](https://news.ycombinator.com/item?id=48576838)

**背景**: 博通于 2023 年 11 月收购 VMware，随后大幅提价，将许可模式从永久许可改为订阅制，并削减对小型客户的支持。这引发了向 Proxmox 等开源替代品的迁移浪潮，这些替代品以更低成本提供类似功能。乐购此举是公开披露的最大规模迁移之一。

**社区讨论**: 评论者普遍批评博通的商业模式具有掠夺性，指出其历史上常通过收购公司、提价和削减服务来获利。一些人强调 Proxmox 作为可行替代方案正获得关注，另一些人则指出备份软件不兼容等迁移挑战。

**标签**: `#VMware`, `#Broadcom`, `#virtualization`, `#enterprise IT`, `#Tesco`

---

<a id="item-7"></a>
## [GLM-5.2 在 Artificial Analysis 开放权重模型中居首](https://artificialanalysis.ai/articles/glm-5-2-is-the-new-leading-open-weights-model-on-the-artificial-analysis-intelligence-index) ⭐️ 8.0/10

由智谱（Z.ai）开发的 GLM-5.2 已成为 Artificial Analysis 智能指数上领先的开放权重模型，其性能接近前沿水平，但定价大幅降低。 这一突破挑战了 Anthropic、OpenAI 和 Google 的专有模型，使全球开发者更容易获得且更负担得起高质量的人工智能。 该模型采用 MIT 许可证发布，专为长时任务设计，但社区报告显示，它可能在复杂编程任务上花费超过 15 分钟进行推理。

hackernews · himata4113 · Jun 17, 09:12 · [社区讨论](https://news.ycombinator.com/item?id=48567759)

**背景**: Z.ai（原智谱 AI）是中国一家知名的 AI 公司，被称为“AI 四小龙”之一，其 GLM 系列模型自 2025 年 7 月起开源。Artificial Analysis 是一个独立的基准测试平台，评估 AI 模型的质量、价格、速度和延迟。GLM-5.2 是最新的旗舰模型，针对长时推理任务进行了优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM-5.2">GLM-5.2</a></li>
<li><a href="https://z.ai/blog/glm-5.2">GLM-5.2: Built for Long-Horizon Tasks</a></li>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些用户赞扬该模型成本低、质量高，称其为对专有供应商的“巨大打击”，而另一些用户则批评其推理效率低下，指出完成一个简单的编程任务需要 15 分钟。此外，还有关于该模型在编程基准测试中与 GPT-5.5 等竞品相比性能的讨论。

**标签**: `#AI/ML`, `#open-weights`, `#LLM`, `#pricing`, `#reasoning`

---

<a id="item-8"></a>
## [Charity Majors: AI 让代码生成变得免费且可抛弃](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

Charity Majors 指出，到 2025 年，代码生产的经济学已发生逆转：生成代码变得几乎免费且即时，代码行从被珍藏的资产变成了可抛弃的商品。 这一转变从根本上改变了软件工程的实践和激励方式，要求更多的纪律而非更少，并对开发者的工作方式和软件构建方式产生广泛影响。 该引文来自 Majors 在 Substack 上发表的文章《AI 要求更多的工程纪律，而非更少》，强调这一变化在 2025 年“几乎一夜之间”发生。

rss · Simon Willison · Jun 17, 17:12

**背景**: 传统上，编写代码是劳动密集型的，因此代码会被仔细地重用和维护。像大型语言模型（LLM）这样的 AI 辅助编程工具可以按需生成代码，极大地降低了创建新代码的成本。

**标签**: `#ai-assisted-programming`, `#generative-ai`, `#software-engineering`, `#economics`, `#charity-majors`

---

<a id="item-9"></a>
## [中国将科创板第五套标准扩展至人工智能与硬科技](https://mp.weixin.qq.com/s/ywLPXkSlqY9S5Vwp8G5saA) ⭐️ 8.0/10

证监会主席吴清在 2026 陆家嘴论坛上宣布，科创板第五套上市标准的适用范围将扩大至人工智能、量子科技、生物制造和具身智能等硬科技领域，允许更多未盈利的硬科技企业上市。 这一政策转变表明政府对人工智能等前沿技术的大力支持，为早期、高研发投入的公司提供了关键的资本渠道。它可能加速创新并重塑中国科技生态系统，尤其有利于寻求公开融资的未盈利 AI 初创企业。 吴清还表示将严查借科技之名蹭热点、炒概念等违法行为，并适时发布规范资本市场人工智能的指导意见。此外，证监会将推出储架发行等再融资改革，以及支持上海国际金融中心建设的四项政策。

telegram · zaihuapd · Jun 17, 08:30

**背景**: 科创板于 2019 年设立，旨在引导资本投向硬科技和创新型企业，设有五套上市标准。第五套标准专门针对尚未盈利但估值预期高的生物科技公司。储架发行是指发行人预先注册证券发行计划，在有效期内分次发行，以提高融资效率。具身智能是指拥有物理身体并能与现实世界交互的 AI 系统，被视为 AI 发展的关键下一步。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://zhoukan.cc/jujiao/2025/0626/062025_347582.html">每日热门： 第 五 套 标 准 正式重启 科 创 板 聚焦构建 创 新新生态_环球周刊网</a></li>
<li><a href="https://wallstreetcn.com/articles/3752510">科 创 板 “ 第 五 套 ”重启首单解析：泰诺麦博核心药品刚上市遇竞品“打5折”</a></li>
<li><a href="https://tubex.chat/zh/article/article-1775822504934-8c93c1">创业板深化改革：第四套标准+ 储 架 发 行 赋能新质生产力 - TubeX.Chat AI</a></li>

</ul>
</details>

**标签**: `#AI`, `#regulation`, `#STAR Market`, `#China`, `#tech policy`

---

<a id="item-10"></a>
## [Anthropic 企业 AI 市场份额首次超越 OpenAI](https://techcrunch.com/2026/06/16/anthropics-latest-feud-with-the-trump-admin-may-actually-help-it-sales-data-suggests/) ⭐️ 8.0/10

根据 Ramp 数据，Anthropic 的企业 AI 订阅份额在 5 月达到 41%，首次超过 OpenAI 的 39.5%。 这一里程碑表明企业 AI 市场发生重大转变，尽管与政府关系紧张，Anthropic 对安全与合规的关注似乎赢得了企业认可。 该数据来自企业支出管理平台 Ramp，而市场份额增长发生在特朗普政府要求 Anthropic 禁止非美国用户访问其最新模型 Mythos 5 和 Fable 5 之际。

telegram · zaihuapd · Jun 17, 09:30

**背景**: Anthropic 是一家以安全与道德 AI 开发闻名的 AI 公司，其 Claude Opus 系列是目前企业使用的主要模型。Ramp 追踪企业软件支出，提供市场份额趋势洞察。与政府的冲突源于对 Anthropic 最先进模型的出口管制担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://ramp.com/enterprise">Enterprise Spend & Expense Management Software | Ramp</a></li>

</ul>
</details>

**标签**: `#AI`, `#Market Share`, `#Anthropic`, `#OpenAI`, `#Enterprise`

---

<a id="item-11"></a>
## [微软借助 OpenAI 模型在中国拓展 AI 业务](https://www.bloomberg.com/news/articles/2026-06-17/microsoft-s-china-ai-business-grows-on-openai-model-sales) ⭐️ 8.0/10

微软通过 Azure 向中国科技公司销售 OpenAI 模型，在华业务快速增长，字节跳动是其最大客户，年投入超 10 亿美元。蚂蚁集团、美团和腾讯也是重要买家。 这一快速增长引发了美国官员和立法者对 AI 安全以及中国公司可能进行模型蒸馏的担忧。这凸显了 AI 领域的地缘政治紧张局势，以及微软作为 OpenAI 与中国之间桥梁的微妙处境。 OpenAI 曾私下抱怨微软未充分阻止中国公司“蒸馏”其模型。微软称只向成熟企业而非个人开发者销售模型，且模型托管在境外数据中心，客户需经互联网访问。

telegram · zaihuapd · Jun 18, 01:06

**背景**: 模型蒸馏是一种将大型强大 AI 模型的知识转移到更小更高效模型的技术，常用于降低成本或便于部署。该过程可合法使用，但应用于专有模型时也会引发知识产权担忧。美中科技竞争加剧，双方都对技术转让和安全风险保持警惕。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_distillation">Model distillation</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#OpenAI`, `#China`, `#AI models`, `#Azure`

---