---
layout: default
title: "Horizon Summary: 2026-06-20 (ZH)"
date: 2026-06-20
lang: zh
---

> From 27 items, 9 important content pieces were selected

---

1. [Project Valhalla 最终在 JDK 28 中落地](#item-1) ⭐️ 9.0/10
2. [ATProto 没有‘实例’——协议架构澄清](#item-2) ⭐️ 8.0/10
3. [挪威禁止小学使用人工智能](#item-3) ⭐️ 8.0/10
4. [法院记录应免费](#item-4) ⭐️ 8.0/10
5. [美国施压 ASML，担忧顶级光刻机流入中国](#item-5) ⭐️ 8.0/10
6. [多款知名纸尿裤检出生殖毒性物质甲酰胺](#item-6) ⭐️ 8.0/10
7. [苹果同意在巴西开放第三方应用商店和外部支付](#item-7) ⭐️ 8.0/10
8. [北航博士生指控教授论文造假](#item-8) ⭐️ 8.0/10
9. [Anthropic 技术人员与白宫会面讨论 AI 模型下线争端](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Project Valhalla 最终在 JDK 28 中落地](https://www.jvm-weekly.com/p/project-valhalla-explained-how-a) ⭐️ 9.0/10

经过十年的开发，Project Valhalla 的值类型和空安全改进将被整合到 JDK 28 中，这标志着 JVM 的一个重要里程碑。 这通过扁平化内存布局和减少间接寻址带来了性能提升，同时空安全特性有助于防止常见编程错误，对 Java 开发者和企业应用产生重大影响。 该实现允许 JVM 将值对象密集存储在数组中，无需每个元素的头部或指针，但堆扁平化可能存在 64 位限制；每个元素可能仍需一个空标志。

hackernews · philonoist · Jun 19, 06:35 · [社区讨论](https://news.ycombinator.com/item?id=48595511)

**背景**: Project Valhalla 是 2014 年启动的 OpenJDK 项目，旨在通过值类型扩展 Java 对象模型，值类型行为类似基本类型但可由用户定义。值类型通过启用扁平化内存布局，旨在结合对象的抽象性和基本类型的性能。空安全是另一个长期期待的特性，以减少空指针异常。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Project_Valhalla_(Java_language)">Project Valhalla (Java language) - Wikipedia</a></li>
<li><a href="https://openjdk.org/projects/valhalla/">Project Valhalla - OpenJDK</a></li>

</ul>
</details>

**社区讨论**: 评论中既有赞赏也有批评：一些用户认为空安全应该更易于采用，而另一些则质疑堆扁平化对于较大对象的实际限制。还有观点认为许多批评者对现代 Java 持有过时的看法。

**标签**: `#Java`, `#JVM`, `#Project Valhalla`, `#value types`, `#null-safety`

---

<a id="item-2"></a>
## [ATProto 没有‘实例’——协议架构澄清](https://overreacted.io/there-are-no-instances-in-atproto/) ⭐️ 8.0/10

Dan Abramov 发表了一篇文章，解释 ATProto（Bluesky 背后的协议）没有像 Mastodon 那样的‘实例’，而是将用户数据（PDS）、数据中继（Relays）和应用服务（AppViews）分离。 这一澄清纠正了关于 ATProto 架构的普遍误解，对于理解去中心化社交媒体如何扩展至关重要。它突出了与 Mastodon 的根本设计差异，影响评估联合方法的开发者和用户。 Relays 是一种优化，用于减少 PDS 和 AppViews 之间的连接数量，并非严格必要。AppViews 从 Relays 获取数据以构建时间线和聚合，而 PDS 存储用户数据和加密密钥。

hackernews · danabramov · Jun 19, 15:10 · [社区讨论](https://news.ycombinator.com/item?id=48599515)

**背景**: Mastodon 和其他基于 ActivityPub 的平台运行‘实例’——独立服务器，托管用户、内容和审核。Bluesky 使用的 ATProto 将这些功能解耦为独立服务：PDS（个人数据服务器）用于存储，Relays 用于数据分发，AppViews 用于向用户呈现内容。这种模块化设计旨在提高可扩展性和用户可移植性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AT_Protocol">AT Protocol - Wikipedia</a></li>
<li><a href="https://atproto.brussels/atproto-architecture">ATProto Architecture • atproto.brussels</a></li>
<li><a href="https://atproto.com/guides/glossary">A collection of terminology used in the AT Protocol and their definitions.</a></li>

</ul>
</details>

**社区讨论**: 评论褒贬不一：一些人赞赏对 ATProto 模块化架构的清晰解释，而另一些人则批评其与 RSS 的类比，并指出实际上 Bluesky 公司仍运行大部分基础设施，使系统事实上去中心化不足。还有人指出 Relays 运行成本高昂，可能成为瓶颈。

**标签**: `#ATProto`, `#Bluesky`, `#decentralization`, `#protocol design`, `#social media architecture`

---

<a id="item-3"></a>
## [挪威禁止小学使用人工智能](https://www.reuters.com/technology/norway-imposes-near-ban-ai-elementary-school-2026-06-19/) ⭐️ 8.0/10

挪威政府宣布，原则上禁止 6 至 13 岁学生使用人工智能，而 14 至 16 岁的学生可在教师监督下谨慎使用。 这为国家层面的教育领域 AI 监管树立了先例，回应了关于基础技能发展和潜在学习干扰的担忧。 禁令适用于 1 至 7 年级（6-13 岁），而初中生（14-16 岁）可在教师指导下谨慎使用 AI 工具。

hackernews · ilreb · Jun 19, 16:03 · [社区讨论](https://news.ycombinator.com/item?id=48600093)

**背景**: 像 ChatGPT 这样的生成式 AI 能快速生成文本，可能削弱幼儿的阅读、写作和理解能力学习。挪威的政策旨在保护基础教育，限制 AI 的使用直到学生掌握核心技能。

**社区讨论**: 评论者大多支持该禁令，将其类比为数学中计算器的使用，并强调在使用 AI 工具前需要先培养推理能力。有人指出 AI 对学生成绩造成了灾难性影响，并警告执行上的挑战。

**标签**: `#AI`, `#education`, `#policy`, `#Norway`, `#debate`

---

<a id="item-4"></a>
## [法院记录应免费](https://www.eff.org/deeplinks/2026/06/court-records-should-be-free) ⭐️ 8.0/10

电子前沿基金会（EFF）发表文章，主张法院记录应免费开放，批评 PACER 系统按页收费的付费墙模式。 此事至关重要，因为获取法院记录是司法公正和透明的基础；高昂费用为个人和小实体设置障碍，削弱了公共问责制。 联邦法院 PACER 费用为每页 1 美元，而爱达荷州等州法院每页收费 10 美元。CourtListener 和 Recap 等工具通过免费分享已购文档来缓解问题。

hackernews · hn_acker · Jun 19, 17:34 · [社区讨论](https://news.ycombinator.com/item?id=48600946)

**背景**: PACER（公共法院电子记录查询系统）是美国联邦法院文件的电子公共访问服务。批评者认为，用于维持系统运转的费用应被免除，因为公共记录属于公众。EFF 等倡导团体长期呼吁免费开放法院记录。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PACER_(law)">PACER (law) - Wikipedia</a></li>
<li><a href="https://pacer.uscourts.gov/">Public Access to Court Electronic Records | PACER: Federal Court Records</a></li>

</ul>
</details>

**社区讨论**: tptacek 用市政铅管更换费用作类比，指出这是一个常见的公共政策难题。jacobmarble 提到爱达荷州法院费用比联邦法院高出十倍。cdolan 称赞 CourtListener 和 Recap 填补了关键空白，而 treebeard901 认为经济成本是政府刻意限制公民权利的一种方式。

**标签**: `#court records`, `#PACER`, `#access to justice`, `#EFF`, `#public policy`

---

<a id="item-5"></a>
## [美国施压 ASML，担忧顶级光刻机流入中国](https://www.bloomberg.com/news/articles/2026-06-19/us-tells-asml-it-s-concerned-china-may-have-top-chip-tool) ⭐️ 8.0/10

美国商务部长向 ASML 高管表示，怀疑一台顶级极紫外光刻机（EUV）可能已流入中国，违反美方主导的出口管制。ASML 坚决否认，称从未向中国出口 EUV 整机。 此事件加剧了中美科技紧张局势，可能导致更严格的半导体出口管制，影响全球供应链和 ASML 的业务。同时也使美欧在芯片政策上的关系紧张。 美方声称掌握 ASML 未善意行事的证据，包括对华出口 EUV 相关运输设备，但拒绝出示。ASML 已散发文件自证清白，并反驳称从未出口任何 EUV 专用组件。

telegram · zaihuapd · Jun 19, 03:09

**背景**: EUV 光刻是一种用于制造先进半导体的尖端技术，能够实现 12 纳米以下的特征尺寸。ASML 是 EUV 系统的唯一供应商，这些系统受到严格的出口管制，以防止中国获得。美国一直在施压盟友收紧这些管制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Extreme_ultraviolet_lithography">Extreme ultraviolet lithography - Wikipedia</a></li>
<li><a href="https://www.asml.com/en/products/euv-lithography-systems">EUV lithography systems – Products | ASML</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#export controls`, `#ASML`, `#US-China`, `#lithography`

---

<a id="item-6"></a>
## [多款知名纸尿裤检出生殖毒性物质甲酰胺](https://t.me/zaihuapd/42051) ⭐️ 8.0/10

经济参考报委托检测发现，好奇、碧芭宝贝、Babycare 等知名品牌婴幼儿纸尿裤中含有生殖毒性物质甲酰胺，部分婴幼儿血液和尿液中也被检出该物质。 甲酰胺可通过皮肤吸收并在体内蓄积，对生殖系统和肝肾造成长期危害，此次曝光揭示了中国纸尿裤安全标准中的重大监管空白。 我国化妆品目录已禁用甲酰胺，但纸尿裤国标尚未将其纳入检测；一名记者穿戴被测纸尿裤一夜后，血液中甲酰胺浓度几乎翻倍。

telegram · zaihuapd · Jun 19, 06:05

**背景**: 甲酰胺是一种工业溶剂，用于部分纸尿裤的生产。小鼠研究显示其会降低生育能力，皮肤吸收是人体主要暴露途径之一。其他国家已对泡沫玩具中的甲酰胺设定限值（如 EN 71-15）。中国现行纸尿裤标准未涵盖甲酰胺，业内呼吁修订。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Formamide">Formamide - Wikipedia</a></li>
<li><a href="https://www.sciencedirect.com/topics/pharmacology-toxicology-and-pharmaceutical-science/formamide">Formamide - an overview | ScienceDirect Topics</a></li>
<li><a href="https://standards.iteh.ai/catalog/standards/sist/50697200-e3d2-4e36-8299-efd4d2a2409c/sist-en-71-15-2025">SIST EN 71-15:2025 - Toy Safety Formamide Limits in Foam Materials</a></li>

</ul>
</details>

**标签**: `#consumer safety`, `#public health`, `#regulatory gap`, `#toxicology`, `#infant products`

---

<a id="item-7"></a>
## [苹果同意在巴西开放第三方应用商店和外部支付](https://t.me/zaihuapd/42059) ⭐️ 8.0/10

苹果与巴西反垄断监管机构达成协议，允许 iPhone 用户在 App Store 之外购买应用和服务，并支持第三方应用商店。相关改变需在 105 天内落实，协议有效期为三年。 这标志着苹果在一个关键市场做出重大让步，可能为其他司法管辖区采取类似反垄断行动树立先例。开发者将获得更多自由来提供替代支付方式和分发渠道，可能降低苹果的佣金费用。 根据协议，开发者可以展示外部支付选项和替代购买链接，苹果的支付系统将与 App Store 解耦。但苹果仍可能对通过外部系统进行的交易收取费用。

telegram · zaihuapd · Jun 19, 11:15

**背景**: 多年来，苹果一直严格控制 iOS 应用分发和支付，要求开发者使用其应用内购买系统并支付 30%的佣金（小型企业为 15%）。这种控制受到全球监管机构的挑战，包括欧盟的《数字市场法案》（DMA）迫使苹果在欧洲允许第三方应用商店。巴西的反垄断调查也源于类似的关于反竞争行为的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://adapty.io/blog/alternative-payments-in-the-app-store/">Alternative payments in the App Store: All you need to know</a></li>
<li><a href="https://eu.36kr.com/en/p/3825979669074820">Apple Unlocks the Door to Third - Party App Stores</a></li>

</ul>
</details>

**标签**: `#Apple`, `#antitrust`, `#Brazil`, `#app store`, `#payments`

---

<a id="item-8"></a>
## [北航博士生指控教授论文造假](https://www.zaobao.com.sg/news/china/story20260619-9231002) ⭐️ 8.0/10

北京航空航天大学前博士生耿江涛公开指控两名教授常凌乾和王军论文数据造假，视频发布后大量网民涌入北航官网，导致网站一度瘫痪。 此案凸显了中国顶尖大学学术诚信问题正受到公众日益严格的审视，也表明民间打假人士在揭露学术不端行为方面的影响力正在上升。 耿江涛于 2025 年从北航退学成为科普博主，自今年 4 月起已接连举报四所大学的五名学者，目前五人全部被处置。

telegram · zaihuapd · Jun 19, 16:02

**背景**: 学术造假一直是中国科研体系的顽疾，多起高调事件损害了顶尖学府的声誉。民间举报人（常为内部人士）已成为关键监督力量，他们通过社交媒体发布证据，推动机构启动调查。

**标签**: `#academic fraud`, `#research integrity`, `#Beihang University`, `#scientific misconduct`, `#China`

---

<a id="item-9"></a>
## [Anthropic 技术人员与白宫会面讨论 AI 模型下线争端](https://t.me/zaihuapd/42064) ⭐️ 8.0/10

Anthropic 的高级技术人员计划下周与白宫官员会面，以解决导致其最先进的 AI 模型 Fable 5 和 Mythos 5 全球下线的争端。 这次会面凸显了 AI 公司与政府监管机构之间在国家安全和外国访问强大 AI 方面的紧张局势升级，可能为未来的 AI 治理和全球可用性树立先例。 特朗普政府命令 Anthropic 阻止外国人使用 Fable 5 和 Mythos 5，理由是国家安全担忧；Anthropic 随后在全球范围内禁用了这两个模型，影响了数亿用户。

telegram · zaihuapd · Jun 20, 02:45

**背景**: Anthropic 的 Mythos 系列模型（包括 Mythos 5 和公开发布的 Fable 5）专为高级任务设计，例如发现软件漏洞。美国政府的命令是基于担心外国对手可能滥用这些模型的强大能力。Anthropic 此前已因 Mythos 5 的黑客能力推迟了其广泛发布，之后才推出了带有安全措施的 Fable 5。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/06/12/technology/anthropic-mythos-fable5-blocked.html">Anthropic Blocks Foreigners From Using Mythos and Fable AI</a></li>
<li><a href="https://www.bbc.com/news/articles/c932g3v3e13o">Anthropic 's Claude Fable 5 and Mythos 5 AI suspended over security...</a></li>
<li><a href="https://news.bitcoin.com/anthropic-fable-5-mythos-5-us-suspension/">Anthropic Disables Fable 5 and Mythos 5 Worldwide After US...</a></li>

</ul>
</details>

**标签**: `#AI政策`, `#AI安全`, `#Anthropic`, `#政府监管`

---