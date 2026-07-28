---
layout: default
title: "Horizon Summary: 2026-07-28 (EN)"
date: 2026-07-28
lang: en
---

> From 25 items, 9 important content pieces were selected

---

1. [Moonshot AI Releases Open-Weight Kimi K3, 2.8T Parameters](#item-1) ⭐️ 9.0/10
2. [High-Risk RCE in Fastjson 1.x Without Gadget](#item-2) ⭐️ 9.0/10
3. [Anthropic clarifies stance on open-weights AI models](#item-3) ⭐️ 8.0/10
4. [Judge Rejects Google's DMCA Scraping Lawsuit](#item-4) ⭐️ 8.0/10
5. [Libsm64 turns Super Mario 64 into a reusable library for other games](#item-5) ⭐️ 8.0/10
6. [Google CEO Teases Gemini 4 as Most Ambitious Pretraining Project](#item-6) ⭐️ 8.0/10
7. [China Rejects US Sanctions Threat Over AI Model Distillation](#item-7) ⭐️ 8.0/10
8. [SMIC Tests China’s First Domestic DUV Lithography Machine](#item-8) ⭐️ 8.0/10
9. [Moonshot AI to Open-Source Kimi-K3, First 3T-Class Frontier Model](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Moonshot AI Releases Open-Weight Kimi K3, 2.8T Parameters](https://t.me/zaihuapd/42793) ⭐️ 9.0/10

Moonshot AI has released Kimi K3, the first open-weight model with 2.8 trillion parameters, achieving 1679 points in the Frontend Code Arena and surpassing Claude Fable 5 to rank first. Kimi K3's open-weight release and top benchmark performance set a new standard for large language models, particularly in frontend code generation, and its novel Kimi Delta Attention architecture could influence future model designs. Kimi K3 uses a hybrid linear attention architecture called Kimi Linear, with a 3:1 ratio of Kimi Delta Attention to global attention, reducing KV cache usage by up to 75% and supporting a 1 million token context window.

telegram · zaihuapd · Jul 27, 06:27

**Background**: Large language models typically use full attention mechanisms that are computationally expensive for long contexts. Kimi Delta Attention extends Gated DeltaNet with per-channel decay control, enabling efficient linear attention. The 2.8 trillion parameter scale makes K3 one of the largest open-weight models ever released.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2510.26692">[2510.26692] Kimi Linear: An Expressive, Efficient Attention ... GitHub - MoonshotAI/Kimi-Linear GitHub - hwilner/kimi-delta-attention: Educational ... Linear Attention: Kimi Delta Attention | Jianyu Huang Kimi Delta Attention - Papers with Code Kimi Linear: An Expressive, Efficient Attention Architecture Kimi K3 Technical Advancements Explained - nextbigfuture.com</a></li>
<li><a href="https://x.com/arena/status/2077824029126504525">Arena.ai on X: "Big news: Kimi-K3 by @Kimi_Moonshot is now #1 in the Frontend Code Arena with 1679 pts, surpassing Claude Fable 5. This is a 17-place jump from Kimi-k2.6 (#18 -> #1). In Frontend, Kimi-K3 ranked #1 in 6 of 7 domains: Brand & Marketing, Reference-Based Design, Data & Analytics, Consumer Product, Simulations, and Content Creation Tools, landing #2 only in Gaming behind Fable 5. The full model weights will be released by July 27. Congrats to the @Kimi_Moonshot team on this major milestone!" / X</a></li>
<li><a href="https://aitoolhunt.co/blog/kimi-k3-benchmarks-frontend-code-arena-2026">Kimi K3 Benchmarks: Frontend Leap and Review Verdicts (2026) | AIToolHunt</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#open-source`, `#benchmark`

---

<a id="item-2"></a>
## [High-Risk RCE in Fastjson 1.x Without Gadget](https://t.me/zaihuapd/42797) ⭐️ 9.0/10

Security researcher Kirill Firsov disclosed a high-risk remote code execution vulnerability in Fastjson versions 1.2.68 to 1.2.83. The exploit requires no gadget chain and no enabled autoType support, and works on JDK 8, 17, and 21. This vulnerability is critical because it bypasses traditional deserialization protections (no gadget and no autoType), affecting a wide range of Java applications. Since Fastjson 1.x is no longer maintained, users must upgrade to Fastjson2 to stay secure. The vulnerability affects Fastjson 1.2.68–1.2.83 and works on multiple JDK versions without requiring classpath gadgets or autoType. The official maintainers stopped supporting Fastjson 1.x in October 2024 and are unlikely to release a patch.

telegram · zaihuapd · Jul 27, 10:31

**Background**: Fastjson is a popular JSON library for Java, commonly used for serialization/deserialization. In Java deserialization, a 'gadget chain' is a sequence of classes that, when deserialized, can lead to arbitrary code execution. 'autoType' is a Fastjson feature that allows specifying type information in JSON, which attackers can abuse. This vulnerability is unusual because it does not require either a gadget chain or autoType, making it easier to exploit.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/alibaba/fastjson/wiki/enable_autotype">enable_autotype · alibaba/fastjson Wiki · GitHub</a></li>

</ul>
</details>

**Tags**: `#安全`, `#漏洞`, `#Fastjson`, `#RCE`, `#高危`

---

<a id="item-3"></a>
## [Anthropic clarifies stance on open-weights AI models](https://www.anthropic.com/news/position-open-weights-models) ⭐️ 8.0/10

Anthropic released a statement denying it advocates banning open-weights models, but calls for mandatory safety testing for all sufficiently capable models, both open and closed. As a leading AI lab, Anthropic's position influences the debate on AI regulation and open-source development, with critics accusing it of favoring regulatory capture that benefits its own business model. The statement follows community backlash and clarifies that Anthropic does not support a ban, but also endorses measures like restricting chip sales to China and cracking down on smuggling, which some see as contradictory to its anti-ban stance.

hackernews · surprisetalk · Jul 27, 22:03 · [Discussion](https://news.ycombinator.com/item?id=49076057)

**Background**: Open-weight models are AI models whose core components are publicly released, allowing anyone to download, inspect, modify, and run them. They are a key part of the open-source AI ecosystem, enabling wider access but also raising safety concerns due to potential misuse.

<details><summary>References</summary>
<ul>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>

</ul>
</details>

**Discussion**: Community comments are largely critical, with many accusing Anthropic of advocating for a de facto ban through burdensome testing requirements. Commenters also point to inconsistencies, such as supporting hardware bans while denying support for software bans, and suggest business motives behind the position.

**Tags**: `#open-weights`, `#AI safety`, `#regulation`, `#Anthropic`, `#AI ethics`

---

<a id="item-4"></a>
## [Judge Rejects Google's DMCA Scraping Lawsuit](https://www.techdirt.com/2026/07/27/judge-rejects-googles-attempt-to-dmca-its-way-out-of-being-scraped/) ⭐️ 8.0/10

A U.S. judge ruled that Google cannot use the Digital Millennium Copyright Act (DMCA) to block third-party services from scraping publicly available search results, marking a significant legal precedent. This decision upholds the legality of scraping public data, which is critical for competition, transparency, and tools like SEO analysis. It also highlights the irony of Google, built on crawling the web, trying to prevent others from doing the same. The case involved Google suing SerpAPI, a service that scrapes Google search results. The judge rejected Google's argument that the scraping amounted to copyright infringement under the DMCA, noting that search results are compilations of facts and not sufficiently creative to warrant copyright protection.

hackernews · cdrnsf · Jul 27, 18:15 · [Discussion](https://news.ycombinator.com/item?id=49073513)

**Background**: The DMCA includes anti-circumvention provisions that prevent bypassing technological measures protecting copyrighted works. Google attempted to argue that scraping its search results violated these provisions, but the court disagreed because the data itself was not copyrighted. The ruling reinforces that scraping publicly accessible data is generally legal in the U.S., provided no other laws are broken.

**Discussion**: Comments expressed frustration with Google's removal of affordable APIs, with users noting they rely on third-party scrapers as alternatives. Some pointed out the irony of Google, a company built on web scraping, using DMCA to block scrapers. Others highlighted societal benefits, such as detecting advertising scams.

**Tags**: `#scraping`, `#DMCA`, `#Google`, `#copyright`, `#legal`

---

<a id="item-5"></a>
## [Libsm64 turns Super Mario 64 into a reusable library for other games](https://github.com/libsm64/libsm64) ⭐️ 8.0/10

libsm64 is a reverse-engineered library that extracts Super Mario 64's character and physics, allowing Mario to be used as a playable character in external game engines like Half-Life 2. This project enables creative cross-game mashups and demonstrates a practical, non-blockchain approach to interoperability, which has been a promise of the metaverse. Developers can now easily integrate Mario into their own projects without needing to implement his complex movement from scratch. The library provides a minimal API defined in libsm64.h, and clients only need to include that header and link the shared library. Community members have already created demos like Mario in Half-Life 2 and maintained a curated list of projects using libsm64.

hackernews · klaussilveira · Jul 27, 10:04 · [Discussion](https://news.ycombinator.com/item?id=49067352)

**Background**: Super Mario 64 is a 1996 platform game for the Nintendo 64, known for its iconic character Mario and precise 3D movement mechanics. libsm64 reverse-engineers the original game's executable to extract the character's animation, physics, and control logic into a standalone C library, which can be compiled for multiple platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/libsm64/libsm64">GitHub - libsm64/libsm64: Mario 64 as a library for use in external game engines · GitHub</a></li>

</ul>
</details>

**Discussion**: Community members are enthusiastic, calling the library incredible and a realization of the metaverse without hype. Some shared demo videos of Mario in Half-Life 2, and one comment jokingly suggested selling "Mario 64 as a service" while reassuring Nintendo not to sue. Another user pointed to an awesome-libsm64 list of interesting projects.

**Tags**: `#reverse engineering`, `#game development`, `#interoperability`, `#retro gaming`, `#libraries`

---

<a id="item-6"></a>
## [Google CEO Teases Gemini 4 as Most Ambitious Pretraining Project](https://9to5google.com/2026/07/26/google-gemini-4-teases/) ⭐️ 8.0/10

Google CEO Sundar Pichai announced during Alphabet's Q2 2026 earnings call that the next-generation large language model, Gemini 4, is already in pretraining—the company's most ambitious effort to date, with a planned release in late 2026. This signals Google's commitment to maintaining leadership in the AI frontier by building even larger foundation models, directly impacting the competitive landscape against rivals like OpenAI and Anthropic. Pichai emphasized that Google will prioritize compute allocation for frontier AGI research to ensure Gemini 4 remains cutting-edge at launch. The Gemini 3.x Flash series will continue with near-monthly updates focusing on intelligent coding capabilities.

telegram · zaihuapd · Jul 27, 04:06

**Background**: Pretraining is the foundational phase where large language models learn broad language understanding from massive text corpora before being fine-tuned for specific tasks. AGI (artificial general intelligence) refers to a hypothetical AI that matches or exceeds human cognitive abilities across virtually all tasks. Google's Gemini series represents its flagship family of multimodal AI models, competing directly with OpenAI's GPT series and others.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sapien.io/blog/fine-tuning-vs-pre-training-key-differences-for-language-models">Fine-Tuning vs. Pre-Training: Their Impact on Language Models</a></li>
<li><a href="https://en.wikipedia.org/wiki/Artificial_general_intelligence">Artificial general intelligence - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Google`, `#Gemini`, `#Large Language Model`, `#Pretraining`

---

<a id="item-7"></a>
## [China Rejects US Sanctions Threat Over AI Model Distillation](https://www.mofcom.gov.cn/syxwfb/art/2026/art_7f1622463a7c48ef9fad600ce0ef702f.html) ⭐️ 8.0/10

China's Ministry of Commerce formally rejected US threats to investigate and sanction Chinese AI companies over alleged model distillation of American AI models, calling the accusations baseless. This dispute underscores escalating US-China tech tensions and could disrupt global AI research collaboration, as model distillation is a common technique used by companies worldwide, including US firms. The Ministry noted that nearly 200 US startups have urged the government not to restrict access to Chinese open-source models, and warned China will take necessary measures to protect its firms' rights if its interests are substantially harmed.

telegram · zaihuapd · Jul 27, 11:01

**Background**: Model distillation is a machine learning technique where a smaller 'student' model learns from a larger 'teacher' model, often used to create efficient AI systems. It is widely adopted in the AI industry for improving performance and reducing computational costs. The US has recently expressed concerns that Chinese companies might use distillation to copy proprietary US AI models, leading to sanctions threats.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://www.cnbc.com/2026/07/25/hat-is-distillation-and-why-is-everyone-so-obsessed-with-it-this-week.html">From Silicon Valley to DC, the tech world is suddenly obsessed with one concept in AI: Distillation</a></li>
<li><a href="https://labelbox.com/guides/model-distillation/">What is Model Distillation?</a></li>

</ul>
</details>

**Tags**: `#AI`, `#model distillation`, `#trade sanctions`, `#China`, `#US`

---

<a id="item-8"></a>
## [SMIC Tests China’s First Domestic DUV Lithography Machine](https://t.me/zaihuapd/42800) ⭐️ 8.0/10

SMIC is trial-running China’s first domestically developed advanced deep ultraviolet (DUV) lithography machine, built by Shanghai startup Yuliangsheng, targeting 28nm production and potentially 7nm via multi-patterning with a goal of mass production by 2027. This marks a significant step in China’s push for semiconductor self-sufficiency, reducing reliance on ASML’s DUV tools and circumventing US export restrictions on EUV lithography. However, the machine is still early-stage and faces challenges in yield and scaling. The machine utilizes 193nm argon fluoride (ArF) laser technology, similar to ASML’s Twinscan series, and most components are now domestically sourced, though some imports remain. SMIC is attempting to reach 7nm using multi-patterning, and even 5nm with lower yields.

telegram · zaihuapd · Jul 27, 14:10

**Background**: Deep ultraviolet (DUV) lithography uses light in the deep ultraviolet spectrum (e.g., 193nm wavelength) to pattern circuits on silicon wafers, enabling chip manufacturing. Multi-patterning lithography uses multiple photomasks to achieve finer patterns than a single exposure, which is key for producing advanced nodes like 7nm without extreme ultraviolet (EUV) tools. The US has restricted the sale of ASML’s EUV machines to China, making domestic DUV development crucial for China’s advanced chip aspirations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DUV_lithography">DUV lithography</a></li>
<li><a href="https://eureka.patsnap.com/article/duv-lithography-explained-how-193nm-arf-lasers-enable-7nm-nodes">DUV Lithography Explained: How 193nm ArF Lasers Enable 7nm...</a></li>
<li><a href="https://eureka.patsnap.com/article/multi-patterning-lithography-why-do-we-need-multiple-masks">Multi - Patterning Lithography : Why Do We Need Multiple Masks?</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#lithography`, `#SMIC`, `#DUV`, `#China tech`

---

<a id="item-9"></a>
## [Moonshot AI to Open-Source Kimi-K3, First 3T-Class Frontier Model](https://t.me/zaihuapd/42802) ⭐️ 8.0/10

Moonshot AI announced it will open-source Kimi-K3, a 2.8-trillion-parameter model built on novel Kimi Delta Attention and Attention Residuals architectures, with weights expected to be released on July 27, 2026 on Hugging Face. As the first open-source 3T-class model, Kimi-K3 pushes the frontier of open-source LLM scale and could accelerate research in long-horizon coding, knowledge work, and complex reasoning, democratizing access to cutting-edge AI capabilities. Kimi-K3 features a 1-million-token context window, native vision capabilities, and agentic abilities like tool use and multi-step planning, all enabled by its Kimi Delta Attention and Attention Residuals architecture. The weights will be released approximately a year from the announcement, in July 2026.

telegram · zaihuapd · Jul 27, 15:15

**Background**: Large language models (LLMs) are neural networks with billions of parameters; the parameter count often correlates with capability. Open-source LLMs, like Meta's Llama or Mistral, allow researchers and developers to inspect, modify, and run models on their own hardware. Kimi Delta Attention is a linear attention mechanism that enables efficient long-context processing, while Attention Residuals replace standard residual connections with a learned, input-dependent aggregation of previous layer outputs, improving representation quality.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/kimi-delta-attention">Kimi Delta Attention : Delta ‐Rule Linear Mechanism</a></li>
<li><a href="https://arxiv.org/abs/2603.15031">[2603.15031] Attention Residuals</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-source`, `#large language model`, `#Kimi-K3`, `#Moonshot AI`

---