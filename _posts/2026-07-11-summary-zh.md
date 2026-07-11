---
layout: default
title: "Horizon Summary: 2026-07-11 (ZH)"
date: 2026-07-11
lang: zh
---

> From 29 items, 11 important content pieces were selected

---

1. [苹果起诉 OpenAI 盗窃商业机密](#item-1) ⭐️ 9.0/10
2. [长征十号乙完成全球首次网系海上回收](#item-2) ⭐️ 9.0/10
3. [SGLang v0.5.15：GLM-5.2 在 Blackwell 上达 500+ tok/s](#item-3) ⭐️ 8.0/10
4. [QuadRF：开源射频相机可视化 WiFi 和无人机](#item-4) ⭐️ 8.0/10
5. [GPT-5.6 Sol Ultra 声称证明循环双覆盖猜想](#item-5) ⭐️ 8.0/10
6. [纽约市禁止欺骗性订阅行为](#item-6) ⭐️ 8.0/10
7. [腾讯洽购 Meta 旗下 AI 初创公司 Manus](#item-7) ⭐️ 8.0/10
8. [OpenAI 和谷歌向被列入黑名单的中国公司提供 AI 模型](#item-8) ⭐️ 8.0/10
9. [中国对氦气实施临时出口禁令](#item-9) ⭐️ 8.0/10
10. [Meta 或因成瘾设计被欧盟罚款 120 亿美元](#item-10) ⭐️ 8.0/10
11. [SK 海力士 CEO 预警 2027 年面临史上最严重内存短缺](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [苹果起诉 OpenAI 盗窃商业机密](https://9to5mac.com/2026/07/10/apple-sues-openai-trade-secret-theft/) ⭐️ 9.0/10

苹果提起诉讼，指控 OpenAI 通过前员工策划盗窃商业机密，包括指示求职者将苹果实物部件带到面试现场。 这一诉讼可能对 AI 行业产生重大影响，凸显了科技巨头之间在人才和知识产权方面的激烈竞争。同时，它也引发了对 OpenAI 伦理问题的质疑，并可能影响企业对其产品的采用。 苹果指控 OpenAI 指示新员工不告知苹果离职一事，并使用机密硬件信息接触苹果供应商。该诉讼有详细证据支持。

hackernews · stock_toaster · Jul 10, 20:47 · [社区讨论](https://news.ycombinator.com/item?id=48865019)

**背景**: 商业机密是赋予竞争优势的机密商业信息。苹果在研发上投入巨大，并保护其产品设计。在硅谷，涉及雇员跳槽的商业机密盗窃诉讼很常见。

**社区讨论**: 社区评论强烈谴责 OpenAI，许多用户认为证据确凿，预测将面临严重法律后果。一些人指出讽刺之处：OpenAI 本身曾面临内容抓取的指控，现在又被指控盗窃。

**标签**: `#Apple`, `#OpenAI`, `#trade secrets`, `#lawsuit`, `#corporate espionage`

---

<a id="item-2"></a>
## [长征十号乙完成全球首次网系海上回收](https://weibo.com/7340734455/R814of1Ki) ⭐️ 9.0/10

2026 年 7 月 10 日，长征十号乙运载火箭从海南商业航天发射场升空，并采用网系回收系统成功在海上回收其第一级，这是全球首次网系火箭回收。 这一突破显著推进了可重复使用火箭技术，降低了发射成本并增加了有效载荷能力，使中国在火箭回收领域与 SpaceX 并肩成为领导者。 网系回收使用滑轮驱动缆绳捕获第一级，简化了箭上结构并降低了飞行器质量。与传统的推进式着陆不同，该方法无需着陆腿，从而减轻了重量。

telegram · zaihuapd · Jul 10, 04:36

**背景**: 火箭回收是可重复使用发射系统的关键，通过重复使用昂贵部件降低单次发射成本。此前，SpaceX 的猎鹰 9 号采用海上平台推进着陆，而中国的长征十号乙引入了网捕方法。长征十号乙是长征十号系列的一个变体，专为载人月球任务设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Long_March_10B">Long March 10B - Wikipedia</a></li>
<li><a href="https://www.globaltimes.cn/page/202607/1365624.shtml?id=12">China enters rocket recovery era as experts highlight... - Global Times</a></li>
<li><a href="https://www.youtube.com/watch?v=2D_GstQJp0U">World's first : China recovers rocket booster with net system at sea ...</a></li>

</ul>
</details>

**标签**: `#rocket recovery`, `#aerospace`, `#long march 10b`, `#space technology`, `#china`

---

<a id="item-3"></a>
## [SGLang v0.5.15：GLM-5.2 在 Blackwell 上达 500+ tok/s](https://github.com/sgl-project/sglang/releases/tag/v0.5.15) ⭐️ 8.0/10

SGLang v0.5.15 针对 Blackwell GPU 上的 GLM-5.2 NVFP4 模型进行了生产级优化，在 8x B300 配置下实现了每用户每秒超过 500 token 的吞吐量。此版本还将 Spec V2 投机解码设为默认，引入了 IndexShare MTP 优化，并支持了 Hunyuan 3、Qwen3.6 等新模型。 这些性能提升使 SGLang 成为大规模部署大型语言模型的有力方案，尤其适用于 GLM-5.2 智能体和长上下文应用。Spec V2 和 IndexShare 优化降低了延迟并提高了吞吐量，为生产部署带来更低成本和更快响应。 Spec V2 通过零开销调度和融合操作实现了 11%的端到端吞吐量提升。IndexShare MTP 通过跨草案步骤重用索引器 top-k，在长上下文中将草案步骤成本降低最多 1.9 倍。该版本还默认启用可中断 CUDA Graph，并引入了针对 KDA 和 GDN 的线性注意力内核。

github · Fridge003 · Jul 10, 22:58

**背景**: SGLang 是一个开源的大型语言模型推理框架。投机解码通过使用更快的草稿模型生成候选 token，再由目标模型验证，从而加速生成。NVFP4 是 NVIDIA 的 4 位浮点精度格式，在效率和准确性之间取得平衡。Blackwell 指 NVIDIA 的下一代 GPU 架构（如 B300）。IndexShare 是一种用于稀疏注意力的跨层重用技术，可减少计算量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2211.17192">Fast Inference from Transformers via Speculative Decoding</a></li>
<li><a href="https://sebastianraschka.com/blog/2026/glm-5-2-indexshare.html">GLM-5.2 IndexShare Architecture Note | Sebastian Raschka, PhD</a></li>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision Inference | NVIDIA Technical Blog</a></li>

</ul>
</details>

**标签**: `#SGLang`, `#GPU inference`, `#speculative decoding`, `#production serving`, `#Blackwell`

---

<a id="item-4"></a>
## [QuadRF：开源射频相机可视化 WiFi 和无人机](https://www.jeffgeerling.com/blog/2026/quadrf-can-spot-drones-and-see-wifi-through-my-wall/) ⭐️ 8.0/10

QuadRF 是一个开源模块化 4x4 MIMO 软件定义无线电板，集成了树莓派 5，被演示为一种射频相机，可以检测无人机并透过墙壁绘制 WiFi 信号图。 该工具将相控阵射频感知民主化，使高级监控和频谱监测对爱好者、安全研究人员和教育工作者变得触手可及，可能提升对无线隐私和安全的意识。 QuadRF 作为实时射频相机运行，具有颜色编码的频率可视化功能，可识别如 WiFi 接入点和无人机等发射器的物理位置。它由树莓派 5 驱动，并采用开放式天线架构。

hackernews · speckx · Jul 10, 15:59 · [社区讨论](https://news.ycombinator.com/item?id=48861717)

**背景**: 软件定义无线电（SDR）是一种无线电通信系统，其中传统上的模拟组件（如混频器和滤波器）通过软件实现。QuadRF 将 SDR 与相控阵技术相结合，利用多天线在空间上分辨信号源。其开源特性允许用户自定义用户界面和处理流程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.crowdsupply.com/scale-rf/quadrf">QuadRF | Crowd Supply</a></li>
<li><a href="https://github.com/dustinbowers/QuadRF">GitHub - dustinbowers/QuadRF</a></li>
<li><a href="https://www.hackster.io/news/quadrf-the-open-source-rf-camera-that-lets-you-see-wi-fi-signals-141ad91f2a2d">QuadRF: The Open Source RF Camera That Lets You See Wi-Fi Signals</a></li>

</ul>
</details>

**社区讨论**: QuadRF 的创建者在评论中参与了互动，回答提问并指出根据反馈进行的改进。一些评论者对‘透过墙壁看到 WiFi’的说法表示不解，而其他人则讨论了潜在的政府监控能力以及与热成像相机的相似之处。

**标签**: `#RF sensing`, `#software-defined radio`, `#drone detection`, `#open source hardware`, `#security`

---

<a id="item-5"></a>
## [GPT-5.6 Sol Ultra 声称证明循环双覆盖猜想](https://cdn.openai.com/pdf/04d1d1e4-bc75-476a-97cf-49055cd98d31/cdc_proof.pdf) ⭐️ 8.0/10

OpenAI 于 2026 年 7 月 10 日发布了一份预印本，声称其 GPT-5.6 Sol Ultra 模型生成了图论中一个长期未解难题——循环双覆盖猜想的证明。 如果得到验证，这将是 AI 自主产生新颖数学证明能力的一个重要里程碑，可能改变数学和理论计算机科学的研究方式。 该证明极其简洁，暗示它利用了专家们未曾发现的巧妙技巧；在同行评审之前，社区仍持怀疑态度。提示中包含了详细指导，要求模型拒绝状态报告和模糊的乐观表态。

hackernews · scrlk · Jul 10, 18:29 · [社区讨论](https://news.ycombinator.com/item?id=48863490)

**背景**: 循环双覆盖猜想询问每个无桥无向图是否都存在一组环，使得每条边恰好出现两次。该猜想由 W.T. Tutte、Itai 和 Rodeh、George Szekeres 以及 Paul Seymour 提出，在图嵌入中等价于圆形嵌入猜想。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover">Cycle double cover - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者注意到提示中存在大量指导，有人观察到很多努力花在告诉模型真正解决问题上。另一个人指出大多数评论者并不关心这个猜想本身，因为过去对该话题的参与度很低。第三位评论者表示怀疑，指出证明的简洁性以及缺乏自主理论构建。

**标签**: `#AI`, `#graph theory`, `#proof`, `#LLM`, `#hype`

---

<a id="item-6"></a>
## [纽约市禁止欺骗性订阅行为](https://www.theguardian.com/us-news/2026/jul/10/new-york-city-deceptive-subscriptions-ban) ⭐️ 8.0/10

纽约市长马姆达尼宣布了一项具有里程碑意义的法律，禁止欺骗性订阅行为和附加费用，要求公司使取消订阅与注册一样简单。 这项法律保护消费者免受隐藏费用和难以取消订阅的困扰，树立了一个先例，可能会影响其他司法管辖区和全球运营的科技公司。 该法律包括'一键取消'要求，并禁止隐藏费用，如未披露的服务费或度假村费，与加州不同，没有为餐厅提供特别豁免。

hackernews · randycupertino · Jul 10, 18:26 · [社区讨论](https://news.ycombinator.com/item?id=48863464)

**背景**: 订阅模式被许多企业使用，从流媒体服务到健身房，通常带有自动续费和难以取消的流程。'水滴定价'和附加费用增加了隐藏成本，导致消费者不满和监管行动。

**社区讨论**: 评论者表达了谨慎乐观，但提出了执法担忧，指出加州类似法律有餐厅豁免。具体投诉包括 PayPal 的旧订阅和未披露的酒店度假费。一些人称赞此举是保护消费者的'合法政府'。

**标签**: `#regulation`, `#consumer protection`, `#subscriptions`, `#New York City`, `#junk fees`

---

<a id="item-7"></a>
## [腾讯洽购 Meta 旗下 AI 初创公司 Manus](https://www.reuters.com/technology/tencent-talks-become-ai-start-up-manus-largest-shareholder-ft-reports-2026-07-10/) ⭐️ 8.0/10

腾讯正在谈判收购 Meta 旗下的 AI 初创公司 Manus，计划成为其最大股东，此前北京要求 Meta 解除对 Manus 的 20 亿美元收购交易。 这笔交易标志着 AI 领域的重大转变，腾讯在地缘政治紧张局势下获得一家有前景的 AI 智能体初创公司的控制权，凸显了中美科技收购博弈。 据知情人士透露，腾讯将与原投资者真格基金和 HSG 联手，以不低于 20 亿美元的价格从 Meta 手中回购 Manus。

telegram · zaihuapd · Jul 10, 06:45

**背景**: Manus 是一套由蝴蝶效应（Butterfly Effect）开发的自主人工智能智能体，该公司创立于中国，总部设在新加坡。这家初创公司因能执行超越简单聊天机器人的任务而备受关注。Meta 此前已同意以 20 亿美元收购 Manus，但该交易被中国监管机构阻止，从而引发当前与腾讯的重新谈判。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus (AI agent) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Manus_AI">Manus AI</a></li>

</ul>
</details>

**标签**: `#Tencent`, `#AI startup`, `#acquisition`, `#Meta`, `#Manus`

---

<a id="item-8"></a>
## [OpenAI 和谷歌向被列入黑名单的中国公司提供 AI 模型](https://www.ft.com/content/5d6aafa1-5d47-4585-aa95-6ec06a6cd20f) ⭐️ 8.0/10

据《金融时报》报道，OpenAI 和谷歌一直通过新加坡子公司向阿里巴巴、百度和腾讯提供先进 AI 服务，这些中国科技巨头的母公司均被列入美国 1260H 黑名单。这些交易目前虽属合法，但已重新引发对 AI 模型实施更严格出口管制的呼声。 这一事件凸显了美国出口管制中的漏洞，因为中国公司可通过海外实体获取前沿 AI 模型，引发了国家安全担忧。这可能会加剧华盛顿关于是否对先进 AI 软件实施监管的辩论。 OpenAI 在发现疑似“模型蒸馏”行为后，暂停了阿里巴巴关联用户的 API 访问并上报美国政府。相比之下，Anthropic 的政策更为严格，全面禁止中国公司及其海外实体访问其前沿 AI 模型。

telegram · zaihuapd · Jul 10, 09:59

**背景**: 1260H 名单是美国国防部发布的所谓“中国军事企业”名单，相关实体可能面临经济制裁。模型蒸馏是一种机器学习技术，将大型“教师”模型的知识迁移到小型“学生”模型，使其更容易在性能较弱的硬件上部署。理解这些概念有助于把握这则新闻的影响，因为美国政府担心 AI 模型可能被用于军事目的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/1260H_list">1260H list</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_distillation">Model distillation</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#export controls`, `#geopolitics`, `#OpenAI`, `#Google`

---

<a id="item-9"></a>
## [中国对氦气实施临时出口禁令](https://wms.mofcom.gov.cn/zcfb/wmgl/art/2026/art_2a795a0d55df4cada91c9fbd2a2cc13a.html) ⭐️ 8.0/10

2026 年 7 月 10 日，中国商务部和海关总署宣布对氦气（海关商品编号 2804290010）实施临时禁止出口管理，立即生效，依据《中华人民共和国对外贸易法》。 鉴于中国是重要的氦气生产国，此禁令可能扰乱全球半导体制造、医学成像及其他高科技产业的关键供应链。 该禁令适用于海关编码 2804290010 的氦气，未指定结束日期；调整将另行公告。该公告由商务部和海关总署联合发布。

telegram · zaihuapd · Jul 10, 13:27

**背景**: 氦气是一种不可再生资源，对于冷却 MRI 机器中的超导磁体、作为半导体制造中的载气以及太空探索至关重要。中国是全球最大的氦气生产国之一，主要通过天然气加工获得；此次出口禁令延续了中国限制战略物资出口的趋势。

**标签**: `#helium`, `#export ban`, `#trade policy`, `#supply chain`, `#semiconductor`

---

<a id="item-10"></a>
## [Meta 或因成瘾设计被欧盟罚款 120 亿美元](https://www.theverge.com/policy/963872/meta-eu-addictive-design-200b-fine-risk-digital-services-act-dsa) ⭐️ 8.0/10

欧盟委员会初步认定，Meta 旗下 Facebook 和 Instagram 的成瘾性设计违反《数字服务法》，可能导致高达 120 亿美元的罚款，并被要求重新设计应用。 此举可能为根据《数字服务法》监管成瘾性技术树立重要先例，迫使 Meta 及其他平台减少以用户参与为导向的功能，更好地保护用户心理健康。 欧盟批评 Meta 提供的限时工具形同虚设，建议的重新设计包括默认关闭无限滚动和自动播放、设置有效的屏幕休息时间，以及减少以参与度为导向的算法推荐。

telegram · zaihuapd · Jul 10, 14:47

**背景**: 《数字服务法》（DSA）是欧盟的一项法规，对大型在线平台，尤其是拥有超过 4500 万欧盟用户的超大型在线平台（VLOP），施加严格的问责和透明度要求。成瘾性设计指无限滚动、自动播放等功能，这些功能故意设计以最大化用户参与度和在平台上的停留时间，往往以用户福祉为代价。DSA 的风险评估义务要求平台减轻系统性风险，例如对心理健康的负面影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Services_Act">Digital Services Act</a></li>
<li><a href="https://digital-strategy.ec.europa.eu/en/policies/digital-services-act">The Digital Services Act | Shaping Europe’s digital future</a></li>
<li><a href="https://algorithmwatch.org/en/dsa-explained/">A guide to the Digital Services Act, the EU’s law to rein in Big Tech - AlgorithmWatch</a></li>

</ul>
</details>

**标签**: `#Meta`, `#EU Regulation`, `#Digital Services Act`, `#Addictive Design`, `#Tech Policy`

---

<a id="item-11"></a>
## [SK 海力士 CEO 预警 2027 年面临史上最严重内存短缺](https://www.reuters.com/world/asia-pacific/sk-hynix-ceo-sees-worst-ever-memory-supply-shortage-2027-says-demand-outstrip-2026-07-10/) ⭐️ 8.0/10

SK 海力士 CEO 郭鲁正警告，全球内存行业将在 2027 年遭遇史上最严重的供应短缺，即使积极扩产，客户需求在 2030 年后仍将超过供应能力。 这一来自主要内存制造商的预测预示着可能出现价格飙升和供应紧张，影响人工智能、数据中心和消费电子产品，从而波及整个科技供应链。 SK 海力士正在考虑在美国、日本和东南亚建设海外晶圆厂，优先选择土地、电力和人力成本最具优势的地区。该公司 2025 年营业利润达创纪录的 47 万亿韩元。

telegram · zaihuapd · Jul 11, 00:45

**背景**: 内存芯片行业具有周期性，供需波动受需求变化和产能投资影响。近年来，AI 和数据中心的需求激增，导致供应紧张。SK 海力士是用于 AI 加速器的高带宽内存（HBM）的主要供应商。

**标签**: `#memory shortage`, `#semiconductor`, `#SK Hynix`, `#supply chain`, `#industry forecast`

---