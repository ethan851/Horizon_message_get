---
layout: default
title: "Horizon Summary: 2026-05-27 (EN)"
date: 2026-05-27
lang: en
---

> From 22 items, 6 important content pieces were selected

---

1. [Alipay Launches Token Pay and AI Wallet for Agent Economy](#item-1) ⭐️ 9.0/10
2. [Big tech's anti-labor playbook has come for Wikipedia](#item-2) ⭐️ 8.0/10
3. [Curl Maintainer Overwhelmed by AI-Assisted Security Reports](#item-3) ⭐️ 8.0/10
4. [Microsoft Copilot Cowork Vulnerability Enables File Exfiltration](#item-4) ⭐️ 8.0/10
5. [Iran Plans Permanent Internet Disconnection for Most Users](#item-5) ⭐️ 8.0/10
6. [Qualcomm to Supply Custom AI ASICs to ByteDance](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Alipay Launches Token Pay and AI Wallet for Agent Economy](https://finance.sina.com.cn/jjxw/2026-05-26/doc-inhzffss1524895.shtml) ⭐️ 9.0/10

On May 26, 2026, Alipay launched two new services: AI Wallet and Token Pay. Users can access the AI Wallet by searching in the Alipay app, and Token Pay enables global subscription and in-app token top-ups for AI companies like MiniMax and Jieyue Xingchen. This marks a significant step in bridging AI services with payment infrastructure, enabling the agentic economy where AI agents can autonomously make payments. It impacts AI developers, businesses, and consumers by providing a dedicated, trusted payment method for AI-driven transactions. The AI Wallet allows consumers to manage and review payments made by AI agents, while Token Pay is designed for large language model companies to accept global subscriptions and in-app token purchases. The services are available immediately in the Alipay app.

telegram · zaihuapd · May 26, 12:31

**Background**: The agentic economy involves AI agents that can autonomously perform tasks, including financial transactions. Traditional payment systems are not built for dynamic, agent-initiated payments, raising issues of trust, fraud, and authorization. Alipay's new services address these challenges by offering a full-stack AI payment solution tailored for the agentic era.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techrepublic.com/article/news-apac-alipay-ai-wallet-token-pay-ai-agents/">Alipay Launches AI Payment Tools for Shopping Agents</a></li>
<li><a href="https://www.morningstar.com/news/business-wire/20260526337824/alipay-launches-next-generation-ai-payment-infrastructure-debuts-ai-wallet-and-token-pay-to-power-agentic-economy">Alipay Launches Next-Generation AI Payment Infrastructure ...</a></li>

</ul>
</details>

**Tags**: `#Alipay`, `#token payments`, `#AI wallet`, `#AI monetization`, `#fintech`

---

<a id="item-2"></a>
## [Big tech's anti-labor playbook has come for Wikipedia](https://medium.com/@jakeorlowitz/wikipedia-is-doing-the-capitalist-thing-56a393232943) ⭐️ 8.0/10

The Wikimedia Foundation laid off a senior MediaWiki developer and the entire community tech team, prompting an editor strike on English Wikipedia. This move signals a troubling shift in the nonprofit's treatment of volunteer contributors, potentially eroding the collaborative foundation of Wikipedia. The laid-off developer, Brooke, was one of the original creators of MediaWiki and a longtime leader in the project. The community tech team maintained the Community Wishlist, which allowed editors to request tooling improvements.

hackernews · cdrnsf · May 26, 20:33 · [Discussion](https://news.ycombinator.com/item?id=48285592)

**Background**: MediaWiki is the free, open-source software that powers Wikipedia and many other wikis. It was originally developed by Magnus Manske and later enhanced by Lee Daniel Crocker, with ongoing development coordinated by the Wikimedia Foundation. The community tech team's work was critical for non-technical editors who rely on custom tools to remain productive.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MediaWiki">MediaWiki</a></li>

</ul>
</details>

**Discussion**: Community comments express shock at the firing of Brooke, a respected long-time developer, and frustration over the loss of the community tech team. Editors are striking to protest the layoffs, which many see as a sign of growing corporate-like behavior at the foundation, despite its nonprofit status. Some commenters also debate the financial health of the foundation, noting that 17 months of runway may not be as secure as it sounds.

**Tags**: `#Wikipedia`, `#Open Source`, `#Layoffs`, `#Wikimedia Foundation`, `#Community Strike`

---

<a id="item-3"></a>
## [Curl Maintainer Overwhelmed by AI-Assisted Security Reports](https://simonwillison.net/2026/May/26/the-pressure/#atom-everything) ⭐️ 8.0/10

Daniel Stenberg, the lead maintainer of the curl project, reports that the rate of AI-assisted security reports has surged to more than one per day, a 4-5x increase from 2024 and double the rate of 2025, causing unprecedented maintainer burnout and pressure. This situation highlights a growing crisis for open source projects, as AI tools enable mass production of high-quality vulnerability reports, overwhelming small maintenance teams and threatening project sustainability. Despite the flood, the vulnerabilities found are predominantly LOW or MEDIUM severity, with the last HIGH severity CVE in October 2023, indicating that curl remains solid software but the volume of reports itself is a major problem.

rss · Simon Willison · May 26, 23:48

**Background**: curl is a widely used open-source command-line tool and library for transferring data with URLs. Its security is critical because it is embedded in countless systems. AI-assisted security research uses large language models (LLMs) to analyze code and generate detailed vulnerability reports, which can dramatically increase the number and quality of reports, straining limited maintainer resources.

**Tags**: `#open source`, `#security`, `#AI`, `#curl`, `#maintainer burnout`

---

<a id="item-4"></a>
## [Microsoft Copilot Cowork Vulnerability Enables File Exfiltration](https://simonwillison.net/2026/May/26/copilot-cowork-exfiltrates-files/#atom-everything) ⭐️ 8.0/10

Researchers from PromptArmor disclosed that Microsoft Copilot Cowork can be exploited via indirect prompt injection to exfiltrate files by sending emails with external images that trigger network requests, leaking pre-authenticated OneDrive download links. This vulnerability highlights a fundamental security challenge in agentic systems: preventing data exfiltration through prompt injection. It affects enterprise users of Microsoft 365 Copilot, potentially allowing attackers to access sensitive files without proper approval. The attack, tracked as CVE-2025-32711 with a CVSS score of 9.3, exploits the agent's ability to send emails to the user's inbox without approval, and uses external images to exfiltrate data when the message is viewed. PromptArmor demonstrated that just five lines of prompt injection within a Copilot Cowork Skills file can compromise the entire Microsoft 365 environment.

rss · Simon Willison · May 26, 15:36

**Background**: Prompt injection is a security vulnerability where user-crafted inputs manipulate an LLM's behavior to override intended instructions. Agentic systems, like Copilot Cowork, are AI agents that can autonomously interact with tools and data, making them susceptible to such attacks if they trust untrusted inputs. Data exfiltration via external images is a classic technique: an email containing an image URL that includes sensitive data in the query string can send that data to an attacker's server when the image is loaded.

<details><summary>References</summary>
<ul>
<li><a href="https://www.evidentlyai.com/llm-guide/prompt-injection-llm">What is prompt injection ? Example attacks, defenses and testing.</a></li>
<li><a href="https://aitoolly.com/ai-news/article/2026-05-26-microsoft-copilot-cowork-vulnerability-indirect-prompt-injection-enables-unauthorized-file-exfiltrat">Microsoft Copilot Cowork File Exfiltration Vulnerability ...</a></li>
<li><a href="https://letsdatascience.com/news/microsoft-copilot-cowork-enables-file-exfiltration-via-echol-ca9b728b">Microsoft Copilot Cowork Enables File Exfiltration via ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#prompt injection`, `#agentic systems`, `#data exfiltration`, `#Microsoft Copilot`

---

<a id="item-5"></a>
## [Iran Plans Permanent Internet Disconnection for Most Users](https://t.me/zaihuapd/41574) ⭐️ 8.0/10

Iranian digital rights activists report that the government is developing a covert plan to permanently disconnect most citizens from the global internet, allowing only government-approved individuals to access a censored international network through a privilege system. This plan would create a domestic 'splinternet' with severe implications for digital rights, freedom of expression, and cybersecurity, setting a precedent for other nations to implement similar internet isolation measures. According to a report by internet monitoring organization Filterwatch, the plan is labeled 'Absolute Digital Isolation' and aims to transform international internet access into a government privilege, with the current blackout since January 8 serving as a test run.

telegram · zaihuapd · May 26, 06:36

**Background**: Iran has long pursued a 'National Information Network' (also known as 'Halal Internet'), a domestic intranet with government-approved content. This new plan would permanently replace the global internet for most users, restricting them to this heavily censored domestic network while only a select few can access a filtered version of the worldwide web. Similar concepts have been discussed in other countries as a means of state control over information.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2026_Internet_blackout_in_Iran">2026 Internet blackout in Iran - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/National_intranet">National intranet - Wikipedia</a></li>
<li><a href="https://filter.watch/english/about-us/">About - Filterwatch - فیلتربان</a></li>

</ul>
</details>

**Tags**: `#internet censorship`, `#Iran`, `#digital rights`, `#cybersecurity`, `#net neutrality`

---

<a id="item-6"></a>
## [Qualcomm to Supply Custom AI ASICs to ByteDance](https://www.bloomberg.com/news/videos/2026-05-26/qualcomm-to-supply-chips-to-tiktok-owner-bytedance-video) ⭐️ 8.0/10

Qualcomm has reached an agreement with ByteDance to supply millions of custom AI ASICs, which ByteDance will use to power its AI services and also help convert its in-house chip designs into mass-produced semiconductors. This deal signals a major shift towards specialized AI hardware at scale, potentially reducing reliance on general-purpose GPUs and highlighting the growing importance of custom silicon for large AI workloads. It could also intensify competition among custom AI chip designers like Broadcom and Marvell. The agreement covers millions of chips, and Qualcomm had previously announced in late April that it would deliver its first ASIC to a hyperscaler this year. ByteDance will use these chips not only for AI inference but also to commercialize its own chip designs.

telegram · zaihuapd · May 27, 02:29

**Background**: An application-specific integrated circuit (ASIC) is a chip customized for a particular use, offering higher efficiency than general-purpose chips for specific tasks like AI inference. Custom AI ASICs are increasingly used by large tech companies to optimize performance and energy consumption for their workloads. Companies like Broadcom and Marvell already supply custom AI chips to hyperscalers such as Google and Amazon, and this partnership marks Qualcomm's entry into that market.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Application-specific_integrated_circuit">Application-specific integrated circuit - Wikipedia</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/custom-ai-asics-examined-from-broadcom-to-mtia">The custom AI ASIC state of play (May 2026) — Broadcom deals, Google TPUs, Meta MTIA & beyond | Tom's Hardware</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#ASIC`, `#Qualcomm`, `#ByteDance`, `#semiconductor`

---