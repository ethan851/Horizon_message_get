---
layout: default
title: "Horizon Summary: 2026-06-15 (ZH)"
date: 2026-06-15
lang: zh
---

> From 25 items, 8 important content pieces were selected

---

1. [Gary Bernhardt 2014 年演讲预言 JavaScript 的演变](#item-1) ⭐️ 9.0/10
2. [科博因 Adobe RMSDK 拒绝有效 ePub 文件](#item-2) ⭐️ 8.0/10
3. [里约热内卢的'本土'LLM 被揭露为权重合并](#item-3) ⭐️ 8.0/10
4. [形式化方法：Jane Street 探讨验证未来](#item-4) ⭐️ 8.0/10
5. [Linux 内核 7.1 发布：修复 WiFi、新 NTFS 驱动、移除旧驱动](#item-5) ⭐️ 8.0/10
6. [AI 为何尚未取代软件工程师](#item-6) ⭐️ 8.0/10
7. [华为开源盘古 2.0，参数最高达 505B](#item-7) ⭐️ 8.0/10
8. [美国政府下令 Anthropic 封锁 Mythos 人工智能模型](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Gary Bernhardt 2014 年演讲预言 JavaScript 的演变](https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript) ⭐️ 9.0/10

Gary Bernhardt 2014 年的演讲《JavaScript 的诞生与死亡》幽默地预言了 JavaScript 将成为通用的编译目标，并最终被更好的底层语言所取代。这一预言随着 TypeScript 的兴起和 WebAssembly 的出现，被证明极具先见之明。 该演讲准确预测了 Web 开发的重大趋势，比如编译为 JavaScript 的语言的出现以及对高性能底层目标的需求。其见解持续影响着开发者对 JavaScript 角色的认知以及 Web 应用性能的未来发展。 该演讲于 2014 年发布，特别提到 asm.js 作为通向通用编译目标的垫脚石，后来影响了 WebAssembly 的发展。演讲还幽默地预言了 2020-2025 年间的一场全球灾难，不过灾难类型猜错了。

hackernews · subset · Jun 14, 12:38 · [社区讨论](https://news.ycombinator.com/item?id=48526661)

**背景**: 编译目标是指编译器将源代码翻译成的语言或格式。历史上，JavaScript 仅仅是源语言，直到作为 JavaScript 子集的 asm.js 出现，成为 C/C++程序的编译目标。WebAssembly（Wasm）是一种低层二进制指令格式，设计为可移植的编译目标，能够在网页及其他环境中实现高性能应用。它于 2015 年宣布，2017 年首次发布，并于 2019 年成为 W3C 推荐标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Compiler">Compiler - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍赞扬该演讲的先见之明，指出其对 JavaScript 演化和 WebAssembly 兴起的准确预测。有人提到了作者著名的“Wat”演讲，还有一条评论幽默地指出：“每隔几年我们就发明一个更好的 JavaScript，然后把它编译成 JavaScript。”

**标签**: `#JavaScript`, `#programming languages`, `#compilation target`, `#Gary Bernhardt`, `#web development`

---

<a id="item-2"></a>
## [科博因 Adobe RMSDK 拒绝有效 ePub 文件](https://andreklein.net/your-epub-is-fine-kobo-disagrees-blame-adobe/) ⭐️ 8.0/10

文章指出，通过验证的 ePub 文件仍被 Kobo 设备拒绝，原因是 Adobe 的 RMSDK 在 EPUB 标准之外施加了更严格、不透明的要求，导致符合标准的文件出现兼容性问题。 这暴露了电子书生态系统中普遍存在的兼容性问题，迫使出版商和开发者不得不应对 Adobe RMSDK 等专有软件，削弱了 EPUB 等开放标准的承诺。 Kobo 使用 Adobe 的 RMSDK 进行渲染，该 SDK 有超出 EPUB 验证范围且未文档化的要求；社区提供的 kepubify 等工作方案可将文件转换为 Kobo 自有格式以绕过该问题。

hackernews · sohkamyung · Jun 14, 22:54 · [社区讨论](https://news.ycombinator.com/item?id=48533848)

**背景**: EPUB 是一种电子书标准格式，有 epubcheck 等验证工具确保合规性。然而，设备制造商通常采用专有渲染引擎；Kobo 使用 Adobe 的 RMSDK，该 SDK 增加了额外限制，导致技术上有效的 ePub 被拒绝。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.adobe.com/in/solutions/ebook/rmsdk/faq.html">Solutions - Ebook - rmsdk - FAQs</a></li>
<li><a href="https://medium.com/@jiminypan/five-interesting-facts-about-adobe-legacy-ebook-rmsdk-b7be0123c874">Five interesting facts about Adobe legacy eBook RMSDK | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Adobe 的质量控制不足和 RMSDK 缺乏支持表示沮丧，指出即使是独立开发者也无法获得访问权限。一些人建议使用 PineNote 等替代设备或通过 kepubify 转换文件，另一些人则批评 EPUB 规范依赖实时标准。

**标签**: `#epub`, `#adobe`, `#kobo`, `#ebooks`, `#drm`

---

<a id="item-3"></a>
## [里约热内卢的'本土'LLM 被揭露为权重合并](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

社区调查发现，里约热内卢市政府发布的 Rio-3.5-Open-397B 模型实际上是约 60%的 Nex-N2 Pro 和 40%的 Qwen3.5-397B-A17B 的加权合并，而非自称的本土微调模型。 这一争议凸显了开源 AI 开发中关于透明度和归属感的日益担忧，尤其是当公共实体在未充分披露的情况下声称模型原创性时。 Rio 模型的每个权重张量在所有 60 层中都与 Nex 和 Qwen 的 0.6/0.4 混合比例相匹配，没有额外微调或蒸馏的证据。

hackernews · unrvl22 · Jun 14, 15:37 · [社区讨论](https://news.ycombinator.com/item?id=48528371)

**背景**: 模型合并是一种将多个基于相同基础架构的微调模型的权重组合的技术，使单个模型无需额外训练即可继承所有源模型的能力。常用方法包括加权平均、SLERP 和 TIES-Merging。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-model-merging-for-llms/">An Introduction to Model Merging for LLMs | NVIDIA Technical Blog</a></li>
<li><a href="https://www.linkedin.com/posts/tanveer-m-a13016a9_the-4-model-merging-techniques-how-to-combine-activity-7436097234850570241-JP8N">Model Merging : Combining Fine-Tuned AI Models for... | LinkedIn</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了失望，并对未经归属利用他人工作获利提出伦理质疑。有人推测所称的蒸馏可能并未包含在上传的模型中，从而造成了混淆。

**标签**: `#AI`, `#LLM`, `#open-source`, `#ethics`, `#model merging`

---

<a id="item-4"></a>
## [形式化方法：Jane Street 探讨验证未来](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 8.0/10

Jane Street 发表了一篇关于编程中形式化方法的文章，强调了它们日益增长的重要性，并探讨了诸如 SAT 求解器和 Boyer-Moore 证明器之类的历史工具，以及包括 AI 辅助验证在内的未来影响。 随着 AI 生成越来越多的代码，将人力从编写转移到验证变得至关重要，而形式化方法为确保正确性提供了严格的数学基础。 文章提到了早期使用 Oppen-Nelson 简化器和 Boyer-Moore 证明器的工作，并讨论了现代方法，例如 Scala 3 中携带编译时证明的表达性类型系统。

hackernews · eatonphil · Jun 14, 12:35 · [社区讨论](https://news.ycombinator.com/item?id=48526633)

**背景**: 形式化方法是用于指定和验证软件正确性的数学技术。它们使用形式化语言来描述系统行为，并使用自动定理证明器或模型检查器来证明属性。该领域已从手动证明发展到现代 SMT 求解器，这些求解器自动化了大部分验证过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Formal_methods">Formal methods - Wikipedia</a></li>
<li><a href="https://web.mit.edu/16.35/www/lecturenotes/FormalMethods.pdf">Introducing Formal Methods - MIT</a></li>
<li><a href="https://www.microsoft.com/en-us/research/project/trusted-ai-assisted-programming/">Trusted AI-assisted Programming - Microsoft Research dafny-annotator: AI-Assisted Verification for Dafny The "Trust, But Verify" Pattern For AI-Assisted Engineering A Toolchain for AI-Assisted Code Specification, Synthesis and ... Towards AI-Assisted Synthesis of Verified Dafny Methods</a></li>

</ul>
</details>

**社区讨论**: 社区评论反映了多样化的经验：一位用户回忆了早期使用 SAT 求解器和 Boyer-Moore 证明器的正确性证明工作，另一位则讨论了在 Scala 3 中使用表达性类型进行编译时证明。一些人表示怀疑，认为形式化规范只是重复测试或实现，而另一些人则强调 AI 代码生成将人类价值转向验证的挑战。

**标签**: `#formal methods`, `#programming`, `#verification`, `#types`, `#software engineering`

---

<a id="item-5"></a>
## [Linux 内核 7.1 发布：修复 WiFi、新 NTFS 驱动、移除旧驱动](https://lore.kernel.org/lkml/CAHk-=wi4BF4bMhZNZ1tqs+FFV4OuZRe3ZqdWB+LxRLmRweUzQw@mail.gmail.com/T/#u) ⭐️ 8.0/10

Linux 内核 7.1 已发布，包含修复慢速 WiFi、新的 NTFS 驱动，以及因 AI 辅助错误报告垃圾信息而移除过时驱动（ISDN、业余无线电、ATM）等特性。 此次发布展示了 AI 如何通过迫使移除鲜少使用的代码来管理 AI 生成的错误报告，从而重塑内核维护，同时通过新 NTFS 驱动和 WiFi 修复提供了更好的硬件支持。 Jakub Kicinski 的移除提交删除了 138,161 行代码。新的 NTFS 驱动取代了之前 Paragon 的 ntfs3 驱动，旨在提供更好的稳定性和性能。

hackernews · berlianta · Jun 14, 16:01 · [社区讨论](https://news.ycombinator.com/item?id=48528729)

**背景**: Linux 内核版本号在足够多的次要版本后会递增主版本号（如 7.1）。AI 生成的错误报告，尤其是来自大型语言模型的报告，日益增多，导致维护者考虑移除旧子系统以减少报告负担。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://devtake.dev/article/linux-7-1-ham-radio-isdn-removal/">Linux 7.1 is yanking ham radio, ISDN, and ATM. The reason: AI …</a></li>
<li><a href="https://www.theregister.com/2026/03/26/greg_kroahhartman_ai_kernel/">Linux kernel czar says AI bug reports aren't slop anymore</a></li>
<li><a href="https://linux.slashdot.org/story/26/05/23/2041253/linus-torvalds-on-how-ai-is-impacting-the-hunt-for-linux-kernel-bugs">Linus Torvalds on How AI is Impacting the Hunt for Linux Kernel Bugs</a></li>

</ul>
</details>

**社区讨论**: 社区成员对 WiFi 修复和新 NTFS 驱动表示兴奋。有人称赞移除旧驱动是 AI 错误报告的积极后果，称之为'去脂'。另一些人指出 7.1 版本只是常规递增，并无特别之处。

**标签**: `#Linux`, `#kernel`, `#open source`, `#AI`, `#bug reporting`

---

<a id="item-6"></a>
## [AI 为何尚未取代软件工程师](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan 和 Sayash Kapoor 发表文章，认为 AI 不会导致软件工程师大规模失业，并引用纽约 WARN 法案披露第一年没有 AI 相关裁员报告作为证据。 这挑战了 AI 将很快自动化软件工程工作的主流观点，表明该职业的核心价值在于深度的人类理解，而不仅仅是代码生成。 文章指出了软件工程的三个真正瓶颈：决定构建什么、验证交付的工作，以及两者所需的深度人类理解。它指出 AI 加快了输入代码的速度，但并未加速这些关键任务。

rss · Simon Willison · Jun 14, 23:54

**背景**: WARN 法案（工人调整和再培训通知法案）要求美国雇主在大规模裁员前提前 60 天通知。纽约于 2025 年 3 月增加了 AI 披露复选框。软件工程远不止编写代码，还需要理解业务需求、调试和沟通。

**标签**: `#AI`, `#software engineering`, `#job displacement`, `#labor market`, `#technology`

---

<a id="item-7"></a>
## [华为开源盘古 2.0，参数最高达 505B](https://t.me/zaihuapd/41948) ⭐️ 8.0/10

在 2026 年华为开发者大会上，华为发布了开源盘古 2.0 模型（openPangu 2.0），包含 505B 参数的 Pro 版和 92B 参数的 Flash 版，均支持 512K 上下文窗口。计划从 6 月 30 日起陆续开源七大组件。 这一来自中国科技巨头的重要开源大模型发布，具备竞争性规格，可能加速基于华为昇腾生态的 AI 开发，并对全球领先者构成挑战。这也表明华为在内部算力有限的情况下，仍致力于开源 AI。 505B 参数的 Pro 版和 92B 参数的 Flash 版均支持 512K token 上下文窗口，使其跻身顶级长上下文模型之列。开源发布包括预训练代码等七大组件，并针对昇腾算力和鸿蒙系统进行了优化。

telegram · zaihuapd · Jun 14, 08:05

**背景**: 华为昇腾 950PR 芯片已成为中国科技公司的主要 AI 芯片，取代了英伟达在中国的市场份额。支持 512K 上下文窗口的大语言模型日益常见，已有十多个模型支持 100 万 token 以上。华为早在多年前大模型尚处萌芽期时就发布了盘古模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huaweicentral.com/ascend-950pr-ai-chip-everything-you-need-to-know/">Ascend 950PR AI Chip: Everything you need to know - Huawei Central</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/huawei-expects-12-billion-in-ai-chip-revenue-this-year-as-nvidias-china-market-share-hits-zero">Huawei braces for $12 billion in AI chip revenue driven by homegrown AI model demand — Chinese fabs can barely keep up as Nvidia's market share craters within the region | Tom's Hardware</a></li>
<li><a href="https://www.morphllm.com/llm-context-window-comparison">LLM Context Window Comparison (2026): 20 Models From 200K to ...</a></li>

</ul>
</details>

**社区讨论**: 来自 Telegram 来源的社区讨论有限，但由于竞争性规格和开源性质，该公告引起了兴趣，不过一些人可能质疑其在昇腾硬件上的实际可用性和性能。

**标签**: `#open-source`, `#large language model`, `#Huawei`, `#Pangu`, `#AI`

---

<a id="item-8"></a>
## [美国政府下令 Anthropic 封锁 Mythos 人工智能模型](https://t.me/zaihuapd/41949) ⭐️ 8.0/10

美国商务部以国家安全权力为由，发布出口管制指令，要求 Anthropic 停止向所有客户（包括外籍员工）提供其 Fable 5 和 Mythos 5 人工智能模型的访问权限。Anthropic 已遵守指令关闭了这两款模型，并表示其他 Claude 模型不受影响。 这标志着美国政府直接干预人工智能模型分发的重要升级，针对的是可能被滥用并构成国家安全风险的先进模型。此举为 AI 模型权重的出口管制树立了先例，可能影响全球人工智能监管及前沿 AI 公司的竞争格局。 该指令的触发原因是对模型可能被越狱绕过安全防护的担忧，尤其是在网络安全和生物学领域存在风险。Anthropic 此前曾发布 Fable 5 作为 Mythos 5 的更安全、面向公众的版本，但政府要求完全封锁这两款模型的访问权限。

telegram · zaihuapd · Jun 14, 09:06

**背景**: Anthropic 的 Mythos 模型是高度强大的人工智能系统，在某些任务上超越人类，但也存在潜在的安全风险。美国政府一直在收紧对先进 AI 技术的出口管制，特别是防止对手获取敏感的模型权重。此举是更广泛监管努力的一部分，旨在平衡 AI 创新与国家安全，近期实体清单和出口管制政策的更新也体现了这一点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/mythos">Claude Mythos \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/United_States_export_controls_on_AI_chips_and_semiconductors">United States export controls on AI chips and semiconductors</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#export controls`, `#national security`, `#Anthropic`, `#AI policy`

---