---
layout: default
title: "Horizon Summary: 2026-07-09 (EN)"
date: 2026-07-09
lang: en
---

> From 33 items, 14 important content pieces were selected

---

1. [OpenAI Launches GPT-Live Voice Assistant with GPT-5.5 Delegation](#item-1) ⭐️ 9.0/10
2. [TypeScript 7.0 Announced with Go-Powered 10x Speed Boost](#item-2) ⭐️ 9.0/10
3. [Bun Rewritten in Rust Using AI Agents](#item-3) ⭐️ 9.0/10
4. [Critical Android Remote Root Exploit Chain Exposed](#item-4) ⭐️ 9.0/10
5. [John Deere owners win right-to-repair in FTC settlement](#item-5) ⭐️ 8.0/10
6. [Mistral's Robostral Navigate: Map-less Robotics Navigation](#item-6) ⭐️ 8.0/10
7. [xAI Releases Grok 4.5 with Improved Efficiency](#item-7) ⭐️ 8.0/10
8. [Decoding a Uniqlo T-Shirt's Obfuscated Bash Script](#item-8) ⭐️ 8.0/10
9. [Cloudflare Meerkat: Global Asynchronous Consensus](#item-9) ⭐️ 8.0/10
10. [Alibaba Orders Employees to Uninstall Claude by July 10](#item-10) ⭐️ 8.0/10
11. [Huawei 5G flagship returns overseas with 1100 Mbps peak speed](#item-11) ⭐️ 8.0/10
12. [Meituan's OWL Model Suspected of Session Data Leak on OpenRouter](#item-12) ⭐️ 8.0/10
13. [Researchers identify apps via leaked EM signals with 99% accuracy](#item-13) ⭐️ 8.0/10
14. [LineageOS Introduces Web-Based Flashing Tool](#item-14) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Launches GPT-Live Voice Assistant with GPT-5.5 Delegation](https://openai.com/index/introducing-gpt-live/) ⭐️ 9.0/10

OpenAI launched GPT-Live, a new voice model powering ChatGPT Voice that enables real-time, natural conversations and can delegate complex queries to GPT-5.5 in the background. GPT-Live bridges the gap between voice interaction and cutting-edge AI capabilities, allowing users to have fluid voice conversations while accessing GPT-5.5's advanced reasoning for tasks like coding and research. The model is available in ChatGPT Voice and a sign-up page for API access has been posted. Early users report long, productive conversations but note the lack of tool/connector integration during voice mode.

hackernews · logickkk1 · Jul 8, 17:03 · [Discussion](https://news.ycombinator.com/item?id=48834405)

**Background**: GPT-Live is a real-time voice assistant model from OpenAI that supports natural conversation and can delegate tasks to GPT-5.5, a large language model released in April 2026 with strong benchmarks in coding and math. Previous voice assistants often used older models, limiting their capabilities. GPT-Live aims to combine the convenience of speech with the power of frontier AI.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/introducing-gpt-live/">Introducing GPT-Live | OpenAI</a></li>
<li><a href="https://openai.com/index/introducing-gpt-5-5/">Introducing GPT‑5.5 - OpenAI</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some users are impressed by the natural conversation and delegation feature, while others express concern that AI voice assistants may further reduce human connection. A notable critique is the inability to use tools or connectors during voice mode, which limits productivity use cases.

**Tags**: `#AI`, `#Voice Assistant`, `#GPT`, `#OpenAI`, `#Natural Language Processing`

---

<a id="item-2"></a>
## [TypeScript 7.0 Announced with Go-Powered 10x Speed Boost](https://devblogs.microsoft.com/typescript/announcing-typescript-7-0/) ⭐️ 9.0/10

Microsoft announced TypeScript 7.0, featuring a complete port of the TypeScript compiler from JavaScript to Go, achieving up to 11.9x speedups on large codebases like VS Code. This dramatic performance improvement makes TypeScript significantly faster for large projects, reducing build times and improving developer productivity across the ecosystem. The compiler rewrite to Go results in 8-12x speedups on real-world codebases, as shown by Microsoft's benchmarks; the Go port maintains full compatibility with existing TypeScript code.

hackernews · DanRosenwasser · Jul 8, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48833715)

**Background**: TypeScript is a typed superset of JavaScript that compiles to plain JavaScript. Its original compiler was written in JavaScript/TypeScript itself, which became a bottleneck for large codebases. Go is a compiled language known for its performance and efficient concurrency, making it a suitable choice for a high-performance compiler.

<details><summary>References</summary>
<ul>
<li><a href="https://www.architecture-weekly.com/p/typescript-migrates-to-go-whats-really">TypeScript Migrates to Go: What's Really Behind That 10x Performance Claim?</a></li>
<li><a href="https://visualstudiomagazine.com/articles/2025/03/11/microsoft-ports-typescript-to-go-for-10x-native-performance-gains.aspx">Microsoft Ports TypeScript to Go for 10x Native Performance Gains -- Visual Studio Magazine</a></li>
<li><a href="https://www.reddit.com/r/ProgrammingLanguages/comments/1j9osva/typescript_compiler_is_being_ported_to_go/">r/ProgrammingLanguages on Reddit: TypeScript compiler is being ported to Go</a></li>

</ul>
</details>

**Discussion**: The community reacted positively, with users posting impressive speedup numbers and praising the team for maintaining two codebases. Some speculated about future Rust rewrites, while others expressed relief at finally having a fast TypeScript compiler.

**Tags**: `#TypeScript`, `#performance`, `#compiler`, `#Microsoft`, `#software-engineering`

---

<a id="item-3"></a>
## [Bun Rewritten in Rust Using AI Agents](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust/#atom-everything) ⭐️ 9.0/10

Bun's creator Jarred Sumner announced a complete rewrite of the JavaScript runtime from Zig to Rust, completed in 11 days using AI coding agents and a TypeScript conformance suite. This rewrite demonstrates that large-scale, agentic-driven codebase rewrites are now feasible, potentially changing how software engineering projects approach foundational language shifts. It also provides Rust a significant win for systems-level runtime development. The estimated token cost was $165,000 at API pricing, but was free for Bun as part of Anthropic. The Rust version achieved 10% faster startup on Linux, improved stability, and reduced binary size by 20%.

rss · Simon Willison · Jul 8, 23:57

**Background**: Bun is a fast all-in-one JavaScript runtime and toolkit that includes a bundler, transpiler, and package manager. It was originally written in Zig, a low-level systems language requiring manual memory management. The rewrite to Rust was driven by persistent memory safety bugs like use-after-free and double-free errors, which Rust's ownership model prevents at compile time.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://bun.com/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the rewrite highlights Zig's memory safety shortcomings and the power of a strong test suite for LLM-driven rewrites. Some praised the discipline and human oversight shown, while others questioned the $165k cost comparison, noting it was subsidized by Anthropic.

**Tags**: `#Bun`, `#Rust`, `#Zig`, `#JavaScript runtime`, `#systems engineering`

---

<a id="item-4"></a>
## [Critical Android Remote Root Exploit Chain Exposed](https://www.coolapk.com/feed/72700258?s=ZGQ2MTVlZjYxMDYyNTM3ZzZhNGUzOThjega1640) ⭐️ 9.0/10

On July 8, 2026, cybersecurity firm Nebula disclosed a remote root exploit chain affecting all Android versions up to Android 17, combining a Firefox browser vulnerability (up to version 151.0.2) and a 15-year-old Linux kernel flaw (CVE-2026-43499, GhostLock). This exploit chain allows attackers to gain persistent root access on any Android device by simply tricking users into clicking a malicious link, posing an unprecedented security risk to billions of devices worldwide. The proof-of-concept code has been uploaded to GitHub, and while full details are withheld, the exploit combines a same-origin policy bypass in Firefox (CVE-2026-8971) with the GhostLock kernel bug (use-after-free in rt_mutex). The Linux kernel has already been patched, but Android vendors must still distribute updates.

telegram · zaihuapd · Jul 8, 13:01

**Background**: A remote root exploit chain allows an attacker to take complete control of a device without physical access, often by chaining multiple vulnerabilities. GhostLock (CVE-2026-43499) is a use-after-free bug in the Linux kernel's real-time mutex (rtmutex) subsystem, introduced in 2011 and patched in April 2026. The Firefox vulnerability (CVE-2026-8971) is a same-origin policy bypass in JAR protocol handling, enabling arbitrary code execution from a malicious website.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/15-year-old-ghostlock-flaw-enables-root.html">15-Year-Old GhostLock Flaw Enables Root and Container Escape on Most Linux Distros</a></li>
<li><a href="https://threat-modeling.com/cve-2026-43499-ghostlock-linux-kernel-root-container-escape/">CVE-2026-43499 "GhostLock": 15-Year-Old Linux Kernel Flaw Gives Local Users Root Access and Container Escape — Public PoC Released - Threat-Modeling.com</a></li>
<li><a href="https://cybersecuritynews.com/15-year-old-ghostlock-linux-kernel-vulnerability/">15-year-old GhostLock Linux Kernel Vulnerability Enables Privilege Escalation Attacks</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2026-8971/">CVE-2026-8971: Mozilla Firefox Auth Bypass Vulnerability</a></li>

</ul>
</details>

**Tags**: `#Android`, `#vulnerability`, `#remote root`, `#Linux kernel`, `#Firefox`

---

<a id="item-5"></a>
## [John Deere owners win right-to-repair in FTC settlement](https://apnews.com/article/john-deere-right-to-repair-agriculture-equipment-cb7514ffedb95c130a976af661f2bc02) ⭐️ 8.0/10

John Deere has settled with the Federal Trade Commission and five states, agreeing to allow farmers and independent repair shops to repair their own equipment, ending years of restrictive practices. This settlement is a major victory for the right-to-repair movement, potentially setting a precedent for other manufacturers and empowering consumers to control their own property. Under the settlement, John Deere must provide diagnostic tools, manuals, and software updates to owners and independent repairers for the next 10 years, and pay $1 million in antitrust enforcement costs.

hackernews · djoldman · Jul 8, 23:37 · [Discussion](https://news.ycombinator.com/item?id=48838876)

**Background**: The right-to-repair movement advocates for consumers' ability to repair their own purchased products without being forced to use authorized dealers. John Deere had been criticized for using software locks and proprietary tools to prevent third-party repairs, particularly in the agricultural sector where equipment downtime is costly.

**Discussion**: Commenters praised Louis Rossmann's advocacy and noted the settlement's symbolic importance, though some criticized the small fine relative to John Deere's profits, and others debated the nature of right-to-repair as a fundamental freedom rather than a negotiated concession.

**Tags**: `#right-to-repair`, `#consumer rights`, `#antitrust`, `#John Deere`, `#legislation`

---

<a id="item-6"></a>
## [Mistral's Robostral Navigate: Map-less Robotics Navigation](https://mistral.ai/news/robostral-navigate/) ⭐️ 8.0/10

Mistral AI released Robostral Navigate, an 8-billion-parameter model that enables robots to navigate complex environments using only a single RGB camera and natural language instructions, achieving 76.6% on the R2R-CE benchmark. This marks a significant advancement in map-less navigation, potentially reducing hardware costs and enabling broader adoption of autonomous robots in indoor settings without pre-mapping. The model operates without LiDAR, depth sensors, or multiple cameras, relying solely on a single RGB camera for visual input, and is not openly released for hobbyist use.

hackernews · ottomengis · Jul 8, 14:09 · [Discussion](https://news.ycombinator.com/item?id=48832212)

**Background**: Traditional robot navigation often requires pre-captured maps or multiple depth sensors. Map-less navigation aims to enable robots to follow natural language instructions in unfamiliar environments using only visual input. The kidnapped robot problem arises when a robot loses localization and cannot navigate even short distances. R2R-CE is a standard benchmark for vision-and-language navigation in continuous environments.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/robostral-navigate/">Robostral Navigate: single-camera AI navigation | Mistral AI</a></li>
<li><a href="https://www.siliconreport.com/mistral-ai-releases-robostral-navigate-a-single-camera-robotics-model-95dac18d">Mistral AI Releases Robostral Navigate, a Single-Camera ...</a></li>

</ul>
</details>

**Discussion**: Community comments expressed enthusiasm about map-less navigation and the potential for hobbyist projects, though noted the model is not publicly available. Some compared it to similar work like PIGEON and discussed challenges with higher-level tasks like object manipulation.

**Tags**: `#robotics`, `#navigation`, `#AI`, `#machine learning`, `#Mistral`

---

<a id="item-7"></a>
## [xAI Releases Grok 4.5 with Improved Efficiency](https://x.ai/news/grok-4-5) ⭐️ 8.0/10

xAI has released Grok 4.5, a new version of its AI model that offers improved reasoning efficiency and competitive pricing at $2 per million input tokens and $6 per million output tokens, trained on trillions of tokens of Cursor data. This release positions Grok as a cost-effective alternative to models like GPT-5.4 and Opus 4.8, potentially reshaping the AI pricing landscape, but ongoing ethical concerns about xAI's practices may limit enterprise adoption. Grok 4.5 reportedly performs at the level of Opus 4.7 on benchmarks while being significantly cheaper; however, critics question benchmark integrity and note that the model's training on proprietary Cursor data may raise data privacy issues.

hackernews · BoumTAC · Jul 8, 18:00 · [Discussion](https://news.ycombinator.com/item?id=48835111)

**Background**: Grok is a family of large language models developed by xAI, Elon Musk's AI company. The models are integrated with the X platform and emphasize real-time information access. xAI has faced scrutiny over content moderation and political bias, with some users questioning the trustworthiness of its models.

<details><summary>References</summary>
<ul>
<li><a href="https://guptadeepak.com/research/grok-ai-explained/">Grok AI Explained: xAI's Model Family, Capabilities, and ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/XAI_(company)">SpaceXAI - Wikipedia</a></li>
<li><a href="https://x.ai/company">Company: Accelerating Scientific Discovery | SpaceXAI</a></li>

</ul>
</details>

**Discussion**: Comments are divided: some praise Grok 4.5's cost-effectiveness and benchmark performance, while others express distrust in xAI due to perceived political manipulation and lack of ethical safeguards. Users also debate the economic viability of the AI arms race.

**Tags**: `#AI`, `#Grok`, `#xAI`, `#machine learning`, `#ethics`

---

<a id="item-8"></a>
## [Decoding a Uniqlo T-Shirt's Obfuscated Bash Script](https://tris.sherliker.net/blog/obfuscated-self-evaluating-bash-script-by-cdn-akamai-being-supplied-to-consumers-via-retail-stores/) ⭐️ 8.0/10

A blog post decodes an obfuscated bash script printed on a Uniqlo t-shirt, which was designed by Akamai and intended to be self-evaluating. This highlights real-world obfuscation and reverse engineering, blending fashion with technical culture, and sparks discussion on script readability and OCR challenges. The shirt uses Roboto Mono font but with kerning, making OCR difficult; a commenter notes a syntax error that prevents the script from running.

hackernews · speerer · Jul 8, 08:46 · [Discussion](https://news.ycombinator.com/item?id=48829312)

**Background**: Bash obfuscation hides the true intent of a script using encoding, compression, encryption, or self-modifying code. This shirt is part of a Uniqlo x Akamai collaboration, and the designer has shared a video explaining the creation process, including intentional OCR resistance.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Bashfuscator/Bashfuscator">GitHub - Bashfuscator/Bashfuscator: A fully configurable and extendable Bash obfuscation framework. This tool is intended to help both red team and blue team. · GitHub</a></li>
<li><a href="https://www.baeldung.com/linux/bash-obfuscate-script">How to Obfuscate a Bash Script to Make It Unreadable | Baeldung on Linux</a></li>

</ul>
</details>

**Discussion**: Community comments include humor about returning the shirt due to a syntax error, references to Martin Kleppe's quine clock, and praise for the designer's video. Some also note the difficulty of OCRing the shirt and speculate whether the script was generated by an LLM.

**Tags**: `#bash`, `#obfuscation`, `#reverse-engineering`, `#uniqlo`, `#hacker-news`

---

<a id="item-9"></a>
## [Cloudflare Meerkat: Global Asynchronous Consensus](https://blog.cloudflare.com/meerkat-introduction/) ⭐️ 8.0/10

Cloudflare Research announced Meerkat, a globally distributed consensus service that implements the QuePaxa asynchronous consensus algorithm, with plans to build a strongly consistent, fault-tolerant key-value store. This is the first production deployment of an asynchronous consensus algorithm (QuePaxa), which eliminates reliance on timeouts and maintains progress even under severe network delays, potentially improving global distributed systems reliability. Compared to leader-based protocols like Raft, Meerkat is leaderless and uses hedging to dynamically manage proposers. However, reads also require global consensus, which may introduce higher latency for read-heavy workloads.

hackernews · bobnamob · Jul 8, 13:18 · [Discussion](https://news.ycombinator.com/item?id=48831565)

**Background**: Most distributed consensus protocols (e.g., Paxos, Raft) are partially synchronous, relying on timeouts for liveness. Asynchronous consensus algorithms like QuePaxa do not depend on timeouts, making them robust to network delays but traditionally considered impractical due to complexity. Cloudflare's Meerkat aims to demonstrate that asynchronous consensus can be efficient in production.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/meerkat-introduction/">Introducing Meerkat- an experiment in global consensus</a></li>
<li><a href="https://bford.info/pub/os/quepaxa/quepaxa.pdf">QuePaxa: Escaping the Tyranny of Timeouts in Consensus QuePaxa: Escaping the Tyranny of Timeouts in Consensus QuePaxa: Escaping the Tyranny of Timeouts in Consensus Artifact Review Summary: QuePaxa: Escaping the tyranny of ... Post by @cloudflare.social — Bluesky</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Meerkat eliminates timeout issues, which is valuable for messy networks, but some expressed concern that every read requires global consensus, limiting its use for read-heavy applications. Others appreciated the innovation and the first production implementation of asynchronous consensus.

**Tags**: `#distributed systems`, `#consensus algorithms`, `#Cloudflare`, `#QuePaxa`, `#asynchronous consensus`

---

<a id="item-10"></a>
## [Alibaba Orders Employees to Uninstall Claude by July 10](https://t.me/zaihuapd/42424) ⭐️ 8.0/10

Alibaba has internally ordered all employees to uninstall Anthropic's Claude products, including models like Sonnet, Opus, and Fable, as well as the Claude Code agent tool, effective July 10. This reverse ban comes after Anthropic accused Alibaba of using approximately 25,000 fake accounts to interact with Claude over 28 million times between April 22 and June 5. This policy marks a significant escalation in corporate AI governance and reflects growing tensions between US and Chinese AI companies over security and data access. It could influence how other large enterprises approach external AI tool usage and may reshape competitive dynamics in the enterprise AI market. The ban covers all Anthropic-related products including Claude Sonnet, Opus, Fable models, and the Claude Code agent. Alibaba previously reimbursed employees for using external models like Claude, GPT, and Gemini, but this policy reverses that practice entirely.

telegram · zaihuapd · Jul 8, 06:09

**Background**: Anthropic is a US-based AI safety company founded by former OpenAI employees, known for its Claude series of large language models. The company offers various Claude models (Haiku, Sonnet, Opus, Fable) and a coding agent tool called Claude Code. Alibaba is a Chinese multinational technology conglomerate that has been investing heavily in AI, including its own models like Tongyi Qianwen. The accusation of fake account usage highlights the competitive and security tensions between AI companies across borders.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/overview">Models overview - Claude Platform Docs</a></li>
<li><a href="https://www.anthropic.com/product/claude-code">Claude Code | Anthropic's agentic coding system</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#enterprise AI`, `#Alibaba`, `#Anthropic`, `#Claude`

---

<a id="item-11"></a>
## [Huawei 5G flagship returns overseas with 1100 Mbps peak speed](https://finance.sina.com.cn/tech/roll/2026-07-08/doc-inihapna8035781.shtml) ⭐️ 8.0/10

Huawei's Pura 90 Pro Max International Edition now natively supports 5G networks, achieving peak download speeds over 1100 Mbps in overseas tests, marking its first 5G flagship release abroad since US sanctions began seven years ago. This release signals Huawei's successful overcoming of US technology restrictions, potentially reshaping the global 5G smartphone market by reintroducing a strong competitor. It also demonstrates the practical application of Huawei's 5A communication technology in real-world networks. The device runs HarmonyOS 6.0.0.125 and incorporates Huawei's 5A communication technology, a suite of terminal-side enhancements for improved signal and speed. Overseas tests confirmed the status bar shows a 5G icon, verifying native 5G support.

telegram · zaihuapd · Jul 8, 12:17

**Background**: Since 2019, US sanctions have prevented Huawei from using 5G-capable chipsets from US suppliers, forcing it to rely on in-house Kirin chips and delayed 5G phone launches. In 2023, the Mate 60 series marked a breakthrough with 5G capability using domestically sourced components. 5A is not 5G itself but a suite of AI-driven communication technologies that optimize network connectivity, including fast access, low latency, and wide coverage, as explained by Huawei.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.biggo.com/news/202602182022_Huawei_5A_Technology_Explained">Huawei's "5A" Explained: Not 5G, But a Smarter Way to Connect — BigGo Finance</a></li>
<li><a href="https://www.huaweicentral.com/huawei-introduces-5a-network-to-this-entry-level-smartphone/">Huawei introduces 5A network to this entry-level smartphone - Huawei Central</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#5G`, `#smartphones`, `#telecommunications`, `#sanctions`

---

<a id="item-12"></a>
## [Meituan's OWL Model Suspected of Session Data Leak on OpenRouter](https://github.com/gumusserv/ProducerBenchV2/blob/83cad6007ef3fe8df33386e8f43738fe62337e16/parsed_source_data/data/) ⭐️ 8.0/10

Screenshots from Xiaohongshu reveal that Meituan's OWL (LongCat) free test model on OpenRouter may have leaked conversation data, with the exposed data appearing in a GitHub repository that has since been made inaccessible. This incident underscores the privacy risks of using large language models for sensitive tasks, as user session logs become new sensitive data assets; it also raises concerns about data handling practices in the AI industry. The GitHub repository was publicly visible at least until July 7, 2026, and was later detected by a Discord bot token scanner that flagged and reset exposed tokens; similar leaks have occurred with models from Google and DeepSeek.

telegram · zaihuapd · Jul 8, 13:35

**Background**: OpenRouter is a unified API that provides access to over 400 AI models, including Meituan's LongCat-2.0, a 1.6-trillion-parameter mixture-of-experts model trained on Chinese chips. LongCat-2.0 was previously known as 'Owl Alpha' and had been leading OpenRouter benchmarks anonymously. A Discord bot token scanner is a tool that automatically detects and revokes exposed API tokens by scanning public repositories.

<details><summary>References</summary>
<ul>
<li><a href="https://www.codecademy.com/article/what-is-openrouter">What is OpenRouter? A Guide with Practical Examples</a></li>
<li><a href="https://venturebeat.com/technology/meituan-open-sources-longcat-2-0-the-1-6t-near-frontier-agentic-coding-model-thats-been-leading-openrouter-trained-entirely-on-chinese-chips">Meituan open sources LongCat-2.0, the 1.6T, near-frontier agentic coding model that's been leading OpenRouter — trained entirely on Chinese chips | VentureBeat</a></li>
<li><a href="https://top.gg/bot/842154960397008896">Add Token Scanner Discord Bot | The #1 Discord Bot and ...</a></li>

</ul>
</details>

**Discussion**: The community on Xiaohongshu has widely shared the leak screenshots, with users warning others not to input sensitive information like API keys or source code into AI models, and discussing the broader implications for data privacy in agent-based systems.

**Tags**: `#大模型安全`, `#数据泄露`, `#隐私`, `#美团`, `#OWL`

---

<a id="item-13"></a>
## [Researchers identify apps via leaked EM signals with 99% accuracy](https://www.scmp.com/news/china/science/article/3359688/chinese-researchers-find-peephole-any-smartphone-its-leaked-radio-signal) ⭐️ 8.0/10

Researchers developed a non-contact forensic technique that analyzes low-frequency electromagnetic signals leaked from smartphones to identify running apps and some operations, achieving up to 99.07% accuracy on iPhone 15 Pro, Xiaomi 15 Pro, and OPPO Reno 13. This side-channel attack reveals a significant privacy vulnerability because it works offline, in airplane mode, and even when the device is encrypted or locked, potentially allowing attackers to spy on user activities without any physical access or system compromise. The technique exploits unintentional electromagnetic emanations from a smartphone's processor and other components during app execution, and does not require any prior access to the device's operating system or stored data.

telegram · zaihuapd · Jul 8, 16:05

**Background**: Electromagnetic side-channel attacks measure the EM radiation emitted by electronic devices during operation, which can leak information about internal states. Past research has shown that power consumption or EM signals can sometimes reveal which apps are running, but practical non-contact attacks with high accuracy on modern smartphones have been limited. This work demonstrates a low-frequency EM attack that is passive and requires no hardware modification to the target device.

**Tags**: `#security`, `#electromagnetic signal`, `#side-channel attack`, `#mobile privacy`

---

<a id="item-14"></a>
## [LineageOS Introduces Web-Based Flashing Tool](https://www.androidauthority.com/lineageos-summertime-update-2026-3685112/) ⭐️ 8.0/10

LineageOS has released a web-based flashing tool called Lineage Flash Tools as part of its summer 2026 update, allowing users to flash devices directly from a browser without installing ADB or Fastboot locally. This tool significantly lowers the barrier for users to install custom ROMs, making the process more accessible and less error-prone, which could expand the custom ROM community. The tool supports Fastboot, ADB, and Samsung Odin protocols, requires a WebUSB-compatible browser like Chrome or Edge, and must be used alongside device-specific Wiki guides; it does not fully replace traditional flashing methods.

telegram · zaihuapd · Jul 9, 01:46

**Background**: WebUSB is a JavaScript API that allows web applications to communicate with USB devices securely, which enables this browser-based flashing. The Odin protocol is used for Samsung devices. Additionally, LineageOS introduced Material 3 Expressive UI in the Updater app and confirmed development of LineageOS 24 based on Android 17.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebUSB">WebUSB - Wikipedia</a></li>
<li><a href="https://source.android.com/docs/core/ota/ab">A/B (seamless) system updates | Android Open Source Project</a></li>

</ul>
</details>

**Tags**: `#LineageOS`, `#custom ROM`, `#web flashing`, `#Android`, `#WebUSB`

---