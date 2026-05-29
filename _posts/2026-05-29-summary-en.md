---
layout: default
title: "Horizon Summary: 2026-05-29 (EN)"
date: 2026-05-29
lang: en
---

> From 32 items, 11 important content pieces were selected

---

1. [Anthropic raises $65B in Series H at $965B valuation](#item-1) ⭐️ 9.0/10
2. [Qualcomm and ByteDance Partner for Custom AI ASICs](#item-2) ⭐️ 9.0/10
3. [Postgres-Only Durable Workflows](#item-3) ⭐️ 8.0/10
4. [GitHub bans researcher for posting zero-day exploits](#item-4) ⭐️ 8.0/10
5. [LLM Writing Tells: A Compilation of Linguistic Patterns](#item-5) ⭐️ 8.0/10
6. [NVIDIA CEO: Taiwan is AI Revolution Center, $150B Annual Investment](#item-6) ⭐️ 8.0/10
7. [China to Assign Digital IDs to Humanoid Robots](#item-7) ⭐️ 8.0/10
8. [Sony Unveils Bravia 9 II & 7 II with RGB LED Backlight](#item-8) ⭐️ 8.0/10
9. [BYD Unveils 4nm 'Xuanji A3' Chip for Autonomous Driving](#item-9) ⭐️ 8.0/10
10. [US DOJ Demands Reddit and X Disclose Anonymous ICE Critics](#item-10) ⭐️ 8.0/10
11. [BYD offers one-year accident liability coverage for city NOA](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic raises $65B in Series H at $965B valuation](https://www.anthropic.com/news/series-h) ⭐️ 9.0/10

Anthropic announced a $65 billion Series H funding round, led by Altimeter Capital, Dragoneer, Greenoaks, Sequoia Capital, and others, at a $965 billion post-money valuation. The company also reported that its run-rate revenue surpassed $47 billion earlier this month. This massive funding round and revenue run-rate signal that Anthropic has surpassed OpenAI in valuation and revenue, indicating a major shift in the AI industry landscape. It underscores strong investor confidence in Anthropic's growth trajectory and its leading position among AI startups. The run-rate revenue of $47 billion is an annualized projection based on recent monthly or quarterly revenue, not actual annual revenue. The Series H round was led by a consortium of top venture capital firms including Altimeter Capital, Dragoneer, Greenoaks, and Sequoia Capital.

hackernews · meetpateltech · May 28, 18:09 · [Discussion](https://news.ycombinator.com/item?id=48313048)

**Background**: Series H funding is a late-stage investment round for mature companies that have already gone through earlier funding stages. Run-rate revenue is a financial metric that extrapolates current revenue over a short period (e.g., a month or quarter) to estimate annual revenue, commonly used by fast-growing companies to indicate their growth trajectory. Post-money valuation is the company's estimated value after the investment is made, calculated as pre-money valuation plus the new investment amount.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/sectors/technology/articles/anthropic-raises-65b-series-h-184801308.html">Anthropic raises $65B in Series H funding at $965B valuation</a></li>
<li><a href="https://www.investopedia.com/terms/r/runrate.asp">Run Rate Explained: Benefits, Risks, and Business Insights</a></li>
<li><a href="https://en.wikipedia.org/wiki/Post-money_valuation">Post-money valuation</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Anthropic has surpassed OpenAI in both revenue run-rate and valuation, with some viewing OpenAI as increasingly shaky. Others questioned the meaning of run-rate revenue and expressed astonishment at the high private valuation before a potential IPO. A few comments also pointed out that these costs are ultimately borne by consumers and investors.

**Tags**: `#Anthropic`, `#funding`, `#AI`, `#valuation`, `#OpenAI`

---

<a id="item-2"></a>
## [Qualcomm and ByteDance Partner for Custom AI ASICs](https://t.me/zaihuapd/41616) ⭐️ 9.0/10

Qualcomm has reached an agreement with ByteDance to develop custom AI ASIC chips, with ByteDance planning to purchase millions of these chips to power its AI services. This partnership underscores a growing trend among tech giants to design custom silicon for AI workloads, reducing reliance on off-the-shelf GPUs. It could reshape the AI hardware supply chain and give ByteDance a competitive edge in AI inference efficiency. Qualcomm had previously announced in late April that it would deliver its first ASIC to a hyperscale cloud provider this year, though neither company has officially confirmed the deal. The partnership would also help ByteDance turn its internal chip designs into mass-producible semiconductors.

telegram · zaihuapd · May 28, 07:09

**Background**: An ASIC (Application-Specific Integrated Circuit) is a chip designed for a specific task rather than general-purpose computing. In AI, companies like Google use Tensor Processing Units (TPUs), which are ASICs optimized for neural network inference and training. Custom AI ASICs can offer better performance, lower power consumption, and reduced cost compared to general-purpose GPUs for dedicated workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tensor_Processing_Unit">Tensor Processing Unit - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#ASIC`, `#Qualcomm`, `#ByteDance`, `#chip design`

---

<a id="item-3"></a>
## [Postgres-Only Durable Workflows](https://www.dbos.dev/blog/postgres-is-all-you-need-for-durable-execution) ⭐️ 8.0/10

A blog post argues that PostgreSQL alone is sufficient for building durable workflows, eliminating the need for specialized workflow engines like Temporal or Restate. This approach could simplify system architectures by reducing external dependencies, lowering operational costs, and leveraging existing PostgreSQL investments. The proposed method uses PostgreSQL's ACID transactions, NOTIFY/LISTEN, or queue-like tables to implement durable execution patterns, avoiding the overhead of separate workflow engines.

hackernews · KraftyOne · May 28, 18:41 · [Discussion](https://news.ycombinator.com/item?id=48313530)

**Background**: Durable execution ensures workflow state persists across failures, typically provided by frameworks like Temporal. PostgreSQL is a relational database with strong consistency and reliability, which can serve as both storage and coordination layer for workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://temporal.io/">Durable Execution Solutions | Temporal</a></li>

</ul>
</details>

**Discussion**: Commenters shared alternative implementations like pgque (using snapshot/truncate to avoid bloat) and absurd (a Postgres-native workflow engine). Some users shared practical experiences comparing DBOS, Restate, and Cloudflare workflows, noting trade-offs in reliability, cost, and speed.

**Tags**: `#PostgreSQL`, `#workflows`, `#durable execution`, `#distributed systems`

---

<a id="item-4"></a>
## [GitHub bans researcher for posting zero-day exploits](https://www.tomshardware.com/tech-industry/cyber-security/microsofts-github-bans-security-researcher-who-posted-zero-day-windows-exploits-because-company-ruined-their-life-expert-claims-action-is-vindictive-and-promises-further-retaliation) ⭐️ 8.0/10

Microsoft's GitHub platform banned a security researcher who publicly posted zero-day exploits for Windows, after the researcher claimed unfair treatment by Microsoft's bug bounty program and vowed further retaliation. This incident highlights tensions between security researchers and major platforms over vulnerability disclosure, bug bounty compensation, and platform governance, potentially chilling responsible disclosure and pushing researchers to sell exploits on the black market. The researcher claimed Microsoft ruined their life and promised further retaliation; an expert described the ban as vindictive. The researcher reportedly used AI to discover the zero-day vulnerabilities.

hackernews · possibilistic · May 28, 21:45 · [Discussion](https://news.ycombinator.com/item?id=48315968)

**Background**: A zero-day exploit refers to a vulnerability unknown to the software vendor, which attackers can exploit before a patch is available. Bug bounty programs are crowdsourced initiatives where companies reward researchers for responsibly disclosing vulnerabilities. Microsoft runs its own bug bounty program, but disputes can arise over compensation and disclosure policies.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/zero-day">What is a Zero-Day Exploit? | IBM</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bug_bounty_program">Bug bounty program</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern that Microsoft's action might push the researcher to sell exploits elsewhere, while others noted the researcher seemed to have a personal vendetta and questioned the role of AI in finding zero-days. Some argued that bug bounty programs typically incentivize payouts, but this case appears exceptional.

**Tags**: `#cybersecurity`, `#zero-day`, `#GitHub`, `#Microsoft`, `#bug bounty`

---

<a id="item-5"></a>
## [LLM Writing Tells: A Compilation of Linguistic Patterns](https://shvbsle.in/various-llm-smells/) ⭐️ 8.0/10

A blog post titled 'Various LLM Smells' compiles a list of linguistic and stylistic patterns that often appear in text generated by large language models, such as 'honest caveat:' and 'load bearing'. As LLM-generated text becomes more prevalent, being able to identify it is crucial for maintaining authenticity in writing and for detecting potential misinformation. This compilation provides practical heuristics for researchers, writers, and everyday users. The post lists specific phrases like '(The) honest caveat:', 'load bearing' (outside architecture), and 'blast radius' (outside explosives), as well as patterns like contrastive negation ('It’s not X, it’s Y'). The community discussion adds further insights, noting that LLM writing feels superior only in areas where the reader lacks expertise.

hackernews · speckx · May 28, 19:02 · [Discussion](https://news.ycombinator.com/item?id=48313810)

**Background**: Stylometry is the study of linguistic style, often used for authorship attribution. Recent research shows that LLM-generated text exhibits distinct stylistic features that can be detected through automated analysis. The 'smells' approach is a heuristic, pattern-based method similar to code smells in software engineering, but applied to natural language.

<details><summary>References</summary>
<ul>
<li><a href="https://rmoff.net/2025/11/25/ai-smells-on-medium/">(AI) Smells on Medium</a></li>
<li><a href="https://www.nature.com/articles/s41599-025-05986-3">Stylometric comparisons of human versus AI-generated creative writing | Humanities and Social Sciences Communications</a></li>

</ul>
</details>

**Discussion**: Community members contributed additional tells, including 'load bearing', 'blast radius', and contrastive negation patterns. One commenter warned that LLM writing feels significantly better only in domains where the reader is not an expert, making detection harder for non-experts. Another suggested using LLMs for critique rather than directly copying output to preserve personal style.

**Tags**: `#LLM`, `#AI-generated text`, `#writing style`, `#heuristics`, `#machine learning`

---

<a id="item-6"></a>
## [NVIDIA CEO: Taiwan is AI Revolution Center, $150B Annual Investment](https://arstechnica.com/tech-policy/2026/05/nvidia-ceo-wants-taiwan-to-be-center-of-ai-revolution-not-us/) ⭐️ 8.0/10

NVIDIA CEO Jensen Huang declared Taiwan the center of the AI revolution and announced plans to invest approximately $150 billion annually in the region, covering AI chip production, system manufacturing, and supply chain partnerships. This massive investment underscores Taiwan's critical role in the global AI hardware supply chain, potentially reshaping investment flows and geopolitical dynamics in semiconductor manufacturing. NVIDIA's new headquarters in Taipei is expected to break ground this year and open by 2030, housing 4,000 employees. Key partners include TSMC, Hon Hai (Foxconn), Wistron, and Quanta.

telegram · zaihuapd · May 28, 07:33

**Background**: NVIDIA is a leading designer of AI chips, and Taiwan's semiconductor ecosystem, anchored by TSMC's advanced manufacturing, is central to producing those chips. The investment represents a significant escalation from previous annual investments of $10-15 billion.

**Tags**: `#英伟达`, `#AI供应链`, `#台湾`, `#投资`, `#芯片制造`

---

<a id="item-7"></a>
## [China to Assign Digital IDs to Humanoid Robots](https://www.scmp.com/tech/policy/article/3354747/china-give-every-humanoid-robot-digital-id-push-boost-industry-standards) ⭐️ 8.0/10

China's Ministry of Industry and Information Technology launched a 'Humanoid Full Lifecycle Management Service Platform' that will assign unique digital IDs to all domestically manufactured humanoid robots, enabling tracking from production to recycling. This initiative standardizes governance of humanoid robots, enhancing traceability, safety monitoring, and liability assignment, while positioning China as a leader in AI robotics regulation. The digital ID system is four-segmented and mandatory for all humanoid robots manufactured in China, with over 28,000 units from more than 100 companies already registered.

telegram · zaihuapd · May 28, 09:08

**Background**: Humanoid robots are robots designed to resemble the human body, often used for interaction with human environments and tools. The standardization committee for humanoid and embodied intelligence was established by MIIT in late 2025 to systematically advance standards. This digital ID system is a key part of those standards, ensuring lifecycle management.

<details><summary>References</summary>
<ul>
<li><a href="https://www.breezyscroll.com/technology-news/china-humanoid-robot-digital-identity-system/">China To Assign Official IDs To Humanoid Robots Just... - BreezyScroll</a></li>
<li><a href="https://www.biometricupdate.com/202605/china-creates-digital-id-for-humanoid-robots">China creates digital ID for humanoid robots | Biometric Update</a></li>
<li><a href="https://www.globaltimes.cn/page/202512/1351625.shtml">China’s MIIT sets up standardization committee for humanoid robots to reinforce sector’s global competitiveness - Global Times</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#humanoid robots`, `#regulation`, `#standards`, `#China`

---

<a id="item-8"></a>
## [Sony Unveils Bravia 9 II & 7 II with RGB LED Backlight](https://www.flatpanelshd.com/news.php?subaction=showfull&amp;id=1779897602) ⭐️ 8.0/10

Sony officially launched its 2026 flagship LCD TVs, Bravia 9 II and Bravia 7 II, on May 27, featuring the industry-first consumer use of 'True RGB' independent red, green, and blue LED backlight technology. This breakthrough delivers near 4000 nits peak brightness and over 90% BT.2020 color coverage, offering a compelling blend of Mini LED brightness and OLED-like color purity, potentially setting a new standard for high-end LCD TVs. The series covers sizes from 50 to 115 inches, including a new 115-inch giant model, but high-end units still offer only two HDMI 2.1 ports and lack Dolby Vision 2 support. Sony leverages its extensive backlight control experience since its 2004 RGB LED TV debut.

telegram · zaihuapd · May 28, 12:15

**Background**: Traditional LCD TVs use white LED backlights with color filters to produce colors. In contrast, RGB LED backlights directly emit red, green, and blue light, enabling purer colors and wider color gamuts without relying on quantum dots. Sony first experimented with this approach in 2004 but only now brings it to mass-market consumer TVs, combining it with modern Mini LED technology for high brightness and precise local dimming.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/16871815855">【科普】RGB-MiniLED电视显示技术详解 - 知乎</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/16968539822">【真机科普】什么是RGB-Mini LED电视？海信RGB三维控色液晶显示技术原理；RGB MiniLED与OLED和MiniLED电视差异，一文看懂！ - 知乎</a></li>
<li><a href="https://display.ofweek.com/2025-04/ART-230001-8500-30660617.html">电视巨头为何纷纷押注 RGB-Mini LED？ - OFweek显示网</a></li>

</ul>
</details>

**Tags**: `#显示技术`, `#电视`, `#消费电子`, `#RGB LED`, `#索尼`

---

<a id="item-9"></a>
## [BYD Unveils 4nm 'Xuanji A3' Chip for Autonomous Driving](https://finance.sina.com.cn/roll/2026-05-28/doc-inhznenn1371824.shtml) ⭐️ 8.0/10

BYD has launched the 'Xuanji A3', a 4nm autonomous driving chip at its 'Dare to' smart strategy event on May 28, 2025. The chip is already in mass production and supports L3/L4 autonomous driving with a combined computing power of over 2100 TOPS from three chips. This marks a major step for BYD in vertical integration, reducing reliance on external chip suppliers and positioning it as a key player in high-end autonomous driving. The 4nm process and high TOPS figure could accelerate mass adoption of L3/L4 features in affordable electric vehicles. The chip leverages BYD's self-developed algorithm optimization, claiming a 100% improvement in computing utilization. BYD also announced it has developed over 2,000 chip products and operates five wafer fabrication plants.

telegram · zaihuapd · May 28, 13:01

**Background**: Autonomous driving chips are specialized processors that handle sensor data and decision-making for self-driving systems. The 4nm process refers to the transistor size, enabling higher performance and energy efficiency. L3 autonomy allows conditional hands-off driving, while L4 can operate without driver intervention in defined areas. TOPS (trillions of operations per second) measures AI computing power; 2100 TOPS is among the highest for automotive chips.

**Tags**: `#autonomous driving`, `#semiconductor`, `#BYD`, `#chip`

---

<a id="item-10"></a>
## [US DOJ Demands Reddit and X Disclose Anonymous ICE Critics](https://www.bloomberg.com/news/articles/2026-05-28/trump-s-doj-ramps-up-probes-of-anonymous-ice-critics-with-x-reddit-subpoenas) ⭐️ 8.0/10

The U.S. Department of Justice has escalated its probe into anonymous critics of U.S. Immigration and Customs Enforcement (ICE) by serving grand jury subpoenas to Reddit and X, demanding the real names, addresses, and financial information of at least two users. This move intensifies the conflict between government investigations and online anonymity, potentially chilling free speech and setting a precedent for how tech platforms handle user privacy under legal pressure. The subpoenas have been upgraded from administrative requests to grand jury subpoenas based on a criminal investigation, but users have not been told the specific charges. A judge is currently reviewing motions to quash the subpoenas.

telegram · zaihuapd · May 28, 14:22

**Background**: U.S. Immigration and Customs Enforcement (ICE) has been a subject of public criticism, particularly for its enforcement actions. The Department of Justice can issue subpoenas to compel platforms to disclose user information. Grand jury subpoenas carry greater legal weight than administrative requests, and failure to comply can lead to contempt charges.

**Tags**: `#US DOJ`, `#ICE`, `#Reddit`, `#X`, `#privacy`

---

<a id="item-11"></a>
## [BYD offers one-year accident liability coverage for city NOA](https://news.mydrivers.com/1/1125/1125729.htm) ⭐️ 8.0/10

BYD announced that from now on, it will cover accident liability for one year for new cars equipped with its God's Eye A and B systems when the city navigation assisted driving feature is engaged, with no cap on compensation. Existing owners of God's Eye A and B can also get this coverage after over-the-air updating to God's Eye 5.0. This policy could set a precedent for liability standards in autonomous driving, potentially increasing consumer trust in assisted driving features and pressuring other automakers to offer similar guarantees. It also aligns with BYD's strategy to democratize advanced driver-assistance systems across its vehicle lineup. The coverage applies only to city navigation assisted driving scenarios, and is limited to the vehicle owner's liability portion with no upper limit. The God's Eye C system, a lower-tier variant, is offered as a paid option priced at 12,000 yuan for new cars.

telegram · zaihuapd · May 29, 01:03

**Background**: City navigation assisted driving (often called city NOA) is an advanced driver-assistance feature that can handle urban roads, including complex intersections, lane changes, and traffic signals, with the driver still required to supervise. BYD's God's Eye system is its proprietary ADAS platform, with different tiers (A, B, C) offering varying levels of capability. Liability for accidents during assisted driving has been a contentious issue; BYD's move to cover the vehicle owner's share marks a significant industry first.

<details><summary>References</summary>
<ul>
<li><a href="https://tech.ifeng.com/c/8tVfo97r5TA">比亚迪发布4nm制程智 驾 芯片，为 城 市 领 航 安全兜底无赔付上限_凤凰网</a></li>
<li><a href="https://www.caixinglobal.com/2025-02-28/caixin-weekly-byd-reaches-new-heights-launches-another-smart-driving-offensive-in-the-new-year-102293276.html">BYD Reaches New Heights, Launches Another Smart Driving Offensive in the New Year</a></li>

</ul>
</details>

**Tags**: `#autonomous driving`, `#BYD`, `#liability`, `#ADAS`, `#electric vehicles`

---