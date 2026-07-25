---
layout: default
title: "Horizon Summary: 2026-07-25 (EN)"
date: 2026-07-25
lang: en
---

> From 31 items, 14 important content pieces were selected

---

1. [Anthropic Launches Claude Opus 5, a New Frontier AI Model](#item-1) ⭐️ 10.0/10
2. [SGLang v0.5.16: DSpark Decoding and 975B Inkling Support](#item-2) ⭐️ 9.0/10
3. [My security camera shipped a GitHub admin token in its login page](#item-3) ⭐️ 9.0/10
4. [IRGC Claims Destruction of Amazon Bahrain Data Center](#item-4) ⭐️ 9.0/10
5. [Two Chinese Mathematicians Win 2026 Fields Medal](#item-5) ⭐️ 9.0/10
6. [Postgres LISTEN/NOTIFY Actually Scales](#item-6) ⭐️ 8.0/10
7. [Why Does Software Keep Getting Worse Despite Coding Advances?](#item-7) ⭐️ 8.0/10
8. [Tech Giants Warn Against Overregulating Open-Weight AI](#item-8) ⭐️ 8.0/10
9. [India orders GitHub to remove Bitchat app citing security](#item-9) ⭐️ 8.0/10
10. [Buz – A fork of Bun using modern Zig, with sub-1s incremental builds](#item-10) ⭐️ 8.0/10
11. [Claude Opus 5: Least Prompt-Injectable Model Yet](#item-11) ⭐️ 8.0/10
12. [China's ChangXin Memory to Near Micron DRAM Capacity by 2026](#item-12) ⭐️ 8.0/10
13. [OpenAI Launches Enterprise AI Agent Platform Presence, Software Stocks Plunge](#item-13) ⭐️ 8.0/10
14. [Jensen Huang: US should allow use of China's open-source AI models](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic Launches Claude Opus 5, a New Frontier AI Model](https://www.anthropic.com/news/claude-opus-5) ⭐️ 10.0/10

Anthropic announced Claude Opus 5, a new flagship AI model with strong benchmark performance and no data retention requirements for general access. This release matters because Opus 5 offers frontier capabilities without the 30-day data retention policy of competing models like Fable, making it attractive for organizations with strict data privacy needs. Its strong performance could shift the competitive landscape among leading AI labs. According to community testing, Opus 5 shows more accurate image-to-HTML conversion than Fable, and its writing style retains 'Claude-isms' similar to its predecessor Opus 4.8, which some users find distinctive.

hackernews · alvis · Jul 24, 16:57 · [Discussion](https://news.ycombinator.com/item?id=49038433)

**Background**: Claude Opus models are Anthropic's most capable and expensive tier. Opus 5 continues this lineage with improved reasoning and vision capabilities. The system card, a pre-deployment safety disclosure, details evaluations and risk thresholds. Unlike some competitors, Anthropic does not require 30-day data retention for general access to Opus models, addressing privacy concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>
<li><a href="https://techjacksolutions.com/ai-tools/anthropic-claude/claude-opus-5-system-card/">Claude Opus 5 System Card, Explained: 6 Safety Findings in ...</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the importance of Opus 5's lack of data retention requirements, with users noting organizations can now access frontier AI without privacy tradeoffs. Some users report real-world testing showing Opus 5 outperforming Fable on image-to-HTML tasks and retaining characteristic Claude writing quirks.

**Tags**: `#AI`, `#LLM`, `#Claude`, `#Anthropic`, `#frontier models`

---

<a id="item-2"></a>
## [SGLang v0.5.16: DSpark Decoding and 975B Inkling Support](https://github.com/sgl-project/sglang/releases/tag/v0.5.16) ⭐️ 9.0/10

SGLang v0.5.16 introduces DSpark, a confidence-driven speculative decoding algorithm achieving up to 383.7 tokens per second, and adds support for the Inkling 975B-parameter multimodal mixture-of-experts model. These innovations significantly improve inference throughput for large language models and enable deployment of extremely large open-weight multimodal models, pushing the boundaries of efficient LLM serving. DSpark drafts semi-autoregressively in blocks and adjusts verification window size based on confidence, while Inkling combines sliding-window attention, full attention, Mamba2 linear attention, and NVFP4 MoE, supporting a 1M-token context.

github · Qiaolin-Yu · Jul 25, 00:13

**Background**: Speculative decoding accelerates LLM inference by using a smaller draft model to generate candidate tokens that are then verified by the target model in parallel. DSpark optimizes this process by adaptively sizing verification windows. Mixture-of-experts (MoE) models like Inkling activate only a subset of parameters per token, enabling larger total parameters with lower computational cost.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/dspark">DSpark : Speculative Decoding</a></li>
<li><a href="https://models.dev/models/thinkingmachines/inkling/">Inkling pricing, providers, and specs | Models .dev</a></li>

</ul>
</details>

**Tags**: `#speculative decoding`, `#LLM inference`, `#large language models`, `#sglang`

---

<a id="item-3"></a>
## [My security camera shipped a GitHub admin token in its login page](https://hhh.hn/hanwha-github-token/) ⭐️ 9.0/10

A security camera from Hanwha was discovered to have a GitHub personal access token hardcoded in its login page, granting admin-level access to the company's GitHub repositories. This exposes a severe supply chain vulnerability, as an attacker could use the token to inject malicious code into the camera's firmware or steal sensitive data, affecting all devices using that firmware. The token was embedded in the login page's HTML source code and had access to multiple repositories, including those containing firmware images and proprietary code.

hackernews · hhh · Jul 24, 11:54 · [Discussion](https://news.ycombinator.com/item?id=49034292)

**Background**: GitHub personal access tokens are used to authenticate API and command-line operations without a password. When leaked, they can be exploited to access repositories. Supply chain security involves protecting software from vulnerabilities introduced during development and distribution. Hardcoding secrets in web pages is a basic security failure.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens">Managing your personal access tokens - GitHub Docs</a></li>
<li><a href="https://www.darkreading.com/vulnerabilities-threats/rising-tide-of-software-supply-chain-attacks">The Rising Tide of Software Supply Chain Attacks</a></li>

</ul>
</details>

**Discussion**: Commenters expressed lack of surprise, noting that many IoT vendors prioritize features over security. Suggestions included isolating cameras on separate VLANs without internet access. One commenter pointed out that US Department of War IP addresses were also baked into the firmware, indicating deeper issues.

**Tags**: `#security`, `#IoT`, `#vulnerability`, `#GitHub`, `#token`

---

<a id="item-4"></a>
## [IRGC Claims Destruction of Amazon Bahrain Data Center](https://houseofsaud.com/irgc-claims-destroyed-amazon-bahrain-data-center/) ⭐️ 9.0/10

The Islamic Revolutionary Guard Corps (IRGC) claims it has destroyed Amazon's Bahrain data center, which hosts the AWS me-south-1 region, taking the entire region offline. This incident marks a major escalation in state-sponsored attacks on critical cloud infrastructure, potentially disrupting services for numerous organizations relying on AWS in the Middle East and highlighting vulnerabilities in centralized cloud architectures. An AWS region like me-south-1 consists of at least three data centers located kilometers apart, suggesting that multiple facilities were attacked. Community analysis identified specific data center buildings (BAH53 and its substation) in Manama that were damaged or destroyed on July 16 and July 22, 2026.

hackernews · thisislife2 · Jul 24, 09:52 · [Discussion](https://news.ycombinator.com/item?id=49033240)

**Background**: AWS regions are geographic areas containing multiple isolated Availability Zones, each with one or more data centers. The me-south-1 region in Bahrain is one of the few AWS regions in the Middle East, alongside a region in Tel Aviv and an upcoming one in Saudi Arabia. The attack underscores the physical security risks to cloud infrastructure during geopolitical conflicts.

<details><summary>References</summary>
<ul>
<li><a href="https://health.aws.amazon.com/health/status?region=me-south-1">Service health - Jul 24, 2026 | AWS Health Dashboard | Global</a></li>
<li><a href="https://docs.aws.amazon.com/global-infrastructure/latest/regions/aws-regions.html">AWS Regions - AWS Regions and Availability Zones</a></li>
<li><a href="https://awsspeedtest.com/regions/me-south-1">Middle East (Bahrain) AWS Region | me-south-1</a></li>

</ul>
</details>

**Discussion**: Comments expressed irony that the only remaining operational AWS region in the Middle East is the one in Tel Aviv. Users also highlighted the scale of the attack, noting that taking down an entire region requires disabling multiple geographically separated data centers, and drew parallels to similar strikes in the Ukraine war.

**Tags**: `#AWS`, `#infrastructure`, `#geopolitics`, `#data center`, `#security`

---

<a id="item-5"></a>
## [Two Chinese Mathematicians Win 2026 Fields Medal](https://t.me/zaihuapd/42748) ⭐️ 9.0/10

The International Mathematical Union announced the 2026 Fields Medal winners, including Deng Yu for his work on partial differential equations and John Pardon for symplectic geometry. This marks the first time two Chinese nationals win the Fields Medal. The Fields Medal is the most prestigious prize in mathematics, and having two Chinese winners signals the rising influence of Chinese mathematicians on the global stage. Their work on PDEs and symplectic geometry has deep implications for mathematical physics and geometry. Deng Yu was recognized for rigorously deriving the Boltzmann equation from hard-sphere dynamics and for probabilistic methods in nonlinear Schrödinger dynamics. John Pardon was recognized for new methods for virtual fundamental cycles and contributions to Fukaya categories in symplectic geometry.

telegram · zaihuapd · Jul 24, 12:51

**Background**: The Fields Medal is awarded every four years to mathematicians under age 40 who have made outstanding contributions. The prize is named after Canadian mathematician John Charles Fields. Deng Yu's work on the Boltzmann equation bridges microscopic particle dynamics to macroscopic gas behavior, while Pardon's work on virtual fundamental cycles is a key tool in enumerative geometry and symplectic topology.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Virtual_fundamental_class">Virtual fundamental class - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Fukaya_category">Fukaya category</a></li>
<li><a href="https://annals.math.princeton.edu/articles/22284">Long time derivation of the Boltzmann equation from hard sphere dyamics | Annals of Mathematics</a></li>

</ul>
</details>

**Tags**: `#Fields Medal`, `#Mathematics`, `#Chinese Mathematicians`, `#PDE`, `#Symplectic Geometry`

---

<a id="item-6"></a>
## [Postgres LISTEN/NOTIFY Actually Scales](https://www.dbos.dev/blog/postgres-listen-notify-scalability) ⭐️ 8.0/10

A blog post from DBOS demonstrates that PostgreSQL's LISTEN/NOTIFY mechanism can scale up to 60,000 notifications per second, debunking the myth that it does not scale. This finding is significant for PostgreSQL practitioners who need lightweight, database-integrated messaging without additional infrastructure, as it shows LISTEN/NOTIFY can handle high-throughput scenarios many applications require. The blog post provides concrete performance benchmarks and practical use cases, such as building durable workflows on top of LISTEN/NOTIFY with DBOS. It also references a previous critical article and corrects the scalability concerns.

hackernews · KraftyOne · Jul 24, 19:05 · [Discussion](https://news.ycombinator.com/item?id=49040296)

**Background**: PostgreSQL's LISTEN and NOTIFY commands enable asynchronous interprocess communication within the same database. A client session uses LISTEN to subscribe to a named channel, and any session can send a notification via NOTIFY to all listeners. This mechanism is often used for real-time updates, cache invalidation, and simple coordination, but some developers have believed it does not scale beyond a few thousand notifications per second.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/sql-notify.html">PostgreSQL: Documentation: 18: NOTIFY</a></li>
<li><a href="https://www.postgresql.org/docs/current/sql-listen.html">PostgreSQL: Documentation: 18: LISTEN</a></li>
<li><a href="https://oneuptime.com/blog/post/2026-01-25-use-listen-notify-real-time-postgresql/view">How to Use Listen/Notify for Real-Time Updates in PostgreSQL</a></li>

</ul>
</details>

**Discussion**: Comments highlight that scalability is a continuum: 60K/s might be too much for some and too little for others. One commenter notes they built a queue on LISTEN/NOTIFY for strong consistency, and another points out that performance issues in early releases have since been fixed.

**Tags**: `#PostgreSQL`, `#database`, `#scalability`, `#messaging`

---

<a id="item-7"></a>
## [Why Does Software Keep Getting Worse Despite Coding Advances?](https://ptrchm.com/posts/nothing-works-and-everyone-is-euphoric/) ⭐️ 8.0/10

The article critiques current software quality, arguing that despite advances in coding (e.g., AI assistance), software has become buggy, bloated, and user-hostile. This reflects widespread frustration among developers and users, highlighting a disconnect between industry hype and actual user experience, and raises questions about software development direction. The article notes that updates now inspire dread rather than excitement, and points to issues like focus stealing, buggy new versions, and a culture where non-technical imposters drive product decisions.

hackernews · pchm · Jul 24, 09:08 · [Discussion](https://news.ycombinator.com/item?id=49033004)

**Background**: The perception that 'coding has been solved' stems from advances like AI code generation and low-code platforms. However, software quality degradation—bloat, bugs, poor UX—persists, often attributed to misguided incentives, rushed releases, and a lack of user-centric design.

**Discussion**: Hacker News commenters largely agree, blaming non-technical managers ('imposters') for prioritizing change over quality, and some recommend using LTS Linux distros to avoid buggy updates. Others highlight specific UX failures like focus stealing on macOS, contrasting with better focus control on KDE Plasma.

**Tags**: `#software quality`, `#user experience`, `#tech industry`, `#productivity`

---

<a id="item-8"></a>
## [Tech Giants Warn Against Overregulating Open-Weight AI](https://www.cnbc.com/2026/07/24/nvidia-microsoft-meta-open-weight-ai-models.html) ⭐️ 8.0/10

Nvidia, Microsoft, and Meta jointly published an open letter warning U.S. policymakers against overregulating open-weight AI models, arguing it would stifle innovation and undermine American leadership in AI. This marks a rare unified stance from major tech companies against proposed regulations, highlighting a growing political divide between open-weight advocates and closed-source competitors like OpenAI and Anthropic. The outcome could shape future U.S. AI policy and global competitiveness. The letter, published on Nvidia's website and endorsed by CEO Jensen Huang, draws parallels to past tech policy battles like the SOPA protests. It also comes amid debates over restricting Chinese open-weight models, with some startups advocating for continued access.

hackernews · louiereederson · Jul 24, 13:32 · [Discussion](https://news.ycombinator.com/item?id=49035303)

**Background**: Open-weight AI models release the trained neural network weights publicly, allowing anyone to download and run the model on their own hardware. This differs from fully open-source models, as the training code and data may remain proprietary. Recent U.S. policy discussions have focused on potential risks of open-weight models from China, leading to calls for regulation.

<details><summary>References</summary>
<ul>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you've been told - Open Source Initiative</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters expressed skepticism about the motives of closed-source companies like Anthropic, with some noting the irony of using Chinese open-weight models for security-sensitive tasks. Others compared the debate to the SOPA protests, suggesting the open-weight side may have broader industry support than previous fights.

**Tags**: `#AI regulation`, `#open-weight`, `#tech industry`, `#policy`, `#artificial intelligence`

---

<a id="item-9"></a>
## [India orders GitHub to remove Bitchat app citing security](https://www.thehindu.com/news/national/government-orders-github-to-remove-bluetooth-based-chat-app-bitchat-over-security-concerns-jack-dorsey/article71262049.ece) ⭐️ 8.0/10

The Indian government has ordered GitHub to remove the Bitchat repository, a Bluetooth-based encrypted messaging app co-created by Jack Dorsey, citing risks of misuse by anti-national elements and criminals. This action raises significant concerns about government censorship and surveillance, especially as Bitchat enables offline P2P communication that bypasses internet monitoring. It also impacts the open-source community's ability to distribute privacy-preserving tools. Bitchat uses Bluetooth Low Energy (BLE) mesh networks and can also leverage the Nostr protocol for internet-based messaging, requiring no user accounts or central servers. The Indian government's order was issued under concerns about circumventing lawful surveillance.

hackernews · rootkea · Jul 24, 14:41 · [Discussion](https://news.ycombinator.com/item?id=49036433)

**Background**: Bitchat is a peer-to-peer encrypted messaging app conceived by Doris Lima and developed by Jack Dorsey, announced in July 2025. It functions over Bluetooth mesh networks without internet or cellular service, making it useful during network restrictions. India has historically taken strict measures to control communications after the 2008 Mumbai attacks, including banning satellite phones.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bitchat">BitChat - Wikipedia</a></li>
<li><a href="https://play.google.com/store/apps/details?id=com.bitchat.droid&hl=en-US">bitchat - Apps on Google Play</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed views: some criticized the government's move as censorship and an attempt to control protest communications, while others noted India's security concerns post-2008 Mumbai attacks. Several users drew parallels to past restrictions on satellite phones and VOIP.

**Tags**: `#censorship`, `#government surveillance`, `#open source`, `#security`, `#India`

---

<a id="item-10"></a>
## [Buz – A fork of Bun using modern Zig, with sub-1s incremental builds](https://ziggit.dev/t/buz-a-drop-in-replacement-for-bun-using-modern-zig-with-sub-1s-incremental-builds/16891) ⭐️ 8.0/10

Buz is a drop-in replacement for Bun that uses modern Zig and achieves sub-1s incremental builds, while also removing over 11,000 lines of dead code. This demonstrates that Bun's build times could have been much faster and highlights the problem of code neglect in large projects. It also sparks discussion about the role of LLMs in code cleanup and the trade-off between feature development and code stewardship. The fork leverages modern Zig features and relies more on Zig's standard library, but Zig incremental compilation does not yet support aarch64, and only the Linux linker supports binary patching.

hackernews · kristoff_it · Jul 24, 09:26 · [Discussion](https://news.ycombinator.com/item?id=49033099)

**Background**: Bun is an all-in-one JavaScript runtime designed as a drop-in replacement for Node.js. Zig is a systems programming language focused on robustness and performance. Incremental builds compile only changed parts of the code, significantly reducing build times. Buz shows how modernizing the codebase and removing dead code can achieve this.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Incremental_build_model">Incremental build model</a></li>

</ul>
</details>

**Discussion**: Commenters expressed surprise at the 11,000 lines of dead code, with some questioning the maintainer's experience. There was criticism of using LLMs to clean up code that LLMs may have originally produced. One commenter noted the tick-tock cycle of features vs. code stewardship in LLM-heavy projects.

**Tags**: `#zig`, `#bun`, `#build-performance`, `#open-source-fork`, `#code-quality`

---

<a id="item-11"></a>
## [Claude Opus 5: Least Prompt-Injectable Model Yet](https://simonwillison.net/2026/Jul/25/boris-cherny/#atom-everything) ⭐️ 8.0/10

Boris Cherny highlighted that Anthropic's Claude Opus 5 is the least prompt-injectable model to date, based on evaluations and red teaming results buried in the model's system card. This marks significant progress in AI safety, as prompt injection is a critical vulnerability in LLMs, making Opus 5 more suitable for sensitive and real-world deployments. The findings are detailed on page 73 of the Claude Opus 5 System Card, which includes evaluations and red teaming results showing strong resistance to prompt injection.

rss · Simon Willison · Jul 25, 00:42

**Background**: Prompt injection is a cybersecurity exploit where malicious inputs cause LLMs to bypass safeguards and produce unintended outputs. System cards released by companies like Anthropic document model capabilities and safety evaluations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection | OWASP Foundation</a></li>
<li><a href="https://www.anthropic.com/system-cards">Model system cards \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#prompt-injection`, `#anthropic`, `#claude`, `#ai-safety`, `#generative-ai`

---

<a id="item-12"></a>
## [China's ChangXin Memory to Near Micron DRAM Capacity by 2026](https://t.me/zaihuapd/42741) ⭐️ 8.0/10

Citrini Research predicts that ChangXin Memory Technologies (CXMT) will reach approximately 350,000 DRAM wafer starts per month by the end of 2026, closing in on Micron's 375,000 wafers per month, making China the world's second largest DRAM producer. This rapid expansion by Chinese DRAM manufacturers could reshape global memory supply chains, reduce dependence on foreign chips, and intensify geopolitical tensions around semiconductor technology. In addition to CXMT, other Chinese firms like SiEn (昇维旭), JinHua (晋华集成), and XMC (a YMTC subsidiary) are also expanding production, potentially pushing total Chinese DRAM capacity to 600,000 wafers per month excluding foreign-owned fabs in China.

telegram · zaihuapd · Jul 24, 07:30

**Background**: DRAM (Dynamic Random Access Memory) is a critical memory chip used in computers, servers, and mobile devices. Currently, the DRAM market is dominated by three players: Samsung, SK Hynix, and Micron, all non-Chinese. China has been investing heavily in domestic semiconductor manufacturing to achieve self-sufficiency, with CXMT being its primary DRAM producer.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://www.techinsights.com/blog/300mm-fab-capacity-surpass-10m-wafers-month-2025">300mm Fab Capacity to Surpass 10M Wafers per Month in 2025</a></li>
<li><a href="https://en.wikipedia.org/wiki/XMC_(company)">XMC (company) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#DRAM`, `#semiconductor`, `#China`, `#manufacturing`, `#memory`

---

<a id="item-13"></a>
## [OpenAI Launches Enterprise AI Agent Platform Presence, Software Stocks Plunge](https://www.businessinsider.com/openai-release-turns-a-bad-week-ugly-for-software-stocks-2026-7) ⭐️ 8.0/10

On July 22, 2026, OpenAI launched Presence, an enterprise AI agent platform that enables companies to deploy and manage AI agents for automating customer service, sales, and internal workflows. Following the announcement, major software stocks such as Workday, Atlassian, HubSpot, and Salesforce experienced significant declines. Presence directly competes with SaaS vendors' own AI agent features, intensifying the disruption of the traditional enterprise software market. This event signals that AI-native platforms are encroaching on established SaaS territories, potentially reshaping the competitive landscape and affecting investor sentiment across the software industry. Presence supports voice and chat dual channels, system operation capabilities, and human-in-the-loop collaboration mechanisms. TD Cowen analysts attributed the IGV software index's ~3% drop on Wednesday largely to OpenAI's product, noting that customer service and sales segments face the highest disruption risk.

telegram · zaihuapd · Jul 24, 12:05

**Background**: An AI agent (AI Agent) is an autonomous software system that can perceive its environment, make decisions, and execute actions to achieve goals, often integrating with enterprise tools. Traditional SaaS platforms like Salesforce, Workday, and Atlassian have been embedding AI agents into their products, but OpenAI's Presence offers a standalone platform that directly competes by providing similar capabilities with its own large language model backend. This marks a shift from AI as a feature to AI as a platform replacing existing SaaS workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ithome.com/0/980/300.htm">OpenAI 推出 OpenAI Presence，布局企业软件赛道 - IT之家</a></li>
<li><a href="https://juejin.cn/post/7665879209437839386">OpenAI Presence 发布：企业级 AI Agent 正式进入工作流</a></li>
<li><a href="https://www.aitop100.cn/infomation/details/34321.html">OpenAI双重大动作：推出企业Agent平台Presence，300亿自建算力中心-AI...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#企业AI`, `#SaaS`, `#市场竞争`, `#股市影响`

---

<a id="item-14"></a>
## [Jensen Huang: US should allow use of China's open-source AI models](https://t.me/zaihuapd/42749) ⭐️ 8.0/10

Nvidia CEO Jensen Huang stated in an interview that China's open-source AI models are 'excellent' and US companies should 'absolutely' be permitted to use them, arguing that such access expands market demand for hardware. This endorsement from a key industry leader challenges the narrative of restricting Chinese AI on national security grounds, potentially influencing US policy and the global AI ecosystem. Huang dismissed the scenario that Chinese companies would push US firms out of the market as zero probability, and he suggested using safety sandboxes to control downloaded Chinese models rather than blanket bans.

telegram · zaihuapd · Jul 24, 13:26

**Background**: Open-source AI models allow developers to freely access, modify, and distribute the underlying code and weights. In recent years, Chinese companies like Alibaba and Baidu have released competitive open-source models, raising concerns in the US about technology transfer and national security.

**Tags**: `#AI开源`, `#黄仁勋`, `#政策`, `#英伟达`, `#中国AI模型`

---