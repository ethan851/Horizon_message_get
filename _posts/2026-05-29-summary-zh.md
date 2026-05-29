---
layout: default
title: "Horizon Summary: 2026-05-29 (ZH)"
date: 2026-05-29
lang: zh
---

> From 32 items, 11 important content pieces were selected

---

1. [Anthropic 以 9650 亿美元估值完成 650 亿美元 H 轮融资](#item-1) ⭐️ 9.0/10
2. [高通与字节跳动合作定制 AI ASIC 芯片](#item-2) ⭐️ 9.0/10
3. [仅用 Postgres 构建持久工作流](#item-3) ⭐️ 8.0/10
4. [GitHub 因发布零日漏洞封禁研究员](#item-4) ⭐️ 8.0/10
5. [LLM 写作痕迹：语言模式汇编](#item-5) ⭐️ 8.0/10
6. [黄仁勋称台湾为 AI 革命中心，英伟达年投 1500 亿美元](#item-6) ⭐️ 8.0/10
7. [中国将为人形机器人分配数字 ID](#item-7) ⭐️ 8.0/10
8. [索尼发布 Bravia 9 II 和 7 II，采用独立 RGB LED 背光](#item-8) ⭐️ 8.0/10
9. [比亚迪发布 4nm 智驾芯片'璇玑 A3'](#item-9) ⭐️ 8.0/10
10. [美国司法部要求 Reddit 和 X 披露匿名 ICE 批评者身份](#item-10) ⭐️ 8.0/10
11. [比亚迪为城市领航辅助驾驶提供一年事故兜底](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic 以 9650 亿美元估值完成 650 亿美元 H 轮融资](https://www.anthropic.com/news/series-h) ⭐️ 9.0/10

Anthropic 宣布完成 650 亿美元的 H 轮融资，由 Altimeter Capital、Dragoneer、Greenoaks、Sequoia Capital 等领投，投后估值达 9650 亿美元。该公司还报告称，其年化运行收入（run-rate revenue）在本月初已超过 470 亿美元。 这轮巨额融资和收入运行率表明 Anthropic 在估值和收入上已超越 OpenAI，标志着 AI 行业格局的重大转变。这凸显了投资者对 Anthropic 增长轨迹及其在 AI 初创公司中领先地位的强烈信心。 470 亿美元的年化运行收入是基于最近月度或季度收入的年化预测，并非实际年收入。H 轮融资由 Altimeter Capital、Dragoneer、Greenoaks 和 Sequoia Capital 等顶级风投机构联合领投。

hackernews · meetpateltech · May 28, 18:09 · [社区讨论](https://news.ycombinator.com/item?id=48313048)

**背景**: H 轮融资是针对成熟公司的晚期投资轮次，这些公司已经历了早期融资阶段。年化运行收入是一种财务指标，将短期（如一个月或一个季度）的当前收入外推以估算年收入，常用于快速增长的公司以显示其增长轨迹。投后估值是投资后公司的估计价值，计算公式为投前估值加上新投资金额。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/sectors/technology/articles/anthropic-raises-65b-series-h-184801308.html">Anthropic raises $65B in Series H funding at $965B valuation</a></li>
<li><a href="https://www.investopedia.com/terms/r/runrate.asp">Run Rate Explained: Benefits, Risks, and Business Insights</a></li>
<li><a href="https://en.wikipedia.org/wiki/Post-money_valuation">Post-money valuation</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 Anthropic 在收入运行率和估值上均已超越 OpenAI，一些人认为 OpenAI 日益不稳。其他人则质疑年化运行收入的含义，并对潜在 IPO 前的超高私有估值表示惊讶。还有一些评论指出这些成本最终由消费者和投资者承担。

**标签**: `#Anthropic`, `#funding`, `#AI`, `#valuation`, `#OpenAI`

---

<a id="item-2"></a>
## [高通与字节跳动合作定制 AI ASIC 芯片](https://t.me/zaihuapd/41616) ⭐️ 9.0/10

高通已与字节跳动达成协议，共同开发定制 AI ASIC 芯片，字节跳动计划采购数百万颗此类芯片，用于支持其 AI 服务的算力需求。 此次合作凸显了科技巨头为 AI 工作负载设计定制芯片、减少对通用 GPU 依赖的趋势。它可能重塑 AI 硬件供应链，并为字节跳动在 AI 推理效率方面带来竞争优势。 高通曾在 4 月底宣布，将于今年向某超大规模云服务商交付首款 ASIC，但双方均未正式确认此交易。该合作还将帮助字节跳动将其内部芯片设计转化为可量产的半导体产品。

telegram · zaihuapd · May 28, 07:09

**背景**: ASIC（专用集成电路）是一种为特定任务而非通用计算设计的芯片。在 AI 领域，谷歌等公司使用张量处理单元（TPU），这是专为神经网络推理和训练优化的 ASIC。定制 AI ASIC 在专用工作负载上相比通用 GPU 能提供更好的性能、更低的功耗和更低的成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tensor_Processing_Unit">Tensor Processing Unit - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#ASIC`, `#Qualcomm`, `#ByteDance`, `#chip design`

---

<a id="item-3"></a>
## [仅用 Postgres 构建持久工作流](https://www.dbos.dev/blog/postgres-is-all-you-need-for-durable-execution) ⭐️ 8.0/10

一篇博客文章主张仅使用 PostgreSQL 即可构建持久工作流，无需 Temporal 或 Restate 等专用工作流引擎。 这种方法可通过减少外部依赖、降低运营成本并利用现有 PostgreSQL 投资来简化系统架构。 所提出的方法利用 PostgreSQL 的 ACID 事务、NOTIFY/LISTEN 或类队列表来实现持久执行模式，避免了单独工作流引擎的开销。

hackernews · KraftyOne · May 28, 18:41 · [社区讨论](https://news.ycombinator.com/item?id=48313530)

**背景**: 持久执行确保工作流状态在故障后仍然保留，通常由 Temporal 等框架提供。PostgreSQL 是一个具有强一致性和可靠性的关系数据库，可以同时作为工作流的存储和协调层。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://temporal.io/">Durable Execution Solutions | Temporal</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了替代实现，如 pgque（使用快照/截断减少膨胀）和 absurd（原生的 Postgres 工作流引擎）。一些用户分享了比较 DBOS、Restate 和 Cloudflare 工作流的实际经验，指出了在可靠性、成本和速度方面的权衡。

**标签**: `#PostgreSQL`, `#workflows`, `#durable execution`, `#distributed systems`

---

<a id="item-4"></a>
## [GitHub 因发布零日漏洞封禁研究员](https://www.tomshardware.com/tech-industry/cyber-security/microsofts-github-bans-security-researcher-who-posted-zero-day-windows-exploits-because-company-ruined-their-life-expert-claims-action-is-vindictive-and-promises-further-retaliation) ⭐️ 8.0/10

微软旗下的 GitHub 平台封禁了一名安全研究员，该研究员公开了针对 Windows 的零日漏洞利用代码，其声称遭到微软漏洞赏金计划的不公正对待，并誓言将进一步报复。 此事件凸显了安全研究员与大型平台在漏洞披露、漏洞赏金报酬和平台治理方面的紧张关系，可能削弱负责任披露的积极性，促使研究员转向黑市出售漏洞利用程序。 该研究员声称微软毁了自己的生活，并承诺进一步报复；有专家称此次封禁是报复行为。据报道，该研究员使用了 AI 技术发现这些零日漏洞。

hackernews · possibilistic · May 28, 21:45 · [社区讨论](https://news.ycombinator.com/item?id=48315968)

**背景**: 零日漏洞利用指软件厂商未知的漏洞，攻击者可在补丁发布前加以利用。漏洞赏金计划是一种众包安全举措，企业奖励负责任披露漏洞的研究人员。微软有自己的漏洞赏金计划，但报酬和披露政策可能引发争议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/zero-day">What is a Zero-Day Exploit? | IBM</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bug_bounty_program">Bug bounty program</a></li>

</ul>
</details>

**社区讨论**: 评论者担心微软此举可能促使该研究员将漏洞利用程序出售给其他方，也有人指出该研究员似乎带有个人仇恨，并质疑 AI 在发现零日漏洞中的作用。有人认为漏洞赏金计划通常有支付激励，但此案似乎是个例外。

**标签**: `#cybersecurity`, `#zero-day`, `#GitHub`, `#Microsoft`, `#bug bounty`

---

<a id="item-5"></a>
## [LLM 写作痕迹：语言模式汇编](https://shvbsle.in/various-llm-smells/) ⭐️ 8.0/10

一篇名为《Various LLM Smells》的博客文章整理了大型语言模型生成文本中常见的语言和风格模式，例如“honest caveat:”和“load bearing”。 随着 LLM 生成文本越来越普遍，能够识别它们对于保持写作的真实性和检测潜在错误信息至关重要。这份汇编为研究人员、写作者和日常用户提供了实用的启发式方法。 该文章列出了诸如“(The) honest caveat:”、非建筑领域的“load bearing”、非爆炸领域的“blast radius”等特定短语，以及对立否定结构（如“It’s not X, it’s Y”）。社区讨论进一步指出，LLM 写作只有在读者不擅长的领域才显得更优秀。

hackernews · speckx · May 28, 19:02 · [社区讨论](https://news.ycombinator.com/item?id=48313810)

**背景**: 文体计量学（Stylometry）是研究语言风格的学科，常用于作者归属。近期研究表明，LLM 生成文本表现出独特的风格特征，可通过自动化分析检测。“气味”方法是一种基于模式的启发式方法，类似于软件工程中的代码气味，但应用于自然语言。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rmoff.net/2025/11/25/ai-smells-on-medium/">(AI) Smells on Medium</a></li>
<li><a href="https://www.nature.com/articles/s41599-025-05986-3">Stylometric comparisons of human versus AI-generated creative writing | Humanities and Social Sciences Communications</a></li>

</ul>
</details>

**社区讨论**: 社区成员贡献了更多痕迹，包括“load bearing”、“blast radius”和对立否定模式。一位评论者警告说，LLM 写作只有在读者不擅长的领域才显得显著优秀，这使得非专家更难检测。另一位建议将 LLM 用于批评而非直接复制输出，以保持个人风格。

**标签**: `#LLM`, `#AI-generated text`, `#writing style`, `#heuristics`, `#machine learning`

---

<a id="item-6"></a>
## [黄仁勋称台湾为 AI 革命中心，英伟达年投 1500 亿美元](https://arstechnica.com/tech-policy/2026/05/nvidia-ceo-wants-taiwan-to-be-center-of-ai-revolution-not-us/) ⭐️ 8.0/10

英伟达 CEO 黄仁勋称台湾为 AI 革命中心，并宣布计划每年在台湾投入约 1500 亿美元，覆盖 AI 芯片生产、系统制造和供应链合作。 这一巨额投资凸显了台湾在全球 AI 硬件供应链中的关键地位，可能重塑半导体制造领域的投资流向和地缘政治格局。 英伟达在台北的新总部预计今年动工、2030 年启用，可容纳 4000 名员工。主要合作伙伴包括台积电、鸿海（富士康）、纬创和广达。

telegram · zaihuapd · May 28, 07:33

**背景**: 英伟达是全球领先的 AI 芯片设计公司，而台湾以台积电先进制造为核心的半导体生态系统是其芯片生产的关键。这项投资较此前每年 100-150 亿美元的规模大幅升级。

**标签**: `#英伟达`, `#AI供应链`, `#台湾`, `#投资`, `#芯片制造`

---

<a id="item-7"></a>
## [中国将为人形机器人分配数字 ID](https://www.scmp.com/tech/policy/article/3354747/china-give-every-humanoid-robot-digital-id-push-boost-industry-standards) ⭐️ 8.0/10

中国工业和信息化部推出了“人形机器人全生命周期管理服务平台”，将为所有国内制造的人形机器人分配唯一数字 ID，实现从生产到回收的全流程追踪。 这一举措标准化了人形机器人的治理，提升了可追溯性、安全监控和责任归属，同时将中国定位为 AI 机器人监管领域的领导者。 数字 ID 系统由四段编码构成，对中国制造的所有人形机器人强制实施，已有来自 100 多家公司的超过 28,000 台机器人完成注册。

telegram · zaihuapd · May 28, 09:08

**背景**: 人形机器人是仿照人类身体形状设计的机器人，常用于与人类环境和工具交互。工信部于 2025 年底成立了人形机器人与具身智能标准化技术委员会，以系统推进标准制定。数字 ID 系统是该标准的关键部分，用于确保全生命周期管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.breezyscroll.com/technology-news/china-humanoid-robot-digital-identity-system/">China To Assign Official IDs To Humanoid Robots Just... - BreezyScroll</a></li>
<li><a href="https://www.biometricupdate.com/202605/china-creates-digital-id-for-humanoid-robots">China creates digital ID for humanoid robots | Biometric Update</a></li>
<li><a href="https://www.globaltimes.cn/page/202512/1351625.shtml">China’s MIIT sets up standardization committee for humanoid robots to reinforce sector’s global competitiveness - Global Times</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#humanoid robots`, `#regulation`, `#standards`, `#China`

---

<a id="item-8"></a>
## [索尼发布 Bravia 9 II 和 7 II，采用独立 RGB LED 背光](https://www.flatpanelshd.com/news.php?subaction=showfull&amp;id=1779897602) ⭐️ 8.0/10

索尼于 5 月 27 日正式推出 2026 年旗舰液晶电视 Bravia 9 II 和 Bravia 7 II，首次在消费电视中采用名为“True RGB”的独立红绿蓝 LED 背光技术。 这一突破实现了近 4000 尼特的峰值亮度和超过 90% 的 BT.2020 色域覆盖，融合了 Mini LED 的亮度与 OLED 般的色彩纯净度，有望为高端液晶电视树立新标杆。 该系列涵盖 50 至 115 英寸多个尺寸，包括全新的 115 英寸巨幕型号，但高端机型仍仅提供两个 HDMI 2.1 接口，且不支持杜比视界 2。索尼自 2004 年首款 RGB LED 电视以来积累了丰富的背光控制经验。

telegram · zaihuapd · May 28, 12:15

**背景**: 传统液晶电视使用白色 LED 背光搭配彩色滤光片来产生颜色。相比之下，RGB LED 背光直接发射红、绿、蓝光，无需依赖量子点即可实现更纯净的色彩和更广的色域。索尼早在 2004 年就尝试过这一方案，但直到现在才将其带入大众消费电视，并结合现代 Mini LED 技术实现高亮度和精准的局部调光。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/16871815855">【科普】RGB-MiniLED电视显示技术详解 - 知乎</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/16968539822">【真机科普】什么是RGB-Mini LED电视？海信RGB三维控色液晶显示技术原理；RGB MiniLED与OLED和MiniLED电视差异，一文看懂！ - 知乎</a></li>
<li><a href="https://display.ofweek.com/2025-04/ART-230001-8500-30660617.html">电视巨头为何纷纷押注 RGB-Mini LED？ - OFweek显示网</a></li>

</ul>
</details>

**标签**: `#显示技术`, `#电视`, `#消费电子`, `#RGB LED`, `#索尼`

---

<a id="item-9"></a>
## [比亚迪发布 4nm 智驾芯片'璇玑 A3'](https://finance.sina.com.cn/roll/2026-05-28/doc-inhznenn1371824.shtml) ⭐️ 8.0/10

比亚迪在 5 月 28 日的'敢为'智能化战略发布会上发布了'璇玑 A3'，这是一款 4nm 工艺的智驾芯片，已实现规模化量产，支持 L3/L4 级自动驾驶，三颗芯片总算力超过 2100 TOPS。 这标志着比亚迪在垂直整合方面的重大进展，减少了对外部芯片供应商的依赖，并使其成为高端自动驾驶领域的关键参与者。4nm 工艺和高算力可能加速 L3/L4 功能在经济型电动车中的大规模普及。 该芯片结合比亚迪自研算法优化，声称算力利用率提升 100%。比亚迪还宣布已推出 2000 多款芯片产品，并拥有 5 座晶圆工厂。

telegram · zaihuapd · May 28, 13:01

**背景**: 自动驾驶芯片是处理传感器数据和决策的专用处理器。4nm 工艺指晶体管尺寸，能实现更高性能和能效。L3 级自动驾驶允许有条件地松开方向盘，L4 级可在特定区域无需驾驶员干预。TOPS（每秒万亿次运算）衡量 AI 算力，2100 TOPS 在车载芯片中处于顶级水平。

**标签**: `#autonomous driving`, `#semiconductor`, `#BYD`, `#chip`

---

<a id="item-10"></a>
## [美国司法部要求 Reddit 和 X 披露匿名 ICE 批评者身份](https://www.bloomberg.com/news/articles/2026-05-28/trump-s-doj-ramps-up-probes-of-anonymous-ice-critics-with-x-reddit-subpoenas) ⭐️ 8.0/10

美国司法部向 Reddit 和 X 发出大陪审团传票，要求提供至少两名匿名用户的真实姓名、地址和银行信息，这些用户曾批评美国移民和海关执法局（ICE）的执法行动。 此举加剧了政府调查与网络匿名性之间的冲突，可能对言论自由产生寒蝉效应，并为科技平台在法律压力下如何处理用户隐私树立先例。 传票已从行政传唤升级为大陪审团传票，理由是基于刑事调查，但用户尚未被告知具体涉嫌何种罪名。法官目前正在审理撤销传票的请求。

telegram · zaihuapd · May 28, 14:22

**背景**: 美国移民和海关执法局（ICE）因其执法行动而受到公众批评。司法部可以发出传票，强制平台披露用户信息。大陪审团传票比行政传票具有更大的法律效力，不遵守可能导致藐视法庭指控。

**标签**: `#US DOJ`, `#ICE`, `#Reddit`, `#X`, `#privacy`

---

<a id="item-11"></a>
## [比亚迪为城市领航辅助驾驶提供一年事故兜底](https://news.mydrivers.com/1/1125/1125729.htm) ⭐️ 8.0/10

比亚迪宣布，即日起为搭载天神之眼 A、B 的新车用户提供一年事故兜底，在城市领航辅助驾驶期间发生事故，比亚迪赔付本车应承担的经济损失，不设上限。老车主通过 OTA 升级到天神之眼 5.0 后也可享受该保障。 该政策可能为自动驾驶责任标准树立先例，增强消费者对辅助驾驶功能的信任，并促使其他车企提供类似保障。这也与比亚迪将高阶智驾系统普及到全系车型的战略一致。 该保障仅适用于城市领航辅助驾驶场景，且只赔付本车应承担的部分，不设上限。天神之眼 C 作为低配版本，新车选装价为 12000 元。

telegram · zaihuapd · May 29, 01:03

**背景**: 城市领航辅助驾驶（常称为城市 NOA）是一种高级驾驶辅助功能，可在城市道路中处理复杂路口、变道和交通信号，但驾驶员仍需保持监控。比亚迪的“天神之眼”是其自主研发的智驾系统，分为 A、B、C 不同等级。辅助驾驶事故中的责任划分一直是争议焦点，比亚迪主动承担本车责任部分，在业内尚属首次。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech.ifeng.com/c/8tVfo97r5TA">比亚迪发布4nm制程智 驾 芯片，为 城 市 领 航 安全兜底无赔付上限_凤凰网</a></li>
<li><a href="https://www.caixinglobal.com/2025-02-28/caixin-weekly-byd-reaches-new-heights-launches-another-smart-driving-offensive-in-the-new-year-102293276.html">BYD Reaches New Heights, Launches Another Smart Driving Offensive in the New Year</a></li>

</ul>
</details>

**标签**: `#autonomous driving`, `#BYD`, `#liability`, `#ADAS`, `#electric vehicles`

---