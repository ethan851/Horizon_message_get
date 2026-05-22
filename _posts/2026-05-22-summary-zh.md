---
layout: default
title: "Horizon Summary: 2026-05-22 (ZH)"
date: 2026-05-22
lang: zh
---

> From 34 items, 12 important content pieces were selected

---

1. [Freenet 以 WebAssembly 驱动的去中心化应用平台重新启动](#item-1) ⭐️ 9.0/10
2. [黄仁勋：英伟达已基本放弃中国 AI 芯片市场](#item-2) ⭐️ 9.0/10
3. [礼来 retatrutide 三期试验平均减重 28.3%](#item-3) ⭐️ 9.0/10
4. [在 MacBook 上使用 Gemma4-31B 和 50GB 交换空间进行本地视频索引](#item-4) ⭐️ 8.0/10
5. [Python 3.15：未被关注的亮点功能](#item-5) ⭐️ 8.0/10
6. [Google Antigravity 更新覆盖用户安装](#item-6) ⭐️ 8.0/10
7. [新闻机构限制互联网档案馆访问其新闻报道](#item-7) ⭐️ 8.0/10
8. [英伟达 Q4 营收 681 亿美元超预期，Q1 指引上调至 780 亿美元](#item-8) ⭐️ 8.0/10
9. [AMD 发布 Ryzen AI Max 400 系列，内存上限达 192 GB](#item-9) ⭐️ 8.0/10
10. [腾讯推出操作系统级 AI 助手 Marvis](#item-10) ⭐️ 8.0/10
11. [中国审查 Meta 收购 Manus，限制创始人离境](#item-11) ⭐️ 8.0/10
12. [DeepSeek API 更新限速与用户隔离](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Freenet 以 WebAssembly 驱动的去中心化应用平台重新启动](https://freenet.org/) ⭐️ 9.0/10

Freenet 已完全重新设计并重新启动，成为一个全球性的去中心化键值存储，其中键是 WebAssembly 合约。目前已上线，并附带早期应用，包括去中心化群聊 (River) 和 CMS (Delta)。 此次重新发布复兴了一个历史性的点对点项目，采用新颖的架构，通过可交换的合并操作在节点间实现快速、一致的状态同步。它提供了一个实用的平台，用于构建完全在浏览器中运行、无需中心化 API 的去中心化应用。 一致性模型基于无冲突复制数据类型（CRDT），要求每个合约定义一个可交换的合并操作。状态更新像病毒一样传播，通常在几秒内达到全局一致。该平台尚未在移动设备上提供。

hackernews · sanity · May 21, 14:34 · [社区讨论](https://news.ycombinator.com/item?id=48223362)

**背景**: Freenet 最初于 2000 年创建，是最早的点对点匿名网络之一。这个新版本是从头开始完全重写的，从文件共享转变为去中心化键值存储，其中应用是 WebAssembly 合约。使用可交换合并操作是受 CRDT 启发，CRDT 能保证无冲突的最终一致性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48223362">Show HN: Freenet, a peer-to-peer platform for decentralized apps</a></li>
<li><a href="https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type">Conflict-free replicated data type - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 一些评论者批评了在未征得原开发团队同意的情况下替换他们的决定，称这是由不积极参与项目的董事会做出的“象牙塔”决策。其他人对合并方法提出了技术担忧，认为它将复杂性推给了用户，并可能容易受到恶意状态声明的攻击，尽管有些人对 WASM 定义网络行为的潜力感到兴奋。

**标签**: `#peer-to-peer`, `#decentralized`, `#webassembly`, `#distributed systems`, `#p2p`

---

<a id="item-2"></a>
## [黄仁勋：英伟达已基本放弃中国 AI 芯片市场](https://www.cnbc.com/2026/05/21/nvidia-jensen-huang-china-ai-chip-market-huawei.html) ⭐️ 9.0/10

英伟达 CEO 黄仁勋宣布，由于美国出口管制，公司已“基本放弃”中国 AI 芯片市场，将市场让给华为等本土厂商。 这标志着 AI 芯片供应链的重大地缘政治转变，中国曾是英伟达的重要收入来源。此举加速了中国在 AI 半导体领域的自力更生，华为的昇腾芯片正成为可行的替代方案。 中国此前占英伟达数据中心收入的至少五分之一。2026 年 4 月，特朗普政府要求对华出口先进芯片须取得许可证，实质上排除了英伟达。黄仁勋表示公司已告知投资者，对获得在华销售先进芯片的许可“不要抱任何期望”。

telegram · zaihuapd · May 21, 05:52

**背景**: 自 2022 年起，美国对向中国出口先进 AI 芯片实施出口管制，最初针对英伟达的 A100 和 H100 GPU。管制措施逐步收紧，阻止了 H100 和 H200 等旗舰芯片的销售。华为开发了自己的 AI 芯片系列——昇腾，其中 910C 的推理性能约为 H100 的 60%。2026 年 2 月，中国 AI 初创公司智谱 AI 完全使用华为昇腾 910B 芯片训练了一个前沿模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://builtin.com/articles/trump-lifts-ai-chip-ban-china-nvidia">Trump Lifted the AI Chip Ban on China, Clearing Nvidia and AMD to Resume Sales: Now What? | Built In</a></li>
<li><a href="https://www.tomshardware.com/pc-components/gpus/huawei-introduces-the-ascend-920-ai-chip-to-fill-the-void-left-by-nvidias-h20">Huawei introduces the Ascend 920 AI chip to fill the... | Tom's Hardware</a></li>
<li><a href="https://thamizhelango.medium.com/mindspore-zhipu-ai-huawei-ascend-how-china-built-a-frontier-ai-model-without-a-single-nvidia-68403d92cedb">MindSpore, Zhipu AI & Huawei Ascend : How China Built... | Medium</a></li>

</ul>
</details>

**标签**: `#AI芯片`, `#出口管制`, `#英伟达`, `#华为`, `#地缘政治`

---

<a id="item-3"></a>
## [礼来 retatrutide 三期试验平均减重 28.3%](https://www.prnewswire.com/news-releases/lillys-triple-agonist-retatrutide-delivered-powerful-weight-loss-in-pivotal-phase-3-obesity-trial-302778859.html) ⭐️ 9.0/10

礼来宣布，其三重激动剂 retatrutide 在 TRIUMPH-1 三期试验中达到所有主要及关键次要终点，12 mg 剂量组在 80 周内平均减重 28.3%，45.3%的参与者减重至少 30%。 这代表了肥胖三期试验中有报告的最高平均减重幅度之一，预示着肥胖及相关合并症药物治疗可能迎来范式转变，具有重大的公共健康影响。 试验纳入约 2500 名肥胖或超重且至少伴有一种体重相关合并症的成人；4 mg 剂量组平均减重 19.0%，12 mg 组因不良事件停药率为 4.1%（安慰剂组为 4.9%），常见副作用以胃肠道反应为主，未观察到心脏或肝脏问题。

telegram · zaihuapd · May 22, 02:18

**背景**: Retatrutide 是一种在研的三重激素受体激动剂，同时靶向 GLP-1、GIP 和胰高血糖素受体，旨在超越现有双激动剂（如 tirzepatide）的减重效果。GLP-1 受体激动剂是一类通过降低食欲和血糖来发挥作用的药物，最初用于 2 型糖尿病，现越来越多用于肥胖症。这种三重机制旨在进一步放大代谢获益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retatrutide">Retatrutide - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC12190491/">Retatrutide—A Game Changer in Obesity Pharmacotherapy - PMC</a></li>

</ul>
</details>

**标签**: `#obesity`, `#clinical trial`, `#GLP-1`, `#retatrutide`, `#weight loss`

---

<a id="item-4"></a>
## [在 MacBook 上使用 Gemma4-31B 和 50GB 交换空间进行本地视频索引](https://blog.simbastack.com/indexed-a-year-of-video-locally/) ⭐️ 8.0/10

一位开发者在一台 2021 年的 MacBook 上，使用 Google 的 Gemma4-31B 模型并借助 50GB 的交换空间，对一年的个人视频素材建立了本地索引。相关代码已以 MIT 许可证发布在 GitHub 上。 这表明大型语言模型可以在消费级硬件上用于实际且保护隐私的个人存档工作，无需依赖云服务。它实现了高效的本地视频检索与分析，该项目还计划与 DaVinci Resolve 等视频编辑软件集成。 Gemma4-31B 模型在 4 位量化下约为 19 GiB，但开发者的设置使用了 28.4 GiB 的模型权重和图像上下文，并启用了额外的交换空间。大量使用交换可能加速 SSD 磨损。该项目还希望利用该索引通过 DaVinci Resolve 加快视频编辑。

hackernews · asenna · May 21, 14:01 · [社区讨论](https://news.ycombinator.com/item?id=48222733)

**背景**: 像 Gemma4-31B 这样的大型语言模型需要大量 RAM；当 RAM 不足时，操作系统会使用磁盘上的交换空间，但这可能降低性能并缩短 SSD 寿命。Gemma4-31B 是 Google 推出的密集 31B 参数模型，在数学和编程基准测试中取得了最先进的成绩，常常超越拥有超过 400B 参数的模型。本地运行此类模型需要精细的内存管理，通常涉及量化和交换。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.google.dev/gemma/docs/core/model_card_4">Gemma 4 model card | Google AI for Developers</a></li>
<li><a href="https://tech-insider.org/google-gemma-4-open-model-benchmarks-2026/">Gemma 4: How a 31B Model Beats 400B Rivals [2026]</a></li>
<li><a href="https://ryanagibson.com/posts/run-llms-larger-than-ram/">How to Run LLMs Larger than RAM · Ryan A. Gibson</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了见解：有人描述了一个使用 Whisper 和嵌入的类似 Electron 应用，有人质疑在量化已降低内存需求的情况下使用交换空间，作者则回应并创建了公开的 GitHub 仓库。讨论反映了对本地视频索引和实际 LLM 部署的兴趣。

**标签**: `#local-llm`, `#video-indexing`, `#personal-archives`, `#gemma`, `#machine-learning`

---

<a id="item-5"></a>
## [Python 3.15：未被关注的亮点功能](https://blog.changs.co.uk/python-315-features-that-didnt-make-the-headlines.html) ⭐️ 8.0/10

Python 3.15 在 threading 模块中新增了迭代器同步原语，并为 collections.Counter 添加了对称差分支持，此外还有多项不太引人注目的改进。 这些新增功能完善了 Python 的并发工具集，并补全了 Counter 的多重集操作，有利于使用线程化迭代器和进行数据分析的开发者。 迭代器同步原语允许对生成器进行安全的并发迭代。Counter 的 symmetric_difference 方法计算两个计数器对象的对称差分，这一特性曾在 Python 增强提案中被提出并在 GitHub 上讨论。

hackernews · rbanffy · May 21, 11:10 · [社区讨论](https://news.ycombinator.com/item?id=48220696)

**背景**: Python 的 threading 模块长期以来提供了锁、事件等同步原语，但迭代器本身并非线程安全。新增的原语填补了这一空白。collections.Counter 类自 Python 2.7 起支持多重集操作，但对称差分一直缺失，如今在 3.15 中被补全。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.python.org/3/library/asyncio-sync.html">Synchronization Primitives — Python 3.14.5 documentation</a></li>
<li><a href="https://docs.python.org/3/library/threadsafety.html">Thread Safety Guarantees — Python 3.14.5 documentation</a></li>
<li><a href="https://discuss.python.org/t/add-symmetric-difference-to-collections-counter/103579">Add symmetric difference to collections.Counter - Ideas - Discussions on Python.org</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一：有人称赞新的迭代器同步功能，也有人质疑功能膨胀。另一位用户指出博客中 Counter 示例可能存在的错误，而关于惰性导入的讨论澄清了它并非新特性。

**标签**: `#Python`, `#Python 3.15`, `#programming languages`, `#features`, `#threading`

---

<a id="item-6"></a>
## [Google Antigravity 更新覆盖用户安装](https://www.0xsid.com/blog/antigravity-bait-n-switch) ⭐️ 8.0/10

Google 发布了新版本的 Antigravity，该版本覆盖了现有安装和用户设置，且没有清晰的迁移方案，导致许多开发者感到困惑并丢失数据。 此次更新削弱了开发者对 Google 工具的信任，暴露了重大的用户体验失败，尤其考虑到 Antigravity 被定位为核心 AI 开发平台。 此次更新将之前的工具（如 Gemini CLI）合并到 Antigravity CLI 和 IDE 中，但未保留现有配置，用户需要手动恢复设置和数据库。

hackernews · ssiddharth · May 21, 13:50 · [社区讨论](https://news.ycombinator.com/item?id=48222529)

**背景**: Google Antigravity 是一套 AI 开发工具，包括 IDE、CLI 和聊天界面。它取代了早期的 Gemini CLI 和 Code Assist 等工具。最近的更新旨在将这些产品统一到 Antigravity 品牌下。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://antigravity.google/changelog">Google Antigravity Changelog</a></li>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/google-io-2026-developer-highlights/">I/O 2026 developer highlights: Antigravity, Gemini API, AI Studio</a></li>
<li><a href="https://developers.googleblog.com/an-important-update-transitioning-gemini-cli-to-antigravity-cli/">An important update: Transitioning Gemini CLI to Antigravity CLI - Google Developers Blog</a></li>

</ul>
</details>

**社区讨论**: 用户表达了强烈不满，有人称之为“诱饵调包”。一位开发者提供了恢复 VS Code 设置和聊天历史的 Python 脚本。其他人则批评 Google 缺乏专注和糟糕的更新策略。

**标签**: `#Google`, `#User Experience`, `#Software Update`, `#Controversy`

---

<a id="item-7"></a>
## [新闻机构限制互联网档案馆访问其新闻报道](https://www.niemanlab.org/2026/05/more-than-340-local-news-outlets-are-limiting-the-internet-archives-access-to-their-journalism/) ⭐️ 8.0/10

超过 340 家地方新闻机构正在通过 robots.txt 文件限制互联网档案馆的 Wayback Machine 抓取和存档其内容，威胁到历史新闻的保存。 这限制了公众对历史新闻的访问，并削弱了档案馆为研究人员、记者和 AI 训练提供资源的能力。这也标志着内容货币化与数字保存之间的紧张关系日益加剧。 这些限制通过 robots.txt 实施，这是一个网络爬虫通常遵守的自愿协议。互联网档案馆必须遵守，否则可能被完全屏蔽，尽管历史上一些档案馆曾出于非商业目的忽略 robots.txt。

hackernews · jaredwiener · May 21, 16:59 · [社区讨论](https://news.ycombinator.com/item?id=48225838)

**背景**: 网络存档是收集和保存网络内容以供未来访问的过程。互联网档案馆的 Wayback Machine 使用自动爬虫抓取网站快照。Robots.txt 是一种标准，允许网站所有者指定哪些部分可以被爬取，但遵守是自愿的。越来越多地使用 robots.txt 阻止存档爬虫反映了保护公共访问与保护付费墙或许可收入之间的冲突。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Robots.txt">Robots.txt</a></li>
<li><a href="https://en.wikipedia.org/wiki/Web_archiving">Web archiving</a></li>
<li><a href="https://en.wikipedia.org/wiki/Digital_preservation">Digital preservation</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了失望，指出历史内容的丢失以及 Wayback Machine 在事实核查和追踪编辑方面的重要性。有人建议折中方案，如延迟一周访问，而其他人则提倡微支付系统，在不阻止存档的情况下补偿出版商。

**标签**: `#Internet Archive`, `#digital preservation`, `#journalism`, `#web archiving`, `#AI training`

---

<a id="item-8"></a>
## [英伟达 Q4 营收 681 亿美元超预期，Q1 指引上调至 780 亿美元](https://t.me/zaihuapd/41498) ⭐️ 8.0/10

英伟达公布 2025 财年第四季度营收 681 亿美元，超出市场预期，其中数据中心业务营收 623 亿美元，每股利润 1.62 美元同样高于预期。公司预计 2026 财年第一季度销售额将达到 780 亿美元，显著高于华尔街预期的 726 亿美元。 这份财报凸显了英伟达 AI 芯片在数据中心领域的持续爆炸式需求，增强了投资者对 AI 硬件周期的信心。上调的指引表明 AI 浪潮仍在加速，影响整个半导体和 AI 生态系统。 尽管营收超预期，但英伟达的游戏和汽车业务未达预期，部分投资者担忧 OpenAI 的融资能力及行业竞争。CEO 黄仁勋指出计算需求呈指数级增长，并已通过战略手段确保库存以应对供应链压力。

telegram · zaihuapd · May 21, 05:10

**背景**: 英伟达是用于 AI 训练和推理的图形处理器（GPU）的领先供应商，尤其是其 H100 和 Blackwell 系列。该公司的季度业绩被视为 AI 行业需求的风向标。数据中心营收目前占英伟达总营收的 90%以上，反映出从 PC 游戏向 AI 计算的转变。

**标签**: `#nvidia`, `#earnings`, `#ai`, `#data center`, `#semiconductor`

---

<a id="item-9"></a>
## [AMD 发布 Ryzen AI Max 400 系列，内存上限达 192 GB](https://www.techpowerup.com/349218/amd-launches-the-ryzen-ai-max-400-series-processors-strix-halo-gets-a-memory-upgrade) ⭐️ 8.0/10

AMD 发布了 Ryzen AI Max 400 系列处理器，这是 Strix Halo 平台的升级版，统一内存从 128 GB 提升至 192 GB，集显最多可分得 160 GB 显存，可运行超 3000 亿参数的大语言模型。 这一进展大幅提升了便携 AI 工作站的能力，使开发者无需独立显卡即可在本地运行大规模 AI 模型，并推动了统一内存架构在高性能移动计算领域的发展趋势。 首发三款均为 PRO 商用型号：旗舰 495 拥有 16 核 CPU 和 40 个计算单元 (CU)，490 和 485 分别为 12 核/8 核配 32 个 CU。消费级版本计划今年晚些时候推出。

telegram · zaihuapd · May 21, 08:15

**背景**: AMD 的 Strix Halo 平台将 CPU、GPU 和 NPU 集成在单芯片中，采用统一内存架构，允许它们共享内存池。与显存受限的传统独立 GPU 方案不同，统一内存使集成 GPU 能访问大容量内存，适用于在本地运行像大语言模型这样的 AI 工作负载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.servethehome.com/framework-desktop-review-a-solid-amd-strix-halo/">Framework Desktop Review A Solid AMD Strix Halo - ServeTheHome</a></li>
<li><a href="https://skip.watch/read?v=AcTmeGpzhBk">Running 110B LLMs on a Laptop: AMD's New APU vs.... - SkipWatch</a></li>

</ul>
</details>

**标签**: `#AMD`, `#Ryzen AI Max`, `#处理器`, `#AI`, `#大语言模型`

---

<a id="item-10"></a>
## [腾讯推出操作系统级 AI 助手 Marvis](https://finance.sina.com.cn/jjxw/2026-05-21/doc-inhyrmmu5949795.shtml) ⭐️ 8.0/10

腾讯正式推出操作系统级 AI 助手 Marvis（马维斯），该产品集成了多智能体编排和端侧隐私模式，现可免邀请码免费下载。 此次发布标志着 AI 深度集成到操作系统层的重要一步，有望改变用户与设备的交互方式，并为大型科技公司的隐私保护 AI 助手树立新标杆。 Marvis 内置 6 个专项 Agent，由主 Agent 统筹调度，并提供了完全在端侧运行的隐私模式，使用本地大模型，确保数据不上云。每位用户每天可享 1000 万免费 Token。

telegram · zaihuapd · May 21, 10:00

**背景**: 多智能体编排是指由主 Agent 将任务分配给多个专项 Agent 协同完成复杂工作流。端侧 AI 直接在用户硬件上运行模型，增强隐私保护并支持离线使用。Marvis 在操作系统层面应用这些概念，将系统、文件、应用和跨端能力统一整合。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Multi-agent_orchestration">Multi-agent orchestration</a></li>
<li><a href="https://grokipedia.com/page/On-device_artificial_intelligence">On-device artificial intelligence</a></li>

</ul>
</details>

**标签**: `#AI`, `#Operating System`, `#Tencent`, `#Privacy`, `#Agent`

---

<a id="item-11"></a>
## [中国审查 Meta 收购 Manus，限制创始人离境](https://t.me/zaihuapd/41509) ⭐️ 8.0/10

中国监管部门正在审查 Meta 收购 AI 初创公司 Manus 是否违反投资规定，并已限制联合创始人 Xiao Hong 和 Ji Yichao 离境。 此次审查表明中国对重大跨境 AI 收购的监管力度加大，可能影响未来的技术交易和地缘政治格局。 两位联合创始人在与国家发改委会面后被通知不得离境，但可在境内自由活动；交易金额未公开，但此前报道称估值约 20 亿美元。

telegram · zaihuapd · May 21, 13:11

**背景**: Manus 是一款通用型 AI 智能体，由蝴蝶效应公司开发，该公司成立于中国，总部位于新加坡。它能自主规划、推理并执行复杂任务。Meta 于 2024 年 12 月宣布收购 Manus 以增强其 AI 能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus ( AI agent) - Wikipedia</a></li>
<li><a href="https://manus.im/">Manus : Hands On AI</a></li>
<li><a href="https://gcmori.medium.com/manus-ai-the-rise-of-the-general-ai-agent-88c54756295a">Manus AI : The Rise of the General AI Agent | by Giancarlo... | Medium</a></li>

</ul>
</details>

**标签**: `#Meta`, `#Acquisition`, `#AI`, `#China Regulation`, `#Geopolitics`

---

<a id="item-12"></a>
## [DeepSeek API 更新限速与用户隔离](https://api-docs.deepseek.com/zh-cn/quick_start/rate_limit) ⭐️ 8.0/10

DeepSeek 更新了 API 文档，明确了 V4 模型的并发限制（deepseek-v4-pro: 500，deepseek-v4-flash: 2500），并引入了 user_id 参数，用于更细粒度的管理，包括内容安全、KVCache 和调度隔离。 此次更新通过允许开发者在单一 API 账号内隔离用户，增强了多租户应用管理能力，并提供清晰的文档帮助用户规划容量，避免 HTTP 429 错误。 超出并发限制会返回 HTTP 429 错误；用户可免费申请扩容以获得更高限制。对于普通 API 用户，所有 user_id 合并计算总并发；已提升配额的账号，每个 user_id 也会受与模型对应的单用户并发限制。

telegram · zaihuapd · May 21, 15:03

**背景**: KVCache（键值缓存）是一种基于 Transformer 的大语言模型优化技术，通过缓存自注意力中的中间键值数据来加速推理。user_id 隔离功能允许 API 使用者为不同终端用户分配不同用户 ID，从而在同一账号内为每个用户实现独立的 KVCache 和调度策略。这对于需要为每个租户提供隔离资源和安全边界的多租户应用尤为有用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/quick_start/rate_limit">Rate Limit & Isolation | DeepSeek API Docs</a></li>
<li><a href="https://hattussa.com/blog/boosting-transformer-efficiency-with-kvcache/">Boosting Transformer Efficiency with KVCache ! - Hattussa Blog...</a></li>

</ul>
</details>

**标签**: `#DeepSeek`, `#API`, `#rate limiting`, `#concurrency`, `#user isolation`

---