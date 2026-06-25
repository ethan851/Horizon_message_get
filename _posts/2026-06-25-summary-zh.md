---
layout: default
title: "Horizon Summary: 2026-06-25 (ZH)"
date: 2026-06-25
lang: zh
---

> From 29 items, 9 important content pieces were selected

---

1. [OpenAI 与博通联手推出首款定制推理芯片 Jalapeño](#item-1) ⭐️ 9.0/10
2. [高通以 40 亿美元收购 AI 初创公司 Modular](#item-2) ⭐️ 9.0/10
3. [Anthropic 指控阿里巴巴对 Claude 发动大规模蒸馏攻击](#item-3) ⭐️ 9.0/10
4. [NVIDIA 45°C 液冷设计大幅降低数据中心用水](#item-4) ⭐️ 8.0/10
5. [Nub：为 Node.js 带来类 Bun 的开发体验](#item-5) ⭐️ 8.0/10
6. [使用生成式 AI 或导致中国学生考试成绩下降](#item-6) ⭐️ 8.0/10
7. [台积电先进制程代工全线涨价 5-10%](#item-7) ⭐️ 8.0/10
8. [美光 26Q3 营收暴增 346%，净利润 282.4 亿美元](#item-8) ⭐️ 8.0/10
9. [谷歌 Play Store 下周在美英欧启用外部计费](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 与博通联手推出首款定制推理芯片 Jalapeño](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI 宣布推出首款定制推理芯片，代号 Jalapeño，与博通合作设计，由台积电制造，开发过程借助 OpenAI 自身的模型加速。 这标志着 OpenAI 的重大战略转变，减少对英伟达 GPU 的依赖，实现大规模低成本推理，可能重塑 AI 硬件格局。 该芯片是专为运行已训练 AI 模型而设计的推理专用 ASIC，OpenAI 声称其模型助力从概念到量产仅用九个月完成设计。

hackernews · jamdesk · Jun 24, 17:47 · [社区讨论](https://news.ycombinator.com/item?id=48663324)

**背景**: 推理芯片是专门为执行训练后 AI 模型而优化的处理器，注重低延迟和高吞吐量。OpenAI 过去主要依赖英伟达 GPU 进行训练和推理，但谷歌 TPU 等定制芯片已展示出显著效率优势。博通是为大型科技公司设计定制 AI ASIC 的领先企业。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://naddod.medium.com/inference-chip-guide-the-foundation-of-scalable-ai-applications-d18f2c22b36c">Inference Chip Guide: The Foundation of Scalable AI Applications | by NADDOD | Medium</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/custom-ai-asics-examined-from-broadcom-to-mtia">The custom AI ASIC state of play (May 2026) — Broadcom deals ...</a></li>
<li><a href="https://tech-insider.org/broadcom-ai-revenue-custom-chips-2026/">Broadcom AI Revenue Surges 106%: Custom Chip Strategy 2026</a></li>

</ul>
</details>

**社区讨论**: 评论者对 AI 加速芯片设计的说法表示怀疑，认为这可能是模糊的营销。还讨论了将权重烧入硅片以实现极高吞吐量的替代方案，以及与谷歌 TPU 等其他定制芯片的比较。

**标签**: `#AI hardware`, `#OpenAI`, `#custom chip`, `#inference`, `#Broadcom`

---

<a id="item-2"></a>
## [高通以 40 亿美元收购 AI 初创公司 Modular](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 9.0/10

2026 年 6 月 24 日，高通宣布以 40 亿美元收购 AI 初创公司 Modular，标志着其向移动芯片之外的 AI 计算领域迈出了重大一步。 此次收购表明高通进军 AI 硬件-软件栈的雄心，通过将 Modular 的 Mojo 语言和基于 MLIR 的编译器技术整合到其产品组合中，可能挑战 NVIDIA 的主导地位。 Modular 以开发 Mojo（一种为 AI 工作负载优化的类 Python 编程语言）而闻名，此前已融资 2.5 亿美元。该交易预计于 2026 年底完成，尚待监管批准。

hackernews · timmyd · Jun 24, 13:49 · [社区讨论](https://news.ycombinator.com/item?id=48659798)

**背景**: Mojo 是一种专有编程语言，结合了 Python 的易用性与 C++、Rust 等系统语言的性能，利用 MLIR 编译器框架支持 CPU、GPU 及其他加速器。Modular 由前苹果和谷歌工程师（包括 LLVM 和 Swift 的创建者 Chris Lattner）于 2022 年创立。此次收购符合高通从移动芯片向 AI 推理和边缘计算领域多元化发展的战略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人质疑战略契合度，指出高通在高端 AI 训练领域存在感有限；也有人认为这是向 RISC-V 和 AI 竞争力迈出的大胆一步。还有人担忧 Mojo 在硬件公司旗下的开源前景。

**标签**: `#Acquisition`, `#AI Infrastructure`, `#Qualcomm`, `#Mojo`, `#Hardware`

---

<a id="item-3"></a>
## [Anthropic 指控阿里巴巴对 Claude 发动大规模蒸馏攻击](https://www.cnbc.com/2026/06/24/anthropic-alibaba-distillation-campaign.html) ⭐️ 9.0/10

Anthropic 正式指控阿里巴巴发动大规模蒸馏攻击，利用近 2.5 万个欺诈账户，在 2026 年 4 月 22 日至 6 月 5 日期间与 Claude 进行了超过 2880 万次交互，试图窃取模型能力。 这是针对 Anthropic 已知最大规模的蒸馏攻击，凸显了美中 AI 竞争加剧，引发对知识产权盗窃和国家安全的严重担忧。 Anthropic 于 6 月 10 日致信美国参议院银行委员会，指控阿里巴巴及其 Qwen AI 实验室参与攻击。攻击发生之际，美国限制了 Anthropic 的 Mythos 和 Fable 模型出口，阿里巴巴也被列入五角大楼的“中国军事公司”清单。

telegram · zaihuapd · Jun 25, 01:36

**背景**: 模型蒸馏是一种技术，较弱的模型通过学习更强模型的输出来以更低成本复制其能力。白宫此前曾指责中国窃取美国 AI 知识产权，蒸馏攻击已被视为美中 AI 竞争中的国家安全问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/research/mythos-preview">Assessing Claude Mythos Preview’s cybersecurity capabilities</a></li>
<li><a href="https://www.iiss.org/online-analysis/cyber-power-matrix/2026/05/ai-distillation-attacks-in-the-uschina-contest/">AI distillation attacks in the US–China contest - iiss.org</a></li>

</ul>
</details>

**标签**: `#AI安全`, `#模型蒸馏`, `#Anthropic`, `#阿里巴巴`, `#知识产权`

---

<a id="item-4"></a>
## [NVIDIA 45°C 液冷设计大幅降低数据中心用水](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 8.0/10

NVIDIA 为其即将推出的 Rubin 世代 AI 服务器宣布了一种新的 45°C 液冷架构，消除了蒸发冷却的用水需求，在保持高效率的同时实现了近乎零的水消耗。 该设计解决了 AI 数据中心日益增长的水足迹问题，每个 50MW 设施每年可为运营商节省超过 400 万美元，并为可持续 AI 基础设施树立了新标准。 该冷却系统以 45°C 的冷却液运行，实现了零风扇和 100%液冷，所有构建 Rubin 基础设施的云提供商都必须采用。量产计划于 2026 年秋季开始。

hackernews · nitin_flanker · Jun 24, 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48660178)

**背景**: 数据中心传统上使用空调或蒸发冷却，消耗大量水和能源。液冷使用冷却液直接从芯片带走热量，将冷却液温度提高到 45°C 可以更有效地将热量排放到环境中，减少或消除对耗水冷却塔的需求。这是行业向节水设计发展的趋势之一，微软也宣布了零水蒸发冷却。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techstory.in/the-45c-breakthrough-nvidias-liquid-cooling-architecture-solves-data-center-water-crisis/">NVIDIA Liquid Cooling Design Cuts Water to Near Zero - TechStory</a></li>
<li><a href="https://icharles.com/articles/nvidia-rubin-45c-liquid-cooling-zero-water">NVIDIA Rubin: 45°C Cooling, Near-Zero Water - iCharles</a></li>

</ul>
</details>

**社区讨论**: 评论中有人质疑该方法的创新性，指出更高温度冷却液已被使用过，并讨论了区域供热等协同效应。一些用户希望获得更多关于气候依赖性的细节，并分享了类似现有设施的例子。

**标签**: `#data center cooling`, `#liquid cooling`, `#energy efficiency`, `#AI infrastructure`, `#NVIDIA`

---

<a id="item-5"></a>
## [Nub：为 Node.js 带来类 Bun 的开发体验](https://github.com/nubjs/nub) ⭐️ 8.0/10

Colin McDonnell 发布了 Nub，这是一个针对 Node.js 的全能工具包，通过 --require 预加载钩子集成了基于 oxc 的转译器、polyfills 和模块解析钩子，模仿了 Bun 的开发体验。 Nub 显著提升了 Node.js 的开发者体验，提供了类似 Bun 的功能而无需离开 Node 生态系统，其作者（Zod 创建者、前 Bun 员工）的信誉增加了项目的可信度，可能影响 Node.js 工具链的未来发展。 Nub 使用 oxc 转译器作为 Node-API 插件以获得高性能，并为 Worker 和 Temporal 等现代 API 注入 polyfills。它运行在原生 Node.js 上，所有增强都是附加性的。

hackernews · colinmcd · Jun 24, 14:14 · [社区讨论](https://news.ycombinator.com/item?id=48660267)

**背景**: Bun 是一个快速的全能 JavaScript 运行时，内置转译和打包功能，但与 Node.js 不兼容。Nub 通过拦截模块加载并添加缺失的 API，在 Node.js 内提供了类似的便利。oxc 转译器是一个用 Rust 编写的高性能 JavaScript/TypeScript 工具链。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Temporal">Temporal - JavaScript | MDN</a></li>
<li><a href="https://repositorystats.com/topic/transpiler">Statistics for the Github transpiler topic - RepositoryStats</a></li>

</ul>
</details>

**社区讨论**: 社区反馈积极：一位用户成功迁移了整个 monorepo 且零问题，称赞其速度。其他人讨论了 --require 与 --import 的使用以及 ESM 支持等技术细节，作者澄清 Nub 使用了预加载钩子。

**标签**: `#nodejs`, `#developer-experience`, `#tooling`, `#typescript`, `#bun`

---

<a id="item-6"></a>
## [使用生成式 AI 或导致中国学生考试成绩下降](https://cepr.org/publications/dp21577) ⭐️ 8.0/10

一项针对 26,811 名中国 7 至 12 年级学生、持续 30 个月的追踪研究发现，使用生成式 AI 虽让作业成绩平均提高 18%、完成时间减少 30%，却导致高风险考试成绩在两年内下降 18%至 24%。 这是首次通过大规模、长期追踪实证研究表明，生成式 AI 在短期内提升作业表现的同时，可能损害真实的学业成绩。这对 AI 对学习和评估的影响，特别是在高风险教育体系中，提出了关键问题。 负面效应在社会科学科目中最为显著，其次是理工科和语言学科；低年级、高成就学生和男生受影响更大。约 80%的 AI 用户表现出“作业外包”特征——作业时间极短但分数高，这些学生承担了主要的成绩损失。

telegram · zaihuapd · Jun 24, 05:15

**背景**: 像 ChatGPT 等生成式 AI 工具已广泛被学生使用。虽然它们能帮助完成作业，但可能会造成虚假的掌握感，因为学生依赖 AI 而非发展自己的理解。这项由 CEPR 发表的研究对现实学业表现进行了多年追踪，提供了证据表明在作业中使用 AI 并不能转化为更好的考试成绩。

**标签**: `#AI`, `#education`, `#research`, `#China`, `#academic performance`

---

<a id="item-7"></a>
## [台积电先进制程代工全线涨价 5-10%](https://36kr.com/newsflashes/3866472254411779) ⭐️ 8.0/10

台积电已通知客户，将在 7nm 及以下所有先进制程上涨价 5%至 10%，这一调整影响约 75%的晶圆营收。 此次涨价将直接影响苹果、英伟达、AMD 等主要芯片设计商，可能推高各类电子产品的成本，并加速整个行业的价格调整。 涨价范围不仅包括 3nm 制程，还扩展到 5nm 和 7nm 等所有先进节点，整体涨幅为 5%至 10%，影响约 75%的晶圆营收来源。

telegram · zaihuapd · Jun 24, 05:45

**背景**: 台积电是全球最大的专业半导体代工厂，为众多领先公司制造芯片。7nm 及以下的先进制程对于高性能计算和移动设备至关重要。近年来，芯片行业面临供应限制和成本上升。

**标签**: `#TSMC`, `#semiconductor`, `#manufacturing`, `#pricing`, `#chip shortage`

---

<a id="item-8"></a>
## [美光 26Q3 营收暴增 346%，净利润 282.4 亿美元](https://www.globenewswire.com/news-release/2026/06/24/3317151/14450/en/micron-technology-inc-reports-record-results-for-the-third-quarter-of-fiscal-2026.html) ⭐️ 8.0/10

美光科技发布 2026 财年第三季度财报，营收达 414.6 亿美元，同比暴增 346%，净利润 282.4 亿美元（相当于每天净赚 3.1 亿美元），主要受 AI 基础设施对 HBM4 等高性能内存的强劲需求推动。 这一创纪录业绩凸显了 AI 如何从根本上重塑内存行业：内存厂商赚取巨额利润，而消费市场面临短缺。该结果预示着被称为“内存末日”的内存供应紧张将持续影响全球供应链和定价多年。 美光数据中心部门营收同比暴增 653%至 1152 亿美元，公司已大规模量产 HBM4 内存，HBM4E 计划于 2027 年投产。毛利率飙升至 84.9%，并签署了 16 份长期战略协议以锁定未来订单。

telegram · zaihuapd · Jun 24, 22:22

**背景**: 自 2025 年起，全球电脑内存短缺（被称为“RAMmageddon”）主要是由于制造商将产能从普通 DRAM 转向用于 AI 数据中心的高利润产品（如高带宽内存 HBM）。HBM 是一种 3D 堆叠 DRAM 技术，为 AI 加速器提供超高带宽和能效。根据 2026 年 Kearney 分析，这种短缺预计至少持续到 2030 年。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HBM_memory_shortage">HBM memory shortage</a></li>
<li><a href="https://semiengineering.com/hbm4e-raises-the-bar-for-ai-memory-bandwidth/">HBM4E Raises The Bar For AI Memory Bandwidth</a></li>

</ul>
</details>

**标签**: `#Micron`, `#Memory`, `#AI`, `#Earnings`, `#Semiconductor`

---

<a id="item-9"></a>
## [谷歌 Play Store 下周在美英欧启用外部计费](https://android-developers.googleblog.com/2026/06/play-expanded-billing.html) ⭐️ 8.0/10

谷歌宣布自 2026 年 6 月 30 日起，允许美国、英国和欧洲经济区的开发者提供第三方应用内计费或通过外部网页链接完成购买，并采用新的费率结构，将服务费与结算费拆分。 这是 Google Play 外部计费的最大规模开放，为开发者提供了更多支付灵活性和潜在的低成本，同时影响谷歌的收入模式及更广泛的应用商店经济。 新结构对首 100 万美元年收入和自动续订订阅收取 10%服务费，使用 Google Play Billing 的交易额外加收 5%结算费；替代计费或外部链接则不适用该 5%结算费。参与 Level Up 或 Apps Experience 计划的开发者从 9 月起还将享受更低费率。

telegram · zaihuapd · Jun 25, 02:33

**背景**: 应用商店通常要求开发者使用自己的计费系统并支付佣金（通常为 15-30%）。外部计费在全球范围内是一个有争议的问题，欧盟等监管机构一直在推动更多开放性。谷歌此前在有限区域进行了小规模外部计费试点；此次扩展到主要市场是一项重大的政策转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://9to5google.com/2026/06/24/google-play-store-external-billing-june-30/">Google Play Store opens external billing starting June 30</a></li>
<li><a href="https://www.androidheadlines.com/2026/06/google-play-store-external-billing-fee-changes.html">Google Play Store Opens Up to External Billing Options</a></li>
<li><a href="https://support.google.com/googleplay/android-developer/answer/10281818?hl=en">Understanding Google Play’s Payments policy</a></li>

</ul>
</details>

**标签**: `#Google Play`, `#billing`, `#app store`, `#policy`, `#developer`

---