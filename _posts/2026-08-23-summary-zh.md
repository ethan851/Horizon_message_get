---
layout: default
title: "Horizon Summary: 2026-08-23 (ZH)"
date: 2026-08-23
lang: zh
---

> From 26 items, 3 important content pieces were selected

---

1. [MCP 路线图：远程服务器转向 HTTP，新增代理授权](#item-1) ⭐️ 8.0/10
2. [亚马逊被曝购书扫描训练 AI，书籍扫描后被销毁](#item-2) ⭐️ 8.0/10
3. [乌兰察布成中国 AI 算力枢纽，承诺容量 12.5 吉瓦](#item-3) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [MCP 路线图：远程服务器转向 HTTP，新增代理授权](https://blog.modelcontextprotocol.io/posts/mcp-roadmap/) ⭐️ 8.0/10

Model Context Protocol（MCP）团队发布了官方路线图，将远程服务器简化为标准 HTTP 工作负载，并引入针对 AI 代理的标准授权机制，支持代理代表用户操作。 MCP 已被 OpenAI、Google DeepMind 等主要 AI 提供商采用，这些变化可能重塑 AI 代理连接工具和服务的方式。对于用户不在场的云端工作负载，标准化的代理授权至关重要。 该路线图将远程 MCP 服务器从专有协议转向 HTTP 原生语义，并增加了服务器识别和信任代理身份的标准方式。社区讨论聚焦于协议复杂度与 REST（表述性状态传递）的比较、实现可行性及上下文膨胀等问题。

hackernews · pentagrama · Aug 22, 13:31 · [社区讨论](https://news.ycombinator.com/item?id=49399591)

**背景**: Model Context Protocol（MCP）是 Anthropic 于 2024 年 11 月推出的开放标准，旨在统一 AI 系统（如大语言模型）与外部工具和数据的集成方式。它就像 AI 的 USB-C 接口，为读取文件、执行函数和处理提示提供了标准化接口。新路线图反映了 MCP 在应用日益增长、调用者逐渐从交互式浏览器会话转向云上代理的背景下的演进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol</a></li>
<li><a href="https://modelcontextprotocol.io/docs/2026-07-28/getting-started/intro">What is the Model Context Protocol (MCP)?</a></li>
<li><a href="https://github.com/modelcontextprotocol">Model Context Protocol - GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一但参与度高。一些开发者欢迎将远程服务器简化为标准 HTTP 工作负载，而另一些人则怀疑多少 MCP 服务器会完整实现新的授权功能。还有观点为 MCP 仅暴露相关工具以节省上下文的能力辩护，质疑其相对于 REST 端点加技能文件的优势，并对标准变动和上下文占用表示不满。

**标签**: `#MCP`, `#AI agents`, `#protocol`, `#HTTP`, `#authorization`

---

<a id="item-2"></a>
## [亚马逊被曝购书扫描训练 AI，书籍扫描后被销毁](https://t.me/zaihuapd/43331) ⭐️ 8.0/10

调查媒体 404 Media 报道，亚马逊正大规模购买纸质书、扫描用于 AI 训练，并随后销毁书籍。调查人员将追踪装置放入一本稀有书，最终追踪到其位于内华达州拉斯维加斯的亚马逊仓库；该仓库员工称，他们收到大量印刷书籍后会剪开装订以加快扫描，书页随即被销毁。 此事意义重大，因为它揭露了全球最大公司之一颇具争议的数据获取方式，引发关于版权、合理使用以及物理销毁书籍的道德与法律问题。继 Anthropic 被曝有类似购书扫描行为后，这一调查进一步加剧了外界对 AI 开发商如何获取训练数据的关注。 调查通过在稀有书中放置物理追踪装置，最终追踪到拉斯维加斯的仓库。据员工称，亚马逊剪掉装订以加快扫描速度，书页随后即被销毁。

telegram · zaihuapd · Aug 22, 15:40

**背景**: AI 训练通常需要海量文本数据，而出版的书籍被视为高质量来源，但大规模数字化会引发版权问题。扫描纸质书然后丢弃是一种极端的批量数字化做法，此前 Anthropic 也被指采用类似方式。404 Media 是报道此事的独立调查媒体。

**标签**: `#AI`, `#copyright`, `#data collection`, `#Amazon`, `#ethics`

---

<a id="item-3"></a>
## [乌兰察布成中国 AI 算力枢纽，承诺容量 12.5 吉瓦](https://www.wired.com/story/the-unlikely-place-at-the-center-of-chinas-ai-boom/) ⭐️ 8.0/10

高盛报告显示，内蒙古乌兰察布自 2016 年以来已开业或开工近 100 个数据中心，中企承诺总容量达 12.5 吉瓦，超过 OpenAI 规划的 10 吉瓦星际之门项目。其中超七成容量是过去一年宣布的，DeepSeek、字节跳动、阿里巴巴和小红书均在此自建 AI 数据中心。 这使得乌兰察布成为全球规模最大的 AI 算力集中建设地之一，表明中国 AI 基础设施扩张的规模已达到或超过美国大型项目。同时也加剧了对水和能源约束的担忧，因为该地区依赖煤电并面临缺水问题。 当地高寒气候、低电价和邻近北京是主要吸引力，但年降水量仅约 14 英寸，上个月当地水厂被迫每晚停水 7 小时。目前约 37%的电力仍来自煤电。

telegram · zaihuapd · Aug 23, 00:55

**背景**: 乌兰察布是内蒙古的一座城市，因气候凉爽、电价低廉而成为数据中心选址的热门地区。星际之门是美国 OpenAI、软银、甲骨文和 MGX 合资的项目，计划到 2029 年投入高达 5000 亿美元建设 AI 基础设施。DeepSeek 是一家以高效开源权重模型著称的中国 AI 公司，字节跳动、阿里巴巴和小红书则是中国主要的互联网和 AI 企业。这些背景有助于理解乌兰察布 12.5 吉瓦承诺为何是一个重要里程碑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stargate_LLC">Stargate LLC - Wikipedia</a></li>
<li><a href="https://openai.com/index/announcing-the-stargate-project/">Announcing The Stargate Project | OpenAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#data centers`, `#China`, `#cloud computing`, `#energy`

---