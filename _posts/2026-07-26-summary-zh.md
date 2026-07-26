---
layout: default
title: "Horizon Summary: 2026-07-26 (ZH)"
date: 2026-07-26
lang: zh
---

> From 21 items, 6 important content pieces were selected

---

1. [vLLM v0.26.0 发布：支持 Inkling 与 DeepSeek-V4 优化](#item-1) ⭐️ 8.0/10
2. [开源权重 AI 迎来 Kubernetes 时刻](#item-2) ⭐️ 8.0/10
3. [Android 可能很快限制设备端 ADB](#item-3) ⭐️ 8.0/10
4. [Ruff v0.16.0 默认规则从 59 条扩展到 413 条](#item-4) ⭐️ 8.0/10
5. [马斯克支持库克对内存涨价的评论，美光指责苹果](#item-5) ⭐️ 8.0/10
6. [近 200 家硅谷公司反对禁止中国开放权重 AI](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0 发布：支持 Inkling 与 DeepSeek-V4 优化](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 现已发布，包含 212 位贡献者的 411 次提交。新增对 Inkling 模型系列的全面支持、跨供应商的 DeepSeek-V4 性能优化，以及通过 head_dtype 选项支持 fp32 精度的 lm_head。 此更新巩固了 vLLM 作为领先推理引擎的地位，支持像 Inkling 这样的前沿模型，并推动了 DeepSeek-V4 的性能极限，直接影响了生产 AI 系统的部署效率和准确性。 Inkling 支持包括分段 CUDA 图、Hopper FA4 相对注意力、MTP=1 推测解码和 NVFP4 量化。DeepSeek-V4 优化通过专门的路由内核实现了 2.94% 的端到端 TPOT 改进，并且 fused_topk_bias 获得了 1.5–2 倍的内核加速。

github · khluu · Jul 25, 10:38

**背景**: vLLM 是一个流行的开源 LLM 推理库，利用 PagedAttention 和连续批处理等技术实现高吞吐量。Inkling 模型来自 Thinking Machines Lab，是一个拥有 975B 总参数、41B 活跃参数的 MoE 变压器，支持文本、图像和音频输入。DeepSeek-V4 是 DeepSeek 的一个重要 LLM，在此版本中从其优化中受益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://vllm.ai/blog/2026-07-15-inkling">TML Inkling on vLLM: Day-0 Support with Optimized Performance | vLLM Blog</a></li>

</ul>
</details>

**标签**: `#vllm`, `#LLM inference`, `#release`, `#performance optimization`, `#DeepSeek`

---

<a id="item-2"></a>
## [开源权重 AI 迎来 Kubernetes 时刻](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

开源权重 AI 模型正逐渐被视为类似 Kubernetes 的基础设施，但在监管、定价和协作开发方面面临挑战。 如果开源权重模型像 Kubernetes 一样普及，它们将普及 AI 访问、降低推理成本并促进协作生态，影响初创公司、企业和地缘政治。 文章将 Kubernetes 在容器编排领域的崛起与开源权重 AI 进行类比。关键挑战包括按来源禁止模型的可行性、波动的‘tokenomics’定价以及需要像 Linux 那样协作开发模型。

hackernews · tknaup · Jul 25, 14:49 · [社区讨论](https://news.ycombinator.com/item?id=49048034)

**背景**: 开源权重 AI 模型允许下载模型参数（权重），用户可运行和自定义，类似于 Meta 的 Llama。这与完全开源 AI 不同，后者还包括训练代码和数据。Kubernetes 是一个开源容器编排平台，通过社区协作成为行业标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>
<li><a href="https://biz.chosun.com/en/en-it/2025/08/06/YNGJCP3ISNEUTGFKBXDS4OXY3I/">OpenAI launches open - weight AI models to enhance... - CHOSUNBIZ</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tokenomics">Tokenomics - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了禁止中国开源权重模型的可行性，ozgung 认为不可能，因为权重只是数字，没有原产国。firasd 批评了‘tokenomics’定价波动性，而 pianopatrick 建议，像 Kubernetes 一样，AI 模型需要公开训练数据和企业合作才能成功。

**标签**: `#open-weight AI`, `#Kubernetes analogy`, `#AI regulation`, `#tokenomics`, `#open source`

---

<a id="item-3"></a>
## [Android 可能很快限制设备端 ADB](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

Android 可能很快限制设备端 ADB（Android 调试桥）的使用，要求用户通过 USB 或无线 ADB 从计算机连接，而不是直接在设备上运行 ADB。 这一变化将影响依赖设备端 ADB 进行调试和侧载应用的开发者和高级用户，可能会提高安全性但降低 Android 设备的灵活性。 攻击向量需要同时启用开发者设置和远程 ADB，对 99.9% 的用户来说不现实，但 Google 仍在考虑限制。该提案还包括限制访问特定 IP 地址或接口。

hackernews · shscs911 · Jul 25, 06:57 · [社区讨论](https://news.ycombinator.com/item?id=49045159)

**背景**: Android 调试桥（ADB）是一个命令行工具，允许开发者与 Android 设备通信，用于调试、安装应用和访问 Unix shell。设备端 ADB 让用户无需计算机即可直接在设备上运行 ADB 命令，这虽然方便，但如果恶意应用获得访问权限，也会带来安全风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_Debug_Bridge">Android Debug Bridge - Wikipedia</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>
<li><a href="https://help.esper.io/hc/en-us/articles/12657625935761-Installing-the-Android-Debug-Bridge-ADB-Tool">Installing the Android Debug Bridge (ADB) Tool – Esper Help</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：一些人认为攻击向量过于小众，不足以证明限制的合理性；而另一些人则视其为 Android 走向锁定的必然步骤，并将其与过去的侧载限制相比较。有人担心 Google 的心态正在偏离开放，技术上的变通方法可能无济于事。

**标签**: `#Android`, `#ADB`, `#Developer Tools`, `#Security`

---

<a id="item-4"></a>
## [Ruff v0.16.0 默认规则从 59 条扩展到 413 条](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0 于 2026 年 7 月 23 日发布，默认规则从 59 条增加到 413 条，导致使用未固定 ruff 依赖的项目立即出现 CI 失败。 默认规则的急剧扩展意味着许多 Python 项目现在会发现数百个以前未被注意到的问题，显著提高代码质量并及早捕获潜在错误。同时，这也破坏了使用未固定依赖的 CI 流水线，迫使开发者要么固定版本，要么更新代码。 此次更新将规则总数从 708 条增加到 968 条，许多新规则针对以前默认未启用的语法错误和运行时错误。该版本包含 `ruff check --fix --unsafe-fixes` 等工具，可帮助自动解决许多新问题。

rss · Simon Willison · Jul 25, 22:44

**背景**: Ruff 是一个用 Rust 编写的极速 Python 代码检查器和格式化工具，提供超过 900 条内置规则，并原生实现了流行的 Flake8 插件。'未固定依赖' 指包的版本未精确指定，因此像这样的升级会在下次安装时自动生效，当引入破坏性更改时可能导致意外的 CI 失败。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.astral.sh/ruff/">Ruff</a></li>
<li><a href="https://github.com/astral-sh/ruff">GitHub - astral-sh/ruff: An extremely fast Python linter and code formatter, written in Rust. · GitHub</a></li>

</ul>
</details>

**标签**: `#ruff`, `#python`, `#linting`, `#breaking changes`

---

<a id="item-5"></a>
## [马斯克支持库克对内存涨价的评论，美光指责苹果](https://t.me/zaihuapd/42761) ⭐️ 8.0/10

埃隆·马斯克转发了蒂姆·库克关于内存价格暴涨的评论，称这是他见过最大的价格上涨。马斯克主张大幅提高产量，并将其与他的特斯拉 Terafab 项目联系起来，而美光首席商务官暗示苹果在 2023 年行业低迷期间的激进供应链压价是导致当前短缺的因素之一。 这突显了内存行业供应链的紧张关系，激进的买方行为可能导致长期产能短缺。马斯克和库克等主要人物的参与表明，内存定价对科技巨头来说是一个关键问题，可能影响产品成本和可用性。 马斯克特别提到他的特斯拉 Terafab 芯片工厂项目，旨在将多个内存上下游设施整合在同一园区。美光首席商务官萨达纳对《华尔街日报》表示，在 2023 年低迷期间，一些客户极力压低价格，导致美光利润转负，无力投资扩大产能。

telegram · zaihuapd · Jul 25, 04:02

**背景**: 内存价格经历周期波动，但最近的暴涨被描述为前所未有。特斯拉的 Terafab 是一个计划投资 200 亿美元的半导体制造设施，位于德克萨斯州奥斯汀，旨在为特斯拉的产品（包括 Cybercab 和 Optimus 机器人）生产先进的 AI 芯片。该项目最早在 2026 年初被提及，并于 2026 年 3 月正式宣布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Terafab">Terafab - Wikipedia</a></li>
<li><a href="https://electrek.co/2026/06/30/tesla-intel-veteran-terafab-director/">Tesla poaches 17-year Intel veteran to lead its 'Terafab' chip plant | Electrek</a></li>

</ul>
</details>

**标签**: `#memory`, `#supply chain`, `#Apple`, `#Elon Musk`, `#industry trends`

---

<a id="item-6"></a>
## [近 200 家硅谷公司反对禁止中国开放权重 AI](https://t.me/zaihuapd/42772) ⭐️ 8.0/10

包括 Proton 和 Y Combinator 在内的近 200 家硅谷公司致信特朗普政府，敦促其不要禁止中国开放权重 AI 模型，并警告此类禁令将损害美国初创企业。 这场联合反对凸显了硅谷初创企业对中国高性价比 AI 模型的深度依赖，禁令可能严重削弱美国在 AI 生态系统中的竞争力。 这封信由 Little Tech Association 组织，该协会认为全面禁令将压垮下一代美国初创公司，而有针对性的安全措施是更好的替代方案。

telegram · zaihuapd · Jul 26, 02:00

**背景**: 开放权重 AI 模型发布了训练好的神经网络权重，允许用户无需依赖云 API 即可托管、微调和部署模型。与完全开源模型不同，开放权重模型可能不提供训练数据和代码。来自 DeepSeek 和阿里巴巴等公司的中国开放权重模型因其低成本和可定制性而被硅谷初创企业广泛使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>
<li><a href="https://engineadvocacyfoundation.medium.com/ai-essentials-what-are-model-weights-2e5b47ec77a1">AI Essentials: What are model weights? | by Engine | Medium</a></li>

</ul>
</details>

**标签**: `#AI policy`, `#US-China relations`, `#open-weight AI`, `#Silicon Valley`, `#startups`

---