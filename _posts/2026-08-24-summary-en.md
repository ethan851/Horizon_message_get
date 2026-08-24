---
layout: default
title: "Horizon Summary: 2026-08-24 (EN)"
date: 2026-08-24
lang: en
---

> From 26 items, 5 important content pieces were selected

---

1. [1998 Essay 'How Complex Systems Fail' Still Shapes Reliability Thinking](#item-1) ⭐️ 9.0/10
2. [Owning Every Device: Reverse Engineering and WebUSB Attack Surface](#item-2) ⭐️ 8.0/10
3. [170,000 Nonprofits Lost All Data in Microsoft Cloud Incident](#item-3) ⭐️ 8.0/10
4. [Nvidia to Spend $6B on Poolside License to Build US Open-Source AI Rival](#item-4) ⭐️ 8.0/10
5. [Alibaba Plans HK$80B Share Placement to Fund AI Push](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [1998 Essay 'How Complex Systems Fail' Still Shapes Reliability Thinking](https://how.complexsystems.fail/) ⭐️ 9.0/10

The 1998 essay 'How Complex Systems Fail' by Richard Cook is being widely discussed on Hacker News, renewing attention to its core arguments. The discussion highlights how its critique of root cause analysis remains relevant to modern reliability engineering. This essay is foundational for incident analysis and reliability engineering, arguing that complex systems fail in ways that defy simple root cause attribution. Its ideas continue to influence how engineers approach failure, safety, and system design. The essay presents principles such as 'complex systems run as broken systems' and 'catastrophe requires multiple failures, not single-point failures.' It also argues that root cause analysis in complex systems is often misguided, a point that Hacker News commenters both endorse and dispute.

hackernews · shortcrct · Aug 23, 15:13 · [Discussion](https://news.ycombinator.com/item?id=49409473)

**Background**: The essay draws on normal accident theory, introduced by sociologist Charles Perrow, which argues that failures are inevitable in complex, tightly coupled systems. In reliability engineering, this perspective challenges traditional root cause analysis, which assumes a single cause can be identified and fixed. The Hacker News discussion connects the essay to practices like chaos engineering, where failures are deliberately introduced to build resilience.

<details><summary>References</summary>
<ul>
<li><a href="https://how.complexsystems.fail/">How Complex Systems Fail</a></li>
<li><a href="https://news.ycombinator.com/item?id=25550685">How Complex Systems Fail (1998) | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Normal_Accidents">Normal Accidents - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters largely praise the essay; tptacek calls it essential and says its critique of root cause analysis is hard to appreciate until you've seen complex systems fail. However, elisbce disagrees with the claim that catastrophe requires multiple failures, citing real-world single points of failure that only avoid disaster due to low failure rates. jedberg notes the essay inspired chaos engineering, which forces failure to prepare systems for it.

**Tags**: `#complex systems`, `#reliability engineering`, `#incident analysis`, `#software engineering`, `#root cause`

---

<a id="item-2"></a>
## [Owning Every Device: Reverse Engineering and WebUSB Attack Surface](https://schlarp.com/posts/everything-i-own-owned/) ⭐️ 8.0/10

The author documents a personal project to reverse engineer and take ownership of every device they own, starting by patching firmware on an ASUS ROG Swift PG42UQ monitor to remove its pixel-cleaning pop-up. The post stresses that WebUSB, WebHID, and WebBluetooth now let a single careless permission-prompt click permanently backdoor an attached device. This matters because it highlights a growing tension: firmware patching makes consumer hardware genuinely user-owned, while web APIs like WebUSB expand the attack surface for malicious sites. For security researchers and everyday users, understanding both sides is essential to protecting attached devices. The author admits the monitor is expensive and that they haven't yet flashed a modified firmware, and a commenter describes bricking a router while trying to add a TFTP boot path to the boot partition. The post concludes that a device is not truly 'owned' until working patches are written to it, and that risk of bricking remains a key barrier.

hackernews · schlarpc · Aug 23, 22:41 · [Discussion](https://news.ycombinator.com/item?id=49413320)

**Background**: WebUSB is a set of browser APIs that allow web pages to communicate with non-standard USB devices, while WebHID exposes human-interface devices like keyboards and gamepads to web applications. These APIs require a user permission prompt, after which a website can send arbitrary commands to the device, creating a security risk. 'Owning' a device in the hardware-hacking sense means running modified firmware on it, which usually involves disassembling, patching branches, and flashing new images — a process where mistakes can brick the hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebUSB">WebUSB - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/WebUSB_API">WebUSB API - Web APIs | MDN</a></li>
<li><a href="https://wicg.github.io/webhid/">WebHID API</a></li>

</ul>
</details>

**Discussion**: Commenters shared practical experiences and opinions: one started with the ASUS PG42UQ monitor's pixel-cleaning overlay, another admitted bricking a router while patching and asked for better glitching tools and safe iterative patching methods. teddyh quoted the key WebUSB/WebHID/WebBluetooth takeaway, philips reported an LLM agent reverse-engineering the Supernote file format in hours, and compiler-devel praised LLMs for enabling software and hardware freedoms the open source movement only dreamed of.

**Tags**: `#security`, `#reverse-engineering`, `#firmware`, `#hardware`, `#webusb`

---

<a id="item-3"></a>
## [170,000 Nonprofits Lost All Data in Microsoft Cloud Incident](https://slate.com/technology/2026/08/microsoft-software-nonprofit-data-delete.html) ⭐️ 8.0/10

According to an August 2026 Slate report, more than 170,000 nonprofit organizations lost all of their data due to Microsoft software, sparking debate over cloud reliability. The incident has raised questions about corporate accountability and the safety of relying on cloud services. Nonprofits rely heavily on Microsoft cloud services to store donor records, financial data, and operational files, so losing everything can be devastating. The incident also raises broader concerns about vendor responsibility, data-retention policies, and the need for independent backups across the nonprofit sector. The exact cause of the data loss remains unclear; one commenter pointed to Microsoft's documentation stating that data should not be deleted for 90 days after license expiration, suggesting a possible policy or technical failure. The case also highlights that cloud storage and SSDs are not inherently reliable for long-term archiving.

hackernews · tchalla · Aug 23, 18:55 · [Discussion](https://news.ycombinator.com/item?id=49411395)

**Background**: Microsoft 365 is widely used by nonprofits, often through donated or discounted licenses. When a subscription ends, Microsoft's retention policies are supposed to preserve data for a period, but systemic failures or confusing policy enforcement can still lead to permanent loss. Cloud services are not a substitute for backups, so organizations should keep independent copies of critical data.

**Discussion**: Commenters were broadly critical: one called Microsoft "not a serious company" and blamed industry-wide unseriousness, while another asked how deletion happened given Microsoft's stated 90-day retention period. Others shared personal experiences and warned that cloud storage and SSDs are not reliable for long-term archiving.

**Tags**: `#Microsoft`, `#Data Loss`, `#Cloud Computing`, `#Nonprofits`, `#Reliability`

---

<a id="item-4"></a>
## [Nvidia to Spend $6B on Poolside License to Build US Open-Source AI Rival](https://www.wsj.com/tech/ai/nvidia-is-spending-6-billion-to-build-a-powerful-u-s-alternative-to-chinese-ai-c51c38cc) ⭐️ 8.0/10

Nvidia invested $1 billion in AI startup Poolside at a $12 billion pre-money valuation and agreed to pay $6 billion to license Poolside's technology and absorb most of its engineers. The engineers will join Nvidia's open-weight Nemotron project, which aims to produce one of the world's strongest open-weight models to compete with Chinese models like DeepSeek and Kimi K3. This deal marks Nvidia's largest move yet into open-weight AI models, intensifying the race against both Chinese open-source labs and US closed-source leaders like OpenAI and Anthropic. It could accelerate the availability of high-performance open models and reshape competitive dynamics in the AI industry. Under the agreement, Poolside's pre-money valuation is $12 billion, and Nvidia's $6 billion license fee does not count toward that valuation. Most of Poolside's more than 100 engineers will move to Nvidia to work on Nemotron, Nvidia's family of open-weight models designed for reasoning, coding, and agentic AI.

telegram · zaihuapd · Aug 23, 04:20

**Background**: Open-weight models release the trained neural network parameters so others can run, fine-tune, and build upon them, though the full training data and code may not be disclosed. Nvidia's Nemotron family includes open models such as Nemotron 3.5 Lightning, a 30B-parameter MoE model with 3B active parameters. Poolside is a US startup focused on large language models for software development. The deal is part of Nvidia's broader push to embed its chips and software in the AI stack while countering the rise of competitive open-source models from China.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/NVIDIA_Nemotron">NVIDIA Nemotron</a></li>
<li><a href="https://money.udn.com/money/story/123398/9708183">輝達斥資60億美元 取得 Poolside 模型授權 壯大 AI ... | 經濟日報</a></li>
<li><a href="https://www.ofweek.com/ai/2025-02/ART-201700-8420-30657041.html">3分钟看懂大 模 型 开 闭 源 战争，谁将主宰未来？ - OFweek 人工智能网</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#AI`, `#open-source`, `#Poolside`, `#investment`

---

<a id="item-5"></a>
## [Alibaba Plans HK$80B Share Placement to Fund AI Push](https://www.jwview.com/jingwei/html/m/08-23/684731.shtml) ⭐️ 8.0/10

Alibaba announced on August 23 a plan to place new shares to non-U.S. investors outside the United States, raising a total of HK$80 billion (800亿港元) — its first new-share placement since its 2019 Hong Kong listing. The net proceeds will be 100% invested in full-stack AI capabilities and AI infrastructure. This marks one of the largest AI-dedicated capital raises by a Chinese technology company and signals Alibaba's aggressive expansion of AI infrastructure to compete with global cloud and AI leaders. It also highlights the intensifying AI capex race among hyperscalers, with implications for AI chip demand, cloud pricing, and the broader AI ecosystem. The placement is aimed at non-U.S. persons residing outside the United States and is Alibaba's first share placement since its 2019 Hong Kong IPO. The company said the net proceeds will be used entirely for full-stack AI capabilities, which typically span underlying compute (chips, servers, data centers), models, and applications.

telegram · zaihuapd · Aug 23, 08:19

**Background**: "Full-stack AI" refers to an enterprise's ability to manage the entire AI technology stack, from underlying compute (self-developed chips, servers, and data centers) to models and applications. Alibaba's pledge to invest all proceeds in full-stack AI capabilities and AI infrastructure implies spending on compute capacity, data centers, model R&D, and potentially in-house silicon. AI infrastructure generally includes AI chips, GPU clusters, and data center networks, which form the physical foundation for large-scale model training and inference.

<details><summary>References</summary>
<ul>
<li><a href="https://www.qbitai.com/2024/02/119135.html">全栈智能才能兑现AI红利？</a></li>
<li><a href="https://m.c114.com.cn/w5339-1301043.html">全栈式AI:巨头的“战略逻辑”及未来生态博弈 - C114通信网</a></li>

</ul>
</details>

**Tags**: `#Alibaba`, `#AI infrastructure`, `#investment`, `#fundraising`

---