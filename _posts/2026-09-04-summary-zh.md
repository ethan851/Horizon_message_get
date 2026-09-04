---
layout: default
title: "Horizon Summary: 2026-09-04 (ZH)"
date: 2026-09-04
lang: zh
---

> From 29 items, 8 important content pieces were selected

---

1. [OpenAI 发布 GPT-6 Astra，ARC-AGI-3 得分 99.9%](#item-1) ⭐️ 9.5/10
2. [OpenAI 推出 GPT-6 Astra，ARC-AGI-3 得分 99.9%](#item-2) ⭐️ 9.0/10
3. [OpenAI 发布 Astra：首个达到“临界”网络安全阈值的模型](#item-3) ⭐️ 9.0/10
4. [用能读懂 68000 汇编的 LLM 将 1993 年 Amiga 游戏移植到 Godot](#item-4) ⭐️ 8.0/10
5. [Audacity 4.0 发布：采用 Qt6 界面，引发社区热议](#item-5) ⭐️ 8.0/10
6. [GPT-6 Astra 仅解少量 ARC-AGI-3 任务，引发成本与智能之争](#item-6) ⭐️ 8.0/10
7. [Google Antigravity 服务条款模糊引发 Google 账号停用担忧](#item-7) ⭐️ 8.0/10
8. [韩国公布 800 万亿韩元半导体集群计划，新建 4 座 DRAM 晶圆厂](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 发布 GPT-6 Astra，ARC-AGI-3 得分 99.9%](https://openai.com/index/gpt-6-astra/) ⭐️ 9.5/10

OpenAI 发布了 GPT-6 Astra，声称在交互式 ARC-AGI-3 基准上取得 99.9% 的成绩，并在 Artificial Analysis Coding Agent Index 上取得重大进展。相关 Hacker News 讨论显示该模型已开始逐步推出。 这是一次重大的前沿模型发布，重新引发了关于基准成绩是否意味着 AGI 级别的推理、还是仅仅代表技能习得的争论。讨论的规模和怀疑态度反映了 AI 社区如何看待基准声明。 ARC-AGI-3 是交互式基准，因此评测 harness 影响很大：有评论者指出，如果使用与 GPT-6 Astra 相同的 responses API harness，GPT-5.6 Sol 的得分约为 30%，而非显示的 7.8%。一些评论者也认为其他基准的提升相对温和。

hackernews · kibae · Sep 3, 18:41 · [社区讨论](https://news.ycombinator.com/item?id=49554643)

**背景**: ARC-AGI-3 是首个面向 AI 智能体的交互式推理基准，要求智能体在陌生回合制环境中探索、推断目标并规划行动，且没有明确指令；人类得分接近 100%，而 AI 系统此前得分很低。Artificial Analysis Coding Agent Index 是一个综合分数，通过仓库任务、终端工作流和基于规则的评估来衡量编程智能体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://artificialanalysis.ai/agents/coding-agents">AI Coding Agent Benchmarks & Leaderboard | Artificial Analysis</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者对 ARC-AGI-3 记分卡表示怀疑，认为由于与以前模型在 harness 上的不一致而具有误导性。一些人认为进展更像是技能习得，呼应了 François Chollet 的《论智能的度量》，并质疑自主购物演示的实用性。

**标签**: `#AI`, `#OpenAI`, `#GPT-6`, `#benchmarks`, `#machine learning`

---

<a id="item-2"></a>
## [OpenAI 推出 GPT-6 Astra，ARC-AGI-3 得分 99.9%](https://simonwillison.net/2026/Sep/3/gpt6-astra/) ⭐️ 9.0/10

OpenAI 发布了 GPT-6 Astra，今天起向部分机构开放，未来几天将向所有 ChatGPT Plus、Pro、Business 和 Enterprise 用户以及 OpenAI API 和 AWS 用户推出。其 API 定价为每百万输入 token 10 美元、每百万输出 token 50 美元，与 Claude Fable 5 持平。 GPT-6 Astra 是 OpenAI 对标 Claude Fable 5 的重要产品，在大多数自报基准上得分更高且定价相同。其 99.9% 的 ARC-AGI-3 得分以及出色的安全性与长上下文表现，标志着智能体推理方面的重大进步，可能重塑 AI 模型竞争格局。 99.9% 的 ARC-AGI-3 成绩是在 OpenAI 自定义的 Provider Adapter 测试台上取得的，该测试台会在多次请求之间保留不透明的推理状态；而默认 ARC-AGI-3 测试台的得分仅为 62.7%。尽管在许多方面表现优异，Astra 在 Artificial Analysis 的 Intelligence Index 上仍落后于 Claude Fable 5.1，得分 61 对 66。

rss · Simon Willison · Sep 3, 20:18

**背景**: ARC-AGI-3 是一个交互式推理基准，要求 AI 智能体探索新环境、推断目标并构建环境动态的内部模型；人类在该基准上可达 100%，而 AI 的得分普遍很低。OpenAI 的 Provider Adapter 测试台采用压缩等技术处理较长对话，使模型能在多次请求之间复用之前的工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">[2603.24621] ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-arc-agi-3-interactive-benchmark">What Is ARC AGI 3? The Interactive AI Benchmark Humans Solve at 100% | MindStudio</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#GPT-6`, `#AI models`, `#benchmarks`, `#LLM`

---

<a id="item-3"></a>
## [OpenAI 发布 Astra：首个达到“临界”网络安全阈值的模型](https://t.me/zaihuapd/43592) ⭐️ 9.0/10

OpenAI 宣布将发布 Astra，这是其首个在网络安全领域超越“临界”阈值（Preparedness Framework）的模型。该模型能自主发现并利用防护严密系统中的未知漏洞，在 ExploitBench 上获得 100%满分，并在内部测试中发现两个零日漏洞。 这是 AI 安全领域的一个重要里程碑，因为这是 OpenAI 首个被正式认定为达到“临界”网络能力的模型，表明前沿 AI 既能强化安全运营，也可能带来新的安全威胁。这可能会加剧业界关于安全部署、监管以及如何衡量 AI 智能体攻击能力的广泛讨论。 为降低风险，OpenAI 推迟了部分开发与发布工作并加强了防护措施。Astra 对网络越狱请求的拒绝率从 GPT-5.6 Sol 的 59%提升至 91.5%，其高级网络能力初期仅向少数测试者开放。

telegram · zaihuapd · Sep 3, 18:47

**背景**: 根据 OpenAI 的 Preparedness Framework（预备框架），如果模型能够在无需人工干预的情况下，在许多加固的真实世界关键系统中识别并开发出可用的零日漏洞，则该模型达到“临界”网络安全阈值。ExploitBench 是由卡内基梅隆大学研究人员创建的基准测试，用于衡量 AI 智能体从接触脆弱代码到触发漏洞、构建利用原语，直至实现任意代码执行的进展程度。OpenAI 的这一判断基于该基准和内部评估，包括实时发现零日漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/responding-next-frontier-critical-cyber-capabilities/">Responding to the next frontier of critical cyber capabilities</a></li>
<li><a href="https://www.cnbc.com/2026/09/01/open-ai-astra-cyber-model.html">OpenAI says Astra AI model crosses 'Critical' cyber capability</a></li>
<li><a href="https://www.explainx.ai/blog/openai-astra-cybersecurity-critical-preparedness-framework-2026">OpenAI Astra: Critical Cyber Tier Confirmed (Sept 2026 ...</a></li>

</ul>
</details>

**标签**: `#AI security`, `#OpenAI`, `#cybersecurity`, `#alignment`, `#Astra`

---

<a id="item-4"></a>
## [用能读懂 68000 汇编的 LLM 将 1993 年 Amiga 游戏移植到 Godot](https://babyloniantwins.com/blog/porting-a-1993-amiga-game-to-godot/) ⭐️ 8.0/10

一位开发者利用 LLM 将他在 1993 年用 MC68000 汇编编写的 Amiga 游戏移植到 Godot 引擎，整个移植只花了一个晚上。这一过程产出了与原二进制文件逐字节一致的重汇编结果和可玩的 Godot 移植版，原版游戏也已免费发布。 这展示了一种将遗留的 68000 汇编代码转换到现代游戏引擎的全新工作流程，大幅降低了复古游戏移植所需的工作量。它可能激励开发者和游戏保护工作者把更多经典汇编语言游戏带到现代平台上。 开发者让模型在 macOS 上用 vasm 汇编代码，并持续迭代直到输出结果与原发布二进制文件逐字节一致，但存在约 108 字节的差异。这个差异源于原游戏是用 AsmOne 汇编到内存中，并把运行中内存的快照保存到磁盘，而不是保存干净的汇编器输出。

hackernews · rabahs · Sep 3, 14:28 · [社区讨论](https://news.ycombinator.com/item?id=49550375)

**背景**: Amiga 是 1980 年代至 1990 年代初流行的个人电脑，许多游戏为了速度和直接访问硬件而使用 Motorola 68000（68k）汇编语言编写。AsmOne 是当时流行的 Amiga 汇编器和 IDE，它在内存中完成汇编，开发者常把内存快照保存为最终游戏文件。vasm 是如今常用的可移植、可重定向汇编器，常用于汇编 68000 等平台的代码。在这次移植中，开发者用 LLM 将 68000 汇编逻辑及相关素材转换到 Godot 这一现代开源游戏引擎中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Motorola_68000">Motorola 68000 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amiga_programming_languages">Amiga programming languages - Wikipedia</a></li>
<li><a href="http://www.compilers.de/vasm.html">Dr. Volker Barthelmann´s Compiler Page</a></li>

</ul>
</details>

**社区讨论**: 评论者们既惊叹又怀旧，称赞作者在 1993 年用 68k 汇编完整编写了一款游戏。不少人用自己类似的实验佐证了这一方法，例如用 LLM 将 ZX81 内存转储移植到 Go，或为 68k 搭建主机移植框架；还有人询问当年游戏的灵感来源和调试故事。

**标签**: `#LLM`, `#retrocomputing`, `#game development`, `#Godot`, `#reverse engineering`

---

<a id="item-5"></a>
## [Audacity 4.0 发布：采用 Qt6 界面，引发社区热议](https://github.com/audacity/audacity/releases/tag/Audacity-4.0.0) ⭐️ 8.0/10

广泛使用的开源音频编辑器 Audacity 4.0 现已发布，带来了基于 Qt6 的用户界面重构，并包含多项修复。这是多年来的首个大版本升级，发布后迅速引发了关于项目技术方向的激烈社区讨论。 Audacity 是最受欢迎的开源音频工具之一，因此这样一次大规模界面更新与修复会影响包括播客制作者、音乐人和教育工作者在内的数百万用户。该版本还重新引发了关于项目治理、遥测历史以及信任问题的讨论，这些问题可能影响用户的采用意愿。 新的 Qt6 界面取代了旧版 GUI 工具包；有测试用户反馈界面更简洁，并修复了项目有时无法保存、片段之间出现“咔哒”噪音等长期不便。然而，一些 Linux 用户仍抱怨 JACK/PipeWire 集成不够持久，且他们期望的工作流改进仍未出现。

hackernews · ClydeN · Sep 3, 10:53 · [社区讨论](https://news.ycombinator.com/item?id=49548395)

**背景**: Audacity 是一款免费开源的音频编辑器，常用于录制和编辑播客与音乐。2021 年，该项目被 Muse Group 收购，随后计划加入遥测和云端功能，引发了社区强烈反应，并催生了 Tenacity、Sneedacity 等分支。Qt6 是跨平台 GUI 框架 Qt 的最新大版本，Audacity 4.0 现已采用该框架。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qt_(software)">Qt (software) - Wikipedia</a></li>
<li><a href="https://arstechnica.com/gadgets/2021/07/no-open-source-audacity-audio-editor-is-not-spyware/">No, open source Audacity audio editor is not “spyware” - Ars Technica</a></li>
<li><a href="https://cloud.smartsound.com/blog/the-uproar-at-audacity-and-its-alternatives/">The uproar at Audacity (and its alternatives) - Smartsound Cloud</a></li>

</ul>
</details>

**社区讨论**: 评论区意见不一：一些人称赞界面更简洁并修复了期待已久的 bug；另一些人则持怀疑态度，因为更新日志似乎并未解决 Linux 上长期存在的音频工作流问题。还有几位用户追问，在遥测风波之后出现的 Tenacity、Sneedacity 等分支是否仍有意义。

**标签**: `#Audacity`, `#audio-editing`, `#open-source`, `#release`, `#UI`

---

<a id="item-6"></a>
## [GPT-6 Astra 仅解少量 ARC-AGI-3 任务，引发成本与智能之争](https://arcprize.org/blog/astra) ⭐️ 8.0/10

OpenAI 的旗舰模型 GPT-6 Astra 在测试中解决了少量 ARC-AGI-3 任务，但每次求解都消耗了大量算力，整体解决率仍然很低。该结果表明，当前前沿模型虽能在 ARC-AGI-3 上取得部分进展，但仍远不及人类——据报道人类几乎能解出该基准中的全部任务。 ARC-AGI-3 旨在衡量流体性、适应性智能，而这正是 AI 仍显薄弱的领域，因此这些结果会影响业界如何评估迈向通用人工智能的进展。每解决一个问题所需的高昂计算成本，也引发了关于此类基准能否在高难度推理工作中具备经济实用性的疑问。 在最新的 ARC-AGI-3 评估中，前沿 AI 模型的解决率据称不足 1%，而绝大多数人类可以完成全部任务。评论区提到，最强模型每道题的成本约为 218–360 美元，并消耗数小时算力；还有人认为，若当前改进趋势持续，其性价比可能在两年内接近人类最低工资水平。

hackernews · vignesh_warar · Sep 3, 19:45 · [社区讨论](https://news.ycombinator.com/item?id=49555691)

**背景**: ARC-AGI（抽象与推理语料库）基准旨在测试 AI 能否适应全新情境，而非依赖记忆过的模式。ARC-AGI-3 将该格式升级为交互式回合制环境，要求智能体通过探索来推断目标、建立内部环境模型并规划行动序列，且没有明确说明规则。GPT-6 Astra 是 OpenAI 面向复杂推理、编码、研究和智能体工作负载推出的旗舰模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence OpenAI's GPT-6 Astra on ARC-AGI-3 | ARC Prize ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence ARC-AGI-3: The New Interactive Reasoning Benchmark ARC-AGI-3 Leaderboard - llm-stats.com</a></li>
<li><a href="https://openai.com/index/gpt-6-astra/">GPT - 6 Astra : A new generation of intelligence | OpenAI</a></li>

</ul>
</details>

**社区讨论**: 评论区普遍持怀疑态度：有人质疑“用最少步数解开蛇形谜题是否真的定义智能”；也有人指出成本下降趋势可能让 AI 在两年内比最低工资的人类解题者更便宜。还有人担心 OpenAI 可能事先拿到任务集，并通过监督式强化学习针对具体题目过拟合，从而削弱该结果的意义。

**标签**: `#AI`, `#OpenAI`, `#ARC-AGI-3`, `#benchmark`, `#GPT-6`

---

<a id="item-7"></a>
## [Google Antigravity 服务条款模糊引发 Google 账号停用担忧](https://twitter.com/GergelyOrosz/status/2095453567955968398) ⭐️ 8.0/10

Google Antigravity 的服务条款包含一项条款：使用第三方软件、工具或服务（例如将 OpenClaw 与 Antigravity OAuth 搭配使用）访问该服务，可能导致“您的账户”被暂停或终止。Antigravity 团队成员 Varun Mohan 澄清，该条款指的是 Antigravity 账户，而非用户的完整 Google 账户，并表示将更新措辞以使含义更明确。 这一模糊措辞之所以重要，是因为许多用户的一个 Google 账号关联着邮件、日历、通讯录及其他关键服务；因 AI 工具使用政策而触发的问题可能让他们失去的不只是该 AI 产品。这也会削弱开发者对 Google AI 产品的信任，尤其是那些认为被封的 Google 账号没有可靠申诉渠道的用户。 引发争议的条款原文为：“使用非我们提供的第三方软件、工具或服务访问本服务（例如使用带 Antigravity OAuth 的 OpenClaw）即违反本协议。此类行为可能导致您的账户被暂停或终止。”Varun Mohan 已在 X 上公开发布澄清，链接为 https://x.com/_mohansolo/status/2095529407033000260。

hackernews · tosh · Sep 3, 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49548452)

**背景**: Google Antigravity 是 Google 提供的一项服务，其服务条款将 Google 通用条款、Google Antigravity 条款和隐私政策合并为具有约束力的协议。条款明确禁止通过第三方软件或 OAuth 流程访问 Antigravity，并可能因此暂停或终止账户。实际操作中，使用 Antigravity 需要登录 Google 账号，因此许多用户将“your account”理解为其整个 Google 账号，而不只是 Antigravity 产品账号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://antigravity.google/terms">Google Antigravity - Terms of Service</a></li>
<li><a href="https://support.google.com/accounts/thread/411322798/appeal-for-antigravity-access-suspension?hl=en">Appeal for Antigravity Access Suspension - Google Account ...</a></li>
<li><a href="https://discuss.ai.google.dev/tag/tos/448">Topics tagged tos | Google AI Developers Forum</a></li>

</ul>
</details>

**社区讨论**: 用户评论普遍担忧，若欧洲 eIDAS 等政府系统强制要求使用 Google/Apple 账号，那么 Google 账号被封可能导致用户无法使用在线政府服务；同时，评论批评对整个账号而非仅 AI 访问权限进行封禁是对用户极不友好的做法，因为账号里往往保存多年的邮件和日历。还有评论者表示，担心 AI 分类器误判且没有可靠恢复渠道，因此不愿使用 Google AI 产品。另一位评论者引用了 Varun Mohan 的澄清，称该措辞仅指 Antigravity 账号，并会进行修改。

**标签**: `#Google`, `#Terms of Service`, `#AI`, `#Account Ban`, `#Policy`

---

<a id="item-8"></a>
## [韩国公布 800 万亿韩元半导体集群计划，新建 4 座 DRAM 晶圆厂](https://t.me/zaihuapd/43585) ⭐️ 8.0/10

韩国产业通商部长官金正宽当天公布了半导体全国集群计划，拟吸引企业投资 800 万亿韩元（约 3.52 万亿元人民币），建设 4 座 DRAM 内存晶圆厂，并在西南圈打造第二个半导体生产基地。 这一大规模投资彰显了韩国在全球内存市场保持领先地位的决心，而全球内存市场预计未来五年将增长四倍以上。该计划将影响全球 DRAM 供应、价格以及半导体产业的竞争格局。 韩国政府还将在未来 15 年内追加投入 30 万亿韩元（约 1321.2 亿元人民币）支持该计划。重点在于内存芯片（尤其是 DRAM），计划在西南圈新建 4 座晶圆厂，以补充现有的半导体设施。

telegram · zaihuapd · Sep 3, 12:01

**背景**: DRAM（动态随机存取存储器）是一种半导体存储器，每个比特的数据存储在一个电容和一个晶体管中，广泛应用于计算机、显卡和便携式设备。半导体晶圆厂（fab）是制造集成电路的工厂，建设一座现代晶圆厂可能耗资数十亿美元，例如台积电为一座 2nm 晶圆厂投资超过 450 亿美元。韩国是三星和 SK 海力士的所在地，在全球内存芯片领域处于领先地位，因此这一国家集群计划是在人工智能相关内存需求激增背景下保持优势的战略举措。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dynamic_random-access_memory">Dynamic random-access memory - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Semiconductor_fabrication_plant">Semiconductor fabrication plant</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#DRAM`, `#South Korea`, `#industry policy`, `#investment`

---