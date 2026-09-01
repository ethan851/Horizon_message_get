---
layout: default
title: "Horizon Summary: 2026-09-01 (ZH)"
date: 2026-09-01
lang: zh
---

> From 29 items, 6 important content pieces were selected

---

1. [指南记录 ChatGPT Work 工具与 Playwright 浏览器技能](#item-1) ⭐️ 8.0/10
2. [谷歌从 Chrome 网上应用店移除 Manifest V2 扩展，包括 uBlock Origin](#item-2) ⭐️ 8.0/10
3. [OpenClaw 2.0 发布史上最大更新，合并逾 1.6 万个拉取请求](#item-3) ⭐️ 8.0/10
4. [苹果官宣换帅：库克卸任 CEO，特努斯接任](#item-4) ⭐️ 8.0/10
5. [欧盟将 ChatGPT、Reddit、Roblox 认定为超大型服务，强化 DSA 监管](#item-5) ⭐️ 8.0/10
6. [小米发布玄戒 O3、O100、D100 三款芯片，覆盖手机、AI 与智驾](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [指南记录 ChatGPT Work 工具与 Playwright 浏览器技能](https://codex-tool-reference.simonw.chatgpt.site/) ⭐️ 8.0/10

开发者 Simon Willison 发布了一份由社区引用的指南，记录 ChatGPT Work 的工具和技能，其中重点介绍了一项引人注目的 control-browser 技能，该技能通过 Node.js REPL 使用 Playwright 驱动浏览器。 这份指南展示了如何通过可复用的技能扩展 ChatGPT Work，尤其是浏览器自动化方面的能力，这可能显著提升 AI 代理工作流和开发者的生产力。 control-browser 技能指示 ChatGPT Work 通过其 Node.js REPL 启动 Playwright 实例，并执行 `nodeRepl.write(await browser.documentation());` 以获取进一步说明。该参考站点还记录了其他工具和技能，社区评论中提到可能存在 token 浪费以及与 Codex 的重叠。

hackernews · ijidak · Aug 31, 14:07 · [社区讨论](https://news.ycombinator.com/item?id=49510000)

**背景**: ChatGPT Work 是 OpenAI 面向企业推出的产品，它整合团队工具中的上下文来完成任务，由 GPT-5.6 等模型驱动。技能（Skills）是可重用、可共享的工作流，包含指令、示例和代码，使 ChatGPT 能够一致地完成特定任务。Playwright 是一个浏览器自动化框架，支持驱动 Chromium、Firefox 和 WebKit，常用于端到端测试和 AI 代理工作流。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://help.openai.com/en/articles/20001066-skills-in-chatgpt">Skills in ChatGPT | OpenAI Help Center</a></li>
<li><a href="https://playwright.dev/">Fast and reliable end-to-end testing for modern web apps | Playwright</a></li>
<li><a href="https://openai.com/chatgpt-work/">ChatGPT Work for every team | OpenAI</a></li>

</ul>
</details>

**社区讨论**: Simon Willison 指出 control-browser 技能最有趣，并解释了其自文档化机制。一些评论者质疑它与 Codex 有何不同，另一些人则警告这些工作工具可能拖慢流程并消耗大量 token。还有一条元评论指出，AI 生成的内容往往有相似的视觉风格，让人想起 Bootstrap 时代。

**标签**: `#ChatGPT`, `#AI tools`, `#Playwright`, `#Developer tools`, `#Simon Willison`

---

<a id="item-2"></a>
## [谷歌从 Chrome 网上应用店移除 Manifest V2 扩展，包括 uBlock Origin](https://webiterate.dev/google-removed-extensions-ublock-origin-108/) ⭐️ 8.0/10

谷歌已从 Chrome 网上应用店移除 Manifest V2 (MV2)扩展，包括广受欢迎的广告拦截器 uBlock Origin。这标志着多年前开始的 MV2 到 Manifest V3 (MV3)迁移进入最后阶段。 这影响了数百万依赖 uBlock Origin 进行广告拦截和隐私保护的 Chrome 用户。用户正被推向 Firefox 等仍支持 MV2 扩展的浏览器，突显了对浏览器垄断和用户选择的担忧。 Manifest V3 用仅在需要时运行的服务工作者替代 MV2 的长驻后台页面，这限制了 uBlock Origin 等扩展拦截网络请求的方式。uBlock Origin 开发者建议使用 Firefox，该扩展在 Firefox 上仍能最佳运行。

hackernews · twapi · Aug 31, 21:10 · [社区讨论](https://news.ycombinator.com/item?id=49514878)

**背景**: Chrome 扩展基于声明权限和能力的清单文件构建。谷歌于 2012 年推出 Manifest V2，后来提出 MV3 以改善安全、性能和用户隐私。然而，MV3 的 declarativeNetRequest API 限制了过滤规则数量，并用更有限的模型替代了阻塞网络请求的方式。uBlock Origin 是由 Raymond Hill 开发的免费开源、高效的内容拦截器，适用于 Chromium 和 Firefox。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V3 | Chrome for Developers</a></li>
<li><a href="https://en.wikipedia.org/wiki/UBlock_Origin">uBlock Origin - Wikipedia</a></li>
<li><a href="https://github.com/gorhill/uBlock">GitHub - gorhill/uBlock: uBlock Origin - An efficient blocker for Chromium and Firefox. Fast and lean. · GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对谷歌的决定表示不满，并建议改用 Firefox。一些人强调广告拦截已成为不太懂技术的用户的安全问题，还有人指出 uBlock Origin 在 Firefox 上始终表现更好。整体情绪是批评 Chrome、支持 Firefox。

**标签**: `#Chrome`, `#Manifest V2`, `#uBlock Origin`, `#WebExtensions`, `#Privacy`

---

<a id="item-3"></a>
## [OpenClaw 2.0 发布史上最大更新，合并逾 1.6 万个拉取请求](https://openclaw.ai/blog/openclaw-2-accidentally) ⭐️ 8.0/10

8 月 30 日，OpenClaw 发布了史上最大更新 2.0 版本，合并了来自 933 名贡献者（含 569 名首次参与者）的逾 1.6 万个拉取请求。该版本全面重做了安装、消息、记忆、技能、模型、浏览器、插件与安全等环节，并新增共享云端会话以支持多人协作。 这标志着 GitHub 上增长最快的开源 AI 助手项目之一迎来了重要里程碑，也体现了该项目庞大而活跃的贡献者社区。此次大规模功能重构可能让 OpenClaw 更易上手、更利于协作，有望加速开发者与 AI 智能体用户的采用。 为了准备这次更新，团队近七周未发布新版本；此次合并的 1.6 万个拉取请求约占项目迄今全部拉取请求的一半。更新还简化了安装流程，重建了浏览器端体验，并引入了支持多人协作的共享云端会话。

telegram · zaihuapd · Aug 31, 04:38

**背景**: OpenClaw 是一个开源个人 AI 助手项目，已成为 GitHub 上增长最快的仓库之一，由数十名维护者和数千名贡献者共同构建个人智能体。它通过技能（Skills）、插件（Plugins）、渠道、模型提供商、工具等能力实现高度可扩展。该项目在完成首次更名后，因其 AI 智能体社交网络 Moltbook 的病毒式传播而关注度大增。拉取请求（Pull Request）是 GitHub 上贡献者提交代码修改、供维护者审核并合并的机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openclaw.ai/">OpenClaw — Open-Source AI Assistant</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw - Wikipedia</a></li>
<li><a href="https://docs.openclaw.ai/tools">Overview · OpenClaw</a></li>

</ul>
</details>

**标签**: `#OpenClaw`, `#open source`, `#AI assistant`, `#release`, `#software update`

---

<a id="item-4"></a>
## [苹果官宣换帅：库克卸任 CEO，特努斯接任](https://t.me/zaihuapd/43516) ⭐️ 8.0/10

苹果宣布管理层交接，现任 CEO 蒂姆·库克将出任董事会执行董事长，硬件工程高级副总裁约翰·特努斯将于 2026 年 9 月 1 日起担任新任 CEO。 这是全球最具影响力的科技公司之一的高层重大变动，将影响苹果的产品战略和整个开发者生态。这标志着苹果领导层的代际更替。 董事会已一致批准这项安排，库克将在整个夏天继续担任 CEO，与特努斯完成过渡。现任董事长 Arthur Levinson 将于 9 月 1 日转任首席独立董事，特努斯同日加入董事会。特努斯 2001 年加入苹果，2013 年升任硬件工程副总裁，2021 年进入高管团队。

telegram · zaihuapd · Aug 31, 10:21

**背景**: 蒂姆·库克自 2011 年起担任苹果 CEO，期间苹果市值增长至约 3 万亿美元。约翰·特努斯是苹果资深硬件高管，负责 iPhone、Mac、iPad、AirPods 等产品。这次交接是苹果有序继任计划的一部分。

**标签**: `#Apple`, `#CEO transition`, `#Tim Cook`, `#John Ternus`, `#tech industry`

---

<a id="item-5"></a>
## [欧盟将 ChatGPT、Reddit、Roblox 认定为超大型服务，强化 DSA 监管](https://www.euronews.com/next/2026/08/31/eu-places-chatgpt-reddit-and-roblox-under-strictest-digital-safety-rules) ⭐️ 8.0/10

8 月 31 日，欧盟委员会依据《数字服务法》（DSA）将 OpenAI 的 ChatGPT 认定为超大型在线搜索引擎，并将 Reddit 和 Roblox 认定为超大型在线平台，因为这三项服务在欧盟的月均活跃用户均超过 4500 万。 这是 AI 聊天机器人首次被划入 DSA 的严格监管层级，意味着欧盟的内容安全监管延伸至生成式 AI 以及高使用量的社区平台。该认定迫使这些服务主动应对非法内容、未成年人保护和用户身心健康等系统性风险，为全球类似监管开创了先例。 这三项服务有四个月的过渡期来完成合规。它们必须开展年度系统性风险评估、接受独立审计，并与欧盟监管机构及经审核的研究人员共享数据，重点涉及非法内容、未成年人保护和用户身心健康风险。

telegram · zaihuapd · Aug 31, 14:39

**背景**: 《数字服务法》（DSA）是欧盟针对数字服务制定的法规，对在欧盟月均活跃用户至少 4500 万（约占欧盟人口 10%）的超大型在线平台（VLOP）和超大型在线搜索引擎（VLOSE）施加更严格的义务。DSA 旨在营造更安全、更透明的在线环境，要求这些超大型服务评估并降低与其运营相关的系统性风险，例如非法内容和虚假信息的传播。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pdf.hanspub.org/ojls2025132_72923414.pdf">欧 盟 《数字服务法案》解读及对我国 的 启示</a></li>
<li><a href="https://www.tmtpost.com/6653184.html">欧 盟 《数字服务法》倒计时： 超 大 平 台 各寻门路-钛媒体官方网站</a></li>

</ul>
</details>

**标签**: `#AI治理`, `#DSA`, `#欧盟`, `#平台监管`

---

<a id="item-6"></a>
## [小米发布玄戒 O3、O100、D100 三款芯片，覆盖手机、AI 与智驾](https://t.me/zaihuapd/43524) ⭐️ 8.0/10

小米发布了三款新一代玄戒芯片：AI 旗舰 SoC 玄戒 O3、带宽达 1.22 TB/s 的高带宽 AI 加速芯片玄戒 O100，以及号称国内首款 3nm 智驾 AI 芯片玄戒 D100。三款芯片均已完成回片验证，面向小米人车家全生态的端侧 AI 算力需求；其中 O3 将首发搭载于小米 18 Fold。 这是小米深化自研芯片战略、在智能手机、智能汽车和智能家居的 AI 计算领域全面竞争的重要一步。旗舰移动 SoC 与 3nm 智驾 AI 芯片的组合，显示出小米希望在端侧 AI 和智能驾驶硬件上成为重要参与者。 玄戒 O3 采用十核全大核 CPU，多核跑分首次突破 15000 分；其 GPU 为 Arm 的 G2-Ultra NX，据称相比上一代玄戒 O1 性能提升 85%、功耗降低 64%。O3 还被称为全球首款支持 LPDDR6 内存的移动处理器；O100 加速芯片面向 1.22 TB/s 高带宽场景，D100 则定位智驾 AI 算力。

telegram · zaihuapd · Aug 31, 15:15

**背景**: SoC（片上系统）把处理器、图形单元、内存控制器和 AI 加速部件集成在一颗芯片上，因而这些芯片可以为小米的多种设备提供算力。LPDDR6 是 JEDEC 发布的下一代内存标准，旨在大幅提升移动和 AI 工作负载的速度与能效，并加入了片内 ECC、错误清扫等可靠性特性。玄戒是小米的自研芯片系列，本次发布表明该系列正从手机扩展到 AI 加速器和车规级芯片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.jedec.org/news/pressreleases/jedec®-releases-new-lpddr6-standard-enhance-mobile-and-ai-memory-performance">JEDEC® Releases New LPDDR6 Standard to Enhance Mobile and AI Memory Performance | JEDEC</a></li>
<li><a href="https://gadgets.beebom.com/guides/xiaomi-xring-o3-benchmark-specs">Xiaomi Xring O3: Benchmarks and Specs | Beebom Gadgets</a></li>

</ul>
</details>

**标签**: `#chip`, `#AI`, `#Xiaomi`, `#SoC`, `#hardware`

---