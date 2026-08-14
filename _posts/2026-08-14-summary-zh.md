---
layout: default
title: "Horizon Summary: 2026-08-14 (ZH)"
date: 2026-08-14
lang: zh
---

> From 27 items, 11 important content pieces were selected

---

1. [Cerebras 与 OpenAI 的 GPT-5.6 Sol Ultrafast 将 HLE 运行速度提升 7 倍](#item-1) ⭐️ 9.0/10
2. [Spaghettifying DRAM 攻击实现处理器级隐藏代码执行](#item-2) ⭐️ 9.0/10
3. [DeepSeek 发布 Harness 并开放 V4-Pro-0813 权重](#item-3) ⭐️ 9.0/10
4. [谷歌推出 Gemini 3.7 Flash，主打性价比](#item-4) ⭐️ 8.0/10
5. [理解成为 LLM 驱动开发的新瓶颈](#item-5) ⭐️ 8.0/10
6. [选择无聊技术，善用创新额度](#item-6) ⭐️ 8.0/10
7. [Oxide 平台上的 Kubernetes：客户需求推动新集成](#item-7) ⭐️ 8.0/10
8. [特朗普签署备忘录，允许私企开展美国支持的进攻性网络行动](#item-8) ⭐️ 8.0/10
9. [DeepMind 发布手语转文字模型 SL2T，首次落地 Pixel 11](#item-9) ⭐️ 8.0/10
10. [谷歌发布 Gemini 3.6 Flash，透露 Gemini 4 已启动预训练](#item-10) ⭐️ 8.0/10
11. [X 开源排名算法，新增工具让用户自查是否被隐形限制](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Cerebras 与 OpenAI 的 GPT-5.6 Sol Ultrafast 将 HLE 运行速度提升 7 倍](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 9.0/10

Cerebras 与 OpenAI 宣布，GPT-5.6 Sol 的 Ultrafast 模式在 11 小时 11 分钟内回答了 Humanity's Last Exam 的全部 2500 道题。这比需要 78 小时 27 分钟连续计算的 Claude Fable 5 快了近 7 倍。 这一结果凸显了推理速度是 AI 竞争的重要前沿，可能将经济价值从模型权重转向专用推理硬件。更快的推理支持更多迭代式思考，从而显著提升输出质量，并使前沿 AI 在实时应用中更加实用。 所用基准是 Humanity's Last Exam，这是一个包含 2500 道跨一百多个学科专家出题的测试集。值得注意的是，有评论者质疑快速模式是否与标准 GPT-5.6 Sol 的准确率完全一致，因为两家公司在公告中都没有明确证实这一点。

hackernews · pr337h4m · Aug 13, 18:10 · [社区讨论](https://news.ycombinator.com/item?id=49289844)

**背景**: Cerebras 制造晶圆级引擎，这是全球最大的 AI 处理器；其 WSE-3 包含 4 万亿个晶体管和 90 万个 AI 优化核心，拥有 44GB 片上 SRAM，为 AI 工作负载提供巨大的内存带宽。Humanity's Last Exam（HLE）是由 Center for AI Safety 和 Scale AI 共同创建的前沿基准，旨在成为覆盖面广泛、最后一个封闭式学术基准。Cerebras 与 OpenAI 一直在合作，让前沿模型以超快推理速度运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras_Systems">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Humanity's_Last_Exam">Humanity's Last Exam - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体积极但存在分歧。一些评论者预测 AI 的经济价值将从模型权重转向推理硬件，并以操作系统最终免费作类比。另一些人赞赏更快推理带来的迭代速度优势，也有少数人对 Ultrafast 模式是否真的与标准准确率一致表示怀疑，指出 Cerebras 和 OpenAI 都没有明确确认性能完全相同。

**标签**: `#AI`, `#inference`, `#hardware`, `#OpenAI`, `#Cerebras`

---

<a id="item-2"></a>
## [Spaghettifying DRAM 攻击实现处理器级隐藏代码执行](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

安全研究员 Christopher Domas 发布了“Spaghettifying DRAM”技术，通过操纵 DRAM 控制器的地址转换来扰乱物理内存，进而访问平台安全处理器、系统管理模式和 CPU 微码等隐藏处理器区域。该攻击已在 AMD Family 16h CPU（如 Jaguar）上演示，可在操作系统之下、即 ring -1 层级运行。 这项研究揭示了一类新型 DRAM 攻击，能够绕过所有高层系统保护机制，削弱受影响 CPU 的硬件可信基础。它对系统安全具有深远影响，波及操作系统厂商、硬件制造商以及旧款 AMD 处理器用户，并引发了对隐藏硬件特权级别的广泛担忧。 该技术利用线性代数重建 DRAM 地址映射，且在内存控制器中翻转单个比特即可解锁隐藏区域。根据 GitHub 仓库说明，该攻击在 AMD Jaguar（2013）上有效，而 Zen 3 的内存控制器寄存器基地址不同，因此该攻击是否适用于更新的 CPU 尚不明确。

hackernews · matt_d · Aug 13, 14:17 · [社区讨论](https://news.ycombinator.com/item?id=49286341)

**背景**: DRAM 控制器负责将物理地址转换为实际内存位置，而这种转换通常对软件不可见。“Spaghettifying DRAM”正是利用了对这些转换的操纵能力，通过重写内存层级来暴露隐藏区域。“Spaghettification（面条化）”一词借自黑洞附近的潮汐拉伸效应，在这里比喻内存被搅乱的过程。在 x86 系统中，特权环（protection ring）用于保护操作系统（ring 0）免受用户程序（ring 3）的干扰，而虚拟机监控程序和固件运行在更高特权级别（ring -1），本次攻击正是瞄准了这一层。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/xoreaxeaxeax/skitter-creek-bath-salts">Spaghettifying DRAM</a></li>
<li><a href="https://zeli.app/en/story/49286341">Spaghettifying DRAM: Unlock Everything on the CPU | Zeli</a></li>
<li><a href="https://en.wikipedia.org/wiki/Protection_ring">Protection ring - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对于 Christopher Domas 即将举行的 Black Hat 演讲表现出极大热情，并盛赞他此前关于逆向工程和硬件安全的演讲。部分评论质疑该攻击对现代 CPU 的适用性，指出目前仅确认 AMD Jaguar 受影响，并追问更新的处理器情况。还有人指出，DRAM 日益复杂化扩大了攻击面，并猜测 Xbox 和 PlayStation 等游戏机安全团队可能会担忧：一旦获得 ring-0 访问权限，系统就可能被完全攻破。

**标签**: `#DRAM`, `#security`, `#hardware exploitation`, `#ring -1`, `#Christopher Domas`

---

<a id="item-3"></a>
## [DeepSeek 发布 Harness 并开放 V4-Pro-0813 权重](https://mp.weixin.qq.com/s/mANdGRI4fO_sEbC1ECEoZQ) ⭐️ 9.0/10

DeepSeek 已发布开源智能体框架 DeepSeek Harness（MIT 协议），并在 Hugging Face 开放了 DeepSeek-V4-Pro-0813 模型权重。该 Harness 采用由 Cordis 驱动的“一切皆插件”架构，提供标准、PTC、极简和创造四种运行模式。 这是开源 AI 生态的一个里程碑式更新：DeepSeek 不仅开放了模型权重，还发布了一个高度可扩展的智能体框架。插件化设计让开发者可以轻松替换或重组模型、工具、调度、UI 等所有组件，可能影响未来智能体框架的构建方式。 该框架以开发者预览版形式发布，GitHub 仓库在公告后不久开放。此前 V4-Pro-0813 权重的 Hugging Face 页面短暂出现 404，随后已恢复。其架构由 Cordis 驱动，Cordis 是一个支持在不重启进程的情况下热加载和卸载插件的元框架。

telegram · zaihuapd · Aug 13, 12:39

**背景**: 智能体框架（agent harness）是将语言模型与工具、记忆、执行环境连接起来的“骨架”，是构建 AI 智能体的基础设施。DeepSeek Harness 将模型、工具、技能、会话、沙箱、存储、循环、调度、UI 等所有能力都设计为可替换的插件，使系统高度模块化。底层框架 Cordis 已在 Koishi 项目中使用多年，专为时空可组合性设计，卸载插件时可还原其产生状态和副作用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepseek.com/harness/en/">DeepSeek Harness developer preview: Everything is a plugin</a></li>
<li><a href="https://github.com/deepseek-ai/deepseek-harness">GitHub - deepseek-ai/deepseek-harness: DeepSeek Harness ...</a></li>
<li><a href="https://github.com/cordiverse/cordis">GitHub - cordiverse/cordis: Meta-Framework of Spatiotemporal Composability · GitHub</a></li>

</ul>
</details>

**社区讨论**: DeepSeek Harness 的作者表示这只是一个早期开发者预览版，可能存在不少粗糙之处和破坏性变更。社区成员特别称赞了可追溯性功能——以只追加会话日志记录模型的一切交互——并指出美国厂商的模型跟踪记录是加密的。还有人讨论了底层 Cordis 框架，并对“一切皆插件”是否会造成开发者的“插件疲劳”提出质疑。

**标签**: `#DeepSeek`, `#AI模型`, `#开源`, `#模型权重`, `#工具`

---

<a id="item-4"></a>
## [谷歌推出 Gemini 3.7 Flash，主打性价比](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 8.0/10

谷歌发布了 Gemini 3.7 Flash，这是其 Flash 系列的最新迭代，基于 Gemini 3.6 Flash，现已用于 Gemini Spark。新模型支持可自定义的思考配置，并推出了将在 2027 年上涨的引人注目的首发定价。 此次发布强化了谷歌在竞争激烈的 LLM 市场中以低成本提供强大性能的策略。依赖 Gemini Flash 系列处理高容量、视觉任务的开发者和企业将直接受到新性价比平衡的影响。 Gemini 3.7 Flash 基于 Gemini 3.6 Flash，对其核心推理基础进行了算法改进。其首发定价将于 2026 年 12 月 31 日翻倍，从 2027 年 1 月 1 日起输入 token 价格将涨至每百万个 1.50 美元，输出 token 涨至每百万个 7.50 美元。

hackernews · thisisauserid · Aug 13, 17:23 · [社区讨论](https://news.ycombinator.com/item?id=49289112)

**背景**: Gemini 是由 Google DeepMind 开发的多模态大语言模型（LLM）系列，包含 Pro、Flash 等不同版本。Flash 系列被定位为低成本、高容量的“工作马”模型，适用于总结、解析和 agentic 工作流等文本及多模态任务。Gemini 3.7 Flash 延续了这一传统，同时添加了视觉能力和可配置的推理深度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-7-flash/">Gemini 3.7 Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/models">Models - Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人称赞该模型在图像转 HTML 任务上的性价比表现，也有人对不寻常的首发定价和快速的迭代节奏表示质疑。多位评论者指出，GPT-5.6 Luna 等竞争对手在基准测试上更优且成本更低，削弱了 Flash 系列的价值主张。

**标签**: `#AI`, `#Google`, `#Gemini`, `#LLM`, `#model release`

---

<a id="item-5"></a>
## [理解成为 LLM 驱动开发的新瓶颈](https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck) ⭐️ 8.0/10

Geoffrey Litt 在文章《理解成为新的瓶颈》中指出，随着 LLM 自动化代码生成，软件开发的关键制约从编写代码转向理解代码与系统。该文在 Hacker News 上引发热议，获得 197 分和 108 条评论。 这一重新定位之所以重要，是因为它挑战了“AI 生成代码越多就等于生产力越高”的假设。如果工程师无法理解他们要发布的、审查的和维护的代码，那么理解——而非生成——就成为软件开发规模、质量和安全性的制约因素。 文章的核心是瓶颈的转移：开发者的精力不再主要花在从头编写代码，而是花在理解 LLM 生成的代码、对照系统架构检查它、并更新自己的心智模型上。评论者也警告说，依赖 LLM 生成“理解”是有缺陷的，因为错误的模型无法可靠地自我验证。

hackernews · sebg · Aug 13, 18:47 · [社区讨论](https://news.ycombinator.com/item?id=49290299)

**背景**: 大型语言模型（LLM）现在能够自动补全并生成大量代码，降低了编写代码的成本。然而，代码仍然需要被审查、调试、扩展并集成到更大的系统中，这些任务需要对系统行为有人的心智模型。该文章提出，这种人类理解工作正在成为更稀缺的资源，工具和实践应该围绕支持理解而非仅仅生成来重新设计。

**社区讨论**: 讨论中不少人认同“理解”在 LLM 出现之前就已经是瓶颈，但也有人指出 LLM 改变了理解发生的时机——从“前置”（写代码之前）变为“后置”（代码生成之后）。一些评论者批评 LLM 生成的 PR 描述过于机械、缺乏动机，并警告不要用 LLM 去生成用于检查 LLM 本身所必需的理解。

**标签**: `#LLMs`, `#software engineering`, `#code comprehension`, `#developer productivity`, `#program management`

---

<a id="item-6"></a>
## [选择无聊技术，善用创新额度](https://mcfunley.com/choose-boring-technology) ⭐️ 8.0/10

在这篇 2015 年的文章中，Dan McKinley 认为工程团队的“创新额度”是有限的，应只把额度花在真正能带来竞争优势的技术上，其余场合则应默认选择成熟可靠、被充分理解的“无聊技术”。 这篇文章为工程领导者提供了一种简单的心智模型，用来做出并解释技术取舍，因此十年来一直很有影响力。在团队考虑采用智能体并需要决定哪里可以承担风险时，这一模型尤其有参考价值。 在该模型中，“无聊”不代表过时，而是指成熟、可靠、被充分理解的技术。每个团队只有少量固定的创新额度，选择新技术会消耗额度，而选择成熟技术则不需要。

hackernews · tosh · Aug 13, 17:48 · [社区讨论](https://news.ycombinator.com/item?id=49289512)

**背景**: Dan McKinley 在 Etsy 担任了六年软件工程师，期间该公司的工程团队以高效率著称，他于 2015 年写下这篇文章。文章提出，每家公司的创新额度实际上是有限的，如果把额度花在不重要的工具上，留给真正关键领域的额度就会变少。更广泛的“无聊技术”思潮认为，成熟技术比时髦的新技术发布更快、故障更少、维护更容易。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/technical-debt-innovation-tokens-case-boring-technology-jeffrey-henry-lhexe">Technical Debt, Innovation Tokens , and the Case for Boring...</a></li>
<li><a href="https://mattrickard.com/innovation-tokens">Innovation Tokens | Matt Rickard</a></li>
<li><a href="https://blog.glyph.im/2024/07/against-innovation-tokens.html">Deciphering Glyph :: Against Innovation Tokens</a></li>

</ul>
</details>

**社区讨论**: 评论者大多盛赞这篇文章；NickNaraghi 称这是“我最喜欢的博文之一”，并说创新额度概念是他作为产品经理和工程负责人职业生涯中最好用的想法之一。theptip 提出，在智能体时代，团队应把所有创新额度都投向智能体本身，其他部分则选用“无聊”的、分布内（in-distribution）技术。不过 insanitybit 提出反驳，认为创新额度的框架很随意、不够严肃，工程师应评估真实风险和取舍，而不是把“新颖”当作弱代理指标。

**标签**: `#software engineering`, `#technology strategy`, `#engineering culture`, `#innovation`, `#essay`

---

<a id="item-7"></a>
## [Oxide 平台上的 Kubernetes：客户需求推动新集成](https://oxide.computer/blog/kubernetes-on-oxide) ⭐️ 8.0/10

Oxide Computer 发布了一篇博客，详细介绍了客户需求如何推动其 Kubernetes 集成工作，包括 oxide-cloud-controller-manager 和基于 Cluster API 的集群供应。文章解释了这些集成背后的设计与动机。 这件事很重要，因为这意味着 Oxide 的机架级云平台开始拥抱标准的 Kubernetes 生态组件，让企业更容易在 Oxide 硬件上运行 Kubernetes 工作负载。采用 Cloud Controller Manager 和 Cluster API 符合行业标准做法，有助于降低厂商锁定风险。 oxide-cloud-controller-manager 是一个 Kubernetes 控制面组件，内嵌了 Oxide 特定的控制逻辑，使集群能够通过 Cloud Controller Manager 架构与 Oxide API 集成。Cluster API 是 Kubernetes 子项目，专注于提供声明式 API 和工具，以简化多个 Kubernetes 集群的供应、升级和运维。

hackernews · stevehipwell · Aug 13, 14:26 · [社区讨论](https://news.ycombinator.com/item?id=49286485)

**背景**: Oxide Computer 提供机架级云计算机，将计算、存储、网络和软件集成到单一平台中。Kubernetes 是一个流行的容器编排系统，而 Cloud Controller Manager 是 Kubernetes 的标准组件，用于让云提供商集成自己的 API。Cluster API 是 Kubernetes 生态的一部分，用于自动化集群生命周期管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/oxidecomputer/oxide-cloud-controller-manager">Oxide Cloud Controller Manager - GitHub</a></li>
<li><a href="https://docs.oxide.computer/guides/integrations/cloud-controller-manager">Cloud Controller Manager / Guides / Oxide</a></li>
<li><a href="https://github.com/kubernetes-sigs/cluster-api">GitHub - kubernetes -sigs/ cluster - api : Home for Cluster API ...</a></li>

</ul>
</details>

**社区讨论**: 评论者对 oxide-cloud-controller-manager 的设计表现出浓厚兴趣，有人猜测会出现 karpenter-provider-oxide。还有人称赞 Cluster API，认为它被低估且具有企业级成熟度；也有一些评论表达了想在家拥有一台 Oxide 机架，或询问 Oxide 与裸机上 kubevirt 的对比。

**标签**: `#Kubernetes`, `#Oxide`, `#Cloud-Controller-Manager`, `#ClusterAPI`, `#Infrastructure`

---

<a id="item-8"></a>
## [特朗普签署备忘录，允许私企开展美国支持的进攻性网络行动](https://www.bloomberg.com/news/articles/2026-08-13/trump-enlists-private-sector-to-boost-cyber-offensive-arsenal) ⭐️ 8.0/10

特朗普总统签署备忘录，允许受联邦政府监督的私营企业在海外开展监控和网络攻击，以打击针对美国人的跨国网络犯罪组织。国土安全部将负责运营该项目，并与司法部协调监督。 这标志着政策上的重大转变，将私营部门的角色扩大到国家许可的进攻性网络行动中。此举可能重塑政府监控和网络安全的规范，引发关于问责制以及企业参与国家安全的边界的质疑。 参与企业须维持至少 100 万美元的保证金或托管款，如不遵守合同约定，该款项将被没收。国土安全部将负责运行该项目，并与司法部协调监督。

telegram · zaihuapd · Aug 13, 05:10

**背景**: 传统上，针对外国犯罪组织的进攻性网络行动属于美国情报和军事机构的职权范围。这份备忘录似乎将这一权力扩展至私营企业，使其处于联邦政府的直接控制和监督之下。要求 100 万美元保证金表明存在财务问责机制，但公告中并未详细说明允许采取的行动范围。

**标签**: `#cybersecurity`, `#surveillance`, `#policy`, `#private sector`, `#US government`

---

<a id="item-9"></a>
## [DeepMind 发布手语转文字模型 SL2T，首次落地 Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

谷歌 DeepMind 发布了大规模多语言手语转文字模型 SL2T，并首次将其部署到消费产品中，在 Pixel 11 的 Gboard 和 Live Transcribe 上上线。初期支持美国手语转英语，后续将扩展到更多语言和设备。 这是无障碍技术领域的重大突破，标志着手语 AI 首次进入日常消费设备。它能让聋人和听障用户通过手语完成输入文字、搜索网页和获取实时字幕等操作，同时推动无障碍技术和 NLP 研究的更广泛创新。 该模型使用超过 10 万小时、涵盖 50 多种手语的数据训练，在 FLEURS-ASL 基准上的零样本 BLEURT 得分达到 70，远超此前纪录。为保护隐私，它只处理手部和身体姿态关键点，而不读取原始视频。

telegram · zaihuapd · Aug 13, 08:55

**背景**: 手语翻译因缺乏大型数据集以及手语固有的视觉连续特性而极具挑战。FLEURS-ASL 将 FLORES/FLEURS 多语言基准扩展到美国手语（以视频形式呈现），BLEURT 则是一种基于参考文本的神经评估指标，用于衡量生成文本与人工标注参考的匹配程度。DeepMind 的 SL2T 借助这些资源训练模型，使其能够零样本泛化到未见过的其他手语。在设备端部署要求高效性，而基于姿态关键点的方法有助于保持处理过程轻量和私密。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/">Putting sign language AI into users’ hands — Google DeepMind</a></li>
<li><a href="https://datanorth.ai/news/google-deepmind-releases-sl2t">Google DeepMind releases SL2T sign language AI - DataNorth</a></li>
<li><a href="https://arxiv.org/abs/2408.13585">[2408.13585] FLEURS-ASL: Including American Sign Language in Massively Multilingual Multitask Evaluation</a></li>

</ul>
</details>

**标签**: `#sign language`, `#AI translation`, `#accessibility`, `#DeepMind`, `#consumer AI`

---

<a id="item-10"></a>
## [谷歌发布 Gemini 3.6 Flash，透露 Gemini 4 已启动预训练](https://t.me/zaihuapd/43177) ⭐️ 8.0/10

谷歌发布了 Gemini 3.6 Flash，新模型相比 Gemini 3.5 Flash 将输出 Token 减少 17%，并用更少的推理步骤和工具调用完成多步任务。谷歌还透露，Gemini 4 的预训练已经启动。 此次发布表明谷歌持续降低大模型推理成本和延迟，以支持实际场景中的智能体应用，对基于 Gemini API 进行开发的开发者和企业具有直接影响。提前透露 Gemini 4 预训练则预示下一代大模型的到来，也加剧了与 OpenAI 和 Anthropic 的竞争。 Gemini 3.6 Flash 的知识截止日期更新至 2026 年 3 月，API 定价为每百万输入 Token 1.5 美元、每百万输出 Token 7.5 美元。谷歌还面向高吞吐、低延迟场景提供 Gemini 3.5 Flash。

telegram · zaihuapd · Aug 13, 17:32

**背景**: 工具调用（tool calling）允许大语言模型调用外部函数和 API，而不仅仅是生成文本，这是自动化工作流和完成多步任务的关键能力。知识截止日期（knowledge cutoff）定义了模型在训练之后没有数据的时点，更新到 2026 年 3 月意味着模型掌握了更近期的信息。计算机操作（computer use）指 AI 通过与人相同的界面（如查看截图并点击）来操作软件，谷歌及其他实验室正日益将这一能力内建到模型中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/tool-calling">What Is Tool Calling? | IBM</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_cutoff">Knowledge cutoff - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/news/developing-computer-use">Developing a computer use model \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI`, `#Google`, `#Gemini`, `#LLM`, `#API`

---

<a id="item-11"></a>
## [X 开源排名算法，新增工具让用户自查是否被隐形限制](https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/) ⭐️ 8.0/10

X 扩大了开源范围，在 GitHub 上以 Apache 2.0 许可证发布了“为你推荐”核心排名引擎，代码规模约为此前版本的 10 至 15 倍。该公司还在设置中推出了透明度工具，符合条件的用户可以下载 JSON 文件，查看自己的账号或帖子是否被排名系统标记。 此举是算法问责方面的重要一步，用户可以借此了解自己是否被隐形限制（shadowban），以及内容是如何被排序的。但由于并非所有组件都已公开，对完全透明的影响仍然有限，可能仍会引发批评。 该透明度工具最初向注册满一年、且近一个月发帖至少 10 次的测试用户开放。值得注意的是，部分用于判断违规内容的 Grok 系统未包含在开源范围内，而排名引擎本身使用 transformer 模型对帖子进行排序。

telegram · zaihuapd · Aug 14, 01:03

**背景**: X 的“为你推荐”信息流由排名算法驱动，该算法基于多种输入过滤内容，并使用 transformer 模型（一种广泛用于现代 AI 的神经网络）对帖子进行排序。隐形限制（shadowban）指在用户不知情的情况下悄悄限制其内容的可见性，长期以来一直是社交平台用户关注的焦点。X 曾在 2023 年开源过部分算法，此次发布是对这一努力的扩展。Grok 是 xAI 的 AI 模型系列，X 已将其整合到平台中用于内容相关流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/xai-org/x-algorithm">GitHub - xai-org/x-algorithm: Algorithm powering the For You feed on X · GitHub</a></li>
<li><a href="https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/">X open sources its ranking algorithm, letting users see if they've been 'shadowbanned' | TechCrunch</a></li>
<li><a href="https://adlibrary.com/guides/x-twitter-algorithm-explained">X (Twitter) Algorithm Explained 2026: How For You Ranks Posts</a></li>

</ul>
</details>

**标签**: `#open-source`, `#algorithm`, `#transparency`, `#social-media`, `#ranking`

---