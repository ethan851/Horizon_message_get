---
layout: default
title: "Horizon Summary: 2026-07-30 (EN)"
date: 2026-07-30
lang: en
---

> From 33 items, 13 important content pieces were selected

---

1. [Run Gemma 4 26B on any M-series Mac with just 2GB RAM](#item-1) ⭐️ 9.0/10
2. [Mitchell Hashimoto Launches Superlogical on Non-Profit Owned Ghostty](#item-2) ⭐️ 9.0/10
3. [Russia charges Telegram founder Durov with aiding terrorism, issues international warrant](#item-3) ⭐️ 9.0/10
4. [OpenAI offers free AI models to 100,000 researchers](#item-4) ⭐️ 9.0/10
5. [AI startups increasingly withhold research publications](#item-5) ⭐️ 8.0/10
6. [KOReader Enhances E-Ink Readers with Open-Source Software](#item-6) ⭐️ 8.0/10
7. [Kimi Releases K3-256k Model at Half Price with 256k Context](#item-7) ⭐️ 8.0/10
8. [AI firms recruit thousands of electricians and carpenters for data centers](#item-8) ⭐️ 8.0/10
9. [AI worms self-propagate through Copilot in Word documents](#item-9) ⭐️ 8.0/10
10. [Long Policy Documents Fail to Govern LLM Agents, Study Finds](#item-10) ⭐️ 8.0/10
11. [Darktable: Free Open-Source RAW Photo Editor Gains Traction](#item-11) ⭐️ 8.0/10
12. [Matthew Green: AI Cryptanalysis Could Validate or Undermine Post-Quantum Algorithms](#item-12) ⭐️ 8.0/10
13. [Report: Hugging Face widely used to generate deepfake nudes](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Run Gemma 4 26B on any M-series Mac with just 2GB RAM](https://github.com/drumih/turbo-fieldfare) ⭐️ 9.0/10

TurboFieldfare, a new open-source inference engine written in Swift and Metal, runs the 4-bit quantized Gemma 4 26B model on any M-series Mac using only ~2 GB of RAM by streaming routed experts from SSD. This breakthrough makes a powerful 26B-parameter model accessible on low-RAM Macs (8GB or 16GB) that previously could not load the full 14GB quantized weights, democratizing on-device AI for millions of users. The engine achieves 5–6 tok/s on an 8GB M2 MacBook Air and 31–35 tok/s on an M5 MacBook Pro, using a small expert cache and bounded parallel pread to mask SSD latency.

hackernews · gitpusher42 · Jul 29, 15:05 · [Discussion](https://news.ycombinator.com/item?id=49098510)

**Background**: Gemma 4 26B is a mixture-of-experts (MoE) model where only a subset of 'expert' layers are active per token, making it suitable for SSD streaming. Traditional inference loads all weights into RAM, but TurboFieldfare keeps only shared layers and KV cache in memory, fetching experts on demand from SSD. This technique builds on earlier work like Flash-MoE that demonstrated streaming large MoE models on consumer hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://gemma4.dev/docs/models">Model Reference | gemma 4 .dev — The Gemma 4 Developer Hub</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://insiderllm.com/guides/flash-moe-run-397b-model-laptop/">Flash-MoE: Run a 397B Model on a 48GB Laptop... | InsiderLLM</a></li>

</ul>
</details>

**Discussion**: The community was highly engaged, with users praising the engineering achievement and sharing real-world benchmarks. Some noted that llama.cpp with mmap can also run large models in limited RAM, but TurboFieldfare's synchronization of SSD reads with inference was seen as a key optimization. There was also a helpful tip for compiling on older macOS versions.

**Tags**: `#inference engine`, `#on-device AI`, `#Gemma`, `#Swift/Metal`, `#model streaming`

---

<a id="item-2"></a>
## [Mitchell Hashimoto Launches Superlogical on Non-Profit Owned Ghostty](https://www.superlogical.com/) ⭐️ 9.0/10

Mitchell Hashimoto announced Superlogical, a new company that builds on the open-source libghostty terminal library, with the core Ghostty project owned by a non-profit foundation. This novel business model separates the open-source core from a for-profit entity, potentially setting a precedent for sustainable open-source development while ensuring the terminal library remains community-owned. Superlogical will use libghostty as a public building block, consuming the same MIT-licensed components available to everyone, and will upstream shared terminal improvements so all libghostty consumers benefit.

hackernews · yan · Jul 29, 15:41 · [Discussion](https://news.ycombinator.com/item?id=49098965)

**Background**: Ghostty is a fast, feature-rich, cross-platform terminal emulator using platform-native UI and GPU acceleration. Its core library, libghostty, is designed for embedding terminal functionality in third-party projects. By transferring Ghostty ownership to a non-profit, Hashimoto ensures the foundational technology remains open and community-governed.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty-org/ghostty: 👻 Ghostty is a fast, feature-rich, and cross-platform terminal emulator that uses platform-native UI and GPU acceleration.</a></li>
<li><a href="https://mitchellh.com/writing/libghostty-is-coming">Libghostty Is Coming – Mitchell Hashimoto</a></li>
<li><a href="https://ghostty.org/">Ghostty</a></li>

</ul>
</details>

**Discussion**: Comments are largely positive, praising the non-profit ownership model and the commitment to upstream contributions. Some users draw parallels to OLE/COM, while a few criticize the enigmatic title of the announcement.

**Tags**: `#software-engineering`, `#open-source`, `#terminal`, `#startup`, `#ghostty`

---

<a id="item-3"></a>
## [Russia charges Telegram founder Durov with aiding terrorism, issues international warrant](https://www.interfax.ru/russia/1106228) ⭐️ 9.0/10

On July 29, Russia's Federal Security Service (FSB) opened a criminal case against Telegram founder Pavel Durov under Article 205.1, Part 1.1 of the Criminal Code (aiding terrorism) and placed him on an international wanted list. This escalation signals a major crackdown by Russian authorities on tech platforms, threatening free speech and privacy for millions of Telegram users in Russia and beyond, and could set a precedent for other governments to target platform executives. The FSB claims Telegram's management refused to delete channels, groups, and bots used by Ukrainian intelligence and terrorist/extremist organizations for planning sabotage, terrorist attacks, mass killings, and online fraud in Russia, causing casualties and billions of rubles in damages.

telegram · zaihuapd · Jul 29, 05:56

**Background**: Pavel Durov is the Russian-born founder of Telegram, a popular encrypted messaging app with over 900 million users worldwide. Telegram has faced pressure from multiple governments over content moderation, but this marks the first criminal terrorism-related charge against its founder personally by a state. Russia previously attempted to block Telegram in 2018 but later lifted the ban.

**Tags**: `#Telegram`, `#Pavel Durov`, `#Russia`, `#legal`, `#terrorism`

---

<a id="item-4"></a>
## [OpenAI offers free AI models to 100,000 researchers](https://openai.com/index/chatgpt-for-academic-researchers/) ⭐️ 9.0/10

On July 29, 2026, OpenAI announced the ChatGPT for Academic Researchers program, offering free access to its frontier GPT-5.6 models to up to 100,000 researchers globally by 2027, with an initial cohort of 10,000 opening this summer. This multi-million dollar initiative significantly lowers barriers for academic research, enabling large-scale AI-assisted studies in genomics, protein modeling, and more, potentially accelerating scientific breakthroughs. Researchers can use GPT-5.6 variants (Luna, Terra, Sol) and invite up to 4 collaborators; data in workspaces is not used for model training by default. The program is part of OpenAI's over $250 million commitment to external research through 2027.

telegram · zaihuapd · Jul 30, 00:17

**Background**: GPT-5.6 is a family of large language models released by OpenAI on July 9, 2026, with three variants: Luna, Terra, and Sol. The Sol variant, previewed in late July 2026, offers advanced capabilities in coding, science, and cybersecurity alongside enhanced safety measures. This initiative follows OpenAI's broader AI for Science push.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT-5.6 Sol: a next-generation model | OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI for Science`, `#Academic Research`, `#GPT-5.6`, `#Machine Learning`

---

<a id="item-5"></a>
## [AI startups increasingly withhold research publications](https://www.science.org/content/article/ai-s-top-startups-are-barely-publishing-their-research) ⭐️ 8.0/10

Top AI startups are barely publishing their research, shifting away from open science to protect competitive advantages, as reported by Science.org. This trend threatens transparency and reproducibility in AI, which are essential for scientific progress and public trust. The article notes that even OpenAI, which began with open research, has reduced publications; citations are used as an imperfect proxy for impact.

hackernews · YeGoblynQueenne · Jul 29, 21:25 · [Discussion](https://news.ycombinator.com/item?id=49103285)

**Background**: Historically, AI research thrived on open publication and collaboration. Startups now fear that publishing their work will allow competitors like OpenAI and Anthropic to copy their results, leaving them with no return on months of effort.

**Discussion**: Commenters shared personal experiences: one startup tried publishing for three years before giving up; another deliberately avoids publishing to prevent copying by larger players. Some criticized the 'blogification' of AI research, making claims harder to verify.

**Tags**: `#AI`, `#research publishing`, `#startups`, `#transparency`, `#HackerNews discussion`

---

<a id="item-6"></a>
## [KOReader Enhances E-Ink Readers with Open-Source Software](https://koreader.rocks/) ⭐️ 8.0/10

KOReader, an open-source ebook reader for e-ink devices, gained significant attention on Hacker News with a popular thread discussing its features and user experiences. The discussion underscores the growing interest in open-source software for e-readers, enabling users to extend the functionality and lifespan of devices like Kindle and Kobo. KOReader supports EPUB, PDF, MOBI, and other formats, and is compatible with Kindle, Kobo, PocketBook, Android, and Linux devices; however, some users report a non-intuitive UI and laggy gestures.

hackernews · Cider9986 · Jul 29, 11:05 · [Discussion](https://news.ycombinator.com/item?id=49095865)

**Background**: E-ink devices like Kindle and Kobo typically run proprietary software that limits customization. KOReader is a free, open-source application that can be installed on jailbroken Kindles or Kobo devices, offering advanced features such as native EPUB/PDF support, customizable gestures, and Calibre synchronization.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/KOReader">KOReader</a></li>
<li><a href="http://koreader.rocks/">KOReader</a></li>

</ul>
</details>

**Discussion**: The Hacker News community shows mixed sentiment: many users praise KOReader for enhancing their e-reader experience, while others criticize its non-intuitive UI, laggy gestures, and overall usability, comparing it to 'the GIMP of e-reader software'.

**Tags**: `#open-source`, `#e-reader`, `#software`, `#kindle`, `#kobo`

---

<a id="item-7"></a>
## [Kimi Releases K3-256k Model at Half Price with 256k Context](https://www.kimi.com/code/docs/en/kimi-code/models) ⭐️ 8.0/10

Kimi unveiled the K3-256k model, offering a 256k-token context window at half the API quota cost of its 1M-token K3 flagship, with the same intelligence within the shorter context. This pricing strategy makes long-context AI more accessible to developers and could pressure competitors to offer tiered pricing based on context length, while still preserving the 1M option for those who need it. The K3-256k model is separate from the 1M version; tools like Kimi Code CLI will automatically compact context if it exceeds 256k when switching. The model is not quantized—only the context window is reduced.

hackernews · monneyboi · Jul 29, 19:25 · [Discussion](https://news.ycombinator.com/item?id=49101852)

**Background**: In large language models, context length refers to the amount of text (in tokens) the model can process at once. Longer context increases computational cost because more tokens need attention. Kimi K3 is a flagship model with 1M-token context, and the 256k variant offers a cost-effective alternative for use cases that don't require full 1M context.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/code/docs/en/kimi-code/models">Model Configuration | Kimi Code Docs</a></li>
<li><a href="https://datanorth.ai/blog/context-length">LLM Context Length & Context Window Explained (2026)</a></li>
<li><a href="https://insiderllm.com/guides/context-length-explained/">Context Length Explained: Why It Eats Your VRAM | InsiderLLM</a></li>

</ul>
</details>

**Discussion**: Community members praised the half-price reduction as 'massive' and noted similarity to OpenAI's context-length pricing step. Some discussed the trade-off of hard cutoff versus smooth gradient, while others clarified it's an API-level change, not a quantized model, just a smaller context.

**Tags**: `#AI`, `#large language models`, `#pricing`, `#context length`, `#API`

---

<a id="item-8"></a>
## [AI firms recruit thousands of electricians and carpenters for data centers](https://www.nytimes.com/2026/07/29/business/economy/data-center-electricians-training.html) ⭐️ 8.0/10

Major AI companies are hiring thousands of electricians and carpenters to build data centers, reflecting a massive labor shift driven by AI infrastructure expansion. This trend highlights the growing demand for skilled tradespeople in AI infrastructure, which could reshape the labor market and training programs for construction trades. The article focuses on the recruitment of electricians and carpenters, but future data centers may also require plumbers due to increased use of liquid cooling systems.

hackernews · thm · Jul 29, 14:43 · [Discussion](https://news.ycombinator.com/item?id=49098198)

**Background**: Data centers are large facilities that house servers and networking equipment for cloud computing and AI. Building them requires specialized construction skills, including electrical wiring and carpentry. The boom in AI has led to a surge in data center construction, creating demand for tradespeople.

**Discussion**: Community comments express caution about the boom-bust nature of data center construction, noting that electricians could face volatile income. Others welcome the well-paying opportunities for tradespeople, and one commenter highlights the future need for plumbers due to liquid cooling trends.

**Tags**: `#AI infrastructure`, `#data centers`, `#labor market`, `#trades`, `#economy`

---

<a id="item-9"></a>
## [AI worms self-propagate through Copilot in Word documents](https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/) ⭐️ 8.0/10

Researcher Håkon Måløy demonstrated a prompt injection attack that turns Microsoft Copilot in Word into a self-replicating AI worm, allowing malicious instructions embedded in documents to spread to new files. This vulnerability exposes a critical security flaw in LLM-integrated applications, as AI agents given broad access can unknowingly execute and propagate hidden instructions, threatening data privacy and system integrity. The attack uses indirect prompt injection where adversarial prompts are hidden in shared documents, and Copilot's inability to distinguish instructions from data enables the worm to self-propagate with no robust mitigation currently available.

hackernews · Canopy9560 · Jul 29, 11:44 · [Discussion](https://news.ycombinator.com/item?id=49096188)

**Background**: AI worms are autonomous malware that exploit large language models and automation pipelines by injecting self-replicating prompts. Prompt injection attacks take advantage of LLMs' inability to distinguish between developer instructions, user inputs, and external content, allowing hidden commands to hijack outputs. As AI agents gain more access to user data and actions, such attacks become increasingly dangerous.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://www.sentinelone.com/cybersecurity-101/cybersecurity/ai-worms/">AI Worms Explained: Adaptive Malware Threats - SentinelOne</a></li>
<li><a href="https://www.emergentmind.com/topics/ai-worms">AI Worms: Autonomous Self-Propagating Malware</a></li>

</ul>
</details>

**Discussion**: Community members expressed concern that the vulnerability class may be unfixable without separating instructions from data, and warned that granting agents excessive access could lead to widespread exploitation, including theft of credentials or wallet data.

**Tags**: `#AI security`, `#prompt injection`, `#Copilot`, `#cybersecurity`, `#worms`

---

<a id="item-10"></a>
## [Long Policy Documents Fail to Govern LLM Agents, Study Finds](https://arxiv.org/abs/2607.25398) ⭐️ 8.0/10

A new study (Handbook.md) demonstrates that long policy documents—even when placed in the context window—fail to reliably govern the behavior of large language model agents, due to context window limitations and model attention deficiencies. This finding challenges the premise that lengthy instructions can effectively control AI agents, raising critical concerns for AI safety and deployment in sensitive domains where strict adherence to policies is required. The paper likely evaluates multiple LLMs on a benchmark where agents must follow a long policy document, finding that performance degrades sharply with document length, and that even state-of-the-art models fail to retain key instructions across extended interactions.

hackernews · spIrr · Jul 29, 13:01 · [Discussion](https://news.ycombinator.com/item?id=49096969)

**Background**: Large language models (LLMs) have limited effective context windows; while models claim support for millions of tokens, practical attention and quantization issues cause information loss from early parts of the input. Agentic AI systems that rely on long policy documents to guide behavior thus risk ignoring or forgetting critical safety constraints. Recent benchmarks like LongSafety and LongSafetyBench also highlight similar failures in long-context safety.

<details><summary>References</summary>
<ul>
<li><a href="https://aclanthology.org/2025.acl-long.1530.pdf">Evaluating Long-Context Safety of Large Language Models</a></li>
<li><a href="https://arxiv.org/html/2502.16971">LongSafety: Evaluating Long-Context Safety of Large Language Models</a></li>

</ul>
</details>

**Discussion**: Commenters generally agree with the findings, citing real-world experiences with models like Claude failing to follow persistent instructions. Some attribute the issue to quantization and poor samplers, while others note that even humans struggle with long policy documents. A recurring point is that effective agentic behavior requires dedicated post-training on specific handbooks.

**Tags**: `#LLM`, `#long context`, `#AI safety`, `#benchmarks`

---

<a id="item-11"></a>
## [Darktable: Free Open-Source RAW Photo Editor Gains Traction](https://www.darktable.org/) ⭐️ 8.0/10

A community discussion on Darktable highlights its impressive features, with many users praising its capability as a free alternative to paid software like Adobe Lightroom, though performance issues and workflow changes have drawn criticism. As an open-source RAW editor, Darktable demonstrates that free software can compete with industry-standard tools, potentially lowering the barrier for photographers and fostering more accessible photo editing workflows. Darktable is a non-destructive RAW developer focused on workflow efficiency, but some users report performance issues on modern hardware and have noted that transitioning between major versions can break existing edits.

hackernews · siatko · Jul 29, 12:33 · [Discussion](https://news.ycombinator.com/item?id=49096654)

**Background**: Darktable is a free and open-source photography application and raw developer released under the GPL-3.0 license. It serves as a virtual lighttable and darkroom for organizing and editing digital negatives, supporting major operating systems including Linux, macOS, Windows, and Solaris. Unlike raster editors like Photoshop, Darktable focuses on non-destructive raw image post-production, allowing photographers to manage large volumes of images efficiently. Some users find its learning curve steep and its workflow conventions different from commercial alternatives like Lightroom.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Darktable">Darktable</a></li>
<li><a href="https://www.darktable.org/">darktable</a></li>

</ul>
</details>

**Discussion**: The discussion is mixed: many users highly praise Darktable for its feature set and quality, with one user saying 'I would happily pay 200 bucks per year' for it, while others criticize its slow performance and disruptive workflow changes between versions. Some users note that Darktable's organizational capabilities are weaker than Lightroom, and an ex-maintainer fork called Ansel exists due to disagreements over the project's direction.

**Tags**: `#open-source`, `#photography`, `#photo-editing`, `#raw-processing`

---

<a id="item-12"></a>
## [Matthew Green: AI Cryptanalysis Could Validate or Undermine Post-Quantum Algorithms](https://simonwillison.net/2026/Jul/29/matthew-green/#atom-everything) ⭐️ 8.0/10

Matthew Green, a respected cryptographer, observed that the current migration to post-quantum cryptography presents an ideal opportunity for AI-driven cryptanalysis to either confirm the security of new algorithms or expose their weaknesses. As the world transitions from traditional public-key cryptography to post-quantum standards, AI's ability to analyze these novel problems could either build confidence in the new algorithms or reveal catastrophic flaws, directly impacting global security infrastructure. Green specifically mentioned HAWK, a lattice-based post-quantum signature scheme, as an example of the many standards currently under consideration. He also referenced Impagliazzo's 'Five Worlds' taxonomy, noting that if AI undermines all hard problems, we might end up in Minicrypt.

rss · Simon Willison · Jul 29, 18:18

**Background**: Post-quantum cryptography aims to develop algorithms resistant to quantum computers. NIST is standardizing new schemes like HAWK, which relies on lattice problems believed to be hard for both classical and quantum computers. AI cryptanalysis uses machine learning to find weaknesses in cryptographic algorithms.

<details><summary>References</summary>
<ul>
<li><a href="https://eprint.iacr.org/2026/1078">Post-Quantum HAWK Signature Acceleration with RISC-V-Based Hardware-Software Co-Design</a></li>
<li><a href="https://hawk-sign.info/">Hawk</a></li>
<li><a href="https://fanpu.io/blog/2022/impagliazzos-five-worlds/">Impagliazzo ' s Five Worlds, or The Computational... | Fan Pu Zeng</a></li>

</ul>
</details>

**Tags**: `#cryptography`, `#post-quantum cryptography`, `#AI`, `#cryptanalysis`, `#public-key algorithms`

---

<a id="item-13"></a>
## [Report: Hugging Face widely used to generate deepfake nudes](https://www.theverge.com/ai-artificial-intelligence/971723/hugging-face-nudify-deepfake-undress-women-children) ⭐️ 8.0/10

A report by the European nonprofit AI Forensics, released on July 28, finds that Hugging Face, an open-source model hosting platform, is heavily used to create non-consensual deepfake pornographic images, with seven of the top nine image editing models easily undressing women upon simple prompts. This report highlights critical safety gaps on a major AI platform, raising urgent questions about content moderation, legal responsibility, and the need for protective measures like prompt filtering and output scanning to prevent harm, especially to minors. The researchers set up a honeypot that received over 1,000 requests in 7 days, of which 73% were sexually explicit and nearly 7% targeted children, despite Hugging Face's policies banning non-consensual intimate content and child nudity.

telegram · zaihuapd · Jul 29, 08:20

**Background**: Hugging Face is a popular open-source platform where developers share machine learning models and datasets, including image generation models. Deepfakes use AI to create realistic but fake images or videos, often without consent. The report underscores that without adequate safeguards, such platforms can be misused for harmful purposes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face</a></li>
<li><a href="https://www.ibm.com/think/topics/hugging-face">What is Hugging Face? - IBM</a></li>

</ul>
</details>

**Tags**: `#AI ethics`, `#deepfake`, `#content moderation`, `#Hugging Face`, `#safety`

---