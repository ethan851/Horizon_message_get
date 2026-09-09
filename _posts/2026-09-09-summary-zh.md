---
layout: default
title: "Horizon Summary: 2026-09-09 (ZH)"
date: 2026-09-09
lang: zh
---

> From 34 items, 8 important content pieces were selected

---

1. [OpenAI 称 AI 破解纳维-斯托克斯难题，却遭剽窃指控](#item-1) ⭐️ 10.0/10
2. [AlphaGenome Atlas：绘制整个人类基因组 DNA 单字母变化的效应图谱](#item-2) ⭐️ 9.0/10
3. [Meta 发布个人 AI 智能体 Muse，主打快速响应与分层安全防护](#item-3) ⭐️ 8.0/10
4. [陶哲轩：AI 正不可再生地消耗开放数学问题](#item-4) ⭐️ 8.0/10
5. [OpenAI 发布 ChatGPT Images 2.5：新增 Sunburst 与 Flare API 模型](#item-5) ⭐️ 8.0/10
6. [中国计划到 2030 年将智能算力提升至 9800 EFLOPS](#item-6) ⭐️ 8.0/10
7. [OpenAI 发布 ChatGPT Images 2.0，强化文本渲染与推理能力](#item-7) ⭐️ 8.0/10
8. [美国指控六家中国 AI 公司借蒸馏技术盗用美方技术](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI 称 AI 破解纳维-斯托克斯难题，却遭剽窃指控](https://simonwillison.net/2026/Sep/8/on-navier-stokes/) ⭐️ 10.0/10

OpenAI 于 2026 年 9 月 8 日宣布，其未公开的内部模型给出了纳维-斯托克斯存在性与光滑性问题的解答，该问题是七个千禧年大奖难题之一。该结果尚未得到外部数学家或克莱数学研究所的验证，并因与纽约大学教授 Tristan Buckmaster 和 Anthropic 数学家 Levent Alpöge 的优先权争议而蒙上阴影。 若经证实，这将是 AI 系统首次解决千禧年大奖难题，可能彻底改变数学发现的方式。这场争议同时引发了对商业情报、数据隐私及 AI 驱动研究伦理的严峻拷问。 OpenAI 表示，其智能体在项目启动约 88 小时后得到该结果，针对纳维-斯托克斯问题约使用了 1300 亿个输出 token，随后又用 GPT-6 Astra 花了 17 小时完成 Lean 形式化验证。Buckmaster 和 Alpöge 已在 8 月 15 日取得相关突破；Buckmaster 指控 OpenAI 在得知他们的工作后才启动类似研究，而 OpenAI 承认它“不能排除”去标识化用户数据帮助改进了其模型。

rss · Simon Willison · Sep 8, 23:55

**背景**: 纳维-斯托克斯方程描述流体的运动，而三维空间中光滑解是否总是存在这一问题，是克莱数学研究所自 2000 年起悬赏一百万美元的七个千禧年大奖难题之一。至今唯一被正式解决的是庞加莱猜想，由格里戈里·佩雷尔曼证明，但他拒绝了奖金。OpenAI 宣布的结果是一个展示光滑性破裂的反例，方法基于 Diego Cordoba 与 Luis Martinez Zoroa 在 2023 年提出的思路，但该结果仍有待克莱数学研究所和数学界的独立验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier–Stokes_existence_and_smoothness_problem">Navier–Stokes existence and smoothness problem</a></li>
<li><a href="https://en.wikipedia.org/wiki/Millennium_Prize_Problems">Millennium Prize Problems</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍强烈批评 OpenAI，有用户指责其查看用户数据、窃取顶尖研究者的成果并试图恫吓对方。也有人指出 OpenAI 自己承认数据泄漏“无法排除”，另一些人则把此事视为 AI 催化下由来已久的学术优先权争夺战。

**标签**: `#AI`, `#mathematics`, `#OpenAI`, `#Navier-Stokes`, `#Millennium Prize Problems`

---

<a id="item-2"></a>
## [AlphaGenome Atlas：绘制整个人类基因组 DNA 单字母变化的效应图谱](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/) ⭐️ 9.0/10

谷歌 DeepMind 发布了 AlphaGenome Atlas，这是一个公开数据库，预测人类基因组中所有约 90 亿个可能的单核苷酸变异的功能影响。这些预测由 AlphaGenome AI 模型预先计算，而非通过实验逐一测定。 这是首个覆盖人类 DNA 中每一个单字母变化的综合性预测图谱，使研究从参考基因组转向变异效应。研究疾病变异、调控基因组学和个体化医疗的科研人员，可以用它来筛选哪些突变最可能具有功能影响。 该图谱涵盖编码区和非编码 DNA，并为每个变异给出估计其分子效应的 AVI 评分。用户可通过交互式网络门户自由访问，无需填写所属机构。

hackernews · utiiiD · Sep 8, 14:55 · [社区讨论](https://news.ycombinator.com/item?id=49611251)

**背景**: 人类基因组由约 30 亿个 DNA 字母组成；其中单个字母的变化即单核苷酸变异，可能改变基因调控或蛋白质功能，并与疾病相关。解读这些变异非常困难，因为大多数变异位于功能尚不明确的非编码区域。AlphaGenome 是一个深度学习模型，通过学到的 DNA 序列与染色质、基因表达等分子特征之间的关系，能够在全基因组范围内对未见过的变异进行评分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/">AlphaGenome Atlas: a high-resolution map of human DNA</a></li>
<li><a href="https://deepmind.google/blog/alphagenome-atlas-a-predictive-map-of-every-possible-dna-letter-change-in-the-human-genome/">AlphaGenome Atlas: Molecular predictions for 9 Billion human DNA variants — Google DeepMind</a></li>

</ul>
</details>

**社区讨论**: 评论者大多对实际应用和覆盖范围感到好奇：有人询问是否包含启动子等调控区域，以及能否用 23andMe 等个人基因组数据筛查致病突变。也有人分享了教程视频，并指出访问 Atlas 无需填写所属机构。还有评论者链接了一项外部实验研究——该研究对病毒基因组进行穷举式突变，作为补充 AlphaGenome 预测的现实基准。

**标签**: `#AI`, `#Genomics`, `#DeepMind`, `#Biology`, `#DNA`

---

<a id="item-3"></a>
## [Meta 发布个人 AI 智能体 Muse，主打快速响应与分层安全防护](https://ai.meta.com/muse/) ⭐️ 8.0/10

Meta 在 ai.meta.com/muse 发布了个人 AI 智能体 Muse，主打快速响应和对提示注入攻击的分层防御。Meta AI 的 David Singleton 还公开了其安全架构的技术细节。 Muse 标志着 Meta 开始大力吸引主流、非专家的 AI 用户，与 ChatGPT 等消费级助手展开直接竞争。Meta 如何在安全与数据隐私方面做出平衡，将影响用户对管理个人信息的 AI 智能体的信任程度。 其安全策略采用多层防御：模型经过训练以识别并抵抗提示注入，系统框架会标记来自不可信来源的内容，确定性代码对结果进行校验，一组集成分类器在智能体无法触达的层面运行。尽管有这些安全声明，评论区仍对 Meta 处理个人数据的方式以及该产品是否真正解决消费者需求表示怀疑。

hackernews · yks · Sep 8, 19:25 · [社区讨论](https://news.ycombinator.com/item?id=49615537)

**背景**: 提示注入（prompt injection）是一种网络安全攻击，利用了大语言模型难以区分开发者指令、用户输入以及网页或文件等不可信内容的特点。对于能够浏览网页或读取文件的 AI 智能体，嵌入在网站内容中的间接提示注入可能引发非预期行为。像 Muse 这样的个人智能体会成为数据的核心入口，因此分层防御对保护用户至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection | OWASP Foundation</a></li>

</ul>
</details>

**社区讨论**: 社区反应褒贬不一：有人认为 Muse 是 Meta 争夺主流 AI 用户的举措，并称赞其响应速度是一大亮点；也有开发者重点介绍了分层的提示注入防御机制。另一些人则对 Meta 的数据隐私承诺表示强烈不信任，认为该产品属于“没人想要”的类型，并指出消费级 AI 往往试图解决人们原本就能轻松应付的问题。

**标签**: `#AI`, `#Meta`, `#Personal Assistant`, `#Security`, `#Product Launch`

---

<a id="item-4"></a>
## [陶哲轩：AI 正不可再生地消耗开放数学问题](https://mathstodon.xyz/@tao/117237320796901560) ⭐️ 8.0/10

陶哲轩在 Mathstodon 上指出，开放数学问题正被 AI 以“不可再生”的方式消耗：机器可能在解决它们时并没有带来新的人类洞见。他还表示，识别出一个有前景的问题如今才是稀缺而宝贵的资源。 作为世界顶尖数学家之一，陶哲轩的这一观点重新定义了 AI 在数学中的角色：进步的瓶颈可能不再是解题能力，而是提出有意义问题的能力。这可能改变数学人才、奖项以及 AI 研究资源的配置方向。 陶哲轩并不是在描述某个具体猜想被某个 AI 系统解决，而是在指出一种结构性后果。即使 AI 给出经过符号验证的答案，数学研究的目标仍是理解；一个没有带来洞见的“已解决问题”只会让一个有趣的课题永久地从领域中消失。

hackernews · _alternator_ · Sep 8, 21:00 · [社区讨论](https://news.ycombinator.com/item?id=49616968)

**背景**: 陶哲轩是菲尔兹奖得主、著名数学家，常在 Mathstodon 等平台上发表关于数学与 AI 的看法。所谓“开放数学问题”是指尚未被解决、吸引许多研究者投入的问题，例如黎曼猜想或纳维-斯托克斯正则性问题。传统数学文化不仅看重正确答案，也看重证明过程带来的新概念和新洞见。随着具备符号推理能力的 AI 系统越来越强，探讨“机器解题”到底意味着什么已经成为一个现实议题。

**社区讨论**: 评论者大多没有简单附和陶哲轩。有人引用阿西莫夫笔下 Multivac 的故事，认为提出正确问题才是真正的瓶颈；也有人调侃称要去算 π 的第 10^10^10 位来载入史册。还有评论者反对“机器解决了问题就会阻碍人类知识”的看法，指出无法被理解的证明只会显得无趣；也有人惊讶开放问题竟是有限资源，并提出 AI 的下一个前沿应该是提出好问题，并可以为此设立奖项。

**标签**: `#AI`, `#mathematics`, `#research`, `#Terence Tao`, `#open problems`

---

<a id="item-5"></a>
## [OpenAI 发布 ChatGPT Images 2.5：新增 Sunburst 与 Flare API 模型](https://simonwillison.net/2026/Sep/8/introducing-chatgpt-images-25/) ⭐️ 8.0/10

OpenAI 于 2026 年 9 月 8 日发布 ChatGPT Images 2.5，称其图像模型已在 ChatGPT 与 API 中生成超过 30 亿张图像。新版本提升了多轮指令遵循能力、对参考照片中主体的保留效果并加快响应速度，同时推出两个新 API 模型 ID：gpt-image-2.5-sunburst 和 gpt-image-2.5-flare。 此次发布巩固了 OpenAI 在 AI 图像生成领域的地位，而多轮编辑与主体一致性正成为该领域越来越关键的需求。开发者与创意工作者如今同时拥有面向日常快速生成的 Flare 和面向精细编辑的 Sunburst，使通过 API 进行高质量迭代修图更加实用。 根据 OpenAI 的说明，Sunburst 面向编辑精度优先的工作流，Flare 面向快速、高质量的日常图像生成。API 更新还支持传入一张或多张参考图片，Simon Willison 更新后的 openai_image.py 命令行工具即演示了文本提示与输入图片结合使用的用法。

rss · Simon Willison · Sep 8, 22:46

**背景**: ChatGPT Images 是 OpenAI 的文生图系统，可通过 ChatGPT 聊天界面以及 API 中的 GPT-Image 模型使用。图像生成模型能够根据文本提示生成图像，并能通过指令编辑已有图片；该领域的一个主要难点是多轮编辑——用户逐轮调整图片时，模型既要理解新的指令，又要保持画面风格与主体身份的一致性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.kanaries.net/articles/gpt-image-2-5">GPT Image 2.5: How to Use It, Flare vs Sunburst, and API ...</a></li>
<li><a href="https://www.callmissed.com/blog/gpt-image-flare-vs-sunburst-key-differences">GPT Image 2.5 Flare vs Sunburst: Key Differences | CallMissed</a></li>
<li><a href="https://www.orcarouter.ai/blog/gpt-image-2-5-flare-sunburst">GPT-Image-2.5 Flare vs Sunburst: New OpenAI Image APIs</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Image Generation`, `#API`, `#AI Models`

---

<a id="item-6"></a>
## [中国计划到 2030 年将智能算力提升至 9800 EFLOPS](https://www.scmp.com/tech/policy/article/3366733/china-targets-fourfold-boost-ai-computing-capacity-2030-major-tech-push) ⭐️ 8.0/10

工信部发布未来五年产业规划，提出到 2030 年将中国智能算力规模提升至 9800 EFLOPS。规划提出 2026 年至 2030 年累计投入 3.8 万亿元用于信息基础设施建设，并有序部署万卡级及 10 万卡以上的智能计算集群。 该政策是官方推动中国 AI 算力规模扩大约四倍的重要举措，可能重塑全球 AI 基础设施的竞争格局。如此大规模的投资与集群部署计划可能影响 AI 硬件供应链，并加速国产 AI 芯片的采用。 截至今年 6 月底，中国智能算力已达到 2185 EFLOPS，同比增长 177%，这意味着要实现 2030 年目标，算力规模需在此基础上增长至 4 倍以上。规划还强调加强基础设施与国产算力芯片的适配，反映出降低对进口加速器依赖的政策方向。

telegram · zaihuapd · Sep 8, 11:23

**背景**: EFLOPS（ExaFLOPS）是衡量计算性能的单位，代表每秒可执行百亿亿（10^18）次浮点运算，AI 领域常使用 FP16 等较低精度格式来衡量。智能算力特指为 AI 任务优化的计算能力。万卡级或 10 万卡级的大规模 AI 集群通过高速网络将数千甚至数万颗 AI 加速芯片连接起来，以更高效地训练大模型。这一概念已成为所谓全球“智能基础设施”竞赛的核心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Floating_point_operations_per_second">Floating point operations per second - Wikipedia</a></li>
<li><a href="https://baike.baidu.com/en/item/EFLOPS/3608460">EFLOPS（A performance unit used to measure the scale of ...</a></li>
<li><a href="https://www.scmp.com/tech/big-tech/article/3352200/supersized-and-scaling-china-pushes-10000-card-computing-clusters-ai-race">Supersized and scaling: China pushes 10,000-card computing clusters in AI race | South China Morning Post</a></li>

</ul>
</details>

**标签**: `#China Tech Policy`, `#AI Infrastructure`, `#Computing Power`, `#EFLOPS`, `#State Investment`

---

<a id="item-7"></a>
## [OpenAI 发布 ChatGPT Images 2.0，强化文本渲染与推理能力](https://t.me/zaihuapd/43693) ⭐️ 8.0/10

OpenAI 于 2026 年 4 月推出基于 GPT Image 2 的 ChatGPT Images 2.0 图像生成模型。该模型首次引入推理能力，可进行联网搜索与结果验证，并能根据单一提示词生成最多 8 张视觉一致的图像。 这标志着 AI 图像生成的一次“阶梯式变革”：模型现在能够推理、搜索网络，并可靠地渲染密集文本，解决了此前文字乱码和复杂构图等长期短板。这将使 AI 生成图像在营销素材、漫画和 UI 设计等实际任务中更加实用。 新模型提升了中文、日语、韩语、印地语和孟加拉语等非拉丁文字脚本的渲染能力，并支持生成多格漫画、UI 元素和营销素材，最高分辨率为 2K。OpenAI 表示，该系统在遵循详细指令、渲染密集文本以及场景中物体的放置与关联方面实现了重大进步。

telegram · zaihuapd · Sep 8, 18:45

**背景**: ChatGPT Images 是 OpenAI 在 ChatGPT 中提供的图像生成功能，基于 GPT Image 系列模型。以往的图像生成模型难以正确渲染文字，尤其是非拉丁语系文字，也无法对提示词进行逻辑推理来验证视觉输出。新版模型新增了可对结果进行核查与验证的推理能力，从而提升了准确性与视觉一致性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.engadget.com/ai/chatgpt-images-20-is-better-at-rendering-non-latin-text-190000153.html">ChatGPT Images 2.0 is better at rendering non-Latin text - Engadget</a></li>
<li><a href="https://www.socialsamosa.com/news-2/chatgpt-images-20-accurac-style-non-english-text-support-11752887">ChatGPT launches Images 2.0 with better accuracy, style and non-English text support</a></li>
<li><a href="https://www.technology.org/2026/04/22/chatgpt-images-2-0-finally-nails-the-one-thing-ai-art-never-could-actual-words/">ChatGPT Images 2.0 Finally Spells Correctly - Technology Org</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#image generation`, `#GPT Image 2`, `#AI models`, `#text rendering`

---

<a id="item-8"></a>
## [美国指控六家中国 AI 公司借蒸馏技术盗用美方技术](https://www.reuters.com/technology/us-accuses-chinese-ai-firms-industrial-scale-theft-ai-technology-2026-09-08/) ⭐️ 8.0/10

9 月 8 日，美国政府指控包括 DeepSeek、Moonshot AI 和阿里巴巴在内的六家中国 AI 公司，利用模型蒸馏技术在工业规模上盗用美国 AI 知识产权。指控中提到的受害企业包括 Anthropic、OpenAI、谷歌和 SpaceX，并称相关行为很可能是在中国政府知情的情况下进行的。 这项指控在习近平主席计划访美及中美 AI 安全对话之前，进一步加剧了中美在人工智能领域的紧张关系。此事可能重塑跨境 AI 合作，影响全球 AI 监管走向，并进一步限制中国企业获取美国 AI 工具和模型的渠道。 美国政府声称，所谓的蒸馏行为降低了中国企业的研发成本，并增强了中国的军事和网络攻击能力。该指控发生在习近平预计访美的数日前，直接与当前的地缘政治和 AI 政策谈判相关联。

telegram · zaihuapd · Sep 9, 01:43

**背景**: 知识蒸馏是一种机器学习技术，通过训练一个较小的“学生模型”来模仿较大的“教师模型”的行为，通常用于提高效率并降低计算成本。该技术在 AI 研发中被广泛使用，但如果企业利用其他公司专有模型的输出结果来训练自己的竞争性系统，就会引发知识产权和授权争议。此次美方指控将这种原本常见的技术，在未获授权且跨越国界的情况下使用时，视为一种工业规模的知识产权盗窃行为。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/knowledge-distillation">What is Knowledge distillation? | IBM</a></li>

</ul>
</details>

**标签**: `#AI`, `#US-China`, `#intellectual property`, `#regulation`, `#geopolitics`

---