---
layout: default
title: "Horizon Summary: 2026-06-18 (EN)"
date: 2026-06-18
lang: en
---

> From 36 items, 11 important content pieces were selected

---

1. [RFC 10008 Defines New HTTP QUERY Method](#item-1) ⭐️ 9.0/10
2. [GLM-5.2: Leading open weights LLM under MIT license](#item-2) ⭐️ 9.0/10
3. [Lore: Open Source VCS for Game Dev Scalability](#item-3) ⭐️ 8.0/10
4. [US Delays Blacklisting DeepSeek, Adds 100+ Chinese Firms to Risk List](#item-4) ⭐️ 8.0/10
5. [U.S. science-politics trust collapses, researchers flee](#item-5) ⭐️ 8.0/10
6. [Tesco moving 40k server workloads off VMware over Broadcom pricing](#item-6) ⭐️ 8.0/10
7. [GLM-5.2 tops open-weights models on Artificial Analysis](#item-7) ⭐️ 8.0/10
8. [Charity Majors: AI makes code generation free and disposable](#item-8) ⭐️ 8.0/10
9. [China Expands STAR Market Listing Rules to AI and Hard Tech](#item-9) ⭐️ 8.0/10
10. [Anthropic tops OpenAI in enterprise AI market share for first time](#item-10) ⭐️ 8.0/10
11. [Microsoft Grows China AI Business via OpenAI Models](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [RFC 10008 Defines New HTTP QUERY Method](https://www.rfc-editor.org/info/rfc10008/) ⭐️ 9.0/10

RFC 10008 introduces a new HTTP QUERY method that allows safe, idempotent requests with a request body, formalizing a pattern previously achieved by sending a body with GET, which was non-standard. This standardization provides a clean solution for complex queries in APIs, improving caching semantics and reducing reliance on POST for non-mutating operations, which could simplify web architecture and developer workflows. The QUERY method is safe and idempotent, but caching its responses requires including the request body in the cache key, which could lead to unbounded cache keys and practical challenges for intermediaries.

hackernews · schappim · Jun 17, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48568502)

**Background**: HTTP GET requests are designed for safe, idempotent data retrieval without a request body. However, for complex queries (e.g., large JSON filters), developers often sent a body with GET, violating HTTP specs and causing interoperability issues. The new QUERY method addresses this by providing a standard, safe way to send queries with a body.

<details><summary>References</summary>
<ul>
<li><a href="https://httpwg.org/http-extensions/draft-ietf-httpbis-safe-method-w-body.html">The HTTP QUERY Method</a></li>
<li><a href="https://horovits.medium.com/http-s-new-method-for-data-apis-http-query-1ff71e6f73f3">HTTP ‘s New Method For Data APIs: HTTP QUERY | Medium</a></li>

</ul>
</details>

**Discussion**: Community comments highlight interest in HTML form support for QUERY and concerns about caching with large request bodies. Some developers note they already use GET with body, while others question the practicality of including bodies in cache keys.

**Tags**: `#HTTP`, `#RFC`, `#web protocol`, `#API design`, `#caching`

---

<a id="item-2"></a>
## [GLM-5.2: Leading open weights LLM under MIT license](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai released GLM-5.2 on June 16, 2026 under the MIT license, a 753-billion-parameter Mixture-of-Experts model with a 1 million token context window, achieving top scores on the Artificial Analysis Intelligence Index among open weights models. This release provides a state-of-the-art open weights LLM that rivals proprietary models, fostering innovation and accessibility in the AI community with a permissive license that enables broad use and customization. GLM-5.2 uses 40 active experts out of a total 753B parameters, consumes more output tokens per task than peers, and is text-only; it ranks second on the Code Arena WebDev leaderboard behind Claude Fable 5.

rss · Simon Willison · Jun 17, 23:58

**Background**: Mixture-of-Experts (MoE) is an architecture where only a subset of parameters are activated per token, allowing large models with efficient inference. Open weights models release the trained parameter weights publicly, enabling fine-tuning and deployment, unlike fully closed models such as GPT-5.5.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://codingscape.com/blog/llms-with-largest-context-windows">LLMs with largest context windows</a></li>

</ul>
</details>

**Discussion**: The article highlights strong buzz and independent benchmarks confirming GLM-5.2's leading performance, though some note its higher token usage compared to other open weights models.

**Tags**: `#AI`, `#LLM`, `#open-weights`, `#MoE`, `#GLM-5.2`

---

<a id="item-3"></a>
## [Lore: Open Source VCS for Game Dev Scalability](https://lore.org/) ⭐️ 8.0/10

Epic Games has open-sourced Lore, a next-generation version control system designed to handle large binary assets and scale to massive teams, targeting game development and other media-centric projects. Lore offers a viable open-source alternative to Perforce, the incumbent VCS in game development, addressing Git's shortcomings with non-text files. It could reduce costs and vendor lock-in for studios while improving collaboration on assets like textures and 3D models. Lore is optimized for projects combining code with large binary assets, supports file locking for exclusive edits, and is maintained by Epic Games with direct integration into Unreal Engine 5. It is designed for unprecedented scalability of both data and teams.

hackernews · regnerba · Jun 17, 14:30 · [Discussion](https://news.ycombinator.com/item?id=48571081)

**Background**: Version control systems (VCS) like Git excel at text-based files but struggle with large binary files such as textures, audio, and 3D models common in game development. Perforce has been the de facto standard in the game industry due to its strong support for large files, file locking, and permissions, but it is proprietary and complex to administer. Lore aims to fill this gap as an open-source, scalable alternative.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/EpicGames/lore">Lore is a next-generation, open source revision control system</a></li>
<li><a href="https://lore.org/">Lore | Next-Generation Open Source Version Control - Lore</a></li>
<li><a href="https://dev.epicgames.com/documentation/unreal-engine/lore-version-control-in-unreal-engine?lang=en-US">Lore Version Control in Unreal Engine - Epic Dev</a></li>

</ul>
</details>

**Discussion**: The HN community largely sees Lore as a much-needed challenger to Perforce for game development, noting its potential for Unreal Engine workflows. Some commenters highlight that Git's UI is unfriendly and that Perforce, while familiar to artists, is showing its age. Overall sentiment is positive, with excitement about an open-source option that addresses real pain points without trying to replace Git for general coding.

**Tags**: `#version control`, `#game development`, `#open source`, `#scalability`, `#perforce alternative`

---

<a id="item-4"></a>
## [US Delays Blacklisting DeepSeek, Adds 100+ Chinese Firms to Risk List](https://www.reuters.com/world/china/us-holds-off-blacklisting-chinas-deepseek-more-than-100-firms-deemed-security-2026-06-17/) ⭐️ 8.0/10

The United States has decided to delay placing Chinese AI company DeepSeek on a trade blacklist, but has added over 100 other Chinese firms to its security risk list, according to a Reuters report. This decision highlights the ongoing US-China tech decoupling and the delicate balance between regulating national security risks and maintaining access to competitive AI technologies. Developers and users of DeepSeek's models may face uncertainty about future access. DeepSeek had been under scrutiny for its advanced, cost-efficient AI models that were trained using export-restricted NVIDIA GPUs. The company remains on a watchlist but not on the Entity List, which would ban US exports to it.

hackernews · giuliomagnifico · Jun 17, 03:55 · [Discussion](https://news.ycombinator.com/item?id=48565498)

**Background**: DeepSeek is a Chinese AI startup founded in 2023, known for developing large language models like DeepSeek-R1 at a fraction of the cost of competitors like OpenAI's GPT-4. Its models are open-weight and trained on weaker, export-restricted chips, challenging US dominance in AI. The US has been tightening export controls on advanced AI chips to China to prevent military use and maintain technological superiority.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>
<li><a href="https://www.deepseek.com/en/">DeepSeek</a></li>

</ul>
</details>

**Discussion**: Commenters expressed a range of opinions: some praised DeepSeek's affordability and coding capability (e.g., using it in VSCode), while others criticized US policies as protectionist and counterproductive, drawing parallels to China's firewall. A few noted that the Entity List does not completely block trade and that Chinese AI firms have minimal dependence on US goods besides NVIDIA GPUs, which are already restricted.

**Tags**: `#geopolitics`, `#AI regulation`, `#DeepSeek`, `#US-China trade`, `#technology policy`

---

<a id="item-5"></a>
## [U.S. science-politics trust collapses, researchers flee](https://www.scientificamerican.com/article/americas-compact-between-science-and-politics-is-broken/) ⭐️ 8.0/10

A Scientific American article reports that the trust between science and U.S. political institutions has broken down, with researchers facing funding freezes, visa restrictions, and political interference in grants. This crisis threatens U.S. leadership in research and innovation, as talented scientists and students are leaving the country or abandoning academia, weakening the nation's scientific enterprise. The article highlights unprecedented political interference, such as prohibiting grants mentioning diversity, equity, and inclusion (DEI), and arbitrary cancellations and delayed disbursements of funds.

hackernews · presspot · Jun 17, 09:54 · [Discussion](https://news.ycombinator.com/item?id=48568058)

**Background**: The U.S. scientific enterprise has long operated on a compact: scientists pursue knowledge free from political interference, and the government funds research with broad bipartisan support. However, recent years have seen increasing politicization of science, with partisan attacks on issues like climate change and COVID-19, and now direct interference in grant-making, undermining the traditional trust.

**Discussion**: Commenters share personal accounts: a researcher's wife operating a rare optical trap microscope is moving abroad due to the mess; professors report dried-up funding and visa restrictions blocking foreign graduate students; the mood in some fields has shifted from cautious optimism to palpable tension, with many established scientists preparing backup plans.

**Tags**: `#science policy`, `#research funding`, `#academia`, `#US politics`, `#immigration`

---

<a id="item-6"></a>
## [Tesco moving 40k server workloads off VMware over Broadcom pricing](https://arstechnica.com/information-technology/2026/06/tesco-moving-40000-server-workloads-off-vmware-amid-broadcoms-abusive-conduct/) ⭐️ 8.0/10

Tesco, the largest UK supermarket chain, announced it is migrating 40,000 server workloads away from VMware in response to Broadcom's aggressive pricing and support cuts following its acquisition of VMware. This massive-scale migration by a major enterprise signals a significant erosion of VMware's dominance in the virtualization market, potentially accelerating the adoption of alternative platforms like Proxmox and forcing Broadcom to reconsider its strategy. Tesco's new virtualization software is unnamed and incompatible with its existing Veeam and Zerto backup tools, creating data security migration challenges. The company is one of many customers reconsidering VMware after Broadcom's post-acquisition price hikes.

hackernews · Bender · Jun 17, 21:00 · [Discussion](https://news.ycombinator.com/item?id=48576838)

**Background**: Broadcom acquired VMware in November 2023 and soon after implemented significant price increases, changed licensing models from perpetual to subscription, and cut support for smaller customers. This has triggered a wave of migration to open-source alternatives like Proxmox, which offers similar functionality at lower cost. Tesco's move is one of the largest publicly disclosed migrations.

**Discussion**: Commenters broadly criticized Broadcom's business model as predatory, noting its history of acquiring firms, raising prices, and cutting services. Some highlighted that Proxmox is gaining traction as a viable alternative, while others pointed out migration challenges such as backup software incompatibility.

**Tags**: `#VMware`, `#Broadcom`, `#virtualization`, `#enterprise IT`, `#Tesco`

---

<a id="item-7"></a>
## [GLM-5.2 tops open-weights models on Artificial Analysis](https://artificialanalysis.ai/articles/glm-5-2-is-the-new-leading-open-weights-model-on-the-artificial-analysis-intelligence-index) ⭐️ 8.0/10

GLM-5.2, developed by Z.ai, has become the leading open-weights model on the Artificial Analysis intelligence index, approaching frontier performance at significantly lower pricing. This breakthrough challenges proprietary models from Anthropic, OpenAI, and Google, making high-quality AI more accessible and affordable for developers worldwide. The model is released under the MIT License and is designed for long-horizon tasks, though community reports indicate it can spend over 15 minutes reasoning on complex coding tasks.

hackernews · himata4113 · Jun 17, 09:12 · [Discussion](https://news.ycombinator.com/item?id=48567759)

**Background**: Z.ai (formerly Zhipu AI) is a Chinese AI company known as one of the 'AI tigers', and its GLM family of models has been open-sourced since July 2025. Artificial Analysis is an independent benchmarking platform that evaluates AI models on quality, price, speed, and latency. GLM-5.2 is the latest flagship model optimized for long-horizon reasoning tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GLM-5.2">GLM-5.2</a></li>
<li><a href="https://z.ai/blog/glm-5.2">GLM-5.2: Built for Long-Horizon Tasks</a></li>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>

</ul>
</details>

**Discussion**: Community responses are mixed: some users celebrate the model's low cost and high quality, calling it a 'huge blow' to proprietary vendors, while others criticize its reasoning inefficiency, noting that it took 15 minutes to complete a simple coding task. There is also discussion about the model's performance in coding benchmarks relative to competitors like GPT-5.5.

**Tags**: `#AI/ML`, `#open-weights`, `#LLM`, `#pricing`, `#reasoning`

---

<a id="item-8"></a>
## [Charity Majors: AI makes code generation free and disposable](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

Charity Majors argues that as of 2025, the economics of code production have reversed: generating code is now nearly free and instantaneous, turning lines of code from treasured assets into disposable commodities. This shift fundamentally changes software engineering practices and incentives, requiring more discipline rather than less, and has broad implications for how developers work and how software is built. The quote comes from Majors' article 'AI demands more engineering discipline. Not less,' published on Substack, highlighting that the change occurred 'practically overnight' in 2025.

rss · Simon Willison · Jun 17, 17:12

**Background**: Traditionally, writing code is labor-intensive, so code is carefully reused and maintained. AI-assisted programming tools like large language models (LLMs) can generate code on demand, drastically reducing the cost of creating new code.

**Tags**: `#ai-assisted-programming`, `#generative-ai`, `#software-engineering`, `#economics`, `#charity-majors`

---

<a id="item-9"></a>
## [China Expands STAR Market Listing Rules to AI and Hard Tech](https://mp.weixin.qq.com/s/ywLPXkSlqY9S5Vwp8G5saA) ⭐️ 8.0/10

CSRC Chairman Wu Qing announced at the 2026 Lujiazui Forum that the STAR Market's fifth set of listing standards will be expanded to cover AI, quantum technology, bio-manufacturing, and embodied intelligence, enabling more unprofitable hard-tech companies to go public. This policy shift signals strong government support for AI and other frontier technologies, providing critical capital access for early-stage, high-R&D companies. It could accelerate innovation and reshape China's tech ecosystem, particularly benefiting unprofitable AI startups seeking public funding. Wu Qing also vowed to crack down on fake tech hype and speculation, and will issue guidelines to regulate AI in capital markets. Additionally, the CSRC will introduce shelf offering reforms and four policies to support Shanghai's financial center construction.

telegram · zaihuapd · Jun 17, 08:30

**Background**: The STAR Market (科创板) was launched in 2019 to channel capital to hard-tech and innovative companies, with five sets of listing standards. The fifth set targets pre-revenue biotech firms with high market valuation expectations. Shelf offering (储架发行) allows issuers to register a securities offering in advance and sell portions over time, improving financing efficiency. Embodied intelligence (具身智能) refers to AI systems with physical bodies capable of interacting with the real world, seen as a key next step in AI development.

<details><summary>References</summary>
<ul>
<li><a href="http://zhoukan.cc/jujiao/2025/0626/062025_347582.html">每日热门： 第 五 套 标 准 正式重启 科 创 板 聚焦构建 创 新新生态_环球周刊网</a></li>
<li><a href="https://wallstreetcn.com/articles/3752510">科 创 板 “ 第 五 套 ”重启首单解析：泰诺麦博核心药品刚上市遇竞品“打5折”</a></li>
<li><a href="https://tubex.chat/zh/article/article-1775822504934-8c93c1">创业板深化改革：第四套标准+ 储 架 发 行 赋能新质生产力 - TubeX.Chat AI</a></li>

</ul>
</details>

**Tags**: `#AI`, `#regulation`, `#STAR Market`, `#China`, `#tech policy`

---

<a id="item-10"></a>
## [Anthropic tops OpenAI in enterprise AI market share for first time](https://techcrunch.com/2026/06/16/anthropics-latest-feud-with-the-trump-admin-may-actually-help-it-sales-data-suggests/) ⭐️ 8.0/10

According to Ramp data, Anthropic's enterprise AI subscription share reached 41% in May, surpassing OpenAI's 39.5% for the first time. This milestone indicates a major shift in the enterprise AI market, as Anthropic's focus on safety and compliance appears to resonate with businesses despite ongoing government tensions. The data comes from Ramp, an enterprise spend management platform, and the market share gain occurred while the Trump administration demanded Anthropic block non-US access to its latest models Mythos 5 and Fable 5.

telegram · zaihuapd · Jun 17, 09:30

**Background**: Anthropic is an AI company known for its focus on safe and ethical AI development. Its Claude Opus series is currently the main model used by enterprises. Ramp tracks software spending across companies, providing insights into market share trends. The conflict with the administration involved export control concerns over Anthropic's most advanced models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://ramp.com/enterprise">Enterprise Spend & Expense Management Software | Ramp</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Market Share`, `#Anthropic`, `#OpenAI`, `#Enterprise`

---

<a id="item-11"></a>
## [Microsoft Grows China AI Business via OpenAI Models](https://www.bloomberg.com/news/articles/2026-06-17/microsoft-s-china-ai-business-grows-on-openai-model-sales) ⭐️ 8.0/10

Microsoft's Azure business in China, which sells OpenAI models to Chinese tech companies, has grown rapidly, with ByteDance as its largest customer spending over $1 billion annually. Other major buyers include Ant Group, Meituan, and Tencent. This rapid growth has sparked concerns among U.S. officials and lawmakers about AI security and potential model distillation by Chinese firms. It highlights the geopolitical tensions in AI and Microsoft's delicate position as a bridge between OpenAI and China. OpenAI has privately complained that Microsoft did not sufficiently prevent Chinese companies from 'distilling' its models. Microsoft claims it only sells to mature enterprises, not individual developers, and that models are hosted on overseas data centers accessed via the internet.

telegram · zaihuapd · Jun 18, 01:06

**Background**: Model distillation is a technique where knowledge from a large, powerful AI model is transferred to a smaller, more efficient one, often for cost or deployment reasons. This process can be used legitimately but also raises intellectual property concerns when applied to proprietary models. The U.S.-China tech rivalry has intensified, with both sides wary of technology transfer and security risks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_distillation">Model distillation</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#OpenAI`, `#China`, `#AI models`, `#Azure`

---