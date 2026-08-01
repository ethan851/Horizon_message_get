---
layout: default
title: "Horizon Summary: 2026-08-01 (ZH)"
date: 2026-08-01
lang: zh
---

> From 31 items, 6 important content pieces were selected

---

1. [电梯调度算法：SCAN、LOOK 与目的楼层派梯](#item-1) ⭐️ 8.0/10
2. [YC 发布 qm：面向工作的多人智能体框架](#item-2) ⭐️ 8.0/10
3. [Tailscale 未能阻止 Hugging Face 入侵事件](#item-3) ⭐️ 8.0/10
4. [DeepSeek V4 Flash 0731：3040 亿参数智能体模型，性价比之王](#item-4) ⭐️ 8.0/10
5. [无状态 MCP 2.0 重燃热情，催生 mcp-explorer 与 datasette-mcp](#item-5) ⭐️ 8.0/10
6. [OpenAI 封禁柬埔寨诈骗团伙的 ChatGPT 账号网络](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [电梯调度算法：SCAN、LOOK 与目的楼层派梯](https://john.fun/elevators) ⭐️ 8.0/10

john.fun/elevators 上的这篇文章对电梯调度算法及其效率进行了技术分析。随之而来的 Hacker News 讨论（901 分、223 条评论）通过将其与磁盘调度和目的楼层派梯系统进行类比，扩展了该话题。 电梯调度影响着从办公大楼到磁盘驱动器等方方面面，简单算法与现代目的楼层派梯之间的取舍具有实际意义。对于希望了解这些算法在真实场景中表现的系统工程师和算法爱好者来说，这场讨论很有价值。 从社区讨论来看，文章可能比较了 FCFS、SSTF、SCAN 和 LOOK 等算法。评论者指出，SCAN 也是一种磁盘调度算法，并且目的楼层派梯在随机目的地场景下可能表现不佳，但在午餐高峰等真实客流模式下表现出色。

hackernews · Jrh0203 · Jul 31, 15:17 · [社区讨论](https://news.ycombinator.com/item?id=49124218)

**背景**: 电梯算法又称 SCAN，它让磁盘臂或电梯沿一个方向移动并在途中处理请求，然后掉头反向服务。LOOK 是 SCAN 的变体，只移动到最后一个待处理请求的位置。目的楼层派梯需要乘客输入目标楼层，系统从而可将去往同一楼层的乘客分组，减少等待和乘坐时间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Destination_dispatch">Destination dispatch - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Elevator_algorithm">Elevator algorithm - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/operating-systems/disk-scheduling-algorithms/">Disk Scheduling Algorithms - GeeksforGeeks</a></li>

</ul>
</details>

**社区讨论**: 评论者将电梯调度与磁盘调度联系起来：peterldowns 指出 HDD 就像一个很长的电梯，SCAN 是一种磁盘调度算法。omoikane 质疑文章的对比，指出目的楼层派梯在真实场景中表现出色；hermanschaaf 则说他在电梯游戏中选择了 LOOK，因为它符合用户预期。还有人分享了 Elevator Saga 游戏链接，并抱怨用户会同时按下上行和下行按钮。

**标签**: `#algorithms`, `#elevators`, `#scheduling`, `#simulation`, `#systems`

---

<a id="item-2"></a>
## [YC 发布 qm：面向工作的多人智能体框架](https://github.com/yc-software/qm) ⭐️ 8.0/10

Y Combinator 发布了 qm，这是一个面向工作的多人智能体（agent）框架，项目托管在 github.com/yc-software/qm。它引入了共享房间和每人单独的作用域，让团队可以协作使用 AI 智能体，同时每个人又能保有自己的个性化智能体。 qm 标志着 AI 从单用户助手向团队级协作智能体的转变，并尝试解决多智能体工作流中最难的问题之一：作用域与权限管理。如果这一方向成功，它可能会影响企业构建内部 AI 工具的方式；该新闻在 Hacker News 上获得 472 分和 101 条评论，也说明开发者社区对其高度关注。 仓库描述中提到“个人与共享作用域”（personal and shared scopes）：用户可以把智能体定制成自己的，同时仍然在 Slack 频道和项目中协作使用它。该框架通过让每个用户拥有自己的作用域、同时支持共享房间，来避免将个人助手扩展到全公司时常见的复杂性问题。

hackernews · tosh · Jul 31, 18:04 · [社区讨论](https://news.ycombinator.com/item?id=49126604)

**背景**: 智能体框架（agent harness）是 AI 模型之外、让智能体真正可用的所有部分，包括上下文管理、工具、记忆和用户界面；Martin Fowler 将其概括为“Agent = Model + Harness”。协作式 AI（Collaborative AI）是一种设计模式，让多个团队成员在共享空间中与 AI 协作并保持协调，而不是每个人孤立地使用 AI。qm 把这个模式应用到了工作场景，让团队能在 Slack 和项目中共享智能体，同时保留个人定制能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/yc-software/qm">GitHub - yc-software/qm: Multiplayer agent harness for work · GitHub</a></li>
<li><a href="https://martinfowler.com/articles/harness-engineering.html">Harness engineering for coding agent users</a></li>
<li><a href="https://www.aiuxdesign.guide/patterns/collaborative-ai">Collaborative AI — What It Is & How to Design Human-AI Collaboration | AI Design Patterns</a></li>

</ul>
</details>

**社区讨论**: 评论既包含质疑也包含认可：有人要求与 Claude Cowork 做对比，并质疑其相比现有工具的优势；也有人分享了一个幽默的故事——智能体自己开始和其他智能体安排会议。做相邻领域（AQ.dev）的开发者认为 qm 的“每人作用域 + 共享房间”是公司级助手的合理答案，还有人表示想了解 qm 如何处理组织级上下文与安全。

**标签**: `#AI agents`, `#multiplayer`, `#Y Combinator`, `#collaboration`, `#developer tools`

---

<a id="item-3"></a>
## [Tailscale 未能阻止 Hugging Face 入侵事件](https://tailscale.com/blog/hugging-face-intrusion) ⭐️ 8.0/10

Tailscale 发布了一篇博客文章分析 Hugging Face 入侵事件，指出没有 Tailscale 漏洞被利用。相反，存储在环境文件中的可复用认证密钥（auth key）使攻击者能够在数天内将 181 个未授权节点注册到 Hugging Face 的 tailnet 中。 这一事件很重要，因为它表明即使是个安全的 Mesh 网状 VPN，也可能因凭据管理不善而被攻破；一个泄漏的可复用认证密钥就让攻击者进入了目标的私有网络。它还暴露了 Tailscale 在告警方面存在的空白，安全从业者应当重视。 泄漏的密钥是一个可复用的 Tailscale 认证密钥，用于创建 CI 节点；攻击者利用它在 Hugging Face 的 tailnet 中注册了 181 个带 CI 身份标签的节点。Tailscale 的节点密钥默认每 180 天过期，但可复用认证密钥如果没有绑定来源/目的地，仍可能被滥用。

hackernews · bluehatbrit · Jul 31, 19:03 · [社区讨论](https://news.ycombinator.com/item?id=49127306)

**背景**: Tailscale 是一个基于 WireGuard 构建的 Mesh 网状 VPN，可通过点对点模型在互联网上的设备之间建立安全连接。在 Tailscale 中，'tailnet' 是指用户的私有设备网络，'node'（节点）是运行 Tailscale 的机器。'Auth key'（认证密钥）是一种预认证密钥，用于将节点自动加入 tailnet，通常用于 CI/CD 等自动化场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tailscale.com/docs/features/access-control/auth-keys">Auth keys · Tailscale Docs</a></li>
<li><a href="https://tailscale.com/learn/understanding-mesh-vpns">Understanding mesh network topology (mesh VPNs)</a></li>

</ul>
</details>

**社区讨论**: 评论区总体对 Tailscale 的透明度表示赞赏，例如用户 john_strinlai 赞扬该公司没有选择沉默。但也有像 ahofmann 这样的用户认为这既是'聪明的营销'，同时指出 Hugging Face 把可复用认证密钥放在环境文件里是糟糕的做法。simonw 指出这次入侵暴露出告警机会，angry_octet 则认为长期凭据应绑定到特定的来源/目的地。

**标签**: `#security`, `#tailscale`, `#credential-management`, `#incident-response`, `#mesh-vpn`

---

<a id="item-4"></a>
## [DeepSeek V4 Flash 0731：3040 亿参数智能体模型，性价比之王](https://simonwillison.net/2026/Jul/31/deepseek-v4-flash-0731/#atom-everything) ⭐️ 8.0/10

DeepSeek 发布了 DeepSeek-V4-Flash-0731，这是一个拥有 3040 亿参数、智能体能力显著增强的模型，定价为每百万输入 token 0.14 美元、每百万输出 token 0.27 美元。Artificial Analysis 将其排在 4280 亿参数的 MiniMax M3 之前。 此次发布巩固了 DeepSeek 在 AI 性价比前沿的领先地位，以远低于竞争对手的价格提供接近顶级的智能水平。这可能会加速智能体 AI 在注重 API 成本的真实应用中的采用。 该模型在 Hugging Face 上大小为 167GB，参数规模为 3040 亿。Simon Willison 通过 OpenRouter 的测试显示，默认推理强度生成的效果一般，而将 `reasoning_effort` 设为 high 后效果大大改善，凸显了推理级别配置的重要性。

rss · Simon Willison · Jul 31, 23:59

**背景**: 智能体 AI 指的是能够在有限监督下实现特定目标的人工智能系统，通常通过模仿人类决策来实时解决问题。Artificial Analysis 智能指数将多项基准测试汇总为单一模型级智能分数，从而可以在模型之间比较智能水平和每个任务的成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>
<li><a href="https://benchlm.ai/benchmarks/artificialanalysis">Artificial Analysis Intelligence Index Leaderboard... | BenchLM.ai</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#LLM`, `#AI`, `#model release`, `#agentic`

---

<a id="item-5"></a>
## [无状态 MCP 2.0 重燃热情，催生 mcp-explorer 与 datasette-mcp](https://simonwillison.net/2026/Jul/31/stateless-mcp/#atom-everything) ⭐️ 8.0/10

Simon Willison 报道了新推出的无状态 MCP 规范（2026-07-28 版 Model Context Protocol 发布），该规范允许通过单个 HTTP 请求调用工具，而无需先初始化会话。他还介绍了基于此协议构建的两个新项目：mcp-explorer 和 datasette-mcp。 这是 MCP 规范自发布以来最重要的一次变更，简化了客户端和服务端的实现，使无状态 MCP 更适合可扩展的 Web 应用。它也让 MCP 重新成为比向 AI 代理授予不受限 shell 访问权更可审计、更可控的替代方案。 新的无状态流程在单个请求中使用 MCP-Protocol-Version、Mcp-Method 和 Mcp-Name 等 HTTP 头，消除了对服务端会话 ID 的需求。2026-07-28 规范还包括扩展框架、Tasks、认证加固，并由 Linux 基金会下的 Agentic AI Foundation 管理。

rss · Simon Willison · Jul 31, 23:13

**背景**: MCP 是 Anthropic 于 2024 年 11 月推出的开放标准，旨在标准化 AI 应用连接外部工具和数据源的方式。早期有状态版本需要两次 HTTP 请求——一次初始化会话并获取 Mcp-Session-Id，另一次调用工具——这增加了复杂性和扩展难度。新的无状态核心将这一过程简化为一次请求，使该协议更简单，也更适用于现代基于代理的应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.modelcontextprotocol.io/posts/2026-07-28-release-candidate/">The 2026-07-28 MCP Specification Release Candidate | Model Context Protocol Blog</a></li>
<li><a href="https://venturebeat.com/infrastructure/mcp-just-got-its-biggest-update-ever-heres-what-changes-for-ai-agents">MCP just got its biggest update ever — here’s what changes for AI agents | VentureBeat</a></li>
<li><a href="https://simonwillison.net/2026/Jul/31/stateless-mcp/">Stateless MCP has recaptured my interest (and inspired mcp - explorer ...</a></li>

</ul>
</details>

**标签**: `#MCP`, `#AI`, `#protocol`, `#agents`, `#tools`

---

<a id="item-6"></a>
## [OpenAI 封禁柬埔寨诈骗团伙的 ChatGPT 账号网络](https://openai.com/index/disrupting-malicious-uses-of-ai-criminal-scam-operation/) ⭐️ 8.0/10

OpenAI 宣布封禁一个很可能位于柬埔寨波贝市的 ChatGPT 账号网络，该团伙利用 ChatGPT 进行投资诈骗、杀猪盘、赌博诈骗和冒充执法人员等犯罪活动。最初公告日期为 2026 年 8 月 4 日，OpenAI 后来将日期更正为 7 月 31 日。 该案例是 AI 聊天机器人被武器化用于大规模金融诈骗及与人口贩运相关活动的典型真实案例。它展示了 AI 服务商如何检测和打击恶意使用，并与行业伙伴及执法部门共享威胁情报。 诈骗分子利用 ChatGPT 生成虚假人设、翻译与受害者的对话，并伪造护照和法律文书图片，通常按“接触、建立情感、骗钱”三步套路作案。OpenAI 在收到 WhatsApp 提供的线索后展开调查；该网络可能接触到数百名目标，单个受害者损失达数千美元，部分生成内容还疑似与人口贩运和强迫劳动有关。

telegram · zaihuapd · Jul 31, 23:41

**背景**: 杀猪盘是一种长期诈骗：犯罪分子先通过网恋或交友逐步获取受害者信任，再诱骗其投资虚假项目。东南亚尤其是柬泰边境地区已成为此类犯罪团伙的聚集地，这些团伙往往还涉及人口贩运和强迫劳动。OpenAI 的处置表明 AI 生成内容已进入此类犯罪链条，也说明平台层面的监控可以产出可执行的威胁情报。

**标签**: `#AI Safety`, `#Cybersecurity`, `#OpenAI`, `#Fraud`, `#Abuse Prevention`

---