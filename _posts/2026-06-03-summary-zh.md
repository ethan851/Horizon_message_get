---
layout: default
title: "Horizon Summary: 2026-06-03 (ZH)"
date: 2026-06-03
lang: zh
---

> From 35 items, 5 important content pieces were selected

---

1. [Anthropic 将 Project Glasswing 扩展至 15 个国家](#item-1) ⭐️ 8.0/10
2. [KDE Plasma 为最后支持 X11 的版本做准备](#item-2) ⭐️ 8.0/10
3. [微软发布 MAI-Thinking-1 和 MAI-Code-1-Flash 模型](#item-3) ⭐️ 8.0/10
4. [特朗普签署 AI 行政令，要求企业自愿提交模型审查](#item-4) ⭐️ 8.0/10
5. [Google 向 Play Store 开发者付费获取私有代码以训练 AI](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic 将 Project Glasswing 扩展至 15 个国家](https://www.anthropic.com/news/expanding-project-glasswing) ⭐️ 8.0/10

Anthropic 已扩大 Project Glasswing 项目，将其未发布的 Claude Mythos 模型部署到 15 个国家的 150 个组织，用于保护关键基础设施安全。 这标志着在利用人工智能保护关键基础设施方面迈出了重要一步，但社区反馈显示了对误报、访问限制以及关于算力能力的潜在动机的担忧。 Claude Mythos 是一款专注于漏洞检测和渗透测试的未发布前沿模型。Anthropic 已承诺提供 1 亿美元的模型使用额度来支持该项目。

hackernews · surprisetalk · Jun 2, 13:15 · [社区讨论](https://news.ycombinator.com/item?id=48369863)

**背景**: Project Glasswing 是 Anthropic 的一项计划，通过与负责基础系统的组织合作，为 AI 时代保障关键软件安全。Claude Mythos 是一款前沿级编码模型，能够识别二进制文件和端点中的漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing: Securing critical software for the AI era \ Anthropic</a></li>
<li><a href="https://techcrunch.com/2026/06/02/anthropic-scales-claude-mythos-to-critical-infrastructure-in-15-countries/">Anthropic scales Claude Mythos to critical infrastructure in 15+ countries</a></li>

</ul>
</details>

**社区讨论**: 第一手报告显示该工具产生了大量噪声和误报；一些评论者怀疑 Anthropic 限制公共访问是出于算力不足而非安全考虑。一家财富 50 强企业的安全团队表示，尽管多次请求，仍无法获得访问权限。

**标签**: `#AI`, `#security`, `#infrastructure`, `#Anthropic`, `#critical systems`

---

<a id="item-2"></a>
## [KDE Plasma 为最后支持 X11 的版本做准备](https://blog.davidedmundson.co.uk/blog/596/) ⭐️ 8.0/10

KDE Plasma 宣布其即将发布的版本将是最后一个支持 X11 显示服务器的版本，标志着完全转向 Wayland。 此举将 Linux 桌面开发整合到 Wayland 上，提高了安全性并现代化了图形栈，但可能会影响依赖 X11 特定功能的用户。 这一决定使 KDE 能够通过移除 X11 代码路径来简化代码库，从而在 Wayland 上实现更快的创新和更好的性能。

hackernews · jandeboevrie · Jun 2, 14:16 · [社区讨论](https://news.ycombinator.com/item?id=48370588)

**背景**: X11 几十年来一直是类 Unix 系统的默认显示服务器协议，但存在安全性和性能限制。Wayland 被设计为现代替代方案，具有更简单的架构和更好的安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wayland_(display_server_protocol)">Wayland (display server protocol)</a></li>
<li><a href="https://en.wikipedia.org/wiki/X11_Window_System">X11 Window System</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了复杂的感受：一些人称赞 KDE 在 Wayland 上的进步和更流畅的性能，而另一些人则强调了显著的倒退，例如缺少无障碍支持和如画中画窗口管理等功能的损坏。

**标签**: `#KDE`, `#Wayland`, `#X11`, `#Linux Desktop`, `#Open Source`

---

<a id="item-3"></a>
## [微软发布 MAI-Thinking-1 和 MAI-Code-1-Flash 模型](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 8.0/10

微软发布了两个新的大语言模型：MAI-Thinking-1（推理模型，总参数 1 万亿，激活参数 350 亿）和 MAI-Code-1-Flash（代码专用模型，总参数 1370 亿，激活参数 50 亿），专为 GitHub Copilot 优化。 这些模型以较低的激活参数实现了有竞争力的性能，可能降低推理成本。它们也凸显了微软对专有商业授权训练数据的投入，不过仍依赖于网络爬取数据。 MAI-Thinking-1 采用混合专家（MoE）架构，每个 token 仅激活 1 万亿参数中的 350 亿。MAI-Code-1-Flash 总参数 1370 亿，激活 50 亿。两者均基于专有网络爬取和 Common Crawl 数据训练，并非完全使用授权数据。

rss · Simon Willison · Jun 2, 22:21

**背景**: 在大语言模型中，总参数指模型完整大小，而激活参数指单次前向推理中实际使用的参数，尤其在混合专家（MoE）架构中。MoE 模型包含多个“专家”子网络，每个 token 仅激活部分专家，从而在低计算成本下实现高容量。理解这一区别对评估新模型的性能和效率至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.f22labs.com/blogs/active-vs-total-parameters-whats-the-difference/">Active vs Total Parameters : What’s the Difference?</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA Technical Blog</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#Microsoft`, `#coding`

---

<a id="item-4"></a>
## [特朗普签署 AI 行政令，要求企业自愿提交模型审查](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/) ⭐️ 8.0/10

2026 年 6 月 2 日，特朗普总统签署了一项行政命令，建立自愿性框架，要求 AI 开发者在公开发布“受保护的尖端模型”前至少 30 天提交给政府进行网络安全审查。该命令还指示建立 AI 网络安全清算所，以协调漏洞扫描和修复。 这项行政命令代表了美国政府直接应对 AI 风险的行动，在国家安全与行业创新之间取得平衡。它可能为未来的 AI 监管开创先例，并影响主要 AI 公司发布最先进模型的方式。 审查期从最初提议的 90 天缩短至 30 天，原因是行业压力和白宫内部意见分歧。该命令明确禁止强制性的政府许可或预检机制，强调自愿的公私合作伙伴关系。

telegram · zaihuapd · Jun 2, 16:44

**背景**: 行政命令是美国总统发布的管理联邦政府运作的指令。“受保护的尖端模型”指那些如果在没有保障措施的情况下发布可能带来网络安全风险的先进 AI 系统。自愿性框架意味着公司可以选择提交模型进行审查，但法律上并不强制要求。AI 网络安全清算所将协调寻找和修复联邦系统软件漏洞的工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://federalnewsnetwork.com/cybersecurity/2026/06/ai-executive-order-sets-stage-for-new-cybersecurity-directives/">AI executive order sets stage for new cybersecurity directives</a></li>
<li><a href="https://www.aba.com/about-us/press-room/press-releases/aba-statement-on-executive-order-promoting-advanced-ai-innovation-and-security">ABA Statement on Executive Order Promoting Advanced AI Innovation ...</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#US government`, `#cybersecurity`, `#executive order`

---

<a id="item-5"></a>
## [Google 向 Play Store 开发者付费获取私有代码以训练 AI](https://www.neowin.net/reports/google-wants-to-pay-play-store-developers-for-code-to-train-its-ai/) ⭐️ 8.0/10

Google 私下联系 Android 开发者，提议付费获取其私有代码库的使用权，用于训练 Gemini AI 和改进开发工具，开发者保留全部知识产权。 这一举措可能使 Google 在缩小 Gemini 与 GitHub Copilot、Claude Code 等竞品差距上获得显著优势，并可能重塑 AI 辅助开发领域的格局。 该提议涉及开发者授予非独家许可，允许 Google 将其代码用于 AI 训练，而 Google 不保留任何所有权。该计划目前通过私下联系 Play Store 开发者逐步推行。

telegram · zaihuapd · Jun 3, 02:47

**背景**: 像 Google 的 Gemini 这样的大型语言模型需要大量高质量代码来提升其辅助开发者的能力。GitHub Copilot（由 OpenAI 驱动）和 Anthropic 的 Claude Code 等竞争对手已经通过使用大量代码库（通常来自公开仓库）训练，确立了强势地位。Google 通过付费获取私有代码的策略可能为其提供独特且高价值的训练数据，从而加速其 AI 开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://antigravity.google/product/antigravity-2">Google Antigravity - Antigravity 2 . 0</a></li>

</ul>
</details>

**标签**: `#Google`, `#AI`, `#Android`, `#Developer Tools`, `#Training Data`

---