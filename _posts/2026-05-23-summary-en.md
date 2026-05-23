---
layout: default
title: "Horizon Summary: 2026-05-23 (EN)"
date: 2026-05-23
lang: en
---

> From 26 items, 7 important content pieces were selected

---

1. [Why Japanese Companies Diversify: Lifetime Employment Roots](#item-1) ⭐️ 8.0/10
2. [Anthropic's Project Glasswing Shows 90.6% True Positive Rate](#item-2) ⭐️ 8.0/10
3. [yt-dlp deprecates Bun support over Rust rewrite concerns](#item-3) ⭐️ 8.0/10
4. [AI-Driven HBM Demand Squeezes Consumer Electronics Memory](#item-4) ⭐️ 8.0/10
5. [ByteDance Open Sources Unified Multimodal Model Lance (3B)](#item-5) ⭐️ 8.0/10
6. [China cracks down on illegal cross-border securities trading](#item-6) ⭐️ 8.0/10
7. [Cloudflare Outage 25 Min Affects 28% HTTP Traffic](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Why Japanese Companies Diversify: Lifetime Employment Roots](https://davidoks.blog/p/why-japanese-companies-do-so-many) ⭐️ 8.0/10

An essay by David Oks argues that Japan's lifetime employment and firm-specific skills naturally lead to corporate diversification, contrasting with Western firms' focus on core competencies. This analysis challenges the Western emphasis on corporate focus and efficiency, offering a different model where employee retention and organizational stability drive broad business portfolios. The essay is over 60% exposition before the core argument: firms with immobile lifetime employees and non-transferable skills must diversify to retain workers. This system requires insulation from shareholder pressure to sustain itself.

hackernews · d0ks · May 22, 15:22 · [Discussion](https://news.ycombinator.com/item?id=48237163)

**Background**: Lifetime employment (shūshin koyō) and seniority-based wages are hallmarks of traditional Japanese corporate culture. These practices encourage firms to invest heavily in employee skills that are specific to the company, making layoffs costly and forcing companies to find new business areas to keep employees productive when demand shifts.

**Discussion**: Comments reflect nuanced views: some see Westerners idealizing Japan, while others note that Western companies once diversified similarly (e.g., IBM). There is also criticism of low job fluidity and the harsh reality for mid-career hires.

**Tags**: `#business strategy`, `#organizational structure`, `#Japan`, `#economics`, `#corporate culture`

---

<a id="item-2"></a>
## [Anthropic's Project Glasswing Shows 90.6% True Positive Rate](https://www.anthropic.com/research/glasswing-initial-update) ⭐️ 8.0/10

Anthropic published an update on Project Glasswing, reporting that 90.6% of 1,752 assessed high- or critical-rated vulnerabilities were confirmed as true positives by independent security firms. This result suggests that AI-assisted static analysis can significantly reduce false positives in vulnerability detection, potentially improving the security of critical open-source software at scale. The evaluation covered vulnerabilities found in open-source codebases, with 62.4% (1,094) confirmed as high- or critical-severity. However, some experts, like the curl maintainer, question whether the improvement over existing tools is substantial.

hackernews · louiereederson · May 22, 19:31 · [Discussion](https://news.ycombinator.com/item?id=48240419)

**Background**: Static analysis tools automatically examine source code for potential vulnerabilities without running the program. Recent advances integrate large language models (LLMs) to reduce false positives and find more complex bugs, as demonstrated by systems like IRIS using GPT-4.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing: Securing critical software for the AI era</a></li>
<li><a href="https://arxiv.org/html/2405.17238v1">LLM-Assisted Static Analysis for Detecting Security Vulnerabilities</a></li>

</ul>
</details>

**Discussion**: Commenters reported positive experiences with similar tools like Codex Security, noting high accuracy and essential use. However, skepticism remains, with references to the curl maintainer's critique that the improvements over existing tools may not be significant.

**Tags**: `#AI`, `#security`, `#vulnerability detection`, `#Anthropic`, `#static analysis`

---

<a id="item-3"></a>
## [yt-dlp deprecates Bun support over Rust rewrite concerns](https://github.com/yt-dlp/yt-dlp/issues/16766) ⭐️ 8.0/10

yt-dlp has officially deprecated support for the Bun JavaScript runtime, citing foreseeable compatibility and security issues arising from Bun's ongoing rewrite from Zig to Rust. This move highlights the fragility of depending on rapidly evolving runtimes and sparks a broader debate about how maintainers should assess trust in upstream projects undergoing major architectural changes. Maintainers noted they cannot fully review the approximately 1 million lines of new Rust code in Bun, leading to the deprecation. The decision affects all future yt-dlp releases, while existing support remains for now.

hackernews · tamnd · May 22, 17:24 · [Discussion](https://news.ycombinator.com/item?id=48238789)

**Background**: yt-dlp is a popular command-line tool for downloading videos from YouTube and other sites, forked from youtube-dl. Bun, initially written in Zig, began a rewrite in Rust in May 2026, reaching 99.8% test compatibility on Linux x64. This significant language switch raised concerns among downstream projects about code reviewability, stability, and security.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cosmicjs.com/blog/bun-rust-rewrite-javascript-runtime">Why Bun is Rewriting in Rust (And What It Means for ...</a></li>
<li><a href="https://startupxo.com/en/news/2026/05/bun-zig-rust-runtime-rewrite/">Bun Rewrites from Zig to Rust — Why a Fast Runtime Is ...</a></li>
<li><a href="https://github.com/yt-dlp/yt-dlp">GitHub - yt - dlp / yt - dlp : A feature-rich command-line audio/video...</a></li>

</ul>
</details>

**Discussion**: Community reactions are divided: some users understand the maintainers' caution due to the difficulty of reviewing a million-line codebase, while others argue that functionality and test results should be the primary criteria, not the language choice. Commenter pizlonator compared the reasoning to rejecting software based on editor preference, emphasizing that only whether it works matters.

**Tags**: `#Bun`, `#yt-dlp`, `#JavaScript`, `#Rust`, `#software maintenance`

---

<a id="item-4"></a>
## [AI-Driven HBM Demand Squeezes Consumer Electronics Memory](https://simonwillison.net/2026/May/22/memory-shortage/#atom-everything) ⭐️ 8.0/10

Memory manufacturers are reallocating wafer capacity from DDR and LPDDR to high-bandwidth memory (HBM) for AI data centers, causing a shortage that is driving up prices for consumer electronics like smartphones and laptops. This shift means consumer electronics will become significantly more expensive over the next few years, particularly impacting budget smartphones in emerging markets. Hardware and software engineers must plan for constrained memory availability and higher costs. HBM wafer allocation is expected to rise from 2% to 20% by the end of 2026, and a gigabyte of HBM consumes more than three times the wafer capacity of a gigabyte of DDR or LPDDR. Only three major memory manufacturers remain, and they consistently under-provision capacity to avoid overinvestment.

rss · Simon Willison · May 22, 22:01

**Background**: DDR and LPDDR are common types of DRAM used in desktops, servers, and mobile devices, while HBM is a specialized high-bandwidth memory used with GPUs for AI workloads. Memory manufacturers have fixed wafer fabrication capacity, and the growing demand for HBM is forcing them to reduce allocation to other memory types. This shortage is structurally different from the pandemic-era chip shortage and is expected to last until at least 2030.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HBM_memory_shortage">HBM memory shortage</a></li>
<li><a href="https://octopart.com/pulse/p/how-ai-broke-memory-market">How AI Broke the Memory Market: Inside the 2024–2026 DRAM ...</a></li>
<li><a href="https://tech-insider.org/memory-chip-shortage-2026-ai-consumer-electronics/">Memory Chip Shortage 2026: HBM Takes 23% of DRAM Wafers</a></li>

</ul>
</details>

**Tags**: `#memory`, `#AI hardware`, `#semiconductors`, `#consumer electronics`, `#supply chain`

---

<a id="item-5"></a>
## [ByteDance Open Sources Unified Multimodal Model Lance (3B)](https://mp.weixin.qq.com/s/Xbfq72cr1796RZxJIs3L1A) ⭐️ 8.0/10

ByteDance has released Lance, a 3B-parameter multimodal model that natively unifies image understanding, video understanding, image generation, video generation, and cross-modal editing. The model is open-sourced under the Apache 2.0 license with weights available on Hugging Face. Lance demonstrates that a relatively small 3B model can achieve strong performance across both understanding and generation tasks, potentially lowering the barrier for deploying unified multimodal AI. Its open-source release enables researchers and developers to build upon a state-of-the-art foundation. Lance employs a shared context and dual-stream expert architecture, using Qwen2.5-VL and Wan2.2 encoders for understanding and generation respectively, with modality-aware positional encoding to resolve sequence boundary confusion. It achieves top results on benchmarks like GenEval (image generation) and VBench (video generation).

telegram · zaihuapd · May 22, 06:40

**Background**: Most multimodal models specialize in either understanding (e.g., image captioning) or generation (e.g., text-to-image), and separate models are typically required for different tasks. Qwen2.5-VL is a vision-language model by Alibaba Cloud known for strong OCR and document understanding, while Wan2.2 is an open-source video generation model. Lance combines both capabilities in a single, lightweight architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen</a></li>
<li><a href="https://github.com/Wan-Video/Wan2.2">GitHub - Wan-Video/Wan2.2: Wan: Open and Advanced Large-Scale Video Generative Models · GitHub</a></li>
<li><a href="https://wan22.io/">Wan2.2 - Open Source MoE Video Generation | Every Shot, Wan Take | wan22.io</a></li>

</ul>
</details>

**Tags**: `#multimodal`, `#open-source`, `#image generation`, `#video generation`, `#AI`

---

<a id="item-6"></a>
## [China cracks down on illegal cross-border securities trading](https://t.me/zaihuapd/41525) ⭐️ 8.0/10

Chinese regulators launched a two-year crackdown on illegal cross-border securities trading, allowing existing investors only to sell and withdraw funds. The China Securities Regulatory Commission has already filed cases against Tiger Brokers, Futu Holdings, and Changqiao Securities for illegal cross-border operations. This crackdown significantly impacts overseas brokerage platforms targeting Chinese investors and the fintech industry. It may reshape cross-border investment flows and regulatory compliance requirements for foreign brokers. The plan sets a two-year period for clearing existing business, after which all related domestic websites, trading software, and supporting servers must be completely shut down. The crackdown targets not only foreign platforms but also domestic associates and intermediaries that facilitate their operations.

telegram · zaihuapd · May 22, 13:55

**Background**: Cross-border securities trading involves Chinese investors using overseas platforms to trade foreign stocks. In 2021, Chinese regulators began warning about the illegality of such activities without approval. Tiger Brokers, Futu, and Changqiao are major platforms that have faced regulatory challenges in mainland China since then.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Futu_Holdings">Futu Holdings</a></li>
<li><a href="https://www.panewslab.com/en/articles/019e4f2a-e565-77eb-8ec5-7a6c79314f6f">Changqiao Securities responded: It will strictly implement all ... - PANews</a></li>
<li><a href="https://www.mexc.com/news/1108190">China Bans Tiger, Futu, and Changqiao for Illegal Cross-Border ...</a></li>

</ul>
</details>

**Tags**: `#regulatory`, `#fintech`, `#China`, `#cross-border`, `#securities`

---

<a id="item-7"></a>
## [Cloudflare Outage 25 Min Affects 28% HTTP Traffic](https://t.me/zaihuapd/41527) ⭐️ 8.0/10

On December 5, 2024, Cloudflare experienced a 25-minute global network outage affecting approximately 28% of HTTP traffic, caused by a fix for a Next.js security vulnerability (CVE-2025-55182) that impacted the WAF managed rulesets for the old FL1 proxy. As a major internet infrastructure provider, such outages impact millions of websites and users, underscoring the fragility of CDN dependencies and the risks of emergency security patches. The outage primarily affected customers using the legacy FL1 proxy with Cloudflare managed rulesets. The fix for CVE-2025-55182, related to React Server Components in Next.js, triggered the WAF malfunction.

telegram · zaihuapd · May 22, 16:15

**Background**: Cloudflare is a global CDN and security platform that routes traffic through proxies like FL1 (legacy) and FL2 (newer, Rust-based). Managed rulesets are pre-configured WAF rules that protect against common web exploits. CVE-2025-55182 is a security vulnerability in Next.js's React Server Components, which Cloudflare attempted to patch via WAF rules.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.cloudflare.com/cloudflare-one/traffic-policies/proxy/">Proxy · Cloudflare One docs</a></li>
<li><a href="https://developers.cloudflare.com/waf/managed-rules/">Managed Rules · Cloudflare Web Application Firewall (WAF) docs</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#outage`, `#CDN`, `#security`, `#Next.js`

---