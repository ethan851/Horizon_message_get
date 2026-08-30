---
layout: default
title: "Horizon Summary: 2026-08-30 (EN)"
date: 2026-08-30
lang: en
---

> From 20 items, 5 important content pieces were selected

---

1. [Tencent Open-Sources Hy4 Preview LLM with Self-Improvement Loop](#item-1) ⭐️ 8.0/10
2. [Good Culture, Not AI, Is the Biggest Productivity Hack](#item-2) ⭐️ 8.0/10
3. [DHS uses obscure customs law to snoop on journalists and NGOs](#item-3) ⭐️ 8.0/10
4. [China Proposes Unified 30,000 km Reliability Test for New Energy Vehicles](#item-4) ⭐️ 8.0/10
5. [Sony Music and Publishers Sue Anthropic Over Pirated Lyrics and Books in Claude Training](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Tencent Open-Sources Hy4 Preview LLM with Self-Improvement Loop](https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/) ⭐️ 8.0/10

Tencent released and open-sourced Hy4 preview, a 770B-parameter mixture-of-experts model, on Hugging Face and OpenRouter. It features an early-stage recursive self-improvement loop where the model optimized its own training methods, data strategies, and evaluation frameworks. This is significant because a major tech company open-sourcing a frontier-scale LLM with self-improvement capabilities could accelerate AI research and adoption. Hy4 preview also gained rapid traction on OpenRouter, processing trillions of tokens within days, indicating strong market demand. Hy4 preview is a mixture-of-experts model with 49B active parameters out of 770B total. It has a 1,048,576-token context window and costs $0.834 per million input tokens and $2.501 per million output tokens on OpenRouter.

hackernews · shenli3514 · Aug 29, 19:33 · [Discussion](https://news.ycombinator.com/item?id=49492632)

**Background**: Mixture-of-experts (MoE) models activate only a subset of parameters per token, reducing compute cost while keeping model capacity large. OpenRouter is an LLM routing service that lets developers access many models through a single API. Self-improvement in language models refers to using the model itself as a verifier or optimizer to refine its own outputs and training processes, a research area gaining traction.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/tencent/Hy4-preview">tencent/Hy4-preview · Hugging Face</a></li>
<li><a href="https://openrouter.ai/tencent/hy4-preview">Hy4 preview - API Pricing & Providers | OpenRouter</a></li>
<li><a href="https://cryptobriefing.com/tencent-hy4-preview-770b-ai-model/">Tencent spotted testing Hy4 model in Yuanbao app as expert-level model</a></li>

</ul>
</details>

**Discussion**: Commenters noted Hy4 preview's 'ludicrous traction' on OpenRouter, processing trillions of tokens in days, and discussed its cheap caching costs. Others raised questions about token density optimization and whether reducing vocabulary could create 'Newspeak' issues, while one commenter criticized the bar charts in the release.

**Tags**: `#AI/ML`, `#LLM`, `#Tencent`, `#Open Source`, `#Self-improvement`

---

<a id="item-2"></a>
## [Good Culture, Not AI, Is the Biggest Productivity Hack](https://newsletter.eng-leadership.com/p/good-culture-is-the-biggest-productivity) ⭐️ 8.0/10

The article argues that a strong engineering culture is a bigger productivity driver than AI, challenging the current hype around AI-driven productivity gains. Its thesis has sparked substantial discussion among practitioners, with several real-world examples reinforcing the importance of culture. This matters because many organizations are heavily investing in AI to boost productivity, possibly neglecting their team culture. The debate affects engineering leaders deciding where to allocate time and resources, and highlights that culture is often the overlooked foundation for any tool's success. The article's thesis is reinforced by community examples: one principal engineer noted a 20-person team that succeeded due to mutual liking and low turnover, while another commenter warned that AI accelerates dysfunction. Core cultural factors cited include predictability, market-rate pay, and team cohesion.

hackernews · gpi · Aug 29, 17:19 · [Discussion](https://news.ycombinator.com/item?id=49491568)

**Background**: Engineering culture refers to shared values, practices, and social dynamics within a development team. Productivity in software engineering is heavily influenced by communication, trust, and stable processes. The article argues that AI tools have limited impact when the underlying culture is poor, while a strong culture can amplify the benefits of AI.

**Discussion**: Commenters largely agree but add nuance: one notes that culture boils down to predictability and fair pay, while another warns that AI accelerates dysfunction. A principal engineer shares that a cohesive, low-turnover team was the most productive they have experienced, and someone else argues AI adoption should be bottom-up.

**Tags**: `#engineering-culture`, `#productivity`, `#leadership`, `#AI`, `#team-management`

---

<a id="item-3"></a>
## [DHS uses obscure customs law to snoop on journalists and NGOs](https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits) ⭐️ 8.0/10

The Department of Homeland Security has used summonses under 19 U.S.C. §1509, an obscure customs-enforcement law, to obtain communications records of journalists, non-profits, and unions. In several cases, the DHS withdrew the summons once challenged in court, while companies such as T-Mobile complied and Google reportedly did not. This matters because it highlights an expanding surveillance power that can bypass traditional judicial oversight, threatening press freedom and the ability of activists and unions to organize without government scrutiny. The practice has drawn bipartisan concern over privacy and civil liberties. The authority, originally designed for customs enforcement, lets CBP compel records without prior court approval, and targets are often not notified until later. A 2017 DHS Inspector General report already found CBP occasionally misused the summons power and lacked clear guidance.

hackernews · firefax · Aug 29, 18:44 · [Discussion](https://news.ycombinator.com/item?id=49492219)

**Background**: Under 19 U.S.C. §1509, U.S. Customs and Border Protection can issue an administrative summons to examine books and witnesses during customs-related investigations. Unlike a grand jury subpoena, a 1509 summons does not require prior approval from a judge, and the subject can be kept in the dark while companies hand over records. The law is rarely used in such contexts, which is why the reports of DHS deploying it against journalists and nonprofits have drawn alarm.

<details><summary>References</summary>
<ul>
<li><a href="https://www.law.cornell.edu/uscode/text/19/1509">19 U.S. Code § 1509 - Examination of books and witnesses</a></li>
<li><a href="https://www.oig.dhs.gov/news/press-releases/2017/11162017/dhs-oig-cites-cbp-misuse-summons-power">DHS OIG Cites CBP for Misuse of Summons Power | Office of Inspector General</a></li>
<li><a href="https://uscode.house.gov/view.xhtml?req=granuleid:USC-1999-title19-section1509&num=0&edition=1999">19 USC 1509: Examination of books and witnesses - House</a></li>

</ul>
</details>

**Discussion**: Commenters noted that a 1509 summons is not self-executing—targets can ignore it until DHS goes to court to enforce it—so companies like T-Mobile that comply without a fight share part of the blame. Others argued the DHS's pattern of withdrawing challenged summonses is a deliberate tactic to avoid an adverse judicial ruling, and some pointed to decentralized communication tools for journalists as a practical response.

**Tags**: `#surveillance`, `#privacy`, `#government`, `#law`, `#journalism`

---

<a id="item-4"></a>
## [China Proposes Unified 30,000 km Reliability Test for New Energy Vehicles](https://t.me/zaihuapd/43489) ⭐️ 8.0/10

The National Technical Committee of Auto Standardization (全国汽标委) has issued draft amendments to three new energy vehicle (NEV) type-approval test procedures for public comment. Under the proposal, the required reliability test mileage for BEVs, PHEVs and FCEVs would double to at least 30,000 km, achieving 'same standards for electric and fuel vehicles'. The change directly targets the 'quick-batch' (速成鸡) vehicle development pattern among Chinese EV startups, which often launch new models without sufficient validation. It will force automakers to take more responsibility for product quality and push the industry back toward safety and reliability, potentially increasing R&D time and costs for every new NEV model. For pure electric vehicles, at least 90% of the 30,000 km (i.e., 27,000 km) must be driven under DC fast-charging conditions to stress-test the battery, motor and electronic control systems. Plug-in hybrids are now required to complete at least 10,000 km in pure-electric mode, closing a testing loophole that previously let them rely mainly on engine operation.

telegram · zaihuapd · Aug 29, 13:30

**Background**: Type-approval testing (定型试验) is a mandatory verification process that a new car model must pass before it can be sold. The 'three-electric system' — the battery, drive motor, and electronic control — is the core of NEVs and directly determines their reliability and safety. DC fast charging supplies high-power direct current to rapidly recharge the battery, which puts far more stress on the battery and thermal management than AC slow charging. Previously, EVs only had to complete 50% of the fuel-vehicle reliability test mileage (15,000 km, with a lower limit of 5,000 km), so the new 30,000 km standard marks a move to 'same standard for electric as for fuel vehicles'.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/403047482">新能源汽车三电系统详解（电池、电机、电控） - 知乎</a></li>
<li><a href="https://post.smzdm.com/p/awwkz6gg/">电 车 可靠性 试 验 只跑油 车 一半，跑了21...</a></li>
<li><a href="https://longhaojiuding.com/news/9018370746.html">直 流 快 充 充 电桩：揭秘其技术核心与选型要点** - 临沂新能源有限公司</a></li>

</ul>
</details>

**Tags**: `#EV regulation`, `#automotive testing`, `#policy`, `#reliability`, `#China`

---

<a id="item-5"></a>
## [Sony Music and Publishers Sue Anthropic Over Pirated Lyrics and Books in Claude Training](https://www.musicbusinessworldwide.com/files/2026/08/COMPLAINT-in-Sony_Music_Publishing_US_LLC_e.pdf) ⭐️ 8.0/10

Sony Music Publishing, Warner Chappell Music, and other publishers filed a federal lawsuit in California against Anthropic and its founders, alleging the company illegally downloaded over 7 million books from pirate libraries such as LibGen and PiLiMi and scraped lyrics with copyright management information removed to train its Claude models. The plaintiffs are seeking statutory damages of up to $150,000 per infringed work and a permanent injunction. This lawsuit is another major legal challenge to the AI industry's practice of training models on copyrighted material without authorization, following earlier settlements and rulings that have reshaped how AI companies source training data. If successful, it could force Anthropic and other labs to pay billions in damages and adopt more transparent data provenance practices. The complaint specifically names LibGen and PiLiMi as sources of pirated books, and alleges that lyrics scraped by Anthropic had their copyright management information stripped, which is a separate violation under the Digital Millennium Copyright Act. The requested statutory damages of $150,000 per work could scale to a massive total given the more than 7 million books allegedly involved, and the suit also targets Anthropic's founders personally.

telegram · zaihuapd · Aug 30, 01:00

**Background**: Anthropic is the AI company behind the Claude large language model family, which is trained on vast amounts of text scraped from the internet and other sources. LibGen (Library Genesis) and PiLiMi (Pirate Library Mirror) are shadow libraries that provide free access to pirated books and academic texts, often without authorization from rights holders. This case fits a broader wave of copyright litigation against AI developers, including earlier lawsuits that led to a reported $1.5 billion settlement, as publishers and creators push back against the unlicensed use of their works in training data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Library_Genesis">Library Genesis - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Shadow_library">Shadow library - Wikipedia</a></li>
<li><a href="https://www.6pages.com/glossary/piratelibrarymirror(pilimi)/">Pirate Library Mirror (PiLiMi) | 6Pages</a></li>

</ul>
</details>

**Tags**: `#AI`, `#legal`, `#copyright`, `#Anthropic`, `#lawsuit`

---