---
layout: default
title: "Horizon Summary: 2026-07-04 (ZH)"
date: 2026-07-04
lang: zh
---

> From 43 items, 13 important content pieces were selected

---

1. [Anthropic 指控阿里巴巴对 Claude 发动大规模蒸馏攻击](#item-1) ⭐️ 9.0/10
2. [本地 SOTA 大模型指南引发成本与云服务辩论](#item-2) ⭐️ 8.0/10
3. [欧洲议会议员遭 Pegasus 间谍软件入侵](#item-3) ⭐️ 8.0/10
4. [Wordgard：ProseMirror 创建者推出的新富文本编辑器](#item-4) ⭐️ 8.0/10
5. [PostgreSQL 与 OOM 杀手：为何启用严格内存过度分配？](#item-5) ⭐️ 8.0/10
6. [Current AI 发布开源 AI 差距地图，索引 421 个产品](#item-6) ⭐️ 8.0/10
7. [谷歌 Gemini Omni Flash 登顶视频生成盲测榜](#item-7) ⭐️ 8.0/10
8. [Claude Fable 5 重新上线：安全过度与配额缩减引发开发者不满](#item-8) ⭐️ 8.0/10
9. [华为 Atlas 350 加速卡搭载昇腾 950PR，性能宣称达 H20 的 2.87 倍](#item-9) ⭐️ 8.0/10
10. [中国拟注销半年未登录账号，强制标注 AI 内容](#item-10) ⭐️ 8.0/10
11. [华为 Mate 80 Pro 凭借鸿蒙优化游戏能效超越骁龙 8 Gen3](#item-11) ⭐️ 8.0/10
12. [NASA 发射私人 LINK 航天器救援雨燕望远镜](#item-12) ⭐️ 8.0/10
13. [腾讯玄武实验室阿图因 AI 在 CyberGym 测试中超越 Mythos](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic 指控阿里巴巴对 Claude 发动大规模蒸馏攻击](https://t.me/zaihuapd/42327) ⭐️ 9.0/10

Anthropic 指控阿里巴巴策划了一场大规模的蒸馏攻击，利用近 2.5 万个欺诈账户，在 2026 年 4 月 22 日至 6 月 5 日期间通过超过 2880 万次交互，窃取其 Claude AI 模型的能力。Anthropic 称这是针对该公司已知的最大规模蒸馏攻击。 这一指控凸显了在人工智能知识产权和国家安全方面日益紧张的局势，因为蒸馏攻击使外国实体能够在未经授权的情况下复制先进的 AI 能力。如果被证实，可能加剧中美科技冲突，并导致对 AI 模型实施更严格的出口管制。 Anthropic 表示，阿里巴巴及其 Qwen 实验室参与了此次攻击，通过系统性地查询 Claude 来提取知识，以训练竞争模型。该公司已致信美国参议院银行委员会，详细说明了这一涉嫌违规行为。

telegram · zaihuapd · Jul 3, 06:21

**背景**: 模型蒸馏是一种技术，较小、能力较弱的模型（学生）通过训练教师模型的输出来学习较大、能力更强的模型（教师）的知识。在未经授权的情况下对专有模型进行蒸馏被视为知识产权盗窃。Anthropic 此前曾警告此类攻击会破坏美国对 AI 技术的出口管制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI安全`, `#知识产权`, `#模型蒸馏`, `#Anthropic`, `#阿里巴巴`

---

<a id="item-2"></a>
## [本地 SOTA 大模型指南引发成本与云服务辩论](https://github.com/jamesob/local-llm) ⭐️ 8.0/10

Jamesob 发布了一份指南，介绍如何构建一个约 4 万美元的高端本地大模型系统，使用四块 GPU 和一个经过裁剪和量化的 GLM-5.2 版本，但社区评论指出，这种本地部署在成本和性能上仍然远不如云订阅服务。 这一讨论凸显了本地 SOTA 大模型对大多数用户而言的不实用性，因为云服务以极低的硬件成本提供了相近的智能水平，从而促使人们将目光转向混合或中端本地解决方案。 该方案实际成本约为 5 万至 5.5 万美元，而非声称的 4 万美元，并使用了经过 REAP 裁剪（移除约 22%专家）、Int8 混合 NVFP4 量化的 GLM-5.2 模型（约 594B 参数）；社区成员建议更便宜的替代方案，如总共 3000 美元的两块 RTX 3090。

hackernews · livestyle · Jul 3, 15:03 · [社区讨论](https://news.ycombinator.com/item?id=48775921)

**背景**: 在本地运行最先进的大语言模型需要大量的显存和算力，通常需要多 GPU 配置以及裁剪和量化等模型压缩技术。云服务如 Claude Opus 和 GPT-4 通过月费提供便捷的类似能力，使得本地部署对个人来说在经济上具有挑战性。

**社区讨论**: 社区观点不一：许多评论者强调成本过高，指出 4 万美元相当于超过 16 年的 Claude Opus 订阅费用，而另一些人则提出中间方案，如使用 128GB 统一内存系统运行 DeepSeek V4。然而，关于本地部署中的量化质量和模型安全性仍存在担忧。

**标签**: `#LLM`, `#local inference`, `#hardware`, `#deep learning`, `#community discussion`

---

<a id="item-3"></a>
## [欧洲议会议员遭 Pegasus 间谍软件入侵](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

公民实验室确认，欧洲议会间谍软件调查委员会成员斯泰利奥斯·库洛格卢在 2022 年和 2023 年多次被 NSO 集团的 Pegasus 间谍软件成功感染。 此次入侵表明国家支持的间谍活动针对欧盟议会监督机构，破坏了民主机构和民选代表的安全。 感染发生于 2022 年 10 月 21 日和 2023 年 3 月 6 日至 7 日，首次感染与已知的针对欧洲俄语和白俄语流亡记者的 Pegasus 行动重叠。

hackernews · ledoge · Jul 3, 20:38 · [社区讨论](https://news.ycombinator.com/item?id=48779683)

**背景**: Pegasus 是以色列公司 NSO 集团开发的强大间谍软件，能够远程入侵移动设备，访问信息、通话和摄像头。该软件被各国政府广泛用于监视记者、活动家和政客。多伦多大学的公民实验室专门检测和分析此类威胁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，调查间谍软件的欧洲议会议员被入侵具有讽刺意味，并讨论了希腊、意大利等欧盟成员国对 Pegasus 的滥用情况。一些人指出议会中个人设备与工作设备缺乏分离。

**标签**: `#cybersecurity`, `#spyware`, `#Pegasus`, `#European Parliament`, `#espionage`

---

<a id="item-4"></a>
## [Wordgard：ProseMirror 创建者推出的新富文本编辑器](https://wordgard.net/) ⭐️ 8.0/10

ProseMirror 的创建者 Marijn Haverbeke 发布了 Wordgard，这是一个新的浏览器内富文本编辑器框架，旨在改善开发者体验并解决与前代产品的设计差异。 Wordgard 代表了富文本编辑器生态系统的一次重大进步，提供了更对开发者友好的 API，并可能影响下一代的基于网页的编辑器，如 Tiptap 或 Obsidian。 Wordgard 不是自由形式的 HTML 编辑器，而是一个结构化内容编辑器，开发者可以控制支持的内容类型，并且从 ProseMirror 没有直接的升级路径，需要大量的迁移工作。

hackernews · indy · Jul 3, 08:50 · [社区讨论](https://news.ycombinator.com/item?id=48772573)

**背景**: ProseMirror 是许多富文本编辑器（包括 Tiptap）经过实战检验的核心基础，以其性能和灵活性著称，但学习曲线陡峭。Wordgard 是同一位作者的新框架，旨在提供更直观的 API 和更好的开发者体验，同时保留结构化文档编辑的核心概念。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wordgard.net/">Wordgard</a></li>
<li><a href="https://prosemirror.net/">ProseMirror</a></li>

</ul>
</details>

**社区讨论**: 社区普遍对 Wordgard 的设计和文档印象深刻，但担心缺乏从 ProseMirror 的升级路径，以及需要静态类型的文档表示。一些用户还表示，对于未能建立富文本编辑的网页标准感到沮丧。

**标签**: `#rich-text editor`, `#web development`, `#prosemirror`, `#javascript`, `#wordgard`

---

<a id="item-5"></a>
## [PostgreSQL 与 OOM 杀手：为何启用严格内存过度分配？](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud 基于其大规模运行 PostgreSQL 的经验，解释了为何对 PostgreSQL 使用 vm.overcommit_memory=2（严格过度分配）以防止 OOM 杀手问题。 此设置可通过防止 OOM 杀手杀死 PostgreSQL 进程来显著提高数据库工作负载的稳定性，但需谨慎测试，因为配置不当可能导致应用崩溃。 文章描述了三种过度分配模式：0（启发式）、1（始终过度分配）和 2（严格不进行过度分配）。模式 2 确保内存耗尽时分配立即失败，这对 PostgreSQL 更安全，但可能破坏依赖过度分配的应用程序。

hackernews · furkansahin · Jul 3, 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48774509)

**背景**: Linux 内核的 OOM（内存不足）杀手是一种在系统内存耗尽时杀死进程的机制。内存过度分配允许分配超出物理 RAM 的虚拟内存，这可能导致 OOM 情况。作为数据库的 PostgreSQL 受益于严格模式以避免意外杀死。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rakeshjain-devops.medium.com/linux-out-of-memory-killer-31e477a45759">Linux Out-Of-Memory Killer . What is this ? | by Rakesh Jain | Medium</a></li>
<li><a href="https://www.linkedin.com/pulse/vmovercommitmemory-sanju-debnath">vm.overcommit_memory</a></li>
<li><a href="https://ssup2.github.io/blog-software/en/docs/theory-analysis/linux-oom-killer/">Linux OOM Killer – ssup2 Blog / Software</a></li>

</ul>
</details>

**社区讨论**: 社区讨论中包含用户对严格过度分配潜在副作用的警告，如阻止 fork。作者承认文章语气可能过于强烈，并指出严格过度分配可能不适用于所有场景。

**标签**: `#PostgreSQL`, `#memory management`, `#OOM killer`, `#Linux`, `#database administration`

---

<a id="item-6"></a>
## [Current AI 发布开源 AI 差距地图，索引 421 个产品](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

非营利组织 Current AI 发布了其开源 AI 差距地图 v0.1，这是一份包含 421 个开源 AI 产品的详细目录——包括 266 个软件工具、85 个模型、50 个数据集和 20 个硬件项目——来自 228 个组织，并将基础数据以 MIT 许可证发布在 GitHub 上。 该地图提供了开源 AI 生态系统的全面结构化概览，帮助研究人员、开发者和资助者识别差距与机遇。凭借 4 亿美元的已承诺资金支持，它可能加速开源 AI 的采用并为战略投资提供信息。 该地图按三个堆栈层（模型组件、产品/用户体验和基础设施）分为 14 个类别。另有 24,400 个工件属于未分类的长尾，在研究和引用之前不会评分。

rss · Simon Willison · Jul 3, 22:04

**背景**: Current AI 是一个全球性非营利合作伙伴关系，于 2025 年 2 月在巴黎 AI 行动峰会上成立。差距地图旨在系统性地索引开源 AI 领域，此前这一领域缺乏统一目录。数据以 1,184 个 YAML 文件形式托管在 GitHub 上，支持通过 Datasette Lite 等工具进行探索。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/jul/3/open-source-ai-gap-map/">Open Source AI Gap Map | Simon Willison’s Weblog</a></li>
<li><a href="https://blog.jarv.tech/p/open-source-ai-gap-map-masshtabnaya-karta-ekosistemy-beea18396340c774">Open Source AI Gap Map : масштабная карта... — blog.jarv.tech</a></li>

</ul>
</details>

**标签**: `#open source`, `#AI`, `#ecosystem mapping`, `#nonprofit`, `#tools`

---

<a id="item-7"></a>
## [谷歌 Gemini Omni Flash 登顶视频生成盲测榜](https://x.com/Designarena/status/2072759122366509130) ⭐️ 8.0/10

谷歌 DeepMind 的视频生成模型 Gemini Omni Flash 在 Video Arena 盲测中以 1404 分登顶榜首，领先字节跳动的 Seedance 2.0 Mini 达 101 分。 这标志着 AI 视频生成领域的重大突破，展示了谷歌在字节跳动 Seedance 系列主导的竞争格局中重获领先地位的能力。该结果凸显了多模态 AI 模型创新的迅猛速度。 Gemini Omni Flash 是基于 Transformer 的多模态模型，支持文本、视觉、视频和音频输入，当前视频输出上限为 10 秒。基于用户盲测投票，谷歌的视频模型排名较之前的 Veo 系列提升了 7 位。

telegram · zaihuapd · Jul 3, 05:51

**背景**: Video Arena 是一个众包盲测基准，用户在不知道模型身份的情况下比较 AI 生成的视频，从而提供无偏见的质量评估。Gemini Omni Flash 是谷歌于 2026 年 5 月推出的 Gemini Omni 系列模型之一，专注于真实物理和对话式视频编辑。字节跳动的 Seedance 2.0 Mini 此前以 1303 分位居榜首。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.madebyagents.com/benchmarks/video-arena">Video Arena Benchmark : Scores, Methodology, and Top AI Models</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-omni-flash/">Gemini Omni Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-omni/">Introducing Gemini Omni</a></li>

</ul>
</details>

**标签**: `#AI`, `#video generation`, `#Google DeepMind`, `#model benchmarking`, `#computer vision`

---

<a id="item-8"></a>
## [Claude Fable 5 重新上线：安全过度与配额缩减引发开发者不满](https://www.bleepingcomputer.com/news/artificial-intelligence/claude-fable-relaunch-disappoints-users-with-nerfed-performance/) ⭐️ 8.0/10

美国解除出口管制后，Anthropic 的 Claude Fable 5 模型重新上线，但订阅用户在 7 月 7 日之前只能使用 50% 的调用额度，之后该模型将不再包含在订阅计划中。此外，过度的安全过滤器频繁误判，在处理包含“漏洞”、“hook”等关键词的 C/C++ 或 Rust 代码时，会自动将模型降级至 Opus 4.8。 此事件凸显了 AI 安全机制与开发者实际可用性之间日益激化的矛盾，可能削弱开发者对 Anthropic 部署实践的信任。若得不到解决，可能会促使开发者转向行为更可预测的竞品模型，影响 Anthropic 在开发者群体中的采用率。 据官方声明，使用限制是由于算力不足，待产能充足后会重新纳入订阅计划。API 和企业按量付费版本仍可完整调用 Fable 5，不会触发降级，但官方尚未出台针对安全误判的优化方案。

telegram · zaihuapd · Jul 3, 07:20

**背景**: Claude Fable 5 是 Anthropic 的旗舰“Mythos 级别”模型，专为复杂编程和知识工作设计。它最初发布后因美国对某些国家先进 AI 模型的出口管制而被限制，近期管制解除后重新上线。大语言模型中的安全过滤器旨在防止有害输出，但过高的阈值会干扰正常的开发工作，例如本次因安全相关关键词而触发误判降级。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-8">Introducing Claude Opus 4.8 \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#Claude`, `#Anthropic`, `#model deployment`, `#developer experience`

---

<a id="item-9"></a>
## [华为 Atlas 350 加速卡搭载昇腾 950PR，性能宣称达 H20 的 2.87 倍](https://t.me/zaihuapd/42329) ⭐️ 8.0/10

在 2026 年华为中国合作伙伴大会上，华为发布并开售搭载全新昇腾 950PR 处理器的 Atlas 350 加速卡，该卡支持 FP4 低精度推理，单卡算力宣称达到英伟达 H20 的 2.87 倍。 此次发布标志着华为在美国出口限制背景下对英伟达在中国 AI 芯片市场主导地位的最激进挑战。FP4 支持和高内存容量可能使本地大语言模型推理更加高效。 昇腾 950PR 提供 1.56 petaflops 的 FP4 性能，Atlas 350 配备 112GB HBM 内存，可单卡加载 70B 参数模型。华为计划在 2026 年出货 75 万颗该芯片。

telegram · zaihuapd · Jul 3, 08:35

**背景**: 昇腾 950PR 是华为最新的 AI 推理芯片，旨在美国出口管制限制英伟达先进 GPU 进入中国的情况下与其竞争。FP4（4 位浮点）是一种低精度格式，可降低 AI 模型的内存和计算需求，英伟达的 Blackwell 架构也支持类似的 FP4 格式 NVFP4。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huaweicentral.com/ascend-950pr-ai-chip-everything-you-need-to-know/">Ascend 950PR AI Chip: Everything you need to know - Huawei Central</a></li>
<li><a href="https://tech-insider.org/huawei-ascend-950pr-ai-chip-nvidia-china-2026/">Huawei Ascend 950PR: The 1.56 PFLOP AI Chip vs Nvidia [2026]</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#Huawei`, `#Ascend`, `#accelerator`, `#FP4`

---

<a id="item-10"></a>
## [中国拟注销半年未登录账号，强制标注 AI 内容](https://mp.weixin.qq.com/s/TfYZaC8ULPvu9JeTqYGkKg) ⭐️ 8.0/10

2025 年 7 月 3 日，国家互联网信息办公室发布《互联网信息服务管理办法（修订草案征求意见稿）》，拟允许平台注销超过 6 个月未登录的账号，并要求对 AI 生成内容进行标识。 该法规将深刻影响中国的用户数据管理和平台合规，解决闲置账号的隐私问题以及 AI 生成内容的透明度问题，涉及数十亿用户和各大科技公司。 草案还要求平台支持解绑原手机号，禁止刷量、操纵热搜等虚假互动行为，并规定大型平台须在 24 小时内处理违法和不良信息投诉。

telegram · zaihuapd · Jul 3, 11:29

**背景**: 中国近年来加强互联网治理，出台了数据安全法和个人信息保护法。本次草案更新了 2011 年的《互联网信息服务管理办法》，以应对 AI 生成内容和账号安全等新挑战，并与全球合成媒体标识趋势保持一致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.auditsocials.com/blog/cross-platform-ai-content-labeling-requirements-2026-meta-google-tiktok-youtube-comparison">AI Content Label Rules 2026: Meta, Google, TikTok, YouTube</a></li>

</ul>
</details>

**标签**: `#Regulations`, `#Internet Policy`, `#AI Governance`, `#User Privacy`, `#Content Moderation`

---

<a id="item-11"></a>
## [华为 Mate 80 Pro 凭借鸿蒙优化游戏能效超越骁龙 8 Gen3](https://www.bilibili.com/video/BV1F7T46wEyT) ⭐️ 8.0/10

极客湾评测显示，搭载麒麟 9030 的华为 Mate 80 Pro Max 凭借原生鸿蒙优化和软硬芯云协同，在游戏能效上超越了骁龙 8 Gen3。 这表明深度的系统级优化可以弥补硬件劣势，可能重塑移动性能基准，并挑战传统芯片领导者的地位。 麒麟 9030 Pro 采用 9 核 14 线程 CPU 和 6 核马良 935 GPU，晶体管规模约 150 亿；虽然理论多核能效介于骁龙 8 Gen2 与 8 Gen3 之间，但实际游戏功耗更低——《原神》极高画质 60 帧仅 4.9W。

telegram · zaihuapd · Jul 3, 13:27

**背景**: 麒麟 9030 系列是华为最新的自研芯片，于 2025 年 11 月发布，采用 5nm 制程。鸿蒙原生应用旨在利用软硬芯云协同，实现更高效的任务调度和功耗管理。这种方法帮助华为在纸面硬件稍逊的情况下缩小了性能差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nanoreview.net/ru/soc/hisilicon-kirin-9030">HiSilicon Kirin 9030 Pro : характеристики, тесты в бенчмарках</a></li>
<li><a href="https://post.smzdm.com/p/aognpnz7/">鸿 蒙 原 生 APP...</a></li>
<li><a href="https://www.21jingji.com/article/20250904/herald/e1eec22c1785149ffafb68b13267b5f3.html">华为三折叠携麒麟9020亮相，折叠屏市场竞争迈向 软 硬 协 同 阶段 - 21...</a></li>

</ul>
</details>

**标签**: `#Huawei`, `#Kirin 9030`, `#HarmonyOS`, `#mobile performance`, `#chipset`

---

<a id="item-12"></a>
## [NASA 发射私人 LINK 航天器救援雨燕望远镜](https://apnews.com/article/swift-nasa-satellite-rescue-katalyst-a7ddd740ca099587c58865f583c7245a) ⭐️ 8.0/10

2026 年 7 月 3 日，NASA 发射了由 Katalyst Space Technologies 建造的 LINK 航天器，旨在提升老化的雨燕天文台的轨道，防止其即将失控再入大气层。 这项任务标志着私人航天器首次尝试捕获并维护美国政府的卫星，可能延长一颗已有 20 年历史的宝贵科学观测站的生命，并展示商业卫星维护能力。 LINK 航天器将使用机械臂抓住雨燕，然后通过推进器将望远镜轨道提升约 240 公里，如果成功，雨燕最快可在 2026 年 9 月恢复科学观测。

telegram · zaihuapd · Jul 3, 15:43

**背景**: 雨燕天文台于 2004 年发射，是一台伽马射线暴探测器，对天体物理学至关重要。由于太阳活动，其轨道持续下降，面临毁灭性再入的危险。卫星维护是一个新兴行业，这次任务可能为未来商业维护政府资产铺平道路。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LINK_spacecraft">LINK spacecraft</a></li>
<li><a href="https://www.nasa.gov/image-article/link-spacecraft-set-for-mission-to-boost-nasas-swift-observatory/">LINK Spacecraft Set for Mission to Boost NASA’s Swift Observatory - NASA</a></li>

</ul>
</details>

**标签**: `#space`, `#satellite servicing`, `#NASA`, `#astronomy`, `#orbital mechanics`

---

<a id="item-13"></a>
## [腾讯玄武实验室阿图因 AI 在 CyberGym 测试中超越 Mythos](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 8.0/10

腾讯玄武实验室的阿图因 AI 在加州大学伯克利分校主导的 CyberGym 网络安全基准测试中获得 84.0%的准确率，超越了 Anthropic 的 Claude Mythos Preview。 这表明开源模型能以不到 0.1%的成本超越领先的闭源系统，凸显了经济高效的 AI 驱动漏洞检测的潜力。 阿图因 AI 基于可本地部署的开源模型 GLM-5.1 构建，预算不到 Mythos 的 0.1%。它在 curl、gnark、OpenSSL、Python cryptography 和 Java bc-java 等项目中发现了多个 Mythos 未检出的高危漏洞，评分最高达 9.3。

telegram · zaihuapd · Jul 3, 16:12

**背景**: CyberGym 是加州大学伯克利分校开发的网络安全基准测试，评估 AI 代理发现和利用真实软件漏洞的能力。GLM-5.1 是 Z.AI 推出的旗舰模型，专为长时间自主任务设计，可持续工作长达 8 小时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://llm-stats.com/benchmarks/cybergym">CyberGym Benchmark Leaderboard | LLM Stats</a></li>
<li><a href="https://mcpbr.org/cybergym">CyberGym : Cybersecurity Exploit Generation Benchmark for... | mcpbr</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.1">GLM - 5 . 1 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#benchmark`, `#vulnerability detection`, `#open-source`

---