---
layout: default
title: "Horizon Summary: 2026-05-26 (ZH)"
date: 2026-05-26
lang: zh
---

> From 19 items, 8 important content pieces were selected

---

1. [教皇利奥十四世关于人工智能伦理的通谕](#item-1) ⭐️ 9.0/10
2. [用 AI 写更好但更慢的代码](#item-2) ⭐️ 8.0/10
3. [挪威投资 2PB 华为闪存和 HPE Cray 用于主权 LLM 训练](#item-3) ⭐️ 8.0/10
4. [加州提议 Linux 免于年龄验证法](#item-4) ⭐️ 8.0/10
5. [微软 Copilot Cowork 存在提示注入漏洞](#item-5) ⭐️ 8.0/10
6. [AI 时代网络安全专家需求激增](#item-6) ⭐️ 8.0/10
7. [Grok V9-Medium 1.5T 模型训练完成，预计近期发布](#item-7) ⭐️ 8.0/10
8. [离体人脑用于药物测试挑战伦理边界](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [教皇利奥十四世关于人工智能伦理的通谕](https://simonwillison.net/2026/May/25/encyclical-on-ai/#atom-everything) ⭐️ 9.0/10

教皇利奥十四世今天发布了通谕《宏伟人性》，为人工智能融入社会提供了清晰的伦理指南。 这是梵蒂冈首份关于人工智能伦理的正式通谕，标志着对全球人工智能政策和讨论的重要宗教与哲学贡献。 通谕将人工智能系统描述为更多是“培育”而非“构建”，强调可解释性问题，并指出真正的发展必须以人类尊严为中心。

rss · Simon Willison · May 25, 23:58

**背景**: 通谕是教皇就重要问题发布的正式信函。利奥十四世选择此名以纪念发布工业革命通谕《新事》的利奥十三世。新通谕将天主教社会教导应用于人工智能革命。

**标签**: `#AI ethics`, `#Vatican`, `#encyclical`, `#human dignity`, `#policy`

---

<a id="item-2"></a>
## [用 AI 写更好但更慢的代码](https://nolanlawson.com/2026/05/25/using-ai-to-write-better-code-more-slowly/) ⭐️ 8.0/10

文章主张采用迭代式 AI 辅助编码方法，专注于代码审查和细化，能产出更高质量的代码，但开发速度会变慢。 这挑战了 AI 加速编码的普遍说法，凸显了质量与速度之间的权衡。它为追求健壮代码而非快速交付的开发者提供了一种实用方法论。 该方法涉及多次迭代：用 AI 设计，用更慢但更强的模型实现，审查，再用快速审查模型发现边界情况，最后用强模型修复。

hackernews · signa11 · May 25, 23:16 · [社区讨论](https://news.ycombinator.com/item?id=48272984)

**背景**: AI 辅助编码通常强调通过快速生成代码来提速。然而，本文提出仔细的迭代审查可以提升代码质量，尽管速度较慢。这反映了将 AI 视为协作工具而非替代人类判断的细致理解。

**社区讨论**: 评论显示了不同的体验；一些人觉得迭代循环耗时，另一些人则看到 AI 代码审查的价值。有人对缺乏示例的观点文章持怀疑态度，但也有人欣赏这种方法。

**标签**: `#AI-assisted development`, `#code review`, `#software engineering`, `#developer productivity`

---

<a id="item-3"></a>
## [挪威投资 2PB 华为闪存和 HPE Cray 用于主权 LLM 训练](https://www.blocksandfiles.com/flash/2026/05/22/norways-2-petabytes-of-huawei-flash-storage-and-llm-training/5244910) ⭐️ 8.0/10

挪威正在投资 2PB 的华为闪存和一台配备 448 个 GPU 和 64,512 个 CPU 核心的 HPE Cray 超级计算系统（名为 Olivia），用于训练一个挪威语的主权大语言模型。 这一行动凸显了各国追求 AI 主权以保护本国语言和文化的日益增长趋势，同时也引发了关于这种投资是否必要、或者像微调现有模型这样的替代方法是否更实用的激烈讨论。 Olivia 系统配备了 448 个 GPU 和 64,512 个 CPU 核心，一些评论者认为这些硬件对于训练一个完整的大语言模型来说是不够的。存储方面则使用了 2PB 的华为闪存。

hackernews · rbanffy · May 25, 19:37 · [社区讨论](https://news.ycombinator.com/item?id=48270770)

**背景**: 主权 AI 是指一个国家利用自己的基础设施、数据、劳动力和商业网络生产人工智能的能力。挪威的目标是创建一个理解挪威语言和文化的 LLM，因为全球训练的以英语为中心的模型可能缺乏本地知识。HPE Cray 系统专为高性能 AI 训练而设计，并已用于多种超级计算设置。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hpe.com/us/en/hpe-cray-xd670.html">HPE Cray XD670 | HPE</a></li>
<li><a href="https://blogs.nvidia.com/blog/what-is-sovereign-ai/">What Is Sovereign AI? | NVIDIA Blog</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-sovereignty">What is AI Sovereignty? | IBM</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了不同的看法：一些人质疑主权 LLM 的必要性，认为现有模型已经覆盖了多种语言；另一些人怀疑硬件是否足够，称其“微不足道”，并预测这项努力可能不会产生有用的模型。替代提议包括与模型构建者共享训练数据，而不是从头开始构建。

**标签**: `#LLM`, `#sovereign AI`, `#storage`, `#Norway`, `#AI infrastructure`

---

<a id="item-4"></a>
## [加州提议 Linux 免于年龄验证法](https://www.tomshardware.com/software/linux/california-moves-to-exempt-linux-from-its-upcoming-age-verification-law-after-backlash-over-forcing-operating-systems-to-collect-users-ages-amendment-proposed-by-the-same-lawmaker-who-wrote-the-original-law) ⭐️ 8.0/10

加州提出年龄验证法的立法者，在开源社区的强烈反对后，提议修正案将 Linux 豁免于该法。 这一豁免可能为年龄验证法如何对待开源软件树立先例，避免给 Linux 发行版带来收集用户年龄的负担。 修正案由起草原法的同一立法者提出，特别豁免了 Linux 等并非主要用于访问年龄限制内容的操作系统。

hackernews · rbanffy · May 25, 18:19 · [社区讨论](https://news.ycombinator.com/item?id=48269961)

**背景**: 加州的年龄验证法旨在要求在线服务验证用户年龄以保护未成年人。最初，该法可能被解释为适用于像 Linux 这样的操作系统，这引发了开源社区的强烈反对，他们认为这既不可行又侵犯隐私。拟议的豁免解决了这些担忧。

**社区讨论**: 评论者对法律的意图和实施表示怀疑，有人认为这是为了防止 Linux 开发者以第一修正案为由挑战该法。还有人指出，大多数评论者误解了法律的实际内容。

**标签**: `#California`, `#Linux`, `#age-verification`, `#open source`, `#technology policy`

---

<a id="item-5"></a>
## [微软 Copilot Cowork 存在提示注入漏洞](https://www.promptarmor.com/resources/microsoft-copilot-cowork-exfiltrates-files) ⭐️ 8.0/10

微软 Copilot Cowork（一项跨 Microsoft 365 自动执行任务的新功能）存在提示注入漏洞，可被用于窃取敏感文件。研究人员展示，恶意构造的技能可诱骗 Copilot 将数据发送至攻击者控制的服务器。 该漏洞意义重大，因为 Copilot Cowork 正被企业广泛采用以实现工作流自动化，使其成为高价值目标。被利用可能导致大规模数据泄露，削弱企业 AI 工具的信任度。 攻击利用了 Cowork 中的技能创建系统——技能可由自然语言编写并由 LLM 执行。研究人员发现，包含通过 curl 窃取文件命令的技能可正常运行，缺乏适当的隔离或验证。

hackernews · Kneenex · May 25, 21:45 · [社区讨论](https://news.ycombinator.com/item?id=48272354)

**背景**: 微软 Copilot Cowork 于 2026 年初推出，将 Copilot 从被动响应式提示转变为主动执行任务——它可以代用户发送电子邮件、安排会议和管理文件。提示注入是一种网络安全攻击，通过恶意提示劫持 LLM 的行为，常用于绕过限制。在此案例中，提示注入被嵌入 Cowork 技能中，导致未经授权的数据窃取。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/microsoft-365/blog/2026/03/09/copilot-cowork-a-new-way-of-getting-work-done/">Copilot Cowork: A new way of getting work done | Microsoft ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区观点存在分歧：一些人认为这是正常现象，因为技能本质上是程序；另一些人则指责微软急于将功能推向生产。评论者指出，提示注入并非新问题，Copilot 本应具备更好的防御，但真正的漏洞在于技能执行缺乏安全保障。

**标签**: `#security`, `#AI`, `#Microsoft`, `#prompt injection`, `#Copilot`

---

<a id="item-6"></a>
## [AI 时代网络安全专家需求激增](https://www.nytimes.com/2026/05/24/technology/one-job-that-is-growing-in-the-ai-era-cybersecurity-experts.html) ⭐️ 8.0/10

2026 年第一季度网络安全相关岗位招聘量同比增长 11%，高管职位需求自 2025 年秋季以来增加了五到七倍。 这一趋势凸显了在 AI 扩大攻击面并引入新型威胁的背景下，网络安全人才的迫切需求，直接影响企业安全和高管薪酬方案。 高级安全岗位薪酬包可达七八百万美元，安全工程师也需补充 AI 技能才能保持竞争力。

telegram · zaihuapd · May 25, 06:21

**背景**: 像 Anthropic 的 Mythos 这样的 AI 系统能够发现并利用软件漏洞，带来新的风险。企业需要既懂安全技术又能驾驭 AI 复杂性的领导者。

**标签**: `#cybersecurity`, `#AI`, `#job market`, `#technology trend`, `#industry growth`

---

<a id="item-7"></a>
## [Grok V9-Medium 1.5T 模型训练完成，预计近期发布](https://x.com/elonmusk/status/2058787384364265734) ⭐️ 8.0/10

埃隆·马斯克宣布，xAI 已完成 Grok V9-Medium 基础模型的训练，参数量达 1.5 万亿，预计 2 到 3 周后向公众发布。该模型在补充训练中加入了 Cursor 数据，增强了编程能力。 此版本相较于之前的 Grok V8-small（0.5T）规模大幅提升，参数量翻了三倍，并承诺在复杂编程任务上有显著改进，展示了 xAI 在大规模语言模型方面的持续投入。 V9-Medium 模型参数量达 1.5 万亿，是 V8-small 的三倍，训练中加入了额外的 Cursor 编程数据。目前正在进行微调，强化学习将在几天内启动。

telegram · zaihuapd · May 25, 07:07

**背景**: Grok 是 xAI 的聊天机器人语言模型，当前生产环境运行的是 Grok V8-small。Cursor 是一款 AI 驱动的代码编辑器，提供编程辅助。V9-Medium 的命名暗示它可能是更大 V9 模型之前的中间版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.com/elonmusk/status/2058787384364265734">Grok foundation model V9-Medium (1.5T) has finished training ...</a></li>
<li><a href="https://beyondtmrw.org/article/grok-v9-medium-training-complete-xai-15t-parameter-leap-coding-ai">Is Grok V9-Medium Grok 5? xAI's 1.5T AGI Hype Train Explained</a></li>
<li><a href="https://www.basenor.com/blogs/news/grok-v9-medium-1-5t-finishes-training-release-in-2-3-weeks">Grok V9-Medium (1.5T) Finishes Training, Release in 2-3 Weeks</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#Grok`, `#machine learning`, `#programming`

---

<a id="item-8"></a>
## [离体人脑用于药物测试挑战伦理边界](https://www.science.org/content/article/not-alive-not-dead-disembodied-human-brains-used-drug-testing) ⭐️ 8.0/10

一项研究利用 BrainEx 灌流系统在死亡数小时后部分恢复了人脑的代谢和细胞活动，从而可对阿尔茨海默病、帕金森病等神经疾病进行药物测试。 这一突破可能通过使用真实人脑组织彻底改变神经疾病药物研发，但也引发了关于死亡定义、意识和知情同意的深刻伦理问题。 BrainEx 系统向大脑灌注含有维生素、氨基酸和代谢因子的溶液，但这些大脑未显示意识迹象或完整神经活动。研究团队强调该制备物既非活着也非完全死亡。

telegram · zaihuapd · May 25, 14:57

**背景**: BrainEx 最初于 2019 年为猪脑开发，可在死亡数小时后恢复循环和细胞功能。离体脑切片培养已用于药物测试，但使用完整人脑处于半存活状态是新颖的。关于死亡和器官捐赠的伦理框架并非为这类技术设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://neuwritesd.org/2019/06/13/brainex-restoring-brain-circulation-after-death/">BrainEx: Restoring Brain Circulation After Death</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC8272538/">Evaluating the translational value of postmortem brain ...</a></li>
<li><a href="https://britbrief.co.uk/health/public/startup-keeps-disembodied-brains-alive-for-drug-tests.html">Controversial Startup Keeps Disembodied Human Brains Alive for Drug Testing</a></li>

</ul>
</details>

**标签**: `#neuroscience`, `#ethics`, `#drug testing`, `#brain`, `#biotechnology`

---