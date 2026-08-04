---
layout: default
title: "Horizon Summary: 2026-08-04 (ZH)"
date: 2026-08-04
lang: zh
---

> From 27 items, 6 important content pieces were selected

---

1. [OpenAI 展示人工智能在数学领域的十项进展](#item-1) ⭐️ 8.0/10
2. [MiniMax H3 上线 ComfyUI 首日支持：开放权重、原生音频与 2K 视频](#item-2) ⭐️ 8.0/10
3. [安迪·帕夫洛加入 ClickHouse，成立 ClickHouse 实验室](#item-3) ⭐️ 8.0/10
4. [DNA 分析设备漏洞恐致 30 年证据遭篡改](#item-4) ⭐️ 8.0/10
5. [英伟达 CMP 170HX 矿卡漏洞解锁 80GB 显存，二手价暴涨](#item-5) ⭐️ 8.0/10
6. [英国再要求苹果开后门 仅限本国公民数据](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 展示人工智能在数学领域的十项进展](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 8.0/10

OpenAI 在其网站上发表了一篇文章，重点介绍了人工智能在数学和理论计算机科学领域的十项突破。这一公告引起了研究界的广泛关注和讨论。 这标志着人工智能正从日常计算向创造性的数学发现迈进，可能从根本上改变研究工作方式。数学家和计算机科学家需要适应基于人工智能的新工具和协作方式。 该文章具体列出了十项进展，但现有的内容中没有详细描述。此公告建立在更广泛的行业努力之上，包括莱顿宣言，其中提到 OpenAI、Google DeepMind 和 Anthropic 是人工智能辅助数学发现的主要参与者。

hackernews · milkshakes · Aug 3, 16:27 · [社区讨论](https://news.ycombinator.com/item?id=49157930)

**背景**: 几个世纪以来，数学发现一直依赖于人类的直觉、猜想和证明。近年来，机器学习和大型语言模型已开始辅助生成假设和搜索证明，这一领域通常被称为机器学习用于定理证明。NeurIPS 和 ICML 上相关教程的出现，以及最近的莱顿宣言，都表明这一领域正在迅速发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Leiden_Declaration_on_Artificial_Intelligence_and_Mathematics">Leiden Declaration on Artificial Intelligence and Mathematics</a></li>
<li><a href="https://www.nature.com/articles/s41567-025-03042-0">Mathematical discovery in the age of artificial intelligence</a></li>

</ul>
</details>

**社区讨论**: 评论者大多感到印象深刻，但他们的解读各不相同。一些人认为进展呈指数曲线，并指出数学可能被人工智能‘消费’掉，而写作等其他领域则落后。另一些人则质疑这种炒作，并提到了该帖在 Hacker News 上的推荐。一个反复出现的主题是对人类数学家的担忧，有评论者引用道格拉斯·亚当斯的话，暗示许多研究人员最近的工作可能会被人工智能的耐力所颠覆。

**标签**: `#AI`, `#mathematics`, `#theoretical computer science`, `#OpenAI`, `#research`

---

<a id="item-2"></a>
## [MiniMax H3 上线 ComfyUI 首日支持：开放权重、原生音频与 2K 视频](https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui) ⭐️ 8.0/10

ComfyUI 宣布对 MiniMax H3 提供 Day-0 支持；H3 是一款开放权重的全模态生成模型，能以最高 2K 分辨率、长度 15 秒生成带原生立体声的视频。该集成让模型可在消费级 GPU（如 RTX 3060）上本地运行。 这标志着开放权重视频生成的重要进展，将一款先进的全模态模型在发布首日就接入 ComfyUI 的节点式工作流。爱好者与专业人士都能在本地生成带音频的 2K 视频，而不再依赖封闭 API，有望加速实验与创意生产。 MiniMax H3 可以在单次请求中混合输入文本、图像、视频和音频，并支持基于指令的编辑，保持未编辑内容稳定。ComfyUI 重新打包的模型文件已发布在 Hugging Face 上；通过剪枝约 40% 的调制权重，总内存占用从 123.6 GB 降至最低 42.5 GB，并结合动态 VRAM 卸载在 RTX 3060 上本地运行。

hackernews · vblanco · Aug 3, 13:34 · [社区讨论](https://news.ycombinator.com/item?id=49155629)

**背景**: MiniMax H3 是 MiniMax 推出的通用全模态生成模型，可同时理解文本、图像、视频和音频，并生成带原生立体声的视频。ComfyUI 是一个开源、基于节点的图形界面与后端，用于构建模块化扩散模型工作流，在 AI 绘画和视频社区中广泛使用。“Day-0 支持”意味着模型发布当天即可在 ComfyUI 中运行，无需等待社区适配器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H 3 : An Open Model Breaking the Boundaries Between Tasks...</a></li>
<li><a href="https://huggingface.co/Comfy-Org/MiniMax-H3">Comfy-Org/ MiniMax - H 3 · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/ComfyUI">ComfyUI</a></li>

</ul>
</details>

**社区讨论**: 用户反馈整体积极：有人用 16 GB 显存的 RTX 4070 Ti Super 在 10 分钟内生成一段 10 秒 480p 视频，称效果“惊艳”；也有人对文生视频的速度和质量感到惊讶。不过，有评论指出复杂镜头仍存在“AI 平滑”伪影，离谱/恶搞场景仍会崩坏；还有评论质疑“剪枝 40% 权重且不损质量”的做法能否迁移到 LLM。

**标签**: `#ComfyUI`, `#MiniMax`, `#video generation`, `#open weights`, `#AI/ML`

---

<a id="item-3"></a>
## [安迪·帕夫洛加入 ClickHouse，成立 ClickHouse 实验室](https://clickhouse.com/blog/andy-pavlo-joins-clickhouse) ⭐️ 8.0/10

知名数据库研究者、卡内基梅隆大学教授安迪·帕夫洛（Andy Pavlo）加入 ClickHouse，成立新的数据库研究实验室 ClickHouse Labs，相关消息已发布在 ClickHouse 博客上。此举将领先的学术界声音直接带入公司的工程团队。 这一事件意义重大，因为它表明商业数据库公司正在 AI 之外的领域投资基础研究，有望将学术思想与生产系统相结合。它可能影响 OLAP 架构的发展方向，尤其是业界向存算分离（decoupled compute and storage）迁移的趋势。 ClickHouse 是一款列式 OLAP 数据库，以高压缩列式存储和分布式查询处理著称。社区评论者也指出，StarRocks 等竞品和 Trino 等查询引擎正汇聚到使用 S3 等对象存储的存算分离架构上。

hackernews · nikolay_sivko · Aug 3, 14:09 · [社区讨论](https://news.ycombinator.com/item?id=49156011)

**背景**: OLAP 数据库针对大规模数据集的分析查询进行优化，通常使用列式存储来提高压缩率和扫描性能。存算分离将持久化存储（如 S3）与无状态计算资源分开，支持独立扩缩容并降低成本，但给数据摄入、索引和连接执行带来挑战。ClickHouse 是 AI 浪潮的重要受益者，设立该实验室也是回馈基础基础设施研究的一种方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://premvishnoi.medium.com/unlocking-the-potential-of-clickhouse-olap-db-architecture-use-cases-and-cost-analysis-56b1aa82bd85">Unlocking the Potential of ClickHouse OLAP DB: Architecture , Use...</a></li>
<li><a href="https://medium.com/@manik.ruet08/decoupling-compute-and-storage-in-modern-data-platforms-0a13f6100613">Decoupling Compute and Storage in Modern Data Platforms | Medium</a></li>
<li><a href="https://clickhouse.com/resources/engineering/unifying-oltp-and-olap">Unifying OLTP and OLAP : HTAP... | ClickHouse Resource Hub</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极，有人称赞这是 AI 领域之外的企业研究实验室，并希望安迪·帕夫洛的 CMU 系列讲座能赞助形式继续。也有评论者提出实质性质疑，包括学术界数据库经费萎缩，以及存算分离对数据摄入、索引和连接性能的影响。

**标签**: `#databases`, `#clickhouse`, `#research`, `#olap`, `#industry-news`

---

<a id="item-4"></a>
## [DNA 分析设备漏洞恐致 30 年证据遭篡改](https://www.wsj.com/tech/cybersecurity/security-flaw-placed-30-years-of-dna-evidence-at-risk-of-hacking-1932775a) ⭐️ 8.0/10

研究人员发现，美国多数犯罪实验室使用的 DNA 分析设备存在漏洞，可对 1995 年以来的法医 DNA 文件进行几乎无法察觉的篡改。赛默飞世尔科技于 7 月承认该漏洞，并发布高危安全公告及加入数字签名的软件更新。 该漏洞威胁到刑事案件调查和法庭审理中数十年的法医 DNA 证据完整性，凸显了美国 200 多家缺乏统一标准的实验室需要加强安全与监管。 研究人员借助 Anthropic 的 Claude 生成的 AI 代码修改 DNA 扫描数据，首次篡改耗时约 45 分钟，且未触发常用分析软件警报。该漏洞编号为 CVE-2026-17583，影响 Thermo Fisher 的 HID 软件产品中的 Applied Biosystems DNA 文件。

telegram · zaihuapd · Aug 3, 05:15

**背景**: 法医 DNA 分析依靠专用仪器和软件生成用于刑事司法的基因图谱。DNA 数据文件通常由毛细管电泳仪器生成，维护其完整性对证据链至关重要。数字签名可帮助验证文件未被篡改。该公司正与美国网络安全和基础设施安全局（CISA）合作，目前尚无实际利用案例。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/thermo-fisher-patches-flaw-that-could.html">Thermo Fisher Patches Flaw That Could Make DNA File Tampering Nearly Undetectable</a></li>
<li><a href="https://cybersecuritynews.com/dna-test-software-vulnerability/">DNA Test Software Vulnerability Allows Attackers to Alter Analysis Data</a></li>
<li><a href="https://www.hindustantimes.com/technology/security-flaw-placed-30-tears-of-dna-evidence-at-risk-of-hacking-101785681888060.html">Security flaw placed 30 tears of DNA evidence at risk of hacking | Technology News (HT Tech)</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#DNA analysis`, `#forensic science`, `#vulnerability`, `#supply chain`

---

<a id="item-5"></a>
## [英伟达 CMP 170HX 矿卡漏洞解锁 80GB 显存，二手价暴涨](https://finance.sina.com.cn/tech/roll/2026-08-03/doc-inikzqsf4659769.shtml) ⭐️ 8.0/10

亚利桑那州立大学研究人员公开了英伟达 CMP 170HX 矿卡上 Falcon 安全协处理器的栈溢出漏洞利用方法。该漏洞绕过 OTP 熔丝锁定，将显存最高扩展到 80GB，FP32 算力从 0.39 TFLOPS 提升到 94 TFLOPS。 这一安全绕过将原本廉价、低性能的矿卡变成了可用的 AI 推理加速器，导致二手价从 300–500 元飙升至 3000–4000 元，海外甚至叫价 1500 美元。它还表明英伟达在 GPU 上的硬件锁定可以被逆转，对硬件安全和 AI 硬件供应链有重要影响。 该漏洞利用 Falcon 安全协处理器中的无界 DMA 溢出劫持权限，并通过逐一修改寄存器来解除算力、显存和 PCIe 等限制。社区验证显示，解锁后的显卡可在 Windows 和 Linux 下运行 AI 图像生成及大语言模型推理，但长期稳定性和不同批次的可解锁上限仍有风险。

telegram · zaihuapd · Aug 3, 11:29

**背景**: CMP 170HX 是英伟达于 2021 年推出的专用加密货币矿卡，采用与 A100 相同的 GA100 核心，但通过 OTP 熔丝对算力、显存和 PCIe 带宽施加硬件锁定。OTP 熔丝是一种一次性可编程的非易失性位，用于永久设置硬件配置，此前被认为不可逆转；研究人员的栈溢出漏洞利用则通过修改运行时的寄存器来解锁硬件。该卡完整保留的 HBM2e 内存总线在适当的 FP32 负载下速度已可媲美真正的 A100，因此解锁后对 AI 推理很有吸引力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://niconiconi.neocities.org/tech-notes/nvidia-cmp-170hx-review/">All GB/s without FLOPS - Nvidia CMP 170HX Review, Performance Lockdown Workaround, Teardown, Watercooling, and Repair</a></li>
<li><a href="https://www.youtube.com/shorts/cIZpgNeolvU">Embedded 101: What Are OTP Fuses? #zephyrrtos #podcast #nvmem - YouTube</a></li>

</ul>
</details>

**标签**: `#hardware-security`, `#GPU`, `#exploit`, `#AI-inference`, `#Nvidia`

---

<a id="item-6"></a>
## [英国再要求苹果开后门 仅限本国公民数据](https://t.me/zaihuapd/42953) ⭐️ 8.0/10

9 月初，英国内政部向苹果发出新的技术能力通知，要求其为英国公民的加密 iCloud 备份创建后门。此前 1 月的一份通知曾要求全球访问权限，引发美英外交争端。 这标志着政府强制要求加密后门的最新升级，对全球隐私与安全具有重大影响。苹果的回应可能为科技公司如何处理政府破坏端到端加密的要求开创先例。 据报道，新通知仅针对英国公民的数据，与早前面向全球的要求不同。苹果此前已于 2 月从英国撤回 iCloud 高级数据保护功能，而非遵从先前的要求。

telegram · zaihuapd · Aug 3, 15:40

**背景**: 英国《2016 年调查权力法》允许内政部发出技术能力通知，要求电信运营商提供拦截数据的能力。iCloud 高级数据保护是苹果可选的端到端加密功能，用于保护包括备份在内的大部分 iCloud 数据，连苹果自身也无法访问密钥。若按通知要求开后门，等同于削弱这种加密以供执法机构访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Investigatory_Powers_Act_2016">Investigatory Powers Act 2016 - Wikipedia</a></li>
<li><a href="https://www.gov.uk/government/publications/investigatory-powers-amendment-bill-factsheets/investigatory-powers-amendment-bill-overview-of-the-notices-regime">Investigatory Powers (Amendment) Bill: Overview of the... - GOV. UK</a></li>
<li><a href="https://support.apple.com/en-us/108756">How to turn on Advanced Data Protection for iCloud - Apple Support</a></li>

</ul>
</details>

**标签**: `#encryption`, `#privacy`, `#UK government`, `#Apple`, `#backdoor`

---