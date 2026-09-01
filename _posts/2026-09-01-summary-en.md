---
layout: default
title: "Horizon Summary: 2026-09-01 (EN)"
date: 2026-09-01
lang: en
---

> From 29 items, 6 important content pieces were selected

---

1. [Guide Documents ChatGPT Work Tools and Playwright Browser Skill](#item-1) ⭐️ 8.0/10
2. [Google Removes Manifest V2 Extensions, Including uBlock Origin, from Chrome Web Store](#item-2) ⭐️ 8.0/10
3. [OpenClaw 2.0: Biggest Update Merges Over 16,000 Pull Requests](#item-3) ⭐️ 8.0/10
4. [Apple Announces CEO Transition: Tim Cook Steps Down, John Ternus to Succeed](#item-4) ⭐️ 8.0/10
5. [EU designates ChatGPT, Reddit, Roblox as very large services under stricter DSA rules](#item-5) ⭐️ 8.0/10
6. [Xiaomi unveils Xuanjie O3, O100, and D100 chips spanning mobile, AI, and automotive](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Guide Documents ChatGPT Work Tools and Playwright Browser Skill](https://codex-tool-reference.simonw.chatgpt.site/) ⭐️ 8.0/10

Developer Simon Willison published a community-referenced guide documenting ChatGPT Work tools and skills, highlighted by a notable control-browser skill that uses Playwright to drive a browser via Node.js REPL. This guide showcases how ChatGPT Work can be extended with reusable skills, particularly for browser automation, which could significantly boost AI-agent workflows and developer productivity. The control-browser skill instructs ChatGPT Work to launch a Playwright instance via its Node.js REPL and execute `nodeRepl.write(await browser.documentation());` to receive further instructions. The reference site also documents other tools and skills, and community comments note potential token waste and overlap with Codex.

hackernews · ijidak · Aug 31, 14:07 · [Discussion](https://news.ycombinator.com/item?id=49510000)

**Background**: ChatGPT Work is OpenAI's enterprise-oriented offering that brings context from team tools to complete tasks, powered by models such as GPT-5.6. Skills are reusable, shareable workflows that include instructions, examples, and code, allowing ChatGPT to perform specific tasks consistently. Playwright is a browser automation framework that drives Chromium, Firefox, and WebKit, commonly used for end-to-end testing and AI-agent workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://help.openai.com/en/articles/20001066-skills-in-chatgpt">Skills in ChatGPT | OpenAI Help Center</a></li>
<li><a href="https://playwright.dev/">Fast and reliable end-to-end testing for modern web apps | Playwright</a></li>
<li><a href="https://openai.com/chatgpt-work/">ChatGPT Work for every team | OpenAI</a></li>

</ul>
</details>

**Discussion**: Simon Willison highlighted the control-browser skill as the most interesting, explaining its self-documenting mechanism. Some commenters questioned how it differs from Codex, while others warned that such work tools can slow down processes and consume many tokens. A meta-comment observed that AI-generated outputs tend to share a similar visual look, reminiscent of the Bootstrap era.

**Tags**: `#ChatGPT`, `#AI tools`, `#Playwright`, `#Developer tools`, `#Simon Willison`

---

<a id="item-2"></a>
## [Google Removes Manifest V2 Extensions, Including uBlock Origin, from Chrome Web Store](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

Google has removed Manifest V2 (MV2) extensions from the Chrome Web Store, including the popular ad blocker uBlock Origin. This marks the final phase of the MV2 to Manifest V3 (MV3) migration that has been underway for years. This affects millions of Chrome users who rely on uBlock Origin for ad blocking and privacy protection. Users are being pushed toward Firefox or other browsers that still support MV2 extensions, highlighting concerns about browser monopoly and user choice. Manifest V3 replaces MV2's long-lived background pages with service workers that only run when needed, which limits how extensions like uBlock Origin can block network requests. uBlock Origin's developer recommends using Firefox, where the extension continues to work best.

hackernews · twapi · Aug 31, 21:10 · [Discussion](https://news.ycombinator.com/item?id=49514878)

**Background**: Chrome extensions are built on a manifest file that declares permissions and capabilities. Google introduced Manifest V2 in 2012 and later proposed MV3 to improve security, performance, and user privacy. However, MV3's declarativeNetRequest API restricts the number of filtering rules and replaces blocking web requests with a more limited model. uBlock Origin is a free, open-source, efficient content blocker for Chromium and Firefox developed by Raymond Hill.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V3 | Chrome for Developers</a></li>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">uBlock Origin - Wikipedia</a></li>
<li><a href="https://github.com/gorhill/uBlock">GitHub - gorhill/uBlock: uBlock Origin - An efficient blocker for Chromium and Firefox. Fast and lean. · GitHub</a></li>

</ul>
</details>

**Discussion**: Commenters broadly express frustration with Google's decision and recommend switching to Firefox. Several highlight that ad blocking has become a safety issue for less tech-savvy users, and some note uBlock Origin always worked better in Firefox. Overall sentiment is critical of Chrome and supportive of Firefox.

**Tags**: `#Chrome`, `#Manifest V2`, `#uBlock Origin`, `#WebExtensions`, `#Privacy`

---

<a id="item-3"></a>
## [OpenClaw 2.0: Biggest Update Merges Over 16,000 Pull Requests](https://openclaw.ai/blog/openclaw-2-accidentally) ⭐️ 8.0/10

On August 30, OpenClaw released version 2.0, its largest update yet, merging over 16,000 pull requests from 933 contributors, including 569 first-time contributors. The release overhauls installation, messaging, memory, skills, models, browser, plugins, and security, and adds shared cloud sessions for multi-user collaboration. This marks a major milestone for one of the fastest-growing open-source AI assistant projects on GitHub, demonstrating an unusually large and active contributor base. The broad feature overhaul could make OpenClaw more accessible and collaborative, potentially accelerating adoption among developers and AI-agent users. The team released no new versions for nearly seven weeks to prepare this update, and the 16,000 merged pull requests represent about half of the project's total pull requests to date. The update simplifies installation, rebuilds the browser-side experience, and introduces shared cloud sessions for multi-user collaboration.

telegram · zaihuapd · Aug 31, 04:38

**Background**: OpenClaw is an open-source personal AI assistant project that has become one of the fastest-growing repositories on GitHub, with dozens of maintainers and thousands of contributors building personal agents. It is designed to be extensible through skills, plugins, channels, model providers, tools, and other runtime capabilities. The project gained viral popularity partly through Moltbook, a social network for AI agents, after its initial rebranding. A pull request is a GitHub mechanism for contributors to propose code changes that maintainers can review and merge.

<details><summary>References</summary>
<ul>
<li><a href="https://openclaw.ai/">OpenClaw — Open-Source AI Assistant</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>
<li><a href="https://docs.openclaw.ai/tools">Overview · OpenClaw</a></li>

</ul>
</details>

**Tags**: `#OpenClaw`, `#open source`, `#AI assistant`, `#release`, `#software update`

---

<a id="item-4"></a>
## [Apple Announces CEO Transition: Tim Cook Steps Down, John Ternus to Succeed](https://t.me/zaihuapd/43516) ⭐️ 8.0/10

Apple announced a leadership transition: current CEO Tim Cook will become executive chairman, and hardware engineering senior vice president John Ternus will become CEO on September 1, 2026. This is a major leadership change at one of the world's most influential tech companies, affecting Apple's product strategy and the broader developer ecosystem. It marks a generational shift in Apple's leadership. The board unanimously approved the arrangement; Cook will continue as CEO through the summer to complete the transition with Ternus. Current chairman Arthur Levinson will become lead independent director, and Ternus will join the board on September 1. Ternus joined Apple in 2001, became hardware engineering VP in 2013, and joined the executive team in 2021.

telegram · zaihuapd · Aug 31, 10:21

**Background**: Tim Cook has been Apple's CEO since 2011, overseeing major product launches and the company's growth to a $3 trillion valuation. John Ternus is a long-time Apple hardware executive responsible for iPhone, Mac, iPad, and AirPods. This transition is part of Apple's planned succession.

**Tags**: `#Apple`, `#CEO transition`, `#Tim Cook`, `#John Ternus`, `#tech industry`

---

<a id="item-5"></a>
## [EU designates ChatGPT, Reddit, Roblox as very large services under stricter DSA rules](https://www.euronews.com/next/2026/08/31/eu-places-chatgpt-reddit-and-roblox-under-strictest-digital-safety-rules) ⭐️ 8.0/10

On August 31, the European Commission designated OpenAI's ChatGPT as a Very Large Online Search Engine and Reddit and Roblox as Very Large Online Platforms under the Digital Services Act (DSA), because each service exceeds 45 million monthly active users in the EU. This is the first time an AI chatbot has been classified under the DSA's strictest tier, extending EU content-safety oversight to generative AI and heavily used community platforms. The designation forces these services to proactively mitigate systemic risks such as illegal content, child safety, and user well-being, setting a precedent for similar global regulation. The three services have a four-month transition period to comply. They must conduct annual systemic risk assessments, undergo independent audits, and share data with EU regulators and vetted researchers, with particular attention to illegal content, minor protection, and mental health risks.

telegram · zaihuapd · Aug 31, 14:39

**Background**: The Digital Services Act (DSA) is an EU regulation that applies to digital services, with stricter obligations for Very Large Online Platforms (VLOPs) and Very Large Online Search Engines (VLOSEs) that have at least 45 million average monthly users in the EU. This threshold covers roughly 10% of the EU population. The DSA aims to create a safer and more transparent online environment, requiring these very large services to assess and mitigate systemic risks associated with their operations, such as the spread of illegal content and disinformation.

<details><summary>References</summary>
<ul>
<li><a href="https://pdf.hanspub.org/ojls2025132_72923414.pdf">欧 盟 《数字服务法案》解读及对我国 的 启示</a></li>
<li><a href="https://www.tmtpost.com/6653184.html">欧 盟 《数字服务法》倒计时： 超 大 平 台 各寻门路-钛媒体官方网站</a></li>

</ul>
</details>

**Tags**: `#AI治理`, `#DSA`, `#欧盟`, `#平台监管`

---

<a id="item-6"></a>
## [Xiaomi unveils Xuanjie O3, O100, and D100 chips spanning mobile, AI, and automotive](https://t.me/zaihuapd/43524) ⭐️ 8.0/10

Xiaomi announced three new Xuanjie-series chips: the Xuanjie O3 AI flagship SoC, the Xuanjie O100 AI accelerator with 1.22 TB/s bandwidth, and the Xuanjie D100, described as China's first 3nm automotive AI chip. All three chips have completed post-silicon verification and target edge-AI computing across Xiaomi's human-vehicle-home ecosystem; the O3 is earmarked to debut in the Xiaomi 18 Fold. This is a major step for Xiaomi as it deepens in-house silicon for AI computing across phones, cars, and smart-home devices. Pairing a flagship mobile SoC with a high-bandwidth AI accelerator and a 3nm automotive chip positions Xiaomi against established players in smartphone SoCs and intelligent-driving hardware. The Xuanjie O3 uses a ten-core all-big-core CPU and records a multi-core score above 15,000 for the first time, while its Arm G2-Ultra NX GPU reportedly improves performance by 85% and cuts power by 64% versus the Xuanjie O1. It is also claimed to be the world's first mobile processor with LPDDR6 support; the O100 provides 1.22 TB/s bandwidth, and the D100 is aimed at autonomous-driving AI workloads.

telegram · zaihuapd · Aug 31, 15:15

**Background**: An SoC (system-on-chip) integrates a processor, graphics, memory controller, and AI acceleration into a single package, which is why these chips can power a wide range of Xiaomi devices. LPDDR6 is a memory standard released by JEDEC to significantly improve speed and power efficiency for mobile and AI workloads, adding features such as on-die ECC and error scrubbing for reliability. Xiaomi's Xuanjie line is its self-developed chip family, and this launch appears to extend it from smartphones into AI accelerators and automotive-grade silicon.

<details><summary>References</summary>
<ul>
<li><a href="https://www.jedec.org/news/pressreleases/jedec®-releases-new-lpddr6-standard-enhance-mobile-and-ai-memory-performance">JEDEC® Releases New LPDDR6 Standard to Enhance Mobile and AI Memory Performance | JEDEC</a></li>
<li><a href="https://gadgets.beebom.com/guides/xiaomi-xring-o3-benchmark-specs">Xiaomi Xring O3: Benchmarks and Specs | Beebom Gadgets</a></li>

</ul>
</details>

**Tags**: `#chip`, `#AI`, `#Xiaomi`, `#SoC`, `#hardware`

---