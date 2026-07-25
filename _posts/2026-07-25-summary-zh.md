---
layout: default
title: "Horizon Summary: 2026-07-25 (ZH)"
date: 2026-07-25
lang: zh
---

> From 31 items, 14 important content pieces were selected

---

1. [Anthropic 发布 Claude Opus 5，新一代前沿 AI 模型](#item-1) ⭐️ 10.0/10
2. [SGLang v0.5.16: 引入 DSpark 推测解码和 975B Inkling 模型支持](#item-2) ⭐️ 9.0/10
3. [安全摄像头在登录页面嵌入了 GitHub 管理员令牌](#item-3) ⭐️ 9.0/10
4. [伊朗革命卫队声称摧毁亚马逊巴林数据中心](#item-4) ⭐️ 9.0/10
5. [两位中国数学家获 2026 年菲尔兹奖](#item-5) ⭐️ 9.0/10
6. [Postgres LISTEN/NOTIFY 确实可扩展](#item-6) ⭐️ 8.0/10
7. [编码进步了，为什么软件却越来越烂？](#item-7) ⭐️ 8.0/10
8. [科技巨头警告勿过度监管开放权重 AI](#item-8) ⭐️ 8.0/10
9. [印度要求 GitHub 移除 Bitchat 应用，称其存在安全隐患](#item-9) ⭐️ 8.0/10
10. [Buz – 使用现代 Zig 的 Bun 分支，增量构建低于 1 秒](#item-10) ⭐️ 8.0/10
11. [Claude Opus 5：最不易受提示注入影响的模型](#item-11) ⭐️ 8.0/10
12. [长鑫存储 2026 年 DRAM 产能或逼近美光](#item-12) ⭐️ 8.0/10
13. [OpenAI 发布企业 AI 智能体平台 Presence，软件股重挫](#item-13) ⭐️ 8.0/10
14. [黄仁勋：美国应允许使用中国开源 AI 模型](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic 发布 Claude Opus 5，新一代前沿 AI 模型](https://www.anthropic.com/news/claude-opus-5) ⭐️ 10.0/10

Anthropic 宣布推出 Claude Opus 5，这是一款新的旗舰 AI 模型，在基准测试中表现强劲，且对一般访问没有数据保留要求。 这一发布之所以重要，是因为 Opus 5 提供了前沿能力，却没有像 Fable 等竞品的 30 天数据保留政策，使其对数据隐私要求严格的组织具有吸引力。其强劲性能可能改变领先 AI 实验室之间的竞争格局。 根据社区测试，Opus 5 在图片到 HTML 转换方面比 Fable 更准确，其写作风格保留了与上代 Opus 4.8 相似的 'Claude 语言习惯'，一些用户认为这很有特色。

hackernews · alvis · Jul 24, 16:57 · [社区讨论](https://news.ycombinator.com/item?id=49038433)

**背景**: Claude Opus 模型是 Anthropic 功能最强、价格最贵的层级。Opus 5 延续了这一系列，改进了推理和视觉能力。系统卡是一份部署前的安全披露文件，详细说明了评估和风险阈值。与一些竞争对手不同，Anthropic 不要求对 Opus 模型的一般访问进行 30 天数据保留，从而解决了隐私问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>
<li><a href="https://techjacksolutions.com/ai-tools/anthropic-claude/claude-opus-5-system-card/">Claude Opus 5 System Card, Explained: 6 Safety Findings in ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调 Opus 5 没有数据保留要求的重要性，用户指出组织现在可以在不牺牲隐私的情况下访问前沿 AI。一些用户报告实际测试显示 Opus 5 在图片转 HTML 任务上优于 Fable，并保留了 Claude 特有的写作风格。

**标签**: `#AI`, `#LLM`, `#Claude`, `#Anthropic`, `#frontier models`

---

<a id="item-2"></a>
## [SGLang v0.5.16: 引入 DSpark 推测解码和 975B Inkling 模型支持](https://github.com/sgl-project/sglang/releases/tag/v0.5.16) ⭐️ 9.0/10

SGLang v0.5.16 引入了基于置信度的推测解码算法 DSpark，最高可达 383.7 tok/s，并增加了对 975B 参数多模态专家混合模型 Inkling 的支持。 这些创新显著提升了大型语言模型的推理吞吐量，并支持部署极大的开源权重多模态模型，推动了高效 LLM 服务的边界。 DSpark 以块为单位进行半自回归草拟，并根据置信度调整验证窗口大小；Inkling 结合了滑动窗口注意力、全注意力、Mamba2 线性注意力和 NVFP4 MoE，支持 100 万 token 的上下文。

github · Qiaolin-Yu · Jul 25, 00:13

**背景**: 推测解码通过使用较小的草稿模型生成候选 token，然后由目标模型并行验证，从而加速 LLM 推理。DSpark 通过自适应调整验证窗口大小来优化此过程。像 Inkling 这样的专家混合模型每个 token 只激活部分参数，从而在较低计算成本下实现更大的总参数量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/dspark">DSpark : Speculative Decoding</a></li>
<li><a href="https://models.dev/models/thinkingmachines/inkling/">Inkling pricing, providers, and specs | Models .dev</a></li>

</ul>
</details>

**标签**: `#speculative decoding`, `#LLM inference`, `#large language models`, `#sglang`

---

<a id="item-3"></a>
## [安全摄像头在登录页面嵌入了 GitHub 管理员令牌](https://hhh.hn/hanwha-github-token/) ⭐️ 9.0/10

一款韩华（Hanwha）安全摄像头被发现其登录页面中硬编码了一个 GitHub 个人访问令牌，该令牌具有公司 GitHub 仓库的管理员权限。 这暴露了一个严重的供应链漏洞，攻击者可能利用该令牌向摄像头固件注入恶意代码或窃取敏感数据，影响所有使用该固件的设备。 该令牌嵌入在登录页面的 HTML 源代码中，并可访问多个仓库，包括包含固件镜像和专有代码的仓库。

hackernews · hhh · Jul 24, 11:54 · [社区讨论](https://news.ycombinator.com/item?id=49034292)

**背景**: GitHub 个人访问令牌用于无需密码即可进行 API 和命令行操作的身份验证。一旦泄露，可能被利用来访问仓库。供应链安全涉及保护软件在开发和分发过程中免受漏洞侵害。在网页中硬编码秘密是一种基本的安全失误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens">Managing your personal access tokens - GitHub Docs</a></li>
<li><a href="https://www.darkreading.com/vulnerabilities-threats/rising-tide-of-software-supply-chain-attacks">The Rising Tide of Software Supply Chain Attacks</a></li>

</ul>
</details>

**社区讨论**: 评论者表示并不惊讶，指出许多物联网厂商优先考虑功能而非安全性。建议包括将摄像头隔离在单独的 VLAN 中且不提供互联网访问。一位评论者指出，固件中还嵌入了美国战争部的 IP 地址，表明存在更深层次的问题。

**标签**: `#security`, `#IoT`, `#vulnerability`, `#GitHub`, `#token`

---

<a id="item-4"></a>
## [伊朗革命卫队声称摧毁亚马逊巴林数据中心](https://houseofsaud.com/irgc-claims-destroyed-amazon-bahrain-data-center/) ⭐️ 9.0/10

伊朗伊斯兰革命卫队（IRGC）声称摧毁了亚马逊在巴林的数据中心，该数据中心托管着 AWS me-south-1 区域，导致整个区域离线。 此次事件标志着针对关键云基础设施的国家级攻击的重大升级，可能扰乱依赖 AWS 中东服务的众多组织，并凸显集中式云架构的脆弱性。 像 me-south-1 这样的 AWS 区域至少由三个相距数公里的数据中心组成，表明多个设施遭到攻击。社区分析确定了位于麦纳麦的特定数据中心建筑（BAH53 及其变电站）在 2026 年 7 月 16 日和 7 月 22 日遭到损坏或摧毁。

hackernews · thisislife2 · Jul 24, 09:52 · [社区讨论](https://news.ycombinator.com/item?id=49033240)

**背景**: AWS 区域是包含多个隔离可用区的地理区域，每个可用区有一个或多个数据中心。巴林的 me-south-1 区域是中东少数几个 AWS 区域之一，另外还有特拉维夫的区域和正在建设的沙特阿拉伯区域。此次攻击凸显了地缘政治冲突期间云基础设施面临的物理安全风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://health.aws.amazon.com/health/status?region=me-south-1">Service health - Jul 24, 2026 | AWS Health Dashboard | Global</a></li>
<li><a href="https://docs.aws.amazon.com/global-infrastructure/latest/regions/aws-regions.html">AWS Regions - AWS Regions and Availability Zones</a></li>
<li><a href="https://awsspeedtest.com/regions/me-south-1">Middle East (Bahrain) AWS Region | me-south-1</a></li>

</ul>
</details>

**社区讨论**: 评论指出，中东唯一仍在运营的 AWS 区域是特拉维夫的那个，这颇具讽刺意味。用户还强调了攻击的规模，指出要摧毁整个区域需要破坏多个地理上分离的数据中心，并与乌克兰战争中的类似打击进行了类比。

**标签**: `#AWS`, `#infrastructure`, `#geopolitics`, `#data center`, `#security`

---

<a id="item-5"></a>
## [两位中国数学家获 2026 年菲尔兹奖](https://t.me/zaihuapd/42748) ⭐️ 9.0/10

国际数学联盟公布了 2026 年菲尔兹奖得主，邓煜因偏微分方程方面的贡献获奖，John Pardon 因辛几何方面的成就获奖。这是首次有两位中国籍数学家同时获得菲尔兹奖。 菲尔兹奖是数学领域最高荣誉，两位中国获奖者标志着中国数学家在全球舞台上的影响力日益增强。他们在偏微分方程和辛几何方面的研究对数学物理和几何学有深远影响。 邓煜因从硬球动力学严格推导出玻尔兹曼方程，以及在非线性薛定谔动力学中的概率方法而获奖。John Pardon 因虚拟基本循环的新方法和辛几何中 Fukaya 范畴的贡献而获奖。

telegram · zaihuapd · Jul 24, 12:51

**背景**: 菲尔兹奖每四年颁发一次，授予 40 岁以下做出杰出贡献的数学家，以加拿大数学家约翰·查尔斯·菲尔兹命名。邓煜关于玻尔兹曼方程的工作连接了微观粒子动力学与宏观气体行为，而 Pardon 关于虚拟基本循环的工作是计数几何和辛拓扑中的关键工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Virtual_fundamental_class">Virtual fundamental class - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fukaya_category">Fukaya category</a></li>
<li><a href="https://annals.math.princeton.edu/articles/22284">Long time derivation of the Boltzmann equation from hard sphere dyamics | Annals of Mathematics</a></li>

</ul>
</details>

**标签**: `#Fields Medal`, `#Mathematics`, `#Chinese Mathematicians`, `#PDE`, `#Symplectic Geometry`

---

<a id="item-6"></a>
## [Postgres LISTEN/NOTIFY 确实可扩展](https://www.dbos.dev/blog/postgres-listen-notify-scalability) ⭐️ 8.0/10

DBOS 的一篇博客文章证明，PostgreSQL 的 LISTEN/NOTIFY 机制每秒可处理多达 60,000 条通知，驳斥了其不可扩展的传言。 这一发现对需要轻量级、与数据库集成的消息传递（无需额外基础设施）的 PostgreSQL 从业者意义重大，因为它表明 LISTEN/NOTIFY 可以处理许多应用所需的高吞吐场景。 该博客文章提供了具体的性能基准测试和实际用例，例如使用 DBOS 在 LISTEN/NOTIFY 之上构建持久工作流。它还引用了一篇早期的批评文章并纠正了可扩展性问题。

hackernews · KraftyOne · Jul 24, 19:05 · [社区讨论](https://news.ycombinator.com/item?id=49040296)

**背景**: PostgreSQL 的 LISTEN 和 NOTIFY 命令实现了同一数据库内的异步进程间通信。客户端会话使用 LISTEN 订阅指定通道，任何会话可通过 NOTIFY 向所有监听者发送通知。这一机制常用于实时更新、缓存失效和简单协调，但一些开发者曾认为其每秒通知数无法超过几千条。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/sql-notify.html">PostgreSQL: Documentation: 18: NOTIFY</a></li>
<li><a href="https://www.postgresql.org/docs/current/sql-listen.html">PostgreSQL: Documentation: 18: LISTEN</a></li>
<li><a href="https://oneuptime.com/blog/post/2026-01-25-use-listen-notify-real-time-postgresql/view">How to Use Listen/Notify for Real-Time Updates in PostgreSQL</a></li>

</ul>
</details>

**社区讨论**: 评论指出可扩展性是一个连续谱：60K/秒对某些系统可能过多，对另一些则不足。一位评论者提到他们基于 LISTEN/NOTIFY 构建了队列以利用强一致性，另一位指出早期版本中的性能问题自那以后已得到修复。

**标签**: `#PostgreSQL`, `#database`, `#scalability`, `#messaging`

---

<a id="item-7"></a>
## [编码进步了，为什么软件却越来越烂？](https://ptrchm.com/posts/nothing-works-and-everyone-is-euphoric/) ⭐️ 8.0/10

该文章批评了当前软件质量状况，认为尽管编码技术（如 AI 辅助）取得了进步，软件却变得漏洞百出、臃肿且对用户不友好。 这反映了开发者和用户普遍的沮丧情绪，凸显了行业炒作与实际用户体验之间的脱节，并引发了对软件开发方向的质疑。 文章指出，现在的更新让人感到恐惧而非兴奋，并指出了焦点劫持、新版本漏洞百出以及非技术冒充者推动产品决策等问题。

hackernews · pchm · Jul 24, 09:08 · [社区讨论](https://news.ycombinator.com/item?id=49033004)

**背景**: “编码问题已解决”的看法源于 AI 代码生成和低代码平台等进步。然而，软件质量下降——臃肿、漏洞、糟糕的用户体验——依然存在，通常归因于激励措施误导、匆忙发布以及缺乏以用户为中心的设计。

**社区讨论**: Hacker News 的评论者普遍认同，指责非技术管理者（“冒充者”）优先追求变化而非质量，有些人建议使用 LTS Linux 发行版以避免有问题的更新。其他人则指出了 macOS 上焦点劫持等具体的 UX 问题，并与 KDE Plasma 上更好的焦点控制进行了对比。

**标签**: `#software quality`, `#user experience`, `#tech industry`, `#productivity`

---

<a id="item-8"></a>
## [科技巨头警告勿过度监管开放权重 AI](https://www.cnbc.com/2026/07/24/nvidia-microsoft-meta-open-weight-ai-models.html) ⭐️ 8.0/10

英伟达、微软和 Meta 联合发表公开信，警告美国政策制定者不要过度监管开放权重 AI 模型，认为这会扼杀创新并削弱美国在 AI 领域的领导地位。 这标志着主要科技公司罕见地统一立场反对拟议中的监管，凸显了开放权重倡导者与 OpenAI、Anthropic 等闭源竞争对手之间日益加深的政治分歧。其结果可能影响未来美国 AI 政策及全球竞争力。 这封公开信发布在英伟达官网，并得到 CEO 黄仁勋的支持，与过去 SOPA 抗议等科技政策斗争相呼应。发布之际正值关于限制中国开放权重模型的辩论，部分初创公司主张继续使用。

hackernews · louiereederson · Jul 24, 13:32 · [社区讨论](https://news.ycombinator.com/item?id=49035303)

**背景**: 开放权重 AI 模型公开发布训练好的神经网络权重，允许任何人下载并在自己的硬件上运行。这与完全开源模型不同，因为训练代码和数据可能仍为专有。美国近期的政策讨论聚焦于中国开放权重模型的潜在风险，因此引发了监管呼声。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you've been told - Open Source Initiative</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者对 Anthropic 等闭源公司的动机表示怀疑，有人指出在对安全性敏感的任务中使用中国开放权重模型的讽刺之处。其他人将这场辩论比作 SOPA 抗议，认为开放权重一方可能比以往斗争获得更广泛的行业支持。

**标签**: `#AI regulation`, `#open-weight`, `#tech industry`, `#policy`, `#artificial intelligence`

---

<a id="item-9"></a>
## [印度要求 GitHub 移除 Bitchat 应用，称其存在安全隐患](https://www.thehindu.com/news/national/government-orders-github-to-remove-bluetooth-based-chat-app-bitchat-over-security-concerns-jack-dorsey/article71262049.ece) ⭐️ 8.0/10

印度政府已命令 GitHub 移除 Bitchat 仓库，这是一款由杰克·多西联合创建的基于蓝牙的加密消息应用，理由是可能被反国家分子和犯罪分子滥用。 这一行动引发了对政府审查和监控的严重担忧，尤其是 Bitchat 能够实现离线点对点通信，从而绕过互联网监控。这也影响了开源社区分发隐私保护工具的能力。 Bitchat 使用低功耗蓝牙（BLE）网状网络，并可通过 Nostr 协议实现基于互联网的消息传递，无需用户账户或中央服务器。印度政府发布该命令是出于对绕过合法监控的担忧。

hackernews · rootkea · Jul 24, 14:41 · [社区讨论](https://news.ycombinator.com/item?id=49036433)

**背景**: Bitchat 是一款点对点加密消息应用，由 Doris Lima 构思、杰克·多西开发，于 2025 年 7 月发布。它通过蓝牙网状网络运行，无需互联网或蜂窝服务，因此在网络受限时非常有用。历史上，印度在 2008 年孟买袭击事件后采取了严格的通信管控措施，包括禁止卫星电话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bitchat">BitChat - Wikipedia</a></li>
<li><a href="https://play.google.com/store/apps/details?id=com.bitchat.droid&hl=en-US">bitchat - Apps on Google Play</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了不同观点：一些人批评政府此举是审查制度，并试图控制抗议通信，而另一些人则指出印度在 2008 年孟买袭击事件后的安全担忧。几位用户将此与过去对卫星电话和 VOIP 的限制相提并论。

**标签**: `#censorship`, `#government surveillance`, `#open source`, `#security`, `#India`

---

<a id="item-10"></a>
## [Buz – 使用现代 Zig 的 Bun 分支，增量构建低于 1 秒](https://ziggit.dev/t/buz-a-drop-in-replacement-for-bun-using-modern-zig-with-sub-1s-incremental-builds/16891) ⭐️ 8.0/10

Buz 是 Bun 的一个替代品，使用现代 Zig 语言，实现了低于 1 秒的增量构建，并删除了超过 11000 行死代码。 这表明 Bun 的构建时间本可以快得多，并突显了大型项目中代码忽视的问题。同时还引发了关于 LLM 在代码清理中作用的讨论，以及功能开发与代码维护之间的权衡。 该分支利用了现代 Zig 特性并更依赖 Zig 的标准库，但 Zig 的增量编译尚不支持 aarch64，且只有 Linux 链接器支持二进制修补。

hackernews · kristoff_it · Jul 24, 09:26 · [社区讨论](https://news.ycombinator.com/item?id=49033099)

**背景**: Bun 是一个一体化 JavaScript 运行时，旨在替代 Node.js。Zig 是一种专注于健壮性和性能的系统编程语言。增量构建只编译代码中更改的部分，显著减少构建时间。Buz 展示了通过现代化代码库和删除死代码来实现这一目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Incremental_build_model">Incremental build model</a></li>

</ul>
</details>

**社区讨论**: 评论者对于 11000 行死代码感到惊讶，有人质疑维护者的经验。还有人批评使用 LLM 清理原本可能是 LLM 生成的代码。一位评论者指出了在大量使用 LLM 的项目中功能开发与代码维护之间的 tick-tock 周期。

**标签**: `#zig`, `#bun`, `#build-performance`, `#open-source-fork`, `#code-quality`

---

<a id="item-11"></a>
## [Claude Opus 5：最不易受提示注入影响的模型](https://simonwillison.net/2026/Jul/25/boris-cherny/#atom-everything) ⭐️ 8.0/10

这标志着 AI 安全领域的重大进步，因为提示注入是 LLM 的关键漏洞，Opus 5 因此更适合敏感和实际应用场景。 该发现详细记录在 Claude Opus 5 系统卡的第 73 页，其中包括评估和红队测试结果，显示出对提示注入的强抵抗力。

rss · Simon Willison · Jul 25, 00:42

**背景**: 提示注入是一种网络安全攻击手段，通过恶意输入使 LLM 绕过安全限制并产生非预期输出。Anthropic 等公司发布的系统卡记录了模型的能力和安全评估结果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection | OWASP Foundation</a></li>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>

</ul>
</details>

**标签**: `#prompt-injection`, `#anthropic`, `#claude`, `#ai-safety`, `#generative-ai`

---

<a id="item-12"></a>
## [长鑫存储 2026 年 DRAM 产能或逼近美光](https://t.me/zaihuapd/42741) ⭐️ 8.0/10

Citrini Research 预测，长鑫存储（CXMT）到 2026 年底将达到约每月 35 万片 DRAM 晶圆启动量，逼近美光的 37.5 万片，届时中国将成为全球第二大 DRAM 生产基地。 中国 DRAM 制造商的快速扩张可能重塑全球存储供应链，减少对外国芯片的依赖，并加剧围绕半导体技术的地缘政治紧张局势。 除了长鑫存储，昇维旭、晋华集成以及长江存储子公司 XMC 等中国企业也在扩产，若全部投产，中国 DRAM 总产能（不含外资在华工厂）可达每月 60 万片。

telegram · zaihuapd · Jul 24, 07:30

**背景**: DRAM（动态随机存取存储器）是用于计算机、服务器和移动设备的关键存储芯片。目前，DRAM 市场由三星、SK 海力士和美光三家非中国企业主导。中国一直在大力投资国内半导体制造以实现自给自足，长鑫存储是其主要的 DRAM 生产商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://www.techinsights.com/blog/300mm-fab-capacity-surpass-10m-wafers-month-2025">300mm Fab Capacity to Surpass 10M Wafers per Month in 2025</a></li>
<li><a href="https://en.wikipedia.org/wiki/XMC_(company)">XMC (company) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#semiconductor`, `#China`, `#manufacturing`, `#memory`

---

<a id="item-13"></a>
## [OpenAI 发布企业 AI 智能体平台 Presence，软件股重挫](https://www.businessinsider.com/openai-release-turns-a-bad-week-ugly-for-software-stocks-2026-7) ⭐️ 8.0/10

2026 年 7 月 22 日，OpenAI 发布了企业 AI 智能体平台 Presence，帮助企业部署和管理 AI 智能体，用于自动化客服、销售及内部流程。消息发布后，Workday、Atlassian、HubSpot、Salesforce 等主要软件股大幅下跌。 Presence 直接与 SaaS 厂商自身的 AI 智能体功能竞争，加剧了对传统企业软件市场的颠覆。这一事件表明，AI 原生平台正在侵蚀成熟的 SaaS 领域，可能重塑竞争格局并影响整个软件行业的投资者情绪。 Presence 支持语音和对话双通道、系统操作能力以及人机协作机制。TD Cowen 分析师将周三 IGV 软件指数约 3% 的下跌主要归因于 OpenAI 的产品，并指出客户服务和销售领域面临最高的颠覆风险。

telegram · zaihuapd · Jul 24, 12:05

**背景**: AI 智能体是一种自主软件系统，能够感知环境、做出决策并执行操作以实现目标，通常与企业工具集成。传统的 SaaS 平台如 Salesforce、Workday 和 Atlassian 一直在将 AI 智能体嵌入其产品中，但 OpenAI 的 Presence 提供独立平台，通过自己的大语言模型后端直接竞争，提供类似能力。这标志着 AI 从功能转变为平台，可能取代现有的 SaaS 工作流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ithome.com/0/980/300.htm">OpenAI 推出 OpenAI Presence，布局企业软件赛道 - IT之家</a></li>
<li><a href="https://juejin.cn/post/7665879209437839386">OpenAI Presence 发布：企业级 AI Agent 正式进入工作流</a></li>
<li><a href="https://www.aitop100.cn/infomation/details/34321.html">OpenAI双重大动作：推出企业Agent平台Presence，300亿自建算力中心-AI...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#企业AI`, `#SaaS`, `#市场竞争`, `#股市影响`

---

<a id="item-14"></a>
## [黄仁勋：美国应允许使用中国开源 AI 模型](https://t.me/zaihuapd/42749) ⭐️ 8.0/10

英伟达 CEO 黄仁勋在采访中表示，中国开源 AI 模型“非常优秀”，美国企业“绝对”应获准使用，并认为这反而会扩大对硬件和芯片的需求。 作为行业领袖的公开表态，此举挑战了以国家安全为由限制中国 AI 的论调，可能影响美国政策及全球 AI 生态格局。 黄仁勋认为中国公司将美国公司挤出市场的可能性为零，并建议通过安全沙箱控制下载的中国模型，而非全面禁止。

telegram · zaihuapd · Jul 24, 13:26

**背景**: 开源 AI 模型允许开发者自由访问、修改和分发底层代码和权重。近年来，阿里巴巴、百度等中国公司发布了有竞争力的开源模型，引发了美国对技术转移和国家安全的担忧。

**标签**: `#AI开源`, `#黄仁勋`, `#政策`, `#英伟达`, `#中国AI模型`

---