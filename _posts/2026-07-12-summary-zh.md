---
layout: default
title: "Horizon Summary: 2026-07-12 (ZH)"
date: 2026-07-12
lang: zh
---

> From 23 items, 8 important content pieces were selected

---

1. [vLLM v0.25.0：MRv2 成为默认，重大架构更新](#item-1) ⭐️ 9.0/10
2. [人形机器人完成全球首例活猪胆囊手术](#item-2) ⭐️ 9.0/10
3. [GPU 云热潮中的循环融资](#item-3) ⭐️ 8.0/10
4. [ClickHouse 通过 peering 将 PgBouncer 吞吐量提升 4 倍](#item-4) ⭐️ 8.0/10
5. [SQLite 中推荐使用严格表以确保类型安全](#item-5) ⭐️ 8.0/10
6. [苹果起诉 OpenAI 系统性窃取商业机密](#item-6) ⭐️ 8.0/10
7. [U-Boot 曝出 6 个漏洞，可在启动时执行代码](#item-7) ⭐️ 8.0/10
8. [智谱创始人唐杰启动“摸高计划”聚焦 AGI](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0：MRv2 成为默认，重大架构更新](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 将 Model Runner V2 设为所有密集模型的默认执行路径，移除了旧版 PagedAttention 实现，并使 Transformers 建模后端达到与原生 vLLM 相同的速度。 此版本显著简化了 vLLM 代码库并提升了性能，使用户更容易部署和提供高吞吐量的大型语言模型。移除旧版注意力机制以及后端之间的速度持平，使得新模型架构和优化的采用更加迅速。 该版本包含来自 232 位贡献者的 558 次提交，支持 LLaVA-OneVision-2 和 GLM-5 等新模型，新增用于工具调用/推理的流式解析引擎，以及支持异构词表的通用推测解码。

github · khluu · Jul 11, 20:06

**背景**: vLLM 是一个开源的高吞吐量 LLM 推理引擎，使用 PagedAttention 高效管理键值缓存内存。Model Runner V2（MRv2）是一种重新设计的执行路径，统一了模型加载和推理，提高了可维护性并支持前缀缓存和实时嵌入等功能。Transformers 后端允许 vLLM 直接运行 Hugging Face 模型而无需转换，此版本使其速度与原生后端持平。

**标签**: `#vllm`, `#LLM inference`, `#model serving`, `#performance optimization`, `#open source`

---

<a id="item-2"></a>
## [人形机器人完成全球首例活猪胆囊手术](https://arstechnica.com/ai/2026/07/humanoid-robots-controlled-by-surgeons-did-world-first-operation-on-live-pigs/) ⭐️ 9.0/10

外科医生远程操控宇树 G1 人形机器人，成功在两头活猪身上完成了全球首例胆囊切除手术，相关成果发表在《自然》期刊。 这表明低成本、通用人形机器人有望让偏远地区、战场或太空等资源匮乏场景也能开展远程手术，可能推动外科医疗的普及。 宇树 G1 机器人基础款售价低至 13,500 美元，配备灵巧手后约 67,000 美元，远低于达芬奇等专用手术机器人（50 万美元以上）。机器人高约 1.5 米，重约 27 公斤。

telegram · zaihuapd · Jul 11, 02:29

**背景**: 远程手术是指外科医生远程操控机器人系统进行手术。传统专用手术机器人（如达芬奇）昂贵且体积庞大。人形机器人则提供了一种灵活且低成本的替代方案，可加装手术工具并通过远程操控执行操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://today.ucsd.edu/story/surgeons-use-teleoperated-humanoid-robots-to-perform-live-surgery-a-world-first">Surgeons Use Teleoperated Humanoid Robots to Perform Live Surgery – a World First</a></li>
<li><a href="https://www.popsci.com/technology/humanoid-robots-perform-surgery/">In groundbreaking first, humanoid robots performed surgery | Popular Science</a></li>
<li><a href="https://www.nature.com/articles/s41586-026-10796-x">In vivo feasibility study of humanoid robots in surgery | Nature</a></li>

</ul>
</details>

**标签**: `#humanoid robots`, `#surgery`, `#teleoperation`, `#medical robotics`, `#Nature`

---

<a id="item-3"></a>
## [GPU 云热潮中的循环融资](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 8.0/10

一项分析揭示，英伟达对 CoreWeave 和 Nebius 等 GPU 云提供商的投资形成了一个循环融资链条：这些提供商用英伟达的股权投资再去购买英伟达价值数十亿美元的 GPU。 这种循环融资引发了对 GPU 基础设施经济可持续性和潜在过度建设的担忧，可能影响整个 AI 云生态系统和投资者情绪。 英伟达投资 20 亿美元获得 CoreWeave 9%的股份，而 CoreWeave 计划 2026 年资本支出 350 亿美元，即英伟达的投资仅占 CoreWeave 单年支出的 5.7%；但更广泛的循环结构仍将 neocloud 与持续购买 GPU 捆绑在一起。

hackernews · adletbalzhanov · Jul 11, 17:21 · [社区讨论](https://news.ycombinator.com/item?id=48873836)

**背景**: 像 CoreWeave 和 Nebius 这样的 GPU 云提供商（neocloud）使用英伟达 GPU 提供 AI 计算服务。循环融资指英伟达投资这些客户，客户再用资金购买更多英伟达硬件，形成闭环，可能虚增需求并掩盖真实市场信号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom">Nvidia, CoreWeave, and Nebius: Inside the Circular Financing of the GPU Boom</a></li>
<li><a href="https://en.wikipedia.org/wiki/CoreWeave">CoreWeave</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nebius_Group">Nebius Group - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论意见不一：有人认为英伟达的小额股权使得循环融资的说法被夸大，而另一些人则争论 GPU 建设的长远盈利能力以及是否会出现产能过剩，并警告这可能成为一个纸牌屋。

**标签**: `#GPU`, `#Nvidia`, `#AI infrastructure`, `#cloud computing`, `#finance`

---

<a id="item-4"></a>
## [ClickHouse 通过 peering 将 PgBouncer 吞吐量提升 4 倍](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse 详细介绍了他们如何通过 peering 和其他优化，将其托管 PostgreSQL 服务中的 PgBouncer 吞吐量提升 4 倍。 这一显著的性能提升使 PgBouncer 对高流量 PostgreSQL 部署更具可扩展性，减少了运行多个连接池实例的需求。 Peering 机制允许取消请求转发到正确的 PgBouncer 进程，消除了路由错误导致的取消失败。该方案使用 SO_REUSEPORT 在同一端口上运行多个进程。

hackernews · saisrirampur · Jul 11, 15:28 · [社区讨论](https://news.ycombinator.com/item?id=48872874)

**背景**: PgBouncer 是 PostgreSQL 的轻量级连接池管理器，用于管理数据库连接。Peering 是 PgBouncer 的一项功能，允许多个进程共享会话状态并转发取消请求，从而减少因取消路由错误导致的额外开销并提升吞吐量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.pgbouncer.org/usage.html">PgBouncer command-line usage</a></li>
<li><a href="https://github.com/pgbouncer/pgbouncer/blob/master/doc/usage.md">pgbouncer/doc/usage.md at master · pgbouncer/pgbouncer</a></li>

</ul>
</details>

**社区讨论**: 社区成员提出了 Odyssey 和 pgdog 等替代方案，并询问了 Kubernetes 中的 peering 支持。总体反响积极，大家关注技术细节和实际部署考虑。

**标签**: `#postgresql`, `#pgbouncer`, `#connection-pooling`, `#performance`, `#scaling`

---

<a id="item-5"></a>
## [SQLite 中推荐使用严格表以确保类型安全](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 8.0/10

一篇博文鼓励 SQLite 用户采用严格表（strict tables）来强制数据类型，社区成员讨论了如 sqlite-utils 等用于转换现有表的工具。 严格表通过防止类型不匹配来提高数据完整性，使 SQLite 对于需要严格类型强制执行的应用程序更加可靠。 严格表自 SQLite 3.37.0 版本起可用，旧版本可通过设置'PRAGMA writable_schema=ON'读取。在 CREATE TABLE 语句末尾添加'STRICT'关键字即可启用。

hackernews · ingve · Jul 11, 17:33 · [社区讨论](https://news.ycombinator.com/item?id=48873940)

**背景**: 与大多数 SQL 数据库不同，SQLite 传统上允许将任何类型插入任何列（灵活类型）。这可能导致意外数据损坏，例如在整数列中存储字符串。严格表强制每列只接受其声明类型的值，使 SQLite 与其他数据库保持一致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite.org/stricttables.html">STRICT Tables</a></li>

</ul>
</details>

**社区讨论**: Simon Willison 为其 sqlite-utils 工具添加了将非严格表转换为严格表的功能。dfabulich 引用了 SQLite 官方关于不将严格设为默认的理由（flextypegood.html）。jll29 表示不同意并希望严格成为默认，而 petilon 指出缺少 Date 等数据类型是一个缺点。

**标签**: `#SQLite`, `#databases`, `#type safety`, `#data integrity`

---

<a id="item-6"></a>
## [苹果起诉 OpenAI 系统性窃取商业机密](https://www.cnbc.com/2026/07/10/apple-openai-lawsuit-trade-secrets.html) ⭐️ 8.0/10

苹果于 2026 年 7 月 10 日在美国加州北区联邦法院起诉 OpenAI、两名前员工及 io Products，指控 OpenAI 通过招聘苹果员工、接触供应商等方式，系统性窃取苹果的产品设计、制造工艺及供应链机密，以加快其消费级硬件研发。 这起诉讼突显出大型科技公司之间在知识产权（尤其是硬件和 AI 领域）上的紧张局势升级。如果指控成立，可能为商业机密保护树立先例，并影响消费硬件市场的竞争格局。 苹果指控前员工 Chang Liu 离职后仍访问内部网络并下载数十份硬件文件；OpenAI 硬件负责人 Tang Yew Tan 被指在离职前将供应商等资料发送至个人邮箱，并要求求职者携带苹果零部件参加面试。苹果称目前有超过 400 名前员工在 OpenAI 工作。

telegram · zaihuapd · Jul 11, 03:14

**背景**: 苹果长期以来在自有硬件设计和制造工艺上投入巨资，这是其产品差异化的关键。OpenAI 主要以其 AI 软件闻名，但正在拓展消费硬件领域，可能与苹果形成竞争。商业机密诉讼在科技行业很常见，用于保护机密信息不被竞争对手获取。

**标签**: `#Apple`, `#OpenAI`, `#Lawsuit`, `#Trade Secrets`, `#Hardware`

---

<a id="item-7"></a>
## [U-Boot 曝出 6 个漏洞，可在启动时执行代码](https://www.bleepingcomputer.com/news/security/new-u-boot-flaws-could-enable-stealthy-firmware-attacks/) ⭐️ 8.0/10

固件安全公司 Binarly 披露了 U-Boot 引导程序中 FIT 镜像签名验证的 6 个漏洞，其中两个可实现任意代码执行，四个可导致设备崩溃，影响自 2013.07 版本以来的众多版本。 这些漏洞位于操作系统启动前的阶段，攻击者可在操作系统和安全软件加载之前执行恶意代码，从而绕过固件安全功能并植入持久性恶意软件。对于支持远程固件更新的 BMC 等系统，攻击者甚至无需物理接触设备即可利用。 这些漏洞位于 FIT（Flattened Image Tree）签名验证代码中，其中两个关键漏洞可导致代码执行，四个可导致拒绝服务。补丁已提交并被 U-Boot 维护者接受，但集成需要硬件厂商完成；已停止支持的设备可能永远无法获得修复。

telegram · zaihuapd · Jul 11, 08:32

**背景**: U-Boot 是一个广泛使用的开源引导程序，适用于嵌入式系统，支持 ARM、x86、RISC-V 等多种架构。它从存储设备或网络加载操作系统内核。FIT 镜像格式将内核、设备树等数据打包成一个镜像，并通过签名验证其真实性和完整性。基板管理控制器（BMC）是用于远程服务器管理的专用微控制器，通常依赖 U-Boot 启动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Das_U-Boot">Das U - Boot - Wikipedia</a></li>
<li><a href="https://docs.u-boot.org/en/latest/usage/fit/signature.html">U-Boot FIT Signature Verification — Das U-Boot unknown version documentation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Intelligent_Platform_Management_Interface">Intelligent Platform Management Interface - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#bootloader`, `#U-Boot`, `#vulnerabilities`, `#firmware`

---

<a id="item-8"></a>
## [智谱创始人唐杰启动“摸高计划”聚焦 AGI](https://mp.weixin.qq.com/s/3CQSkf_kBnXiCDgS4L-Cgg) ⭐️ 8.0/10

智谱 AI 创始人唐杰宣布启动“摸高计划”，提出通向 AGI 的四座高峰：长程任务、自治智能体、完全自我训练和极致安全治理，并投入百亿级资源攻坚机械可解释性。 该计划标志着中国主要 AI 实验室从短期商业变现转向长期 AGI 研究的战略转变，可能影响全球 AI 竞争格局。对安全性和可解释性的强调回应了业界对黑盒 AI 系统的日益担忧。 计划包括百亿级资源投入机械可解释性，以打开神经网络“黑盒”。智谱 GLM-5.2 模型据称接近最前沿能力，并因其开源 MIT 许可证而受到技术社群欢迎。

telegram · zaihuapd · Jul 11, 13:59

**背景**: 机械可解释性是 AI 安全研究的一个子领域，旨在通过分析内部电路和特征，将神经网络逆向工程为人类可理解的算法。智谱 AI（现已更名为 Z.ai）以其开源 GLM 系列大语言模型而闻名，GLM-5 是一个 745B 参数、202K 上下文长度的模型。该公司自 2025 年 7 月起以 MIT 许可证发布模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://en.wikipedia.org/wiki/Z.ai">Z.ai - Wikipedia</a></li>
<li><a href="https://glm5.ai/">GLM -5 - Zhipu AI's Flagship Foundation Model</a></li>

</ul>
</details>

**标签**: `#AGI`, `#AI Safety`, `#Zhipu`, `#Interpretability`, `#Chinese AI`

---