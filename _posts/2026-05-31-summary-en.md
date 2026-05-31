---
layout: default
title: "Horizon Summary: 2026-05-31 (EN)"
date: 2026-05-31
lang: en
---

> From 30 items, 10 important content pieces were selected

---

1. [Microsoft degrades perpetually-licensed Office for Mac to view-only](#item-1) ⭐️ 9.0/10
2. [Accenture to Acquire Ookla for $1.2 Billion](#item-2) ⭐️ 8.0/10
3. [Voxel Space Rendering Algorithm Explained](#item-3) ⭐️ 8.0/10
4. [Zig ELF Linker Improvements Boost Incremental Compilation](#item-4) ⭐️ 8.0/10
5. [OpenRouter Raises $113M Series B for LLM API](#item-5) ⭐️ 8.0/10
6. [Openrsync: OpenBSD's Security-Focused rsync Implementation](#item-6) ⭐️ 8.0/10
7. [Pope Leo's First Encyclical Attacks Technological Messianism](#item-7) ⭐️ 8.0/10
8. [Anthropic Details Sandbox Techniques for Claude AI](#item-8) ⭐️ 8.0/10
9. [Python ASGI apps in browser via Pyodide + service worker](#item-9) ⭐️ 8.0/10
10. [FROST Attack Reveals Browsing via SSD Timing](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Microsoft degrades perpetually-licensed Office for Mac to view-only](https://consumerrights.wiki/w/Microsoft_Office_2019_and_2021_for_Mac_view-only_conversion_(2026)) ⭐️ 9.0/10

Microsoft has announced that perpetually-licensed Office 2019 and 2021 for Mac will be converted to view-only mode starting in 2026, preventing editing without a Microsoft 365 subscription. This move undermines the perpetual license model by retroactively reducing functionality of already-purchased software, forcing users toward subscriptions and raising significant consumer rights concerns. The conversion applies specifically to Office 2019 and 2021 for Mac, with edit functionality requiring a Microsoft 365 subscription; viewer mode only allows viewing and printing, not editing.

hackernews · antipurist · May 30, 23:26 · [Discussion](https://news.ycombinator.com/item?id=48341578)

**Background**: A perpetual software license authorizes indefinite use of a specific version of software, which traditionally does not expire or lose functionality. Viewer mode is a Microsoft feature that restricts Office apps to read-only access when no valid license is detected, typically used for unlicensed users.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Software_license">Software license - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/microsoft-365-apps/licensing-activation/overview-viewer-mode">Overview of viewer mode for Microsoft 365 Apps - Microsoft 365 Apps | Microsoft Learn</a></li>
<li><a href="https://www.techtarget.com/whatis/definition/perpetual-software-license">What Is a Perpetual Software License ? – Definition from TechTarget</a></li>

</ul>
</details>

**Discussion**: Commenters express outrage, with many calling for boycotts and switching to alternatives like LibreOffice. Some point out potential violations of Australian consumer law, while others speculate the change is to force licensing for AI agent usage.

**Tags**: `#Microsoft`, `#Office`, `#software licensing`, `#consumer rights`, `#perpetual license`

---

<a id="item-2"></a>
## [Accenture to Acquire Ookla for $1.2 Billion](https://newsroom.accenture.com/news/2026/accenture-to-acquire-ookla-to-strengthen-network-intelligence-and-experience-with-data-and-ai-for-enterprises) ⭐️ 8.0/10

Accenture announced the acquisition of Ookla, the company behind Speedtest and Downdetector, for approximately $1.2 billion. The deal aims to strengthen Accenture's network intelligence and AI-driven services for enterprises. This acquisition gives Accenture access to vast amounts of real-world network performance data, enabling deeper insights and AI-driven optimization for telecom operators and enterprises. It highlights the increasing value of proprietary data in the consulting and IT services industry. Ookla's platform collects over 250 million consumer-initiated tests per month, plus controlled drive, walk, and embedded testing. The deal includes brands like Speedtest, Downdetector, Ekahau, and RootMetrics.

hackernews · Garbage · May 30, 16:28 · [Discussion](https://news.ycombinator.com/item?id=48337987)

**Background**: Ookla is best known for Speedtest.net, a widely used internet speed testing tool. However, its core business is selling aggregated network performance data to telecom companies. Accenture already entered this space through its earlier acquisition of Umlaut, making this deal a consolidation of competitive assets.

**Discussion**: Commenters emphasize that the deal is fundamentally a data acquisition, as Ookla's true value lies in selling network data to telcos. Some express surprise at the $1.2B price, while others offer insider perspectives on the company's revenue model and competitive dynamics.

**Tags**: `#acquisition`, `#network intelligence`, `#data`, `#telco`, `#AI`

---

<a id="item-3"></a>
## [Voxel Space Rendering Algorithm Explained](https://s-macke.github.io/VoxelSpace/) ⭐️ 8.0/10

A technical demo and explanation of the Voxel Space terrain rendering algorithm, originally used in the 1992 game Comanche, has been published with core code in less than 20 lines. This algorithm demonstrates an efficient 2.5D rendering technique that allowed realistic terrain on early 90s hardware, inspiring retro-computing enthusiasts and game developers to explore similar approaches. The Voxel Space algorithm is not true voxel rendering; it uses a heightmap with colored columns and ray casting, similar to a 2.5D engine. The core rendering loop fits in under 20 lines of code.

hackernews · davikr · May 30, 14:25 · [Discussion](https://news.ycombinator.com/item?id=48336564)

**Background**: Voxel Space is a 2.5D terrain rendering technique that represents the landscape as a heightmap with a color map, rendering columns of pixels rather than triangles. It was used in the game Comanche (1992) to achieve realistic terrain on limited hardware. Unlike true 3D voxels, it only allows viewing from above, not full 3D freedom.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/s-macke/VoxelSpace">GitHub - s-macke/VoxelSpace: Terrain rendering algorithm in less than ...</a></li>
<li><a href="https://jbaker.graphics/writings/voxelspace.html">Voxelspace in a Compute Shader - jbaker.graphics</a></li>

</ul>
</details>

**Discussion**: Commenters clarified that the technique is a heightmap, not true voxels, and shared personal projects such as ports to AGS Engine and a C++ version using the original map. Some recalled the game's historical impact and minimal test methodology inspired by its first mission.

**Tags**: `#graphics`, `#rendering`, `#retro-computing`, `#game-development`, `#algorithms`

---

<a id="item-4"></a>
## [Zig ELF Linker Improvements Boost Incremental Compilation](https://ziglang.org/devlog/2026/#2026-05-30) ⭐️ 8.0/10

Zig's latest devlog details significant improvements to its ELF linker, which are a critical step toward enabling fast iteration and incremental compilation across all targets. These improvements make Zig a more viable replacement for C, potentially allowing developers to iterate at the speed of high-level languages while retaining C or Rust-level performance. The devlog focuses on incremental linking, which only relinks changed portions, dramatically speeding up the edit-compile-test cycle, but it may be mutually exclusive with link-time optimization (LTO).

hackernews · kristoff_it · May 30, 17:29 · [Discussion](https://news.ycombinator.com/item?id=48338673)

**Background**: An ELF (Executable and Linkable Format) linker is a tool that combines object files into a single executable or library. Incremental compilation recompiles only modified portions of a program rather than the whole project, enabling faster development cycles. Zig, a systems programming language, aims to be a modern replacement for C with improved safety and build system.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Executable_and_Linkable_Format">Executable and Linkable Format - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Incremental_compilation">Incremental compilation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Incremental_compiler">Incremental compiler - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community is highly enthusiastic, with comments viewing the linker as a key step toward Zig becoming 'THE C replacement.' Developers are considering Zig as a transpilation target and discuss porting VMs like Raku's MOARVM to Zig. One commenter raises the trade-off with link-time optimization.

**Tags**: `#Zig`, `#linker`, `#compiler`, `#systems programming`, `#devlog`

---

<a id="item-5"></a>
## [OpenRouter Raises $113M Series B for LLM API](https://openrouter.ai/announcements/series-b) ⭐️ 8.0/10

OpenRouter announced a $113M Series B funding round led by CapitalG, with participation from NVentures, ServiceNow Ventures, MongoDB Ventures, Snowflake Ventures, Databricks Ventures, AMP PBC, and Pace Capital, alongside existing investors Andreessen Horowitz and Menlo Ventures. This substantial investment highlights OpenRouter's critical role as a unified API proxy for large language models, simplifying access to over 400 models and reducing friction for developers. The funding will help OpenRouter scale its infrastructure and expand its offerings, potentially accelerating adoption of AI across the developer ecosystem. OpenRouter's service includes features like billing caps, which many model providers lack, and charges a small markup (around 5%) over raw provider costs. The co-founder emphasized that the company remains founder-led and founder-controlled, and plans to use the funding to build a strong financial foundation for long-term growth.

hackernews · freeCandy · May 30, 17:27 · [Discussion](https://news.ycombinator.com/item?id=48338660)

**Background**: OpenRouter is a service that provides a unified API for accessing hundreds of large language models (LLMs) from different providers, allowing developers to switch between models easily without integrating multiple distinct APIs. It acts as a proxy, offering additional features like billing caps, logging, and model fallback. As the LLM landscape rapidly evolves with many new models emerging, OpenRouter reduces friction for developers experimenting with different models.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/">OpenRouter</a></li>
<li><a href="https://www.codecademy.com/article/what-is-openrouter">What is OpenRouter? A Guide with Practical Examples</a></li>

</ul>
</details>

**Discussion**: Community members like simonw highlighted OpenRouter's low friction and billing caps as key advantages, while numlocked (co-founder) addressed questions about the funding, emphasizing founder control and long-term vision. Some commenters expressed concerns about the sustainability of the 5% surcharge and potential consolidation in the future, but overall sentiment was positive, acknowledging OpenRouter's utility for experimenting with various models.

**Tags**: `#AI infrastructure`, `#LLM API`, `#funding`, `#OpenRouter`, `#AI tools`

---

<a id="item-6"></a>
## [Openrsync: OpenBSD's Security-Focused rsync Implementation](https://github.com/kristapsdz/openrsync) ⭐️ 8.0/10

Openrsync is a new implementation of the rsync tool by the OpenBSD team, emphasizing security through the use of pledge and unveil system calls. It is being developed as part of an RPKI validator. This implementation aims to provide a more secure alternative to the widely-used rsync, potentially reducing vulnerabilities in file synchronization. It has gained traction in the community and sparked debate about security features and portability. Openrsync currently does not support all rsync features; for example, it has a known issue with the --rsync-path option behavior. It is primarily developed on OpenBSD and relies on OpenBSD's pledge and unveil for sandboxing.

hackernews · sph · May 30, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48334854)

**Background**: Rsync is a popular tool for efficiently transferring and synchronizing files. OpenBSD's pledge and unveil are system calls that allow programs to restrict their access to system resources, enhancing security by limiting the damage from potential exploits. Openrsync leverages these to provide a hardened rsync alternative.

<details><summary>References</summary>
<ul>
<li><a href="https://man.openbsd.org/pledge.2">pledge(2) - OpenBSD manual pages</a></li>
<li><a href="https://lwn.net/Articles/767137/">OpenBSD's unveil() - LWN.net</a></li>

</ul>
</details>

**Discussion**: Users report that openrsync is improving but still has gaps compared to Samba's rsync, such as with --rsync-path. Some note its development within a RPKI validator context. Others mention alternative implementations like a Go version by Michael Stapelberg. The discussion highlights the importance of pledge/unveil for security.

**Tags**: `#rsync`, `#OpenBSD`, `#security`, `#implementation`

---

<a id="item-7"></a>
## [Pope Leo's First Encyclical Attacks Technological Messianism](https://www.economist.com/europe/2026/05/28/leos-first-encyclical-attacks-technological-messianism) ⭐️ 8.0/10

Pope Leo XIV issued his first encyclical on May 28, 2026, criticizing the belief that technology can bring salvation, which he terms 'technological messianism'. This encyclical marks a significant intervention by the Catholic Church in debates over AI ethics and the growing influence of tech leaders promoting transhumanist or quasi-religious narratives about AI. The encyclical does not reject technology outright but warns against treating it as a source of ultimate salvation, echoing earlier papal concerns about the ethical limits of technological progress.

hackernews · 1vuio0pswjnm7 · May 30, 10:30 · [Discussion](https://news.ycombinator.com/item?id=48334710)

**Background**: Technological messianism refers to the belief that technological advancement alone can solve humanity's deepest problems and bring about a utopian future. The Catholic Church has historically engaged with modern ideologies, and this encyclical continues that tradition by addressing the quasi-religious fervor surrounding AI and transhumanism.

<details><summary>References</summary>
<ul>
<li><a href="https://www.biomedima.org/techno-messianism/">Techno- Messianism | BioMedima</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transhumanism">Transhumanism</a></li>

</ul>
</details>

**Discussion**: Commenters largely welcomed the Pope's critique, with some noting its relevance to figures like Peter Thiel who discuss the Antichrist in relation to AI. Others debated the proper control of technology—whether by creators, users, governments, or religious institutions.

**Tags**: `#religion`, `#AI ethics`, `#technology critique`, `#transhumanism`

---

<a id="item-8"></a>
## [Anthropic Details Sandbox Techniques for Claude AI](https://simonwillison.net/2026/May/30/how-we-contain-claude/#atom-everything) ⭐️ 8.0/10

Anthropic published a detailed technical overview of the sandbox methods used to contain Claude across Claude.ai, Claude Code, and Cowork, including gVisor, Seatbelt, Bubblewrap, and full VMs. This addresses a common gap in documentation for AI sandboxing, helping users and developers better understand and trust the security boundaries of Claude products. Claude.ai uses gVisor, Claude Code uses Seatbelt on macOS and Bubblewrap on Linux, and Claude Cowork runs a full VM. The post also discusses a previously covered file exfiltration vector via api.anthropic.com/v1/files.

rss · Simon Willison · May 30, 21:36

**Background**: Sandboxing is a security technique that isolates applications to limit their access to system resources. gVisor is a container sandbox by Google that implements Linux syscalls in userspace. Seatbelt is macOS's native sandbox tool, and Bubblewrap is a lightweight Linux sandbox used by Flatpak. These tools help prevent malicious code or AI agents from accessing sensitive data or causing harm.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GVisor">gVisor - Wikipedia</a></li>
<li><a href="https://github.com/michaelneale/agent-seatbelt-sandbox">GitHub - michaelneale/agent-seatbelt-sandbox: using native macos sandboxing to stop data egress · GitHub</a></li>
<li><a href="https://github.com/containers/bubblewrap">GitHub - containers/bubblewrap: Low-level unprivileged sandboxing tool used by Flatpak and similar projects · GitHub</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#sandboxing`, `#Claude`, `#security`, `#gVisor`

---

<a id="item-9"></a>
## [Python ASGI apps in browser via Pyodide + service worker](https://simonwillison.net/2026/May/30/pyodide-asgi-browser/#atom-everything) ⭐️ 8.0/10

Simon Willison demonstrated running Python ASGI apps in the browser using Pyodide and a service worker instead of a web worker, overcoming the limitation that web workers cannot execute <script> tags. He provided demos of a basic ASGI FastCGI app and Datasette 1.0a31 running in the browser. This approach enables richer Python web applications to run fully in the browser, including those relying on JavaScript plugins, without needing a server. It could significantly expand the capabilities of tools like Datasette Lite and other browser-based Python environments. The solution uses a service worker to intercept network requests and execute Python ASGI apps inside Pyodide, allowing JavaScript in <script> tags to execute normally. The project was built with assistance from Claude Opus 4.8 via Claude Code for web.

rss · Simon Willison · May 30, 21:02

**Background**: Pyodide is a Python distribution for the browser based on WebAssembly, allowing Python code to run client-side. ASGI (Asynchronous Server Gateway Interface) is a standard for asynchronous Python web applications. Web Workers run scripts in background threads but cannot access the DOM or execute inline JavaScript, whereas service workers can intercept network requests and run persistently, enabling full page functionality.

<details><summary>References</summary>
<ul>
<li><a href="https://pyodide.org/">Pyodide — Version 0.29.4</a></li>
<li><a href="https://en.wikipedia.org/wiki/ASGI">ASGI</a></li>
<li><a href="https://web.dev/learn/pwa/service-workers">Service workers | web.dev</a></li>

</ul>
</details>

**Tags**: `#Pyodide`, `#ASGI`, `#Service Workers`, `#WebAssembly`, `#Python`

---

<a id="item-10"></a>
## [FROST Attack Reveals Browsing via SSD Timing](https://futurism.com/future-society/websites-spying-solid-state-drive) ⭐️ 8.0/10

Researchers have disclosed the FROST attack, which uses the browser's Origin Private File System (OPFS) API to measure SSD read/write timing and infer a victim's open websites and applications with high accuracy (88.95% for websites, 95.83% for apps) without requiring any permissions or user interaction. This attack significantly expands the browser side-channel threat landscape by exploiting a previously overlooked hardware resource (SSD) and a legitimate browser API, posing a serious privacy risk to users who may have sensitive tabs open simultaneously. The researchers bypassed OS caching by creating files larger than system memory, ensuring disk accesses hit the physical SSD. The attack currently works on Mac and Linux; Windows is not immune but was not tested. Enabling cross-origin isolation policies can restore high-resolution timers for better accuracy.

telegram · zaihuapd · May 31, 01:55

**Background**: Side-channel attacks exploit indirect information (like timing or power consumption) to infer secrets. The Origin Private File System (OPFS) is a browser API that allows web apps to store data in a sandboxed file system on the user's device. By measuring the time taken for OPFS read/write operations, an attacker can detect contention on the SSD caused by other processes, revealing which websites or apps are active.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/cyber-security/researchers-say-they-can-spy-on-your-browsing-by-measuring-ssd-activity-through-a-browser-api">Researchers say they can spy on your browsing by measuring SSD activity through a browser API — claim FROST attack requires no permissions or user interaction to identify which apps and websites you're using | Tom's Hardware</a></li>
<li><a href="https://arstechnica.com/security/2026/05/websites-have-a-new-way-to-spy-on-visitors-analyzing-their-ssd-activity/">Websites have a new way to spy on visitors: Analyzing their SSD activity - Ars Technica</a></li>
<li><a href="https://cyberinsider.com/new-frost-attack-leverages-ssd-side-channel-to-reveal-browsing-activity/">New FROST attack leverages SSD side-channel to reveal browsing activity</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#side-channel attack`, `#privacy`, `#SSD`, `#browser security`

---