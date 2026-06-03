---
layout: default
title: "Horizon Summary: 2026-06-03 (EN)"
date: 2026-06-03
lang: en
---

> From 35 items, 5 important content pieces were selected

---

1. [Anthropic Expands Project Glasswing to 15 Countries](#item-1) ⭐️ 8.0/10
2. [KDE Plasma Prepares for Last X11-Supported Release](#item-2) ⭐️ 8.0/10
3. [Microsoft Announces MAI-Thinking-1 and MAI-Code-1-Flash Models](#item-3) ⭐️ 8.0/10
4. [Trump Signs AI Executive Order, Voluntary Model Review](#item-4) ⭐️ 8.0/10
5. [Google to pay Play Store developers for private code to train AI](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Anthropic Expands Project Glasswing to 15 Countries](https://www.anthropic.com/news/expanding-project-glasswing) ⭐️ 8.0/10

Anthropic has expanded Project Glasswing, deploying its unreleased Claude Mythos model to secure critical infrastructure across 15 countries and 150 organizations. This marks a significant step in using AI for critical infrastructure defense, but community feedback reveals concerns about false positives, access limitations, and potential ulterior motives regarding compute capacity. Claude Mythos is an unreleased frontier model focused on vulnerability detection and penetration testing. Anthropic has committed $100 million in model usage credits to support the initiative.

hackernews · surprisetalk · Jun 2, 13:15 · [Discussion](https://news.ycombinator.com/item?id=48369863)

**Background**: Project Glasswing is Anthropic's initiative to secure critical software for the AI era by partnering with organizations responsible for foundational systems. Claude Mythos represents a frontier-level coding model that can identify vulnerabilities in binaries and endpoints.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing: Securing critical software for the AI era \ Anthropic</a></li>
<li><a href="https://techcrunch.com/2026/06/02/anthropic-scales-claude-mythos-to-critical-infrastructure-in-15-countries/">Anthropic scales Claude Mythos to critical infrastructure in 15+ countries</a></li>

</ul>
</details>

**Discussion**: First-hand reports indicate the tool generates excessive noise with many false positives, while some commenters suspect Anthropic is limiting public access due to compute shortages rather than security concerns. A Fortune 50 security team also reported being unable to obtain access despite repeated requests.

**Tags**: `#AI`, `#security`, `#infrastructure`, `#Anthropic`, `#critical systems`

---

<a id="item-2"></a>
## [KDE Plasma Prepares for Last X11-Supported Release](https://blog.davidedmundson.co.uk/blog/596/) ⭐️ 8.0/10

KDE Plasma announced that its upcoming release will be the last to support the X11 display server, marking a full transition to Wayland. This move consolidates Linux desktop development around Wayland, improving security and modernizing the graphics stack, but may impact users relying on X11-specific features. The decision allows KDE to simplify its codebase by removing X11 code paths, enabling faster innovation and better performance on Wayland.

hackernews · jandeboevrie · Jun 2, 14:16 · [Discussion](https://news.ycombinator.com/item?id=48370588)

**Background**: X11 was the default display server protocol for Unix-like systems for decades, but suffers from security and performance limitations. Wayland was designed as a modern replacement with simpler architecture and better security.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wayland_(display_server_protocol)">Wayland (display server protocol)</a></li>
<li><a href="https://en.wikipedia.org/wiki/X11_Window_System">X11 Window System</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed feelings: some praised KDE's progress on Wayland and smoother performance, while others highlighted significant regressions such as missing accessibility support and broken features like 'picture in picture' window management.

**Tags**: `#KDE`, `#Wayland`, `#X11`, `#Linux Desktop`, `#Open Source`

---

<a id="item-3"></a>
## [Microsoft Announces MAI-Thinking-1 and MAI-Code-1-Flash Models](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 8.0/10

Microsoft announced two new large language models: MAI-Thinking-1, a reasoning model with 1 trillion total parameters and 35 billion active parameters, and MAI-Code-1-Flash, a code-specialist model with 137 billion total parameters and 5 billion active parameters, optimized for GitHub Copilot. These models demonstrate competitive performance with significantly lower active parameter counts, potentially reducing inference costs. They also highlight Microsoft's investment in proprietary, commercially licensed training data, though they still rely on web crawls. MAI-Thinking-1 uses a Mixture of Experts (MoE) architecture where only 35 billion of its 1 trillion parameters are activated per token. MAI-Code-1-Flash claims 137B total with 5B active. Both models are trained on a combination of proprietary web crawl and Common Crawl data, not solely on licensed data.

rss · Simon Willison · Jun 2, 22:21

**Background**: In large language models, total parameters refer to the full size of the model, while active parameters are those used in a forward pass, especially in Mixture of Experts (MoE) architectures. MoE models have multiple 'expert' sub-networks and only activate a subset per token, enabling high capacity with lower computational cost. This distinction is crucial for understanding the performance and efficiency claims of new models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.f22labs.com/blogs/active-vs-total-parameters-whats-the-difference/">Active vs Total Parameters : What’s the Difference?</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#Microsoft`, `#coding`

---

<a id="item-4"></a>
## [Trump Signs AI Executive Order, Voluntary Model Review](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/) ⭐️ 8.0/10

On June 2, 2026, President Trump signed an executive order establishing a voluntary framework for AI developers to submit 'protected cutting-edge models' to the government for cybersecurity review at least 30 days before public release. It also directs the creation of an AI cybersecurity clearinghouse to coordinate vulnerability scanning and remediation. This executive order represents a direct U.S. government action to address AI risks, balancing national security with industry innovation. It could set a precedent for future AI regulation and affect how major AI companies release their most advanced models. The review period was shortened from an initially proposed 90 days to 30 days due to industry pressure and internal White House disagreements. The order explicitly prohibits mandatory government licensing or pre-check mechanisms, emphasizing a voluntary public-private partnership.

telegram · zaihuapd · Jun 2, 16:44

**Background**: An executive order is a directive issued by the U.S. President that manages operations of the federal government. 'Protected cutting-edge models' refer to advanced AI systems that could pose cybersecurity risks if released without safeguards. The voluntary framework means companies can choose to submit their models for review, but are not legally required to do so. The AI cybersecurity clearinghouse will coordinate efforts to find and fix software vulnerabilities across federal systems.

<details><summary>References</summary>
<ul>
<li><a href="https://federalnewsnetwork.com/cybersecurity/2026/06/ai-executive-order-sets-stage-for-new-cybersecurity-directives/">AI executive order sets stage for new cybersecurity directives</a></li>
<li><a href="https://www.aba.com/about-us/press-room/press-releases/aba-statement-on-executive-order-promoting-advanced-ai-innovation-and-security">ABA Statement on Executive Order Promoting Advanced AI Innovation ...</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#US government`, `#cybersecurity`, `#executive order`

---

<a id="item-5"></a>
## [Google to pay Play Store developers for private code to train AI](https://www.neowin.net/reports/google-wants-to-pay-play-store-developers-for-code-to-train-its-ai/) ⭐️ 8.0/10

Google is privately contacting Android developers, offering payment for access to their private code repositories to train its Gemini AI and improve development tools, while developers retain full IP rights. This move could give Google a significant advantage in narrowing the gap between Gemini and rival coding assistants like GitHub Copilot and Claude Code, potentially reshaping the AI-assisted development landscape. The offer involves a non-exclusive license to use developers' code for AI training, with Google retaining no ownership rights. The program is currently being rolled out via private outreach to Play Store developers.

telegram · zaihuapd · Jun 3, 02:47

**Background**: Large language models like Google's Gemini require vast amounts of high-quality code to improve their ability to assist developers. Competitors such as GitHub Copilot (powered by OpenAI) and Anthropic's Claude Code have already established strong positions by training on extensive codebases, often from public repositories. Google's strategy to pay for private code access could provide it with unique, high-value training data that is not publicly available, potentially accelerating its AI development.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://antigravity.google/product/antigravity-2">Google Antigravity - Antigravity 2 . 0</a></li>

</ul>
</details>

**Tags**: `#Google`, `#AI`, `#Android`, `#Developer Tools`, `#Training Data`

---