---
layout: default
title: "Horizon Summary: 2026-06-04 (EN)"
date: 2026-06-04
lang: en
---

> From 28 items, 13 important content pieces were selected

---

1. [US Plans to Dismantle AMOC Monitoring System](#item-1) ⭐️ 9.0/10
2. [Elixir v1.20 Introduces Gradual Typing](#item-2) ⭐️ 9.0/10
3. [Google Unveils Gemma 4 12B: Encoder-Free Multimodal Model](#item-3) ⭐️ 9.0/10
4. [Let's Encrypt Plans Post-Quantum Certificates via Merkle Trees](#item-4) ⭐️ 9.0/10
5. [Uber Caps Employee AI Tool Spending to $1500/Month](#item-5) ⭐️ 8.0/10
6. [DaVinci Resolve 21 Unveiled with Photo Management and AI Tools](#item-6) ⭐️ 8.0/10
7. [Espressif Announces ESP32-S31: RISC-V SoC with SIMD Instructions](#item-7) ⭐️ 8.0/10
8. [Mathematicians Warn of AI's Rapid Gains](#item-8) ⭐️ 8.0/10
9. [In-depth Analysis of Original PlayStation Architecture](#item-9) ⭐️ 8.0/10
10. [Google lets websites opt out of AI search results](#item-10) ⭐️ 8.0/10
11. [Qianwen Opens Platform to Third-Party Agents and Skills](#item-11) ⭐️ 8.0/10
12. [HTTP/2 Bomb Attack Crashes Major Web Servers Remotely](#item-12) ⭐️ 8.0/10
13. [Altman: OpenAI's top internal user consumes ~100B tokens monthly](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [US Plans to Dismantle AMOC Monitoring System](https://e360.yale.edu/digest/trump-ooi-amoc) ⭐️ 9.0/10

The U.S. government intends to dismantle the RAPID array, a system that has monitored the Atlantic Meridional Overturning Circulation (AMOC) at 26.5°N since 2004. This decision comes despite growing evidence that the AMOC is at risk of collapse due to climate change. AMOC collapse would have catastrophic global climate impacts, and losing continuous monitoring would eliminate early warning capabilities. This move underscores the ongoing tension between climate science funding and other national priorities. The RAPID array is a relatively inexpensive system compared to major defense projects, yet it provides essential data for understanding AMOC behavior. Recent studies indicate the AMOC is at its weakest in over 1,600 years and may be approaching a tipping point.

hackernews · rguiscard · Jun 4, 00:44 · [Discussion](https://news.ycombinator.com/item?id=48392232)

**Background**: The Atlantic Meridional Overturning Circulation (AMOC) is a system of ocean currents that transports warm water northward and cold water southward, playing a vital role in regulating global climate. The RAPID array at 26.5°N has been providing continuous observations of the AMOC since 2004, enabling scientists to track its strength and variability. Without such monitoring, detecting abrupt changes or imminent collapse would become much more difficult.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Atlantic_meridional_overturning_circulation">Atlantic meridional overturning circulation - Wikipedia</a></li>
<li><a href="https://oceanservice.noaa.gov/facts/amoc.html">What is the Atlantic Meridional Overturning Circulation (AMOC)?</a></li>
<li><a href="https://www.theguardian.com/environment/2026/apr/15/critical-atlantic-current-significantly-more-likely-to-collapse-than-thought">Critical Atlantic current significantly more likely to collapse than thought | Oceans | The Guardian</a></li>
<li><a href="https://climate.metoffice.cloud/amoc.html">AMOC | Climate Dashboard</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC10590665/">From theory to RAPID AMOC observations: a personal voyage of...</a></li>

</ul>
</details>

**Discussion**: Comments on the news express frustration over cutting climate monitoring while spending heavily on military projects like the F-35, noting the relative cheapness of the RAPID array. Some users highlight the political undertones in how the story is framed, while others emphasize the importance of continuous data for climate modeling.

**Tags**: `#climate science`, `#oceanography`, `#policy`, `#research funding`, `#AMOC`

---

<a id="item-2"></a>
## [Elixir v1.20 Introduces Gradual Typing](https://elixir-lang.org/blog/2026/06/03/elixir-v1-20-0-released/) ⭐️ 9.0/10

Elixir v1.20, released on June 3, 2026, introduces gradual typing as a core feature, allowing developers to optionally add static type annotations while preserving dynamic typing for unannotated code. This marks a major evolution for Elixir, addressing a long-standing demand for static typing in the functional programming community and potentially attracting developers who prefer type safety without sacrificing the language's dynamic flexibility. The gradual typing system is based on research by Jeremy Siek and Walid Taha, integrated into the compiler, and provides a sound type system with runtime checks where necessary.

hackernews · cloud8421 · Jun 3, 19:02 · [Discussion](https://news.ycombinator.com/item?id=48388324)

**Background**: Gradual typing is a type system that allows mixing static and dynamic typing within the same language, enabling incremental addition of type annotations for improved safety without a full rewrite. Elixir previously relied on Dialyzer for type inference, but the new system offers deeper integration and soundness.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gradual_typing">Gradual typing</a></li>
<li><a href="https://jsiek.github.io/home/WhatIsGradualTyping.html">What is Gradual Typing | Jeremy Siek</a></li>

</ul>
</details>

**Discussion**: Community comments show excitement mixed with skepticism, with some developers welcoming the move toward types while others question performance trade-offs compared to Dialyzer's success typing approach. There is debate over whether gradual typing can match the efficiency of fully static systems.

**Tags**: `#Elixir`, `#gradual typing`, `#functional programming`, `#language design`, `#type systems`

---

<a id="item-3"></a>
## [Google Unveils Gemma 4 12B: Encoder-Free Multimodal Model](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemma-4-12b/) ⭐️ 9.0/10

Google DeepMind released Gemma 4 12B, a compact encoder-free multimodal model that processes vision and audio directly through the language model backbone without a separate vision encoder. This design significantly reduces model size and hardware requirements, enabling powerful multimodal AI to run on consumer-grade laptops with 16GB RAM, democratizing access to advanced AI capabilities. The model replaces traditional vision encoders with a lightweight embedding module consisting of a single matrix multiplication, positional embedding, and normalizations, totaling only 35M parameters. It is released under the Apache 2.0 license.

hackernews · rvz · Jun 3, 16:04 · [Discussion](https://news.ycombinator.com/item?id=48385906)

**Background**: Traditional multimodal large language models (LLMs) rely on separate vision encoders (e.g., SigLIP with 550M parameters) and audio encoders (300M parameters) to process non-text inputs. These encoders add significant computational overhead. Gemma 4 12B's encoder-free architecture feeds raw vision and audio tokens directly into the LLM backbone, greatly improving efficiency and enabling local inference on consumer hardware without cloud dependencies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/06/03/google-deepmind-releases-gemma-4-12b-an-encoder-free-multimodal-model-with-native-audio-that-runs-on-a-16-gb-laptop/">Google DeepMind Releases Gemma 4 12B: An Encoder - Free ...</a></li>
<li><a href="https://dev.to/gilles_hamelink_ea9ff7d93/unlocking-3d-understanding-the-rise-of-encoder-free-multimodal-models-b03">"Unlocking 3D Understanding: The Rise of Encoder - Free Multimodal ..."</a></li>

</ul>
</details>

**Discussion**: Community members tested the Q4 quantized version and reported decent results but noted occasional syntax errors like extra brackets or commas. Some expressed curiosity about the encoder-free design, questioning whether it truly eliminates encoding. Others praised it as an optimal small-model solution for affordable hardware, while a user questioned Google's business rationale for releasing open models.

**Tags**: `#AI`, `#multimodal`, `#machine learning`, `#Gemma`, `#open source`

---

<a id="item-4"></a>
## [Let's Encrypt Plans Post-Quantum Certificates via Merkle Trees](https://letsencrypt.org/2026/06/03/pq-certs) ⭐️ 9.0/10

Let's Encrypt announced plans to adopt post-quantum certificates using Merkle Tree Certificates (MTCs) to prepare for the era of quantum computing. The announcement was made on June 3, 2026. As the largest Certificate Authority by issuance, Let's Encrypt's transition to post-quantum cryptography sets a critical precedent for the entire internet's security infrastructure. This move addresses the looming threat of quantum computers breaking current public-key cryptography, often referred to as 'Q-Day'. Merkle Tree Certificates are a new certificate format that integrates public logging to reduce overhead from large post-quantum signatures and short-lived certificates. The transition involves significant changes to X.509 certificates and Certificate Transparency, and is expected to be a complex project.

hackernews · SGran · Jun 3, 15:06 · [Discussion](https://news.ycombinator.com/item?id=48385114)

**Background**: Post-quantum cryptography (PQC) refers to algorithms designed to be secure against attacks from quantum computers, which could break widely used algorithms like RSA and ECDSA using Shor's algorithm. NIST released its first PQC standards in 2024. Merkle Tree Certificates (MTCs) are a proposed format that combines certificate issuance with public logging, aiming to reduce the performance impact of large PQC signatures in TLS handshakes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography</a></li>
<li><a href="https://www.ietf.org/archive/id/draft-davidben-tls-merkle-tree-certs-09.html">Merkle Tree Certificates</a></li>
<li><a href="https://blog.cloudflare.com/bootstrap-mtc/">Keeping the Internet fast and secure: introducing Merkle Tree Certificates</a></li>

</ul>
</details>

**Discussion**: Community members expressed a mix of excitement and concern: one noted that we are living in a 'science fiction future', while another highlighted the challenge of replacing decades of battle-tested infrastructure. A developer pointed out limitations in current Certificate Transparency and introduced an existing MTC-compatible implementation called Cordon. Another user asked about quantum resistance of ed25519 signatures.

**Tags**: `#post-quantum cryptography`, `#Let's Encrypt`, `#Merkle Tree`, `#certificate transparency`, `#PKI`

---

<a id="item-5"></a>
## [Uber Caps Employee AI Tool Spending to $1500/Month](https://simonwillison.net/2026/Jun/3/uber-caps-usage/#atom-everything) ⭐️ 8.0/10

Uber has implemented a $1,500 monthly token spending cap per AI coding tool for all employees, after blowing its 2026 AI budget in just four months due to heavy use of agentic coding tools like Claude Code and Cursor. This reveals real-world enterprise cost management challenges as AI coding agents gain rapid adoption, with spending caps potentially becoming a common practice. It also provides a benchmark for the productivity value these tools deliver—around 11% of an engineer's median compensation. The cap applies per tool, so an engineer using both Cursor and Claude Code could spend up to $3,000 per month combined. Individual subscribers currently benefit from subsidized plans costing ~$100/month for similar usage, but those plans are not available to large enterprises like Uber.

rss · Simon Willison · Jun 3, 12:01 · [Discussion](https://news.ycombinator.com/item?id=48383056)

**Background**: AI coding agents like Claude Code and Cursor are tools that autonomously edit code, run commands, and assist developers. They consume tokens from large language models (LLMs), and costs scale with usage. Uber's 2026 AI budget was set in 2025, before the explosive popularity of such tools was anticipated.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Discussion**: Comments debate whether AI coding is a fad or lasting trend, with one noting that companies already pay thousands per seat. Others question if flash models suffice and suggest that large models still struggle with major changes requiring human oversight. Some highlight the need to consider fully-loaded engineer costs rather than just salary.

**Tags**: `#AI`, `#cost management`, `#enterprise`, `#coding agents`, `#productivity`

---

<a id="item-6"></a>
## [DaVinci Resolve 21 Unveiled with Photo Management and AI Tools](https://www.blackmagicdesign.com/products/davinciresolve/whatsnew) ⭐️ 8.0/10

Blackmagic Design has released DaVinci Resolve 21, a major update that introduces a new photo management and editing module, enhanced motion graphics tools, and various AI-powered features such as object removal and facial recognition. This release significantly expands DaVinci Resolve's capabilities beyond video production into photo management, potentially challenging specialized tools like Lightroom and Affinity Photo. It also provides a compelling alternative for Linux users who lack robust photo editing options. The update includes a Fusion motion graphics overhaul with new Fusion templates, and the DaVinci Neural Engine now powers AI features like 'Ultra Beauty' and 'Surface Tracking'. The photo management module allows importing, organizing, and editing raw photos with color grading tools.

hackernews · pentagrama · Jun 3, 14:18 · [Discussion](https://news.ycombinator.com/item?id=48384482)

**Background**: DaVinci Resolve is a professional non-linear video editing and color grading application developed by Blackmagic Design. It has historically focused on video post-production, but version 21 marks its first major expansion into photo editing. The DaVinci Neural Engine is a machine learning system that powers various AI-assisted features within the software.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DaVinci_Resolve">DaVinci Resolve - Wikipedia</a></li>
<li><a href="https://www.blackmagicdesign.com/products/davinciresolve/whatsnew">DaVinci Resolve – What’s New | Blackmagic Design</a></li>

</ul>
</details>

**Discussion**: Community reaction is largely positive, with users praising the photo management capabilities as a potential game-changer for Linux photo editing. Some express fatigue with the heavy marketing of AI features, but acknowledge their practical benefits in editing workflows.

**Tags**: `#davinci-resolve`, `#video-editing`, `#blackmagic-design`, `#photo-management`, `#ai`

---

<a id="item-7"></a>
## [Espressif Announces ESP32-S31: RISC-V SoC with SIMD Instructions](https://www.espressif.com/en/products/socs/esp32-s31) ⭐️ 8.0/10

Espressif announced the ESP32-S31, a dual-core RISC-V microcontroller running at up to 320 MHz with SIMD instructions, enabling Rust-based embedded development without proprietary toolchains. This chip simplifies embedded development by allowing standard Rust toolchains via `rustup target add riscv32imac-unknown-none-elf`, reducing reliance on proprietary SDKs. It also brings SIMD capabilities to low-cost IoT devices, expanding performance possibilities. The ESP32-S31 features 60 GPIOs, a Bitscrambler peripheral similar to Raspberry Pi Pico's PIO for flexible data transformation, and is built for advanced IoT applications requiring multi-protocol connectivity and rich human-machine interfaces.

hackernews · volemo · Jun 3, 16:10 · [Discussion](https://news.ycombinator.com/item?id=48385965)

**Background**: RISC-V is an open-source instruction set architecture (ISA) that allows custom extensions. SIMD (Single Instruction, Multiple Data) enables parallel processing of multiple data points with one instruction, improving performance for tasks like audio/video processing. Espressif's previous ESP32 chips used Tensilica Xtensa cores; the shift to RISC-V opens up more open-source toolchains.

<details><summary>References</summary>
<ul>
<li><a href="https://www.espressif.com/en/products/socs/esp32-s31">ESP32-S31 Dual-Core RISC-V + Multi-Protocol SoC | Espressif Systems</a></li>
<li><a href="https://en.wikipedia.org/wiki/Single_instruction,_multiple_data">Single instruction , multiple data - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/ESP32-S2">ESP32-S2</a></li>

</ul>
</details>

**Discussion**: The community expressed enthusiasm for the SIMD instructions and Rust support, with one commenter noting that RISC-V cores make compilation as simple as `rustup target add`. There was also discussion about naming confusion, as many chips are called "ESP32" despite different architectures, and a mention of the Bitscrambler peripheral's similarity to PIO.

**Tags**: `#ESP32`, `#RISC-V`, `#Embedded Systems`, `#Espressif`, `#Rust`

---

<a id="item-8"></a>
## [Mathematicians Warn of AI's Rapid Gains](https://www.science.org/content/article/mathematicians-issue-warning-ai-rapidly-gains-ground) ⭐️ 8.0/10

Mathematicians have issued a formal warning about the rapid advancement of artificial intelligence in mathematical research, expressing concerns over issues of attribution, verification, and potential disruption to the field. This warning is significant because it comes from authoritative voices in mathematics and highlights deep-seated concerns about AI's impact on research integrity and the human role in the field. The warning focuses on AI's ability to generate and verify proofs, potentially sidelining human mathematicians. Community discussions reveal a spectrum of opinions, from fears of irrelevance to comparisons with past technological disruptions.

hackernews · pseudolus · Jun 3, 10:05 · [Discussion](https://news.ycombinator.com/item?id=48382052)

**Background**: Artificial intelligence, particularly large language models, is increasingly used in scientific research. In mathematics, AI has been employed to prove theorems and discover patterns, raising questions about the role of human intuition and rigorous verification.

**Discussion**: Comments show mixed sentiments: some draw parallels to artists and authors impacted by AI, others note AI's suitability for practical problems, and a few fear a future where humans become mere noise in the mathematical process.

**Tags**: `#AI`, `#mathematics`, `#research ethics`, `#machine learning`

---

<a id="item-9"></a>
## [In-depth Analysis of Original PlayStation Architecture](https://www.copetti.org/writings/consoles/playstation/) ⭐️ 8.0/10

Rodrigo Copetti's practical analysis of the original PlayStation's hardware has been reposted on Hacker News, detailing the CPU, memory mapping, and graphics system with annotated diagrams and explanations. This comprehensive resource helps retro developers, emulator authors, and enthusiasts understand the PS1's unique design constraints and innovations, which are crucial for accurate emulation and preservation of classic games. The PlayStation uses a 32-bit MIPS R3000A CPU at 33.8688 MHz with a Geometry Transformation Engine (GTE) for 3D vector math, and its memory map includes a 1 KB scratchpad mapped over the data cache for fast developer access.

hackernews · gregsadetsky · Jun 3, 10:24 · [Discussion](https://news.ycombinator.com/item?id=48382142)

**Background**: The original PlayStation, released in 1994, was a landmark console that popularized 3D gaming. Its architecture combined a custom CPU, GPU, and sound processor on a single board, with memory mapping techniques that allowed efficient data access. Understanding these details is key for emulation and homebrew development.

<details><summary>References</summary>
<ul>
<li><a href="https://www.copetti.org/writings/consoles/playstation/">PlayStation Architecture | A Practical Analysis</a></li>
<li><a href="https://psx-spx.consoledev.net/memorymap/">Memory Map - PlayStation Specifications - psx-spx</a></li>
<li><a href="https://en.wikipedia.org/wiki/PlayStation_technical_specifications">PlayStation technical specifications - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters shared technical anecdotes, including a trick in Metal Gear Solid where bomb placement was encoded by OR-ing a pointer with an address flag. Others praised the website's design and asked for recommendations on PS1 web emulators using JavaScript or WebAssembly.

**Tags**: `#PlayStation`, `#console architecture`, `#retro gaming`, `#hardware`, `#computer engineering`

---

<a id="item-10"></a>
## [Google lets websites opt out of AI search results](https://9to5google.com/2026/06/02/google-ai-mode-overviews-opt-out/) ⭐️ 8.0/10

Google has introduced a new toggle in Search Console that allows website owners to opt out of appearing in AI Overviews and AI Mode, without affecting their regular search rankings or Discover feed presence. The feature is currently being tested in the UK and will roll out globally. This policy change gives publishers unprecedented control over how their content is used by Google's AI features, addressing long-standing concerns about traffic loss and inaccuracies in AI-generated summaries. It sets a precedent for balancing AI innovation with website owner rights in the search ecosystem. The opt-out applies to AI Overviews, AI Mode, and AI Overviews in Discover, while regular search results and Discover feed remain unaffected. Google is also introducing generative AI search statistics in Search Console to help site owners track impressions and performance.

telegram · zaihuapd · Jun 3, 12:00

**Background**: AI Overviews is a Google Search feature that generates AI-powered summaries of search results, which has been criticized for its inaccuracies and for reducing click-through rates to websites. Google Discover is a personalized content feed that suggests articles to users based on their interests. Search Console is a free tool for webmasters to monitor and optimize their site's presence in Google Search. The opt-out option comes after pressure from UK regulators and publisher complaints about declining traffic from AI-generated content.

<details><summary>References</summary>
<ul>
<li><a href="https://9to5google.com/2026/06/02/google-ai-mode-overviews-opt-out/">Google will let websites opt-out of AI Mode & Overviews in Search</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_AI_Overviews">Google AI Overviews</a></li>
<li><a href="https://the-decoder.com/google-lets-sites-opt-out-of-ai-search-results-knowing-most-have-nowhere-else-to-go/">Google lets sites opt out of AI search results, knowing most have nowhere else to go</a></li>

</ul>
</details>

**Tags**: `#Google`, `#AI Search`, `#Search Console`, `#SEO`, `#AI Overviews`

---

<a id="item-11"></a>
## [Qianwen Opens Platform to Third-Party Agents and Skills](https://www.stcn.com/article/detail/3941333.html) ⭐️ 8.0/10

Qianwen app announced full openness to third-party Agents and Skills, allowing enterprises to operate their own branded agents on the platform. First batch testers include Luckin Coffee, KFC, and China Eastern Airlines. This move signals Alibaba's strategic push to build an AI agent ecosystem, similar to OpenAI's GPT store, enabling wide enterprise adoption and customization. It could accelerate enterprise AI integration across various industries. The platform opening covers both Agents and Skills, with enterprises able to deploy branded agents customized for their services. The first batch includes companies from food, beverage, and aviation sectors.

telegram · zaihuapd · Jun 3, 12:15

**Background**: AI agents are autonomous programs that use large language models and external tools to perform complex tasks. Skills are reusable capability definitions that define how an AI behaves in specific workflows. Qianwen, also known as Tongyi Qianwen, is Alibaba Cloud's family of large language models. Opening the platform to third-party developers follows the trend of building platform-based AI ecosystems, similar to what OpenAI did with GPTs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/insights/enterprise-ai-agents">Enterprise AI Agents: Beyond Productivity | IBM</a></li>
<li><a href="https://www.youmaximize.com/blog/the-ai-skills-vault-how-to-build-reusable-ai-skills-for-video-saas-and-design-workflows">The AI Skills Vault: How to Build Reusable AI Skills for... | YouMaximize</a></li>

</ul>
</details>

**Tags**: `#AI`, `#enterprise AI`, `#Qianwen`, `#agents`, `#platform opening`

---

<a id="item-12"></a>
## [HTTP/2 Bomb Attack Crashes Major Web Servers Remotely](https://blog.calif.io/p/codex-discovered-a-hidden-http2-bomb) ⭐️ 8.0/10

Researchers disclosed a new denial-of-service attack called HTTP/2 Bomb that exploits HPACK compression amplification and Slowloris-like connection holding to exhaust server memory, affecting default HTTP/2 configurations of NGINX, Apache HTTPD, Microsoft IIS, Envoy, and Cloudflare Pingora. This attack is critical because it can bring down hundreds of thousands of websites within seconds using a modest 100 Mbps home network connection, and multiple major servers remain unpatched, posing a widespread remote DoS threat. A single client can hold 32 GB of memory in Apache httpd or Envoy within about 20 seconds; NGINX patched in 1.29.8+, Apache in mod_http2 v2.0.41, while IIS, Envoy, and Pingora have no patches yet.

telegram · zaihuapd · Jun 3, 15:00

**Background**: HPACK is a header compression scheme used in HTTP/2 to reduce overhead; it can amplify small inputs into large decompressed data. Slowloris is a classic DoS attack that keeps many connections open slowly, exhausting server resources. The HTTP/2 Bomb combines these two: the compression bomb quickly allocates memory, and the connection hold prevents memory from being freed, leading to rapid exhaustion.

<details><summary>References</summary>
<ul>
<li><a href="https://cyberinsider.com/new-http-2-bomb-attack-can-exhaust-server-memory-in-seconds/">New “HTTP/2 Bomb” attack can exhaust server memory in seconds | CyberInsider</a></li>
<li><a href="https://thehackernews.com/2026/06/new-http2-bomb-vulnerability-allows.html">New HTTP/2 Bomb Vulnerability Allows Remote DoS on NGINX, Apache, IIS, Envoy & Cloudflare</a></li>
<li><a href="https://www.securityweek.com/http-2-bomb-exploit-knocks-web-servers-offline-in-seconds/">'HTTP/2 Bomb' Exploit Knocks Web Servers Offline in Seconds - SecurityWeek</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#HTTP/2`, `#denial-of-service`, `#web server`

---

<a id="item-13"></a>
## [Altman: OpenAI's top internal user consumes ~100B tokens monthly](https://www.businessinsider.com/sam-altman-openai-top-token-spender-ai-costs-issue-2026-6) ⭐️ 8.0/10

Sam Altman revealed at a corporate event that OpenAI's highest internal user consumes approximately 100 billion tokens per month, and external users consume even more. He also noted that six and a half years ago, the top user consumed only 100,000 tokens monthly, which was likely the global leader at the time, but now that amount is just the global average. This disclosure underscores the massive scaling of AI model usage and the rising cost pressures that come with it, impacting pricing strategies and model efficiency improvements across the industry. It highlights the economic challenges of deploying advanced AI at scale, as costs have become a 'huge problem' that OpenAI is actively addressing. Altman mentioned that OpenAI fosters a culture of high token usage internally, but AI cost pressures are escalating. He noted that cost issues were rarely discussed in early 2026 (likely a misquote or future reference; context suggests the present), but now they are a major problem, and the company is working on improving models to deliver more value at lower cost.

telegram · zaihuapd · Jun 4, 02:31

**Background**: In AI models like OpenAI's GPT series, tokens are the basic units of text processing; they can be as short as a character or as long as a word, and models charge based on token count. The dramatic increase from 100,000 to 100 billion tokens per month over six years illustrates the exponential growth in AI adoption and the need for more efficient architectures.

<details><summary>References</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/ai-tokens-explained/">What Are AI Tokens ? The Language and Currency... | NVIDIA Blog</a></li>
<li><a href="https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them">What are tokens and how to count them? | OpenAI Help Center</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI costs`, `#token usage`, `#scaling AI`

---