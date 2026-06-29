---
layout: default
title: "Horizon Summary: 2026-06-29 (ZH)"
date: 2026-06-29
lang: zh
---

> From 25 items, 5 important content pieces were selected

---

1. [GLM 5.2 在网络安全基准测试中超越 Claude](#item-1) ⭐️ 8.0/10
2. [用 Claude Code 获取 MRI 第二意见](#item-2) ⭐️ 8.0/10
3. [布朗大学教授揭露大规模 AI 作弊事件](#item-3) ⭐️ 8.0/10
4. [KIDS 法案要求在线年龄验证](#item-4) ⭐️ 8.0/10
5. [谷歌因算力短缺限制 Meta 使用 Gemini AI](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [GLM 5.2 在网络安全基准测试中超越 Claude](https://semgrep.dev/blog/2026/we-have-mythos-at-home-glm-52-beats-claude-in-our-cyber-benchmarks/) ⭐️ 8.0/10

据报道，拥有 7530 亿参数的开源大语言模型 GLM 5.2 在 Semgrep 进行的网络安全基准测试中超越了 Claude，每发现一个漏洞的成本约为 0.17 美元，而 Claude Code 为 0.32 美元。 这挑战了闭源模型在专业领域的主导地位，并突显了开源模型的快速进步，特别是在安全任务方面，GLM 5.2 以更低的成本展现出强劲性能。 尽管基准测试结果令人印象深刻，但一些社区成员指出，GLM 5.2 的 7530 亿参数需要强大的硬件才能本地部署，而且与“Claude”的比较混淆了 Claude Code（一个代理工具）与底层大语言模型。

hackernews · jms703 · Jun 28, 17:50 · [社区讨论](https://news.ycombinator.com/item?id=48709670)

**背景**: GLM（通用语言模型）是由智谱 AI 开发的一系列大语言模型，GLM 5.2 是其最新的开源版本，针对长周期任务进行了优化，并拥有 100 万 token 的上下文窗口。网络安全基准测试评估大语言模型在漏洞检测和代码分析等任务上的表现，Semgrep 的测试专门衡量模型发现其工具 Mythos 通常能发现的漏洞的能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openlm.ai/glm-5.2/">GLM-5.2 - openlm.ai</a></li>
<li><a href="https://z.ai/blog/glm-5.2">GLM-5.2: Built for Long-Horizon Tasks - z.ai</a></li>
<li><a href="https://www.hackthebox.com/blog/ai-range-llm-security-benchmark">Benchmarking LLMs for cybersecurity: Inside HTB AI Range’s first evaluation</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：一些用户称赞 GLM 5.2 在日常编程中的实用性和成本效益，而另一些人则质疑将开源模型与专有代理产品进行比较的有效性，并指出其他模型基准测试的不一致性。巨大的参数量也引发了对本地推理硬件要求的实际担忧。

**标签**: `#AI/ML`, `#LLM`, `#benchmark`, `#model comparison`, `#open source`

---

<a id="item-2"></a>
## [用 Claude Code 获取 MRI 第二意见](https://antoine.fi/mri-analysis-using-claude-code-opus) ⭐️ 8.0/10

一位用户借助 Anthropic 的 Claude Code（一款 AI 编码辅助工具）分析了自己的肩部 MRI 扫描结果，以此获得第二意见，并将这一过程记录并发布到网上。 这一案例展示了一种新颖却充满争议的通用 AI 在个人医疗中的应用，引发了关于信任、可靠性以及 AI 在医疗决策中适当角色的讨论。 该分析仅基于一张二维 MRI 切片，而非完整的三维数据集，一位放射科医生指出这不足以进行全面评估。

hackernews · engmarketer · Jun 28, 16:35 · [社区讨论](https://news.ycombinator.com/item?id=48708941)

**背景**: Claude Code 是 Anthropic 推出的一款智能编码工具，它能理解代码库并自动化开发任务，但并非为医疗用途设计或认证。虽然已有专门的 AI 工具用于 MRI 解读，但这些工具同样需要验证，并不能取代专业的医疗判断。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>
<li><a href="https://mriagi.com/">MRIAGI – AI-Powered MRI Scan Interpretation in Seconds</a></li>

</ul>
</details>

**社区讨论**: 一位放射科医生评论称，正确评估需要完整的三维数据集；其他用户则分享了误诊的个人经历，并讨论了 AI 的便利性与对值得信赖的专业医疗需求之间的张力。

**标签**: `#AI`, `#healthcare`, `#LLM`, `#trust`, `#MRI`

---

<a id="item-3"></a>
## [布朗大学教授揭露大规模 AI 作弊事件](https://english.elpais.com/education/2026-06-28/ai-fraud-at-brown-university-academic-integrity-is-at-risk.html) ⭐️ 8.0/10

布朗大学的一位教授公开报告称，学生在考试中广泛使用 AI，严重违反学术诚信。 此事件引发关于大学应如何调整评估方法的迫切讨论，可能推动改为现场手写考试等变革。 教授的揭露在网上引起高度关注，超过 400 条评论讨论了对抗性课程设计和口头面试等解决方案。

hackernews · geox · Jun 28, 16:41 · [社区讨论](https://news.ycombinator.com/item?id=48708991)

**背景**: 像 ChatGPT 这样的生成式 AI 工具可以完成许多学术任务，引发了广泛的作弊担忧。传统的开卷考试尤其容易受到冲击，促使教育工作者重新考虑考试形式。

**社区讨论**: 评论者分享了不同见解：一位教授主张现场手写考试，另一位将课程设计视为对抗性问题，还有一位质疑评分制度本身的价值。有人指出学生使用 AI 的博弈论激励。

**标签**: `#AI ethics`, `#academic integrity`, `#education`, `#AI fraud`, `#cheating`

---

<a id="item-4"></a>
## [KIDS 法案要求在线年龄验证](https://www.eff.org/deeplinks/2026/06/kids-act-would-require-age-checks-get-online) ⭐️ 8.0/10

美国众议院两党达成协议的《儿童互联网安全法案》（KIDS Act）将要求所有用户在受覆盖的在线平台上进行年龄验证，可能需向第三方提供政府颁发的身份证件。 这项立法可能从根本上重塑网络隐私和言论自由，迫使成年人为访问网站而交出个人信息，批评者警告称这可能导致监控和审查。 KIDS 法案放弃了 KOSA 的注意义务，但增加了对所有用户的强制性年龄验证；受覆盖的平台包括那些使用个人数据进行广告或内容推荐的平台，但像 Hacker News 这样的简单讨论网站可能被豁免。

hackernews · bilsbie · Jun 28, 11:56 · [社区讨论](https://news.ycombinator.com/item?id=48706560)

**背景**: 年龄验证技术包括政府身份证检查、面部识别等，但都存在隐私、安全和有效性问题。KIDS 法案是保护未成年人在线安全的更广泛努力的一部分，但批评者认为它侵犯了成年人的权利，且未能解决伤害的根本原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eff.org/deeplinks/2026/06/kids-act-would-require-age-checks-get-online">The KIDS Act Would Require Age Checks To Get Online</a></li>
<li><a href="https://www.politico.com/live-updates/2026/06/22/congress/guthrie-and-pallone-cement-deal-for-kids-online-safety-package-00969686">Lawmakers cement bipartisan deal for kids online safety package</a></li>
<li><a href="https://www.techtimes.com/articles/318896/20260623/house-kids-act-deal-drops-kosa-duty-care-adds-age-verification-all-users.htm">House KIDS Act Deal Drops KOSA Duty of Care, Adds Age Verification for ...</a></li>

</ul>
</details>

**社区讨论**: 评论者质疑社交媒体与心理健康之间关联的证据，指出一项纵向研究发现影响很小，并指出了游说关系（例如 Alphabet 公司）。其他人则强调了在多年建议不要在线分享个人信息后，现在却要求提供个人信息的讽刺之处。

**标签**: `#privacy`, `#age verification`, `#internet regulation`, `#policy`, `#EFF`

---

<a id="item-5"></a>
## [谷歌因算力短缺限制 Meta 使用 Gemini AI](https://www.ft.com/content/c5d52f72-71ef-40bc-bad3-61afdba8b378) ⭐️ 8.0/10

谷歌于 2026 年 3 月告知 Meta，无法提供其请求的全部 Gemini AI 算力，该限制至今有效，已导致 Meta 部分内部 AI 项目延迟。 这表明 AI 算力瓶颈已影响甚至大型科技公司，可能减缓 AI 发展，并加剧对云和基础设施资源的竞争。 Meta 已采取应对措施，鼓励员工更高效地使用 tokens，并加速自研模型 Muse Spark 的开发，该模型由其 Meta 超级智能实验室近期推出。

telegram · zaihuapd · Jun 28, 07:38

**背景**: 在生成式 AI 中，token 是模型处理的文本单元（如词或子词），token 限制约束输入长度和计算成本。Muse Spark 是 Meta 新推出的多模态 AI 模型，具备强大的推理和编码能力，旨在减少对 Gemini 等外部模型的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.novelvista.com/blogs/ai-and-ml/understanding-tokens-in-generative-ai">What is a Token in Generative AI ? | Understanding Tokens</a></li>
<li><a href="https://www.theguardian.com/technology/2026/apr/09/meta-first-ai-model-muse-sparks">Meta debuts new AI model in first test of costly... | The Guardian</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#compute shortage`, `#Google`, `#Meta`, `#Gemini`

---