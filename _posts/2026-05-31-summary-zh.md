---
layout: default
title: "Horizon Summary: 2026-05-31 (ZH)"
date: 2026-05-31
lang: zh
---

> From 30 items, 10 important content pieces were selected

---

1. [微软将永久授权的 Office for Mac 降级为只读模式](#item-1) ⭐️ 9.0/10
2. [埃森哲以 12 亿美元收购 Ookla](#item-2) ⭐️ 8.0/10
3. [Voxel Space 渲染算法详解](#item-3) ⭐️ 8.0/10
4. [Zig ELF 链接器改进提升增量编译能力](#item-4) ⭐️ 8.0/10
5. [OpenRouter 获 1.13 亿美元 B 轮融资](#item-5) ⭐️ 8.0/10
6. [Openrsync：OpenBSD 注重安全的 rsync 实现](#item-6) ⭐️ 8.0/10
7. [教宗利奥首道通谕抨击技术救世主义](#item-7) ⭐️ 8.0/10
8. [Anthropic 详解 Claude AI 的沙盒技术](#item-8) ⭐️ 8.0/10
9. [通过 Pyodide 和服务线程在浏览器中运行 Python ASGI 应用](#item-9) ⭐️ 8.0/10
10. [FROST 攻击利用 SSD 计时窥探浏览活动](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [微软将永久授权的 Office for Mac 降级为只读模式](https://consumerrights.wiki/w/Microsoft_Office_2019_and_2021_for_Mac_view-only_conversion_(2026)) ⭐️ 9.0/10

微软宣布，从 2026 年起，永久授权的 Office 2019 和 2021 for Mac 将转换为只读模式，用户若无 Microsoft 365 订阅则无法进行编辑。 这一举措削弱了永久授权模式，通过追溯性地降低已购买软件的功能，迫使用户转向订阅制，并引发了重大的消费者权益担忧。 该转换专门适用于 Office 2019 和 2021 for Mac，编辑功能需要 Microsoft 365 订阅；查看模式仅允许查看和打印，无法编辑。

hackernews · antipurist · May 30, 23:26 · [社区讨论](https://news.ycombinator.com/item?id=48341578)

**背景**: 永久软件授权允许用户无限期使用特定版本的软件，传统上不会过期或丧失功能。查看模式是微软的一项功能，当检测到无有效许可证时，将 Office 应用限制为只读访问，通常用于未授权用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Software_license">Software license - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/microsoft-365-apps/licensing-activation/overview-viewer-mode">Overview of viewer mode for Microsoft 365 Apps - Microsoft 365 Apps | Microsoft Learn</a></li>
<li><a href="https://www.techtarget.com/whatis/definition/perpetual-software-license">What Is a Perpetual Software License ? – Definition from TechTarget</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了愤怒，许多人呼吁抵制并转向 LibreOffice 等替代品。一些人指出这可能违反澳大利亚消费者法，而另一些人猜测这一变化是为了强制对 AI 代理使用进行授权。

**标签**: `#Microsoft`, `#Office`, `#software licensing`, `#consumer rights`, `#perpetual license`

---

<a id="item-2"></a>
## [埃森哲以 12 亿美元收购 Ookla](https://newsroom.accenture.com/news/2026/accenture-to-acquire-ookla-to-strengthen-network-intelligence-and-experience-with-data-and-ai-for-enterprises) ⭐️ 8.0/10

埃森哲宣布以约 12 亿美元收购 Ookla，后者是 Speedtest 和 Downdetector 的母公司。此次收购旨在增强埃森哲的网络智能和 AI 驱动服务能力。 此次收购使埃森哲能够获取海量真实网络性能数据，从而为电信运营商和企业提供更深度的洞察和 AI 驱动的优化。这凸显了专有数据在咨询和 IT 服务行业中日益增长的价值。 Ookla 平台每月收集超过 2.5 亿次用户发起的测试，外加受控的驾车、步行和嵌入式测试。交易涵盖 Speedtest、Downdetector、Ekahau 和 RootMetrics 等品牌。

hackernews · Garbage · May 30, 16:28 · [社区讨论](https://news.ycombinator.com/item?id=48337987)

**背景**: Ookla 以 Speedtest.net 闻名，这是一个广泛使用的网络测速工具。然而，其核心业务是向电信公司出售聚合的网络性能数据。埃森哲此前已通过收购 Umlaut 进入该领域，因此本次交易是对竞争资产的整合。

**社区讨论**: 评论者强调，这笔交易本质上是一次数据收购，Ookla 的真正价值在于向电信运营商出售网络数据。有人对 12 亿美元的价格表示惊讶，也有人从内部视角分享了对该公司收入模式和竞争格局的看法。

**标签**: `#acquisition`, `#network intelligence`, `#data`, `#telco`, `#AI`

---

<a id="item-3"></a>
## [Voxel Space 渲染算法详解](https://s-macke.github.io/VoxelSpace/) ⭐️ 8.0/10

一个技术演示和解释页面发布了，展示了 1992 年游戏《Comanche》中使用的 Voxel Space 地形渲染算法，核心代码不到 20 行。 该算法展示了一种高效的 2.5D 渲染技术，使得 90 年代初的硬件能够呈现逼真的地形，激励了复古计算爱好者和游戏开发者探索类似方法。 Voxel Space 算法并非真正的体素渲染；它使用高度图配合彩色列和光线投射，类似于 2.5D 引擎。核心渲染循环不到 20 行代码。

hackernews · davikr · May 30, 14:25 · [社区讨论](https://news.ycombinator.com/item?id=48336564)

**背景**: Voxel Space 是一种 2.5D 地形渲染技术，将地形表示为高度图和颜色图，渲染像素列而非三角形。该技术用于 1992 年的游戏《Comanche》，在有限硬件上实现了逼真的地形。与真正的 3D 体素不同，它只能从上方视角观察，不具备完整的 3D 自由度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/s-macke/VoxelSpace">GitHub - s-macke/VoxelSpace: Terrain rendering algorithm in less than ...</a></li>
<li><a href="https://jbaker.graphics/writings/voxelspace.html">Voxelspace in a Compute Shader - jbaker.graphics</a></li>

</ul>
</details>

**社区讨论**: 评论者澄清该技术是高度图而非真正的体素，并分享了个人项目，如移植到 AGS 引擎和使用原始地图的 C++版本。有些人回忆了该游戏的历史影响以及从第一个任务中获得的极简测试方法论启发。

**标签**: `#graphics`, `#rendering`, `#retro-computing`, `#game-development`, `#algorithms`

---

<a id="item-4"></a>
## [Zig ELF 链接器改进提升增量编译能力](https://ziglang.org/devlog/2026/#2026-05-30) ⭐️ 8.0/10

这些改进使 Zig 成为更可行的 C 语言替代品，有可能让开发者在保持 C 或 Rust 级别性能的同时，以高级语言的速度进行迭代。 该开发日志侧重于增量链接，仅重新链接更改的部分，极大地加快了编辑-编译-测试循环，但它可能与链接时优化（LTO）互斥。

hackernews · kristoff_it · May 30, 17:29 · [社区讨论](https://news.ycombinator.com/item?id=48338673)

**背景**: ELF（可执行与可链接格式）链接器是一种将目标文件组合成单个可执行文件或库的工具。增量编译仅重新编译程序中已修改的部分，而非整个项目，从而实现更快的开发周期。Zig 是一种系统编程语言，旨在成为 C 语言的现代替代品，具有更好的安全性和构建系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Executable_and_Linkable_Format">Executable and Linkable Format - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Incremental_compilation">Incremental compilation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Incremental_compiler">Incremental compiler - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区高度热情，评论认为链接器是 Zig 成为“C 语言替代品”的关键一步。开发者正在考虑将 Zig 作为转译目标，并讨论将 Raku 的 MOARVM 等虚拟机移植到 Zig。一位评论者提出了与链接时优化的权衡。

**标签**: `#Zig`, `#linker`, `#compiler`, `#systems programming`, `#devlog`

---

<a id="item-5"></a>
## [OpenRouter 获 1.13 亿美元 B 轮融资](https://openrouter.ai/announcements/series-b) ⭐️ 8.0/10

OpenRouter 宣布完成 1.13 亿美元 B 轮融资，由 CapitalG 领投，NVentures、ServiceNow Ventures、MongoDB Ventures、Snowflake Ventures、Databricks Ventures、AMP PBC 和 Pace Capital 参投，现有投资方 Andreessen Horowitz 和 Menlo Ventures 继续跟投。 这一大额投资凸显了 OpenRouter 作为大语言模型统一 API 代理的关键作用，它简化了 400 多个模型的访问，降低了开发者的使用门槛。这笔资金将帮助 OpenRouter 扩展基础设施和服务，可能加速 AI 在开发者生态中的普及。 OpenRouter 的服务包括计费上限等许多模型提供商尚未提供的功能，并收取相对于原始提供商成本的小幅加价（约 5%）。联合创始人强调公司仍由创始人主导和控制，计划利用这笔资金为长期发展建立稳固的财务基础。

hackernews · freeCandy · May 30, 17:27 · [社区讨论](https://news.ycombinator.com/item?id=48338660)

**背景**: OpenRouter 是一项提供统一 API 的服务，用于访问来自不同提供商的数百种大语言模型（LLM），让开发者无需集成多个不同的 API 即可轻松切换模型。它充当代理角色，提供计费上限、日志记录和模型回退等额外功能。随着 LLM 领域快速发展，众多新模型涌现，OpenRouter 降低了开发者尝试不同模型的摩擦。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/">OpenRouter</a></li>
<li><a href="https://www.codecademy.com/article/what-is-openrouter">What is OpenRouter? A Guide with Practical Examples</a></li>

</ul>
</details>

**社区讨论**: 社区成员如 simonw 强调 OpenRouter 的低摩擦和计费上限是主要优势，联合创始人 numlocked 回应了融资问题，强调创始人控制和长期愿景。一些评论者对 5% 加价的可持续性和未来的整合表示担忧，但总体情绪积极，认可 OpenRouter 在尝试多种模型方面的实用性。

**标签**: `#AI infrastructure`, `#LLM API`, `#funding`, `#OpenRouter`, `#AI tools`

---

<a id="item-6"></a>
## [Openrsync：OpenBSD 注重安全的 rsync 实现](https://github.com/kristapsdz/openrsync) ⭐️ 8.0/10

Openrsync 是 OpenBSD 团队开发的一个新的 rsync 工具实现，通过使用 pledge 和 unveil 系统调用来强调安全性。该工具正在作为 RPKI 验证器的一部分进行开发。 该实现旨在为广泛使用的 rsync 提供一个更安全的替代方案，可能减少文件同步中的漏洞。它已在社区中获得关注，并引发了关于安全特性和可移植性的讨论。 Openrsync 目前不支持所有 rsync 功能；例如，它在 --rsync-path 选项行为上存在已知问题。它主要在 OpenBSD 上开发，并依赖 OpenBSD 的 pledge 和 unveil 进行沙箱隔离。

hackernews · sph · May 30, 10:51 · [社区讨论](https://news.ycombinator.com/item?id=48334854)

**背景**: Rsync 是一种用于高效传输和同步文件的流行工具。OpenBSD 的 pledge 和 unveil 是系统调用，允许程序限制其对系统资源的访问，通过限制潜在漏洞利用的损害来增强安全性。Openrsync 利用这些特性提供了一个加固的 rsync 替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://man.openbsd.org/pledge.2">pledge(2) - OpenBSD manual pages</a></li>
<li><a href="https://lwn.net/Articles/767137/">OpenBSD's unveil() - LWN.net</a></li>

</ul>
</details>

**社区讨论**: 用户反馈 openrsync 正在改进，但与 Samba 的 rsync 相比仍有差距，例如在 --rsync-path 方面。一些人提到它是在 RPKI 验证器背景下开发的。其他人则提到了替代实现，如 Michael Stapelberg 的 Go 版本。讨论强调了 pledge/unveil 对安全的重要性。

**标签**: `#rsync`, `#OpenBSD`, `#security`, `#implementation`

---

<a id="item-7"></a>
## [教宗利奥首道通谕抨击技术救世主义](https://www.economist.com/europe/2026/05/28/leos-first-encyclical-attacks-technological-messianism) ⭐️ 8.0/10

教宗利奥十四世于 2026 年 5 月 28 日发布其首道通谕，批评认为技术能够带来救赎的信念，并将其称为'技术救世主义'。 这道通谕标志着天主教会对 AI 伦理讨论的重大介入，针对科技领袖宣扬的类宗教或超人类主义叙事。 通谕并未全盘否定技术，而是警告不应将其视为终极救赎之源，呼应了此前教宗对技术进步伦理边界的关切。

hackernews · 1vuio0pswjnm7 · May 30, 10:30 · [社区讨论](https://news.ycombinator.com/item?id=48334710)

**背景**: 技术救世主义指认为仅凭技术进步就能解决人类最深层次问题并带来乌托邦未来的信念。天主教会历史上曾与现代意识形态交锋，这道通谕延续了这一传统，回应了围绕 AI 和超人类主义的准宗教狂热。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.biomedima.org/techno-messianism/">Techno- Messianism | BioMedima</a></li>
<li><a href="https://en.wikipedia.org/wiki/Transhumanism">Transhumanism</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍欢迎教宗的批评，部分人指出其与彼得·蒂尔等人物讨论 AI 与敌基督的相关性。还有人辩论技术的适当控制权应属于创造者、用户、政府还是宗教机构。

**标签**: `#religion`, `#AI ethics`, `#technology critique`, `#transhumanism`

---

<a id="item-8"></a>
## [Anthropic 详解 Claude AI 的沙盒技术](https://simonwillison.net/2026/May/30/how-we-contain-claude/#atom-everything) ⭐️ 8.0/10

Anthropic 发布了一份详细的技术概述，介绍了在 Claude.ai、Claude Code 和 Cowork 中用于隔离 Claude 的沙盒方法，包括 gVisor、Seatbelt、Bubblewrap 和完整虚拟机。 这填补了 AI 沙盒文档中常见的空白，帮助用户和开发者更好地理解和信任 Claude 产品的安全边界。 Claude.ai 使用 gVisor，Claude Code 在 macOS 上使用 Seatbelt，在 Linux 上使用 Bubblewrap，而 Claude Cowork 运行完整的虚拟机。文章还讨论了之前报道过的通过 api.anthropic.com/v1/files 进行的数据外泄途径。

rss · Simon Willison · May 30, 21:36

**背景**: 沙盒是一种安全技术，用于隔离应用程序以限制其对系统资源的访问。gVisor 是谷歌开发的容器沙盒，它在用户空间实现 Linux 系统调用。Seatbelt 是 macOS 的原生沙盒工具，Bubblewrap 是 Flatpak 使用的轻量级 Linux 沙盒。这些工具有助于防止恶意代码或 AI 代理访问敏感数据或造成损害。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GVisor">gVisor - Wikipedia</a></li>
<li><a href="https://github.com/michaelneale/agent-seatbelt-sandbox">GitHub - michaelneale/agent-seatbelt-sandbox: using native macos sandboxing to stop data egress · GitHub</a></li>
<li><a href="https://github.com/containers/bubblewrap">GitHub - containers/bubblewrap: Low-level unprivileged sandboxing tool used by Flatpak and similar projects · GitHub</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#sandboxing`, `#Claude`, `#security`, `#gVisor`

---

<a id="item-9"></a>
## [通过 Pyodide 和服务线程在浏览器中运行 Python ASGI 应用](https://simonwillison.net/2026/May/30/pyodide-asgi-browser/#atom-everything) ⭐️ 8.0/10

Simon Willison 展示了使用 Pyodide 和服务线程（而非 Web Worker）在浏览器中运行 Python ASGI 应用的方法，克服了 Web Worker 无法执行 <script> 标签的限制。他提供了基础 ASGI FastCGI 应用和 Datasette 1.0a31 在浏览器中运行的演示。 这种方法使得更丰富的 Python Web 应用能够完全在浏览器中运行，包括那些依赖 JavaScript 插件的应用，而无需服务器。它可能显著扩展 Datasette Lite 等基于浏览器的 Python 环境的能力。 该解决方案使用服务线程拦截网络请求，并在 Pyodide 内部执行 Python ASGI 应用，使得 <script> 标签中的 JavaScript 能够正常执行。该项目是在 Claude Opus 4.8 通过 Claude Code for web 的协助下完成的。

rss · Simon Willison · May 30, 21:02

**背景**: Pyodide 是一个基于 WebAssembly 的浏览器端 Python 发行版，允许 Python 代码在客户端运行。ASGI（异步服务器网关接口）是异步 Python Web 应用的标准。Web Worker 在后台线程运行脚本，但无法访问 DOM 或执行内联 JavaScript，而服务线程可以拦截网络请求并持久运行，从而实现完整的页面功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pyodide.org/">Pyodide — Version 0.29.4</a></li>
<li><a href="https://en.wikipedia.org/wiki/ASGI">ASGI</a></li>
<li><a href="https://web.dev/learn/pwa/service-workers">Service workers | web.dev</a></li>

</ul>
</details>

**标签**: `#Pyodide`, `#ASGI`, `#Service Workers`, `#WebAssembly`, `#Python`

---

<a id="item-10"></a>
## [FROST 攻击利用 SSD 计时窥探浏览活动](https://futurism.com/future-society/websites-spying-solid-state-drive) ⭐️ 8.0/10

研究人员披露了 FROST 攻击，该攻击利用浏览器的 Origin Private File System (OPFS) API 测量 SSD 读写计时，以高准确率（网站 88.95%，应用 95.83%）推断受害者打开的网站和应用，无需任何权限或用户交互。 该攻击通过利用先前被忽视的硬件资源（SSD）和合法的浏览器 API，显著扩展了浏览器侧信道威胁的范围，对可能同时打开敏感标签页的用户构成严重的隐私风险。 研究人员通过创建大于系统内存的文件绕过操作系统缓存，确保磁盘访问触及物理 SSD。该攻击目前在 Mac 和 Linux 上有效；Windows 并非免疫但未经测试。启用跨源隔离策略可恢复高精度计时器以提高准确率。

telegram · zaihuapd · May 31, 01:55

**背景**: 侧信道攻击利用间接信息（如时间或功耗）来推断秘密。Origin Private File System (OPFS) 是一种浏览器 API，允许 Web 应用在用户设备的沙盒文件系统中存储数据。通过测量 OPFS 读写操作所需的时间，攻击者可以检测到由其他进程引起的 SSD 资源竞争，从而揭示哪些网站或应用正在活动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/cyber-security/researchers-say-they-can-spy-on-your-browsing-by-measuring-ssd-activity-through-a-browser-api">Researchers say they can spy on your browsing by measuring SSD activity through a browser API — claim FROST attack requires no permissions or user interaction to identify which apps and websites you're using | Tom's Hardware</a></li>
<li><a href="https://arstechnica.com/security/2026/05/websites-have-a-new-way-to-spy-on-visitors-analyzing-their-ssd-activity/">Websites have a new way to spy on visitors: Analyzing their SSD activity - Ars Technica</a></li>
<li><a href="https://cyberinsider.com/new-frost-attack-leverages-ssd-side-channel-to-reveal-browsing-activity/">New FROST attack leverages SSD side-channel to reveal browsing activity</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#side-channel attack`, `#privacy`, `#SSD`, `#browser security`

---