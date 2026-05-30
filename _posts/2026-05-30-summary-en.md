---
layout: default
title: "Horizon Summary: 2026-05-30 (EN)"
date: 2026-05-30
lang: en
---

> From 29 items, 12 important content pieces were selected

---

1. [China Certifies 9 Domestic AI Chips for Government Procurement](#item-1) ⭐️ 9.0/10
2. [Blue Origin New Glenn rocket explodes during static fire test](#item-2) ⭐️ 9.0/10
3. [vllm v0.22.0 released with DeepSeek V4, Model Runner V2, Rust frontend](#item-3) ⭐️ 8.0/10
4. [SQLite Deemed Sufficient for Durable Workflows](#item-4) ⭐️ 8.0/10
5. [Defining AI Slop as Output Lacking Motivation](#item-5) ⭐️ 8.0/10
6. [GTA 6 Developers Form Union to Combat Crunch Culture](#item-6) ⭐️ 8.0/10
7. [Developers Must Stay Smarter Than AI Coding Agents](#item-7) ⭐️ 8.0/10
8. [Microsoft 0-day feud escalates as researcher threatens another exploit dump](#item-8) ⭐️ 8.0/10
9. [Datasette 1.0a31 adds write queries and saved queries](#item-9) ⭐️ 8.0/10
10. [Anthropic surpasses OpenAI as most valuable AI startup](#item-10) ⭐️ 8.0/10
11. [Security flaws in India's CBSE online grading system exposed](#item-11) ⭐️ 8.0/10
12. [Huawei Proposes Tao's Law for Time-Domain Chip Scaling](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [China Certifies 9 Domestic AI Chips for Government Procurement](https://www.tomshardware.com/tech-industry/semiconductors/china-certifies-nine-domestic-ai-chips-for-government-procurement) ⭐️ 9.0/10

The China Information Security Testing and Evaluation Center has added an 'AI training and inference chip' category to its security certification framework, certifying nine domestic AI processors for the first time. The certified chips include Huawei's Ascend, Alibaba's T-Head Zhenwu, Biren Technology, and Hygon, among others. This certification will serve as the procurement basis for government agencies and state-owned enterprises, marking a significant policy shift toward domestic AI chips. It accelerates China's push for technological self-reliance in critical semiconductor sectors. The certification is valid for three years, and notable absentees include Cambricon and Baidu's Kunlun. The list covers chips used for both AI training and inference, indicating a comprehensive approach to secure procurement.

telegram · zaihuapd · May 29, 08:41

**Background**: China's 'Anke' (safe and reliable) procurement catalog is a government-endorsed list of secure and trustworthy IT products, mandated for use by critical information infrastructure operators. The inclusion of AI chips for the first time extends this framework to advanced computing hardware, reflecting growing concerns over reliance on foreign technology like NVIDIA's GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anbob.com/archives/8415.html">2023、2024、2025、2026 四批次数据库 安可 ( 安全 可靠测评) 目录 列表 – ...</a></li>
<li><a href="https://blog.csdn.net/yts1985/article/details/139064348">第一批 安全 可靠测评结果 (1-2023)_ 安可目录 -CSDN博客</a></li>
<li><a href="https://cloud.tencent.com/developer/article/1958838">国务院要求关键信息基础设施运营者应优先 采购 「 安可 产品和服务」：包...</a></li>

</ul>
</details>

**Tags**: `#国产芯片`, `#AI芯片`, `#政府采购`, `#半导体`, `#自主可控`

---

<a id="item-2"></a>
## [Blue Origin New Glenn rocket explodes during static fire test](https://arstechnica.com/space/2026/05/blue-origins-new-glenn-rocket-just-exploded-during-a-static-fire-test/) ⭐️ 9.0/10

On May 28, 2026, Blue Origin's New Glenn heavy-lift rocket exploded during a static fire test at Cape Canaveral, destroying the vehicle and severely damaging launch pad infrastructure. The anomaly occurred while firing the seven BE-4 engines on the first stage. This incident significantly delays Blue Origin's launch schedule, impacting NASA's Artemis program lunar lander missions and Amazon's Project Kuiper satellite broadband deployment. It also raises questions about the reliability of the BE-4 engine and New Glenn's readiness for flight. The explosion occurred during the NG-4 mission preparation, which was to launch 48 Amazon Kuiper satellites. There were no injuries, but the launch pad's lightning protection tower collapsed. Blue Origin has not yet announced a timeline for recovery or return to flight.

telegram · zaihuapd · May 29, 11:08

**Background**: A static fire test is a routine pre-launch test where the rocket's engines are fired at full power while the vehicle remains securely clamped to the pad. The BE-4 is an oxygen-rich staged combustion engine burning liquid oxygen and methane, developed by Blue Origin and also used on United Launch Alliance's Vulcan rocket. Project Kuiper (now Amazon Leo) is Amazon's low Earth orbit satellite internet constellation, which has contracted launches from multiple providers including Blue Origin.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Static_fire_test">Static fire test</a></li>
<li><a href="https://en.wikipedia.org/wiki/BE-4">BE-4 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Project_Kuiper">Project Kuiper</a></li>

</ul>
</details>

**Tags**: `#Blue Origin`, `#New Glenn`, `#rocket explosion`, `#NASA Artemis`, `#aerospace`

---

<a id="item-3"></a>
## [vllm v0.22.0 released with DeepSeek V4, Model Runner V2, Rust frontend](https://github.com/vllm-project/vllm/releases/tag/v0.22.0) ⭐️ 8.0/10

vllm v0.22.0 is released with 459 commits from 230 contributors, featuring major hardening for DeepSeek V4, advances in Model Runner V2 toward becoming the default, and an experimental Rust frontend. This release significantly improves inference performance and hardware support for large language models, especially for DeepSeek V4, and introduces a new Rust frontend that may reduce overhead. It demonstrates vllm's continued evolution as a critical tool in the AI inference ecosystem. Notable technical improvements include NVFP4 fused MoE support for DeepSeek V4, MTP speculative decoding, multi-tier KV cache offloading beyond CPU memory, and batch-invariant inference with a 28.9% end-to-end latency improvement using Cutlass FP8.

github · khluu · May 29, 10:28

**Background**: vllm is an open-source, high-throughput LLM inference engine that optimizes serving of large models. DeepSeek V4 is a state-of-the-art Mixture-of-Experts model. Model Runner V2 (MRv2) is a refactored inference pipeline aiming for better performance and maintainability. The experimental Rust frontend replaces the Python layer for lower overhead and faster startup.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-speculative-decoding-for-reducing-latency-in-ai-inference/">An Introduction to Speculative Decoding for Reducing Latency in AI Inference | NVIDIA Technical Blog</a></li>
<li><a href="https://deepwiki.com/vllm-project/vllm/7.4-moe-quantization-and-backend-selection">MoE Quantization and Backend Selection | vllm-project/vllm | DeepWiki</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#LLM inference`, `#DeepSeek V4`, `#Model Runner`, `#Rust`

---

<a id="item-4"></a>
## [SQLite Deemed Sufficient for Durable Workflows](https://obeli.sk/blog/sqlite-is-all-you-need-for-durable-workflows/) ⭐️ 8.0/10

A blog post argues that SQLite is sufficient for building durable workflows, sparking a debate about its suitability for production concurrency compared to alternatives like Postgres. This matters because many developers are evaluating lightweight database options for workflow orchestration, and the debate highlights the trade-offs between simplicity and concurrency. SQLite supports unlimited concurrent readers but only one writer at a time, which can be a bottleneck for write-heavy workflows. Some commenters propose using SQLite with S3 compare-and-swap or sharding to improve concurrency.

hackernews · tomasol · May 29, 17:54 · [Discussion](https://news.ycombinator.com/item?id=48326802)

**Background**: Durable workflows ensure that long-running or multi-step operations complete reliably even in the face of failures, often using a database to persist state. SQLite is an embedded SQL database that requires no server process, making it simple to deploy, but it has limited concurrency compared to client-server databases like Postgres.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite.org/whentouse.html">Appropriate Uses For SQLite</a></li>
<li><a href="https://www.inngest.com/uses/durable-workflows">Inngest - Durable Workflows</a></li>
<li><a href="https://jellyfin.org/posts/SQLite-locking/">SQLite concurrency and why you should care about it | Jellyfin</a></li>

</ul>
</details>

**Discussion**: Community comments show divided opinions: some praise SQLite's simplicity for small projects (e.g., replacing multiple SaaS tools), while others argue it's unsuitable for production due to concurrency limits. A novel solution uses SQLite sessions extension with S3 compare-and-swap for safe concurrent access.

**Tags**: `#SQLite`, `#workflows`, `#databases`, `#concurrency`, `#distributed-systems`

---

<a id="item-5"></a>
## [Defining AI Slop as Output Lacking Motivation](https://noperator.dev/posts/you-can-just-say-it/) ⭐️ 8.0/10

A blog post by antirez defines AI slop as output that lacks fundamental motivation, distinguishing the misuse of AI from AI itself. The post emphasizes that slop arises from a lack of understanding or intent, not from the use of LLMs. This distinction provides a clear mental model for critiquing AI misuse without blaming the technology, which is crucial for software engineers and writers navigating the AI era. It helps preserve the value of human intentionality in communication. The post is deliberately concise, contrasting with AI slop, and the author is antirez of noperator.dev. The community discussion has 115 comments, with high engagement (score 8.0, 231 points).

hackernews · antirez · May 29, 15:54 · [Discussion](https://news.ycombinator.com/item?id=48324853)

**Background**: AI slop refers to low-quality, meaningless content generated by AI, often criticized for lacking substance. The term gained traction in tech communities as AI-generated text became widespread. This post argues that slop is not inherent to AI but stems from users who produce output without genuine motivation or understanding.

**Discussion**: Community comments are largely positive and reflective. Cautiouscat highlights a friend's quote about preferring raw prompts over LLM-generated emails. Beering hopes AI can decouple human value from work output. Antirez himself calls it the best definition of AI slop. Sbiru93 finds personal relief, and drooby notes art and sport retain value due to creator intent.

**Tags**: `#AI`, `#LLM`, `#writing`, `#slop`, `#communication`

---

<a id="item-6"></a>
## [GTA 6 Developers Form Union to Combat Crunch Culture](https://rockstarintel.com/gta-6-developers-announce-rockstar-games-union/) ⭐️ 8.0/10

Rockstar Games developers working on Grand Theft Auto VI have announced the formation of a union to demand pay transparency, flexible working hours, and an end to compulsory overtime known as crunch culture. This unionization effort addresses systemic labor exploitation in the video game industry, where crunch culture leads to 65–80 hour work weeks without proper compensation. If successful, it could set a precedent for other game studios and improve both working conditions and game quality. The union's demands include pay transparency, flexible working, and an end to crunch—a practice of unpaid overtime common in game development. Industry data shows crunch can persist for months around game launches, affecting employee health and retention.

hackernews · AndrewKemendo · May 29, 15:32 · [Discussion](https://news.ycombinator.com/item?id=48324499)

**Background**: Crunch culture refers to the norm of extended, unpaid overtime in video game development, often driven by corporate pressure and peer influence. Workers may face 65–80 hour weeks for months, leading to burnout and high turnover. Unionization is a growing response to these conditions, with this effort at Rockstar Games being a notable example.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Crunch_(video_games)">Crunch (video games) - Wikipedia</a></li>
<li><a href="https://jacobin.com/2023/10/video-game-workers-crunch-exploitation-union-organizing">The Video Game Industry Calls It “Crunch.” Workers Call It Exploitation.</a></li>

</ul>
</details>

**Discussion**: Commenters expressed support for the union, highlighting the disparity between game developer pay and big tech salaries, and noting that crunch exploits workers. Some pointed out the difficulty of unionizing in the US due to outsourcing and H1B visas, but overall sentiment was positive towards better working conditions.

**Tags**: `#labor rights`, `#gaming industry`, `#unionization`, `#crunch culture`

---

<a id="item-7"></a>
## [Developers Must Stay Smarter Than AI Coding Agents](https://vickiboykis.com/2026/05/28/we-should-be-more-tired-than-the-model/) ⭐️ 8.0/10

A blog post argues that developers must maintain greater understanding and critical thinking than AI models they use, emphasizing human oversight in AI-assisted coding. This highlights the evolving role of developers from writing code to supervising AI agents, addressing concerns about skill retention and the need for higher-level oversight in software engineering. The author suggests that the bottleneck in AI-assisted coding is understanding, and that abstraction is a key tool for managing complexity, but notes that developers have never truly mastered abstraction.

hackernews · tosh · May 29, 12:12 · [Discussion](https://news.ycombinator.com/item?id=48322118)

**Discussion**: Commenters have mixed views: some agree that developer skill remains crucial, while others see a shift toward product management skills and question whether skill loss is as severe as claimed.

**Tags**: `#AI-assisted coding`, `#software engineering`, `#developer skills`, `#productivity`

---

<a id="item-8"></a>
## [Microsoft 0-day feud escalates as researcher threatens another exploit dump](https://www.theregister.com/security/2026/05/28/microsoft-0-day-feud-escalates-as-researcher-threatens-another-windows-exploit-dump/5248085) ⭐️ 8.0/10

A security researcher threatened to release additional zero-day exploits for Microsoft Windows, escalating a public feud over responsible disclosure and compensation. This threatens to expose millions of Windows users to unpatched vulnerabilities and highlights ongoing tensions between the security research community and large vendors over disclosure practices. The researcher claims Microsoft violated coordinated vulnerability disclosure (CVD) principles by failing to communicate or provide adequate compensation, prompting the threat of a public exploit dump.

hackernews · Cider9986 · May 29, 19:37 · [Discussion](https://news.ycombinator.com/item?id=48328175)

**Background**: A zero-day vulnerability is a security flaw unknown to the software vendor, making it exploitable before a patch is available. Responsible disclosure, also known as coordinated vulnerability disclosure (CVD), is a process where researchers report vulnerabilities privately to give vendors time to fix them before public disclosure. Disputes can arise when researchers feel vendors are unresponsive or unfair in bounties.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero - day vulnerability - Wikipedia</a></li>
<li><a href="https://www.bugcrowd.com/resources/guide/what-is-responsible-disclosure/">What is Responsible Disclosure? | Bugcrowd</a></li>
<li><a href="https://www.hackerone.com/knowledge-center/why-you-need-responsible-disclosure-and-how-get-started">Why You Need Responsible Disclosure and How to Get Started | HackerOne</a></li>

</ul>
</details>

**Discussion**: Commenters largely sympathized with the researcher, criticizing Microsoft's complex bug reporting system and lack of proper acknowledgment. Some expressed concern for potential victims of the leaked exploits, while others noted the difficulty vendors face in handling a flood of reports, including AI-generated spam and unrealistic expectations.

**Tags**: `#security`, `#0-day`, `#Microsoft`, `#responsible disclosure`, `#exploit`

---

<a id="item-9"></a>
## [Datasette 1.0a31 adds write queries and saved queries](https://simonwillison.net/2026/May/29/datasette/#atom-everything) ⭐️ 8.0/10

Datasette 1.0a31 introduces the ability for users with permissions to execute write queries (INSERT, UPDATE, DELETE) and to save stored queries (formerly canned queries) privately or for other users. This release marks a major step toward Datasette 1.0, transforming it from a read-only tool into one that supports database modifications, enabling collaborative data editing and query sharing within an instance. The new execute query interface supports templated insert/update/delete queries, and users can only execute statements for which they have the appropriate permission (e.g., CREATE TABLE requires create-table permission). Stored queries are renamed from canned queries.

rss · Simon Willison · May 29, 03:32

**Background**: Datasette is an open-source tool for exploring and publishing SQLite databases. Previously, it only allowed read-only queries. This alpha release adds write capabilities, making it more interactive and suitable for applications that need data editing. The term 'stored queries' replaces the previous name 'canned queries'.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/latest/sql_queries.html">Running SQL queries - Datasette documentation</a></li>
<li><a href="https://github.com/datasette/datasette-queries">Save SQL queries in Datasette - GitHub</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#SQL`, `#database`, `#data publishing`, `#open source`

---

<a id="item-10"></a>
## [Anthropic surpasses OpenAI as most valuable AI startup](https://www.nytimes.com/2026/05/28/technology/anthropic-tops-openai-valuation.html) ⭐️ 8.0/10

Anthropic has raised $65 billion in Series H funding, reaching a post-money valuation of $965 billion, overtaking OpenAI's estimated $852 billion valuation to become the most valuable AI startup. This valuation milestone signals a major shift in the AI industry, with investors showing immense confidence in Anthropic's technology and market position. It highlights the intense competition and capital investment required to lead in the large language model space. Anthropic's Claude family of models, including the latest Claude Opus 4.8, have achieved state-of-the-art performance in enterprise AI tasks. The $65 billion round is one of the largest private funding rounds in history, with funds primarily allocated to computing power, model training, and commercialization.

telegram · zaihuapd · May 29, 03:29

**Background**: Anthropic is an AI company founded by former OpenAI employees, focused on developing large language models with a strong emphasis on safety and ethical compliance through its constitutional AI technique. Its flagship product Claude competes directly with OpenAI's GPT series. The valuation surge reflects the growing market demand for advanced AI agents and enterprise solutions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/05/28/anthropic-open-ai-startup-value.html">Anthropic tops OpenAI as most valuable AI startup, nears $1T ...</a></li>
<li><a href="https://www.theguardian.com/technology/2026/may/28/anthropic-ai-valuation">Anthropic reaches valuation of $965bn, beating OpenAI to become...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model ) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#funding`, `#Anthropic`, `#valuation`, `#industry news`

---

<a id="item-11"></a>
## [Security flaws in India's CBSE online grading system exposed](https://ni5arga.com/blog/posts/hacking-cbse/) ⭐️ 8.0/10

A researcher disclosed multiple critical security vulnerabilities in the CBSE online examination grading system, including hardcoded master passwords, OTP validation on the client side, bypassable login pages, and password reset without old password verification, potentially leading to account takeover and score manipulation. These vulnerabilities threaten the integrity of India's high-stakes board examinations, potentially allowing mass score tampering and undermining educational fairness. The incident highlights critical security deficiencies in government-run education systems that handle sensitive data. The researcher reported the issues to India's CERT-In on February 25, 2026, but CBSE initially denied the vulnerabilities. The author later provided screenshots, screen recordings, and archive links as evidence, and discovered an additional SQL injection vulnerability before the site was taken offline.

telegram · zaihuapd · May 29, 05:52

**Background**: Hardcoded passwords refer to credentials embedded directly in source code, making them easily extractable. OTP verification performed on the client side can be bypassed by intercepting or modifying network requests. SQL injection is an attack technique that injects malicious SQL statements into input fields to manipulate backend databases. These are well-known security flaws that should have been prevented during development.

<details><summary>References</summary>
<ul>
<li><a href="https://en.m.wikipedia.org/wiki/One-time_password">One-time password - Wikipedia</a></li>
<li><a href="https://en.m.wikipedia.org/wiki/SQL">SQL - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#安全漏洞`, `#漏洞披露`, `#网络安全`, `#网上阅卷系统`, `#印度`

---

<a id="item-12"></a>
## [Huawei Proposes Tao's Law for Time-Domain Chip Scaling](https://t.me/zaihuapd/41648) ⭐️ 8.0/10

At the 2026 International Symposium on Circuits and Systems in Shanghai, Huawei introduced 'Tao's Law,' a new semiconductor scaling principle that replaces geometric scaling with time-domain scaling. The company also announced it has designed and mass-produced 381 chips using this approach over the past six years, and will launch a new Kirin chip with logic folding technology this fall. Tao's Law offers a potential path to continue semiconductor advancement beyond the limits of Moore's Law, which is reaching physical constraints. If successful, it could reshape the global chip industry and reduce reliance on extreme ultraviolet lithography, with Huawei claiming that high-end chips could achieve transistor density equivalent to 1.4nm process by 2031. The Kirin 2026 chip using logic folding is reported to achieve a transistor density of 238 million transistors per square millimeter, higher than TSMC's N3E process. However, early benchmark estimates show its single-core performance trailing Qualcomm's latest flagship by about 47% on Geekbench 6.

telegram · zaihuapd · May 30, 02:18

**Background**: Moore's Law, the observation that the number of transistors on a chip doubles roughly every two years, has driven semiconductor progress for decades but is now slowing due to physical limits. Traditional geometric scaling shrinks transistor dimensions, while Tao's Law focuses on reducing time constants—the time needed for signals to switch—through multi-level optimization across devices, circuits, and systems. Logic folding is a chip design technique that stacks logic layers to increase density, similar to 3D stacking but more aggressive, and is part of Huawei's broader strategy to innovate under U.S. export restrictions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.globaltimes.cn/page/202605/1361994.shtml">The Tau Scaling Law comes out: Chinese innovation is... - Global Times</a></li>
<li><a href="https://en.c114.com.cn/577/a1311082.html">Huawei Unveils New Semiconductor Law : The " Tao ..."</a></li>
<li><a href="https://www.gizmochina.com/2026/05/25/huawei-previews-kirin-2026-chip-with-higher-transistor-density-and-efficiency/">Huawei previews Kirin 2026 chip with higher transistor density and...</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#Moore's law`, `#Huawei`, `#chip design`, `#technology breakthrough`

---