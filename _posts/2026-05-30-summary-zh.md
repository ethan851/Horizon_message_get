---
layout: default
title: "Horizon Summary: 2026-05-30 (ZH)"
date: 2026-05-30
lang: zh
---

> From 29 items, 12 important content pieces were selected

---

1. [中国首次将 9 款国产 AI 芯片纳入政府采购目录](#item-1) ⭐️ 9.0/10
2. [蓝色起源新格伦火箭静态点火测试爆炸](#item-2) ⭐️ 9.0/10
3. [vllm v0.22.0 发布，带来 DeepSeek V4、Model Runner V2 和 Rust 前端](#item-3) ⭐️ 8.0/10
4. [SQLite 被视为足以用于持久化工作流](#item-4) ⭐️ 8.0/10
5. [AI 垃圾：缺乏动机的输出](#item-5) ⭐️ 8.0/10
6. [GTA 6 开发者成立工会以对抗加班文化](#item-6) ⭐️ 8.0/10
7. [开发者必须比 AI 编码助手更聪明](#item-7) ⭐️ 8.0/10
8. [微软零日漏洞纠纷升级，研究员威胁再次泄露漏洞利用](#item-8) ⭐️ 8.0/10
9. [Datasette 1.0a31 新增写入查询和保存查询功能](#item-9) ⭐️ 8.0/10
10. [Anthropic 估值超越 OpenAI，成为最高估值 AI 公司](#item-10) ⭐️ 8.0/10
11. [印度 CBSE 网上阅卷系统安全漏洞曝光](#item-11) ⭐️ 8.0/10
12. [华为提出“韬定律”，以时间缩微推动芯片演进](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [中国首次将 9 款国产 AI 芯片纳入政府采购目录](https://www.tomshardware.com/tech-industry/semiconductors/china-certifies-nine-domestic-ai-chips-for-government-procurement) ⭐️ 9.0/10

中国信息安全测评中心首次在安全认证框架下新增“AI 训练与推理芯片”品类，共有 9 款国产 AI 处理器通过认证，包括华为昇腾、阿里平头哥镇武、壁仞科技、海光等。 该认证将作为政府机构和国有企业采购的依据，标志着政策向国产 AI 芯片的重大倾斜，加速了中国在关键半导体领域实现技术自主可控的进程。 认证有效期为三年，寒武纪和百度昆仑芯未出现在名单中。该目录覆盖用于 AI 训练和推理的芯片，体现了全面安全的采购思路。

telegram · zaihuapd · May 29, 08:41

**背景**: 中国的“安可”安全可靠采购目录是政府认可的 IT 产品清单，关键信息基础设施运营者必须优先采购。首次将 AI 芯片纳入该目录，将这一框架扩展至先进计算硬件，反映了对依赖英伟达等外国技术的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anbob.com/archives/8415.html">2023、2024、2025、2026 四批次数据库 安可 ( 安全 可靠测评) 目录 列表 – ...</a></li>
<li><a href="https://blog.csdn.net/yts1985/article/details/139064348">第一批 安全 可靠测评结果 (1-2023)_ 安可目录 -CSDN博客</a></li>
<li><a href="https://cloud.tencent.com/developer/article/1958838">国务院要求关键信息基础设施运营者应优先 采购 「 安可 产品和服务」：包...</a></li>

</ul>
</details>

**标签**: `#国产芯片`, `#AI芯片`, `#政府采购`, `#半导体`, `#自主可控`

---

<a id="item-2"></a>
## [蓝色起源新格伦火箭静态点火测试爆炸](https://arstechnica.com/space/2026/05/blue-origins-new-glenn-rocket-just-exploded-during-a-static-fire-test/) ⭐️ 9.0/10

这一事件严重延误了蓝色起源的发射计划，影响了 NASA 阿尔忒弥斯计划的月球着陆器任务和亚马逊 Project Kuiper 卫星宽带部署。同时引发了对 BE-4 发动机可靠性和新格伦火箭飞行准备状态质疑。 爆炸发生在 NG-4 任务准备阶段，原计划发射 48 颗亚马逊 Kuiper 卫星。无人员伤亡，但发射台的闪电防护塔倒塌。蓝色起源尚未公布修复和复飞时间表。

telegram · zaihuapd · May 29, 11:08

**背景**: 静态点火测试是一种常规的发射前测试，火箭发动机以全功率点火，但火箭被牢牢固定在发射台上。BE-4 是一种富氧分级燃烧发动机，使用液氧和甲烷，由蓝色起源开发，也用于联合发射联盟的火神火箭。Project Kuiper（现更名为 Amazon Leo）是亚马逊的低地球轨道卫星互联网星座，已与包括蓝色起源在内的多家供应商签订了发射合同。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Static_fire_test">Static fire test</a></li>
<li><a href="https://en.wikipedia.org/wiki/BE-4">BE-4 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Project_Kuiper">Project Kuiper</a></li>

</ul>
</details>

**标签**: `#Blue Origin`, `#New Glenn`, `#rocket explosion`, `#NASA Artemis`, `#aerospace`

---

<a id="item-3"></a>
## [vllm v0.22.0 发布，带来 DeepSeek V4、Model Runner V2 和 Rust 前端](https://github.com/vllm-project/vllm/releases/tag/v0.22.0) ⭐️ 8.0/10

vllm v0.22.0 正式发布，包含来自 230 位贡献者的 459 次提交，主要亮点包括对 DeepSeek V4 的重大加固、Model Runner V2 的进展使其逐步成为默认选项，以及实验性的 Rust 前端。 此版本显著提升了大语言模型的推理性能和硬件支持，尤其是针对 DeepSeek V4，并引入了可能降低开销的实验性 Rust 前端。这表明 vllm 作为 AI 推理生态系统关键工具的持续演进。 值得注意的技术改进包括为 DeepSeek V4 添加的 NVFP4 融合 MoE 支持、MTP 推测解码、超越 CPU 内存的多层级 KV 缓存卸载，以及使用 Cutlass FP8 实现批量无关推理，端到端延迟降低 28.9%。

github · khluu · May 29, 10:28

**背景**: vllm 是一个开源、高吞吐量的大语言模型推理引擎，专为优化大型模型的服务而设计。DeepSeek V4 是一个先进的混合专家模型。Model Runner V2 (MRv2) 是重构的推理流水线，旨在提升性能和可维护性。实验性的 Rust 前端用于替代 Python 层，以降低开销并加快启动速度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-speculative-decoding-for-reducing-latency-in-ai-inference/">An Introduction to Speculative Decoding for Reducing Latency in AI Inference | NVIDIA Technical Blog</a></li>
<li><a href="https://deepwiki.com/vllm-project/vllm/7.4-moe-quantization-and-backend-selection">MoE Quantization and Backend Selection | vllm-project/vllm | DeepWiki</a></li>

</ul>
</details>

**标签**: `#vllm`, `#LLM inference`, `#DeepSeek V4`, `#Model Runner`, `#Rust`

---

<a id="item-4"></a>
## [SQLite 被视为足以用于持久化工作流](https://obeli.sk/blog/sqlite-is-all-you-need-for-durable-workflows/) ⭐️ 8.0/10

一篇博文主张 SQLite 足以构建持久化工作流，引发了关于其在生产并发场景下是否适合与 Postgres 等替代方案相比的讨论。 这一点很重要，因为许多开发者正在评估用于工作流编排的轻量级数据库选项，而这场辩论凸显了简单性与并发性之间的权衡。 SQLite 支持无限并发读取，但每次只允许一个写入者，这可能成为写入密集型工作流的瓶颈。一些评论者提议使用 SQLite 结合 S3 的 compare-and-swap 或分片来改善并发性。

hackernews · tomasol · May 29, 17:54 · [社区讨论](https://news.ycombinator.com/item?id=48326802)

**背景**: 持久化工作流确保长时间运行或多步骤的操作即使在出现故障时也能可靠完成，通常使用数据库来持久化状态。SQLite 是一个嵌入式 SQL 数据库，无需服务器进程，部署简单，但与 Postgres 等客户端-服务器数据库相比，并发能力有限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite.org/whentouse.html">Appropriate Uses For SQLite</a></li>
<li><a href="https://www.inngest.com/uses/durable-workflows">Inngest - Durable Workflows</a></li>
<li><a href="https://jellyfin.org/posts/SQLite-locking/">SQLite concurrency and why you should care about it | Jellyfin</a></li>

</ul>
</details>

**社区讨论**: 社区评论意见分歧：一些人称赞 SQLite 在小型项目中的简洁性（例如替换多个 SaaS 工具），而另一些人则认为由于其并发限制，不适合生产环境。一个新颖的解决方案使用 SQLite sessions 扩展结合 S3 的 compare-and-swap 实现安全的并发访问。

**标签**: `#SQLite`, `#workflows`, `#databases`, `#concurrency`, `#distributed-systems`

---

<a id="item-5"></a>
## [AI 垃圾：缺乏动机的输出](https://noperator.dev/posts/you-can-just-say-it/) ⭐️ 8.0/10

antirez 的一篇博客文章将 AI 垃圾定义为缺乏基本动机的输出，区分了对 AI 的滥用与 AI 本身。文章强调，垃圾内容源于缺乏理解或意图，而非使用大语言模型。 这种区分提供了一个清晰的思维模型，可以在不指责技术本身的情况下批判 AI 的滥用，这对在 AI 时代中航行的软件工程师和写作者至关重要。它有助于保留人类在沟通中的意图价值。 文章刻意简洁，与 AI 垃圾形成对比，作者是 noperator.dev 的 antirez。社区讨论有 115 条评论，参与度高（评分 8.0，231 分）。

hackernews · antirez · May 29, 15:54 · [社区讨论](https://news.ycombinator.com/item?id=48324853)

**背景**: AI 垃圾指由 AI 生成的低质量、无意义的内容，常因缺乏实质而受到批评。随着 AI 生成的文本变得普遍，这个术语在技术社区中流行起来。这篇文章认为，垃圾并非 AI 固有，而是源于用户在没有真实动机或理解的情况下产生输出。

**社区讨论**: 社区评论普遍积极且具有反思性。cautiouscat 引用了朋友的话，更希望收到原始提示而非 LLM 生成的邮件。beering 希望 AI 能将人类价值与工作产出脱钩。antirez 本人称这是对 AI 垃圾的最佳定义。sbiru93 感到个人解脱，drooby 指出艺术和体育因创作者意图而保有价值。

**标签**: `#AI`, `#LLM`, `#writing`, `#slop`, `#communication`

---

<a id="item-6"></a>
## [GTA 6 开发者成立工会以对抗加班文化](https://rockstarintel.com/gta-6-developers-announce-rockstar-games-union/) ⭐️ 8.0/10

参与《侠盗猎车手 VI》开发的 Rockstar Games 员工宣布成立工会，要求薪资透明、弹性工作以及结束名为“加班文化”的强制加班。 此次工会化运动旨在解决游戏行业系统性的劳工剥削问题，其中加班文化导致员工每周工作 65-80 小时且无合理补偿。若成功，可能为其他游戏工作室树立先例，并改善工作条件及游戏质量。 工会的要求包括薪资透明、弹性工作以及结束加班——游戏开发中常见的无薪加班现象。行业数据显示，游戏发布前后数月内加班可能持续，影响员工健康与留存率。

hackernews · AndrewKemendo · May 29, 15:32 · [社区讨论](https://news.ycombinator.com/item?id=48324499)

**背景**: 加班文化指视频游戏开发中普遍存在的长时间无薪加班现象，通常由公司压力和同辈影响驱动。员工可能连续数月每周工作 65-80 小时，导致倦怠和高离职率。工会化是对这些状况日益增长的回应，Rockstar Games 的此次行动是一个显著例子。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Crunch_(video_games)">Crunch (video games) - Wikipedia</a></li>
<li><a href="https://jacobin.com/2023/10/video-game-workers-crunch-exploitation-union-organizing">The Video Game Industry Calls It “Crunch.” Workers Call It Exploitation.</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了对工会的支持，指出游戏开发者薪资与大型科技公司之间的差距，并强调加班文化剥削员工。有人指出在美国由于外包和 H1B 签证而难以组建工会，但总体情绪对改善工作条件持积极态度。

**标签**: `#labor rights`, `#gaming industry`, `#unionization`, `#crunch culture`

---

<a id="item-7"></a>
## [开发者必须比 AI 编码助手更聪明](https://vickiboykis.com/2026/05/28/we-should-be-more-tired-than-the-model/) ⭐️ 8.0/10

一篇博客文章认为，开发者必须保持比他们使用的 AI 模型更深入的理解和批判性思维，强调在 AI 辅助编码中的人工监督。 这突显了开发者角色从编写代码向监督 AI 代理的演变，涉及技能保留的担忧以及在软件工程中需要更高层次监督的问题。 作者认为 AI 辅助编码的瓶颈在于理解，抽象是管理复杂性的关键工具，但指出开发者从未真正掌握抽象。

hackernews · tosh · May 29, 12:12 · [社区讨论](https://news.ycombinator.com/item?id=48322118)

**社区讨论**: 评论者意见不一：有人同意开发者技能依然关键，另一些人则认为角色正向产品管理技能转变，并质疑技能退化是否如所述那般严重。

**标签**: `#AI-assisted coding`, `#software engineering`, `#developer skills`, `#productivity`

---

<a id="item-8"></a>
## [微软零日漏洞纠纷升级，研究员威胁再次泄露漏洞利用](https://www.theregister.com/security/2026/05/28/microsoft-0-day-feud-escalates-as-researcher-threatens-another-windows-exploit-dump/5248085) ⭐️ 8.0/10

一名安全研究员威胁要发布更多针对微软 Windows 的零日漏洞利用代码，使关于负责任披露和补偿的公开纠纷升级。 这可能导致数百万 Windows 用户面临未修补的漏洞风险，并凸显了安全研究社区与大型厂商在披露实践上的持续紧张关系。 该研究员声称微软违反了协调漏洞披露（CVD）原则，未能进行沟通或提供足够的补偿，从而引发公开泄露漏洞利用的威胁。

hackernews · Cider9986 · May 29, 19:37 · [社区讨论](https://news.ycombinator.com/item?id=48328175)

**背景**: 零日漏洞是软件厂商未知的安全缺陷，导致其在补丁发布前可被利用。负责任披露（也称协调漏洞披露 CVD）是指研究者私下报告漏洞，让厂商有时间修复后再公开披露的过程。当研究者认为厂商回应不及时或赏金不公时，可能引发争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero - day vulnerability - Wikipedia</a></li>
<li><a href="https://www.bugcrowd.com/resources/guide/what-is-responsible-disclosure/">What is Responsible Disclosure? | Bugcrowd</a></li>
<li><a href="https://www.hackerone.com/knowledge-center/why-you-need-responsible-disclosure-and-how-get-started">Why You Need Responsible Disclosure and How to Get Started | HackerOne</a></li>

</ul>
</details>

**社区讨论**: 评论者大多同情研究员，批评微软复杂的漏洞报告系统和缺乏适当的认可。一些人担心泄露的漏洞利用会危及潜在受害者，而另一些人指出厂商在处理大量报告（包括 AI 生成的垃圾信息和不切实际的期望）时所面临的困难。

**标签**: `#security`, `#0-day`, `#Microsoft`, `#responsible disclosure`, `#exploit`

---

<a id="item-9"></a>
## [Datasette 1.0a31 新增写入查询和保存查询功能](https://simonwillison.net/2026/May/29/datasette/#atom-everything) ⭐️ 8.0/10

Datasette 1.0a31 引入了权限用户执行写入查询（INSERT、UPDATE、DELETE）以及保存存储查询（原“canned queries”）的功能，可设为私密或供实例中其他用户使用。 此版本是迈向 Datasette 1.0 的重要一步，将其从只读工具转变为支持数据库修改的工具，实现了实例内的协作数据编辑和查询共享。 新的执行查询界面支持模板化的插入/更新/删除查询，用户只能执行其有相应权限的语句（例如 CREATE TABLE 需要 create-table 权限）。存储查询是原“canned queries”的重新命名。

rss · Simon Willison · May 29, 03:32

**背景**: Datasette 是一个用于探索和发布 SQLite 数据库的开源工具。此前，它只允许只读查询。这个 alpha 版本增加了写入能力，使其更具交互性，适合需要数据编辑的应用场景。“存储查询”一词取代了之前的名称“canned queries”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.datasette.io/en/latest/sql_queries.html">Running SQL queries - Datasette documentation</a></li>
<li><a href="https://github.com/datasette/datasette-queries">Save SQL queries in Datasette - GitHub</a></li>

</ul>
</details>

**标签**: `#datasette`, `#SQL`, `#database`, `#data publishing`, `#open source`

---

<a id="item-10"></a>
## [Anthropic 估值超越 OpenAI，成为最高估值 AI 公司](https://www.nytimes.com/2026/05/28/technology/anthropic-tops-openai-valuation.html) ⭐️ 8.0/10

Anthropic 完成 650 亿美元 H 轮融资，投后估值达到 9650 亿美元，超过 OpenAI 的约 8520 亿美元估值，成为估值最高的 AI 初创公司。 这一估值里程碑标志着 AI 行业的重大转变，投资者对 Anthropic 的技术和市场地位显示出巨大信心。它凸显了在大语言模型领域领先所需的激烈竞争和资本投入。 Anthropic 的 Claude 模型系列，包括最新的 Claude Opus 4.8，在企业 AI 任务中实现了顶尖性能。650 亿美元的融资轮是历史上最大的私人融资之一，资金主要用于算力、模型训练和商业化。

telegram · zaihuapd · May 29, 03:29

**背景**: Anthropic 是一家由前 OpenAI 员工创立的 AI 公司，专注于开发大语言模型，并通过其宪法 AI 技术强调安全性和合规性。其旗舰产品 Claude 直接与 OpenAI 的 GPT 系列竞争。估值飙升反映了市场对高级 AI agent 和企业解决方案的需求不断增长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/05/28/anthropic-open-ai-startup-value.html">Anthropic tops OpenAI as most valuable AI startup, nears $1T ...</a></li>
<li><a href="https://www.theguardian.com/technology/2026/may/28/anthropic-ai-valuation">Anthropic reaches valuation of $965bn, beating OpenAI to become...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model ) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI`, `#funding`, `#Anthropic`, `#valuation`, `#industry news`

---

<a id="item-11"></a>
## [印度 CBSE 网上阅卷系统安全漏洞曝光](https://ni5arga.com/blog/posts/hacking-cbse/) ⭐️ 8.0/10

一名研究者披露了印度中央中等教育委员会（CBSE）高考网上阅卷系统的多项严重漏洞，包括前端硬编码主密码、OTP 在浏览器端校验、可绕过登录访问页面、改任意账号密码不验证旧密码等，可能导致阅卷员账号被接管并篡改分数。 这些漏洞威胁到印度高考的公平性，可能导致大规模分数篡改，损害教育公信力。该事件凸显了处理敏感数据的官方教育系统在安全设计上的重大缺陷。 研究者于 2026 年 2 月 25 日向印度 CERT-In 报告了这些漏洞，但 CBSE 最初否认漏洞存在。作者随后补充了截图、录屏和归档链接作为证据，并在网站下线前发现了额外的 SQL 注入漏洞。

telegram · zaihuapd · May 29, 05:52

**背景**: 硬编码密码是指直接将密码嵌入源代码中，容易被提取。OTP 在客户端校验意味着一次性密码可以在浏览器端被拦截或修改而绕过。SQL 注入是一种通过在输入字段中注入恶意 SQL 语句来操纵后端数据库的攻击手段。这些都是开发阶段本应避免的常见安全漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.m.wikipedia.org/wiki/One-time_password">One-time password - Wikipedia</a></li>
<li><a href="https://en.m.wikipedia.org/wiki/SQL">SQL - Wikipedia</a></li>

</ul>
</details>

**标签**: `#安全漏洞`, `#漏洞披露`, `#网络安全`, `#网上阅卷系统`, `#印度`

---

<a id="item-12"></a>
## [华为提出“韬定律”，以时间缩微推动芯片演进](https://t.me/zaihuapd/41648) ⭐️ 8.0/10

在上海举行的 2026 国际电路与系统研讨会上，华为提出了以“时间缩微”替代“几何缩微”的半导体演进新原则“韬定律”。华为还宣布，过去六年已据此设计量产了 381 款芯片，今年秋季将推出采用逻辑折叠技术的新麒麟芯片。 “韬定律”为在摩尔定律逼近物理极限后继续推进半导体发展提供了可能的路径。如果成功，它可能重塑全球芯片产业，并减少对极紫外光刻技术的依赖。华为声称，到 2031 年基于该定律的高端芯片晶体管密度可达 1.4 纳米制程同等水平。 采用逻辑折叠技术的麒麟 2026 芯片据称可实现每平方毫米 2.38 亿个晶体管的密度，高于台积电 N3E 工艺。然而，早期基准测试估计其单核性能在 Geekbench 6 上比高通最新旗舰落后约 47%。

telegram · zaihuapd · May 30, 02:18

**背景**: 摩尔定律是指芯片上晶体管数量大约每两年翻一番的观察结果，几十年来推动了半导体进步，但因物理限制而逐渐放缓。传统的几何缩微缩小晶体管尺寸，而“韬定律”则通过器件、电路、芯片到系统的多层级协同优化，降低时间常数（信号切换所需时间）。逻辑折叠是一种芯片设计技术，通过堆叠逻辑层来增加密度，类似于 3D 堆叠但更为激进，是华为在美国出口限制下进行创新战略的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.globaltimes.cn/page/202605/1361994.shtml">The Tau Scaling Law comes out: Chinese innovation is... - Global Times</a></li>
<li><a href="https://en.c114.com.cn/577/a1311082.html">Huawei Unveils New Semiconductor Law : The " Tao ..."</a></li>
<li><a href="https://www.gizmochina.com/2026/05/25/huawei-previews-kirin-2026-chip-with-higher-transistor-density-and-efficiency/">Huawei previews Kirin 2026 chip with higher transistor density and...</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#Moore's law`, `#Huawei`, `#chip design`, `#technology breakthrough`

---