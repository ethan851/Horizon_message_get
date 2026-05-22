---
layout: default
title: "Horizon Summary: 2026-05-22 (EN)"
date: 2026-05-22
lang: en
---

> From 34 items, 12 important content pieces were selected

---

1. [Freenet Relaunches as a Wasm-Powered Decentralized App Platform](#item-1) ⭐️ 9.0/10
2. [Nvidia CEO Says Company Has Abandoned China AI Chip Market](#item-2) ⭐️ 9.0/10
3. [Eli Lilly's retatrutide achieves 28.3% weight loss in phase 3 trial](#item-3) ⭐️ 9.0/10
4. [Local Video Indexing on MacBook with Gemma4-31B and 50GB Swap](#item-4) ⭐️ 8.0/10
5. [Python 3.15: Lesser-Known Features Shine](#item-5) ⭐️ 8.0/10
6. [Google Antigravity Update Overwrites User Installations](#item-6) ⭐️ 8.0/10
7. [News outlets block Internet Archive from archiving their journalism](#item-7) ⭐️ 8.0/10
8. [Nvidia Q4 revenue beats at $68.1B, Q1 guidance raised to $78B](#item-8) ⭐️ 8.0/10
9. [AMD Launches Ryzen AI Max 400 Series with 192 GB Memory](#item-9) ⭐️ 8.0/10
10. [Tencent Launches OS-Level AI Assistant Marvis](#item-10) ⭐️ 8.0/10
11. [China Reviews Meta's Manus Acquisition, Restricts Founders](#item-11) ⭐️ 8.0/10
12. [DeepSeek API Updates Rate Limits and User Isolation](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Freenet Relaunches as a Wasm-Powered Decentralized App Platform](https://freenet.org/) ⭐️ 9.0/10

Freenet has been completely redesigned and relaunched as a global decentralized key-value store where keys are WebAssembly contracts. It is now live with early applications including a decentralized group chat (River) and a CMS (Delta). This re-release revives a historic peer-to-peer project with a novel architecture that achieves fast, consistent state synchronization across peers using commutative merge operations. It offers a practical platform for building decentralized applications that run entirely in the browser without centralized APIs. The consistency model is based on Conflict-Free Replicated Data Types (CRDTs), requiring every contract to define a commutative merge operation. State updates propagate like a virus, typically achieving global consistency in seconds. The platform is not yet available on mobile devices.

hackernews · sanity · May 21, 14:34 · [Discussion](https://news.ycombinator.com/item?id=48223362)

**Background**: Freenet was originally created in 2000 as one of the first peer-to-peer anonymity networks. This new version is a complete rewrite from scratch, moving from file sharing to a decentralized key-value store where applications are WebAssembly contracts. The use of commutative merge operations is inspired by CRDTs, which guarantee eventual consistency without conflicts.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48223362">Show HN: Freenet, a peer-to-peer platform for decentralized apps</a></li>
<li><a href="https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type">Conflict-free replicated data type - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Some commenters criticized the decision to replace the original development team without their consent, calling it an "ivory tower" move by a board that was not active on the project. Others raised technical concerns about the merge approach, arguing that it pushes complexity onto users and may be vulnerable to malicious state claims, though some were excited about the potential of WASM-defined network behavior.

**Tags**: `#peer-to-peer`, `#decentralized`, `#webassembly`, `#distributed systems`, `#p2p`

---

<a id="item-2"></a>
## [Nvidia CEO Says Company Has Abandoned China AI Chip Market](https://www.cnbc.com/2026/05/21/nvidia-jensen-huang-china-ai-chip-market-huawei.html) ⭐️ 9.0/10

Nvidia CEO Jensen Huang announced that the company has 'essentially given up' on the Chinese AI chip market due to U.S. export restrictions, effectively ceding the market to domestic players like Huawei. This marks a major geopolitical shift in the AI chip supply chain, as China was once a significant revenue source for Nvidia. It accelerates China's push for self-sufficiency in AI semiconductors, with Huawei's Ascend chips emerging as a viable alternative. China previously accounted for at least one-fifth of Nvidia's data center revenue. In April 2026, the Trump administration required licenses for exporting advanced chips to China, effectively blocking Nvidia. Huang stated the company has told investors not to expect any licenses for selling advanced chips in China.

telegram · zaihuapd · May 21, 05:52

**Background**: Since 2022, the U.S. has imposed export controls on advanced AI chips to China, initially targeting Nvidia's A100 and H100 GPUs. The controls have tightened over time, blocking sales of flagship chips like the H100 and H200. Huawei has developed its own AI chip series, Ascend, with the 910C delivering about 60% of the H100's inference performance. In February 2026, Chinese AI startup Zhipu AI trained a frontier model entirely on Huawei's Ascend 910B chips.

<details><summary>References</summary>
<ul>
<li><a href="https://builtin.com/articles/trump-lifts-ai-chip-ban-china-nvidia">Trump Lifted the AI Chip Ban on China, Clearing Nvidia and AMD to Resume Sales: Now What? | Built In</a></li>
<li><a href="https://www.tomshardware.com/pc-components/gpus/huawei-introduces-the-ascend-920-ai-chip-to-fill-the-void-left-by-nvidias-h20">Huawei introduces the Ascend 920 AI chip to fill the... | Tom's Hardware</a></li>
<li><a href="https://thamizhelango.medium.com/mindspore-zhipu-ai-huawei-ascend-how-china-built-a-frontier-ai-model-without-a-single-nvidia-68403d92cedb">MindSpore, Zhipu AI & Huawei Ascend : How China Built... | Medium</a></li>

</ul>
</details>

**Tags**: `#AI芯片`, `#出口管制`, `#英伟达`, `#华为`, `#地缘政治`

---

<a id="item-3"></a>
## [Eli Lilly's retatrutide achieves 28.3% weight loss in phase 3 trial](https://www.prnewswire.com/news-releases/lillys-triple-agonist-retatrutide-delivered-powerful-weight-loss-in-pivotal-phase-3-obesity-trial-302778859.html) ⭐️ 9.0/10

Eli Lilly announced that retatrutide, a triple agonist, met all primary and key secondary endpoints in the phase 3 TRIUMPH-1 trial, with the 12 mg dose achieving an average weight loss of 28.3% over 80 weeks, and 45.3% of participants losing at least 30% of their body weight. This represents one of the highest average weight losses ever reported in a phase 3 obesity trial, signaling a potential paradigm shift in pharmacotherapy for obesity and related comorbidities, with substantial public health implications. The trial enrolled approximately 2,500 adults with obesity or overweight and at least one weight-related comorbidity; 4 mg dose achieved 19.0% average weight loss, and discontinuation due to adverse events was 4.1% for 12 mg group (vs. 4.9% for placebo), with gastrointestinal side effects being common but no identified cardiac or liver issues.

telegram · zaihuapd · May 22, 02:18

**Background**: Retatrutide is an investigational triple hormone receptor agonist that simultaneously targets GLP-1, GIP, and glucagon receptors, designed to enhance weight loss beyond existing dual agonists like tirzepatide. GLP-1 receptor agonists are a class of medications that reduce appetite and blood sugar, originally developed for type 2 diabetes and now increasingly used for obesity. This triple mechanism aims to further amplify metabolic benefits.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retatrutide">Retatrutide - Wikipedia</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC12190491/">Retatrutide—A Game Changer in Obesity Pharmacotherapy - PMC</a></li>

</ul>
</details>

**Tags**: `#obesity`, `#clinical trial`, `#GLP-1`, `#retatrutide`, `#weight loss`

---

<a id="item-4"></a>
## [Local Video Indexing on MacBook with Gemma4-31B and 50GB Swap](https://blog.simbastack.com/indexed-a-year-of-video-locally/) ⭐️ 8.0/10

A developer built a local video index of a year's personal footage using Google's Gemma4-31B model on a 2021 MacBook, utilizing 50GB of swap memory to handle the model's memory footprint. The code was released on GitHub under the MIT license. This shows that large language models can be deployed for practical, privacy-preserving personal archival work on consumer hardware without relying on cloud services. It enables efficient local video retrieval and analysis, and the project plans to integrate with video editing software like DaVinci Resolve. The Gemma4-31B model at 4-bit quantization would be about 19 GiB, but the developer's setup used 28.4 GiB for model weights and image context, with additional swap usage. The heavy swap may accelerate SSD wear. The project also aims to leverage the index for faster video editing via DaVinci Resolve.

hackernews · asenna · May 21, 14:01 · [Discussion](https://news.ycombinator.com/item?id=48222733)

**Background**: Large language models (LLMs) like Gemma4-31B require significant RAM; when RAM is insufficient, operating systems use swap space on disk, which can slow performance and reduce SSD lifespan. Gemma4-31B is a dense 31B parameter model from Google that achieves state-of-the-art results on math and coding benchmarks, often surpassing models with over 400B parameters. Running such models locally requires careful memory management, often involving quantization and swap.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.google.dev/gemma/docs/core/model_card_4">Gemma 4 model card | Google AI for Developers</a></li>
<li><a href="https://tech-insider.org/google-gemma-4-open-model-benchmarks-2026/">Gemma 4: How a 31B Model Beats 400B Rivals [2026]</a></li>
<li><a href="https://ryanagibson.com/posts/run-llms-larger-than-ram/">How to Run LLMs Larger than RAM · Ryan A. Gibson</a></li>

</ul>
</details>

**Discussion**: Commenters shared insights: one described a similar Electron app using Whisper and embeddings, another questioned the swap usage given quantization reduces memory needs, and the author responded by creating a public GitHub repo. The discussion reflects interest in local video indexing and practical LLM deployment.

**Tags**: `#local-llm`, `#video-indexing`, `#personal-archives`, `#gemma`, `#machine-learning`

---

<a id="item-5"></a>
## [Python 3.15: Lesser-Known Features Shine](https://blog.changs.co.uk/python-315-features-that-didnt-make-the-headlines.html) ⭐️ 8.0/10

Python 3.15 introduces iterator synchronization primitives in the threading module and adds symmetric difference support to collections.Counter, among other behind-the-scenes improvements. These additions improve Python's concurrency toolkit and complete the multiset operations on Counter, benefiting developers working with threaded iterators and data analysis tasks. The iterator synchronization primitives allow safe concurrent iteration over generators. Counter's symmetric_difference method computes the symmetric difference of two counter objects, a feature requested in Python Enhancement Proposals and discussed on GitHub.

hackernews · rbanffy · May 21, 11:10 · [Discussion](https://news.ycombinator.com/item?id=48220696)

**Background**: Python's threading module has long provided synchronization primitives like locks and events, but iterators were not thread-safe. The new primitives address this gap. The collections.Counter class, introduced in Python 2.7, supports multiset operations; symmetric difference was the missing operation, now added in 3.15.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.python.org/3/library/asyncio-sync.html">Synchronization Primitives — Python 3.14.5 documentation</a></li>
<li><a href="https://docs.python.org/3/library/threadsafety.html">Thread Safety Guarantees — Python 3.14.5 documentation</a></li>
<li><a href="https://discuss.python.org/t/add-symmetric-difference-to-collections-counter/103579">Add symmetric difference to collections.Counter - Ideas - Discussions on Python.org</a></li>

</ul>
</details>

**Discussion**: Commenters show mixed reactions: some praise the new iterator synchronization, while one user questions feature creep. Another user notes a potential error in the blog's Counter example, and a discussion about lazy imports clarifies that it is not a new feature.

**Tags**: `#Python`, `#Python 3.15`, `#programming languages`, `#features`, `#threading`

---

<a id="item-6"></a>
## [Google Antigravity Update Overwrites User Installations](https://www.0xsid.com/blog/antigravity-bait-n-switch) ⭐️ 8.0/10

Google released a new version of Antigravity that overwrites existing installations and user settings without clear migration, causing confusion and data loss for many developers. This update undermines trust in Google's developer tools and highlights a major user experience failure, especially as Antigravity is positioned as a key AI development platform. The update merges previous tools like Gemini CLI into Antigravity CLI and IDE, but does not preserve existing configurations, requiring users to manually restore settings and databases.

hackernews · ssiddharth · May 21, 13:50 · [Discussion](https://news.ycombinator.com/item?id=48222529)

**Background**: Google Antigravity is a suite of AI development tools including an IDE, CLI, and chat interface. It was introduced as a replacement for earlier tools like Gemini CLI and Code Assist. The recent update aimed to unify these products under the Antigravity brand.

<details><summary>References</summary>
<ul>
<li><a href="https://antigravity.google/changelog">Google Antigravity Changelog</a></li>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/google-io-2026-developer-highlights/">I/O 2026 developer highlights: Antigravity, Gemini API, AI Studio</a></li>
<li><a href="https://developers.googleblog.com/an-important-update-transitioning-gemini-cli-to-antigravity-cli/">An important update: Transitioning Gemini CLI to Antigravity CLI - Google Developers Blog</a></li>

</ul>
</details>

**Discussion**: Users expressed strong frustration, with some describing it as a 'bait and switch'. A developer provided a Python script to restore VS Code settings and chat history. Others criticized Google's lack of focus and poor update strategy.

**Tags**: `#Google`, `#User Experience`, `#Software Update`, `#Controversy`

---

<a id="item-7"></a>
## [News outlets block Internet Archive from archiving their journalism](https://www.niemanlab.org/2026/05/more-than-340-local-news-outlets-are-limiting-the-internet-archives-access-to-their-journalism/) ⭐️ 8.0/10

More than 340 local news outlets are using robots.txt files to restrict the Internet Archive's Wayback Machine from crawling and archiving their content, threatening the preservation of historical journalism. This limits public access to historical news and reduces the archive's ability to serve as a resource for researchers, journalists, and AI training. It also signals a growing tension between content monetization and digital preservation. The restrictions are implemented via robots.txt, a voluntary protocol that web crawlers typically respect. The Internet Archive must comply or risk being blocked entirely, though some archives have historically ignored robots.txt for non-commercial purposes.

hackernews · jaredwiener · May 21, 16:59 · [Discussion](https://news.ycombinator.com/item?id=48225838)

**Background**: Web archiving is the process of collecting and preserving web content for future access. The Internet Archive's Wayback Machine uses automated crawlers to capture snapshots of websites. Robots.txt is a standard that allows website owners to specify which parts of their site can be crawled, but compliance is voluntary. The growing use of robots.txt to block archival bots reflects a conflict between preserving public access and protecting revenue from paywalls or licensing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Robots.txt">Robots.txt</a></li>
<li><a href="https://en.wikipedia.org/wiki/Web_archiving">Web archiving</a></li>
<li><a href="https://en.wikipedia.org/wiki/Digital_preservation">Digital preservation</a></li>

</ul>
</details>

**Discussion**: Commenters expressed disappointment, noting the loss of historical content and the importance of the Wayback Machine for fact-checking and tracking edits. Some suggested a compromise like one-week delayed access, while others advocated for micropayment systems to compensate publishers without blocking archives.

**Tags**: `#Internet Archive`, `#digital preservation`, `#journalism`, `#web archiving`, `#AI training`

---

<a id="item-8"></a>
## [Nvidia Q4 revenue beats at $68.1B, Q1 guidance raised to $78B](https://t.me/zaihuapd/41498) ⭐️ 8.0/10

Nvidia reported Q4 fiscal 2025 revenue of $68.1 billion, exceeding market expectations, with data center revenue of $62.3 billion and EPS of $1.62 also beating estimates. The company guided Q1 fiscal 2026 revenue to $78 billion, significantly above the $72.6 billion consensus. This earnings report underscores sustained explosive demand for Nvidia's AI chips in data centers, reinforcing investor confidence in the AI hardware cycle. The raised guidance suggests the AI boom is still accelerating, impacting the entire semiconductor and AI ecosystem. Despite beating on top line, Nvidia's gaming and automotive segments missed expectations, and some investors expressed concerns about OpenAI's fundraising ability and competitive dynamics. CEO Jensen Huang noted exponential computing demand and strategic inventory measures to address supply chain pressures.

telegram · zaihuapd · May 21, 05:10

**Background**: Nvidia is the dominant supplier of graphics processing units (GPUs) used for AI training and inference, particularly its H100 and Blackwell series. The company's quarterly results are closely watched as a bellwether for AI industry demand. Data center revenue now accounts for over 90% of Nvidia's total revenue, reflecting the shift from PC gaming to AI computing.

**Tags**: `#nvidia`, `#earnings`, `#ai`, `#data center`, `#semiconductor`

---

<a id="item-9"></a>
## [AMD Launches Ryzen AI Max 400 Series with 192 GB Memory](https://www.techpowerup.com/349218/amd-launches-the-ryzen-ai-max-400-series-processors-strix-halo-gets-a-memory-upgrade) ⭐️ 8.0/10

AMD announced the Ryzen AI Max 400 series processors, an upgrade to the Strix Halo platform, increasing unified memory from 128 GB to 192 GB, with up to 160 GB allocable to the integrated GPU for running large language models with over 300 billion parameters. This development significantly boosts the capability of portable AI workstations, enabling developers to run massive AI models locally without discrete GPUs, and drives the trend of unified memory architectures in high-performance mobile computing. The first three models are PRO versions: the flagship 495 with 16 CPU cores and 40 Compute Units (CUs), and the 490 and 485 with 12/8 cores and 32 CUs respectively. Consumer variants are planned for later this year.

telegram · zaihuapd · May 21, 08:15

**Background**: AMD's Strix Halo platform integrates CPU, GPU, and NPU into a single chip with a unified memory architecture, allowing them to share a pool of memory. Unlike traditional discrete GPU setups where VRAM is limited, unified memory enables the integrated GPU to access large memory blocks, making it suitable for AI workloads like running large language models (LLMs) locally.

<details><summary>References</summary>
<ul>
<li><a href="https://www.servethehome.com/framework-desktop-review-a-solid-amd-strix-halo/">Framework Desktop Review A Solid AMD Strix Halo - ServeTheHome</a></li>
<li><a href="https://skip.watch/read?v=AcTmeGpzhBk">Running 110B LLMs on a Laptop: AMD's New APU vs.... - SkipWatch</a></li>

</ul>
</details>

**Tags**: `#AMD`, `#Ryzen AI Max`, `#处理器`, `#AI`, `#大语言模型`

---

<a id="item-10"></a>
## [Tencent Launches OS-Level AI Assistant Marvis](https://finance.sina.com.cn/jjxw/2026-05-21/doc-inhyrmmu5949795.shtml) ⭐️ 8.0/10

Tencent has officially launched Marvis, an operating system-level AI assistant with multi-agent orchestration and an on-device privacy mode, now available for free download without an invite code. This launch marks a significant step in integrating AI deeply into the OS layer, potentially transforming user interaction with devices and setting a new standard for privacy-preserving AI assistants from major tech companies. Marvis features six specialized agents coordinated by a main agent, and offers a privacy mode that runs entirely on-device using a local large language model, ensuring data never leaves the device. Each user receives 10 million free tokens per day.

telegram · zaihuapd · May 21, 10:00

**Background**: Multi-agent orchestration involves a lead agent that delegates tasks to specialized worker agents to handle complex workflows efficiently. On-device AI runs models directly on the user's hardware, enhancing privacy and enabling offline functionality. Marvis applies these concepts at the OS level to unify system, file, application, and cross-device capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Multi-agent_orchestration">Multi-agent orchestration</a></li>
<li><a href="https://grokipedia.com/page/On-device_artificial_intelligence">On-device artificial intelligence</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Operating System`, `#Tencent`, `#Privacy`, `#Agent`

---

<a id="item-11"></a>
## [China Reviews Meta's Manus Acquisition, Restricts Founders](https://t.me/zaihuapd/41509) ⭐️ 8.0/10

Chinese regulators are reviewing Meta's acquisition of AI startup Manus for potential investment violations, and have restricted co-founders Xiao Hong and Ji Yichao from leaving the country. This review signals heightened Chinese scrutiny over major cross-border AI acquisitions, potentially impacting future tech deals and geopolitical dynamics. The co-founders were told they cannot leave China after meeting with the National Development and Reform Commission, though they can travel domestically; the acquisition amount was not disclosed but earlier reports valued it at $2 billion.

telegram · zaihuapd · May 21, 13:11

**Background**: Manus is a general-purpose AI agent developed by Butterfly Effect, a company founded in China and based in Singapore. It autonomously executes complex tasks using tools like planning, reasoning, and action. Meta announced the acquisition in December 2024 to boost its AI capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus ( AI agent) - Wikipedia</a></li>
<li><a href="https://manus.im/">Manus : Hands On AI</a></li>
<li><a href="https://gcmori.medium.com/manus-ai-the-rise-of-the-general-ai-agent-88c54756295a">Manus AI : The Rise of the General AI Agent | by Giancarlo... | Medium</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#Acquisition`, `#AI`, `#China Regulation`, `#Geopolitics`

---

<a id="item-12"></a>
## [DeepSeek API Updates Rate Limits and User Isolation](https://api-docs.deepseek.com/zh-cn/quick_start/rate_limit) ⭐️ 8.0/10

DeepSeek has updated its API documentation to specify concurrency limits for V4 models (deepseek-v4-pro: 500, deepseek-v4-flash: 2500) and introduced a user_id parameter for finer-grained management including content safety, KVCache, and scheduling isolation. This update improves multi-tenant application management by allowing developers to isolate users within a single API account, and provides clear documentation to help users plan capacity and avoid HTTP 429 errors. Exceeding the concurrency limit returns an HTTP 429 error; users can request a free capacity expansion for higher limits. For standard API users, all user_ids share the account's total concurrency, while accounts with upgraded quotas have per-user_id concurrency limits matching the model.

telegram · zaihuapd · May 21, 15:03

**Background**: KVCache (Key-Value Cache) is an optimization technique in transformer-based large language models that caches intermediate key-value data from self-attention to speed up inference. The user_id isolation feature allows API consumers to assign different user IDs to different end users, enabling separate KVCache and scheduling policies per user within the same account. This is particularly useful for multi-tenant applications where each tenant requires isolated resources and security boundaries.

<details><summary>References</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/quick_start/rate_limit">Rate Limit & Isolation | DeepSeek API Docs</a></li>
<li><a href="https://hattussa.com/blog/boosting-transformer-efficiency-with-kvcache/">Boosting Transformer Efficiency with KVCache ! - Hattussa Blog...</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#API`, `#rate limiting`, `#concurrency`, `#user isolation`

---