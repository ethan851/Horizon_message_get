---
layout: default
title: "Horizon Summary: 2026-08-26 (EN)"
date: 2026-08-26
lang: en
---

> From 36 items, 12 important content pieces were selected

---

1. [Apple unveils M6 and M5 Ultra with big performance and AI leap](#item-1) ⭐️ 9.0/10
2. [OpenAI Claims Custom Jalapeño Chip Outperforms Nvidia Blackwell](#item-2) ⭐️ 9.0/10
3. [FDA Authorizes First Wearable That Tracks Both Ketones and Blood Sugar](#item-3) ⭐️ 8.0/10
4. [Apple Unveils Mac Studio with M5 Max and M5 Ultra for Local AI](#item-4) ⭐️ 8.0/10
5. [Apple Unveils Mac mini with M6 and M5 Pro Chips](#item-5) ⭐️ 8.0/10
6. [Nitter Receives Cease and Desist, Shuts Down All Public Instances](#item-6) ⭐️ 8.0/10
7. [My Friend Aaron Reveals the Destructive Pull of Get-Rich-Quick Schemes](#item-7) ⭐️ 8.0/10
8. [Firefox 157 to Enable JPEG XL by Default Across All Platforms](#item-8) ⭐️ 8.0/10
9. [SpaceX Confirms New Starbase Facility in Louisiana](#item-9) ⭐️ 8.0/10
10. [SpaceX to Launch Nvidia Vera Rubin NVL72 Into Orbit by 2027](#item-10) ⭐️ 8.0/10
11. [NVIDIA Benchmarks Vera Rubin NVL72: 30x Throughput Gain on DeepSeek Agents](#item-11) ⭐️ 8.0/10
12. [Microsoft Paint, Photos Embed Invisible Remote-Review Watermarks in Local AI Images](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Apple unveils M6 and M5 Ultra with big performance and AI leap](https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/) ⭐️ 9.0/10

On August 25, 2026, Apple announced the M6, its first 2nm chip, and the M5 Ultra, its first quad-die chip and most powerful processor ever. The M6 features a 12-core CPU, 12-core GPU, and Dual 16-core Neural Engine delivering up to 2x peak AI compute. This marks Apple's aggressive push into on-device AI compute, potentially reshaping the high-end laptop and workstation market. The M6's 2nm process and M5 Ultra's quad-die architecture set new benchmarks for performance-per-watt and AI capabilities in Apple silicon. The M5 Ultra is built by connecting two dual-die M5 Max chips via next-generation UltraFusion technology, achieving inter-die bandwidth over 4.4TB/s. The M6 is Apple's first 2nm chip, and Apple states that system frameworks can automatically utilize both Neural Engines simultaneously for faster model execution.

hackernews · interpol_p · Aug 25, 13:01 · [Discussion](https://news.ycombinator.com/item?id=49433292)

**Background**: Apple silicon refers to Apple's custom ARM-based system-on-a-chip (SoC) family, replacing Intel processors in Macs since 2020. The Neural Engine is a dedicated processor for machine learning tasks, and UltraFusion is Apple's proprietary chip-to-chip interconnect that scales performance by combining multiple dies. These announcements continue Apple's push to integrate advanced AI features on-device.

<details><summary>References</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/08/apple-introduces-m6-and-m5-ultra-for-a-big-leap-in-performance-and-ai-compute/">Apple introduces M6 and M5 Ultra for a big leap in performance and AI ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_M6">Apple M6 - Wikipedia</a></li>
<li><a href="https://www.macrumors.com/2026/08/25/apple-debuts-m5-ultra/">Apple Debuts M5 Ultra as Most Powerful Chip Ever - MacRumors</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement about the performance gains but also criticized high prices, with one estimating a fully maxed-out Mac Studio would cost around $24,699. Some highlighted rumors that Apple may skip M6 Pro/Max/Ultra to focus on an AI-focused M7, while others compared the chip competition to the late 90s.

**Tags**: `#Apple`, `#Chip`, `#AI compute`, `#Hardware`, `#M6`

---

<a id="item-2"></a>
## [OpenAI Claims Custom Jalapeño Chip Outperforms Nvidia Blackwell](https://newsletter.semianalysis.com/p/openai-jalapeno-better-than-nvidia) ⭐️ 9.0/10

OpenAI has published initial test results for its custom inference chip, Jalapeño, co-designed with Broadcom. The company claims it delivers higher energy efficiency and lower latency than Nvidia's Blackwell processors on large language models including GPT-OSS 120B, DeepSeek R1 670B, and Kimi K2.5 1T. This marks a major escalation in the AI hardware race, as a leading AI lab directly challenges Nvidia's dominance. If Jalapeño lives up to the claims, it could lower inference costs, reduce OpenAI's dependence on Nvidia GPUs, and push the broader industry toward specialized inference chips. Jalapeño is an LLM-optimized ASIC focused on inference, not training, and represents the first step in OpenAI's multi-generation compute platform. The test results cover peak-throughput workloads on several large models, with the company emphasizing throughput per watt and latency improvements.

hackernews · bmulholland · Aug 25, 14:06 · [Discussion](https://news.ycombinator.com/item?id=49434378)

**Background**: Nvidia's Blackwell architecture is the current flagship GPU platform for AI, powering systems like the GB200 NVL72 and RTX 50-series. OpenAI has historically relied on Nvidia GPUs for both training and inference, but has been investing in custom silicon to optimize costs and performance. Jalapeño is an application-specific integrated circuit (ASIC) designed specifically to run large language models faster and more efficiently than general-purpose GPUs. This move is part of a broader trend of AI labs, including Anthropic, developing their own hardware to gain a competitive edge.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/openais-jalapeño-chip-what-developers-need-know-its-move-ashish-jain-9uoof">OpenAI ’s Jalapeño Chip : What Developers Need to Know About Its...</a></li>
<li><a href="https://www.nxcode.io/resources/news/openai-broadcom-jalapeno-inference-chip-developer-guide-2026">OpenAI Jalapeño Chip Guide: What It Means for AI Coding... | NxCode</a></li>
<li><a href="https://www.tomshardware.com/pc-components/gpus/nvidia-blackwell-architecture-deep-dive-a-closer-look-at-the-upgrades-coming-with-rtx-50-series-gpus">Nvidia Blackwell architecture deep dive: A closer... | Tom's Hardware</a></li>

</ul>
</details>

**Discussion**: Commenters offered a range of technical and strategic perspectives. Some speculated about baking model weights directly into chips or compared this to the early GPU market's fragmentation, while others questioned specific claims and noted that human speech remains far more energy-efficient. Overall sentiment was analytical and cautiously optimistic, with attention to trade-offs like FP4 precision and die size.

**Tags**: `#AI Hardware`, `#OpenAI`, `#Nvidia`, `#Chip Design`, `#Inference`

---

<a id="item-3"></a>
## [FDA Authorizes First Wearable That Tracks Both Ketones and Blood Sugar](https://www.fda.gov/news-events/press-announcements/fda-authorizes-first-wearable-device-continuously-monitors-both-ketone-levels-and-blood-sugar) ⭐️ 8.0/10

The U.S. Food and Drug Administration has authorized the first wearable device that continuously monitors both ketone levels and blood glucose. This marks a regulatory first for combined metabolic tracking in a single wearable. This milestone could significantly improve daily management for people with diabetes, especially those at risk of diabetic ketoacidosis, and for individuals following ketogenic or low-carb diets. It also paves the way for future closed-loop or automated insulin delivery systems that incorporate ketone data. The device appears to be a sensor inserted under the skin, similar to a continuous glucose monitor, rather than a noninvasive wearable. Ketones in the blood are typically elevated only during fasting, low-carbohydrate intake, or when blood sugar is poorly controlled, so the feature may be most useful for specific patient groups.

hackernews · sunnynagra · Aug 25, 19:07 · [Discussion](https://news.ycombinator.com/item?id=49439017)

**Background**: Ketone bodies are molecules produced by the liver from fatty acids when glucose is not available for energy, such as during fasting or low-carb diets; they can be measured in blood, urine, or breath. Continuous glucose monitors (CGMs) are small wearable sensors that track glucose levels in real time through a filament inserted under the skin. This new device combines both capabilities in one wearable, offering a more complete picture of metabolic state.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ketone_bodies">Ketone bodies - Wikipedia</a></li>
<li><a href="https://my.clevelandclinic.org/health/body/25177-ketones">Ketones: What They Are, Function, Tests & Normal Levels</a></li>
<li><a href="https://medicalxpress.com/news/2026-07-wearable-tracks-glucose-ketone-biomarkers.html">New wearable ring tracks glucose , ketone and other biomarkers in...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed emotional support, with one sharing a personal story of a friend who died from diabetic ketoacidosis, while others voiced skepticism about the accuracy of noninvasive sensing and questioned the 'wearable' label since it is inserted into the arm. A technical comment noted that ketones are only elevated in extreme dietary or glycemic states, so the feature may have limited utility for an average diabetic. Calls for better reimbursement to increase access were also raised.

**Tags**: `#FDA`, `#wearables`, `#health-tech`, `#diabetes`, `#medical-devices`

---

<a id="item-4"></a>
## [Apple Unveils Mac Studio with M5 Max and M5 Ultra for Local AI](https://www.apple.com/newsroom/2026/08/apple-introduces-new-mac-studio-with-m5-max-and-m5-ultra/) ⭐️ 8.0/10

Apple announced the new Mac Studio featuring its M5 Max and M5 Ultra chips, calling it the company's most powerful Mac ever. Pre-orders are open, with availability starting September 22. This matters because Apple is positioning the Mac Studio as a local AI workstation capable of running frontier-class AI models on-device, potentially reducing reliance on cloud AI. It could appeal to developers and researchers who need high memory bandwidth and performance for large language models without cloud costs. The M5 generation adds a neural accelerator to each GPU core, and the M5 Max scales up to 40 GPU cores. The M5 Ultra, built from two M5 Max dies via UltraFusion, reportedly offers up to 1.2 TB/s memory bandwidth; community discussion notes high pricing, with 256GB memory around $10,000 and 512GB versions potentially delayed until October.

hackernews · interpol_p · Aug 25, 13:03 · [Discussion](https://news.ycombinator.com/item?id=49433316)

**Background**: Apple silicon is a line of ARM-based system-on-a-chip (SoC) designs used in Macs, iPhones, and iPads. The M5 is the latest generation, succeeding the M4, and introduces a next-generation GPU architecture with integrated Neural Accelerators for AI workloads. The M1 Ultra, introduced in 2022, established the UltraFusion interconnect that combines two dies; the M5 Ultra likely follows the same approach. Mac Studio is a desktop computer aimed at professionals, offering more performance and ports than a MacBook Pro in a stationary form factor.

<details><summary>References</summary>
<ul>
<li><a href="https://www.apple.com/newsroom/2026/08/apple-introduces-new-mac-studio-with-m5-max-and-m5-ultra/">Apple introduces new Mac Studio with M 5 Max and M 5 Ultra - Apple</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_M5">Apple M5 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_M1_Ultra">Apple M1 Ultra</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some praise Apple's focus on local AI and note achievable token throughput (e.g., ~1000+ tok/s prefill for a non-quantized DeepSeek V4), while others criticize high memory prices, the overuse of 'up to' in marketing, and lack of future-proofing for models over 1 trillion parameters. There's also speculation about pairing a Studio with a laptop for remote use.

**Tags**: `#apple`, `#hardware`, `#ai`, `#mac-studio`, `#m5`

---

<a id="item-5"></a>
## [Apple Unveils Mac mini with M6 and M5 Pro Chips](https://www.apple.com/newsroom/2026/08/apple-unveils-a-more-powerful-mac-mini-featuring-the-all-new-m6-and-m5-pro/) ⭐️ 8.0/10

In August 2026, Apple announced a new Mac mini powered by the all-new M6 and M5 Pro chips. The M6 is Apple's first 2nm chip, while the M5 Pro is the higher-end option previously introduced in the MacBook Pro. This update brings Apple's latest silicon to its most accessible desktop, giving developers and prosumers a compact, powerful machine. It also marks a pricing shift for the Mac mini, which has historically been Apple's budget-friendly entry point and is now crossing the €1000 threshold in some configurations. The M6 is Apple's first 2nm chip, with a 12-core CPU, 12-core GPU, and a Dual 16-core Neural Engine that doubles AI performance. The M5 Pro, built on Apple's new Fusion Architecture, offers up to an 18-core CPU, 20-core GPU, hardware-accelerated ray tracing, and a 16-core Neural Engine.

hackernews · runako · Aug 25, 13:13 · [Discussion](https://news.ycombinator.com/item?id=49433450)

**Background**: Apple began transitioning its Mac lineup from Intel processors to its own ARM-based 'Apple silicon' chips with the M1 in late 2020. The Mac mini has long served as Apple's most affordable desktop, appealing to developers and home users. The M-series naming follows a pattern: base chips use a simple number (e.g., M6), while 'Pro' and 'Max' variants offer more CPU and GPU cores for demanding workflows. The M6 represents a major process node shrink to 2nm, while the M5 Pro is an upper-mid-range chip introduced earlier in 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apple_M6">Apple M 6 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_M5">Apple M5 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_m1_chip">Apple m1 chip</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed feelings: some are happy with their previous budget M4 Mac mini purchases, while others lament the end of the ultra-cheap Mac mini era as European prices now exceed €1000. There are also complaints about the lack of immediate ordering availability, a request for direct M6 vs M5 Pro benchmarks rather than comparisons to older M1 chips, and some concern about Apple's 'always-on agentic computing' marketing language.

**Tags**: `#Apple`, `#Mac mini`, `#M6`, `#M5 Pro`, `#hardware`

---

<a id="item-6"></a>
## [Nitter Receives Cease and Desist, Shuts Down All Public Instances](https://github.com/zedeus/nitter/issues/1442) ⭐️ 8.0/10

Nitter project received cease and desist letters, prompting maintainers to shut down all public instances pending legal advice. The announcement was made on the project's GitHub issue tracker, with no immediate details about the sender or specific claims. This legal action threatens a widely used privacy tool and signals growing corporate hostility toward open-source projects that bypass platform limitations. It directly impacts privacy-conscious users and community-run instances that rely on Nitter to access Twitter/X without tracking, ads, or an account. The announcement gave no specific details about the letters or the sender, only that legal advice is being sought and instances will remain down for the foreseeable future. The project's GitHub wiki and third-party health trackers already list many instances as offline, and the developer has long advised users not to use instances for scraping.

hackernews · Banditoz · Aug 25, 17:08 · [Discussion](https://news.ycombinator.com/item?id=49437283)

**Background**: Nitter is a free and open-source alternative frontend for Twitter/X focused on privacy and performance. It routes all requests through a server-side backend so the client never talks to Twitter directly, preventing IP tracking and JavaScript fingerprinting, and it requires no user account. Nitter is typically accessed through community-run instances, which are listed in its wiki and monitored by uptime trackers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nitter">Nitter - Wikipedia</a></li>
<li><a href="https://github.com/zedeus/nitter">GitHub - zedeus/nitter: Alternative Twitter front-end Active Nitter instances · GitHub Nitter - Wikipedia A nitter instance that still works almost perfectly Instances - zedeus/nitter GitHub Wiki Nitter Instance Health - d420</a></li>

</ul>
</details>

**Discussion**: Commenters expressed disappointment and frustration, noting that many organizations still use X as their main communication channel, with one saying this should push people to leave X but expecting little change. Others suggested middle powers should offer legal protection for such privacy projects, calling U.S. tech companies hostile. Some commenters reminded that Nitter instances should not be used for scraping, and a few used the opportunity to praise supportive community maintainers (e.g., dang from Hacker News) as a contrast.

**Tags**: `#privacy`, `#legal`, `#open-source`, `#twitter`, `#nitter`

---

<a id="item-7"></a>
## [My Friend Aaron Reveals the Destructive Pull of Get-Rich-Quick Schemes](https://rorz.io/writing/my-friend-aaron) ⭐️ 8.0/10

The personal essay 'My Friend Aaron' was posted to Hacker News by author sarreph and quickly rose to the front page, earning 429 points and 117 comments. The story traces a friend's slow descent into get-rich-quick schemes involving AI, prediction markets, and live streaming. The essay has struck a nerve in the tech community because it captures a recognizable archetype: the relentless 'schemer' who chases shortcuts instead of steady work. It has sparked broader reflection on startup culture, parasocial relationships, and the human cost of founder myths. The story weaves together several recognizable modern elements: heavy AI use, prediction markets, live streaming, and a friend who gradually loses his moral compass. The author noted that he originally submitted the piece to a writing contest and received no response, making the front-page reception on HN far more meaningful.

hackernews · sarreph · Aug 25, 16:53 · [Discussion](https://news.ycombinator.com/item?id=49437069)

**Background**: Hacker News is a technology-focused social news site where community members share articles and long-form personal essays about startup life. This essay participates in a longstanding tradition of tech-culture writing that examines the personality types and psychological pressures common in startup ecosystems. The 'schemer' is a familiar figure in that world: someone constantly hunting for an angle rather than doing unglamorous work.

**Discussion**: Commenters widely praised the writing, with many saying they personally know an 'Aaron' and could see how the character's delusions evolved believably. Discussion also connected the story to Justin.tv and Twitch, noting how livestreaming fosters parasocial friendships, and to the broader pattern of otherwise capable people wasting years on dubious schemes.

**Tags**: `#startup-culture`, `#personal-essay`, `#hackernews`, `#tech-culture`, `#writing`

---

<a id="item-8"></a>
## [Firefox 157 to Enable JPEG XL by Default Across All Platforms](https://groups.google.com/a/mozilla.org/g/dev-platform/c/3YMV4MS34KA?pli=1) ⭐️ 8.0/10

Firefox 157 will include JPEG XL support enabled by default on all platforms, according to a Mozilla dev-platform announcement. This marks a major step toward adoption of the next-generation image format across the web. With both Firefox and Chromium reportedly moving to enable JPEG XL by default, the industry is converging on a modern image format that offers superior compression and features. This could speed up web-wide adoption of JPEG XL and eventually displace legacy JPEG and PNG in many use cases. The announcement confirms that desktop and mobile builds of Firefox 157 will be affected, with the change appearing in the beta branch. Community discussion notes that both Firefox and Chromium base their implementations on jxl-rs, a Rust library, while Apple has shipped the C++ libjxl.

hackernews · yboris · Aug 25, 17:55 · [Discussion](https://news.ycombinator.com/item?id=49437946)

**Background**: JPEG XL (or JXL) is a free and open image format standardized as ISO/IEC 18181, developed by the Joint Photographic Experts Group, Google, and Cloudinary. It supports both lossy and lossless compression, wide color gamut, high dynamic range, and high bit depth, making it well suited for web delivery and professional photography. Unlike older formats such as JPEG, PNG, and WebP, JPEG XL offers significantly better compression efficiency and features such as progressive decoding and lossless JPEG transcoding.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/JPEG_XL">JPEG XL - Wikipedia</a></li>
<li><a href="https://jpeg.org/jpegxl/">JPEG - JPEG XL</a></li>
<li><a href="https://jpegxl.info/">JPEG XL: Superior Image Compression</a></li>

</ul>
</details>

**Discussion**: Commenters expressed curiosity about Apple's approach, wondering whether it will use Rust for its JPEG XL implementation or continue with the shipped C++ libjxl. Others hope JXL will become the universal default so that even non-technical users stop sharing JPEGs, while some asked for browser features to automatically convert JXL to other formats for sites that don't support it.

**Tags**: `#jpeg-xl`, `#web-platform`, `#browsers`, `#image-formats`, `#mozilla`

---

<a id="item-9"></a>
## [SpaceX Confirms New Starbase Facility in Louisiana](https://www.spacex.com/sites/starbase-la) ⭐️ 8.0/10

SpaceX has officially confirmed plans to build a new Starbase facility in Louisiana, following months of speculation. The announcement highlights economic opportunities for the region and unique launch advantages, including improved access to Sun-synchronous orbits. This marks SpaceX's second Starbase after the Texas facility, potentially transforming coastal Louisiana's economy and expanding the company's launch capabilities. It could create decades of construction and operations jobs in one of the US's poorest areas, while providing strategic orbital access. The proposed Louisiana site provides favorable access to Sun-synchronous orbits (SSO), with a launch angle of about 98° relative to the equator. Speculation about the site had been circulating since May, and the official page's environmental copy has drawn criticism for nearly identical duplicated paragraphs.

hackernews · bilsbie · Aug 25, 16:37 · [Discussion](https://news.ycombinator.com/item?id=49436822)

**Background**: SpaceX Starbase is the company's industrial complex and rocket launch facility, currently located in South Texas near Brownsville, where the company develops and tests its Starship vehicles. The site was incorporated as a city named Starbase, Texas in May 2025 after a voter-approved election. A new Louisiana facility would be SpaceX's second such privately owned launch and production base, following years of expansion at the original Texas location.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SpaceX_Starbase">SpaceX Starbase</a></li>

</ul>
</details>

**Discussion**: Community reactions are broadly positive about the local economic impact, with one commenter noting a decade or two of solid work for welders, concrete workers, and contractors in coastal Louisiana. Others are enthusiastic about ambitious real-world engineering projects, but some remain skeptical of Musk's timelines. Critics also pointed out that the official page contains nearly identical duplicated paragraphs about shoreline restoration and marshland rebuilding, suggesting the copy may have been generated by an LLM.

**Tags**: `#SpaceX`, `#Starbase`, `#Louisiana`, `#Space industry`, `#Launch site`

---

<a id="item-10"></a>
## [SpaceX to Launch Nvidia Vera Rubin NVL72 Into Orbit by 2027](https://www.theregister.com/off-prem/2026/08/25/spacex-claims-it-will-put-a-vera-rubin-nvl72-rack-scale-system-into-orbit-next-year/5292067) ⭐️ 8.0/10

SpaceX announced plans to launch an Nvidia Vera Rubin NVL72 rack-scale AI system into orbit by 2027, marking an early effort to test orbital AI computing. The system combines 72 Rubin GPUs and 36 Vera CPUs and consumes over 100 kilowatts. If successful, this could move the industry closer to space-based data centers, reducing dependence on terrestrial land, electricity, cooling, and water. It would also expand AI infrastructure beyond Earth and test whether the most advanced AI hardware can operate reliably in orbit. The NVL72 is designed to act as a single giant GPU, using NVLink 6 switching, ConnectX-9 SuperNICs, BlueField-4 DPUs, and liquid cooling, so any orbital deployment must solve power supply, heat rejection, radiation shielding, and data communications. SpaceX has not yet disclosed the launch vehicle, target orbit altitude, or how the system will be powered and cooled in space.

telegram · zaihuapd · Aug 25, 08:03

**Background**: Nvidia's Vera Rubin NVL72 is a rack-scale AI supercomputer that packages 72 Rubin GPUs and 36 Vera CPUs with high-bandwidth NVLink 6 interconnect so the whole rack behaves like one massive GPU, designed for next-generation agentic AI. Space-based data centers are a concept that would place AI processing and storage in satellites, potentially cutting the land, electricity, and water consumed by terrestrial data centers, but they face significant engineering and economic barriers including power generation and thermal management in orbit.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/technologies/rubin/">Infrastructure for Scalable AI Reasoning | NVIDIA Vera Rubin Platform</a></li>
<li><a href="https://en.wikipedia.org/wiki/Space-based_data_center">Space-based data center - Wikipedia</a></li>
<li><a href="https://www.gao.gov/products/gao-26-109012">Science & Tech Spotlight: Data Centers in Space | U.S. GAO</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#Nvidia`, `#Vera Rubin`, `#AI Infrastructure`, `#Space Computing`

---

<a id="item-11"></a>
## [NVIDIA Benchmarks Vera Rubin NVL72: 30x Throughput Gain on DeepSeek Agents](https://blogs.nvidia.com/blog/vera-rubin-nvl72-efficiency-ai-agents/) ⭐️ 8.0/10

NVIDIA published its first on-chip benchmark results for the Vera Rubin NVL72, reporting up to 30x higher throughput per megawatt and up to 35x lower cost per million tokens versus the GB300 when running DeepSeek-V4-Pro on agentic coding tasks. The company also announced that Groq 3 LPX is now in full production, hitting 3,400 tokens per second on Gemma 4 31B, and introduced a Vera CPU for agentic workloads. This milestone is significant because agentic AI demands extremely low latency and high throughput for multi-step reasoning and tool use. The dramatic performance-per-watt and cost improvements could reshape datacenter economics and accelerate enterprise adoption of AI agents, affecting NVIDIA, cloud providers, and end users alike. Vera Rubin NVL72 unifies 72 Rubin GPUs and 36 Vera CPUs in a single liquid-cooled rack via sixth-generation NVLink, whereas the GB300 NVL72 is built on Blackwell Ultra with 72 GPUs and 36 Grace CPUs. The Groq 3 LPX accelerator is co-designed with the Vera Rubin platform for low-latency inference, and SpaceXAI has announced plans to deploy Vera CPUs and send an optimized rack to space by 2028.

telegram · zaihuapd · Aug 25, 14:48

**Background**: Rack-scale AI systems package hundreds of GPUs and CPUs in a single liquid-cooled enclosure connected by a high-speed fabric to form a shared-memory pool. NVIDIA's GB300 NVL72, based on Blackwell Ultra, pairs 72 GPUs with 36 Grace CPUs; the new Vera Rubin NVL72 replaces these with 72 Rubin GPUs and 36 Vera CPUs over NVLink 6. Agentic AI refers to models that autonomously plan and execute multi-step tasks, which demands very fast token generation and lower per-token costs — exactly the focus of this benchmark.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/vera-rubin-nvl72/">Rack-Scale Agentic AI Supercomputer | NVIDIA Vera Rubin NVL72</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/gb300-nvl72/">Designed for AI Reasoning Performance & Efficiency | NVIDIA GB300 NVL72</a></li>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-groq-3-lpx-now-in-full-production-with-world-class-speed-for-agentic-ai">NVIDIA Groq 3 LPX Now in Full Production With World-Class ...</a></li>

</ul>
</details>

**Tags**: `#NVIDIA`, `#Vera Rubin`, `#DeepSeek`, `#AI Hardware`, `#Datacenter`

---

<a id="item-12"></a>
## [Microsoft Paint, Photos Embed Invisible Remote-Review Watermarks in Local AI Images](https://xusheng.dev/posts/reversing/mspaint_invisible_watermark/main/) ⭐️ 8.0/10

Research reveals Microsoft Paint and Photos embed a 16-byte GUID returned by a remote prompt-review service as an invisible watermark in locally generated images; Paint treats generation as a failure if the watermark cannot be written. Even on Copilot+ PCs with local NPUs, prompt review and provenance signing still require network connectivity. This challenges assumptions that Microsoft's AI image generation on Copilot+ PCs is fully local and private, because every generated image carries a remote-review identifier. It raises privacy and censorship concerns, and shows how content provenance (C2PA) can be linked to user prompts through invisible watermarks. The watermark consists of a 16-byte GUID embedded in image pixels, and the same GUID can also be written into C2PA metadata contained in the file. This means provenance metadata and pixel-level watermarks are tied to the remote review result, not purely local generation.

telegram · zaihuapd · Aug 26, 00:53

**Background**: C2PA (Coalition for Content Provenance and Authenticity) is an open technical standard for establishing the origin and edits of digital content, promoted by the Content Authenticity Initiative founded by Adobe, The New York Times and Twitter. Microsoft has been integrating C2PA-based provenance metadata into its AI tools to label AI-generated media. However, this research shows that even 'local' generation on NPUs depends on a remote review service whose GUID is invisibly embedded in output images.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/C2PA">C2PA</a></li>
<li><a href="https://c2pa.org/">C2PA | Providing Origins of Media Content</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#watermarking`, `#Microsoft`, `#AI generation`, `#security`

---