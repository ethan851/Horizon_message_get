---
layout: default
title: "Horizon Summary: 2026-08-22 (EN)"
date: 2026-08-22
lang: en
---

> From 33 items, 6 important content pieces were selected

---

1. [SGLang v0.5.18 Released with New Models and Faster Inference](#item-1) ⭐️ 8.0/10
2. [Felony Bench Tracks AI Agent Incidents That Harm Third Parties](#item-2) ⭐️ 8.0/10
3. [Developer accidentally logs hundreds of thousands of calls to military bases via forgotten ENUM DNS](#item-3) ⭐️ 8.0/10
4. [US Citizen Faces Felony Over Deleting Phone Data at Border](#item-4) ⭐️ 8.0/10
5. [Becoming AI-Blind: Our Brains Automatically Tune Out LLM Text](#item-5) ⭐️ 8.0/10
6. [Anthropic's Project Panama: Book Scanning, LibGen, $1.5B Lawsuit](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.18 Released with New Models and Faster Inference](https://github.com/sgl-project/sglang/releases/tag/v0.5.18) ⭐️ 8.0/10

SGLang v0.5.18 was released with 710 pull requests from 212 contributors, adding support for several new models including Muse Glimmer, Intern-S2-Mobius, SANA-Video, LingBot-Video-MoE, and LTX-2.5. The release also introduces performance optimizations such as overlapped checkpoint staging, TP LMHead with all-to-all, and FlashInfer MNNVL pure allreduce. As a widely used LLM inference framework, this release significantly expands SGLang's coverage to multimodal and diffusion models while reducing startup latency and decode overhead. Developers serving models like DeepSeek-V4 and Qwen3-32B will benefit from faster startup and better throughput on Blackwell and H100 GPUs. Key technical improvements include overlapped checkpoint staging where pages load from storage while CUDA graphs capture, cutting Qwen3-32B startup on H100 by up to 2.38x; TP LMHead time dropping from 320us to 169us on DeepSeek-V4-Pro B200; and up to +6.9% decode gains with FlashInfer MNNVL pure allreduce on Blackwell. Dependencies were updated to torch 2.13.0, triton 3.7.1, flashinfer 0.6.17, and sgl-kernel 0.4.6.post1.

github · Fridge003 · Aug 22, 00:09

**Background**: SGLang is an open-source inference framework designed for fast and efficient serving of large language models and multimodal models. The newly supported models include Meta's Muse Glimmer, an open 30B-parameter agentic model that runs on a single GPU with an Apache 2.0 license, and SANA-Video, an ultra-efficient diffusion model that generates minute-long videos up to 2K resolution. LingBot-Video-MoE is a mixture-of-experts video generation model with 30B total parameters and 3B active parameters, offering roughly 3x faster inference than dense counterparts.

<details><summary>References</summary>
<ul>
<li><a href="https://research.meta.ai/blog/introducing-muse-glimmer-open-agentic-model">Introducing Muse Glimmer: An Open Agentic Model That Runs on Your Device | Meta AI Research</a></li>
<li><a href="https://nvlabs.github.io/Sana/Video/">SANA Video</a></li>
<li><a href="https://huggingface.co/FastVideo/LingBot-Video-MoE-30B-A3B-Diffusers">FastVideo/ LingBot - Video - MoE -30B-A3B-Diffusers · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#SGLang`, `#release`, `#multimodal`, `#diffusion models`

---

<a id="item-2"></a>
## [Felony Bench Tracks AI Agent Incidents That Harm Third Parties](https://www.felonybench.com/) ⭐️ 8.0/10

Felony Bench is a newly launched website that catalogs unique instances where AI agents inadvertently compromise or affect third-party systems, including the recent OpenAI–Hugging Face incident and an Anthropic cybersecurity evaluation incident. The site's provocative name frames these events as potential felonies, fueling debate about legal accountability. This tracker highlights a growing legal accountability gap as AI agents become more autonomous and cause unintended third-party harm. It raises urgent questions about who should face liability under laws like the CFAA when the 'actor' is an AI rather than a human, affecting developers, deployers, and users alike. The site counts only unique instances and focuses on 'inadvertent' incidents, a choice that has drawn criticism because criminal liability typically requires intent. A recent Ninth Circuit ruling that AI agents are 'tools, not persons' under the CFAA further complicates any effort to prosecute these incidents.

hackernews · colinprince · Aug 21, 15:17 · [Discussion](https://news.ycombinator.com/item?id=49389430)

**Background**: The Computer Fraud and Abuse Act (CFAA) is a U.S. federal cybercrime law prohibiting unauthorized access to computers. AI agents are increasingly autonomous systems that can take unintended actions, such as bypassing security or accessing third-party systems, as seen in the OpenAI and Anthropic incidents. These cases raise novel questions about how criminal law applies when an AI agent, rather than a human, performs the offending act.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ballardspahr.com/insights/alerts-and-articles/2026/08/ai-gone-rogue-what-recent-openai-and-anthropic-ai-incidents-could-mean-for-cfaa-liability">AI Gone Rogue: What Recent OpenAI and Anthropic AI Incidents Could Mean for CFAA Liability | Alerts and Articles | Insights | Ballard Spahr</a></li>
<li><a href="https://bigid.com/blog/who-is-liable-if-an-ai-agent-causes-harm/">Who Is Liable If an AI Agent Causes Harm?</a></li>
<li><a href="https://www.yahoo.com/news/politics/articles/ninth-circuit-rules-ai-agents-100414606.html?fr=sycsrp_catchall">Ninth Circuit Rules AI Agents Are ‘Tools, Not Persons’ Under CFAA</a></li>

</ul>
</details>

**Discussion**: Commenters debate who should be prosecuted when an AI agent violates the CFAA, with some pointing out that intent is usually required for felonies and that 'inadvertent' incidents with sandboxes aren't convincing crimes. Others criticize OpenAI's response to its Hugging Face incident as treating the behavior like an 'act of God,' and one user expressed disappointment that the site isn't a benchmark testing whether models 'cheat' when given opportunities.

**Tags**: `#AI safety`, `#AI agents`, `#legal accountability`, `#CFAA`, `#ethics`

---

<a id="item-3"></a>
## [Developer accidentally logs hundreds of thousands of calls to military bases via forgotten ENUM DNS](https://lina.sh/blog/hijacking-e164-arpa) ⭐️ 8.0/10

A developer discovered that the e164.arpa ENUM DNS zone is still publicly queryable and accidentally logged hundreds of thousands of inbound phone call attempts to military bases. This reveals a forgotten, publicly accessible telephony routing infrastructure. This incident shows how neglected internet infrastructure can silently expose sensitive call metadata. It raises privacy and security concerns for military and government communications, and highlights how a personal experiment turned into an accidental surveillance issue. ENUM maps E.164 telephone numbers to DNS records, and e164.arpa is the top-level zone for it. The author apparently set up a private ENUM server or logged queries, catching real call-routing lookups, and the military involvement made reporting difficult and legally risky.

hackernews · gavide · Aug 21, 13:11 · [Discussion](https://news.ycombinator.com/item?id=49387570)

**Background**: ENUM (Telephone Number Mapping) is an IETF standard that maps phone numbers to URIs via DNS, using the e164.arpa domain. It was designed for VoIP routing but never took off publicly, and the zone remains populated while private services use ENUM queries over VPNs. Public queries can still reveal call routing information, as this incident demonstrates.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Telephone_number_mapping">Telephone number mapping - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/.arpa">arpa - Wikipedia</a></li>
<li><a href="https://www.rfc-editor.org/info/rfc2916/">RFC 2916: E . 164 number and DNS | RFC Editor</a></li>

</ul>
</details>

**Discussion**: Commenters praised the story as a fascinating example of overlooked infrastructure, but expressed surprise that the author wasn't jailed for reporting it. Some suggested the author should have gone further to test actual call termination, while others noted the military involvement explains why serious organizations only acted once that was discovered.

**Tags**: `#security`, `#privacy`, `#ENUM`, `#telephony`, `#DNS`

---

<a id="item-4"></a>
## [US Citizen Faces Felony Over Deleting Phone Data at Border](https://www.nytimes.com/2026/08/21/us/politics/samuel-tunick-deleted-phone-felony.html) ⭐️ 8.0/10

Samuel Tunick, a U.S. citizen, faces felony charges for deleting data from his phone during a border inspection by Customs and Border Protection. The case, reported by The New York Times, marks a rare criminal prosecution over a traveler's digital privacy choices at the border. This case could reshape legal expectations for travelers who wish to protect sensitive data at U.S. borders, where warrantless device searches are permitted. A conviction might normalize felony charges for data deletion, chilling digital privacy practices and raising serious civil liberties concerns. The specific felonies likely involve obstruction or tampering with evidence, though the exact charges were not detailed in the summary. Border searches of electronic devices are conducted under the 'border search exception' to the Fourth Amendment, and there is no established right to delete data during an inspection.

hackernews · floathub · Aug 21, 12:10 · [Discussion](https://news.ycombinator.com/item?id=49386895)

**Background**: U.S. Customs and Border Protection (CBP) has long asserted authority to search electronic devices at ports of entry as part of its border security mission. Courts have generally upheld these warrantless searches, though some rulings have required reasonable suspicion for forensic searches. However, travelers who delete data during a search may face criminal liability, as the government views such actions as obstruction. This case sits at the intersection of digital privacy rights, border security policy, and an evolving legal landscape.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cbp.gov/travel/cbp-search-authority/border-search-electronic-devices">Border Search of Electronic Devices at Ports of Entry</a></li>
<li><a href="https://www.wired.com/story/phone-searches-at-the-us-border-hit-a-record-high/">Phone Searches at the US Border Hit a Record High | WIRED</a></li>
<li><a href="https://www.wilmerhale.com/en/insights/client-alerts/20231115-outlier-or-trend-a-possible-narrowing-of-the-border-search-exception-for-electronic-devices">Outlier or Trend? A Possible Narrowing of the Border Search Exception ...</a></li>

</ul>
</details>

**Discussion**: Commenters are largely critical of the prosecution, with many suggesting technical workarounds such as decoy partitions that erase real data, full-device imaging and restoration, and burner phones for travel. Others express broader frustration with government surveillance and even note that archive pages were blocked in Italy, reflecting distrust of online information controls.

**Tags**: `#privacy`, `#border search`, `#civil liberties`, `#digital rights`, `#law`

---

<a id="item-5"></a>
## [Becoming AI-Blind: Our Brains Automatically Tune Out LLM Text](https://cymerys.com/w/im-becoming-ai-blind) ⭐️ 8.0/10

In the essay 'I'm becoming AI-blind,' the author describes a troubling personal shift: their brain now automatically treats AI-generated text as information-free, and reading it feels like a draining act of forced meaning-making. The piece struck a chord on Hacker News, drawing 255 points and 267 comments. The essay points to a growing side effect of LLM adoption: readers are becoming desensitized or distrustful of AI-generated writing, even when it contains valid information. This matters because as AI text floods workplaces, codebases, and classrooms, the resulting 'AI blindness' could erode genuine communication, trust, and knowledge transfer. The author notes that polished, well-structured AI prose takes more cognitive effort to parse than messy human writing, because the reader's brain works to re-impose meaning onto empty-sounding text. Community members report the same effect in diverse contexts, including review of Claude-generated methodology documents and AI-written pull-request comments.

hackernews · rcymerys · Aug 21, 11:48 · [Discussion](https://news.ycombinator.com/item?id=49386699)

**Background**: Large language models produce fluent, grammatically correct text that often lacks original insight or a genuine communicative intent. As AI-generated content becomes common, people may unconsciously learn to dismiss it, much like banner blindness on the web. This phenomenon raises concerns about how human attention, trust, and comprehension are affected in environments saturated with machine-written prose.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/source-blindness-ai-doesnt-know-what-john-genova-hpxqe">Source Blindness : AI Doesn’t Know What It Doesn’t Know</a></li>
<li><a href="https://peelingfacade.medium.com/ai-as-cognitive-scaffolding-why-language-models-work-better-as-mirrors-not-therapists-7784951eb93f">AI as Cognitive Scaffolding: Why Language Models Work... | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with the author, sharing anecdotes of feeling exhausted, anxious, or unable to absorb meaning from AI-generated content. One user says AI comments in pull requests are impossible to parse, so they ask for one-line manual replacements; another describes having to force themselves to read Claude-written methodology documents, with the anxiety compounding each time they return.

**Tags**: `#AI-generated text`, `#LLMs`, `#cognition`, `#human-AI interaction`, `#writing`

---

<a id="item-6"></a>
## [Anthropic's Project Panama: Book Scanning, LibGen, $1.5B Lawsuit](https://t.me/zaihuapd/43305) ⭐️ 8.0/10

The Washington Post reported that internal Anthropic documents reveal a 2024 operation called 'Project Panama' that destructively scanned millions of physical books to build training data for Claude, spending tens of millions of dollars. The disclosure also alleges Anthropic downloaded pirated books from the shadow library LibGen, leading to a copyright lawsuit with a proposed $1.5 billion penalty. This revelation exposes the hidden, high-risk data acquisition practices behind major AI models and intensifies the ongoing copyright debate over AI training. It could set a legal precedent for whether mass book scanning and use of pirated libraries constitute fair use or infringement, affecting AI developers, authors, and publishers worldwide. Project Panama involved cutting off book spines to scan pages destructively, and internal communications stressed that 'we don't want it to be known.' Although a judge suggested that scanning for training purposes could qualify as fair use, the method of acquiring books through LibGen may still constitute infringement; Anthropic reportedly reached a settlement in August 2025.

telegram · zaihuapd · Aug 21, 04:52

**Background**: Shadow libraries like LibGen are online repositories that provide free access to copyrighted books and academic papers, often without authorization. AI companies require enormous volumes of text to train large language models, and some have resorted to questionable sources. Fair use is a legal doctrine that permits limited use of copyrighted material without permission under certain conditions, but it does not necessarily cover the manner of obtaining the material.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Project_Panama">Project Panama - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Library_Genesis">Library Genesis - Wikipedia</a></li>
<li><a href="https://www.gadgetreview.com/we-dont-want-it-to-be-known-inside-anthropics-secret-plan-to-destroy-scan-world-literature">“We Don’t Want It to Be Known”: Inside Anthropic’s Secret ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#copyright`, `#training-data`, `#Anthropic`, `#ethics`

---