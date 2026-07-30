---
layout: default
title: "Horizon Summary: 2026-07-30 (ZH)"
date: 2026-07-30
lang: zh
---

> From 33 items, 13 important content pieces were selected

---

1. [在任意 M 系列 Mac 上仅用 2GB 内存运行 Gemma 4 26B](#item-1) ⭐️ 9.0/10
2. [Mitchell Hashimoto 发布 Superlogical，基于非营利组织拥有的 Ghostty](#item-2) ⭐️ 9.0/10
3. [俄罗斯指控 Telegram 创始人杜罗夫协助恐怖活动，发出国际通缉](#item-3) ⭐️ 9.0/10
4. [OpenAI 向十万研究人员免费提供 AI 模型](#item-4) ⭐️ 9.0/10
5. [AI 初创公司越来越少发表研究成果](#item-5) ⭐️ 8.0/10
6. [KOReader：开源软件增强电子墨水阅读器体验](#item-6) ⭐️ 8.0/10
7. [Kimi 发布 K3-256k 模型，上下文 256k，价格减半](#item-7) ⭐️ 8.0/10
8. [AI 公司为数据中心招募数千电工和木工](#item-8) ⭐️ 8.0/10
9. [AI 蠕虫通过 Word 文档中的 Copilot 自我传播](#item-9) ⭐️ 8.0/10
10. [研究发现长政策文件无法有效约束 LLM 代理](#item-10) ⭐️ 8.0/10
11. [Darktable：免费开源 RAW 照片编辑器受关注](#item-11) ⭐️ 8.0/10
12. [Matthew Green：AI 密码分析或可验证或颠覆后量子算法](#item-12) ⭐️ 8.0/10
13. [报告：Hugging Face 被广泛用于生成深度伪造裸照](#item-13) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [在任意 M 系列 Mac 上仅用 2GB 内存运行 Gemma 4 26B](https://github.com/drumih/turbo-fieldfare) ⭐️ 9.0/10

TurboFieldfare 是一个用 Swift 和 Metal 编写的开源推理引擎，通过从 SSD 流式传输路由专家，在任何 M 系列 Mac 上仅用约 2GB 内存即可运行 4 位量化的 Gemma 4 26B 模型。 这一突破使强大的 26B 参数模型可在低内存 Mac（8GB 或 16GB）上运行，此前这些设备无法加载完整的 14GB 量化权重，从而为数百万用户普及了设备端 AI。 该引擎在 8GB M2 MacBook Air 上达到 5–6 tok/s，在 M5 MacBook Pro 上达到 31–35 tok/s，通过小型专家缓存和有界并行预读来掩盖 SSD 延迟。

hackernews · gitpusher42 · Jul 29, 15:05 · [社区讨论](https://news.ycombinator.com/item?id=49098510)

**背景**: Gemma 4 26B 是一种混合专家（MoE）模型，每个 token 仅激活一部分“专家”层，适合 SSD 流式传输。传统推理会将所有权重加载到内存中，而 TurboFieldfare 仅将共享层和 KV 缓存保留在内存中，按需从 SSD 获取专家。该技术借鉴了早期的 Flash-MoE 等工作，后者展示了在消费级硬件上流式传输大型 MoE 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gemma4.dev/docs/models">Model Reference | gemma 4 .dev — The Gemma 4 Developer Hub</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://insiderllm.com/guides/flash-moe-run-397b-model-laptop/">Flash-MoE: Run a 397B Model on a 48GB Laptop... | InsiderLLM</a></li>

</ul>
</details>

**社区讨论**: 社区反应热烈，用户称赞这项工程成就并分享了实际基准测试。一些人指出 llama.cpp 配合 mmap 也能在有限内存中运行大模型，但 TurboFieldfare 将 SSD 读取与推理同步被视为关键优化。还提供了在旧版 macOS 上编译的有用提示。

**标签**: `#inference engine`, `#on-device AI`, `#Gemma`, `#Swift/Metal`, `#model streaming`

---

<a id="item-2"></a>
## [Mitchell Hashimoto 发布 Superlogical，基于非营利组织拥有的 Ghostty](https://www.superlogical.com/) ⭐️ 9.0/10

Mitchell Hashimoto 宣布成立 Superlogical 公司，该公司基于开源终端库 libghostty 构建，而核心项目 Ghostty 由非营利基金会拥有。 这种创新的商业模式将开源核心与营利实体分离，可能为可持续的开源开发树立先例，同时确保终端库由社区所有。 Superlogical 将把 libghostty 作为公共构建模块，使用与所有人相同的 MIT 许可组件，并将上游共享终端改进，使所有 libghostty 用户受益。

hackernews · yan · Jul 29, 15:41 · [社区讨论](https://news.ycombinator.com/item?id=49098965)

**背景**: Ghostty 是一个快速、功能丰富、跨平台的终端模拟器，使用原生界面和 GPU 加速。其核心库 libghostty 旨在将终端功能嵌入第三方项目。通过将 Ghostty 所有权转移给非营利组织，Hashimoto 确保基础技术保持开放并受社区治理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ghostty-org/ghostty">GitHub - ghostty-org/ghostty: 👻 Ghostty is a fast, feature-rich, and cross-platform terminal emulator that uses platform-native UI and GPU acceleration.</a></li>
<li><a href="https://mitchellh.com/writing/libghostty-is-coming">Libghostty Is Coming – Mitchell Hashimoto</a></li>
<li><a href="https://ghostty.org/">Ghostty</a></li>

</ul>
</details>

**社区讨论**: 评论普遍积极，赞扬非营利所有权模式和上游贡献的承诺。一些用户将其与 OLE/COM 类比，少数人批评公告标题晦涩难懂。

**标签**: `#software-engineering`, `#open-source`, `#terminal`, `#startup`, `#ghostty`

---

<a id="item-3"></a>
## [俄罗斯指控 Telegram 创始人杜罗夫协助恐怖活动，发出国际通缉](https://www.interfax.ru/russia/1106228) ⭐️ 9.0/10

7 月 29 日，俄罗斯联邦安全局（FSB）依据《刑法》第 205.1 条第 1.1 款对 Telegram 创始人帕维尔·杜罗夫提起刑事指控，指控其协助恐怖活动，并将其列入国际通缉名单。 此举标志着俄罗斯当局对科技平台进行重大打压，威胁到俄罗斯及全球数百万 Telegram 用户的言论自由和隐私，并可能为其他国家针对平台高管树立先例。 FSB 声称，Telegram 管理层拒不删除被乌克兰情报机构及恐怖、极端主义组织用于在俄罗斯境内策划破坏活动、恐怖袭击、大规模杀戮及网络诈骗的频道、群组和机器人，导致多人伤亡和数十亿卢布损失。

telegram · zaihuapd · Jul 29, 05:56

**背景**: 帕维尔·杜罗夫是俄罗斯出生的 Telegram 创始人，Telegram 是一款全球拥有超过 9 亿用户的流行加密通讯应用。Telegram 曾面临多国政府在内容审核上的压力，但这是国家首次针对其创始人本人提出与恐怖主义相关的刑事指控。俄罗斯曾在 2018 年试图屏蔽 Telegram，但后来解除了禁令。

**标签**: `#Telegram`, `#Pavel Durov`, `#Russia`, `#legal`, `#terrorism`

---

<a id="item-4"></a>
## [OpenAI 向十万研究人员免费提供 AI 模型](https://openai.com/index/chatgpt-for-academic-researchers/) ⭐️ 9.0/10

2026 年 7 月 29 日，OpenAI 宣布推出 ChatGPT for Academic Researchers 项目，计划在 2027 年前向全球多达 10 万名研究人员免费提供其前沿 GPT-5.6 模型，首批 1 万人将于今年夏季开放。 这项价值数百万美元的举措大大降低了学术研究的门槛，使得在基因组学、蛋白质建模等领域进行大规模 AI 辅助研究成为可能，有望加速科学突破。 研究人员可以使用 GPT-5.6 系列模型（Luna、Terra、Sol），并最多邀请 4 位合作者；工作区默认不将数据用于模型训练。该项目是 OpenAI 到 2027 年投入超过 2.5 亿美元支持外部科研的一部分。

telegram · zaihuapd · Jul 30, 00:17

**背景**: GPT-5.6 是 OpenAI 于 2026 年 7 月 9 日发布的大型语言模型系列，包含 Luna、Terra 和 Sol 三个变体。Sol 变体于 2026 年 7 月下旬预览，在编程、科学和网络安全方面具备先进能力，并配备了更强的安全措施。该项目是 OpenAI 推动 AI 助力科学研究的更广泛举措的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT-5.6 Sol: a next-generation model | OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI for Science`, `#Academic Research`, `#GPT-5.6`, `#Machine Learning`

---

<a id="item-5"></a>
## [AI 初创公司越来越少发表研究成果](https://www.science.org/content/article/ai-s-top-startups-are-barely-publishing-their-research) ⭐️ 8.0/10

顶尖 AI 初创公司几乎不再发表研究成果，为保护竞争优势而远离开放科学，据 Science.org 报道。 这一趋势威胁到 AI 领域的透明度和可重复性，而这些对于科学进步和公众信任至关重要。 文章指出，即使是起初开放研究的 OpenAI 也减少了发表；引用量被用作影响力的不完美代理指标。

hackernews · YeGoblynQueenne · Jul 29, 21:25 · [社区讨论](https://news.ycombinator.com/item?id=49103285)

**背景**: 历史上，AI 研究依赖公开出版和合作蓬勃发展。如今，初创公司担心发表成果会让 OpenAI、Anthropic 等竞争对手抄袭，使数月努力付诸东流。

**社区讨论**: 评论者分享了个人经历：一家初创公司尝试发表三年后放弃；另一家故意不发表以防被大公司抄袭。有人批评 AI 研究的“博客化”，使得声明更难验证。

**标签**: `#AI`, `#research publishing`, `#startups`, `#transparency`, `#HackerNews discussion`

---

<a id="item-6"></a>
## [KOReader：开源软件增强电子墨水阅读器体验](https://koreader.rocks/) ⭐️ 8.0/10

KOReader，一款用于电子墨水设备的开源电子书阅读器，在 Hacker News 上引起了广泛关注，讨论其功能和用户体验。 这一讨论凸显了用户对电子阅读器开源软件日益增长的兴趣，使 Kindle 和 Kobo 等设备功能更丰富、寿命更长。 KOReader 支持 EPUB、PDF、MOBI 等多种格式，兼容 Kindle、Kobo、PocketBook、Android 和 Linux 设备；但部分用户反映界面不直观且手势操作有延迟。

hackernews · Cider9986 · Jul 29, 11:05 · [社区讨论](https://news.ycombinator.com/item?id=49095865)

**背景**: Kindle 和 Kobo 等电子墨水设备通常运行限制自定义的专有软件。KOReader 是一款免费开源应用，可安装在已越狱的 Kindle 或 Kobo 设备上，提供原生 EPUB/PDF 支持、可定制手势和 Calibre 同步等高级功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/KOReader">KOReader</a></li>
<li><a href="http://koreader.rocks/">KOReader</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区意见不一：许多用户称赞 KOReader 提升了阅读体验，但也有人批评其界面不直观、手势延迟以及可用性，称其为‘电子阅读器界的 GIMP’。

**标签**: `#open-source`, `#e-reader`, `#software`, `#kindle`, `#kobo`

---

<a id="item-7"></a>
## [Kimi 发布 K3-256k 模型，上下文 256k，价格减半](https://www.kimi.com/code/docs/en/kimi-code/models) ⭐️ 8.0/10

Kimi 推出了 K3-256k 模型，提供 256k 令牌的上下文窗口，API 配额成本仅为 100 万令牌旗舰版 K3 的一半，且在短上下文内保持相同智能。 这一定价策略使长上下文 AI 对开发者更易用，可能促使竞争对手根据上下文长度提供分级定价，同时仍为需要 1M 上下文的用户保留选项。 K3-256k 模型与 1M 版本是分开的；切换时，像 Kimi Code CLI 这样的工具会自动压缩超过 256k 的上下文。该模型未量化，仅上下文窗口缩小。

hackernews · monneyboi · Jul 29, 19:25 · [社区讨论](https://news.ycombinator.com/item?id=49101852)

**背景**: 在大语言模型中，上下文长度指模型一次能处理的文本量（以令牌计）。更长上下文会增加计算成本，因为需要关注更多令牌。Kimi K3 是拥有 1M 令牌上下文的旗舰模型，256k 变体为不需要完整 1M 上下文的用例提供了经济高效的替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/code/docs/en/kimi-code/models">Model Configuration | Kimi Code Docs</a></li>
<li><a href="https://datanorth.ai/blog/context-length">LLM Context Length & Context Window Explained (2026)</a></li>
<li><a href="https://insiderllm.com/guides/context-length-explained/">Context Length Explained: Why It Eats Your VRAM | InsiderLLM</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞价格减半为'重大'，并注意到与 OpenAI 的上下文长度定价阶梯相似。一些人讨论了硬性截止与平滑梯度的权衡，而另一些人澄清这是 API 级别的更改，模型未量化，只是上下文更小。

**标签**: `#AI`, `#large language models`, `#pricing`, `#context length`, `#API`

---

<a id="item-8"></a>
## [AI 公司为数据中心招募数千电工和木工](https://www.nytimes.com/2026/07/29/business/economy/data-center-electricians-training.html) ⭐️ 8.0/10

大型 AI 公司正在招聘数千名电工和木工来建设数据中心，这反映了 AI 基础设施扩张带来的大规模劳动力转移。 这一趋势凸显了 AI 基础设施对熟练技工日益增长的需求，可能重塑建筑行业的劳动力市场和培训项目。 该文章重点关注电工和木工的招聘，但由于液冷系统的使用增加，未来数据中心可能还需要水管工。

hackernews · thm · Jul 29, 14:43 · [社区讨论](https://news.ycombinator.com/item?id=49098198)

**背景**: 数据中心是容纳服务器和网络设备的大型设施，用于云计算和 AI。建设数据中心需要专业的建筑技能，包括布线和木工。AI 的繁荣导致数据中心建设激增，从而对技工产生需求。

**社区讨论**: 社区评论对数据中心建设的繁荣-萧条周期性表示谨慎，指出电工可能面临收入波动。其他人则欢迎技工获得高薪机会，还有评论者强调了液冷趋势下未来对水管工的需求。

**标签**: `#AI infrastructure`, `#data centers`, `#labor market`, `#trades`, `#economy`

---

<a id="item-9"></a>
## [AI 蠕虫通过 Word 文档中的 Copilot 自我传播](https://enklypesalt.com/posts/context-collapse-part3-ai-worming-through-word/) ⭐️ 8.0/10

研究员 Håkon Måløy 展示了一种提示注入攻击，能将 Word 中的微软 Copilot 变成自我复制的 AI 蠕虫，使嵌入文档的恶意指令传播到新文件。 该漏洞暴露了集成 LLM 的应用程序中的关键安全缺陷，因为获得广泛权限的 AI 代理可能无意中执行并传播隐藏指令，威胁数据隐私和系统完整性。 该攻击利用间接提示注入，将对抗性提示隐藏在共享文档中，而 Copilot 无法区分指令与数据，使得蠕虫能够自我传播，目前尚无可靠的缓解措施。

hackernews · Canopy9560 · Jul 29, 11:44 · [社区讨论](https://news.ycombinator.com/item?id=49096188)

**背景**: AI 蠕虫是一种自主恶意软件，通过注入自复制提示来利用大语言模型和自动化流程。提示注入攻击利用 LLM 无法区分开发者指令、用户输入和外部内容的弱点，使隐藏命令劫持输出。随着 AI 代理获得更多用户数据和操作权限，此类攻击变得愈发危险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://www.sentinelone.com/cybersecurity-101/cybersecurity/ai-worms/">AI Worms Explained: Adaptive Malware Threats - SentinelOne</a></li>
<li><a href="https://www.emergentmind.com/topics/ai-worms">AI Worms: Autonomous Self-Propagating Malware</a></li>

</ul>
</details>

**社区讨论**: 社区成员认为，若不将指令与数据分离，此类漏洞可能无法修复，并警告说授予代理过多权限可能导致广泛利用，包括窃取凭证或钱包数据。

**标签**: `#AI security`, `#prompt injection`, `#Copilot`, `#cybersecurity`, `#worms`

---

<a id="item-10"></a>
## [研究发现长政策文件无法有效约束 LLM 代理](https://arxiv.org/abs/2607.25398) ⭐️ 8.0/10

一项新研究（Handbook.md）表明，长政策文件即使被放入上下文窗口，也无法可靠地约束大语言模型代理的行为，这是因为上下文窗口的限制和模型注意力缺陷。 这一发现挑战了长指令能有效控制 AI 代理的假设，对人工智能安全以及在需要严格遵守政策的敏感领域的部署提出了严重担忧。 该论文在基准测试中评估了多种 LLM，要求代理遵循长政策文件，发现性能随文档长度急剧下降，即使是先进模型也无法在长时间交互中保留关键指令。

hackernews · spIrr · Jul 29, 13:01 · [社区讨论](https://news.ycombinator.com/item?id=49096969)

**背景**: 大语言模型的上下文窗口实际有效长度有限；尽管模型声称支持百万级 token，实际的注意力机制和量化问题会导致输入早期部分的信息丧失。因此，依赖长政策文件指导行为的代理型 AI 系统可能忽略或遗忘关键的安全约束。最近发布的 LongSafety 和 LongSafetyBench 等基准测试也指出了类似的长上下文安全性失败。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://aclanthology.org/2025.acl-long.1530.pdf">Evaluating Long-Context Safety of Large Language Models</a></li>
<li><a href="https://arxiv.org/html/2502.16971">LongSafety: Evaluating Long-Context Safety of Large Language Models</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认同这一发现，并分享了使用 Claude 等模型时无法持续遵守指令的真实体验。有人指出原因在于量化问题和糟糕的采样器，也有人认为即使是人类也难以处理长政策文档。一个反复出现的观点是，有效的智能代理行为需要对特定手册进行专门的后期训练。

**标签**: `#LLM`, `#long context`, `#AI safety`, `#benchmarks`

---

<a id="item-11"></a>
## [Darktable：免费开源 RAW 照片编辑器受关注](https://www.darktable.org/) ⭐️ 8.0/10

一场关于 Darktable 的社区讨论突显了其令人印象深刻的功能，许多用户称赞它是 Adobe Lightroom 等付费软件的免费替代品，但性能问题和工作流程变更也招致了批评。 作为一款开源 RAW 编辑器，Darktable 证明了免费软件可以与行业标准工具竞争，可能降低摄影师的门槛，并促进更易使用的照片编辑工作流程。 Darktable 是一款注重工作流程效率的非破坏性 RAW 处理器，但一些用户反映在现代硬件上存在性能问题，并指出在主要版本之间切换可能会破坏现有编辑。

hackernews · siatko · Jul 29, 12:33 · [社区讨论](https://news.ycombinator.com/item?id=49096654)

**背景**: Darktable 是一款根据 GPL-3.0 许可发布的免费开源摄影应用程序和 RAW 处理器。它作为虚拟的灯桌和暗房，用于组织和管理数字底片，支持包括 Linux、macOS、Windows 和 Solaris 在内的主要操作系统。与 Photoshop 等光栅编辑器不同，Darktable 专注于非破坏性 RAW 图像后期制作，使摄影师能够高效管理大量图像。一些用户认为其学习曲线陡峭，其工作流习惯与 Lightroom 等商业替代品有所不同。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Darktable">Darktable</a></li>
<li><a href="https://www.darktable.org/">darktable</a></li>

</ul>
</details>

**社区讨论**: 讨论呈现混合态度：许多用户高度赞扬 Darktable 的功能集和质量，有用户称‘我愿意每年为此支付 200 美元’，而另一些用户则批评其性能缓慢以及版本之间的破坏性工作流变更。一些用户指出 Darktable 的组织能力弱于 Lightroom，由于对项目方向的分歧，前维护者创建了名为 Ansel 的分支。

**标签**: `#open-source`, `#photography`, `#photo-editing`, `#raw-processing`

---

<a id="item-12"></a>
## [Matthew Green：AI 密码分析或可验证或颠覆后量子算法](https://simonwillison.net/2026/Jul/29/matthew-green/#atom-everything) ⭐️ 8.0/10

知名密码学家 Matthew Green 指出，当前向后量子密码学的转型为 AI 驱动的密码分析提供了绝佳时机，这些分析可能确认新算法的安全性，也可能暴露其弱点。 在全球从传统公钥密码转向后量子标准的背景下，AI 分析这些新型问题的能力可能增强对新算法的信心，也可能揭示灾难性漏洞，直接影响全球安全基础设施。 Green 特别提到 HAWK——一种基于格的后量子签名方案——作为当前众多候选标准的例子。他还引用了 Impagliazzo 的‘五个世界’分类，指出如果 AI 破坏了所有困难问题，我们可能最终落入 Minicrypt 世界。

rss · Simon Willison · Jul 29, 18:18

**背景**: 后量子密码学旨在开发能够抵抗量子计算机的算法。NIST 正在标准化像 HAWK 这样的新方案，这些方案依赖于被认为对经典和量子计算机都困难的问题。AI 密码分析利用机器学习来寻找密码算法的弱点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eprint.iacr.org/2026/1078">Post-Quantum HAWK Signature Acceleration with RISC-V-Based Hardware-Software Co-Design</a></li>
<li><a href="https://hawk-sign.info/">Hawk</a></li>
<li><a href="https://fanpu.io/blog/2022/impagliazzos-five-worlds/">Impagliazzo ' s Five Worlds, or The Computational... | Fan Pu Zeng</a></li>

</ul>
</details>

**标签**: `#cryptography`, `#post-quantum cryptography`, `#AI`, `#cryptanalysis`, `#public-key algorithms`

---

<a id="item-13"></a>
## [报告：Hugging Face 被广泛用于生成深度伪造裸照](https://www.theverge.com/ai-artificial-intelligence/971723/hugging-face-nudify-deepfake-undress-women-children) ⭐️ 8.0/10

欧洲非营利组织 AI Forensics 于 7 月 28 日发布的报告发现，开源模型托管平台 Hugging Face 被大量用于制作非自愿深度伪造色情图片，排名前九的图像编辑模型中有七个能根据简单提示轻易为女性“脱衣”。 该报告突显了主要 AI 平台上的关键安全漏洞，引发了关于内容审核、法律责任以及采取提示词过滤和输出扫描等措施以防止伤害（尤其是对未成年人）的紧迫问题。 研究人员设置了一个蜜罐，在 7 天内收到超过 1000 条请求，其中 73%为涉性内容，近 7%针对儿童，尽管 Hugging Face 的政策禁止非自愿性内容和儿童裸露。

telegram · zaihuapd · Jul 29, 08:20

**背景**: Hugging Face 是一个流行的开源平台，开发者在此分享机器学习模型和数据集，包括图像生成模型。深度伪造利用 AI 创建逼真但虚假的图像或视频，通常未经同意。该报告强调，如果没有适当的防护措施，此类平台可能被滥用于有害目的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Hugging_Face">Hugging Face</a></li>
<li><a href="https://www.ibm.com/think/topics/hugging-face">What is Hugging Face? - IBM</a></li>

</ul>
</details>

**标签**: `#AI ethics`, `#deepfake`, `#content moderation`, `#Hugging Face`, `#safety`

---