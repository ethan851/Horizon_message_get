---
layout: default
title: "Horizon Summary: 2026-06-19 (ZH)"
date: 2026-06-19
lang: zh
---

> From 34 items, 6 important content pieces were selected

---

1. [一万个 GitHub 仓库传播木马恶意软件](#item-1) ⭐️ 9.0/10
2. [医院和大学以 90%更低成本重新利用药物](#item-2) ⭐️ 8.0/10
3. [工具检查你的名字是否“在模型权重中”](#item-3) ⭐️ 8.0/10
4. [Modos 彩色电子纸显示器实现 60Hz 刷新率](#item-4) ⭐️ 8.0/10
5. [苹果与英特尔达成初步芯片代工协议](#item-5) ⭐️ 8.0/10
6. [国家网信办就分布式数字身份规则征求意见](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [一万个 GitHub 仓库传播木马恶意软件](https://orchidfiles.com/github-repositories-distributing-malware/) ⭐️ 9.0/10

研究人员发现超过 10,000 个 GitHub 仓库在分发木马恶意软件，通过克隆合法仓库并推送恶意提交来利用 AI 代理和开发者信任。 这一大规模供应链攻击可能感染大量开发者及终端用户，凸显了 AI 代理被诱骗信任恶意仓库的风险日益增长。 攻击者针对新仓库而非流行仓库，并频繁删除和推送新提交以在搜索结果中显示为最新，旨在欺骗抓取仓库依赖的 AI 代理。

hackernews · theorchid · Jun 18, 11:45 · [社区讨论](https://news.ycombinator.com/item?id=48583928)

**背景**: 供应链攻击针对软件供应链中安全性较低的元素，例如被注入恶意软件的克隆仓库。攻击者希望开发者或 AI 代理下载恶意代码，然后通过依赖关系传播。AI 编程代理自动获取包的兴起放大了此类攻击的风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack</a></li>
<li><a href="https://siliconangle.com/2025/06/02/sysdig-detects-ai-assisted-malware-exploiting-open-webui-misconfigurations/">Sysdig detects AI -assisted malware exploiting Open... - SiliconANGLE</a></li>

</ul>
</details>

**社区讨论**: 评论者指出该攻击针对 AI 代理而非人类，通过出现在搜索中实现。一位用户分享了个人经历，其名字被附加到无关项目上。另有人提到迪士尼工程师从 GitHub 下载恶意 AI 工具的事件。讨论还注意到频繁的提交更新有助于仓库在“最后更新”搜索中排名靠前。

**标签**: `#security`, `#malware`, `#GitHub`, `#supply chain attacks`, `#AI agents`

---

<a id="item-2"></a>
## [医院和大学以 90%更低成本重新利用药物](https://www.kcl.ac.uk/news/hospitals-and-universities-repurposing-drugs-at-90-lower-cost) ⭐️ 8.0/10

医院和大学正以极低的成本重新利用现有药物治疗新适应症，例如使用癌症药物 Avastin 治疗黄斑变性，每剂约 50 美元，而 Lucentis 需要 1500 美元。 这种方法可以大幅降低医疗成本并改善治疗的可及性，尤其适用于黄斑变性和罕见病等新药开发成本过高的疾病。 Avastin 和 Lucentis 分子相似，但 Avastin 未包装成眼用注射剂，导致成本差异。目前尚无明确的监管途径可在未获制造商同意的情况下扩展药物用途，这成为广泛应用的障碍。

hackernews · giuliomagnifico · Jun 18, 10:33 · [社区讨论](https://news.ycombinator.com/item?id=48583386)

**背景**: 药物再利用是指研究已批准药物的新适应症。这是一种成本效益高的策略，因为药物的安全性已知，减少了开发时间和费用。常见例子包括使用氟西汀治疗年龄相关性黄斑变性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Drug_repurposing">Drug repurposing</a></li>
<li><a href="https://www.nih.gov/news-events/nih-research-matters/repurposing-drugs-treat-age-related-macular-degeneration">Repurposing drugs to treat age-related macular degeneration | National Institutes of Health (NIH)</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了现实世界的例子，如 Avastin 与 Lucentis 治疗黄斑变性的对比，以及 Cures Within Reach 在罕见病方面的成功。他们还指出了监管和激励方面的挑战，例如 Spravato（艾司氯胺酮）作为氯胺酮的改进版获得专利，以及超说明书使用缺乏明确途径。

**标签**: `#drug repurposing`, `#healthcare costs`, `#pharmaceuticals`, `#macular degeneration`

---

<a id="item-3"></a>
## [工具检查你的名字是否“在模型权重中”](https://www.intheweights.com/) ⭐️ 8.0/10

新网站“Are You in the Weights?”允许用户并行查询多个大型语言模型，查看它们对给定姓名或用户名的识别强度，从而揭示个人数据在模型权重中的痕迹。 该工具凸显了人们对 LLM 中隐私和记忆化问题的日益关注，因为它展示了模型可以在未经同意的情况下从训练数据中保留个人信息，可能使用户面临被识别或提取攻击的风险。 该工具并行查询前沿和小型模型，聚类响应并提供识别分数。用户必须使用真实姓名或用户名，这引发了隐私问题；网站报告称分数是非确定性的，并且添加更多关键词会提高分数。

hackernews · turtlesoup · Jun 18, 20:49 · [社区讨论](https://news.ycombinator.com/item?id=48591348)

**背景**: 大型语言模型（LLM）在大量文本上进行训练，包括网页和社交媒体帖子等公共数据。在训练过程中，模型可能会记住特定信息，包括个人姓名和用户名，这种现象称为记忆化。如果攻击者可以提示模型泄露这些数据，就会带来隐私风险。该网站通过直接向模型询问个人身份来利用这一现象。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/html/2410.02650v1">Undesirable Memorization in Large Language Models: A Survey</a></li>
<li><a href="https://www.scirp.org/journal/paperinformation?paperid=133625">Evaluating Privacy Leakage and Memorization Attacks on Large Language Models (LLMs) in Generative AI Applications</a></li>
<li><a href="https://proceedings.mlr.press/v202/yu23c/yu23c.pdf">Bag of Tricks for Training Data Extraction from Language Models</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了不同的结果：有人发现他们的用户名在使用了数十年后得到了高度识别，而有些人发现模型更倾向于一个同名的名人。隐私问题被提出，导致许多人避免使用真实姓名。一位用户注意到，添加更多个人关键词会提高分数，并且观察到了非确定性的特点。

**标签**: `#LLMs`, `#privacy`, `#online identity`, `#AI recognition`, `#tool`

---

<a id="item-4"></a>
## [Modos 彩色电子纸显示器实现 60Hz 刷新率](https://spectrum.ieee.org/modos-e-paper-monitor) ⭐️ 8.0/10

Modos 这家两人创业公司正在开发一款 13.3 英寸彩色电子纸显示器，原生分辨率 3200×2400，刷新率达 60Hz，将电子纸技术推近主流 LCD 性能。 如果成功，这款显示器将能实现适合长时间阅读且可在户外使用、功耗极低的电子纸显示器，为辅助显示器和便携设备开辟新可能。 这款名为 Modos Flow 的显示器支持触摸输入，目标是实现日常使用的响应速度；但由于电子纸物理粒子运动的限制，面板实际响应时间可能仍比 LCD 慢。

hackernews · Vinnl · Jun 18, 11:41 · [社区讨论](https://news.ycombinator.com/item?id=48583897)

**背景**: 电子纸显示器利用带电粒子反射环境光，具有低功耗和户外可读性，但历史上刷新率慢且色彩有限。E Ink 等厂商的最新进展改善了色彩和刷新率，但 60Hz 仍是电子纸的一个里程碑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Electronic_paper">Electronic paper - Wikipedia</a></li>
<li><a href="https://spectrum.ieee.org/e-paper-display-modos">E-Paper Display Reaches the Realm of LCD Screens - IEEE Spectrum</a></li>

</ul>
</details>

**社区讨论**: 社区评论积极，用户称其是'最令人兴奋的发展之一'，并指出这可能是首款响应速度足以日常使用的电子墨水显示器。也有人对高刷新率对电子纸面板寿命的影响表示好奇。

**标签**: `#e-paper`, `#displays`, `#hardware`, `#alternative technology`

---

<a id="item-5"></a>
## [苹果与英特尔达成初步芯片代工协议](https://t.me/zaihuapd/42031) ⭐️ 8.0/10

苹果与英特尔已达成初步协议，由英特尔代工生产部分苹果设备所需的芯片。该协议经过一年多的谈判后最终敲定。 该协议使苹果芯片供应链多元化，减少对台积电的依赖，同时增强英特尔的代工业务，这对美国半导体政策至关重要。 目前尚不清楚哪些苹果设备（iPhone、iPad 或 Mac）将采用英特尔制造的芯片。美国政府（由商务部长牵头）大力推动此次合作，目前英特尔已与英伟达、SpaceX 和苹果三家建立了代工合作伙伴关系。

telegram · zaihuapd · Jun 18, 09:19

**背景**: 代工协议意味着一家公司制造另一家公司设计的芯片。苹果目前严重依赖台积电为 iPhone、iPad 和 Mac 生产芯片。英特尔正在扩大其代工服务，作为美国推动国内半导体制造的一部分。

**标签**: `#Apple`, `#Intel`, `#Semiconductor`, `#Foundry`, `#Supply Chain`

---

<a id="item-6"></a>
## [国家网信办就分布式数字身份规则征求意见](https://www.cac.gov.cn/2026-06/18/c_1783525605384124.htm) ⭐️ 8.0/10

2026 年 6 月 18 日，国家互联网信息办公室发布《促进分布式数字身份互通互认应用规定（征求意见稿）》并向社会公开征求意见，截止日期为 7 月 18 日。该规定明确了基于区块链的分布式数字身份，由标识符、密钥、可验证凭证和可验证声明构成，支持用户自主管理身份信息，可用于登录认证、数据授权等场景。 这是一项重要的政策举措，为中国去中心化数字身份建立了监管框架，可能影响区块链采用以及金融、交通、海关、税务和数字人民币等领域的跨平台身份互通互认。这可能会为政府主导的分布式身份系统树立全球先例。 该规定提出建设分布式数字身份公共服务体系，依托国家区块链网络建设“身份链”。境内外个人、机构和工业设备均可自愿申请注册，相关机构需履行数据安全和个人信息保护义务。

telegram · zaihuapd · Jun 19, 01:39

**背景**: 分布式数字身份（DDID），也称为自主权身份（SSI），将身份数据的控制权从中心化提供者转移给用户。可验证凭证（VC）是遵循 W3C 标准、防篡改的数字文档，允许颁发者、持有者和验证者之间进行可信交互。“身份链”概念利用区块链为跨平台身份验证创建去中心化基础架构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reply.com/en/data-world/decentralised-digital-identity-will-change-everything">Decentralised Digital Identity ( DDID ) will change how we... | Reply</a></li>
<li><a href="https://en.wikipedia.org/wiki/Verifiable_credentials">Verifiable credentials</a></li>
<li><a href="https://chain.link/article/onchain-identity-verification">Onchain Identity Verification Explained | Chainlink</a></li>

</ul>
</details>

**标签**: `#distributed identity`, `#blockchain`, `#regulation`, `#China`, `#digital identity`

---