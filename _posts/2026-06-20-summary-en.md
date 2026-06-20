---
layout: default
title: "Horizon Summary: 2026-06-20 (EN)"
date: 2026-06-20
lang: en
---

> From 27 items, 9 important content pieces were selected

---

1. [Project Valhalla Finally Lands in JDK 28](#item-1) ⭐️ 9.0/10
2. [ATProto Has No 'Instances' — A Protocol Architecture Clarification](#item-2) ⭐️ 8.0/10
3. [Norway bans AI in elementary schools](#item-3) ⭐️ 8.0/10
4. [Court Records Should Be Free](#item-4) ⭐️ 8.0/10
5. [US Pressures ASML over Possible EUV Machine in China](#item-5) ⭐️ 8.0/10
6. [Popular diaper brands in China found to contain reproductive toxin formamide](#item-6) ⭐️ 8.0/10
7. [Apple Agrees to Allow Third-Party App Stores and External Payments in Brazil](#item-7) ⭐️ 8.0/10
8. [Beihang PhD Student Accuses Professors of Paper Fabrication](#item-8) ⭐️ 8.0/10
9. [Anthropic Engineers Meet White House Over AI Model Shutdown](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Project Valhalla Finally Lands in JDK 28](https://www.jvm-weekly.com/p/project-valhalla-explained-how-a) ⭐️ 9.0/10

After a decade of development, Project Valhalla's value types and null-safety improvements are being integrated into JDK 28, marking a major milestone for the JVM. This brings performance benefits through flattened memory layouts and reduced indirection, while null-safety features help prevent common programming errors, significantly impacting Java developers and enterprise applications. The implementation allows JVM to store value objects densely in arrays without per-element headers or pointers, but heap flattening may have a 64-bit limit; a null flag may still be needed for each element.

hackernews · philonoist · Jun 19, 06:35 · [Discussion](https://news.ycombinator.com/item?id=48595511)

**Background**: Project Valhalla is an OpenJDK effort started in 2014 to extend the Java object model with value types, which behave like primitives but are user-defined. Value types aim to combine the abstraction of objects with the performance of primitives by enabling flat memory layouts. Null-safety is another long-desired feature to reduce NullPointerExceptions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Project_Valhalla_(Java_language)">Project Valhalla (Java language) - Wikipedia</a></li>
<li><a href="https://openjdk.org/projects/valhalla/">Project Valhalla - OpenJDK</a></li>

</ul>
</details>

**Discussion**: Comments reflect a mix of appreciation and critique: some users argue that null-safety should be simpler to adopt, while others question the practical limitations of heap flattening for larger objects. There's also sentiment that many critics have outdated views of modern Java.

**Tags**: `#Java`, `#JVM`, `#Project Valhalla`, `#value types`, `#null-safety`

---

<a id="item-2"></a>
## [ATProto Has No 'Instances' — A Protocol Architecture Clarification](https://overreacted.io/there-are-no-instances-in-atproto/) ⭐️ 8.0/10

Dan Abramov published an article explaining that ATProto, the protocol behind Bluesky, does not have 'instances' like Mastodon, but instead separates user data (PDS), data relay (Relays), and application serving (AppViews). This clarification corrects a widespread misconception about ATProto's architecture, which is crucial for understanding how decentralized social media can scale. It highlights a fundamental design difference from Mastodon, affecting developers and users evaluating federation approaches. Relays are an optimization to reduce the number of connections between PDSes and AppViews, and are not strictly necessary. AppViews fetch data from Relays to build timelines and aggregates, while PDSes store user data and cryptographic keys.

hackernews · danabramov · Jun 19, 15:10 · [Discussion](https://news.ycombinator.com/item?id=48599515)

**Background**: Mastodon and other ActivityPub-based platforms operate with 'instances' — independent servers that host users, content, and moderation. ATProto, used by Bluesky, decouples these functions into separate services: Personal Data Servers (PDS) for storage, Relays for data distribution, and AppViews for presenting content to users. This modular design aims to improve scalability and user portability.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AT_Protocol">AT Protocol - Wikipedia</a></li>
<li><a href="https://atproto.brussels/atproto-architecture">ATProto Architecture • atproto.brussels</a></li>
<li><a href="https://atproto.com/guides/glossary">A collection of terminology used in the AT Protocol and their definitions.</a></li>

</ul>
</details>

**Discussion**: Comments were mixed: some appreciated the clear explanation of ATProto's modular architecture, while others criticized the analogy to RSS and pointed out that in practice, Bluesky the corporation still runs most of the infrastructure, making the system de facto centralized. Some noted that Relays are expensive to run and a potential bottleneck.

**Tags**: `#ATProto`, `#Bluesky`, `#decentralization`, `#protocol design`, `#social media architecture`

---

<a id="item-3"></a>
## [Norway bans AI in elementary schools](https://www.reuters.com/technology/norway-imposes-near-ban-ai-elementary-school-2026-06-19/) ⭐️ 8.0/10

Norway's government announced a near-ban on AI for students aged 6-13, while allowing cautious use for ages 14-16 under teacher supervision. This sets a precedent for national AI regulation in education, addressing concerns about foundational skill development and potential learning disruptions. The ban applies to grades 1-7 (ages 6-13), while lower secondary students (14-16) may use AI tools carefully with teacher guidance.

hackernews · ilreb · Jun 19, 16:03 · [Discussion](https://news.ycombinator.com/item?id=48600093)

**Background**: Generative AI like ChatGPT can produce text quickly, potentially undermining reading, writing, and comprehension learning for young children. Norway's policy aims to protect foundational education by restricting AI until students have developed core skills.

**Discussion**: Commenters largely support the ban, drawing parallels to calculator use in math and emphasizing the need for reasoning skills before AI tools. Some note AI has been a disaster for student outcomes and warn of enforcement challenges.

**Tags**: `#AI`, `#education`, `#policy`, `#Norway`, `#debate`

---

<a id="item-4"></a>
## [Court Records Should Be Free](https://www.eff.org/deeplinks/2026/06/court-records-should-be-free) ⭐️ 8.0/10

The Electronic Frontier Foundation (EFF) published an article arguing that court records should be freely accessible, criticizing the paywall system of PACER that charges users per page. This matters because access to court records is fundamental to justice and transparency; high fees create barriers for individuals and small entities, undermining public accountability. PACER fees are $1 per page for federal courts, while state courts like Idaho charge $10 per page. Tools like CourtListener and Recap help by sharing purchased documents for free.

hackernews · hn_acker · Jun 19, 17:34 · [Discussion](https://news.ycombinator.com/item?id=48600946)

**Background**: PACER (Public Access to Court Electronic Records) is the electronic public access service for U.S. federal court documents. Critics argue that the fees, which fund the system, should be waived because public records belong to the public. The EFF and other advocacy groups have long called for making court records free.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PACER_(law)">PACER (law) - Wikipedia</a></li>
<li><a href="https://pacer.uscourts.gov/">Public Access to Court Electronic Records | PACER: Federal Court Records</a></li>

</ul>
</details>

**Discussion**: tptacek draws an analogy to municipal lead pipe replacement costs, highlighting a common public policy conundrum. jacobmarble notes that Idaho state court fees are ten times higher than federal fees. cdolan praises CourtListener and Recap for filling a vital niche, while treebeard901 argues that financial cost is one way the government intentionally limits access to rights.

**Tags**: `#court records`, `#PACER`, `#access to justice`, `#EFF`, `#public policy`

---

<a id="item-5"></a>
## [US Pressures ASML over Possible EUV Machine in China](https://www.bloomberg.com/news/articles/2026-06-19/us-tells-asml-it-s-concerned-china-may-have-top-chip-tool) ⭐️ 8.0/10

The US Commerce Secretary has told ASML executives that it suspects a top EUV lithography machine may have been exported to China, violating US-led export controls. ASML denies this, stating it has never shipped an EUV system to China. This incident heightens US-China tech tensions and could lead to stricter semiconductor export controls, impacting global supply chains and ASML's operations. It also strains US-Europe relations over chip policy. The US claims it has evidence of ASML not acting in good faith, including export of EUV-related transport equipment to China, but has not disclosed it. ASML has distributed documents to prove compliance and asserts it never exported any EUV-specific components.

telegram · zaihuapd · Jun 19, 03:09

**Background**: EUV lithography is a cutting-edge technology used to manufacture advanced semiconductors with features as small as 12 nm. ASML is the sole supplier of EUV systems, which are subject to strict export controls to prevent China from obtaining them. The US has been pressuring allies to tighten these controls.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Extreme_ultraviolet_lithography">Extreme ultraviolet lithography - Wikipedia</a></li>
<li><a href="https://www.asml.com/en/products/euv-lithography-systems">EUV lithography systems – Products | ASML</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#export controls`, `#ASML`, `#US-China`, `#lithography`

---

<a id="item-6"></a>
## [Popular diaper brands in China found to contain reproductive toxin formamide](https://t.me/zaihuapd/42051) ⭐️ 8.0/10

Economic Reference News commissioned testing found formamide, a reproductive toxin, in popular infant diaper brands including HUGGIES, Bébé, and Babycare; traces were also detected in infants' blood and urine. Formamide can be absorbed through skin and accumulate, posing long-term risks to reproductive health and vital organs; this exposé reveals a critical regulatory gap in China's diaper safety standards. China's cosmetic regulations already ban formamide, but national diaper standards do not test for it; a journalist wearing one tested diaper overnight saw his blood formamide level nearly double.

telegram · zaihuapd · Jun 19, 06:05

**Background**: Formamide is an industrial solvent used in production of some diapers. Studies in mice show it reduces fertility, and dermal absorption is a major human exposure route. Other countries limit formamide in foam toys (e.g., EN 71-15). China's current diaper standards do not cover formamide, leading to calls for revision.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Formamide">Formamide - Wikipedia</a></li>
<li><a href="https://www.sciencedirect.com/topics/pharmacology-toxicology-and-pharmaceutical-science/formamide">Formamide - an overview | ScienceDirect Topics</a></li>
<li><a href="https://standards.iteh.ai/catalog/standards/sist/50697200-e3d2-4e36-8299-efd4d2a2409c/sist-en-71-15-2025">SIST EN 71-15:2025 - Toy Safety Formamide Limits in Foam Materials</a></li>

</ul>
</details>

**Tags**: `#consumer safety`, `#public health`, `#regulatory gap`, `#toxicology`, `#infant products`

---

<a id="item-7"></a>
## [Apple Agrees to Allow Third-Party App Stores and External Payments in Brazil](https://t.me/zaihuapd/42059) ⭐️ 8.0/10

Apple has reached an agreement with Brazilian antitrust regulators to allow iPhone users to purchase apps and services outside the App Store and support third-party app stores. The changes must be implemented within 105 days, and the agreement lasts for three years. This marks a significant concession by Apple in a key market and could set a precedent for other jurisdictions pursuing similar antitrust actions. Developers will gain more freedom to offer alternative payment methods and distribution channels, potentially reducing Apple's commission fees. Under the agreement, developers can display external payment options and alternative purchase links, and Apple's payment system will be decoupled from the App Store. However, Apple may still charge fees on transactions made through external systems.

telegram · zaihuapd · Jun 19, 11:15

**Background**: For years, Apple has maintained tight control over iOS app distribution and payments, requiring developers to use its in-app purchase system and pay a 30% commission (15% for small businesses). This control has been challenged by regulators worldwide, including the European Union's Digital Markets Act (DMA) which forced Apple to allow third-party app stores in Europe. Brazil's antitrust investigation followed similar concerns about anticompetitive practices.

<details><summary>References</summary>
<ul>
<li><a href="https://adapty.io/blog/alternative-payments-in-the-app-store/">Alternative payments in the App Store: All you need to know</a></li>
<li><a href="https://eu.36kr.com/en/p/3825979669074820">Apple Unlocks the Door to Third - Party App Stores</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#antitrust`, `#Brazil`, `#app store`, `#payments`

---

<a id="item-8"></a>
## [Beihang PhD Student Accuses Professors of Paper Fabrication](https://www.zaobao.com.sg/news/china/story20260619-9231002) ⭐️ 8.0/10

Former Beihang University PhD student Geng Jiangtao publicly accused two professors, Chang Lingqian and Wang Jun, of fabricating data in papers published in Nature and other journals, prompting a surge of visitors that crashed the university's website. This case highlights growing public scrutiny of research integrity in China's top universities, and the increasing influence of citizen whistleblowers in exposing academic fraud. Geng, who dropped out of Beihang's PhD program in 2025 to become a science communicator, has since April targeted five scholars from four universities, all of whom faced consequences.

telegram · zaihuapd · Jun 19, 16:02

**Background**: Academic fraud has been a persistent issue in China's research system, with several high-profile cases damaging the reputation of elite institutions. Citizen whistleblowers, often former insiders, have emerged as key watchdogs, using social media to publish evidence and pressure institutions to investigate.

**Tags**: `#academic fraud`, `#research integrity`, `#Beihang University`, `#scientific misconduct`, `#China`

---

<a id="item-9"></a>
## [Anthropic Engineers Meet White House Over AI Model Shutdown](https://t.me/zaihuapd/42064) ⭐️ 8.0/10

Anthropic senior technical staff are scheduled to meet with White House officials next week to resolve a dispute that led to the global shutdown of their most advanced AI models, Fable 5 and Mythos 5. This meeting highlights escalating tensions between AI companies and government regulators over national security and foreign access to powerful AI, which could set a precedent for future AI governance and global availability. The Trump administration ordered Anthropic to block foreign nationals from using Fable 5 and Mythos 5, citing national security concerns; Anthropic responded by disabling both models worldwide for hundreds of millions of users.

telegram · zaihuapd · Jun 20, 02:45

**Background**: Anthropic's Mythos-class models, including Mythos 5 and the publicly released Fable 5, are designed for advanced tasks such as finding software vulnerabilities. The U.S. government's order was based on fears that foreign adversaries could misuse the models' powerful capabilities. Anthropic had already delayed Mythos 5's wider release due to its hacking potential before instituting safety measures for Fable 5.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/06/12/technology/anthropic-mythos-fable5-blocked.html">Anthropic Blocks Foreigners From Using Mythos and Fable AI</a></li>
<li><a href="https://www.bbc.com/news/articles/c932g3v3e13o">Anthropic 's Claude Fable 5 and Mythos 5 AI suspended over security...</a></li>
<li><a href="https://news.bitcoin.com/anthropic-fable-5-mythos-5-us-suspension/">Anthropic Disables Fable 5 and Mythos 5 Worldwide After US...</a></li>

</ul>
</details>

**Tags**: `#AI政策`, `#AI安全`, `#Anthropic`, `#政府监管`

---