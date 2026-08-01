---
layout: default
title: "Horizon Summary: 2026-08-01 (EN)"
date: 2026-08-01
lang: en
---

> From 31 items, 6 important content pieces were selected

---

1. [Elevator Scheduling Algorithms: SCAN, LOOK, and Destination Dispatch](#item-1) ⭐️ 8.0/10
2. [YC releases qm: a multiplayer agent harness for work](#item-2) ⭐️ 8.0/10
3. [Tailscale Didn't Stop the Hugging Face Intrusion](#item-3) ⭐️ 8.0/10
4. [DeepSeek V4 Flash 0731: 304B Agentic Model, Best Value per Dollar](#item-4) ⭐️ 8.0/10
5. [Stateless MCP 2.0 Reignites Interest with New Tools](#item-5) ⭐️ 8.0/10
6. [OpenAI Bans Cambodian Scam Network's ChatGPT Accounts](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Elevator Scheduling Algorithms: SCAN, LOOK, and Destination Dispatch](https://john.fun/elevators) ⭐️ 8.0/10

The article at john.fun/elevators provides a technical analysis of elevator scheduling algorithms and their efficiency. The accompanying Hacker News discussion (901 points, 223 comments) expands the topic by drawing parallels to disk scheduling and destination dispatch systems. Elevator scheduling affects everything from office towers to disk drives, and the trade-offs between simple algorithms and modern destination dispatch have practical implications. The discussion is valuable for systems engineers and algorithm enthusiasts who want to understand how these algorithms perform in real-world conditions. The article likely compares algorithms such as FCFS, SSTF, SCAN, and LOOK, as reflected in the community discussion. Commenters note that SCAN is also a disk-scheduling algorithm, and that destination dispatch may underperform with random destinations but excel with realistic traffic patterns like lunchtime rushes.

hackernews · Jrh0203 · Jul 31, 15:17 · [Discussion](https://news.ycombinator.com/item?id=49124218)

**Background**: The elevator algorithm, also known as SCAN, moves a disk arm or elevator in one direction, servicing requests along the way, then reverses direction. LOOK is a variant that only travels as far as the last pending request. Destination dispatch requires passengers to enter their destination floor, allowing the system to group passengers going to the same floor and reduce travel times.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Destination_dispatch">Destination dispatch - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Elevator_algorithm">Elevator algorithm - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/operating-systems/disk-scheduling-algorithms/">Disk Scheduling Algorithms - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: Commenters connect elevator scheduling to disk scheduling: peterldowns notes that a HDD acts like a long elevator and that SCAN is a disk-scheduling algorithm. omoikane questions the article's comparison by pointing out that destination dispatch excels in real-world patterns, and hermanschaaf says he chose LOOK for his elevator game because it matches user expectations. Others share links to the Elevator Saga game and complain about users pressing both up and down buttons.

**Tags**: `#algorithms`, `#elevators`, `#scheduling`, `#simulation`, `#systems`

---

<a id="item-2"></a>
## [YC releases qm: a multiplayer agent harness for work](https://github.com/yc-software/qm) ⭐️ 8.0/10

Y Combinator has released qm, an open-source multiplayer agent harness for work, hosted at github.com/yc-software/qm. It introduces shared rooms and per-person scopes so teams can run AI agents collaboratively while each person keeps a personalized agent. qm points to a shift from single-user AI assistants to team-level, collaborative AI agents, addressing a hard problem: scoping and permissions in multi-agent workflows. If successful, it could influence how companies build internal AI tools, and the 472-point Hacker News discussion shows strong early interest from developers. The repository describes 'personal and shared scopes': people customize the agent to be theirs, yet still work with it collaboratively in Slack channels and projects. The harness is designed to avoid the complexity of scaling a personal assistant to a whole company by giving each user their own scope while enabling shared rooms.

hackernews · tosh · Jul 31, 18:04 · [Discussion](https://news.ycombinator.com/item?id=49126604)

**Background**: An agent harness is everything around the AI model that makes an agent useful — context handling, tools, memory, and user interfaces; Martin Fowler describes it as 'Agent = Model + Harness'. Collaborative AI is a design pattern where multiple team members work with AI in shared spaces while maintaining coordination, rather than each person using AI in isolation. qm applies this pattern specifically to work environments, letting teams share agents in Slack and projects while preserving individual customization.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/yc-software/qm">GitHub - yc-software/qm: Multiplayer agent harness for work · GitHub</a></li>
<li><a href="https://martinfowler.com/articles/harness-engineering.html">Harness engineering for coding agent users</a></li>
<li><a href="https://www.aiuxdesign.guide/patterns/collaborative-ai">Collaborative AI — What It Is & How to Design Human-AI Collaboration | AI Design Patterns</a></li>

</ul>
</details>

**Discussion**: Comments mix skepticism and validation: one asks for a 'qm vs Claude Cowork' comparison and questions the advantage over existing tools, while another shares a humorous anecdote about an agent scheduling meetings with other agents. A builder in an adjacent space (AQ) says qm's per-person scopes plus shared rooms are 'a sane answer' for company-wide assistants, and others express interest in how qm handles org-wide context and security.

**Tags**: `#AI agents`, `#multiplayer`, `#Y Combinator`, `#collaboration`, `#developer tools`

---

<a id="item-3"></a>
## [Tailscale Didn't Stop the Hugging Face Intrusion](https://tailscale.com/blog/hugging-face-intrusion) ⭐️ 8.0/10

Tailscale published a blog post analyzing the Hugging Face intrusion, revealing that no Tailscale vulnerability was exploited. Instead, a reusable auth key stored in an environment file allowed attackers to enroll 181 unauthorized nodes into Hugging Face's tailnet over several days. This matters because it underscores that even a secure mesh VPN can be undermined by poor credential hygiene; a single leaked reusable auth key gave attackers a foothold in the target's private network. It also highlights an alerting gap in Tailscale that security practitioners should address. The leaked key was a reusable Tailscale auth key used to create CI nodes, and attackers enrolled 181 nodes into Hugging Face's tailnet with CI identity tags. Tailscale's node keys expire by default after 180 days, but reusable auth keys with no origin/destination binding make such attacks possible.

hackernews · bluehatbrit · Jul 31, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49127306)

**Background**: Tailscale is a mesh VPN built on WireGuard that creates secure, peer-to-peer connections between devices across the internet. In Tailscale, a 'tailnet' is the private network of a user's devices, and 'nodes' are machines that run Tailscale. 'Auth keys' are pre-authenticated secrets used to add nodes to a tailnet without interactive SSO, often for CI/CD automation.

<details><summary>References</summary>
<ul>
<li><a href="https://tailscale.com/docs/features/access-control/auth-keys">Auth keys · Tailscale Docs</a></li>
<li><a href="https://tailscale.com/learn/understanding-mesh-vpns">Understanding mesh network topology (mesh VPNs)</a></li>

</ul>
</details>

**Discussion**: Comments were largely positive about Tailscale's transparency, with users like john_strinlai praising the company for not staying quiet. However, some like ahofmann viewed the post as 'smart marketing' while noting that Hugging Face made a poor choice by putting a reusable auth key in an env file. simonw pointed out that the intrusion points to an alerting opportunity, and angry_octet argued that long-lived credentials should be bound to specific origins/destinations.

**Tags**: `#security`, `#tailscale`, `#credential-management`, `#incident-response`, `#mesh-vpn`

---

<a id="item-4"></a>
## [DeepSeek V4 Flash 0731: 304B Agentic Model, Best Value per Dollar](https://simonwillison.net/2026/Jul/31/deepseek-v4-flash-0731/#atom-everything) ⭐️ 8.0/10

DeepSeek released DeepSeek-V4-Flash-0731, a 304B-parameter model with substantially enhanced agentic capabilities, priced at $0.14 per million input tokens and $0.27 per million output tokens. Artificial Analysis ranks it ahead of MiniMax M3, a 428B parameter model. This release reinforces DeepSeek's leadership in the cost-performance frontier of AI, offering near-top intelligence at a fraction of the price of competitors. It could accelerate adoption of agentic AI in real-world applications that are sensitive to API costs. The model is 167GB on Hugging Face with 304B parameters. Simon Willison's test via OpenRouter showed that default reasoning effort produced a mediocre image, while setting `reasoning_effort high` yielded a much better result, highlighting the importance of reasoning-level configuration.

rss · Simon Willison · Jul 31, 23:59

**Background**: Agentic AI refers to artificial intelligence systems that can accomplish specific goals with limited supervision, often by mimicking human decision-making. The Artificial Analysis Intelligence Index aggregates multiple benchmarks into a single model-level intelligence score, enabling comparisons of intelligence and cost per task across models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>
<li><a href="https://artificialanalysis.ai/">AI Model & API Providers Analysis | Artificial Analysis</a></li>
<li><a href="https://benchlm.ai/benchmarks/artificialanalysis">Artificial Analysis Intelligence Index Leaderboard... | BenchLM.ai</a></li>

</ul>
</details>

**Tags**: `#DeepSeek`, `#LLM`, `#AI`, `#model release`, `#agentic`

---

<a id="item-5"></a>
## [Stateless MCP 2.0 Reignites Interest with New Tools](https://simonwillison.net/2026/Jul/31/stateless-mcp/#atom-everything) ⭐️ 8.0/10

Simon Willison reports on the rollout of the Stateless MCP specification (the 2026-07-28 Model Context Protocol release), which enables tools to be called with a single HTTP request instead of requiring a session initialization step. He also introduced two new projects built on this protocol: mcp-explorer and datasette-mcp. This is the most significant MCP spec change since its launch, simplifying both client and server implementations and making stateless MCP a better fit for scalable web applications. It also restores MCP's appeal as a more auditable and controllable alternative to giving AI agents unrestricted shell access. The new stateless flow uses HTTP headers such as MCP-Protocol-Version, Mcp-Method, and Mcp-Name in a single request, eliminating the need for server-side session IDs. The 2026-07-28 specification also includes an extensions framework, Tasks, authentication hardening, and is stewarded by the Agentic AI Foundation under the Linux Foundation.

rss · Simon Willison · Jul 31, 23:13

**Background**: MCP is an open standard introduced by Anthropic in November 2024 to standardize how AI applications connect to external tools and data sources. The earlier stateful version required two HTTP requests — one to initialize a session and obtain an Mcp-Session-Id, and another to call the tool — which added complexity and scalability challenges. The new stateless core reduces this to one request, making the protocol simpler and more practical for modern agent-based applications.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.modelcontextprotocol.io/posts/2026-07-28-release-candidate/">The 2026-07-28 MCP Specification Release Candidate | Model Context Protocol Blog</a></li>
<li><a href="https://venturebeat.com/infrastructure/mcp-just-got-its-biggest-update-ever-heres-what-changes-for-ai-agents">MCP just got its biggest update ever — here’s what changes for AI agents | VentureBeat</a></li>
<li><a href="https://simonwillison.net/2026/Jul/31/stateless-mcp/">Stateless MCP has recaptured my interest (and inspired mcp - explorer ...</a></li>

</ul>
</details>

**Tags**: `#MCP`, `#AI`, `#protocol`, `#agents`, `#tools`

---

<a id="item-6"></a>
## [OpenAI Bans Cambodian Scam Network's ChatGPT Accounts](https://openai.com/index/disrupting-malicious-uses-of-ai-criminal-scam-operation/) ⭐️ 8.0/10

OpenAI announced the disruption of a ChatGPT account network likely based in Poipet, Cambodia, that was used for investment fraud, pig-butchering scams, gambling fraud, and impersonating law enforcement. The initial announcement was dated August 4, 2026, and OpenAI later corrected the date to July 31. This case is a prominent real-world example of AI chatbots being weaponized for large-scale financial fraud and human-trafficking-related activity. It shows how AI providers can detect and disrupt malicious usage while sharing threat intelligence with industry partners and law enforcement. The scammers used ChatGPT to generate fake personas, translate conversations with victims, and forge images of passports and legal documents, following a 'contact, build trust, extract money' playbook. OpenAI began the investigation after receiving a tip from WhatsApp; the network may have reached hundreds of targets, with individual victim losses in the thousands of dollars, and some generated content appeared tied to human trafficking and forced labor.

telegram · zaihuapd · Jul 31, 23:41

**Background**: Pig-butchering scams are long-term frauds in which criminals groom victims through romance or friendship before persuading them to invest in fake schemes. Southeast Asia, especially the Cambodia-Thailand border area, has become a hub for such criminal syndicates, which often also engage in human trafficking and forced labor. OpenAI's action highlights that AI-generated content is now part of these operations and that platform-level monitoring can produce actionable threat intelligence.

**Tags**: `#AI Safety`, `#Cybersecurity`, `#OpenAI`, `#Fraud`, `#Abuse Prevention`

---