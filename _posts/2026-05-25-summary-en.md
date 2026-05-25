---
layout: default
title: "Horizon Summary: 2026-05-25 (EN)"
date: 2026-05-25
lang: en
---

> From 24 items, 7 important content pieces were selected

---

1. [Trojanized Telegram on APKPure Has Spyware Backdoor](#item-1) ⭐️ 9.0/10
2. [Memory hits ~2/3 of AI chip component costs](#item-2) ⭐️ 8.0/10
3. [Constraint Decay: LLM Agents Struggle with Architectural Rules](#item-3) ⭐️ 8.0/10
4. [Vivado 2026.1 Removes Free Linux Support](#item-4) ⭐️ 8.0/10
5. [Armin Ronacher Criticizes AI-Generated Bug Reports](#item-5) ⭐️ 8.0/10
6. [Huawei announces 'Tao's Law' using time scaling for semiconductors](#item-6) ⭐️ 8.0/10
7. [Epic Reveals Unreal Engine 6, First Game: Rocket League](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Trojanized Telegram on APKPure Has Spyware Backdoor](https://x.com/EricParker/status/2058411298195661221) ⭐️ 9.0/10

Security researcher Eric Parker discovered that the official Telegram app (version 12.6.5) downloaded from APKPure has been repackaged with a spyware framework called DataCollector, which is embedded in classes3.dex with over 3000 lines of code. This backdoor can steal all chat history, contacts, photos, documents, GPS location, and SIM card information, compromising user privacy severely. Users who downloaded Telegram from APKPure are at high risk of data theft. The stolen data is encrypted using AES-GCM and exfiltrated to command-and-control server at IP 38.190.225.166. The malicious injection specifically targets the official Telegram build, not the original app from Telegram's own website.

telegram · zaihuapd · May 24, 11:38

**Background**: APKPure is a third-party Android app store that allows users to download APK files directly, bypassing Google Play. Unlike official app stores, third-party platforms lack rigorous security checks, making them a common vector for distributing repackaged malware. In this case, the attacker took the legitimate Telegram APK, decompiled it, added malicious code in a new dex file, re-signed it, and distributed it through APKPure.

<details><summary>References</summary>
<ul>
<li><a href="https://m.apkpure.com/">APKPure: Download APK on Android with Free APK Downloader</a></li>

</ul>
</details>

**Tags**: `#security`, `#spyware`, `#Telegram`, `#APKPure`, `#mobile malware`

---

<a id="item-2"></a>
## [Memory hits ~2/3 of AI chip component costs](https://epoch.ai/data-insights/ai-chip-component-cost-shares) ⭐️ 8.0/10

According to Epoch AI, memory costs have grown to nearly two-thirds of total AI chip component costs, driven by the high price of High Bandwidth Memory (HBM) used in AI accelerators. This cost shift has major implications for AI hardware pricing, suggesting that AI inference and training could see a ~3x hardware cost reduction once DRAM supply catches up with demand. HBM consumes about three times the wafer capacity of DDR5 per gigabyte, and the complexity of its manufacturing keeps yields low. Community discussion notes that even without new technology, waiting for supply to meet demand could cut costs significantly.

hackernews · intelkishan · May 24, 16:31 · [Discussion](https://news.ycombinator.com/item?id=48258684)

**Background**: AI chips such as GPUs and NPUs rely on High Bandwidth Memory (HBM) to feed data to thousands of parallel cores. HBM stacks DRAM dies vertically, offering high bandwidth and low power consumption, but it is expensive to produce. The surge in AI demand has pushed memory cost share from a minor fraction to nearly two-thirds.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.tomshardware.com/pc-components/ram/hbm-is-eating-your-ram">Here's why HBM is coming for your PC's RAM — HBM consumes around three times the wafer capacity of DDR5 per gigabyte, as AI supercharges demand for chips and advanced packaging | Tom's Hardware</a></li>
<li><a href="https://www.appliedmaterials.com/us/en/semiconductor/markets-and-inflections/memory/hbm.html">High Bandwidth Memory (HBM)</a></li>

</ul>
</details>

**Discussion**: Community comments highlight that RAM prices have soared, with one user noting that 96GB of DDR4 cost $250 two years ago but $1200 now. Some argue that DRAM capacity growth (20-25% per year) is insufficient to meet AI demand, while others say they will delay hardware upgrades until prices drop.

**Tags**: `#AI hardware`, `#memory pricing`, `#chip costs`, `#supply chain`

---

<a id="item-3"></a>
## [Constraint Decay: LLM Agents Struggle with Architectural Rules](https://arxiv.org/abs/2605.06445) ⭐️ 8.0/10

A new systematic study reveals that LLM agents exhibit 'constraint decay,' where their adherence to explicit architectural rules degrades as the number of constraints increases during multi-file backend code generation. This finding highlights a critical reliability gap for production-grade backend development using LLM agents, as they perform well in unconstrained prototyping but become unreliable when strict architectural rules must be followed. The study found that models silently drop the least prominent constraints when constraint counts rise, and framework conventions are abandoned before explicit contracts. The performance drop was observed consistently across tested models, though frontier models were not fully evaluated due to cost.

hackernews · wek · May 24, 12:55 · [Discussion](https://news.ycombinator.com/item?id=48256912)

**Background**: LLM agents are autonomous systems that use large language models to generate code. Constraint decay is a newly identified failure mode where an agent's adherence to initially confirmed rules gradually weakens over extended interactions. This study specifically examined multi-file backend code generation under structural constraints, a common task in real-world software engineering.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.06445">[2605.06445] Constraint Decay: The Fragility of LLM Agents in ... Constraint Decay in Backend Code Generation - agentpatterns.ai Constraint Decay: The Fragility of LLM Agents in Backend Code ... Constraint Decay: The Fragility of LLM Agents in Back End ... Constraint Collapse and Fidelity Decay: When Feedback Stops ... Constraint Decay: A New Failure Type in the Era of Large ...</a></li>
<li><a href="https://www.agentpatterns.ai/verification/constraint-decay-backend-agents/">Constraint Decay in Backend Code Generation - agentpatterns.ai</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with the findings, with one user noting their own experience of having to add more constraints as complexity grows. Another pointed out that the study did not test the latest frontier models, which might perform better, but overall the discussion validated the phenomenon of constraint decay in practice.

**Tags**: `#LLM agents`, `#code generation`, `#AI reliability`, `#software engineering`, `#constraint decay`

---

<a id="item-4"></a>
## [Vivado 2026.1 Removes Free Linux Support](https://adaptivesupport.amd.com/s/question/0D5Pd00001YQLdMKAX/why-is-vivado-20261-dropping-linux-support-for-free-tier-?language=en_US) ⭐️ 8.0/10

AMD's Vivado 2026.1 update removes Linux support from the free Basic tier, while Windows continues to be supported. This change was confirmed in an official forum post from AMD. This decision could alienate students, hobbyists, and developers who rely on Linux for FPGA development, potentially shrinking the AMD/Xilinx ecosystem. It may drive users to competing vendors like Lattice or Intel, which offer more Linux-friendly free tools. Only the free Basic tier loses Linux support; paid Standard and Enterprise editions retain Linux capabilities. The free tier is essential for learning and small-scale projects, and its Linux removal is a significant barrier for many users.

hackernews · zdw · May 24, 04:14 · [Discussion](https://news.ycombinator.com/item?id=48254309)

**Background**: Vivado is AMD's integrated design environment for FPGAs (field-programmable gate arrays) and adaptive SoCs. FPGAs are reconfigurable chips used in hardware acceleration, communications, and embedded systems. The free tier, previously known as WebPACK, allows full access to certain device families without cost, crucial for education and hobbyist adoption.

<details><summary>References</summary>
<ul>
<li><a href="https://www.amd.com/en/products/software/adaptive-socs-and-fpgas/vivado.html">Vivado Overview - AMD</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vivado">Vivado - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Field-programmable_gate_array">Field-programmable gate array - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community responses are overwhelmingly negative, with users calling the move short-sighted and anti-ecosystem. Many compare unfavorably to Lattice's free-for-basic-chips policy and express concerns that AMD is prioritizing monetization over user growth. Some users indicate they will switch vendors for future projects.

**Tags**: `#AMD`, `#Xilinx`, `#Vivado`, `#FPGA`, `#Linux`

---

<a id="item-5"></a>
## [Armin Ronacher Criticizes AI-Generated Bug Reports](https://simonwillison.net/2026/May/24/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Armin Ronacher has publicly criticized the increasing prevalence of AI-generated bug reports in open source projects, specifically highlighting how LLM-reworded issues often contain inaccurate conclusions and false confidence. He proposes a simple, human-observed format for issue reporting: describe the command run, expected behavior, actual behavior, and exact error/log. This matters because AI-generated bug reports degrade the quality of issue tracking, wasting maintainers' time on misleading or irrelevant information. As LLMs become more integrated into developer workflows, this issue will affect the sustainability and efficiency of open source maintenance. Ronacher calls these reports 'slop issues,' noting they often include 'fake-minimal repros,' incorrect root cause guesses, and irrelevant error lists. His proposed three-step format aims to strip away AI-generated noise and focus on direct human observation.

rss · Simon Willison · May 24, 18:46

**Background**: The rise of generative AI tools has led to an increase in users submitting bug reports that have been automatically rewritten or expanded by LLMs. These reports often sound confident but are factually unreliable, creating additional work for maintainers who must parse and verify the content. Ronacher, a prominent figure in the Python and open source communities, is known for creating Flask and Click.

**Tags**: `#open source`, `#bug reports`, `#LLMs`, `#software engineering`

---

<a id="item-6"></a>
## [Huawei announces 'Tao's Law' using time scaling for semiconductors](https://www.peopleapp.com/column/30052220655-500007509895) ⭐️ 8.0/10

At the 2026 IEEE ISCAS conference in Shanghai, Huawei presented the Tau (τ) Scaling Law, which replaces traditional geometric scaling with time scaling. The company claims to have designed and mass-produced 381 chips over the past six years using this principle, and will launch a new Kirin phone chip with logic folding technology this fall. This law could provide a new path for semiconductor advancement as Moore's Law approaches physical limits, potentially reshaping the industry's R&D direction. If validated, it may allow continued performance improvements without requiring extreme miniaturization, benefiting the entire electronics ecosystem. The Tau Scaling Law focuses on systematically reducing the time constant (τ) across device, circuit, chip, and system levels. Huawei predicts that by 2031, chips based on this law could achieve a transistor density equivalent to a 1.4nm process.

telegram · zaihuapd · May 25, 01:35

**Background**: Moore's Law, which states that the number of transistors on a chip doubles roughly every two years, has driven semiconductor progress for decades. However, as transistor sizes approach atomic scales, geometric scaling becomes increasingly difficult and costly. Traditional scaling methods like Dennard scaling have also faced limitations. The Tau Scaling Law proposes a paradigm shift by optimizing temporal performance instead of reducing physical dimensions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/5/ieee-iscas-tau-scaling">HUAWEI Presents the Tau (τ) Scaling Law, Enabling Breakthroughs in ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Moore's_law">Moore's law - Wikipedia</a></li>
<li><a href="https://www.globaltimes.cn/page/202605/1361841.shtml">Huawei unveils new semiconductor law, charting fresh path for ...</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#Huawei`, `#Moore's Law`, `#chip design`, `#innovation`

---

<a id="item-7"></a>
## [Epic Reveals Unreal Engine 6, First Game: Rocket League](https://www.pcgamer.com/gaming-industry/epic-reveals-first-unreal-engine-6-game-and-its-not-fortnite/) ⭐️ 8.0/10

Epic Games announced Unreal Engine 6 at the Rocket League Championship Series in Paris, and confirmed that Rocket League will upgrade directly from Unreal Engine 3 to UE6. This marks a major new version of a widely-used game engine, signaling Epic's strategic direction and potential impact on game development, especially as Unreal Engine 5 faced optimization criticisms. Rocket League has been running on UE3 since its release, so the jump to UE6 represents a generational leap equivalent to a sequel. The UE6 teaser also included footage from Fortnite, suggesting a unified metaverse push.

telegram · zaihuapd · May 25, 02:20

**Background**: Unreal Engine is a 3D game engine developed by Epic Games, first used in the 1998 game Unreal. It is considered middleware that provides core functionality for game development. Epic has previously released UE5 in 2022, which became widely adopted but faced criticism for performance issues on PC.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unreal_Engine">Unreal Engine - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Game_engine">Game engine - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#unreal-engine`, `#game-development`, `#epic-games`, `#announcement`, `#engine-update`

---