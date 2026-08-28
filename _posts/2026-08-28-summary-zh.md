---
layout: default
title: "Horizon Summary: 2026-08-28 (ZH)"
date: 2026-08-28
lang: zh
---

> From 29 items, 10 important content pieces were selected

---

1. [通过 zip 与模块遮蔽破解 Claude Code Opus 5 Auto Mode](#item-1) ⭐️ 9.0/10
2. [Cloudflare 通过优化 DNS 缓存节省 100 TB 内存](#item-2) ⭐️ 8.0/10
3. [小型语言模型迎来实用化转折点](#item-3) ⭐️ 8.0/10
4. [Pollen Robotics 发布开源双足机器人 Microduck](#item-4) ⭐️ 8.0/10
5. [谷歌推出 Gemini Omni 1.1 Flash，支持 4K 视频生成](#item-5) ⭐️ 8.0/10
6. [Experiential：开源 Rust LLM 网关，基于使用流量训练更优模型](#item-6) ⭐️ 8.0/10
7. [数据驱动项目揭示 Claude 的「承重」式词汇癖好](#item-7) ⭐️ 8.0/10
8. [84 天反编译 N64 游戏：逆向工程深度解析](#item-8) ⭐️ 8.0/10
9. [Anthropic 开放模型硬件标准预览，打造 AI 操控物理设备通用规范](#item-9) ⭐️ 8.0/10
10. [腾讯发布混元 Hy4 preview，盲测得分略胜 GLM-5.3 与 Kimi K3](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [通过 zip 与模块遮蔽破解 Claude Code Opus 5 Auto Mode](https://simonwillison.net/2026/Aug/27/breaking-claude-code-opus-5-auto-mode/) ⭐️ 9.0/10

Johann Rehberger 发现了一种提示注入攻击，在约 80%的情况下可绕过 Claude Code Opus 5 Auto Mode。该攻击诱使代理解压包含恶意 struct.py 的 zip 压缩包，当代理导入 base64 时，Python 会加载这个本地模块。 Anthropic 已将 Auto Mode 设为 Claude Code 的默认设置，并声称它能防御提示注入，因此这一发现直接挑战了这些安全承诺。由于该攻击利用常见的压缩包解压和 Python 导入机制，它威胁到任何处理不可信文件或网页内容的 Claude Code 用户。 Auto Mode 将工具调用交由安全分类器处理，以阻止不可逆、破坏性或面向外部的操作；在几次运行中，分类器甚至拒绝了 Claude 自己发出的终止已检测到的恶意进程的命令。Rehberger 建议在容器、虚拟机或操作系统沙箱中运行无人值守代理，限制网络出口，监控代理运行，并且不向代理运行时暴露主目录或凭据。

rss · Simon Willison · Aug 27, 22:50

**背景**: 提示注入是一类攻击，将恶意指令嵌入到 AI 模型处理的内容中，从而劫持模型的行为。Claude Code 的 Auto Mode 使用独立的分类器（例如在 Opus 5 运行时使用 Sonnet-5）来评判工具调用，并在不提示用户的情况下阻止危险操作。Python 模块遮蔽是指本地文件与标准库模块同名，导致 Python 导入系统优先加载本地文件。在该攻击中，从 zip 压缩包解压出的恶意 struct.py 会在代理代码导入 base64 时被执行，因为 base64 内部会导入 struct。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://veganmosfet.codeberg.page/posts/2026-08-12-opus5_automode/">Prompt Injection Experiments with Opus - 5 in Claude Code ...</a></li>
<li><a href="https://openillumi.com/en/en-torch-utils-error-fix-shadowing/">Stop `AttributeError: torch._utils`: Fix PyTorch File Shadowing</a></li>
<li><a href="https://www.pythontutorials.net/blog/attributeerror-module-object-has-no-attribute-reader/">How to Fix AttributeError: ' module ' object has no... — pythontutorials...</a></li>

</ul>
</details>

**标签**: `#security`, `#prompt injection`, `#Claude Code`, `#vulnerability`, `#AI agents`

---

<a id="item-2"></a>
## [Cloudflare 通过优化 DNS 缓存节省 100 TB 内存](https://blog.cloudflare.com/dns-cache-memory-optimization-1111/) ⭐️ 8.0/10

Cloudflare 在一篇新的工程博客文章中详细介绍了如何通过优化缓存的数据结构和内存分配，在其全球 1.1.1.1 DNS 解析器上节省了约 100 TB 内存。这次优化的重点是 DNS 缓存条目的存储和分配方式，而不是改变解析器的功能。 这很重要，因为 DNS 解析器以巨大规模运行，内存是 anycast 基础设施的重要成本因素。如此大规模的减少内存使用可以降低资本和运营支出，同时为数亿用户提高缓存效率和整体响应性能。 根据社区评论，优化包括避免为缓存条目记录数据单独分配内存、对某些数据结构使用单次大分配，以及仔细对齐结构体字段以减少填充浪费。文章还讨论了在 Rust 的安全保证与将多个独立列表合并到单个内存块的需求之间的权衡。

hackernews · TangerineDream · Aug 27, 17:17 · [社区讨论](https://news.ycombinator.com/item?id=49468083)

**背景**: 1.1.1.1 是 Cloudflare 的公共 DNS 解析器，在全球处理大量查询。DNS 解析器会缓存映射信息以加快查找速度；这些缓存存储在内存中，因此随着流量增长，缓存的内存占用也会增大。优化缓存条目的布局和分配可以在不影响解析器行为的情况下产生可观的节省。

**社区讨论**: 评论者普遍对这种方法表示赞赏，有人指出这表明系统编程仍然很重要。其他人分享了相关的内存优化经历，并指出了结构体对齐等替代技术，而一些讨论则关注将多个独立向量合并到单个列表是否损害了 Rust 的安全保证。

**标签**: `#DNS`, `#memory optimization`, `#systems programming`, `#Cloudflare`, `#performance`

---

<a id="item-3"></a>
## [小型语言模型迎来实用化转折点](https://calv.info/small-models-have-arrived) ⭐️ 8.0/10

一篇文章指出，小型语言模型已到达实用相关性的临界点，并预测围绕快速、廉价、'够用就好'的模型将涌现大量新的消费级和企业级应用。该文在 AI 社区引起强烈共鸣，评分 8/10，引发了数百条评论。 其意义在于，它标志着行业从'不惜代价扩大规模'的范式转向效率、隐私和成本效益。如果小模型在许多任务上已经够用，初创企业和传统企业就不必依赖前沿实验室，设备端和边缘 AI 将变得可行，消费级 AI 公司也可能终于出现。 小型语言模型通常定义为参数少于 400 亿的模型，因此可以在个人电脑和智能设备上运行。文章评论者强调，早在'思考型'模型出现之前，配备 Guidance 等工具的 70 亿参数本地模型就能驱动智能编码工作流，可见紧凑模型已取得多大进展。

hackernews · tosh · Aug 27, 15:56 · [社区讨论](https://news.ycombinator.com/item?id=49466917)

**背景**: 大型语言模型（LLM）包含数千亿甚至数万亿参数，训练和部署需要极其庞大的计算资源。小型语言模型（SLM）采用相似的架构，但参数少得多，并常通过知识蒸馏、剪枝和量化等技术进行优化。这些技术让紧凑模型能在边缘设备上运行，同时缩小与前沿模型之间的'能力差距'。这一趋势常被比作费曼所说的'底层大有可为'，因为很多应用实际上并不需要庞大的世界知识。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Small_language_model">Small language model</a></li>
<li><a href="https://medium.com/@deniz.kenan.kilic/scaling-smarter-an-overview-of-large-language-models-llms-and-their-compression-techniques-part-4e6bc846c215">Scaling Smarter: An Overview of Large Language Models ... | Medium</a></li>
<li><a href="https://blog.spheron.network/6-compression-techniques-for-language-models">6 Compression Techniques for Language Models</a></li>

</ul>
</details>

**社区讨论**: 社区整体反馈积极且富有洞见。评论者分享了使用本地 70 亿参数模型的实际实验，指出投资者困惑于消费级 AI 公司为何稀少，并讨论 AI 工作的本质——'IQ 180'式突破与'token 输出机'式执行。一条热门评论认为，在避免不必要世界知识的专用小模型上存在'底层空间'。

**标签**: `#small language models`, `#AI`, `#machine learning`, `#LLM`, `#efficiency`

---

<a id="item-4"></a>
## [Pollen Robotics 发布开源双足机器人 Microduck](https://pollen-robotics.com/microduck/) ⭐️ 8.0/10

Pollen Robotics 发布了 Microduck，这是一款小型开源双足机器人，搭载 AI 加速器和 50 Hz 板载策略循环。它出厂自带七种预训练行为，并支持在本地或通过 Hugging Face Jobs 训练额外行为，可导出为 ONNX。 Microduck 为尝试基于学习的双足运动和具身 AI 提供了一个可及的开源入口。其 AI 加速器和可训练策略循环降低了爱好者和研究人员在真实硬件上部署强化学习策略的门槛。 具体规格包括 Rockchip RK3566 处理器（带 AI 加速器）、1GB 内存、32GB 存储、Wi-Fi、蓝牙、麦克风、扬声器、两个 NFC 天线和约一小时续航的可拆卸电池。机器人重 800 克，采用 Dynamixel 伺服电机，出厂自带七种行为，包括行走、坐立、站立、踢腿、从地面拾取、轮滑和自恢复。

hackernews · robotswantdata · Aug 27, 10:57 · [社区讨论](https://news.ycombinator.com/item?id=49462763)

**背景**: AI 加速器，或称神经处理单元（NPU），是一种专门用于加速人工智能和机器学习工作负载（例如用于感知和控制的神经网络）的硬件。在基于学习的机器人技术中，“策略”是一个将观测映射到动作的神经网络；策略循环反复将当前观测输入网络并执行所产生的动作来控制机器人。Microduck 的板载策略循环以 50 Hz 运行，使得双足行为的实时推理成为可能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_accelerator">AI accelerator</a></li>
<li><a href="https://voxel51.com/glossary/policy">What is a policy in robotics and reinforcement learning? | Voxel51</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了详细规格并称赞其开源方法，同时有人指出模拟器中的键盘映射为 AZERTY（因为 Pollen Robotics 是法国公司），建议增加 QWERTY/QWERTZ 支持。还有人列出了其他开源双足和四足机器人，另一位则强调 MuJoCo 是常用于训练强化学习策略的物理引擎。

**标签**: `#robotics`, `#open-source`, `#AI`, `#hardware`, `#bipedal`

---

<a id="item-5"></a>
## [谷歌推出 Gemini Omni 1.1 Flash，支持 4K 视频生成](https://blog.google/innovation-and-ai/technology/developers-tools/build-with-gemini-omni-1-1-flash/) ⭐️ 8.0/10

谷歌发布了 Gemini Omni 1.1 Flash，这是一个面向生产环境的更新，为 Gemini API 和 Google AI Studio 增加了生成式视频能力。开发者现在可以按 10 秒递增将场景延长至最多 40 秒，指定首尾关键帧，并生成 1080p 或 4K 分辨率输出。 此次更新巩固了谷歌在快速发展的 AI 视频生成领域的地位，为开发者提供了更强的创作控制和更高质量的输出。这也凸显了谷歌在视频模型上持续投入，将其视为通向世界模型的路径，与 OpenAI 据报道放弃 Sora 形成对比。 场景扩展基于之前的一段 10 秒画面，以 10 秒为增量累加，总共延长至 40 秒。该 API 还支持指定首尾帧、先以 360p 生成草稿预览，再以 1080p 或 4K 进行最终渲染；视频生成使用 Interactions API，而非标准的 generateContent 端点，且该模型使用谷歌 TPU 训练。

hackernews · saretup · Aug 27, 17:06 · [社区讨论](https://news.ycombinator.com/item?id=49467922)

**背景**: Gemini Omni Flash 是 Gemini API 中谷歌默认的视频生成模型，与 Veo 系列并列，供不同工作流使用。Google AI Studio 于 2023 年 12 月首次发布，是一个基于 Web 的集成开发环境，让开发者及非技术用户可以使用 Gemini 模型进行原型开发，包括图像、视频和音频生成。像 Gemini Omni Flash 这样的文本到视频模型可以根据自然语言提示生成短视频片段，也是研究可模拟环境的世界模型的关键要素。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/build-with-gemini-omni-1-1-flash/">Build with Gemini Omni 1 . 1 Flash</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/video">Video generation in the Gemini API | Google AI for Developers</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-omni-flash/">Gemini Omni Flash - Model Card — Google DeepMind</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者表达了怀疑与猜测的混合情绪：有人认为 AI 最终会吞噬所有科技公司，也有人指出关于影视和配音演员所受影响的讨论太少了。有评论者赞赏谷歌在 OpenAI 放弃 Sora 后仍持续投资视频生成，还有人开玩笑说谷歌员工写提示词时应加上“请确保页面兼容 Firefox”，另有人抱怨谷歌仍未发布新版 Gemini Pro。

**标签**: `#Gemini`, `#AI`, `#Video Generation`, `#Google`, `#Developers`

---

<a id="item-6"></a>
## [Experiential：开源 Rust LLM 网关，基于使用流量训练更优模型](https://github.com/experientiallabs/experiential) ⭐️ 8.0/10

团队发布了 Experiential，一个开源的、Rust 原生的 LLM 网关，将自托管模型、前沿模型和开源模型统一到一个 API 之后。它在 BYOK 请求下增加不到 1 毫秒的延迟，在由官方提供供应商密钥时增加不到 2 毫秒，并通过自动化 codex agent 每日刷新超过 1000 个模型。 该项目回应了在碎片化 LLM 生态中对低延迟、零加价网关日益增长的需求，为 LiteLLM 等工具提供了一个真正开源的替代方案。其可选的使用流量驱动的模型路由与微调功能，可以帮助开发者在成本与质量之间做更好的权衡，而不只是简单地代理 token。 该网关使用标准化的 OpenTelemetry traces 来挖掘代表性任务，然后利用 text world models、LLM judge 以及基于 prompt 嵌入的最近邻分类器，将每个请求路由至最优模型。它还支持缓存命中优化建议、新模型推荐以及可选的定制模型训练，同时可完全部署在自托管基础设施上，或通过零加价的托管版本使用。

hackernews · SilenN · Aug 27, 21:18 · [社区讨论](https://news.ycombinator.com/item?id=49471407)

**背景**: LLM 网关是一种中间层，为应用程序提供统一 API，以访问多个 LLM 供应商、自托管模型或本地模型，负责路由、认证、成本跟踪和故障转移。OpenTelemetry traces 是一种带有上下文和关联性的结构化日志，用于展示请求在分布式系统中的流转路径。Text world models 是从文本中模拟交互环境的 AI 模型，在此处用于生成逼真的回放场景，以评估不同模型在实际任务上的表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/World_model_(artificial_intelligence)">World model (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://opentelemetry.io/docs/concepts/signals/traces/">Traces | OpenTelemetry</a></li>
<li><a href="https://www.truefoundry.com/blog/llm-gateway">What Is an LLM Gateway and How Does It Work?</a></li>

</ul>
</details>

**社区讨论**: 评论者提出了尖锐的问题，例如缓存机制——在多个模型之间切换可能导致缓存输入 token 成本激增——以及它与 LiteLLM 的区别。不少人赞赏其开源、零加价的做法和基于 Tinker 微调的思路，认为这是一个很有潜力的起点。

**标签**: `#LLM gateway`, `#open source`, `#Rust`, `#AI infrastructure`, `#model routing`

---

<a id="item-7"></a>
## [数据驱动项目揭示 Claude 的「承重」式词汇癖好](https://louisabraham.github.io/load-bearing/) ⭐️ 8.0/10

一个新的数据驱动网站分析了 Claude 最常滥用的短语，重点指出「load-bearing」及其他 LLM 输出中的风格化口头禅。作者通过 GitHub Actions 每天更新数据集，每天处理约 1000 个拉取请求。 这件事很重要，因为它量化了一个日益令人反感的现象：LLM 的文本越来越依赖空洞的修辞短语，这些短语只是暗示洞察力，而非真正提供洞察力。该分析为提示工程师和普通用户提供了一个具体目标，用以减少 AI 的「腔调」并提升输出质量。 除了「load-bearing」，该网站还标记了「the crux」和「first-class citizen」等口头禅。作者提到，有用户用奥威尔式规则要求 Claude 避免使用陈腐隐喻，Claude 却回应说这条规则「与我自己的系统提示相冲突」。

hackernews · Labo333 · Aug 27, 08:59 · [社区讨论](https://news.ycombinator.com/item?id=49461817)

**背景**: 「load-bearing」最初用来描述承重结构构件，例如支撑建筑物重量的墙壁。在 LLM 的输出中，它被挪用为修辞填充物，让陈述显得更重要。研究人员和论坛用户注意到，聊天机器人有相似的风格化口头禅，例如滥用介词短语，这是因为模型被训练成模仿模式，而不是有目的地写作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.merriam-webster.com/dictionary/load-bearing">Load-bearing | Definition & Meaning - Merriam-Webster</a></li>
<li><a href="https://dictionary.cambridge.org/dictionary/english/load-bearing">LOAD-BEARING | English meaning - Cambridge Dictionary</a></li>
<li><a href="https://talk.macpowerusers.com/t/llm-as-posts-on-this-forum/36379">LLM as posts on this forum - MPU Talk</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞该网站简洁、不带偏见的呈现方式，并指出一个讽刺现象：一个聚焦 LLM 的分析反而避免了 LLM 式的冗长。一位用户分享说，Claude 承认奥威尔的「绝不用印刷品中常见的隐喻」规则与它的系统提示相冲突；另一些人则担心，AI 生成的训练数据正在让所有模型的这类风格问题变得更严重。

**标签**: `#LLM`, `#Claude`, `#linguistics`, `#data analysis`, `#prompt engineering`

---

<a id="item-8"></a>
## [84 天反编译 N64 游戏：逆向工程深度解析](https://blog.chrislewis.au/decompiling-a-nintendo-64-game-in-84-days/) ⭐️ 8.0/10

一位开发者发布了一篇详细博客，讲述如何在 84 天内反编译一款任天堂 64（N64）游戏，并介绍了所使用的新式逆向工程工具与流程。该文章在 Hacker News 上引发了热烈讨论，获得了 233 个点赞和 137 条评论。 这个项目表明，借助大语言模型和不断改进的工具，经典游戏的反编译变得更加可行。它也凸显了社区对保护和增强复古游戏的努力，这可能推动发行商提供官方重制版或现代移植版。 文章中强调了大语言模型辅助开发是加速反编译的关键，这一趋势在 LLM4Decompile 和 DecLLM 等近期研究中也有所体现。在复古游戏社区，成功的反编译通常会催生重编译（recomp）项目，从而实现 Bug 修复、画质提升等现代功能。

hackernews · knackers · Aug 27, 15:01 · [社区讨论](https://news.ycombinator.com/item?id=49466006)

**背景**: 反编译（Decompilation）是将已编译程序的机器码转换回 C 等高级、可读语言的过程。对于任天堂 64 等早期主机上的游戏（通常用 C 和汇编编写），爱好者社区开展了‘decomp’项目，试图重建与原始源码相近的代码。这些项目对游戏保存、Mod 制作和重新发行很有价值，但有时也会引发版权争议。近年，大语言模型已被用于反编译，以提高输出可读性并自动化繁琐步骤。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/albertan017/LLM4Decompile">GitHub - albertan017/LLM4Decompile: Reverse Engineering: Decompiling Binary Code with Large Language Models · GitHub</a></li>
<li><a href="https://arxiv.org/abs/2403.05286">[2403.05286] LLM4Decompile: Decompiling Binary Code with Large Language Models</a></li>
<li><a href="https://kindatechnical.com/reverse-engineering-code-decompilation/index.html">A Guide to Reverse Engineering and Code Decompilation - All Topics</a></li>

</ul>
</details>

**社区讨论**: 总体来看，评论区反响极为正面，大家盛赞作者的技能和整个“decomp”（反编译）运动，并提及《龙骑传说》等类似重编译项目。多位用户讨论了大语言模型如何极大提升逆向工程效率，也有人质疑发行商为何不利用这些反编译成果推出官方重制版。还有不少人对作者为什么选择《雪板小子》而非《时之笛》这类更知名的作品感到好奇。

**标签**: `#reverse engineering`, `#decompilation`, `#N64`, `#LLM`, `#retro gaming`

---

<a id="item-9"></a>
## [Anthropic 开放模型硬件标准预览，打造 AI 操控物理设备通用规范](https://www.anthropic.com/news/model-hardware-standard-research-preview) ⭐️ 8.0/10

Anthropic 已开放其“模型硬件标准”（MHS）的研究预览。这是一个共享规范，可让 AI 智能体安全操控显微镜、液体处理器和机械臂等物理设备。公司表示，设备集成时间可从数周或数月缩短至几小时甚至几分钟。 这标志着 Anthropic 首次大举进军“物理 AI”领域，可能让 MHS 成为 AI 模型与硬件之间的通用接口。由于该标准据称可与任何 AI 模型配合使用，它有望加速生物技术、机器人、制造和量子计算等领域的自动化进程。 首批合作伙伴包括基因泰克、卡内基梅隆大学和量子计算公司 QuEra。QuEra 报告称，其 AI 控制器可在 99.3% 的情况下无需人工干预恢复量子计算机的激光锁定；Anthropic 计划在完成安全评估后开源 MHS。

telegram · zaihuapd · Aug 28, 01:38

**背景**: AI 智能体通常与软件而非物理设备交互，因此控制实验室工具或机器人通常需要定制化的设备专属集成，耗时数周甚至数月。MHS 旨在将这一接口标准化，就像 USB 统一了设备连接一样，让物理硬件对 AI 来说真正实现“即插即用”。目前研究预览仅向一小批科学实验室和先进制造商开放。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/model-hardware-standard-research-preview">Previewing the Model Hardware Standard \ Anthropic</a></li>
<li><a href="https://www.cnbc.com/2026/08/27/anthropic-pushes-into-physical-world-with-new-standard-to-help-ai-agents-operate-machines.html">Anthropic pushes into physical world with new standard to help AI agents operate machines</a></li>

</ul>
</details>

**标签**: `#AI`, `#Hardware`, `#Robotics`, `#Anthropic`, `#Automation`

---

<a id="item-10"></a>
## [腾讯发布混元 Hy4 preview，盲测得分略胜 GLM-5.3 与 Kimi K3](https://mp.weixin.qq.com/s/ymr3X878B8oa2XP15CH8TQ) ⭐️ 8.0/10

2026 年 8 月 28 日，腾讯发布了迄今最强的开源模型 Hy4 preview，总参数量 770B、活跃参数 49B、上下文窗口 1M token。在 203 个盲测工程任务中，它以 2.99 分小幅领先 GLM-5.3（2.92）和 Kimi K3（2.94）。 这一发布标志着腾讯进入开源大模型前沿，与 GLM、Kimi 等模型正面竞争，可能重塑开源生态格局。其 MoE 架构以仅 49B 的活跃参数实现接近前沿的工程能力，有望推动长周期软件工程、文档办公和科研场景的广泛应用，并加剧 API 定价竞争。 该模型采用混合专家（MoE）架构：770B 总参数代表显存占用，而每个 token 实际只激活 49B 参数，从而在质量与推理成本之间取得平衡。API 定价为每 100 万输入 tokens 0.834 美元、每 100 万输出 tokens 2.501 美元，并已上线腾讯云、GitHub、Hugging Face、ModelScope、AtomGit、OpenRouter 等渠道。

telegram · zaihuapd · Aug 28, 06:11

**背景**: 混合专家（MoE）是一种稀疏架构：总参数量决定显存占用，而每个 token 只激活其中一部分参数，因此推理计算量主要取决于活跃参数而非总参数量。盲测工程任务评估会先隐去模型身份再打分，以减少偏见，从而更公平地比较模型在真实软件工程和智能体任务上的表现。GLM-5.3 和 Kimi K3 分别是智谱 AI 与月之暗面推出的开源前沿大模型，代表了同一竞争空间内两种不同的扩展路线。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://localmodel.run/guides/mixture-of-experts">Mixture of experts (MoE) explained for local LLMs · localmodel.run</a></li>
<li><a href="https://localaimaster.com/blog/mixture-of-experts-explained">Mixture of Experts Explained: How DeepSeek... | Local AI Master</a></li>
<li><a href="https://tech.bixoto.com/glm-5-3-vs-kimi-k3-753b-vs-2-8t-the-older-weights-just-won-on-points/">GLM - 5 . 3 vs Kimi K 3 : 753B vs 2.8T. The Older... - Bixoto Tech Blog</a></li>

</ul>
</details>

**标签**: `#AI`, `#LLM`, `#Tencent`, `#Open Source`, `#Model Release`

---