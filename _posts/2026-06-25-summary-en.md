---
layout: default
title: "Horizon Summary: 2026-06-25 (EN)"
date: 2026-06-25
lang: en
---

> From 29 items, 9 important content pieces were selected

---

1. [OpenAI unveils first custom inference chip Jalapeño with Broadcom](#item-1) ⭐️ 9.0/10
2. [Qualcomm Acquires AI Startup Modular for $4B](#item-2) ⭐️ 9.0/10
3. [Anthropic accuses Alibaba of massive distillation attack on Claude](#item-3) ⭐️ 9.0/10
4. [NVIDIA's 45°C Liquid Cooling Slashes Data Center Water Use](#item-4) ⭐️ 8.0/10
5. [Nub: Bring Bun-like DX to Node.js](#item-5) ⭐️ 8.0/10
6. [Generative AI Use Linked to Lower Exam Scores in Chinese Students](#item-6) ⭐️ 8.0/10
7. [TSMC to raise advanced process prices by 5-10%](#item-7) ⭐️ 8.0/10
8. [Micron Q3 FY2026 Revenue Surges 346% YoY, Net Profit $28.24B](#item-8) ⭐️ 8.0/10
9. [Google Play Enables External Billing in US, UK, EU from June 30](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI unveils first custom inference chip Jalapeño with Broadcom](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI announced its first custom inference chip, named Jalapeño, developed in partnership with Broadcom and manufactured by TSMC, with development accelerated by OpenAI's own AI models. This marks a major strategic shift for OpenAI, reducing reliance on NVIDIA GPUs and enabling cost-optimized inference at scale, potentially reshaping the AI hardware landscape. The chip is an inference-only ASIC designed specifically for running trained AI models, and OpenAI claims its models helped accelerate the design process from concept to production in nine months.

hackernews · jamdesk · Jun 24, 17:47 · [Discussion](https://news.ycombinator.com/item?id=48663324)

**Background**: An inference chip is a specialized processor optimized to execute AI models after training, focusing on low latency and high throughput. OpenAI, like many AI companies, has historically relied on NVIDIA GPUs for both training and inference, but custom chips like Google's TPU have shown significant efficiency gains. Broadcom is a leading designer of custom AI ASICs for major tech companies.

<details><summary>References</summary>
<ul>
<li><a href="https://naddod.medium.com/inference-chip-guide-the-foundation-of-scalable-ai-applications-d18f2c22b36c">Inference Chip Guide: The Foundation of Scalable AI Applications | by NADDOD | Medium</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/custom-ai-asics-examined-from-broadcom-to-mtia">The custom AI ASIC state of play (May 2026) — Broadcom deals ...</a></li>
<li><a href="https://tech-insider.org/broadcom-ai-revenue-custom-chips-2026/">Broadcom AI Revenue Surges 106%: Custom Chip Strategy 2026</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about the claim that AI accelerated the chip design, calling it potentially vague marketing. There was also technical discussion about alternative approaches like burning weights into silicon for extreme throughput, as well as comparisons to Google's TPU and other custom chips.

**Tags**: `#AI hardware`, `#OpenAI`, `#custom chip`, `#inference`, `#Broadcom`

---

<a id="item-2"></a>
## [Qualcomm Acquires AI Startup Modular for $4B](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 9.0/10

On June 24, 2026, Qualcomm announced the acquisition of AI startup Modular for $4 billion, marking a major push into AI compute beyond mobile chips. This acquisition signals Qualcomm's ambition to compete in the AI hardware-software stack, potentially challenging NVIDIA's dominance by integrating Modular's Mojo language and MLIR-based compiler technology into Qualcomm's portfolio. Modular is known for developing Mojo, a Python-like programming language optimized for AI workloads, and has raised $250 million prior to the acquisition. The deal is expected to close in late 2026, pending regulatory approval.

hackernews · timmyd · Jun 24, 13:49 · [Discussion](https://news.ycombinator.com/item?id=48659798)

**Background**: Mojo is a proprietary programming language that combines Python's usability with the performance of system languages like C++ and Rust, using the MLIR compiler framework to target CPUs, GPUs, and other accelerators. Modular was founded in 2022 by former Apple and Google engineers, including Chris Lattner, creator of LLVM and Swift. The acquisition aligns with Qualcomm's strategy to diversify beyond mobile chips into AI inference and edge computing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some question the strategic fit, noting Qualcomm's limited presence in high-end AI training, while others see it as a bold move toward RISC-V and AI competitiveness. Concerns also arise about Mojo's future as an open-source language under a hardware company.

**Tags**: `#Acquisition`, `#AI Infrastructure`, `#Qualcomm`, `#Mojo`, `#Hardware`

---

<a id="item-3"></a>
## [Anthropic accuses Alibaba of massive distillation attack on Claude](https://www.cnbc.com/2026/06/24/anthropic-alibaba-distillation-campaign.html) ⭐️ 9.0/10

Anthropic has formally accused Alibaba of orchestrating a massive distillation attack on its Claude AI models, using nearly 25,000 fraudulent accounts to conduct over 28.8 million interactions between April 22 and June 5, 2026, in an attempt to extract model capabilities. This is the largest known distillation attack against Anthropic, highlighting escalating tensions in US-China AI competition and raising serious concerns about intellectual property theft and national security. Anthropic sent a letter to the US Senate Banking Committee on June 10, implicating Alibaba and its Qwen AI lab. The attack occurred around the time the US restricted exports of Anthropic's Mythos and Fable models, and Alibaba was also added to the Pentagon's Chinese military company list.

telegram · zaihuapd · Jun 25, 01:36

**Background**: Model distillation is a technique where a weaker model learns from the outputs of a stronger model to replicate its capabilities at lower cost. The White House has previously accused China of stealing US AI intellectual property, and distillation attacks have been framed as a national security concern in the US-China AI rivalry.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/detecting-and-preventing-distillation-attacks">Detecting and preventing distillation attacks \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/research/mythos-preview">Assessing Claude Mythos Preview’s cybersecurity capabilities</a></li>
<li><a href="https://www.iiss.org/online-analysis/cyber-power-matrix/2026/05/ai-distillation-attacks-in-the-uschina-contest/">AI distillation attacks in the US–China contest - iiss.org</a></li>

</ul>
</details>

**Tags**: `#AI安全`, `#模型蒸馏`, `#Anthropic`, `#阿里巴巴`, `#知识产权`

---

<a id="item-4"></a>
## [NVIDIA's 45°C Liquid Cooling Slashes Data Center Water Use](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 8.0/10

NVIDIA announced a new 45°C liquid cooling architecture for its upcoming Rubin-generation AI servers that eliminates the need for water evaporation cooling, achieving near-zero water consumption while maintaining high efficiency. This design addresses the growing water footprint of AI data centers, potentially saving operators over $4 million annually per 50MW facility, and sets a new standard for sustainable AI infrastructure. The cooling system operates with coolant at 45°C, enabling zero fans and 100% liquid cooling, and is required for all cloud providers building Rubin infrastructure. Mass production is scheduled to begin in autumn 2026.

hackernews · nitin_flanker · Jun 24, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48660178)

**Background**: Data centers traditionally use air conditioning or evaporative cooling, which consume significant water and energy. Liquid cooling uses a coolant to remove heat directly from chips, and raising the coolant temperature to 45°C allows for more efficient heat rejection to the environment, reducing or eliminating the need for water-intensive cooling towers. This is part of a broader industry trend toward water-efficient designs, with Microsoft also announcing zero-water evaporation cooling.

<details><summary>References</summary>
<ul>
<li><a href="https://techstory.in/the-45c-breakthrough-nvidias-liquid-cooling-architecture-solves-data-center-water-crisis/">NVIDIA Liquid Cooling Design Cuts Water to Near Zero - TechStory</a></li>
<li><a href="https://icharles.com/articles/nvidia-rubin-45c-liquid-cooling-zero-water">NVIDIA Rubin: 45°C Cooling, Near-Zero Water - iCharles</a></li>

</ul>
</details>

**Discussion**: Comments raised questions about the novelty of the approach, noting that higher coolant temperatures have been used before, and discussed synergies like district heating. Some users expressed interest in more details on climate dependencies and shared examples of similar existing facilities.

**Tags**: `#data center cooling`, `#liquid cooling`, `#energy efficiency`, `#AI infrastructure`, `#NVIDIA`

---

<a id="item-5"></a>
## [Nub: Bring Bun-like DX to Node.js](https://github.com/nubjs/nub) ⭐️ 8.0/10

Colin McDonnell released Nub, an all-in-one toolkit for Node.js that enhances the runtime with an oxc-powered transpiler, polyfills, and module resolution hooks via a --require preload, mimicking Bun's developer experience. Nub significantly improves Node.js developer experience by offering Bun-like features without leaving Node's ecosystem, and its author's reputation (Zod creator, ex-Bun) adds credibility. It could influence how Node.js tooling evolves. Nub uses the oxc transpiler as a Node-API add-on for performance, and injects polyfills for modern APIs like Worker and Temporal. It runs on stock Node.js, making all enhancements additive.

hackernews · colinmcd · Jun 24, 14:14 · [Discussion](https://news.ycombinator.com/item?id=48660267)

**Background**: Bun is a fast all-in-one JavaScript runtime with built-in transpilation and bundling, but it is not Node.js-compatible. Nub provides similar convenience within Node.js by intercepting module loading and adding missing APIs. The oxc transpiler is a high-performance JavaScript/TypeScript toolchain written in Rust.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Temporal">Temporal - JavaScript | MDN</a></li>
<li><a href="https://repositorystats.com/topic/transpiler">Statistics for the Github transpiler topic - RepositoryStats</a></li>

</ul>
</details>

**Discussion**: Community feedback is positive: one user successfully migrated their monorepo with zero issues, praising its speed. Others discussed technical nuances like the use of --require vs --import and ESM support, with the author clarifying that Nub uses a preload hook.

**Tags**: `#nodejs`, `#developer-experience`, `#tooling`, `#typescript`, `#bun`

---

<a id="item-6"></a>
## [Generative AI Use Linked to Lower Exam Scores in Chinese Students](https://cepr.org/publications/dp21577) ⭐️ 8.0/10

A study of 26,811 Chinese grade 7–12 students over 30 months found that generative AI use improved homework scores by 18% and reduced completion time by 30%, but led to an 18–24% drop in high-stakes exam scores within two years. This is the first large-scale, long-term empirical study demonstrating that generative AI can harm real academic achievement, even as it boosts short-term homework performance. It raises critical questions about AI's impact on learning and assessment, especially in high-stakes educational systems. The negative effects were most pronounced in social sciences, followed by STEM and languages; younger students, high achievers, and males were more affected. About 80% of AI users exhibited an 'homework outsourcing' pattern—very short homework time with high scores—and these students bore the main performance losses.

telegram · zaihuapd · Jun 24, 05:15

**Background**: Generative AI tools like ChatGPT and similar models have become widely accessible to students. While they can help with homework, they may create a false sense of mastery because students rely on AI rather than developing their own understanding. This study, published by CEPR, tracked real-world academic performance over years, offering evidence that AI use in homework does not translate to better exam results.

**Tags**: `#AI`, `#education`, `#research`, `#China`, `#academic performance`

---

<a id="item-7"></a>
## [TSMC to raise advanced process prices by 5-10%](https://36kr.com/newsflashes/3866472254411779) ⭐️ 8.0/10

TSMC has notified customers of a 5-10% price increase across all advanced process nodes (7nm and below), affecting approximately 75% of its wafer revenue. This price hike will directly impact major chip designers like Apple, NVIDIA, and AMD, potentially raising costs for a wide range of electronics and accelerating industry-wide price adjustments. The price increase covers not only 3nm but also all advanced nodes including 5nm and 7nm, with an overall range of 5-10%, and applies to approximately 75% of TSMC's wafer revenue sources.

telegram · zaihuapd · Jun 24, 05:45

**Background**: TSMC is the world's largest dedicated independent semiconductor foundry, manufacturing chips for many leading companies. Advanced process nodes (7nm and below) are critical for high-performance computing and mobile devices. The chip industry has faced supply constraints and rising costs in recent years.

**Tags**: `#TSMC`, `#semiconductor`, `#manufacturing`, `#pricing`, `#chip shortage`

---

<a id="item-8"></a>
## [Micron Q3 FY2026 Revenue Surges 346% YoY, Net Profit $28.24B](https://www.globenewswire.com/news-release/2026/06/24/3317151/14450/en/micron-technology-inc-reports-record-results-for-the-third-quarter-of-fiscal-2026.html) ⭐️ 8.0/10

Micron Technology reported record fiscal Q3 2026 revenue of $414.6 billion, a 346% year-over-year increase, and net profit of $28.24 billion (approximately $3.1 billion per day), driven by surging demand from AI infrastructure for high-performance memory such as HBM4. This record performance underscores how AI is fundamentally reshaping the memory industry, with memory makers reaping massive profits while consumer markets face shortages. The results signal that the memory supply crunch, often called 'RAMmageddon', will continue to impact global supply chains and pricing for years. Micron's data center segment revenue surged 653% year-over-year to $115.2 billion, and the company has already mass-produced HBM4 memory, with HBM4E planned for 2027. Gross margin jumped to 84.9%, and Micron has signed 16 long-term strategic agreements to secure future orders.

telegram · zaihuapd · Jun 24, 22:22

**Background**: Starting in 2025, a global computer memory shortage known as 'RAMmageddon' has been driven by manufacturers reallocating production capacity from commodity DRAM to high-margin products like High Bandwidth Memory (HBM) for AI data centers. HBM is a 3D-stacked DRAM technology that provides ultra-high bandwidth and energy efficiency for AI accelerators. According to a 2026 Kearney analysis, this shortage is expected to last at least until 2030.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HBM_memory_shortage">HBM memory shortage</a></li>
<li><a href="https://semiengineering.com/hbm4e-raises-the-bar-for-ai-memory-bandwidth/">HBM4E Raises The Bar For AI Memory Bandwidth</a></li>

</ul>
</details>

**Tags**: `#Micron`, `#Memory`, `#AI`, `#Earnings`, `#Semiconductor`

---

<a id="item-9"></a>
## [Google Play Enables External Billing in US, UK, EU from June 30](https://android-developers.googleblog.com/2026/06/play-expanded-billing.html) ⭐️ 8.0/10

Google announced that starting June 30, 2026, it will allow developers in the US, UK, and European Economic Area to offer third-party in-app billing or external web links for purchases, with a new fee structure that separates service and processing fees. This marks the largest expansion of external billing on Google Play, giving developers more payment flexibility and potentially lower costs, while impacting Google's revenue model and the broader app store economy. The new structure charges a 10% service fee on the first $1M annual revenue and auto-renewing subscriptions, with an additional 5% settlement fee for transactions using Google Play Billing; alternative billing or external links incur no settlement fee. Developers enrolled in the Level Up or Apps Experience programs will receive even lower rates starting September.

telegram · zaihuapd · Jun 25, 02:33

**Background**: App stores like Google Play typically require developers to use their own billing system and pay a commission (often 15-30%). External billing has been a contentious issue globally, with regulators in the EU and elsewhere pushing for more openness. Google previously ran a small pilot for external billing in limited regions; this expansion to major markets is a significant policy shift.

<details><summary>References</summary>
<ul>
<li><a href="https://9to5google.com/2026/06/24/google-play-store-external-billing-june-30/">Google Play Store opens external billing starting June 30</a></li>
<li><a href="https://www.androidheadlines.com/2026/06/google-play-store-external-billing-fee-changes.html">Google Play Store Opens Up to External Billing Options</a></li>
<li><a href="https://support.google.com/googleplay/android-developer/answer/10281818?hl=en">Understanding Google Play’s Payments policy</a></li>

</ul>
</details>

**Tags**: `#Google Play`, `#billing`, `#app store`, `#policy`, `#developer`

---