---
layout: default
title: "Horizon Summary: 2026-08-23 (EN)"
date: 2026-08-23
lang: en
---

> From 26 items, 3 important content pieces were selected

---

1. [MCP Roadmap Moves Remote Servers to HTTP, Adds Agent Authorization](#item-1) ⭐️ 8.0/10
2. [Amazon Reportedly Buys and Destroys Books to Scan for AI Training](#item-2) ⭐️ 8.0/10
3. [Ulanqab Emerges as China's AI Datacenter Hub with 12.5 GW Commitments](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [MCP Roadmap Moves Remote Servers to HTTP, Adds Agent Authorization](https://blog.modelcontextprotocol.io/posts/mcp-roadmap/) ⭐️ 8.0/10

The Model Context Protocol (MCP) team published an official roadmap that simplifies remote servers to standard HTTP workloads and introduces standardized agent authorization for AI agents acting on behalf of users. MCP has been adopted by major AI providers such as OpenAI and Google DeepMind, so these changes could reshape how AI agents connect to tools and services. Standardized agent authorization is essential for cloud-based workloads where users are not directly present. The roadmap moves remote MCP servers away from a bespoke protocol toward HTTP-native semantics, and adds a standardized way for servers to recognize and trust agent identities. Community debate highlights questions about protocol complexity versus REST, adoption feasibility, and the potential for context bloat.

hackernews · pentagrama · Aug 22, 13:31 · [Discussion](https://news.ycombinator.com/item?id=49399591)

**Background**: The Model Context Protocol (MCP) is an open standard introduced by Anthropic in November 2024 to unify how AI systems like large language models integrate with external tools and data. It acts like a USB-C port for AI, providing a standardized interface for reading files, executing functions, and handling prompts. The new roadmap reflects MCP's evolution as adoption grows and more callers become cloud-based agents rather than interactive browser sessions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol</a></li>
<li><a href="https://modelcontextprotocol.io/docs/2026-07-28/getting-started/intro">What is the Model Context Protocol (MCP)?</a></li>
<li><a href="https://github.com/modelcontextprotocol">Model Context Protocol - GitHub</a></li>

</ul>
</details>

**Discussion**: The community response is mixed but engaged. Some developers welcome the simplification of remote servers to standard HTTP workloads, while others doubt whether many MCP servers will fully implement the new authorization features. Additional viewpoints defend MCP's ability to expose only relevant tools to save context, question its advantage over REST endpoints with a skills file, and express frustration over standard shifts and context-hungry behavior.

**Tags**: `#MCP`, `#AI agents`, `#protocol`, `#HTTP`, `#authorization`

---

<a id="item-2"></a>
## [Amazon Reportedly Buys and Destroys Books to Scan for AI Training](https://t.me/zaihuapd/43331) ⭐️ 8.0/10

Investigative outlet 404 Media reports that Amazon is purchasing physical books at scale, scanning them for AI training, and then destroying the volumes. A tracking device placed in a rare book led to an Amazon warehouse in Las Vegas, Nevada, where employees said books are received, cut from bindings for faster scanning, and then discarded. This is significant because it exposes a controversial data-sourcing practice by one of the world's largest companies, raising ethical and legal questions about copyright, fair use, and the physical destruction of books. It adds to growing scrutiny over how AI developers obtain training data, particularly after similar book-scanning practices were reported at Anthropic. The investigation is based on a physical tracking device planted in a rare book that was traced to the Las Vegas facility. Employees reportedly cut off bindings to speed up scanning, after which the scanned pages are destroyed.

telegram · zaihuapd · Aug 22, 15:40

**Background**: AI training typically requires vast amounts of text data, and publishers' books are considered high-quality sources, but digitizing them at scale raises copyright issues. Scanning physical books and discarding them is an extreme variant of mass digitization, and it has previously been linked to Anthropic. 404 Media is an independent journalism outlet that reported this story.

**Tags**: `#AI`, `#copyright`, `#data collection`, `#Amazon`, `#ethics`

---

<a id="item-3"></a>
## [Ulanqab Emerges as China's AI Datacenter Hub with 12.5 GW Commitments](https://www.wired.com/story/the-unlikely-place-at-the-center-of-chinas-ai-boom/) ⭐️ 8.0/10

A Goldman Sachs report says nearly 100 data centers in Ulanqab, Inner Mongolia, are open or under construction since 2016, with Chinese companies committing 12.5 GW of total capacity—more than OpenAI's planned 10 GW Stargate. Over 70% of that capacity was announced in the past year, with DeepSeek, ByteDance, Alibaba, and Xiaohongshu building AI data centers there. This makes Ulanqab one of the largest concentrated AI compute buildouts in the world, signaling that China's AI infrastructure expansion is proceeding at a scale comparable to or larger than major US projects. It also sharpens concerns about water and energy constraints, since the region relies on coal power and faces water shortages. The region's cold climate, cheap electricity, and proximity to Beijing are key attractions, but annual precipitation is only about 14 inches and last month a local water plant had to stop supply for seven hours each night. About 37% of local electricity still comes from coal power.

telegram · zaihuapd · Aug 23, 00:55

**Background**: Ulanqab is a city in Inner Mongolia that has become a favored site for data centers because of its cool climate and low energy costs. The Stargate Project is a US joint venture by OpenAI, SoftBank, Oracle, and MGX that plans to invest up to $500 billion in AI infrastructure by 2029. DeepSeek is a Chinese AI company known for efficient, open-weight models, and ByteDance, Alibaba, and Xiaohongshu are major Chinese internet and AI players. These context points help explain why the 12.5 GW commitment in Ulanqab is a significant milestone.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stargate_LLC">Stargate LLC - Wikipedia</a></li>
<li><a href="https://openai.com/index/announcing-the-stargate-project/">Announcing The Stargate Project | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#data centers`, `#China`, `#cloud computing`, `#energy`

---