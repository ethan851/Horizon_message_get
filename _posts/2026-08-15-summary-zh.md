---
layout: default
title: "Horizon Summary: 2026-08-15 (ZH)"
date: 2026-08-15
lang: zh
---

> From 28 items, 12 important content pieces were selected

---

1. [Qwen 发布 Qwen3.8-27B 开源权重模型，推理出色且可运行在笔记本上](#item-1) ⭐️ 9.0/10
2. [GLM-5.3：具备突现网络能力的尖端编程模型](#item-2) ⭐️ 9.0/10
3. [步入黑暗：执法黑客时代来临](#item-3) ⭐️ 8.0/10
4. [Opus 5 体验变差：后训练优化对象是智能体而非人类](#item-4) ⭐️ 8.0/10
5. [Firefox 成为唯一支持完整版 uBlock Origin 的主流浏览器](#item-5) ⭐️ 8.0/10
6. [讽刺网站“Every Fucking Website”嘲讽糟糕的网页设计](#item-6) ⭐️ 8.0/10
7. [不要分类，要“幻觉”：先生成标签再用嵌入匹配](#item-7) ⭐️ 8.0/10
8. [Vivodyne 的 AI 机器人实验室每年测试 300 万份人体组织，目标终结动物试验。](#item-8) ⭐️ 8.0/10
9. [小红书开源 dots3-note：280B MoE，16B 激活参数](#item-9) ⭐️ 8.0/10
10. [苹果官宣换帅：库克卸任 CEO，特努斯 2026 年接任](#item-10) ⭐️ 8.0/10
11. [PostgreSQL 高危 to_char 漏洞可致任意代码执行](#item-11) ⭐️ 8.0/10
12. [苹果联手阿里训练中国专属 AI 模型，或成首个获批外企](#item-12) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Qwen 发布 Qwen3.8-27B 开源权重模型，推理出色且可运行在笔记本上](https://huggingface.co/Qwen/Qwen3.8-27B-FP8) ⭐️ 9.0/10

Qwen 在 Hugging Face 上发布了 Qwen3.8-27B——一个稠密型 270 亿参数的开源权重视觉语言模型，并同时提供 FP8 量化版本。该模型基于 Qwen3.5 架构，支持原生 262K token 上下文窗口与可配置的推理模式。 这次发布意义重大，因为一个能在笔记本上运行且推理能力出色的 270 亿参数开源权重模型，降低了本地 AI 开发的门槛，也减少了对云端 API 的依赖。它也表明非美国实验室正在快速追赶前沿闭源模型，给整个 AI 生态带来更大的竞争压力。 Qwen3.8-27B 是面向编程、专业工作、研究和长周期智能体任务设计的稠密视觉语言模型，具有更强的自主规划与环境反馈处理能力。社区测试显示它能在 llama.cpp 中本地运行，但一名 RTX 5090 用户用 ninfer 引擎测得约 138 tokens/秒，几乎是朴素 llama.cpp 设置速度的两倍。

hackernews · erdaltoprak · Aug 14, 15:00 · [社区讨论](https://news.ycombinator.com/item?id=49299605)

**背景**: 开源权重模型会把训练好的神经网络权重公开发布，让开发者可以自行托管、微调和改造，但通常不会公开训练数据或完整训练代码。Qwen 是阿里巴巴的大语言模型与多模态模型系列，Qwen3.8-27B 是一个能同时处理文本和图像的视觉语言模型。它的“思考”模式可以开关，让用户在更快的响应与更逐步的推理之间取舍；262K token 的原生上下文窗口则使它可以在单次输入中处理很长的文档或多图像内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://lmstudio.ai/models/qwen3.8">Qwen3.8 - lmstudio.ai</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的反响非常正面：有评论者称它是“我在笔记本电脑上见过的模型画出的最好的鹈鹕”，另一位则表示它是继 Gemma 4 之后第二个正确通过其私有推理基准的本地模型。也有人指出，它的思考轨迹使用简略、便签式的语言，可能降低 MTP 预测质量，并且 VRAM 占用效率似乎不如 Gemma 4 或 Glimmer。一位开发者报告称，在 RTX 5090 上使用 ninfer 引擎可获得约 138 tokens/秒，约为朴素 llama.cpp 设置速度的两倍。

**标签**: `#LLM`, `#Open Source`, `#Qwen`, `#Local AI`, `#Model Release`

---

<a id="item-2"></a>
## [GLM-5.3：具备突现网络能力的尖端编程模型](https://z.ai/blog/glm-5.3) ⭐️ 9.0/10

Z.ai 发布了 GLM-5.3，这是一款基于 GLM-5.2 基座模型进行后训练的新旗舰模型，在复杂软件工程、智能体任务和安全研究方面取得重大进展。该版本突显了突现的网络安全能力，包括自主漏洞发现与利用代码适配，并提供三档思考强度和 1M 上下文窗口。 此次发布标志着前沿 AI 进入新阶段：编程模型日益能够自主执行安全研究工作，用户甚至报告了真实的 0-day 发现与利用场景。这加剧了关于开源权重模型在收益与滥用风险之间权衡的争论，同时也改变了与 OpenAI 和 Anthropic 的竞争格局。 GLM-5.3 与 GLM-5.2 使用相同的基座模型，所有改进均来自后训练，并提供三档思考强度以及 1M token 上下文窗口。Z.ai 还上线了漏洞协同披露页面（cvd.z.ai），似乎反映了对开源软件的大规模扫描，其中许多 CVE 仍处于保密期。

hackernews · pella · Aug 14, 05:19 · [社区讨论](https://news.ycombinator.com/item?id=49294997)

**背景**: GLM-5.3 是 Z.ai 在 GLM 系列中的旗舰模型，该系列是由智谱 AI 开发的大语言模型家族。LLM 的突现能力是指随着模型规模扩大而突然、不可预测地出现的能力，而此次发布是商业编程模型中首次明确将这种能力与网络安全联系起来。前沿编程模型是使用大上下文推理来理解源文件、依赖关系和复杂编码任务的高级 AI 系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.3">GLM - 5 . 3 - Overview - Z. AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.together.ai/models/glm-5-3">GLM - 5 . 3 API: Pricing, Benchmarks & Docs | Together AI</a></li>
<li><a href="https://arxiv.org/abs/2206.07682">[2206.07682] Emergent Abilities of Large Language Models</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极但带有谨慎态度。用户报告了令人印象深刻的实际结果，例如在模型无缝执行包含 WordPress 插件 0-day 和内核漏洞利用的红队场景后，订阅从 18 美元迅速升级到 80 美元；也有人指出它仍略逊于 Claude Sonnet 和 Fable 等竞品，并对大规模漏洞扫描成本不断上升提出质疑。

**标签**: `#AI`, `#LLM`, `#cybersecurity`, `#coding`, `#model release`

---

<a id="item-3"></a>
## [步入黑暗：执法黑客时代来临](https://blog.cryptographyengineering.com/2026/08/14/everything-is-about-to-go-dark/) ⭐️ 8.0/10

这篇发布于 2026 年 8 月 14 日的博客文章剖析了‘Going Dark（走向黑暗）’辩论，并指出执法黑客已成为绕过加密通信的核心手段。文章认为，简单要求开后门的时代正在被利用软件漏洞和部署网络调查技术所取代。 这场辩论的结果将影响加密政策，进而关系到数十亿用户的隐私与安全。随着执法部门越来越多地转向黑客手段而非合法后门，端到端加密的可靠性以及国家资助入侵的规则需要公众审视。 这篇分析指出，可用软件漏洞的数量可能很快接近上限，从而限制基于黑客手段的访问方式。它还强调，执法黑客往往依赖保密、欺骗和漏洞储备，这引发了关于监督与披露机制的担忧。

hackernews · vslira · Aug 14, 20:52 · [社区讨论](https://news.ycombinator.com/item?id=49304447)

**背景**: “Going Dark（走向黑暗）”问题指的是：政府在法律上有权搜查某台设备或某段通信，却因强加密而缺乏技术手段。执法黑客（又称网络调查技术，NITs）通过键盘记录器、漏洞利用或其他方式，在加密生效前访问目标设备。美国的政策和法律框架难以跟上技术发展，Apple 与 FBI 的纠纷便是一个例子。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.csis.org/blogs/strategic-technologies-blog/encryption-and-going-dark-cutting-through-gordian-knot">Encryption and Going Dark – Cutting through the Gordian Knot | CSIS</a></li>
<li><a href="https://www.congress.gov/crs-product/R44827">Law Enforcement Using and Disclosing Technology Vulnerabilities | Congress.gov | Library of Congress</a></li>
<li><a href="https://www.justsecurity.org/60785/shining-light-federal-law-enforcements-computer-hacking-tools/">Shining a Light on Federal Law Enforcement’s Use of Computer Hacking Tools</a></li>

</ul>
</details>

**社区讨论**: 评论区讨论热烈且观点不一。Animats 提供了物理窃听时代电话线路费用的历史背景；mbroshi 不同意博文中关于可用漏洞将很快见顶的判断。fitblipper 嘲笑了‘Going Dark’这一说法，指出监控摄像头普及、元数据大量共享；Insimwytim 则对比了尖端攻击与现实世界中常见的安全失误。

**标签**: `#cryptography`, `#law enforcement`, `#encryption`, `#surveillance`, `#security`

---

<a id="item-4"></a>
## [Opus 5 体验变差：后训练优化对象是智能体而非人类](https://mun-logadan.github.io/why-does-opus-5-feel-worse/) ⭐️ 8.0/10

一篇新文章认为，Anthropic 于 2026 年 7 月 24 日发布的 Claude Opus 5 之所以让人用起来感觉更差，是因为其后训练优先服务智能体之间的通信，生成省略、抽象且让人类读者疲惫的文本。作者指出，该模型的输出是为其他 AI 智能体而不是为人优化的。 这一批评揭示了一个前沿模型开发的潜在转向：随着模型越来越多地以智能体任务为基准评估，人类可读性和对话体验可能被排在次要位置。开发者和普通用户可能因与写作风格面向机器优化的模型交互而承受隐性的效率成本。 文章特别指出，该模型喜欢写绕开重点的省略句、过于抽象的措辞，以及用无生命名词作主语来制造句尾的'意外揭示'。社区反馈还提到，模型频繁地自我坦白和冗长的'诚实'也是让人疲惫的风格的一部分。

hackernews · numeri · Aug 14, 10:12 · [社区讨论](https://news.ycombinator.com/item?id=49296740)

**背景**: 后训练（post-training）指的是大型语言模型在初始预训练之后的阶段，通过 RLHF、指令微调、推理微调等技术让模型行为朝预期目标发展。当这些目标强调自主智能体的任务完成（如编程、研究或多步工具使用）时，模型可能内化更适合其他智能体而非人类交流的表达模式。Claude Opus 5 作为一款强大的智能体编程模型发布，价格仅为 Claude Fable 5 的一半，这也反映出 Anthropic 对智能体性能的关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-opus-5">Introducing Claude Opus 5 \ Anthropic</a></li>
<li><a href="https://benchlm.ai/models/claude-opus-5">Claude Opus 5 Benchmarks, Pricing & Speed (August 2026)</a></li>
<li><a href="https://rlhfbook.com/">Reinforcement Learning from Human Feedback and LLM Post - Training</a></li>

</ul>
</details>

**社区讨论**: 评论区大多赞同文章论点：有用户觉得 Opus 5 的省略式和跳跃式写作令人恼火，另有用户用完了额度后转向 OpenAI 的 Sol，因为 Opus 5 的'诚实'坦白令人筋疲力尽。一种反复出现的猜测是，人类已不再是后训练的目标受众；至少一位用户退回 Opus 4.8，认为模型质量明显下滑。

**标签**: `#AI`, `#language models`, `#UX`, `#agent communication`, `#model behavior`

---

<a id="item-5"></a>
## [Firefox 成为唯一支持完整版 uBlock Origin 的主流浏览器](https://www.pcworld.com/article/3212428/firefox-is-now-the-last-major-browser-that-still-supports-ublock-origin.html) ⭐️ 8.0/10

随着 Chrome 全面转向 Manifest V3，uBlock Origin 完整版已无法在基于 Chromium 的浏览器中运行，Firefox 因此成为唯一仍完全支持它的主流浏览器。 uBlock Origin 被广泛视为广告拦截的黄金标准，因此它在 Chrome 上的缺失削弱了用户对广告和追踪器的控制。这巩固了 Firefox 作为注重隐私用户首选浏览器的地位，也标志着浏览器扩展能力的重大转变。 Chrome 的 Manifest V3 用 declarativeNetRequest API 取代了阻塞式 webRequest API，这会限制过滤规则数量，并缺少 uBlock Origin 的动态过滤能力。非官方移植版 uBlock-mv3 试图让完整版适配 MV3，但面临很大限制。

hackernews · DemiGuru · Aug 14, 19:03 · [社区讨论](https://news.ycombinator.com/item?id=49303202)

**背景**: Manifest V3 是 Google 于 2020 年推出的最新扩展平台，表面上是为了提升隐私、安全和性能，但它将 webRequestBlocking 权限限定给企业托管的扩展。uBlock Origin 是一款广受欢迎的开源内容拦截器，依赖强大的 webRequest API 实时拦截广告和追踪器。Chrome、Edge 等 Chromium 浏览器正在迁移到 MV3，迫使广告拦截插件改用功能较弱的 declarativeNetRequest API。Firefox 扩展了对后台脚本和 Manifest V2 的支持，因此 uBlock Origin 仍可继续运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.chrome.com/docs/extensions/develop/migrate/what-is-mv3">Extensions / Manifest V 3 | Chrome for Developers</a></li>
<li><a href="https://adblock-tester.com/ad-blockers/manifest-v3-ad-blocker-impact/">The Manifest V3 Changes — Did Google Just Break Your Ad Blocker? (And What to Do Next) - AdBlock Tester</a></li>
<li><a href="https://extensionworkshop.com/documentation/develop/manifest-v3-migration-guide/">Manifest V 3 migration guide | Firefox Extension Workshop</a></li>

</ul>
</details>

**社区讨论**: 评论者大多称赞 Firefox 对 uBlock Origin 更新的审核及其完整功能支持，同时批评 Google 的 MV3 改动不尊重用户。有人提到非官方移植版 uBlock-mv3，并讨论了 Lite 版的拦截质量；还有开发者表示，由于 MV3 使扩展失效，他们关闭了自己的扩展。

**标签**: `#Firefox`, `#uBlock Origin`, `#Manifest V3`, `#Ad-blocking`, `#Browser Extensions`

---

<a id="item-6"></a>
## [讽刺网站“Every Fucking Website”嘲讽糟糕的网页设计](https://lxe.github.io/everywebsite/) ⭐️ 8.0/10

讽刺网站“Every Fucking Website”（2020）模仿了激进的弹窗、Cookie 横幅和自动播放视频等现代网页设计反模式。该网站在 Hacker News 上走红，获得了大量评论和 8.0/10 的评分。 这种讽刺凸显了这些 UX 暗黑模式已经变得多么侵入性和普遍，引发了关于它们对用户信任和浏览体验影响的更广泛讨论。对网页开发者和设计师而言，这场讨论突显了转化优化与尊重用户之间的张力。 该网站托管在 lxe.github.io 上，据一位评论者称，它只从自己的域名加载 JavaScript，不像典型网站那样从 12-18 个外部域名加载。评论者还表示缺少一些反模式，比如“在 App 中更好”的提示、虚假的购买通知和强制账户登录弹窗。

hackernews · doubletwoyou · Aug 14, 14:31 · [社区讨论](https://news.ycombinator.com/item?id=49299222)

**背景**: 这种自我指涉的讽刺作品通过重现现代网页体验中最令人沮丧的部分来实现效果。用户越来越频繁地遇到 Cookie 横幅、新闻通讯弹窗和持续追踪提示，这些都会阻碍内容阅读。该网站模仿这些模式，对当前的网页设计趋势进行了犀利批判，而病毒式传播的回应表明许多用户对此深有同感。

**社区讨论**: 评论者以幽默和认同感回应，分享了他们与暗黑模式打交道的亲身经历。有人承认，像“有人刚刚购买了 X”这样的提示确实能显著提升电商转化率，尽管代价是“轻微的自憎”。其他人则开玩笑说该网站加载太快、缺少跨域跟踪，或者没有谷歌登录弹窗。

**标签**: `#web-design`, `#ux`, `#satire`, `#web-development`, `#community-discussion`

---

<a id="item-7"></a>
## [不要分类，要“幻觉”：先生成标签再用嵌入匹配](https://simonwillison.net/2026/Aug/14/dont-classify-hallucinate/) ⭐️ 8.0/10

西蒙·威利森介绍了道格·特恩布尔提出的标签方案：与其让 LLM 从成千上万个现有标签中选择，不如让它先“凭空”生成看似合理的标签，再用向量嵌入把这些标签映射到语料库中最接近的真实标签。威利森计划用这个方法来处理博客上 1,856 个尚未打标签的旧帖子。 这一方法意义重大，因为当标签集合非常庞大、超出上下文限制时，LLM 直接分类变得不切实际——这是真实内容打标和电商场景中的常见难题。该技术把“生成”和“固定词表”解耦，提供了一种可扩展的零样本替代方案，并且用现有嵌入模型就能轻松实现。 道格·特恩布尔的示例提示词要求模型为家具/家居用品创造全新的分类，并给出标签形态示例，比如“Furniture / Living Room Furniture / Coffee Tables & End Tables / Coffee Tables”，然后让模型为“brown coffee table”这样的查询生成分类。生成之后，这些“幻觉”标签会被向量化，并通过向量相似度检索匹配到最接近的现有标签，思路与 HyDE（假设性文档嵌入）一脉相承。

rss · Simon Willison · Aug 14, 21:54

**背景**: 向量嵌入能将词、句子或文档表示为稠密的数值向量，从而编码语义信息，使含义相近的内容在向量空间中彼此靠近。向量相似度检索（最近邻搜索）可以找到与查询向量最相似的内容，广泛应用于搜索和 RAG（检索增强生成）系统中。HyDE 是一种相关的检索技术：当相关文档稀缺时，先为查询生成一篇假设性文档，再利用它的嵌入来改进检索。这些概念正是“先无约束生成标签、再映射到已知词表”这一思路的基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vector_embedding">Vector embedding</a></li>
<li><a href="https://www.geeksforgeeks.org/data-science/hypothetical-document-embeddings-hyde-hyde/">Introduction to Hypothetical Document Embeddings (HyDE)</a></li>
<li><a href="https://docs.opensearch.org/latest/vector-search/getting-started/vector-search-basics/">Vector search basics | OpenSearch Documentation</a></li>

</ul>
</details>

**标签**: `#LLM`, `#embeddings`, `#tagging`, `#vector search`, `#AI`

---

<a id="item-8"></a>
## [Vivodyne 的 AI 机器人实验室每年测试 300 万份人体组织，目标终结动物试验。](https://www.fastcompany.com/91589344/the-worlds-largest-biological-datacenter-could-help-make-animal-testing-obsolete) ⭐️ 8.0/10

Vivodyne 在旧金山南部设有 12 个“蜂巢”机器人实验室，通过 AI 设计的实验每年可对超过 300 万个实验室培养的人体组织样本进行受控试验。这一容量约为美国全部临床试验总量的两倍。 鉴于约 90%的临床试验在通过动物试验后仍告失败，这一突破可能大幅加速药物研发并减少对动物试验的依赖。如果成功，它或能让更安全、更有效的药物更快造福患者。 每个实验室被描述为“壁橱大小”，总容量是美国所有临床试验总和的两倍。该平台将实验室培养的 3D 人体组织与 AI 驱动的实验设计相结合，从而规模化生成人类数据。

telegram · zaihuapd · Aug 14, 01:48

**背景**: 实验室培养的 3D 人体组织通常被称为类器官，比动物模型更真实地模拟人体器官，越来越多地用于药物测试。传统临床前测试仍大量依赖动物模型，而后者往往无法预测人体反应，是临床试验失败率高的原因之一。AI 驱动的实验设计利用算法自动规划和优化高通量实验，使筛选的规模和速度大幅提升。Vivodyne 的系统正将这些趋势结合起来，以前所未有的规模生成人类数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.vivodyne.com/">Vivodyne | Make biology computable</a></li>
<li><a href="https://www.hsci.harvard.edu/organoids">hsci.harvard.edu/ organoids</a></li>
<li><a href="https://www.mdpi.com/2076-3417/15/9/5208">A Helping Hand: A Survey About AI-Driven Experimental Design ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#drug discovery`, `#biotech`, `#animal testing`, `#robotics`

---

<a id="item-9"></a>
## [小红书开源 dots3-note：280B MoE，16B 激活参数](https://x.com/dotsstudioai/status/2088083314855018521) ⭐️ 8.0/10

小红书 dots 实验室开源了 dots3-note preview，这是 dots3 系列首个开放权重模型。它是一个 280B 参数的混合专家（MoE）模型，激活参数仅 16B，支持 512K 上下文，可处理文本、图片、视频和音频输入。 此次发布让 AI 社区能够以较低推理成本使用大型多模态 MoE 模型，可能推动开源智能体研究。同时引入了新的强化学习方法 TEMPO，以及两个真实场景智能体基准，提高了长程任务评测的标准。 模型权重以 Apache 2.0 许可在 Hugging Face 上发布，GitHub 提供了八卡 GPU 推理指南。配套的 VibeSearchBench 和 VibeLifeBench 基准面向更真实、更难评估的长程智能体场景。

telegram · zaihuapd · Aug 14, 08:27

**背景**: 混合专家（MoE）模型每个 token 只激活部分参数，因此能在总参数量很大的情况下降低计算成本。小红书 dots3-note 延续了开源大型 MoE 模型的趋势；TEMPO 是一种新的强化学习方法，通过自批判和测试时价值估计来训练长程智能体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/studio-dots-ai/dots3-note-prev">GitHub - studio-dots-ai/dots3-note-prev: dots3 note preview</a></li>
<li><a href="https://eu.36kr.com/en/p/3938759517896072">Xiaohongshu Open-Sourced Dots3-Note: The Same-Series Model ...</a></li>
<li><a href="https://vibebench.github.io/VibeLifeBench_homepage/">VibeLifeBench — Can Your Life Agent Be Proactive and Persistent in...</a></li>

</ul>
</details>

**标签**: `#open-source`, `#MoE`, `#reinforcement-learning`, `#multimodal`, `#agent-benchmark`

---

<a id="item-10"></a>
## [苹果官宣换帅：库克卸任 CEO，特努斯 2026 年接任](https://t.me/zaihuapd/43191) ⭐️ 8.0/10

苹果宣布管理层交接：现任 CEO 蒂姆·库克将卸任，出任董事会执行董事长；硬件工程高级副总裁约翰·特努斯将从 2026 年 9 月 1 日起担任新任 CEO。董事会已一致批准这项安排。 这是自 2011 年库克接替史蒂夫·乔布斯以来苹果首次更换 CEO，对科技行业而言具有历史性意义。特努斯长期负责 iPhone、Mac、iPad、AirPods 等核心硬件产品，他的接任意味着苹果将保持战略延续性。 根据方案，现任董事长 Arthur Levinson 将于 9 月 1 日转任首席独立董事，特努斯同日加入董事会。特努斯 2001 年加入苹果，2013 年升任硬件工程副总裁，2021 年进入高管团队。

telegram · zaihuapd · Aug 14, 11:00

**背景**: 蒂姆·库克自 2011 年接替史蒂夫·乔布斯出任苹果 CEO，带领公司成长为全球市值最高的企业之一。此次换帅是一次经过精心规划的接班安排，库克转任执行董事长后将继续为过渡提供支持。约翰·特努斯是苹果硬件产品线的核心人物，因此被视为顺理成章的继任者。执行董事长是专注战略与董事会治理的职务，与负责日常运营的 CEO 角色不同。

**标签**: `#Apple`, `#CEO Transition`, `#Tech Industry`, `#Leadership`, `#Tim Cook`

---

<a id="item-11"></a>
## [PostgreSQL 高危 to_char 漏洞可致任意代码执行](https://www.postgresql.org/support/security/CVE-2026-14669/) ⭐️ 8.0/10

PostgreSQL 披露了高危漏洞 CVE-2026-14669，这是 to_char(timestamptz) 函数在处理超长 POSIX 时区缩写时引发的堆缓冲区溢出。该漏洞可使低权限数据库用户以 PostgreSQL 服务进程的操作系统权限执行任意代码。 该漏洞 CVSS 评分为 8.8，严重程度很高，需要立即修补。由于受影响版本涵盖多个受支持的版本分支，许多生产数据库都处于风险之中，管理员应尽快应用小版本更新以防止系统被入侵。 受影响版本包括 18.5、17.11、16.15、15.19 和 14.24 之前的版本。由于 18.5 因回归问题未正式发布，18 系列用户应升级至 18.6；其他系列用户应分别升级至 17.11、16.15、15.19 或 14.24。修补只需替换程序文件并重启服务，无需转储数据库或运行 pg_upgrade。

telegram · zaihuapd · Aug 14, 14:35

**背景**: PostgreSQL 的 to_char() 函数将时间戳、数字等值转换为格式化字符串。timestamptz 数据类型（带时区的时间戳）存储时间戳及时区信息。POSIX 时区缩写是类似 "EST" 的短字符串，用于引用时区；在格式函数中处理超长或格式错误的缩写可能造成堆缓冲区溢出。正确打补丁并理解升级路径对数据库安全至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/functions-formatting.html">PostgreSQL: Documentation: 18: 9.8. Data Type Formatting Functions</a></li>
<li><a href="https://www.postgresql.org/docs/current/datatype-datetime.html">PostgreSQL: Documentation: 18: 8.5. Date/Time Types</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#CVE`, `#security`, `#vulnerability`, `#to_char`

---

<a id="item-12"></a>
## [苹果联手阿里训练中国专属 AI 模型，或成首个获批外企](https://www.reuters.com/business/retail-consumer/apple-trains-its-own-ai-model-china-market-with-alibabas-support-sources-say-2026-08-14/) ⭐️ 8.0/10

苹果在阿里巴巴支持下，正专门为中国市场训练一款大语言模型，放弃此前依赖第三方模型的策略。Apple Intelligence 预计在未来数月随 iOS 更新在华上线，中国网信办已对其生成式 AI 服务完成备案。 若获批，苹果将成为首个获北京批准在华提供自有 AI 模型的外国公司。这一重大战略举措对 AI 监管、市场竞争以及苹果在中国智能手机和 AI 生态中的地位都具有深远影响。 这款中国专属模型由苹果自研，并获得阿里的算力支持，取代了此前整合第三方 AI 合作伙伴的方式。中国网信办已于上个月备案该生成式 AI 服务，预计将在未来数月内通过 iOS 更新上线。

telegram · zaihuapd · Aug 14, 14:47

**背景**: 中国要求所有面向公众的生成式 AI 服务向网信办完成备案，涵盖自研、微调及调用第三方模型等情况。截至 2025 年 6 月，全国已有 439 款生成式 AI 服务完成备案。该监管框架由《生成式人工智能服务管理暂行办法》及相关技术要求定义，要求企业提交模型安全、数据处理和算法透明度等材料。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.tencent.com/developer/article/2541787">生成式人工智能服务上线备案（大模型备案）材料清单详解-腾讯云开发者...</a></li>
<li><a href="https://developer.aliyun.com/article/1674963">生成式人工智能服务上线备案（大模型备案）材料清单详解</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1919326896111489390">生成式人工智能服务大模型备案申请全流程及核心要求 - 知乎</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AI`, `#China`, `#Alibaba`, `#Regulation`

---