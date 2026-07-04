---
layout: default
title: "Horizon Summary: 2026-07-04 (EN)"
date: 2026-07-04
lang: en
---

> From 43 items, 13 important content pieces were selected

---

1. [Anthropic Accuses Alibaba of Massive Distillation Attack on Claude](#item-1) ⭐️ 9.0/10
2. [Local SOTA LLM Guide Sparks Cost vs. Cloud Debate](#item-2) ⭐️ 8.0/10
3. [EU Parliament Member Hacked with Pegasus Spyware](#item-3) ⭐️ 8.0/10
4. [Wordgard: New Rich-Text Editor from ProseMirror Creator](#item-4) ⭐️ 8.0/10
5. [PostgreSQL and OOM Killer: Why Strict Memory Overcommit?](#item-5) ⭐️ 8.0/10
6. [Current AI Launches Open Source AI Gap Map Indexing 421 Products](#item-6) ⭐️ 8.0/10
7. [Google Gemini Omni Flash Tops Video Arena Blind Test](#item-7) ⭐️ 8.0/10
8. [Claude Fable 5 Relaunch: Developers Frustrated by Safety Overreach and Reduced Quotas](#item-8) ⭐️ 8.0/10
9. [Huawei Atlas 350 with Ascend 950PR Claims 2.87x H20 Performance](#item-9) ⭐️ 8.0/10
10. [China proposes deleting inactive accounts, mandating AI labels](#item-10) ⭐️ 8.0/10
11. [Huawei Mate 80 Pro Gaming Efficiency Beats Snapdragon 8 Gen3 via HarmonyOS](#item-11) ⭐️ 8.0/10
12. [NASA Launches Private LINK Spacecraft to Rescue Swift Telescope](#item-12) ⭐️ 8.0/10
13. [Tencent Xuanwu Lab's Atuin AI Surpasses Mythos on CyberGym](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic Accuses Alibaba of Massive Distillation Attack on Claude](https://t.me/zaihuapd/42327) ⭐️ 9.0/10

Anthropic has accused Alibaba of orchestrating a massive distillation attack, using nearly 25,000 fraudulent accounts to extract capabilities from its Claude AI model through over 28.8 million interactions between April 22 and June 5, 2026. Anthropic claims this is the largest known distillation attack against the company. This accusation highlights growing tensions over AI intellectual property and national security, as distillation attacks enable foreign entities to replicate advanced AI capabilities without authorization. If proven, it could escalate US-China tech conflicts and lead to tighter export controls on AI models. Anthropic stated that Alibaba and its Qwen lab participated in the attack, which involved systematically querying Claude to extract knowledge for training competing models. The company has sent a letter to the US Senate Banking Committee detailing the alleged breach.

telegram · zaihuapd · Jul 3, 06:21

**Background**: Model distillation is a technique where a smaller, less capable model (the student) learns from a larger, more capable model (the teacher) by training on the teacher's outputs. While legitimate when authorized, using distillation on proprietary models without permission is considered intellectual property theft. Anthropic has previously warned about such attacks undermining US export controls on AI technology.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI安全`, `#知识产权`, `#模型蒸馏`, `#Anthropic`, `#阿里巴巴`

---

<a id="item-2"></a>
## [Local SOTA LLM Guide Sparks Cost vs. Cloud Debate](https://github.com/jamesob/local-llm) ⭐️ 8.0/10

Jamesob published a guide on building a high-end local LLM setup for roughly $40,000, using four GPUs and a pruned, quantized version of GLM-5.2, while community comments reveal that such setups remain far more expensive and lower quality than cloud subscriptions. This discussion underscores the impracticality of local SOTA LLMs for most users, as cloud services offer comparable intelligence at a fraction of the hardware cost, shifting the focus toward hybrid or mid-range local solutions. The proposed build costs $50,000–55,000 instead of the stated $40,000, and relies on a REAP-pruned (≈22% experts removed) Int8-mix NVFP4 quantized GLM-5.2 model with about 594B parameters; community members suggest cheaper alternatives like 2× RTX 3090s for $3,000 total.

hackernews · livestyle · Jul 3, 15:03 · [Discussion](https://news.ycombinator.com/item?id=48775921)

**Background**: Running state-of-the-art large language models locally requires massive VRAM and compute power, often necessitating multi-GPU setups and model compression techniques like pruning and quantization. Cloud services such as Claude Opus and GPT-4 offer easy access to similar capabilities for a monthly fee, making local deployment economically challenging for individuals.

**Discussion**: Community sentiment is mixed: many commenters highlight the exorbitant cost, noting that $40,000 equals over 16 years of Claude Opus subscription, while others propose intermediate options like 128GB unified memory systems running DeepSeek V4. However, concerns remain about quantization quality and model safety in local setups.

**Tags**: `#LLM`, `#local inference`, `#hardware`, `#deep learning`, `#community discussion`

---

<a id="item-3"></a>
## [EU Parliament Member Hacked with Pegasus Spyware](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

Citizen Lab has confirmed that Stelios Kouloglou, a member of the European Parliament's committee investigating spyware, was successfully infected with NSO Group's Pegasus spyware on multiple occasions in 2022 and 2023. This breach demonstrates that state-sponsored espionage targets EU parliamentary oversight bodies, undermining democratic institutions and the security of elected representatives. The infections occurred on October 21, 2022, and March 6-7, 2023, with the first infection overlapping a known Pegasus campaign targeting Russian and Belarusian exiled journalists in Europe.

hackernews · ledoge · Jul 3, 20:38 · [Discussion](https://news.ycombinator.com/item?id=48779683)

**Background**: Pegasus is a powerful spyware developed by Israeli firm NSO Group, capable of remotely compromising mobile devices to access messages, calls, and cameras. It has been widely used by governments to surveil journalists, activists, and politicians. Citizen Lab, based at the University of Toronto, specializes in detecting and analyzing such threats.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>

</ul>
</details>

**Discussion**: Commenters noted the irony of an EU parliament member investigating spyware being hacked, and discussed broader abuse of Pegasus by EU member states like Greece and Italy. Some pointed out the lack of separation between personal and work devices in parliament.

**Tags**: `#cybersecurity`, `#spyware`, `#Pegasus`, `#European Parliament`, `#espionage`

---

<a id="item-4"></a>
## [Wordgard: New Rich-Text Editor from ProseMirror Creator](https://wordgard.net/) ⭐️ 8.0/10

Marijn Haverbeke, the creator of ProseMirror, has released Wordgard, a new in-browser rich-text editor framework that aims to improve developer experience and address design differences from its predecessor. Wordgard represents a significant evolution in the rich-text editor ecosystem, offering a more developer-friendly API and potentially influencing the next generation of web-based editors like Tiptap or Obsidian. Wordgard is not a free-form HTML editor but a structured content editor where developers control supported content types, and there is no direct upgrade path from ProseMirror, requiring substantial migration effort.

hackernews · indy · Jul 3, 08:50 · [Discussion](https://news.ycombinator.com/item?id=48772573)

**Background**: ProseMirror is a battle-tested core foundation for many rich-text editors, including Tiptap, known for its performance and flexibility but also for its steep learning curve. Wordgard is a new framework from the same author that aims to provide a more intuitive API and better developer experience while maintaining the core concepts of structured document editing.

<details><summary>References</summary>
<ul>
<li><a href="https://wordgard.net/">Wordgard</a></li>
<li><a href="https://prosemirror.net/">ProseMirror</a></li>

</ul>
</details>

**Discussion**: The community is generally impressed with Wordgard's design and documentation, but there are concerns about the lack of an upgrade path from ProseMirror and the need for statically-typed document representations. Some users also expressed frustration that a web standard for rich-text editing has not been established.

**Tags**: `#rich-text editor`, `#web development`, `#prosemirror`, `#javascript`, `#wordgard`

---

<a id="item-5"></a>
## [PostgreSQL and OOM Killer: Why Strict Memory Overcommit?](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud explains why it uses vm.overcommit_memory=2 (strict overcommit) for PostgreSQL to prevent OOM killer issues, based on their experience running PostgreSQL at scale. This setting can significantly improve stability for database workloads by preventing the OOM killer from killing PostgreSQL processes, but it requires careful testing as it can cause application crashes if not configured properly. The article describes three overcommit modes: 0 (heuristic), 1 (always overcommit), and 2 (strict no overcommit). Mode 2 ensures memory allocation fails immediately when memory is exhausted, which is safer for PostgreSQL but can break applications that rely on overcommit.

hackernews · furkansahin · Jul 3, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48774509)

**Background**: The Linux kernel's OOM (Out-Of-Memory) killer is a mechanism that kills processes when the system runs out of memory. Memory overcommit allows allocating more virtual memory than physical RAM, which can lead to OOM situations. PostgreSQL, as a database, benefits from strict mode to avoid unexpected kills.

<details><summary>References</summary>
<ul>
<li><a href="https://rakeshjain-devops.medium.com/linux-out-of-memory-killer-31e477a45759">Linux Out-Of-Memory Killer . What is this ? | by Rakesh Jain | Medium</a></li>
<li><a href="https://www.linkedin.com/pulse/vmovercommitmemory-sanju-debnath">vm.overcommit_memory</a></li>
<li><a href="https://ssup2.github.io/blog-software/en/docs/theory-analysis/linux-oom-killer/">Linux OOM Killer – ssup2 Blog / Software</a></li>

</ul>
</details>

**Discussion**: The community discussion includes cautions from users about potential side effects of strict overcommit, such as preventing forks. The author acknowledges the article's tone may be too strong and notes that strict overcommit may not be suitable for all scenarios.

**Tags**: `#PostgreSQL`, `#memory management`, `#OOM killer`, `#Linux`, `#database administration`

---

<a id="item-6"></a>
## [Current AI Launches Open Source AI Gap Map Indexing 421 Products](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

The non-profit Current AI released v0.1 of its Open Source AI Gap Map, a detailed catalog of 421 open-source AI products—including 266 software tools, 85 models, 50 datasets, and 20 hardware projects—from 228 organizations, with underlying data released under an MIT license on GitHub. This map provides a comprehensive, structured overview of the open-source AI ecosystem, helping researchers, developers, and funders identify gaps and opportunities. Backed by $400 million in committed capital, it could accelerate the adoption of open-source AI and inform strategic investments. The map is organized into 14 categories across three stack layers: model components, product/UX, and infrastructure. An additional 24,400 artifacts are in an uncategorized long tail, unscored until researched and cited.

rss · Simon Willison · Jul 3, 22:04

**Background**: Current AI is a global non-profit partnership founded at the AI Action Summit in Paris in February 2025. The Gap Map aims to systematically index the open-source AI landscape, which previously lacked a unified catalog. The data is available as 1,184 YAML files on GitHub, enabling exploration via tools like Datasette Lite.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/jul/3/open-source-ai-gap-map/">Open Source AI Gap Map | Simon Willison’s Weblog</a></li>
<li><a href="https://blog.jarv.tech/p/open-source-ai-gap-map-masshtabnaya-karta-ekosistemy-beea18396340c774">Open Source AI Gap Map : масштабная карта... — blog.jarv.tech</a></li>

</ul>
</details>

**Tags**: `#open source`, `#AI`, `#ecosystem mapping`, `#nonprofit`, `#tools`

---

<a id="item-7"></a>
## [Google Gemini Omni Flash Tops Video Arena Blind Test](https://x.com/Designarena/status/2072759122366509130) ⭐️ 8.0/10

Google DeepMind's Gemini Omni Flash video generation model has achieved the top spot on the Video Arena blind test ranking with a score of 1404 points, surpassing ByteDance's Seedance 2.0 Mini by 101 points. This marks a significant breakthrough in AI video generation, demonstrating Google's ability to regain leadership in a competitive space dominated by ByteDance's Seedance series. The result underscores the rapid pace of innovation in multimodal AI models. Gemini Omni Flash is a transformer-based multimodal model supporting text, vision, video, and audio inputs, currently capped at 10 seconds of video output. Google's video model ranking improved by 7 positions from the previous Veo series, based on blind user voting.

telegram · zaihuapd · Jul 3, 05:51

**Background**: Video Arena is a crowd-sourced blind test benchmark where users compare AI-generated videos without knowing which model produced them, providing an unbiased quality assessment. The gemini Omni Flash model was introduced by Google in May 2026 as part of the Gemini Omni family, focusing on real-world physics and conversational video editing. ByteDance's Seedance 2.0 Mini had previously held the top position with 1303 points.

<details><summary>References</summary>
<ul>
<li><a href="https://www.madebyagents.com/benchmarks/video-arena">Video Arena Benchmark : Scores, Methodology, and Top AI Models</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-omni-flash/">Gemini Omni Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-omni/">Introducing Gemini Omni</a></li>

</ul>
</details>

**Tags**: `#AI`, `#video generation`, `#Google DeepMind`, `#model benchmarking`, `#computer vision`

---

<a id="item-8"></a>
## [Claude Fable 5 Relaunch: Developers Frustrated by Safety Overreach and Reduced Quotas](https://www.bleepingcomputer.com/news/artificial-intelligence/claude-fable-relaunch-disappoints-users-with-nerfed-performance/) ⭐️ 8.0/10

Anthropic's Claude Fable 5 model has been relaunched after US export controls were lifted, but subscribers now face a 50% usage quota until July 7, after which the model will no longer be included in subscription plans. Additionally, excessive safety filters cause frequent false positives, automatically downgrading the model to Opus 4.8 when processing C/C++ or Rust code containing keywords like 'vulnerability' or 'hook'. This incident highlights the growing tension between AI safety mechanisms and practical usability for developers, potentially undermining trust in Anthropic's deployment practices. If not addressed, it could drive developers toward competing models with more predictable behavior, impacting Anthropic's adoption in the developer community. According to official statements, the usage restrictions are due to insufficient computing capacity, and the model will be reintegrated into subscription plans when capacity is adequate. The API and enterprise pay-per-use versions still provide full access to Fable 5 without downgrade, but no optimization for safety false positives has been announced.

telegram · zaihuapd · Jul 3, 07:20

**Background**: Claude Fable 5 is Anthropic's flagship 'Mythos-class' model, designed for complex coding and knowledge work tasks. It was initially launched but then restricted due to US export controls on advanced AI models to certain countries. After the controls were lifted, the model became available again. Safety filters in LLMs are intended to prevent harmful outputs, but excessive thresholds can interfere with legitimate development work, as seen here with false triggers on security-related keywords.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-8">Introducing Claude Opus 4.8 \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#Claude`, `#Anthropic`, `#model deployment`, `#developer experience`

---

<a id="item-9"></a>
## [Huawei Atlas 350 with Ascend 950PR Claims 2.87x H20 Performance](https://t.me/zaihuapd/42329) ⭐️ 8.0/10

At the 2026 Huawei China Partner Conference, Huawei announced and started sales of the Atlas 350 accelerator card featuring the new Ascend 950PR processor, which supports FP4 low-precision inference and claims 2.87 times the single-card computing power of Nvidia's H20. This launch marks Huawei's most aggressive challenge yet to Nvidia's dominance in the Chinese AI chip market, especially amid US export restrictions. The FP4 support and high memory capacity could enable more efficient inference of large language models locally. The Ascend 950PR delivers 1.56 petaflops of FP4 performance and the Atlas 350 has 112 GB of HBM memory, allowing single-card loading of a 70B parameter model. Huawei plans to ship 750,000 of these chips in 2026.

telegram · zaihuapd · Jul 3, 08:35

**Background**: The Ascend 950PR is Huawei's latest AI inference chip, designed to compete with Nvidia's offerings under US export controls that restrict advanced Nvidia GPUs to China. FP4 (4-bit floating point) is a low-precision format that reduces memory and compute requirements for AI models, and Nvidia's Blackwell architecture also supports a similar FP4 format called NVFP4.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huaweicentral.com/ascend-950pr-ai-chip-everything-you-need-to-know/">Ascend 950PR AI Chip: Everything you need to know - Huawei Central</a></li>
<li><a href="https://tech-insider.org/huawei-ascend-950pr-ai-chip-nvidia-china-2026/">Huawei Ascend 950PR: The 1.56 PFLOP AI Chip vs Nvidia [2026]</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#Huawei`, `#Ascend`, `#accelerator`, `#FP4`

---

<a id="item-10"></a>
## [China proposes deleting inactive accounts, mandating AI labels](https://mp.weixin.qq.com/s/TfYZaC8ULPvu9JeTqYGkKg) ⭐️ 8.0/10

On July 3, 2025, China's Cyberspace Administration released a revised draft of the Internet Information Service Management Measures for public comment, proposing that platforms may delete accounts inactive for over 6 months and must label AI-generated content. This regulation would significantly impact user data management and platform compliance in China, addressing privacy protection against idle accounts and transparency for AI-generated content, affecting billions of users and major tech companies. The draft also requires platforms to allow users to unbind old phone numbers, prohibits fake engagement practices like manipulating trending topics, and mandates large platforms to handle illegal content complaints within 24 hours.

telegram · zaihuapd · Jul 3, 11:29

**Background**: China has been tightening internet governance with laws on data security and personal information protection. This draft updates the 2011 Internet Information Service Management Measures to address new challenges like AI-generated content and account security, aligning with global trends on synthetic media labeling.

<details><summary>References</summary>
<ul>
<li><a href="https://www.auditsocials.com/blog/cross-platform-ai-content-labeling-requirements-2026-meta-google-tiktok-youtube-comparison">AI Content Label Rules 2026: Meta, Google, TikTok, YouTube</a></li>

</ul>
</details>

**Tags**: `#Regulations`, `#Internet Policy`, `#AI Governance`, `#User Privacy`, `#Content Moderation`

---

<a id="item-11"></a>
## [Huawei Mate 80 Pro Gaming Efficiency Beats Snapdragon 8 Gen3 via HarmonyOS](https://www.bilibili.com/video/BV1F7T46wEyT) ⭐️ 8.0/10

Geekerwan's review reveals that the Huawei Mate 80 Pro Max, powered by the Kirin 9030 chipset, achieves superior gaming power efficiency compared to the Snapdragon 8 Gen3, thanks to native HarmonyOS optimizations and software-hardware-chip-cloud synergy. This demonstrates that deep OS-level optimization can overcome hardware disadvantages, potentially reshaping mobile performance benchmarks and challenging the dominance of conventional chipset leaders. The Kirin 9030 Pro features a 9-core, 14-thread CPU and a 6-core Maliang 935 GPU with ~15 billion transistors; while its theoretical multi-core efficiency lies between Snapdragon 8 Gen2 and 8 Gen3, real-world gaming power consumption is lower—only 4.9W for Genshin Impact at 60fps high quality.

telegram · zaihuapd · Jul 3, 13:27

**Background**: The Kirin 9030 series is Huawei's latest in-house chipset, announced in November 2025 and built on a 5nm process. HarmonyOS native applications are designed to leverage software-hardware-chip-cloud synergy, allowing for more efficient task scheduling and power management. This approach helps Huawei close the performance gap despite using less advanced hardware on paper.

<details><summary>References</summary>
<ul>
<li><a href="https://nanoreview.net/ru/soc/hisilicon-kirin-9030">HiSilicon Kirin 9030 Pro : характеристики, тесты в бенчмарках</a></li>
<li><a href="https://post.smzdm.com/p/aognpnz7/">鸿 蒙 原 生 APP...</a></li>
<li><a href="https://www.21jingji.com/article/20250904/herald/e1eec22c1785149ffafb68b13267b5f3.html">华为三折叠携麒麟9020亮相，折叠屏市场竞争迈向 软 硬 协 同 阶段 - 21...</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#Kirin 9030`, `#HarmonyOS`, `#mobile performance`, `#chipset`

---

<a id="item-12"></a>
## [NASA Launches Private LINK Spacecraft to Rescue Swift Telescope](https://apnews.com/article/swift-nasa-satellite-rescue-katalyst-a7ddd740ca099587c58865f583c7245a) ⭐️ 8.0/10

On July 3, 2026, NASA launched the LINK spacecraft built by Katalyst Space Technologies to boost the orbit of the aging Swift Observatory, preventing its imminent reentry. This mission marks the first attempt by a private spacecraft to capture and service a U.S. government satellite, potentially extending the life of a valuable 20-year-old scientific observatory and demonstrating commercial satellite servicing capabilities. The LINK spacecraft will use a robotic arm to grapple Swift and then fire its thrusters to raise the telescope's orbit by approximately 240 kilometers, with Swift potentially resuming science operations by September 2026 if successful.

telegram · zaihuapd · Jul 3, 15:43

**Background**: The Swift Observatory, launched in 2004, is a gamma-ray burst hunter that has been crucial for astrophysics. Its orbit has been decaying due to solar activity, threatening a destructive reentry. Satellite servicing is a nascent industry, and this mission could pave the way for future commercial servicing of government assets.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LINK_spacecraft">LINK spacecraft</a></li>
<li><a href="https://www.nasa.gov/image-article/link-spacecraft-set-for-mission-to-boost-nasas-swift-observatory/">LINK Spacecraft Set for Mission to Boost NASA’s Swift Observatory - NASA</a></li>

</ul>
</details>

**Tags**: `#space`, `#satellite servicing`, `#NASA`, `#astronomy`, `#orbital mechanics`

---

<a id="item-13"></a>
## [Tencent Xuanwu Lab's Atuin AI Surpasses Mythos on CyberGym](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 8.0/10

Tencent Xuanwu Lab's Atuin AI achieved 84.0% accuracy on the UC Berkeley CyberGym benchmark, surpassing Anthropic's Claude Mythos Preview. This demonstrates that an open-source model can outperform a leading closed-source system at less than 0.1% of the cost, highlighting the potential for cost-effective AI-driven vulnerability detection. Atuin AI is built on the open-source GLM-5.1 model, which can be deployed locally, and its budget was under 0.1% of Mythos's. It discovered multiple high-severity vulnerabilities missed by Mythos in projects like curl, gnark, OpenSSL, Python cryptography, and Java bc-java, with scores up to 9.3.

telegram · zaihuapd · Jul 3, 16:12

**Background**: CyberGym is a cybersecurity benchmark from UC Berkeley that evaluates AI agents on discovering and exploiting real-world software vulnerabilities. GLM-5.1 is Z.AI's flagship model designed for long-horizon autonomous tasks, capable of continuous work for up to 8 hours.

<details><summary>References</summary>
<ul>
<li><a href="https://llm-stats.com/benchmarks/cybergym">CyberGym Benchmark Leaderboard | LLM Stats</a></li>
<li><a href="https://mcpbr.org/cybergym">CyberGym : Cybersecurity Exploit Generation Benchmark for... | mcpbr</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.1">GLM - 5 . 1 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cybersecurity`, `#benchmark`, `#vulnerability detection`, `#open-source`

---