---
layout: default
title: "Horizon Summary: 2026-08-15 (EN)"
date: 2026-08-15
lang: en
---

> From 28 items, 12 important content pieces were selected

---

1. [Qwen Releases Qwen3.8-27B Open-Weight Model with Strong Reasoning and Laptop-Runnable Performance](#item-1) ⭐️ 9.0/10
2. [GLM-5.3: Frontier coding model with emergent cyber capabilities](#item-2) ⭐️ 9.0/10
3. [Going Dark and the Rise of Law Enforcement Hacking](#item-3) ⭐️ 8.0/10
4. [Opus 5 feels worse because post-training optimizes for agents, not humans](#item-4) ⭐️ 8.0/10
5. [Firefox becomes the last major browser supporting full uBlock Origin](#item-5) ⭐️ 8.0/10
6. [Satirical Site 'Every Fucking Website' Mocks Web Design Anti-Patterns](#item-6) ⭐️ 8.0/10
7. [Don't Classify, Hallucinate: Generate Tags, Then Match via Embeddings](#item-7) ⭐️ 8.0/10
8. [Vivodyne's AI robot labs test 3 million human tissues yearly, aiming to end animal testing.](#item-8) ⭐️ 8.0/10
9. [Xiaohongshu Open-Sources dots3-note: 280B MoE, 16B Active](#item-9) ⭐️ 8.0/10
10. [Apple Announces CEO Transition: Tim Cook to Step Down, John Ternus to Succeed](#item-10) ⭐️ 8.0/10
11. [PostgreSQL Critical to_char Flaw Allows Arbitrary Code Execution](#item-11) ⭐️ 8.0/10
12. [Apple Trains China-Specific AI Model with Alibaba, May Be First Foreign Approval](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Qwen Releases Qwen3.8-27B Open-Weight Model with Strong Reasoning and Laptop-Runnable Performance](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 9.0/10

Qwen released Qwen3.8-27B, a dense 27-billion-parameter open-weight vision-language model, on Hugging Face, alongside an FP8 quantized version. Built on the Qwen3.5 architecture, it supports a native 262K-token context window and configurable reasoning. This release is significant because a 27B open-weight model can run on a laptop while delivering strong reasoning, which lowers the barrier to local AI development and reduces dependence on hosted APIs. It also shows that non-US labs are quickly closing the gap with frontier closed models, increasing competitive pressure on the wider AI ecosystem. Qwen3.8-27B is a dense vision-language model built for coding, professional work, research, and long-horizon agentic tasks, with stronger autonomous planning and environment-feedback handling. Community tests show it runs locally in llama.cpp, but one RTX 5090 user measured roughly 138 tokens per second with the ninfer engine, about double the speed of a naive llama.cpp setup.

hackernews · erdaltoprak · Aug 14, 15:00 · [Discussion](https://news.ycombinator.com/item?id=49299605)

**Background**: Open-weight models make the trained neural network weights publicly available, so developers can self-host, fine-tune, and adapt them, but they usually do not release the training data or full training code. Qwen is Alibaba's family of large language and multimodal models, and Qwen3.8-27B is a vision-language model that can process both text and images. Its 'thinking' mode can be toggled to trade speed for more step-by-step reasoning, and the 262K-token context window lets it ingest very long documents or multi-image inputs in a single pass.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://lmstudio.ai/models/qwen3.8">Qwen3.8 - lmstudio.ai</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>

</ul>
</details>

**Discussion**: Hacker News reaction was very positive: one commenter called it 'absolutely the best pelican I've seen from a model that runs on my laptop,' while another said it was the second local model after Gemma 4 to correctly pass one of their private reasoning benchmarks. Other users pointed out that its thinking trace uses clipped, note-like language that may reduce MTP prediction quality, and that VRAM usage appeared less efficient than Gemma 4 or Glimmer. One developer reported the ninfer engine delivered roughly 138 tokens/s on an RTX 5090, about double the speed of a naive llama.cpp setup.

**Tags**: `#LLM`, `#Open Source`, `#Qwen`, `#Local AI`, `#Model Release`

---

<a id="item-2"></a>
## [GLM-5.3: Frontier coding model with emergent cyber capabilities](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

Z.ai has released GLM-5.3, a new flagship model post-trained from the GLM-5.2 base that delivers major advances in complex software engineering, agent tasks, and security research. The release highlights emergent cyber capabilities, including autonomous vulnerability discovery and exploit adaptation, alongside three thinking effort levels and a 1M context window. This release signals a new phase in frontier AI where coding models are increasingly capable of autonomous security work, with users reporting real 0-day discovery and exploitation scenarios. It intensifies debates about the trade-offs between open-weight model benefits and potential misuse, while also shifting the competitive landscape against OpenAI and Anthropic. GLM-5.3 uses the same base model as GLM-5.2, with all improvements coming from post-training, and is offered in three thinking effort levels with a 1M-token context. Z.ai has also set up a coordinated vulnerability disclosure page (cvd.z.ai) that appears to reflect large-scale scanning of open-source software, with many CVEs still under embargo.

hackernews · pella · Aug 14, 05:19 · [Discussion](https://news.ycombinator.com/item?id=49294997)

**Background**: GLM-5.3 is Z.ai's flagship model in the GLM series, a family of large language models developed by Zhipu AI. Emergent abilities in LLMs are capabilities that appear suddenly and unpredictably as models scale up, and this release marks one of the first times such abilities are explicitly tied to cybersecurity in a commercial coding model. Frontier coding models are advanced AI systems that use large-context reasoning to understand source files, dependencies, and complex coding tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM - 5 . 3 - Overview - Z. AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.together.ai/models/glm-5-3">GLM - 5 . 3 API: Pricing, Benchmarks & Docs | Together AI</a></li>
<li><a href="https://arxiv.org/abs/2206.07682">[2206.07682] Emergent Abilities of Large Language Models</a></li>

</ul>
</details>

**Discussion**: Community reaction is largely positive but mixed with caution. Users report impressive real-world results, such as a $18 subscription being upgraded to $80 after the model seamlessly executed a red-team scenario with WordPress plugin 0-days and kernel exploits; others note it is still slightly behind competitors like Claude Sonnet and Fable, and question the escalating cost of large-scale vulnerability scanning.

**Tags**: `#AI`, `#LLM`, `#cybersecurity`, `#coding`, `#model release`

---

<a id="item-3"></a>
## [Going Dark and the Rise of Law Enforcement Hacking](https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/) ⭐️ 8.0/10

This blog post from August 14, 2026 examines the 'going dark' debate and argues that law enforcement hacking has become the central workaround for encrypted communications. It contends that the era of simply demanding backdoors is giving way to exploiting software vulnerabilities and deploying network investigative techniques. The outcome of this debate shapes encryption policy, affecting billions of users' privacy and security. As law enforcement increasingly turns to hacking rather than legal backdoors, the reliability of end-to-end encryption and the rules for state-sponsored intrusion demand public scrutiny. The analysis notes a likely ceiling on the number of useful software bugs, which would limit hack-based access over time. It also highlights that law enforcement hacking often depends on secrecy, deception, and vulnerability stockpiling, raising oversight and disclosure concerns.

hackernews · vslira · Aug 14, 20:52 · [Discussion](https://news.ycombinator.com/item?id=49304447)

**Background**: The 'going dark' problem refers to a situation where the government has lawful authority to search a device or communication but lacks the technical means because of strong encryption. Law enforcement hacking, also called network investigative techniques (NITs), uses keyloggers, exploits, or other means to access devices before encryption is applied. U.S. policy and legal frameworks have struggled to keep pace, as shown by disputes like the Apple/FBI case.

<details><summary>References</summary>
<ul>
<li><a href="https://www.csis.org/blogs/strategic-technologies-blog/encryption-and-going-dark-cutting-through-gordian-knot">Encryption and Going Dark – Cutting through the Gordian Knot | CSIS</a></li>
<li><a href="https://www.congress.gov/crs-product/R44827">Law Enforcement Using and Disclosing Technology Vulnerabilities | Congress.gov | Library of Congress</a></li>
<li><a href="https://www.justsecurity.org/60785/shining-light-federal-law-enforcements-computer-hacking-tools/">Shining a Light on Federal Law Enforcement’s Use of Computer Hacking Tools</a></li>

</ul>
</details>

**Discussion**: Commenters were engaged and divided. Animats provided historical context on physical wiretapping costs, while mbroshi disagreed with the post's claim that the supply of useful bugs will soon plateau. fitblipper mocked the 'going dark' label given the ubiquity of surveillance cameras and metadata sharing, and Insimwytim contrasted sophisticated attacks with ordinary security failures.

**Tags**: `#cryptography`, `#law enforcement`, `#encryption`, `#surveillance`, `#security`

---

<a id="item-4"></a>
## [Opus 5 feels worse because post-training optimizes for agents, not humans](https://mun-logadan.github.io/why-does-opus-5-feel-worse/) ⭐️ 8.0/10

A new essay argues that Anthropic's Claude Opus 5, released on July 24, 2026, feels worse to work with because its post-training prioritizes agent-to-agent communication, yielding elliptical, abstract prose that exhausts human readers. The author contends the model's output is optimized for other AI agents rather than for people. This critique highlights a potential shift in frontier-model development: as models are increasingly benchmarked on agentic tasks, human readability and conversational UX may be deprioritized. Developers and everyday users could face hidden productivity costs from interacting with models whose writing style is optimized for machines. The article specifically calls out elliptical sentences that orbit a point, overly abstract phrasing, and inanimate nouns as sentence subjects used to create a 'surprise' reveal at the end. Community reports also note the model's frequent self-confessions and verbose 'honesty' as part of the exhausting style.

hackernews · numeri · Aug 14, 10:12 · [Discussion](https://news.ycombinator.com/item?id=49296740)

**Background**: Post-training refers to the phase after an LLM's initial pre-training, which includes techniques like RLHF, instruction tuning, and reasoning fine-tuning to shape behavior toward desired objectives. When those objectives emphasize autonomous agent task completion—such as coding, research, or multi-step tool use—models may internalize communication patterns suited to other agents, not human interaction. Claude Opus 5 was launched as a strong agentic coding model at half the price of Claude Fable 5, reflecting Anthropic's focus on agentic performance.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-opus-5">Introducing Claude Opus 5 \ Anthropic</a></li>
<li><a href="https://benchlm.ai/models/claude-opus-5">Claude Opus 5 Benchmarks, Pricing & Speed (August 2026)</a></li>
<li><a href="https://rlhfbook.com/">Reinforcement Learning from Human Feedback and LLM Post - Training</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with the article's thesis: one user found Opus 5's elliptical and jumpy writing annoying, while another burned through credits and switched to OpenAI's Sol because Opus 5's 'being honest' confessions were exhausting. A recurring speculation was that humans are no longer the target audience of post-training, and at least one user reverted to Opus 4.8, claiming quality has clearly declined.

**Tags**: `#AI`, `#language models`, `#UX`, `#agent communication`, `#model behavior`

---

<a id="item-5"></a>
## [Firefox becomes the last major browser supporting full uBlock Origin](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 8.0/10

With Chrome's rollout of Manifest V3, the full version of uBlock Origin no longer works in Chromium-based browsers, leaving Firefox as the only major browser that still fully supports it. uBlock Origin is widely regarded as the gold-standard ad blocker, so its loss on Chrome weakens user control over ads and trackers. This reinforces Firefox's position as the go-to browser for privacy-conscious users and signals a broader shift in browser extension capabilities. Chrome's Manifest V3 replaces the blocking webRequest API with the declarativeNetRequest API, which limits the number of filter rules and lacks the dynamic filtering capabilities of uBlock Origin. An unofficial port, uBlock-mv3, attempts to bring the full version to MV3 but faces significant restrictions.

hackernews · DemiGuru · Aug 14, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49303202)

**Background**: Manifest V3 is Google's latest extension platform, introduced in 2020, ostensibly to improve privacy, security, and performance, but it restricts the webRequestBlocking permission to enterprise-managed extensions. uBlock Origin is a popular open-source content blocker that relies on the powerful webRequest API to block ads and trackers in real time. Chrome, Edge, and other Chromium browsers are migrating to MV3, forcing ad blockers to use the less-capable declarativeNetRequest API. Firefox has extended support for background scripts and continues to support Manifest V2, allowing uBlock Origin to keep working.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V 3 | Chrome for Developers</a></li>
<li><a href="https://adblock-tester.com/ad-blockers/manifest-v3-ad-blocker-impact/">The Manifest V3 Changes — Did Google Just Break Your Ad Blocker? (And What to Do Next) - AdBlock Tester</a></li>
<li><a href="https://extensionworkshop.com/documentation/develop/manifest-v3-migration-guide/">Manifest V 3 migration guide | Firefox Extension Workshop</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised Firefox for vetting uBlock Origin's updates and supporting its full functionality, while criticizing Google's MV3 changes as anti-user. Some pointed to an unofficial MV3 port (uBlock-mv3) and discussed the Lite version's ad-blocking quality, and one developer said they shut down their extensions because MV3 made them useless.

**Tags**: `#Firefox`, `#uBlock Origin`, `#Manifest V3`, `#Ad-blocking`, `#Browser Extensions`

---

<a id="item-6"></a>
## [Satirical Site 'Every Fucking Website' Mocks Web Design Anti-Patterns](https://lxe.github.io/everywebsite/) ⭐️ 8.0/10

A satirical website, 'Every Fucking Website' (2020), parodies modern web design anti-patterns like aggressive pop-ups, cookie banners, and autoplaying videos. The site went viral on Hacker News, drawing hundreds of comments and a score of 8.0/10. The satire highlights how intrusive and widespread these UX dark patterns have become, prompting a broader conversation about their impact on user trust and browsing experience. For web developers and designers, the discussion underscores the tension between conversion optimization and user respect. The site is hosted at lxe.github.io and, according to one commenter, loads JavaScript only from its own domain—unlike typical sites that pull from 12-18 external domains. Commenters also noted missing anti-patterns such as 'better in the app' prompts, fake purchase notifications, and mandatory account login pop-ups.

hackernews · doubletwoyou · Aug 14, 14:31 · [Discussion](https://news.ycombinator.com/item?id=49299222)

**Background**: This self-referential satire works by recreating the most frustrating parts of the modern web experience. Users increasingly face cookie banners, newsletter pop-ups, and persistent tracking prompts that obstruct content. The website mirrors these patterns to offer a pointed critique of current web design trends, and the viral response shows that many users share the sentiment.

**Discussion**: Commenters reacted with humor and recognition, sharing their own experiences with dark patterns. Some admitted that techniques like 'someone bought X' alerts genuinely boost conversion rates in e-commerce, even at the cost of 'mild self-loathing.' Others joked about the site being too fast, lacking cross-domain tracking, or needing a Google login pop-up.

**Tags**: `#web-design`, `#ux`, `#satire`, `#web-development`, `#community-discussion`

---

<a id="item-7"></a>
## [Don't Classify, Hallucinate: Generate Tags, Then Match via Embeddings](https://simonwillison.net/2026/Aug/14/dont-classify-hallucinate/) ⭐️ 8.0/10

Simon Willison highlights Doug Turnbull's technique for tagging content with large vocabularies: instead of forcing an LLM to choose from thousands of existing tags, let it hallucinate plausible tags and then use vector embeddings to map those to the nearest real tags. Willison plans to apply this method to the 1,856 untagged older posts on his blog. This matters because LLM classification becomes impractical when the label set is enormous and exceeds context limits, a common problem in real-world content tagging and e-commerce. The technique offers a scalable, zero-shot alternative by decoupling generation from a fixed vocabulary, and it is easy to implement with existing embedding models. The example prompt from Doug Turnbull instructs the model to create novel furniture/home goods classifications and provides examples of the tag shape, such as "Furniture / Living Room Furniture / Coffee Tables & End Tables / Coffee Tables", then asks for classifications for a query like "brown coffee table". After generation, the hallucinated tags are embedded and matched to the nearest existing tags via vector similarity search, a technique conceptually similar to HyDE (Hypothetical Document Embeddings).

rss · Simon Willison · Aug 14, 21:54

**Background**: Vector embeddings represent words, sentences, or documents as dense numeric vectors that encode semantic meaning, so similar items are close together in vector space. Vector similarity search (nearest neighbor search) finds items most similar to a query vector, and is widely used in search and RAG systems. HyDE is a related retrieval technique that generates a hypothetical document for a query and uses its embedding to improve retrieval when relevant documents are scarce. These concepts underpin the idea of generating unconstrained tags and then mapping them to a known vocabulary.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vector_embedding">Vector embedding</a></li>
<li><a href="https://www.geeksforgeeks.org/data-science/hypothetical-document-embeddings-hyde-hyde/">Introduction to Hypothetical Document Embeddings (HyDE)</a></li>
<li><a href="https://docs.opensearch.org/latest/vector-search/getting-started/vector-search-basics/">Vector search basics | OpenSearch Documentation</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#embeddings`, `#tagging`, `#vector search`, `#AI`

---

<a id="item-8"></a>
## [Vivodyne's AI robot labs test 3 million human tissues yearly, aiming to end animal testing.](https://www.fastcompany.com/91589344/the-worlds-largest-biological-datacenter-could-help-make-animal-testing-obsolete) ⭐️ 8.0/10

Vivodyne has 12 'hive' robotic laboratories south of San Francisco that use AI-designed experiments to conduct controlled trials on more than 3 million lab-grown human tissue samples per year. This capacity is about twice the total volume of all clinical trials in the United States. This could dramatically accelerate drug discovery and reduce reliance on animal testing, given that about 90% of clinical trials fail even after passing animal tests. If successful, it may lead to safer and more effective medicines reaching patients much faster. Each lab is described as being 'closet-sized,' and the combined capacity is twice that of all U.S. clinical trials. The platform combines lab-grown 3D human tissues with AI-driven experimental design to generate human data at scale.

telegram · zaihuapd · Aug 14, 01:48

**Background**: Lab-grown 3D human tissues, often called organoids, mimic human organs more realistically than animal models and are increasingly used for drug testing. Traditional preclinical testing still relies heavily on animal models, which often fail to predict human responses, contributing to high clinical trial failure rates. AI-driven experimental design uses algorithms to automatically plan and optimize high-throughput experiments, enabling far larger and faster screening. Vivodyne's system brings these trends together to generate human data at an unprecedented scale.

<details><summary>References</summary>
<ul>
<li><a href="https://www.vivodyne.com/">Vivodyne | Make biology computable</a></li>
<li><a href="https://www.hsci.harvard.edu/organoids">hsci.harvard.edu/ organoids</a></li>
<li><a href="https://www.mdpi.com/2076-3417/15/9/5208">A Helping Hand: A Survey About AI-Driven Experimental Design ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#drug discovery`, `#biotech`, `#animal testing`, `#robotics`

---

<a id="item-9"></a>
## [Xiaohongshu Open-Sources dots3-note: 280B MoE, 16B Active](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

Xiaohongshu's Dots Lab open-sourced dots3-note preview, the first open-weight model in the dots3 family. It is a 280B-parameter Mixture-of-Experts model with 16B active parameters, supporting a 512K-token context and text, image, video, and audio inputs. This release gives the AI community access to a large multimodal MoE model with low inference cost, potentially boosting open-source agent research. It also introduces TEMPO, a new reinforcement learning method, and two real-world agent benchmarks, raising the bar for long-horizon task evaluation. The model is released with Apache 2.0 weights on Hugging Face, and GitHub provides an eight-GPU serving guide. The associated VibeSearchBench and VibeLifeBench benchmarks target realistic, harder-to-evaluate long-horizon agent scenarios.

telegram · zaihuapd · Aug 14, 08:27

**Background**: Mixture-of-Experts models activate only a subset of parameters per token, allowing large total parameter counts with lower compute. Xiaohongshu's dots3-note continues a trend of open-sourcing big MoE models; TEMPO is introduced as a reinforcement learning method that uses self-critique and test-time value estimation to train long-horizon agents.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/studio-dots-ai/dots3-note-prev">GitHub - studio-dots-ai/dots3-note-prev: dots3 note preview</a></li>
<li><a href="https://eu.36kr.com/en/p/3938759517896072">Xiaohongshu Open-Sourced Dots3-Note: The Same-Series Model ...</a></li>
<li><a href="https://vibebench.github.io/VibeLifeBench_homepage/">VibeLifeBench — Can Your Life Agent Be Proactive and Persistent in...</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#MoE`, `#reinforcement-learning`, `#multimodal`, `#agent-benchmark`

---

<a id="item-10"></a>
## [Apple Announces CEO Transition: Tim Cook to Step Down, John Ternus to Succeed](https://t.me/zaihuapd/43191) ⭐️ 8.0/10

Apple announced a leadership transition: Tim Cook will step down as CEO and become executive chairman of the board, while hardware engineering senior vice president John Ternus will take over as CEO on September 1, 2026. The board has unanimously approved the arrangement. This marks the first CEO change at Apple since 2011, when Tim Cook succeeded Steve Jobs, making it a historic moment for the tech industry. Ternus's appointment signals continuity, given his long tenure overseeing Apple's core hardware products such as iPhone, Mac, iPad, and AirPods. Per the plan, current chairman Arthur Levinson will transition to lead independent director on September 1, the same day Ternus joins the board. Ternus joined Apple in 2001, was promoted to vice president of hardware engineering in 2013, and entered the executive team in 2021.

telegram · zaihuapd · Aug 14, 11:00

**Background**: Tim Cook has served as Apple's CEO since 2011, succeeding Steve Jobs, and has led the company to become one of the world's most valuable enterprises. This transition is a carefully planned succession, with Cook staying on as executive chairman to ensure continuity. John Ternus has been a key figure behind Apple's hardware lineup, making him a natural successor. The executive chairman role focuses on strategy and board governance, distinct from the CEO's day-to-day operations.

**Tags**: `#Apple`, `#CEO Transition`, `#Tech Industry`, `#Leadership`, `#Tim Cook`

---

<a id="item-11"></a>
## [PostgreSQL Critical to_char Flaw Allows Arbitrary Code Execution](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL disclosed critical vulnerability CVE-2026-14669, a heap buffer overflow in the to_char(timestamptz) function triggered by overly long POSIX time zone abbreviations. This flaw lets low-privileged database users execute arbitrary code with the OS privileges of the PostgreSQL server process. With a CVSS score of 8.8, this vulnerability is highly severe and demands immediate patching. Because affected versions span multiple supported release lines, many production databases are exposed, and admins should apply the minor updates as soon as possible to prevent potential system compromise. Affected versions are those before 18.5, 17.11, 16.15, 15.19, and 14.24. Since 18.5 was not formally released due to a regression, users on the 18 series should upgrade to 18.6; other series should upgrade to 17.11, 16.15, 15.19, or 14.24. The patch requires only a program file replacement and service restart, not a dump/reload or pg_upgrade.

telegram · zaihuapd · Aug 14, 14:35

**Background**: PostgreSQL's to_char() function converts timestamps, numbers, and other values into formatted strings. The timestamptz data type (timestamp with time zone) stores timestamps along with time zone information. POSIX time zone abbreviations are short strings like "EST" that reference time zones; processing extremely long or malformed abbreviations in the format function can overflow a heap buffer. Proper patching and understanding of the upgrade path is critical for database security.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/functions-formatting.html">PostgreSQL: Documentation: 18: 9.8. Data Type Formatting Functions</a></li>
<li><a href="https://www.postgresql.org/docs/current/datatype-datetime.html">PostgreSQL: Documentation: 18: 8.5. Date/Time Types</a></li>

</ul>
</details>

**Tags**: `#PostgreSQL`, `#CVE`, `#security`, `#vulnerability`, `#to_char`

---

<a id="item-12"></a>
## [Apple Trains China-Specific AI Model with Alibaba, May Be First Foreign Approval](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 8.0/10

Apple is training a dedicated large language model for the Chinese market with Alibaba's support, abandoning its previous reliance on third-party models. Apple Intelligence is expected to launch in China with an iOS update in the coming months, and the Cyberspace Administration of China has already filed its generative AI service. If approved, Apple would become the first foreign company authorized by Beijing to offer its own proprietary AI model in China. This marks a significant strategic move with major implications for AI regulation, market competition, and Apple's positioning in the Chinese smartphone and AI ecosystem. The China-specific model is being developed in-house with Alibaba's computational support, replacing the previous approach of integrating third-party AI partners. The Cyberspace Administration of China registered the generative AI service last month, and the rollout is slated for the next few months via iOS updates.

telegram · zaihuapd · Aug 14, 14:47

**Background**: China requires all public-facing generative AI services to complete a filing process with the Cyberspace Administration of China, covering self-developed, fine-tuned, and third-party models. As of June 2025, 439 generative AI services had completed this filing. The regulatory framework is defined by the Interim Measures for Generative AI Services Management and related technical requirements, which mandate materials on model safety, data handling, and algorithm transparency.

<details><summary>References</summary>
<ul>
<li><a href="https://cloud.tencent.com/developer/article/2541787">生成式人工智能服务上线备案（大模型备案）材料清单详解-腾讯云开发者...</a></li>
<li><a href="https://developer.aliyun.com/article/1674963">生成式人工智能服务上线备案（大模型备案）材料清单详解</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1919326896111489390">生成式人工智能服务大模型备案申请全流程及核心要求 - 知乎</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#AI`, `#China`, `#Alibaba`, `#Regulation`

---