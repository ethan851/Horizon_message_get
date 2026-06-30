---
layout: default
title: "Horizon Summary: 2026-06-30 (EN)"
date: 2026-06-30
lang: en
---

> From 30 items, 8 important content pieces were selected

---

1. [vLLM v0.24.0 Released with Major Optimizations and New Model Support](#item-1) ⭐️ 9.0/10
2. [Rocket Lab acquires Iridium in historic $8B deal](#item-2) ⭐️ 9.0/10
3. [Supreme Court: Geofence Warrants Need Constitutional Protections](#item-3) ⭐️ 9.0/10
4. [Game Boy JIT to WASM Beats Native Interpreter](#item-4) ⭐️ 8.0/10
5. [Full Pipeline of a CUDA Kernel Launch Explained](#item-5) ⭐️ 8.0/10
6. [Samsung, SK Hynix to Announce Record AI Investments](#item-6) ⭐️ 8.0/10
7. [CXMT signs $3B DRAM supply deal with Tencent](#item-7) ⭐️ 8.0/10
8. [Tesla Releases FSD v14 Lite for HW3 Vehicles](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.24.0 Released with Major Optimizations and New Model Support](https://github.com/vllm-project/vllm/releases/tag/v0.24.0) ⭐️ 9.0/10

The vLLM project released version 0.24.0 with 571 commits from 256 contributors, adding support for MiniMax-M3 and DeepSeek-V4 models, along with performance optimizations such as FlashInfer sparse index cache and Model Runner V2 quantization support. This release significantly improves the efficiency and versatility of vLLM, a widely used open-source LLM inference engine, benefiting developers deploying large language models in production with better performance and broader model compatibility. Notable technical improvements include the FlashInfer sparse index cache for DeepSeek-V4 (2-4% TTFT improvement), MXFP4 precision support for MiniMax-M3, and a cluster-cooperative topK kernel for low-latency sparse attention. Model Runner V2 now enables quantized models by default.

github · khluu · Jun 29, 19:41

**Background**: vLLM is an open-source high-performance inference engine for large language models, designed to deliver fast and efficient serving. It utilizes techniques like PagedAttention and continuous batching to optimize throughput and memory usage. The project supports a wide range of models and hardware backends, including NVIDIA and AMD GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.flashinfer.ai/api/sparse.html">flashinfer.sparse - FlashInfer 0.6.13 documentation</a></li>
<li><a href="https://rocm.blogs.amd.com/artificial-intelligence/w4a6-quant-mm/README.html">MXFP6 and MXFP 4 Mixed Precision for Accelerating... — ROCm Blogs</a></li>
<li><a href="https://github.com/vllm-project/vllm/blob/main/csrc/libtorch_stable/cooperative_topk.cu">vllm/csrc/libtorch_stable/cooperative_topk.cu at main - GitHub</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#AI inference`, `#model serving`, `#LLM optimization`, `#open source`

---

<a id="item-2"></a>
## [Rocket Lab acquires Iridium in historic $8B deal](https://investors.rocketlabcorp.com/news-releases/news-release-details/rocket-lab-acquire-iridium-historic-deal-creating-fully) ⭐️ 9.0/10

Rocket Lab announced on June 29 that it will acquire Iridium Communications in a cash-and-stock deal valued at approximately $8 billion, with an offer of $54 per share. The transaction has been unanimously approved by both boards and is expected to close by mid-2027, pending regulatory and Iridium shareholder approvals. This merger creates a fully integrated satellite and launch company, combining Rocket Lab's launch and spacecraft manufacturing with Iridium's global LEO satellite network, L-band spectrum, and over 500 partner ecosystem. It positions the combined entity to expand into satellite IoT, direct-to-device, and PNT markets, similar to how SpaceX leveraged Starlink to secure a baseline of launches. Iridium has over 2.55 million active subscribers, with 2025 revenue of $871.7 million and operating EBITDA of $495 million at a 57% margin. Rocket Lab has secured a $3.6 billion bridge loan commitment to support the acquisition. The deal values Iridium at an enterprise value of about $8 billion.

hackernews · everfrustrated · Jun 29, 14:09 · [Discussion](https://news.ycombinator.com/item?id=48719485)

**Background**: Rocket Lab is a leading launch provider and satellite manufacturer, known for its Electron rocket and upcoming Neutron. Iridium operates a constellation of 66 LEO satellites providing global voice and data services, including satellite phones and IoT connectivity. The acquisition allows Rocket Lab to own its own satellite constellation and spectrum, ensuring a steady launch demand and reducing reliance on external satellite customers.

**Discussion**: Community reactions highlight strategic parallels to SpaceX's Starlink model, with users noting that Rocket Lab gains a guaranteed launch baseline and profitable satellite business. Some express environmental concerns about space debris and the commercialization of low Earth orbit, while others praise the move as a smart hedge against market dips. A telegram comment summarizes the deal's financial details and strategic expansion into IoT and D2D markets.

**Tags**: `#space industry`, `#acquisition`, `#satellite communications`, `#Rocket Lab`, `#Iridium`

---

<a id="item-3"></a>
## [Supreme Court: Geofence Warrants Need Constitutional Protections](https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision) ⭐️ 9.0/10

On June 29, 2026, the US Supreme Court ruled that geofence warrants constitute a search under the Fourth Amendment, requiring probable cause and a warrant. The decision came in a case where law enforcement used a geofence warrant to obtain location data from Google's Sensorvault to identify suspects in a bank robbery. This landmark ruling establishes constitutional protections for digital location data, significantly impacting law enforcement surveillance practices and privacy rights. It sets a precedent that limits the use of bulk location data retrieval without individualized suspicion, affecting how police can use geofence warrants nationwide. The case involved a geofence warrant that directed Google to provide device IDs within 150 meters of a bank during a 30-minute window, initially returning 19 accounts. The court held that such a search implicates a reasonable expectation of privacy, as modern cell phones are pervasive and constantly track location.

hackernews · cdrnsf · Jun 29, 15:54 · [Discussion](https://news.ycombinator.com/item?id=48720924)

**Background**: A geofence warrant, also known as a reverse location warrant, is a search warrant that orders a company like Google to identify all mobile devices within a defined geographic area over a specific time period. Unlike traditional warrants targeting known individuals, geofence warrants seek to identify unknown suspects by their location data. Google's Sensorvault is a database that stores historical location data from users who have opted into location history. The widespread use of such warrants has raised privacy concerns due to their potential for mass surveillance and the minimal oversight previously required.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geofence_warrant">Geofence warrant</a></li>
<li><a href="https://www.scotusblog.com/2026/06/court-rules-that-law-enforcements-use-of-geofence-warrant-was-a-search/">Court rules that law enforcement’s use of “geofence warrant ...</a></li>

</ul>
</details>

**Discussion**: Commenters drew parallels between geofence warrants and wiretapping, noting that digital surveillance lacks the physical resource constraints that historically limited wiretap abuse. Some highlighted the specific data tranches in this case, where Google provided device IDs, then account email addresses, and finally subscriber information. Others mentioned alternative identification methods, such as cross-referencing hotel guest lists with IP geolocation, as illustrated in the Petraeus scandal. Overall, sentiment was supportive of the ruling as a necessary check on expanding surveillance powers.

**Tags**: `#privacy`, `#law`, `#surveillance`, `#Supreme Court`, `#geofence`

---

<a id="item-4"></a>
## [Game Boy JIT to WASM Beats Native Interpreter](https://humphri.es/blog/WATaBoy/) ⭐️ 8.0/10

WATaBoy, a Game Boy emulator, uses just-in-time (JIT) compilation to translate Game Boy instructions into WebAssembly (WASM), outperforming a native interpreter written in C. This approach demonstrates a novel way to achieve high-performance emulation on platforms that restrict native JIT, such as iOS, by leveraging WebAssembly's JIT capabilities inside browsers. The JIT compiler emits WASM modules dynamically, achieving a 25% performance improvement over the native interpreter in benchmarks; however, Firefox was found to be 25% slower than Chrome and Safari.

hackernews · energeticbark · Jun 29, 15:02 · [Discussion](https://news.ycombinator.com/item?id=48720190)

**Background**: JIT compilation compiles code at runtime to native machine code for faster execution, while interpreters execute instructions directly without compilation. WebAssembly is a low-level binary format that runs efficiently in modern browsers, and it can itself be JIT-compiled by the browser's JavaScript engine.

**Discussion**: Commenters praised the project as impressive for an undergraduate, and noted that WASM overhead (≈20%) is far lower than interpreter overhead (≈1000%), making the result expected. Some discussed iOS JIT restrictions and alternative approaches like JavaScript eval().

**Tags**: `#JIT compilation`, `#WebAssembly`, `#Game Boy emulation`, `#JavaScript`, `#emulator performance`

---

<a id="item-5"></a>
## [Full Pipeline of a CUDA Kernel Launch Explained](https://fergusfinn.com/blog/what-happens-when-you-run-a-gpu-kernel/) ⭐️ 8.0/10

A detailed blog post explains the complete pipeline from triggering a CUDA kernel on the CPU to its execution on the GPU, including the doorbell mechanism and warp scheduling. This deep dive bridges a common knowledge gap for CUDA developers by illuminating the often-opaque journey of a kernel launch from driver to hardware execution. The article covers the doorbell mechanism for submitting work to the GPU, the Queue Metadata (QMD) format, and warp scheduling with eligibility conditions, plus the implicit synchronization of commands in the default CUDA stream.

hackernews · mezark · Jun 29, 13:11 · [Discussion](https://news.ycombinator.com/item?id=48718863)

**Background**: In CUDA, a kernel is a function that runs on the GPU in parallel across many threads. Threads are grouped into warps (typically 32 threads), and the GPU schedules warps for execution. The doorbell mechanism is how the CPU notifies the GPU that new work is ready in a command queue. Warp scheduling is a technique where the GPU's warp scheduler rapidly switches between warps to hide latency.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Thread_block_(CUDA_programming)">Thread block (CUDA programming) - Wikipedia</a></li>
<li><a href="https://modal.com/gpu-glossary/device-hardware/warp-scheduler">What is a Warp Scheduler? | GPU Glossary</a></li>

</ul>
</details>

**Discussion**: Commenters highly praised the article for its clarity and depth, particularly the doorbell and QMD explanations. One user noted the contrast with Vulkan's explicit synchronization, and another speculated about the future of kernel optimization companies.

**Tags**: `#CUDA`, `#GPU`, `#kernel launch`, `#parallel computing`, `#systems`

---

<a id="item-6"></a>
## [Samsung, SK Hynix to Announce Record AI Investments](https://t.me/zaihuapd/42235) ⭐️ 8.0/10

Samsung and SK Hynix will announce massive AI investment plans at a national briefing led by President Lee Jae-myung on June 29. Samsung's ten-year plan involves 1,000 trillion won (about $648 billion), the largest in South Korean history, while SK Hynix aims to double capacity in five years and raise $29 billion via a U.S. listing. This investment signals a major strategic shift by South Korean semiconductor giants toward AI hardware, potentially reshaping the global AI chip supply chain. The scale could accelerate AI infrastructure buildout and intensify competition with memory leaders like Micron. On the same day, shares of both Samsung Electronics and SK Hynix fell over 9%, partly due to Apple-related concerns. The investments focus on semiconductors, AI data centers, and physical AI, with Samsung committing to the largest single corporate spending plan in Korean history.

telegram · zaihuapd · Jun 29, 07:00

**Background**: AI data centers are specialized facilities optimized for training and running AI models, relying heavily on high-bandwidth memory (HBM) like that produced by SK Hynix and Samsung. Physical AI refers to AI systems that can perceive and act in the physical world, such as robots and autonomous vehicles, which require advanced chips and memory. The announcement underscores South Korea's ambition to lead in the AI hardware race.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/glossary/generative-physical-ai/">What is Physical AI? | NVIDIA Glossary</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_data_center">AI data center</a></li>
<li><a href="https://grokipedia.com/page/Physical_AI">Physical AI</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#AI`, `#investment`, `#Samsung`, `#SK Hynix`

---

<a id="item-7"></a>
## [CXMT signs $3B DRAM supply deal with Tencent](https://www.reuters.com/world/china/chinas-cxmt-wins-3-billion-memory-supply-deal-with-tencent-sources-say-2026-06-29/) ⭐️ 8.0/10

Chinese DRAM maker CXMT has signed a long-term supply deal worth nearly $3 billion with Tencent to provide server memory chips over a period of three to five years. This deal marks a major adoption of Chinese-made memory chips by a top tech firm, potentially reshaping the global DRAM supply chain and reducing reliance on foreign suppliers like Samsung and SK Hynix. The agreement is valued at over 20 billion yuan (about $2.94 billion), with the contract duration reported as three years by two sources and five years by another. CXMT is also reportedly in talks with Alibaba Cloud, ByteDance, and Xiaomi.

telegram · zaihuapd · Jun 29, 09:31

**Background**: CXMT is one of China's leading DRAM manufacturers, crucial for the country's push for semiconductor self-sufficiency. DRAM is a type of memory used in servers, PCs, and smartphones. Historically, the DRAM market has been dominated by Samsung, SK Hynix, and Micron.

**Tags**: `#DRAM`, `#China`, `#Tencent`, `#supply chain`, `#memory chips`

---

<a id="item-8"></a>
## [Tesla Releases FSD v14 Lite for HW3 Vehicles](https://x.com/Tesla_AI/status/2071592820889260101) ⭐️ 8.0/10

Tesla released FSD v14 Lite on June 29, 2026, enabling HW3 vehicles to gain HW4-level self-driving and automatic parking capabilities. This update significantly improves the autonomous driving experience for millions of HW3 Tesla owners, bridging the gap between hardware generations and extending the lifespan of older vehicles. The update includes features previously exclusive to HW4, such as reinforcement learning and offline models, and introduces new capabilities like starting from park, reversing, and parking at destination.

telegram · zaihuapd · Jun 30, 02:26

**Background**: Tesla's Full Self-Driving (FSD) system is a suite of advanced driver-assistance features. Hardware 3 (HW3) and Hardware 4 (HW4) are different generations of Tesla's onboard computer, with HW4 offering more processing power and additional sensors, enabling more advanced autonomous driving capabilities. FSD v14 Lite is a specialized software version that brings HW4-level features to HW3 vehicles through software optimization and knowledge distillation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.basenor.com/blogs/news/tesla-update-v14-lite-1">FSD 14 Lite: Everything HW3 Owners Need to Know</a></li>
<li><a href="https://www.notateslaapp.com/news/4038/tesla-announces-fsd-v14-lite-features-and-release-timeline">Tesla Provides Update on FSD v14 Lite for HW3: Included ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Autopilot_hardware">Tesla Autopilot hardware - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#FSD`, `#autonomous driving`, `#HW3`, `#update`

---