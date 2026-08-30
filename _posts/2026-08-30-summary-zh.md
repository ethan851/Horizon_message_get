---
layout: default
title: "Horizon Summary: 2026-08-30 (ZH)"
date: 2026-08-30
lang: zh
---

> From 20 items, 5 important content pieces were selected

---

1. [腾讯开源 Hy4 预览版大模型，具备自我改进能力](#item-1) ⭐️ 8.0/10
2. [优秀文化才是最大生产力提升，而非 AI](#item-2) ⭐️ 8.0/10
3. [DHS 利用鲜为人知的海关法窥探记者与非营利组织](#item-3) ⭐️ 8.0/10
4. [中国拟将新能源车定型试验里程统一提高至 3 万公里](#item-4) ⭐️ 8.0/10
5. [索尼音乐等起诉 Anthropic：用盗版歌词与书籍训练 Claude](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [腾讯开源 Hy4 预览版大模型，具备自我改进能力](https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/) ⭐️ 8.0/10

腾讯发布了并开源了 Hy4 preview，这是一个 770B 参数的混合专家模型，已在 Hugging Face 和 OpenRouter 上线。它具备早期递归自我改进循环，模型可优化自身的训练方法、数据策略和评估框架。 此举意义重大，因为一家大型科技公司开源具备自我改进能力的尖端规模大语言模型，可能加速 AI 研究和应用。Hy4 preview 在 OpenRouter 上迅速获得大量使用，短短几天内处理了数万亿 token，表明市场需求强劲。 Hy4 preview 是一个混合专家模型，总参数量 770B，激活参数 49B。其上下文窗口为 1,048,576 个 token，在 OpenRouter 上的定价为每百万输入 token 0.834 美元、每百万输出 token 2.501 美元。

hackernews · shenli3514 · Aug 29, 19:33 · [社区讨论](https://news.ycombinator.com/item?id=49492632)

**背景**: 混合专家（MoE）模型每个 token 仅激活部分参数，从而在保持大容量的同时降低计算成本。OpenRouter 是一种 LLM 路由服务，开发者通过统一 API 即可访问多个模型。语言模型的自我改进指利用模型自身作为验证器或优化器，来改进其输出和训练过程，这是目前日益受关注的研究方向。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/tencent/Hy4-preview">tencent/Hy4-preview · Hugging Face</a></li>
<li><a href="https://openrouter.ai/tencent/hy4-preview">Hy4 preview - API Pricing & Providers | OpenRouter</a></li>
<li><a href="https://cryptobriefing.com/tencent-hy4-preview-770b-ai-model/">Tencent spotted testing Hy4 model in Yuanbao app as expert-level model</a></li>

</ul>
</details>

**社区讨论**: 评论者提到 Hy4 preview 在 OpenRouter 上“极其惊人的使用量”，几天内处理了数万亿 token，并讨论了其较低的缓存成本。还有人质疑 token 密度优化，认为缩小词表可能造成“新语（Newspeak）”问题；另有评论者批评发布中的柱状图排序不合理。

**标签**: `#AI/ML`, `#LLM`, `#Tencent`, `#Open Source`, `#Self-improvement`

---

<a id="item-2"></a>
## [优秀文化才是最大生产力提升，而非 AI](https://newsletter.eng-leadership.com/p/good-culture-is-the-biggest-productivity) ⭐️ 8.0/10

该文章认为，强大的工程文化比 AI 更能驱动生产力，对当前围绕 AI 驱动生产力提升的炒作提出了挑战。其论点在从业者中引发了大量讨论，多个真实案例也印证了文化的重要性。 这一点很重要，因为许多组织正大力投资 AI 以提升生产力，却可能忽视了团队文化。这场讨论影响着工程领导者决定如何分配时间和资源，也凸显了文化往往是任何工具取得成功却被忽视的基础。 文章的论点得到了社区案例的支持：一位首席工程师提到，一个 20 人团队因成员彼此喜欢且流动率低而取得成功；另一位评论者则警告 AI 会加速功能失调。被提及的核心文化因素包括可预测性、市场薪酬和团队凝聚力。

hackernews · gpi · Aug 29, 17:19 · [社区讨论](https://news.ycombinator.com/item?id=49491568)

**背景**: 工程文化是指开发团队内共享的价值观、实践和社交动态。软件工程中的生产力在很大程度上受沟通、信任和稳定流程的影响。文章认为，当基础文化不佳时，AI 工具的影响力有限，而强大的文化则可以放大 AI 的益处。

**社区讨论**: 评论者大体认同但补充了细微差别：一位指出文化归根结底是可预测性和公平薪酬，另一位则警告 AI 会加速功能失调。一位首席工程师分享道，一个凝聚力强、流动率低的团队是他们经历过的最具生产力的团队，还有人认为 AI 的采用应自下而上。

**标签**: `#engineering-culture`, `#productivity`, `#leadership`, `#AI`, `#team-management`

---

<a id="item-3"></a>
## [DHS 利用鲜为人知的海关法窥探记者与非营利组织](https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits) ⭐️ 8.0/10

美国国土安全部（DHS）利用一项鲜为人知的海关执法法条（19 U.S.C. §1509）发出传票，获取记者、非营利组织和工会的通信记录。在数起案件中，DHS 在法庭上受到挑战后撤回了传票，而 T-Mobile 等公司选择配合，据报道谷歌则没有配合。 此事之所以重要，是因为它凸显了一种可绕开传统司法监督的监控权力正在扩大，威胁到新闻自由以及活动人士和工会免受政府监视的组织能力。这一做法已引起跨党派人士对隐私和公民自由的担忧。 这项权力原本用于海关执法，允许海关与边境保护局（CBP）在未经法院事先批准的情况下强制获取记录，而目标对象往往事后才收到通知。DHS 监察长 2017 年的报告已发现，CBP 偶尔滥用传票权力，且缺乏明确指引。

hackernews · firefax · Aug 29, 18:44 · [社区讨论](https://news.ycombinator.com/item?id=49492219)

**背景**: 根据《美国法典》第 19 编第 1509 条，美国海关与边境保护局（CBP）可在与海关有关的调查中发出行政传票，要求检查账簿和询问证人。与大陪审团传票不同，1509 传票不需要事先获得法官批准，而且当企业交出记录时，调查对象可能毫不知情。此前极少有在这种场景下使用该法律的报道，因此 DHS 对记者和非营利组织动用该手段的消息引发了警惕。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.law.cornell.edu/uscode/text/19/1509">19 U.S. Code § 1509 - Examination of books and witnesses</a></li>
<li><a href="https://www.oig.dhs.gov/news/press-releases/2017/11162017/dhs-oig-cites-cbp-misuse-summons-power">DHS OIG Cites CBP for Misuse of Summons Power | Office of Inspector General</a></li>
<li><a href="https://uscode.house.gov/view.xhtml?req=granuleid:USC-1999-title19-section1509&num=0&edition=1999">19 USC 1509: Examination of books and witnesses - House</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，1509 传票并非自动生效——目标方可以无视它，直到 DHS 诉请法院强制执行——因此，像 T-Mobile 这样不抵抗就配合的企业也负有部分责任。还有人认为，DHS 在受到质疑后撤回传票的做法，是一种蓄意避免不利司法裁决的策略。一些评论者则推荐去中心化的通信工具，作为记者的实际应对手段。

**标签**: `#surveillance`, `#privacy`, `#government`, `#law`, `#journalism`

---

<a id="item-4"></a>
## [中国拟将新能源车定型试验里程统一提高至 3 万公里](https://t.me/zaihuapd/43489) ⭐️ 8.0/10

全国汽标委就三项新能源汽车定型试验规程修改单公开征求意见，拟将纯电、混动及燃料电池车的可靠性行驶试验总里程翻倍至不低于 3 万公里，实现'油电同标'。 这项修改直接针对部分造车新势力'速成鸡'式地未经充分测试就密集推新车的乱象，将进一步压实企业质量责任。新规将迫使车企为每款新车型投入更长的测试周期和更高的研发成本，倒逼行业回归安全与品质底线。 纯电动车要求直流快充工况下的行驶里程占比不低于 90%（至少 2.7 万公里），以更充分考验三电系统在快充条件下的可靠性。插电混动车则新增了纯电模式单独跑满不少于 1 万公里的硬性指标，弥补了此前可主要靠发动机工况完成测试的漏洞。

telegram · zaihuapd · Aug 29, 13:30

**背景**: 定型试验是新车上市前必须通过的一项强制性验证流程，用于确认车辆在各种条件下的安全性与可靠性。'三电系统'——动力电池、驱动电机、电控系统——是新能源汽车的核心技术，直接决定其可靠性与安全性。直流快充通过大功率直流电为电池快速补电，相比交流慢充对电池和热管理系统的考验大得多。此前旧规只要求电动车按燃油车可靠性试验里程的 50%执行（即 1.5 万公里，下限 5000 公里），因此新的 3 万公里标准意味着'油电同标'。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/403047482">新能源汽车三电系统详解（电池、电机、电控） - 知乎</a></li>
<li><a href="https://post.smzdm.com/p/awwkz6gg/">电 车 可靠性 试 验 只跑油 车 一半，跑了21...</a></li>
<li><a href="https://longhaojiuding.com/news/9018370746.html">直 流 快 充 充 电桩：揭秘其技术核心与选型要点** - 临沂新能源有限公司</a></li>

</ul>
</details>

**标签**: `#EV regulation`, `#automotive testing`, `#policy`, `#reliability`, `#China`

---

<a id="item-5"></a>
## [索尼音乐等起诉 Anthropic：用盗版歌词与书籍训练 Claude](https://www.musicbusinessworldwide.com/files/2026/08/COMPLAINT-in-Sony_Music_Publishing_US_LLC_e.pdf) ⭐️ 8.0/10

索尼音乐出版、华纳查佩尔音乐等多家公司在美国加州联邦法院对 Anthropic 及其创始人提起诉讼，指控该公司从 LibGen、PiLiMi 等盗版库非法下载逾 700 万本书，并在删除版权管理信息后抓取歌词用于训练 Claude 模型。原告要求按每件作品最高 15 万美元计算法定赔偿，并申请永久禁令。 这起诉讼是对 AI 行业未经授权使用受版权保护材料训练模型这一做法的又一重大法律挑战，此前已有和解与判例在改变 AI 公司获取训练数据的方式。若原告胜诉，可能迫使 Anthropic 等公司支付数十亿美元赔偿，并采用更透明的数据来源管理机制。 起诉书明确点名 LibGen 和 PiLiMi 作为盗版书籍来源，并指控 Anthropic 抓取的歌词被删除了版权管理信息，这属于《数字千年版权法》(DMCA)项下的独立侵权行为。鉴于涉及据称超过 700 万本书，按每件作品 15 万美元的法定赔偿计算，总金额可能极为庞大；诉讼还将 Anthropic 的创始人列为被告。

telegram · zaihuapd · Aug 30, 01:00

**背景**: Anthropic 是开发 Claude 大语言模型系列的 AI 公司，其模型依赖于从互联网和其他来源抓取的海量文本进行训练。LibGen（Library Genesis）和 PiLiMi（Pirate Library Mirror）是影子图书馆，未经版权方授权提供盗版书籍和学术文献的免费访问。这起案件属于针对 AI 开发商的一系列版权诉讼浪潮的一部分——此前类似诉讼已促成据报道达 15 亿美元的和解——反映出出版方和创作者对训练数据中未经授权使用其作品的反击。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Library_Genesis">Library Genesis - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Shadow_library">Shadow library - Wikipedia</a></li>
<li><a href="https://www.6pages.com/glossary/piratelibrarymirror(pilimi)/">Pirate Library Mirror (PiLiMi) | 6Pages</a></li>

</ul>
</details>

**标签**: `#AI`, `#legal`, `#copyright`, `#Anthropic`, `#lawsuit`

---