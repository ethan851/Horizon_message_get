---
layout: default
title: "Horizon Summary: 2026-07-09 (ZH)"
date: 2026-07-09
lang: zh
---

> From 33 items, 14 important content pieces were selected

---

1. [OpenAI 推出 GPT-Live 语音助手，可委托任务给 GPT-5.5](#item-1) ⭐️ 9.0/10
2. [TypeScript 7.0 发布，借助 Go 语言实现 10 倍速度提升](#item-2) ⭐️ 9.0/10
3. [用 AI 智能体将 Bun 重写为 Rust](#item-3) ⭐️ 9.0/10
4. [安卓全版本远程 Root 漏洞链曝光](#item-4) ⭐️ 9.0/10
5. [约翰迪尔用户赢得维修权，FTC 和解](#item-5) ⭐️ 8.0/10
6. [Mistral 推出 Robostral Navigate：无地图机器人导航](#item-6) ⭐️ 8.0/10
7. [xAI 发布 Grok 4.5，效率提升](#item-7) ⭐️ 8.0/10
8. [解码优衣库 T 恤上的混淆 Bash 脚本](#item-8) ⭐️ 8.0/10
9. [Cloudflare Meerkat：全球异步共识协议](#item-9) ⭐️ 8.0/10
10. [阿里巴巴要求员工在 7 月 10 日前卸载 Claude](#item-10) ⭐️ 8.0/10
11. [华为 5G 旗舰重返海外，峰值速度突破 1100 Mbps](#item-11) ⭐️ 8.0/10
12. [美团 OWL 模型在 OpenRouter 测试中疑似会话数据泄露](#item-12) ⭐️ 8.0/10
13. [研究团队通过电磁泄漏识别手机应用，准确率 99%](#item-13) ⭐️ 8.0/10
14. [LineageOS 推出网页刷机工具](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 推出 GPT-Live 语音助手，可委托任务给 GPT-5.5](https://openai.com/index/introducing-gpt-live/) ⭐️ 9.0/10

OpenAI 推出了 GPT-Live，这是一种新语音模型，为 ChatGPT Voice 提供支持，可实现实时自然对话，并能在后台将复杂查询委托给 GPT-5.5。 GPT-Live 弥合了语音交互与前沿 AI 能力之间的差距，让用户在进行流畅语音对话的同时，能访问 GPT-5.5 的高级推理能力来处理编程和研究等任务。 该模型已在 ChatGPT Voice 中可用，并已开放 API 访问的注册页面。早期用户报告了长时间、富有成效的对话，但指出语音模式下缺乏工具/连接器集成。

hackernews · logickkk1 · Jul 8, 17:03 · [社区讨论](https://news.ycombinator.com/item?id=48834405)

**背景**: GPT-Live 是 OpenAI 推出的实时语音助手模型，支持自然对话并能将任务委托给 GPT-5.5。GPT-5.5 是 2026 年 4 月发布的大型语言模型，在编程和数学基准测试中表现优异。以往的语音助手通常使用较旧的模型，能力有限。GPT-Live 旨在将语音的便利性与前沿 AI 的威力结合起来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-live/">Introducing GPT-Live | OpenAI</a></li>
<li><a href="https://openai.com/index/introducing-gpt-5-5/">Introducing GPT‑5.5 - OpenAI</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：一些用户对自然对话和委托功能印象深刻，而另一些人则担心 AI 语音助手可能进一步减少人际交流。一个显著的批评是语音模式下无法使用工具或连接器，这限制了生产力场景的使用。

**标签**: `#AI`, `#Voice Assistant`, `#GPT`, `#OpenAI`, `#Natural Language Processing`

---

<a id="item-2"></a>
## [TypeScript 7.0 发布，借助 Go 语言实现 10 倍速度提升](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

微软宣布发布 TypeScript 7.0，其编译器从 JavaScript 完全移植到 Go，在 VS Code 等大型代码库上实现了高达 11.9 倍的加速。 这一显著的性能提升使 TypeScript 在大型项目中更快，缩短了构建时间，提升了整个生态系统的开发者效率。 编译器用 Go 重写后，在真实代码库上实现了 8-12 倍的加速，微软的基准测试证明了这一点；Go 移植版完全兼容现有的 TypeScript 代码。

hackernews · DanRosenwasser · Jul 8, 16:06 · [社区讨论](https://news.ycombinator.com/item?id=48833715)

**背景**: TypeScript 是 JavaScript 的类型化超集，编译为纯 JavaScript。其原始编译器本身用 JavaScript/TypeScript 编写，成为大型代码库的性能瓶颈。Go 是一种编译型语言，以高性能和高效并发著称，非常适合构建高性能编译器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.architecture-weekly.com/p/typescript-migrates-to-go-whats-really">TypeScript Migrates to Go: What's Really Behind That 10x Performance Claim?</a></li>
<li><a href="https://visualstudiomagazine.com/articles/2025/03/11/microsoft-ports-typescript-to-go-for-10x-native-performance-gains.aspx">Microsoft Ports TypeScript to Go for 10x Native Performance Gains -- Visual Studio Magazine</a></li>
<li><a href="https://www.reddit.com/r/ProgrammingLanguages/comments/1j9osva/typescript_compiler_is_being_ported_to_go/">r/ProgrammingLanguages on Reddit: TypeScript compiler is being ported to Go</a></li>

</ul>
</details>

**社区讨论**: 社区反应积极，用户发布了令人印象深刻的加速数据，并称赞团队同时维护两个代码库。有人猜测未来是否会再次用 Rust 重写，也有人对终于有了一个快速的 TypeScript 编译器表示欣慰。

**标签**: `#TypeScript`, `#performance`, `#compiler`, `#Microsoft`, `#software-engineering`

---

<a id="item-3"></a>
## [用 AI 智能体将 Bun 重写为 Rust](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 9.0/10

Bun 的创建者 Jarred Sumner 宣布将 JavaScript 运行时从 Zig 完全重写为 Rust，借助 AI 编码智能体和 TypeScript 一致性测试套件，在 11 天内完成。 这次重写表明，大规模、由智能体驱动的代码库重写现在已成为可能，可能改变软件工程项目处理基础语言迁移的方式。同时，它为 Rust 在系统级运行时开发领域赢得了重要胜利。 估计的 API 令牌成本为 16.5 万美元，但由于 Bun 属于 Anthropic，实际免费。Rust 版本在 Linux 上启动速度提高了 10%，稳定性改善，二进制文件大小减少了 20%。

rss · Simon Willison · Jul 8, 23:57

**背景**: Bun 是一个快速的全能 JavaScript 运行时和工具包，包含打包器、转译器和包管理器。它最初用 Zig 编写，Zig 是一种需要手动管理内存的低级系统语言。重写为 Rust 是因为存在持久的内存安全漏洞，如释放后使用和双重释放错误，而 Rust 的所有权模型可在编译时防止这些问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://bun.com/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，这次重写凸显了 Zig 在内存安全方面的不足，以及强大的测试套件对 LLM 驱动重写的重要性。一些人称赞了展示出的纪律性及人工监督，而另一些人对 16.5 万美元的成本比较提出质疑，指出这是由 Anthropic 补贴的。

**标签**: `#Bun`, `#Rust`, `#Zig`, `#JavaScript runtime`, `#systems engineering`

---

<a id="item-4"></a>
## [安卓全版本远程 Root 漏洞链曝光](https://www.coolapk.com/feed/72700258?s=ZGQ2MTVlZjYxMDYyNTM3ZzZhNGUzOThjega1640) ⭐️ 9.0/10

2026 年 7 月 8 日，网络安全公司 Nebula 披露了一套影响安卓 17 及所有旧版本的远程 Root 漏洞链，该链结合了 Firefox 浏览器（至 151.0.2 版本）的漏洞和一个潜伏 15 年的 Linux 内核缺陷（CVE-2026-43499，GhostLock）。 该漏洞链允许攻击者仅通过诱骗用户点击恶意链接即可获取任何安卓设备的持久 Root 权限，对全球数十亿设备构成前所未有的安全威胁。 概念验证代码已上传至 GitHub，完整细节暂未披露，该漏洞链结合了 Firefox 的同源策略绕过漏洞（CVE-2026-8971）和 GhostLock 内核缺陷（rt_mutex 中的释放后重用）。Linux 内核已完成修复，但安卓厂商仍需推出更新。

telegram · zaihuapd · Jul 8, 13:01

**背景**: 远程 Root 漏洞链使攻击者无需物理接触即可完全控制设备，通常通过组合多个漏洞实现。GhostLock（CVE-2026-43499）是 Linux 内核实时互斥体（rtmutex）子系统中的释放后重用漏洞，于 2011 年引入，2026 年 4 月修复。Firefox 漏洞（CVE-2026-8971）是 JAR 协议处理中的同源策略绕过，允许恶意网站执行任意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/15-year-old-ghostlock-flaw-enables-root.html">15-Year-Old GhostLock Flaw Enables Root and Container Escape on Most Linux Distros</a></li>
<li><a href="https://threat-modeling.com/cve-2026-43499-ghostlock-linux-kernel-root-container-escape/">CVE-2026-43499 "GhostLock": 15-Year-Old Linux Kernel Flaw Gives Local Users Root Access and Container Escape — Public PoC Released - Threat-Modeling.com</a></li>
<li><a href="https://cybersecuritynews.com/15-year-old-ghostlock-linux-kernel-vulnerability/">15-year-old GhostLock Linux Kernel Vulnerability Enables Privilege Escalation Attacks</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2026-8971/">CVE-2026-8971: Mozilla Firefox Auth Bypass Vulnerability</a></li>

</ul>
</details>

**标签**: `#Android`, `#vulnerability`, `#remote root`, `#Linux kernel`, `#Firefox`

---

<a id="item-5"></a>
## [约翰迪尔用户赢得维修权，FTC 和解](https://apnews.com/article/john-deere-right-to-repair-agriculture-equipment-cb7514ffedb95c130a976af661f2bc02) ⭐️ 8.0/10

约翰迪尔（John Deere）与美国联邦贸易委员会及五个州达成和解，同意允许农民和独立维修店自行维修设备，结束了多年的限制性做法。 这次和解是维修权运动的一大胜利，可能为其他制造商树立先例，并赋予消费者控制自己财产的权利。 根据和解协议，约翰迪尔必须在未来 10 年内向车主和独立维修店提供诊断工具、手册和软件更新，并支付 100 万美元的反垄断执法费用。

hackernews · djoldman · Jul 8, 23:37 · [社区讨论](https://news.ycombinator.com/item?id=48838876)

**背景**: 维修权运动倡导消费者有权自行维修所购产品，而无需被迫使用授权经销商。约翰迪尔曾因使用软件锁和专有工具阻止第三方维修而受到批评，尤其是在农业领域，设备停机成本高昂。

**社区讨论**: 评论者赞扬了 Louis Rossmann 的倡导，并指出和解的象征性意义，但也有人批评罚款相对于约翰迪尔的利润微不足道，而其他人则争论维修权作为基本自由而非谈判让步的本质。

**标签**: `#right-to-repair`, `#consumer rights`, `#antitrust`, `#John Deere`, `#legislation`

---

<a id="item-6"></a>
## [Mistral 推出 Robostral Navigate：无地图机器人导航](https://mistral.ai/news/robostral-navigate/) ⭐️ 8.0/10

Mistral AI 发布了 Robostral Navigate，一个 8B 参数的模型，使机器人仅凭单个 RGB 摄像头和自然语言指令就能在复杂环境中导航，在 R2R-CE 基准上达到 76.6%。 这标志着无地图导航领域的重大进步，可能降低硬件成本，并使自主机器人在无需预先地图的室内环境中得到更广泛应用。 该模型无需激光雷达、深度传感器或多摄像头，仅依赖单个 RGB 摄像头进行视觉输入，且尚未对爱好者开放。

hackernews · ottomengis · Jul 8, 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48832212)

**背景**: 传统机器人导航通常需要预先获取的地图或多个深度传感器。无地图导航旨在让机器人仅凭视觉输入就能在陌生环境中遵循自然语言指令。“被绑架机器人问题”是指机器人失去定位后无法进行任何短距离导航。R2R-CE 是连续环境中视觉语言导航的标准基准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/robostral-navigate/">Robostral Navigate: single-camera AI navigation | Mistral AI</a></li>
<li><a href="https://www.siliconreport.com/mistral-ai-releases-robostral-navigate-a-single-camera-robotics-model-95dac18d">Mistral AI Releases Robostral Navigate, a Single-Camera ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论对无地图导航和爱好者项目的潜力表示热情，但指出该模型尚未公开发布。一些人将其与类似工作（如 PIGEON）比较，并讨论了高级任务（如物体操作）的挑战。

**标签**: `#robotics`, `#navigation`, `#AI`, `#machine learning`, `#Mistral`

---

<a id="item-7"></a>
## [xAI 发布 Grok 4.5，效率提升](https://x.ai/news/grok-4-5) ⭐️ 8.0/10

xAI 发布了 Grok 4.5，这是其 AI 模型的新版本，具有改进的推理效率和有竞争力的定价：输入每百万 token 2 美元，输出每百万 token 6 美元，模型使用数万亿个来自 Cursor 的数据 token 进行训练。 此次发布使 Grok 成为 GPT-5.4 和 Opus 4.8 等模型的经济高效替代品，可能重塑 AI 定价格局，但关于 xAI 实践的持续伦理担忧可能限制企业采用。 据报道，Grok 4.5 在基准测试中表现达到 Opus 4.7 水平，但价格显著更低；然而，批评者质疑基准测试的可靠性，并指出模型使用专有的 Cursor 数据进行训练可能引发数据隐私问题。

hackernews · BoumTAC · Jul 8, 18:00 · [社区讨论](https://news.ycombinator.com/item?id=48835111)

**背景**: Grok 是由 Elon Musk 的 AI 公司 xAI 开发的一系列大型语言模型。这些模型与 X 平台集成，强调实时信息访问。xAI 一直因内容审核和政治偏见而受到审查，一些用户质疑其模型的可靠性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://guptadeepak.com/research/grok-ai-explained/">Grok AI Explained: xAI's Model Family, Capabilities, and ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/XAI_(company)">SpaceXAI - Wikipedia</a></li>
<li><a href="https://x.ai/company">Company: Accelerating Scientific Discovery | SpaceXAI</a></li>

</ul>
</details>

**社区讨论**: 评论意见分歧：一些人称赞 Grok 4.5 的成本效益和基准测试表现，而另一些人则因 xAI 被认为存在政治操纵和缺乏伦理保障而表示不信任。用户们还就 AI 军备竞赛的经济可行性展开辩论。

**标签**: `#AI`, `#Grok`, `#xAI`, `#machine learning`, `#ethics`

---

<a id="item-8"></a>
## [解码优衣库 T 恤上的混淆 Bash 脚本](https://tris.sherliker.net/blog/obfuscated-self-evaluating-bash-script-by-cdn-akamai-being-supplied-to-consumers-via-retail-stores/) ⭐️ 8.0/10

一篇博文解码了优衣库 T 恤上印制的混淆 Bash 脚本，该脚本由 Akamai 设计，旨在实现自求值。 这突显了现实世界中的混淆和逆向工程，将时尚与技术文化相结合，并引发了关于脚本可读性和 OCR 挑战的讨论。 该 T 恤使用了 Roboto Mono 字体但带有字距调整，增加了 OCR 难度；有评论者指出脚本存在语法错误，导致无法运行。

hackernews · speerer · Jul 8, 08:46 · [社区讨论](https://news.ycombinator.com/item?id=48829312)

**背景**: Bash 混淆通过编码、压缩、加密或自修改代码来隐藏脚本的真实意图。这款 T 恤是优衣库与 Akamai 合作系列的一部分，设计师分享了一段视频，解释制作过程，包括有意增加 OCR 难度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Bashfuscator/Bashfuscator">GitHub - Bashfuscator/Bashfuscator: A fully configurable and extendable Bash obfuscation framework. This tool is intended to help both red team and blue team. · GitHub</a></li>
<li><a href="https://www.baeldung.com/linux/bash-obfuscate-script">How to Obfuscate a Bash Script to Make It Unreadable | Baeldung on Linux</a></li>

</ul>
</details>

**社区讨论**: 社区评论包括因语法错误退回 T 恤的幽默、对 Martin Kleppe quine 时钟的提及，以及对设计师视频的赞扬。还有人指出 OCR 识别该 T 恤很困难，并猜测脚本是否由 LLM 生成。

**标签**: `#bash`, `#obfuscation`, `#reverse-engineering`, `#uniqlo`, `#hacker-news`

---

<a id="item-9"></a>
## [Cloudflare Meerkat：全球异步共识协议](https://blog.cloudflare.com/meerkat-introduction/) ⭐️ 8.0/10

Cloudflare 研究团队宣布推出 Meerkat，这是一个全球分布式共识服务，实现了 QuePaxa 异步共识算法，并计划构建一个强一致、容错的键值存储系统。 这是异步共识算法（QuePaxa）的首次生产部署，消除了对超时的依赖，即使在网络延迟严重的情况下也能保持进展，有望提升全球分布式系统的可靠性。 与基于领导者的协议（如 Raft）相比，Meerkat 是无领导者的，并采用 hedging 机制动态管理提议者。然而，读操作也需要全局共识，这可能为读密集型工作负载引入更高的延迟。

hackernews · bobnamob · Jul 8, 13:18 · [社区讨论](https://news.ycombinator.com/item?id=48831565)

**背景**: 大多数分布式共识协议（如 Paxos、Raft）是部分同步的，依赖超时来保证活跃性。像 QuePaxa 这样的异步共识算法不依赖超时，因此对网络延迟具有鲁棒性，但传统上因复杂性被认为不实用。Cloudflare 的 Meerkat 旨在证明异步共识可以在生产中高效运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.cloudflare.com/meerkat-introduction/">Introducing Meerkat- an experiment in global consensus</a></li>
<li><a href="https://bford.info/pub/os/quepaxa/quepaxa.pdf">QuePaxa: Escaping the Tyranny of Timeouts in Consensus QuePaxa: Escaping the Tyranny of Timeouts in Consensus QuePaxa: Escaping the Tyranny of Timeouts in Consensus Artifact Review Summary: QuePaxa: Escaping the tyranny of ... Post by @cloudflare.social — Bluesky</a></li>

</ul>
</details>

**社区讨论**: 评论指出，Meerkat 消除了超时问题，对复杂网络环境很有价值，但有人担心每次读操作都需要全局共识，限制了其在读密集型应用中的使用。其他人则赞赏这一创新以及异步共识的首次生产实现。

**标签**: `#distributed systems`, `#consensus algorithms`, `#Cloudflare`, `#QuePaxa`, `#asynchronous consensus`

---

<a id="item-10"></a>
## [阿里巴巴要求员工在 7 月 10 日前卸载 Claude](https://t.me/zaihuapd/42424) ⭐️ 8.0/10

阿里巴巴内部下令要求所有员工在 7 月 10 日前卸载 Anthropic 旗下的 Claude 产品，包括 Sonnet、Opus、Fable 等模型以及 Claude Code 代理工具。此前，Anthropic 指控阿里巴巴在 4 月 22 日至 6 月 5 日期间，使用约 2.5 万个虚假账号与 Claude 交互超过 2800 万次。 这一政策标志着企业 AI 治理的重大升级，反映了中美 AI 公司在安全和数据访问方面的紧张关系加剧。它可能影响其他大型企业对待外部 AI 工具的方式，并重塑企业 AI 市场的竞争格局。 禁令涵盖所有 Anthropic 相关产品，包括 Claude Sonnet、Opus、Fable 模型和 Claude Code 代理。阿里巴巴此前曾报销员工使用 Claude、GPT、Gemini 等外部模型的费用，但此次政策完全扭转了这种做法。

telegram · zaihuapd · Jul 8, 06:09

**背景**: Anthropic 是一家总部位于美国的人工智能安全公司，由前 OpenAI 员工创立，以其 Claude 系列大型语言模型而闻名。该公司提供多种 Claude 模型（Haiku、Sonnet、Opus、Fable）以及名为 Claude Code 的编码代理工具。阿里巴巴是一家中国跨国科技集团，一直在大举投资 AI，包括其自有模型如通义千问。虚假账号的指控凸显了跨境 AI 公司之间的竞争和安全紧张局势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/overview">Models overview - Claude Platform Docs</a></li>
<li><a href="https://www.anthropic.com/product/claude-code">Claude Code | Anthropic's agentic coding system</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#enterprise AI`, `#Alibaba`, `#Anthropic`, `#Claude`

---

<a id="item-11"></a>
## [华为 5G 旗舰重返海外，峰值速度突破 1100 Mbps](https://finance.sina.com.cn/tech/roll/2026-07-08/doc-inihapna8035781.shtml) ⭐️ 8.0/10

华为 Pura 90 Pro Max 国际版目前已原生支持 5G 网络，海外实测峰值下载速率突破 1100 Mbps，标志着美国制裁七年后华为 5G 旗舰首次重返海外市场。 此次发布标志着华为成功突破美国技术封锁，通过重新引入强有力的竞争对手，可能重塑全球 5G 智能手机市场。同时也展示了华为 5A 通信技术在真实网络中的实际应用。 该设备运行 HarmonyOS 6.0.0.125，并搭载华为 5A 通信技术——一套终端侧增强技术，用于改善信号和速度。海外测试确认状态栏显示 5G 图标，验证了原生 5G 支持。

telegram · zaihuapd · Jul 8, 12:17

**背景**: 自 2019 年以来，美国制裁阻止华为使用美国供应商的 5G 芯片组，迫使其依赖自研麒麟芯片并推迟 5G 手机发布。2023 年，Mate 60 系列采用国产组件实现了 5G 能力，标志着一项突破。5A 并非 5G 本身，而是一套 AI 驱动的通信技术套件，用于优化网络连接，包括快速接入、低延迟和广覆盖，正如华为所解释的那样。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.biggo.com/news/202602182022_Huawei_5A_Technology_Explained">Huawei's "5A" Explained: Not 5G, But a Smarter Way to Connect — BigGo Finance</a></li>
<li><a href="https://www.huaweicentral.com/huawei-introduces-5a-network-to-this-entry-level-smartphone/">Huawei introduces 5A network to this entry-level smartphone - Huawei Central</a></li>

</ul>
</details>

**标签**: `#Huawei`, `#5G`, `#smartphones`, `#telecommunications`, `#sanctions`

---

<a id="item-12"></a>
## [美团 OWL 模型在 OpenRouter 测试中疑似会话数据泄露](https://github.com/gumusserv/ProducerBenchV2/blob/83cad6007ef3fe8df33386e8f43738fe62337e16/parsed_source_data/data/) ⭐️ 8.0/10

小红书截图显示，美团在 OpenRouter 上公开测试的免费模型 OWL（LongCat）疑似发生对话数据泄露，相关数据曾出现在 GitHub 仓库中，该仓库目前已无法公开访问。 此事件凸显了使用大语言模型处理敏感任务时的隐私风险，用户会话日志已成为新的敏感数据资产；同时也引发了业界对数据处置实践的关注。 该 GitHub 仓库至少在 2026 年 7 月 7 日之前公开可见，随后被 Discord 机器人 token 扫描器发现并重置了暴露的令牌；类似泄露事件也曾发生在 Google 和 DeepSeek 等模型上。

telegram · zaihuapd · Jul 8, 13:35

**背景**: OpenRouter 是一个统一 API，提供对 400 多个 AI 模型的访问，包括美团基于国产芯片训练的 1.6 万亿参数混合专家模型 LongCat-2.0（此前以“Owl Alpha”匿名身份在 OpenRouter 上领先基准测试）。Discord 机器人 token 扫描器是一种自动检测并撤销公开仓库中暴露的 API 令牌的工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.codecademy.com/article/what-is-openrouter">What is OpenRouter? A Guide with Practical Examples</a></li>
<li><a href="https://venturebeat.com/technology/meituan-open-sources-longcat-2-0-the-1-6t-near-frontier-agentic-coding-model-thats-been-leading-openrouter-trained-entirely-on-chinese-chips">Meituan open sources LongCat-2.0, the 1.6T, near-frontier agentic coding model that's been leading OpenRouter — trained entirely on Chinese chips | VentureBeat</a></li>
<li><a href="https://top.gg/bot/842154960397008896">Add Token Scanner Discord Bot | The #1 Discord Bot and ...</a></li>

</ul>
</details>

**社区讨论**: 小红书用户广泛转发泄露截图，警告他人不要在 AI 模型中输入 API 密钥、源代码等敏感信息，并讨论了对基于智能体的系统数据隐私的更广泛影响。

**标签**: `#大模型安全`, `#数据泄露`, `#隐私`, `#美团`, `#OWL`

---

<a id="item-13"></a>
## [研究团队通过电磁泄漏识别手机应用，准确率 99%](https://www.scmp.com/news/china/science/article/3359688/chinese-researchers-find-peephole-any-smartphone-its-leaked-radio-signal) ⭐️ 8.0/10

研究人员开发了一种非接触式取证技术，通过分析手机运行时泄漏的低频电磁信号来识别正在使用的应用及部分操作，在 iPhone 15 Pro、小米 15 Pro 和 OPPO Reno 13 上对抖音、微信视频通话等应用的识别准确率最高达 99.07%。 这种侧信道攻击揭示了一个重大的隐私漏洞，因为它在离线、飞行模式、加密或锁定状态下仍能工作，攻击者无需物理接触或入侵系统即可监视用户活动。 该技术利用智能手机处理器及其他组件在执行应用时无意泄漏的电磁辐射，且无需预先访问设备的操作系统或存储数据。

telegram · zaihuapd · Jul 8, 16:05

**背景**: 电磁侧信道攻击通过测量电子设备运行时发出的电磁辐射来泄露内部状态信息。过去的研究表明，功耗或电磁信号有时能揭示正在运行的应用，但针对现代智能手机的高精度非接触式攻击一直受限。这项研究展示了一种低频电磁攻击，它属于被动攻击，且无需对目标设备进行任何硬件改造。

**标签**: `#security`, `#electromagnetic signal`, `#side-channel attack`, `#mobile privacy`

---

<a id="item-14"></a>
## [LineageOS 推出网页刷机工具](https://www.androidauthority.com/lineageos-summertime-update-2026-3685112/) ⭐️ 8.0/10

LineageOS 在 2026 年夏季更新中推出了网页刷机工具 Lineage Flash Tools，用户可直接在浏览器中刷机，无需本地安装 ADB 和 Fastboot。 该工具大幅降低了用户安装自定义 ROM 的门槛，使刷机过程更简单且不易出错，有助于扩大自定义 ROM 社区。 该工具支持 Fastboot、ADB 和三星 Odin 协议，需要使用支持 WebUSB 的浏览器（如 Chrome 或 Edge），并且必须配合设备专属 Wiki 安装指南使用，不能完全替代传统刷机流程。

telegram · zaihuapd · Jul 9, 01:46

**背景**: WebUSB 是一种 JavaScript API，允许网页应用安全地与 USB 设备通信，从而实现基于浏览器的刷机。Odin 协议用于三星设备。此外，LineageOS 在 Updater 应用中引入了 Material 3 Expressive 界面，并确认基于 Android 17 的 LineageOS 24 已进入开发阶段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebUSB">WebUSB - Wikipedia</a></li>
<li><a href="https://source.android.com/docs/core/ota/ab">A/B (seamless) system updates | Android Open Source Project</a></li>

</ul>
</details>

**标签**: `#LineageOS`, `#custom ROM`, `#web flashing`, `#Android`, `#WebUSB`

---