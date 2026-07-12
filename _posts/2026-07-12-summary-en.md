---
layout: default
title: "Horizon Summary: 2026-07-12 (EN)"
date: 2026-07-12
lang: en
---

> From 23 items, 8 important content pieces were selected

---

1. [vLLM v0.25.0: Major Overhaul with MRv2 Default](#item-1) ⭐️ 9.0/10
2. [Humanoid Robot Performs World-First Live Pig Gallbladder Surgery](#item-2) ⭐️ 9.0/10
3. [Circular Financing in GPU Cloud Boom](#item-3) ⭐️ 8.0/10
4. [ClickHouse scales PgBouncer 4x with peering](#item-4) ⭐️ 8.0/10
5. [Prefer strict tables in SQLite for type safety](#item-5) ⭐️ 8.0/10
6. [Apple sues OpenAI for systematic trade secret theft](#item-6) ⭐️ 8.0/10
7. [6 U-Boot vulnerabilities enable boot-time code execution](#item-7) ⭐️ 8.0/10
8. [Zhipu Founder Tang Jie Launches 'Touch High' AGI Plan](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0: Major Overhaul with MRv2 Default](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 makes Model Runner V2 the default execution path for all dense models, removes the legacy PagedAttention implementation, and achieves speed parity between the Transformers modeling backend and native vLLM. This release significantly simplifies the vLLM codebase and improves performance, making it easier for users to deploy and serve large language models with high throughput. The removal of legacy attention and parity between backends enables faster adoption of new model architectures and optimizations. The release includes 558 commits from 232 contributors, support for new models like LLaVA-OneVision-2 and GLM-5, a new Streaming Parser Engine for tool-call/reasoning, and universal speculative decoding for heterogeneous vocabularies.

github · khluu · Jul 11, 20:06

**Background**: vLLM is an open-source high-throughput LLM inference engine that uses PagedAttention to manage key-value cache memory efficiently. Model Runner V2 (MRv2) is a redesigned execution path that unifies model loading and inference, improving maintainability and enabling new features like prefix caching and real-time embeddings. The Transformers backend allows vLLM to run Hugging Face models directly without conversion, and this release makes it as fast as the native backend.

**Tags**: `#vllm`, `#LLM inference`, `#model serving`, `#performance optimization`, `#open source`

---

<a id="item-2"></a>
## [Humanoid Robot Performs World-First Live Pig Gallbladder Surgery](https://arstechnica.com/ai/2026/07/humanoid-robots-controlled-by-surgeons-did-world-first-operation-on-live-pigs/) ⭐️ 9.0/10

Surgeons remotely controlled a Unitree G1 humanoid robot to perform the world's first live gallbladder surgery on two pigs, as published in Nature. This demonstrates that low-cost, general-purpose humanoid robots could make remote surgery accessible in underserved areas, battlefields, or space, potentially democratizing surgical care. The Unitree G1 robot costs as low as $13,500 (base) or ~$67,000 with dexterous hands, far less than specialized systems like Da Vinci (over $500,000). The robot is 1.5 m tall and weighs 27 kg.

telegram · zaihuapd · Jul 11, 02:29

**Background**: Teleoperated surgery uses robotic systems controlled remotely by a surgeon. Traditionally, specialized surgical robots like Da Vinci are expensive and large. Humanoid robots offer a flexible and affordable alternative, as they can be adapted with surgical tools and controlled via teleoperation.

<details><summary>References</summary>
<ul>
<li><a href="https://today.ucsd.edu/story/surgeons-use-teleoperated-humanoid-robots-to-perform-live-surgery-a-world-first">Surgeons Use Teleoperated Humanoid Robots to Perform Live Surgery – a World First</a></li>
<li><a href="https://www.popsci.com/technology/humanoid-robots-perform-surgery/">In groundbreaking first, humanoid robots performed surgery | Popular Science</a></li>
<li><a href="https://www.nature.com/articles/s41586-026-10796-x">In vivo feasibility study of humanoid robots in surgery | Nature</a></li>

</ul>
</details>

**Tags**: `#humanoid robots`, `#surgery`, `#teleoperation`, `#medical robotics`, `#Nature`

---

<a id="item-3"></a>
## [Circular Financing in GPU Cloud Boom](https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom) ⭐️ 8.0/10

An analysis reveals that Nvidia's investments in GPU cloud providers like CoreWeave and Nebius create a circular financing loop, where these providers use Nvidia's equity funding to purchase billions of dollars worth of Nvidia GPUs. This circular financing raises concerns about the economic sustainability and potential overbuilding of GPU infrastructure, which could impact the entire AI cloud ecosystem and investor sentiment. Nvidia invested $2 billion for a 9% stake in CoreWeave, which plans $35 billion in CapEx in 2026, meaning Nvidia's contribution is only 5.7% of CoreWeave's single-year spending; the broader circular structure nonetheless ties neoclouds to continued GPU purchasing.

hackernews · adletbalzhanov · Jul 11, 17:21 · [Discussion](https://news.ycombinator.com/item?id=48873836)

**Background**: GPU cloud providers (neoclouds) like CoreWeave and Nebius offer AI computing services using Nvidia GPUs. Circular financing refers to Nvidia investing in these customers, who then use the funds to buy more Nvidia hardware, creating a closed loop that may inflate demand and mask true market signals.

<details><summary>References</summary>
<ul>
<li><a href="https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom">Nvidia, CoreWeave, and Nebius: Inside the Circular Financing of the GPU Boom</a></li>
<li><a href="https://en.wikipedia.org/wiki/CoreWeave">CoreWeave</a></li>
<li><a href="https://en.wikipedia.org/wiki/Nebius_Group">Nebius Group - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments are divided: some argue Nvidia's small equity stake makes the circular claim overstated, while others debate the long-term profitability of GPU builds and whether overcapacity looms, with a warning it could become a house of cards.

**Tags**: `#GPU`, `#Nvidia`, `#AI infrastructure`, `#cloud computing`, `#finance`

---

<a id="item-4"></a>
## [ClickHouse scales PgBouncer 4x with peering](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse detailed how they improved PgBouncer throughput by 4x using peering and other optimizations for their managed PostgreSQL service. This significant performance improvement makes PgBouncer more scalable for high-traffic PostgreSQL deployments, reducing the need for multiple connection pooler instances. Peering enables cancel requests to be forwarded to the correct PgBouncer process, eliminating misrouted cancellations. The setup uses SO_REUSEPORT to run multiple processes on the same port.

hackernews · saisrirampur · Jul 11, 15:28 · [Discussion](https://news.ycombinator.com/item?id=48872874)

**Background**: PgBouncer is a lightweight connection pooler for PostgreSQL that manages database connections. Peering is a PgBouncer feature that allows multiple processes to share session state and forward cancel requests, reducing overhead from misrouted cancellations and improving throughput.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pgbouncer.org/usage.html">PgBouncer command-line usage</a></li>
<li><a href="https://github.com/pgbouncer/pgbouncer/blob/master/doc/usage.md">pgbouncer/doc/usage.md at master · pgbouncer/pgbouncer</a></li>

</ul>
</details>

**Discussion**: Community members suggested alternatives like Odyssey and pgdog, and asked about Kubernetes peering support. Overall sentiment was positive, with interest in the technical details and practical deployment considerations.

**Tags**: `#postgresql`, `#pgbouncer`, `#connection-pooling`, `#performance`, `#scaling`

---

<a id="item-5"></a>
## [Prefer strict tables in SQLite for type safety](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 8.0/10

A blog post encourages SQLite users to adopt strict tables, which enforce data types, and community members discuss tools like sqlite-utils for converting existing tables. Strict tables improve data integrity by preventing type mismatches, making SQLite more reliable for applications that require rigorous type enforcement. Strict tables are available since SQLite version 3.37.0, and older versions can still read them with 'PRAGMA writable_schema=ON'. The keyword 'STRICT' is added at the end of a CREATE TABLE statement.

hackernews · ingve · Jul 11, 17:33 · [Discussion](https://news.ycombinator.com/item?id=48873940)

**Background**: Unlike most SQL databases, SQLite traditionally allows inserting any type into any column (flexible typing). This can lead to accidental data corruption, e.g., storing a string in an integer column. Strict tables enforce that each column only accepts values of its declared type, aligning SQLite with other databases.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite.org/stricttables.html">STRICT Tables</a></li>

</ul>
</details>

**Discussion**: Simon Willison added a feature to his sqlite-utils tool to transform non-strict tables to strict. dfabulich pointed to SQLite's official rationale for not making strict the default (flextypegood.html). jll29 disagreed and expressed a desire for strict as default, while petilon noted the lack of certain data types like Date as a downside.

**Tags**: `#SQLite`, `#databases`, `#type safety`, `#data integrity`

---

<a id="item-6"></a>
## [Apple sues OpenAI for systematic trade secret theft](https://www.cnbc.com/2026/07/10/apple-openai-lawsuit-trade-secrets.html) ⭐️ 8.0/10

Apple filed a lawsuit on July 10, 2026, in the U.S. District Court for the Northern District of California against OpenAI, two former employees, and io Products, alleging that OpenAI systematically stole Apple's product design, manufacturing processes, and supply chain secrets to accelerate its consumer hardware development. This lawsuit highlights escalating tensions between major tech companies over intellectual property, especially in hardware and AI. If proven, it could set a precedent for trade secret protection and affect competition in the consumer hardware market. Apple alleges that former employee Chang Liu accessed internal networks and downloaded dozens of hardware files after leaving, and that OpenAI hardware head Tang Yew Tan sent supplier information to his personal email before departure and asked job candidates to bring Apple components to interviews. Apple claims over 400 former employees now work at OpenAI.

telegram · zaihuapd · Jul 11, 03:14

**Background**: Apple has long invested heavily in proprietary hardware design and manufacturing processes, which are key to its product differentiation. OpenAI, primarily known for AI software, has been expanding into consumer hardware, potentially competing with Apple. Trade secret lawsuits are common in the tech industry to protect confidential information from competitors.

**Tags**: `#Apple`, `#OpenAI`, `#Lawsuit`, `#Trade Secrets`, `#Hardware`

---

<a id="item-7"></a>
## [6 U-Boot vulnerabilities enable boot-time code execution](https://www.bleepingcomputer.com/news/security/new-u-boot-flaws-could-enable-stealthy-firmware-attacks/) ⭐️ 8.0/10

Security vendor Binarly disclosed six vulnerabilities in the U-Boot bootloader's FIT image signature verification, two of which allow arbitrary code execution and four cause device crashes, affecting versions since 2013.07. These flaws reside in the pre-OS boot phase, enabling attackers to execute malicious code before the operating system and security software load, potentially bypassing firmware protections and implanting persistent malware. For systems with remote firmware update capabilities like BMCs, exploitation may occur without physical access. The vulnerabilities were found in the FIT (Flattened Image Tree) signature verification code, with two critical flaws enabling code execution and four denial-of-service issues. Patches have been submitted and accepted by U-Boot maintainers, but deployment requires integration by hardware vendors; end-of-life devices may never receive fixes.

telegram · zaihuapd · Jul 11, 08:32

**Background**: U-Boot is a widely used open-source bootloader for embedded systems, supporting many architectures like ARM, x86, and RISC-V. It loads the operating system kernel from storage or network. The FIT image format packages kernel, device tree, and other data into a single image, with signatures to verify authenticity and integrity. Baseboard Management Controllers (BMCs) are specialized microcontrollers for remote server management, often relying on U-Boot for booting.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Das_U-Boot">Das U - Boot - Wikipedia</a></li>
<li><a href="https://docs.u-boot.org/en/latest/usage/fit/signature.html">U-Boot FIT Signature Verification — Das U-Boot unknown version documentation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Intelligent_Platform_Management_Interface">Intelligent Platform Management Interface - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#security`, `#bootloader`, `#U-Boot`, `#vulnerabilities`, `#firmware`

---

<a id="item-8"></a>
## [Zhipu Founder Tang Jie Launches 'Touch High' AGI Plan](https://mp.weixin.qq.com/s/3CQSkf_kBnXiCDgS4L-Cgg) ⭐️ 8.0/10

Zhipu AI founder Tang Jie announced the 'Touch High' plan, outlining a path to AGI through four key challenges: long-horizon tasks, autonomous agents, self-training, and safety governance, with a massive investment in mechanistic interpretability. This plan signals a strategic shift for a major Chinese AI lab toward long-term AGI research over short-term monetization, potentially influencing the global AI race. The emphasis on safety and interpretability addresses growing concerns about black-box AI systems. The plan includes a huge investment in mechanistic interpretability to open the 'black box' of neural networks. Zhipu's GLM-5.2 model is reportedly close to frontier capabilities and is popular due to its open-source MIT license.

telegram · zaihuapd · Jul 11, 13:59

**Background**: Mechanistic interpretability is a subfield of AI safety research that aims to reverse-engineer neural networks into human-understandable algorithms by analyzing internal circuits and features. Zhipu AI (now rebranded as Z.ai) is known for its open-source GLM family of large language models, with GLM-5 being a 745B parameter model with 202K context length. The company has released models under the MIT License since July 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://en.wikipedia.org/wiki/Z.ai">Z.ai - Wikipedia</a></li>
<li><a href="https://glm5.ai/">GLM -5 - Zhipu AI's Flagship Foundation Model</a></li>

</ul>
</details>

**Tags**: `#AGI`, `#AI Safety`, `#Zhipu`, `#Interpretability`, `#Chinese AI`

---