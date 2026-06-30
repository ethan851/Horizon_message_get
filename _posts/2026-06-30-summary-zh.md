---
layout: default
title: "Horizon Summary: 2026-06-30 (ZH)"
date: 2026-06-30
lang: zh
---

> From 30 items, 8 important content pieces were selected

---

1. [vLLM v0.24.0 发布：重大优化与新模型支持](#item-1) ⭐️ 9.0/10
2. [火箭实验室收购铱星，80 亿美元历史性交易](#item-2) ⭐️ 9.0/10
3. [最高法院：地理围栏搜查令需受宪法保护](#item-3) ⭐️ 9.0/10
4. [Game Boy JIT 编译为 WASM 超越原生解释器](#item-4) ⭐️ 8.0/10
5. [CUDA 内核启动的完整流程解析](#item-5) ⭐️ 8.0/10
6. [三星与 SK 海力士宣布创纪录的 AI 投资计划](#item-6) ⭐️ 8.0/10
7. [长鑫存储与腾讯签 30 亿美元 DRAM 供应协议](#item-7) ⭐️ 8.0/10
8. [特斯拉推送 FSD v14 Lite，HW3 车型获升级](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.24.0 发布：重大优化与新模型支持](https://github.com/vllm-project/vllm/releases/tag/v0.24.0) ⭐️ 9.0/10

vLLM 项目发布了 v0.24.0 版本，包含来自 256 位贡献者的 571 次提交，新增了对 MiniMax-M3 和 DeepSeek-V4 模型的支持，并进行了性能优化，例如 FlashInfer 稀疏索引缓存和 Model Runner V2 量化支持。 此版本显著提升了 vLLM（一个广泛使用的开源 LLM 推理引擎）的效率和通用性，使开发者在生产环境中部署大语言模型时获得更好的性能和更广泛的模型兼容性。 值得注意的技术改进包括 DeepSeek-V4 的 FlashInfer 稀疏索引缓存（TTFT 提升 2-4%）、MiniMax-M3 的 MXFP4 精度支持，以及用于低延迟稀疏注意力的集群协作 topK 内核。Model Runner V2 现在默认启用量化模型。

github · khluu · Jun 29, 19:41

**背景**: vLLM 是一个用于大语言模型的开源高性能推理引擎，旨在提供快速高效的模型服务。它利用 PagedAttention 和连续批处理等技术来优化吞吐量和内存使用。该项目支持多种模型和硬件后端，包括 NVIDIA 和 AMD GPU。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.flashinfer.ai/api/sparse.html">flashinfer.sparse - FlashInfer 0.6.13 documentation</a></li>
<li><a href="https://rocm.blogs.amd.com/artificial-intelligence/w4a6-quant-mm/README.html">MXFP6 and MXFP 4 Mixed Precision for Accelerating... — ROCm Blogs</a></li>
<li><a href="https://github.com/vllm-project/vllm/blob/main/csrc/libtorch_stable/cooperative_topk.cu">vllm/csrc/libtorch_stable/cooperative_topk.cu at main - GitHub</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#AI inference`, `#model serving`, `#LLM optimization`, `#open source`

---

<a id="item-2"></a>
## [火箭实验室收购铱星，80 亿美元历史性交易](https://investors.rocketlabcorp.com/news-releases/news-release-details/rocket-lab-acquire-iridium-historic-deal-creating-fully) ⭐️ 9.0/10

火箭实验室于 6 月 29 日宣布，将以现金加股票方式收购铱星通信公司，交易价值约 80 亿美元，每股作价 54 美元。该交易已获双方董事会一致批准，有待监管机构和铱星股东批准，预计 2027 年年中完成。 此次合并打造了一家完全集成的卫星和发射公司，将火箭实验室的发射和航天器制造能力与铱星的全球低轨卫星网络、L 波段频谱和 500 多家合作伙伴生态相结合。合并后的实体有望拓展卫星物联网、直连设备和 PNT 市场，类似于 SpaceX 利用星链确保基础发射量的模式。 铱星拥有超过 255 万活跃订阅者，2025 年营收 8.717 亿美元，运营 EBITDA 为 4.95 亿美元，利润率 57%。火箭实验室已获得 36 亿美元过桥贷款承诺以支持此次收购。该交易对铱星的企业估值约为 80 亿美元。

hackernews · everfrustrated · Jun 29, 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48719485)

**背景**: 火箭实验室是领先的发射服务提供商和卫星制造商，以电子火箭和即将推出的中子火箭而闻名。铱星运营着由 66 颗低轨卫星组成的星座，提供全球语音和数据服务，包括卫星电话和物联网连接。此次收购使火箭实验室能够拥有自己的卫星星座和频谱，确保稳定的发射需求，并减少对外部卫星客户的依赖。

**社区讨论**: 社区反应强调了与 SpaceX 星链模式的战略相似性，用户指出火箭实验室获得了有保障的发射基线和盈利的卫星业务。有人表达了对太空垃圾和低地球轨道商业化的环境担忧，而另一些人则称赞此举是对市场波动的明智对冲。Telegram 评论总结了交易的财务细节以及向物联网和 D2D 市场的战略拓展。

**标签**: `#space industry`, `#acquisition`, `#satellite communications`, `#Rocket Lab`, `#Iridium`

---

<a id="item-3"></a>
## [最高法院：地理围栏搜查令需受宪法保护](https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision) ⭐️ 9.0/10

2026 年 6 月 29 日，美国最高法院裁定，地理围栏搜查令构成第四修正案下的搜查行为，需要具备可能原因并取得搜查令。该裁决源于一起执法部门利用地理围栏搜查令从 Google 的 Sensorvault 获取位置数据以识别银行抢劫案嫌疑人的案件。 这一里程碑式的裁决为数字位置数据建立了宪法保护，对执法监控实践和隐私权产生重大影响。它确立了限制在没有个体化怀疑的情况下批量检索位置数据的先例，影响了全国警方如何使用地理围栏搜查令。 该案涉及一份地理围栏搜查令，指示 Google 提供在银行周围 150 米范围内、30 分钟窗口内的设备 ID，最初返回了 19 个账户。法院认为，此类搜查涉及合理的隐私期待，因为现代手机无处不在并持续追踪位置。

hackernews · cdrnsf · Jun 29, 15:54 · [社区讨论](https://news.ycombinator.com/item?id=48720924)

**背景**: 地理围栏搜查令，也称为反向位置搜查令，是一种命令像 Google 这样的公司识别在特定地理区域内、特定时间段内的所有移动设备的搜查令。与传统针对已知个人的搜查令不同，地理围栏搜查令通过位置数据识别未知嫌疑人。Google 的 Sensorvault 是一个存储已开启位置历史记录的用户历史位置数据的数据库。此类搜查令的广泛使用因其大规模监控的潜力以及此前要求的最低监督而引发了隐私担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geofence_warrant">Geofence warrant</a></li>
<li><a href="https://www.scotusblog.com/2026/06/court-rules-that-law-enforcements-use-of-geofence-warrant-was-a-search/">Court rules that law enforcement’s use of “geofence warrant ...</a></li>

</ul>
</details>

**社区讨论**: 评论者将地理围栏搜查令与窃听相提并论，指出数字监控缺乏历史上限制窃听滥用的物理资源约束。一些人强调了本案中的具体数据批次，即 Google 先提供设备 ID，然后是账户电子邮件地址，最后是订阅者信息。还有人提到了替代识别方法，例如如彼得雷乌斯丑闻中所示的将酒店宾客名单与 IP 地理定位进行交叉比对。总体而言，舆论支持该裁决，认为这是对不断扩大的监控权力的必要制衡。

**标签**: `#privacy`, `#law`, `#surveillance`, `#Supreme Court`, `#geofence`

---

<a id="item-4"></a>
## [Game Boy JIT 编译为 WASM 超越原生解释器](https://humphri.es/blog/WATaBoy/) ⭐️ 8.0/10

WATaBoy 是一个 Game Boy 模拟器，它通过即时（JIT）编译将 Game Boy 指令转换为 WebAssembly（WASM），性能超过了用 C 语言编写的原生解释器。 这种方法展示了一种新颖的方式，通过利用浏览器内 WebAssembly 的 JIT 能力，在限制原生 JIT 的平台上（如 iOS）实现高性能模拟。 JIT 编译器动态生成 WASM 模块，在基准测试中比原生解释器性能提升 25%；但发现 Firefox 比 Chrome 和 Safari 慢 25%。

hackernews · energeticbark · Jun 29, 15:02 · [社区讨论](https://news.ycombinator.com/item?id=48720190)

**背景**: JIT 编译在运行时将代码编译为本地机器码以加快执行速度，而解释器则直接执行指令而不编译。WebAssembly 是一种低级二进制格式，在现代浏览器中高效运行，它本身也可以由浏览器的 JavaScript 引擎进行 JIT 编译。

**社区讨论**: 评论者称赞该项目对本科生来说令人印象深刻，并指出 WASM 开销（约 20%）远低于解释器开销（约 1000%），因此结果符合预期。一些人讨论了 iOS 的 JIT 限制以及 JavaScript eval()等替代方法。

**标签**: `#JIT compilation`, `#WebAssembly`, `#Game Boy emulation`, `#JavaScript`, `#emulator performance`

---

<a id="item-5"></a>
## [CUDA 内核启动的完整流程解析](https://fergusfinn.com/blog/what-happens-when-you-run-a-gpu-kernel/) ⭐️ 8.0/10

一篇详细博客文章解释了从 CPU 触发 CUDA 内核到 GPU 执行的完整流水线，包括门铃机制和线程束调度。 这篇深度文章填补了 CUDA 开发者常见知识空白，阐明了内核启动从驱动到硬件执行的通常不透明的路径。 文章涵盖了向 GPU 提交工作的门铃机制、队列元数据(QMD)格式以及带有就绪条件的线程束调度，还介绍了默认 CUDA 流中命令的隐式同步。

hackernews · mezark · Jun 29, 13:11 · [社区讨论](https://news.ycombinator.com/item?id=48718863)

**背景**: 在 CUDA 中，内核是一个在 GPU 上并行运行的函数，涉及大量线程。线程被分组为线程束（通常 32 个线程），GPU 调度线程束执行。门铃机制是 CPU 通知 GPU 命令队列中有新工作的方式。线程束调度是 GPU 的线程束调度器在就绪的线程束之间快速切换以隐藏延迟的技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Thread_block_(CUDA_programming)">Thread block (CUDA programming) - Wikipedia</a></li>
<li><a href="https://modal.com/gpu-glossary/device-hardware/warp-scheduler">What is a Warp Scheduler? | GPU Glossary</a></li>

</ul>
</details>

**社区讨论**: 评论者们高度赞扬了文章的清晰度和深度，特别是门铃和 QMD 的解释。一位用户指出了与 Vulkan 显式同步的对比，另一位则推测了内核优化公司的未来。

**标签**: `#CUDA`, `#GPU`, `#kernel launch`, `#parallel computing`, `#systems`

---

<a id="item-6"></a>
## [三星与 SK 海力士宣布创纪录的 AI 投资计划](https://t.me/zaihuapd/42235) ⭐️ 8.0/10

三星和 SK 海力士将于 6 月 29 日在总统李在明主持的国家简报会上宣布大规模 AI 投资计划。三星拟公布 1000 万亿韩元（约 6480 亿美元）的十年支出方案，为韩国史上最大规模；SK 海力士计划五年内将产能翻倍，并在美国上市筹资 290 亿美元。 这一投资表明韩国半导体巨头向 AI 硬件的重大战略转向，可能重塑全球 AI 芯片供应链。其规模将加速 AI 基础设施建设，并加剧与美光等内存领导者的竞争。 同日，三星电子和 SK 海力士股价均下跌超 9%，部分原因与苹果相关担忧有关。投资重点聚焦半导体、AI 数据中心和物理 AI，三星承诺了韩国史上最大规模的单一企业支出计划。

telegram · zaihuapd · Jun 29, 07:00

**背景**: AI 数据中心是为训练和运行 AI 模型而优化的专用设施，严重依赖高带宽内存（HBM），而 SK 海力士和三星正是这类内存的生产商。物理 AI 指能够在物理世界中感知和行动的 AI 系统，例如机器人和自动驾驶车辆，它们需要先进的芯片和内存。此次公告凸显了韩国在 AI 硬件竞赛中领先的雄心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/glossary/generative-physical-ai/">What is Physical AI? | NVIDIA Glossary</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_data_center">AI data center</a></li>
<li><a href="https://grokipedia.com/page/Physical_AI">Physical AI</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#AI`, `#investment`, `#Samsung`, `#SK Hynix`

---

<a id="item-7"></a>
## [长鑫存储与腾讯签 30 亿美元 DRAM 供应协议](https://www.reuters.com/world/china/chinas-cxmt-wins-3-billion-memory-supply-deal-with-tencent-sources-say-2026-06-29/) ⭐️ 8.0/10

中国 DRAM 制造商长鑫存储（CXMT）与腾讯签署了一项价值近 30 亿美元的长期供应协议，将在三到五年内提供服务器内存芯片。 这笔交易标志着中国科技巨头大规模采用国产内存芯片，可能重塑全球 DRAM 供应链，减少对三星、SK 海力士等外国供应商的依赖。 该协议价值超过 200 亿元人民币（约 29.4 亿美元），合同期限根据消息来源不同为三年或五年。据报道，长鑫存储还在与阿里云、字节跳动和小米洽谈。

telegram · zaihuapd · Jun 29, 09:31

**背景**: 长鑫存储是中国领先的 DRAM 制造商之一，对于中国推动半导体自给自足至关重要。DRAM 是一种用于服务器、个人电脑和智能手机的内存芯片。历史上，DRAM 市场由三星、SK 海力士和美光主导。

**标签**: `#DRAM`, `#China`, `#Tencent`, `#supply chain`, `#memory chips`

---

<a id="item-8"></a>
## [特斯拉推送 FSD v14 Lite，HW3 车型获升级](https://x.com/Tesla_AI/status/2071592820889260101) ⭐️ 8.0/10

特斯拉于 2026 年 6 月 29 日发布 FSD v14 Lite，使 HW3 车型获得 HW4 级别的自动驾驶和自动泊车能力。 此次更新显著提升了数百万 HW3 特斯拉车主的自动驾驶体验，缩小了硬件代际差距，延长了旧款车型的使用寿命。 该更新包含了此前 HW4 独占的功能，如强化学习和离线模型，并引入了从停车位启动、倒车以及在目的地停车等新能力。

telegram · zaihuapd · Jun 30, 02:26

**背景**: 特斯拉的全自动驾驶（FSD）系统是一套高级驾驶辅助功能。硬件 3（HW3）和硬件 4（HW4）是特斯拉车载计算机的不同代际，HW4 提供更强的处理能力和更多传感器，从而实现更先进的自动驾驶能力。FSD v14 Lite 是一个专门的软件版本，通过软件优化和知识蒸馏将 HW4 级别的功能带到 HW3 车辆上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.basenor.com/blogs/news/tesla-update-v14-lite-1">FSD 14 Lite: Everything HW3 Owners Need to Know</a></li>
<li><a href="https://www.notateslaapp.com/news/4038/tesla-announces-fsd-v14-lite-features-and-release-timeline">Tesla Provides Update on FSD v14 Lite for HW3: Included ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Autopilot_hardware">Tesla Autopilot hardware - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Tesla`, `#FSD`, `#autonomous driving`, `#HW3`, `#update`

---