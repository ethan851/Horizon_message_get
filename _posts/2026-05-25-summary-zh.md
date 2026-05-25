---
layout: default
title: "Horizon Summary: 2026-05-25 (ZH)"
date: 2026-05-25
lang: zh
---

> From 24 items, 7 important content pieces were selected

---

1. [APKPure 上的 Telegram 官方版内含间谍后门](#item-1) ⭐️ 9.0/10
2. [内存成本占 AI 芯片组件近三分之二](#item-2) ⭐️ 8.0/10
3. [约束衰减：LLM 智能体在架构规则下的脆弱性](#item-3) ⭐️ 8.0/10
4. [Vivado 2026.1 移除免费版 Linux 支持](#item-4) ⭐️ 8.0/10
5. [Armin Ronacher 批评 AI 生成的错误报告](#item-5) ⭐️ 8.0/10
6. [华为提出'韬定律'：以时间缩微替代几何缩微](#item-6) ⭐️ 8.0/10
7. [Epic 公布虚幻引擎 6，首款游戏《火箭联盟》](#item-7) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [APKPure 上的 Telegram 官方版内含间谍后门](https://x.com/EricParker/status/2058411298195661221) ⭐️ 9.0/10

该后门可窃取全部聊天记录、通讯录、照片、文档、GPS 定位和 SIM 卡信息，严重威胁用户隐私。从 APKPure 下载 Telegram 的用户面临极高的数据泄露风险。 被盗数据使用 AES-GCM 加密后上传至位于 38.190.225.166 的命令与控制服务器。恶意注入专门针对官方 Telegram 构建版本，而非来自 Telegram 官网的原版应用。

telegram · zaihuapd · May 24, 11:38

**背景**: APKPure 是一个第三方 Android 应用商店，允许用户直接下载 APK 文件，绕过 Google Play。与官方应用商店不同，第三方平台缺乏严格的安全检查，因此常被用于分发重新打包的恶意软件。在此事件中，攻击者获取了合法的 Telegram APK，反编译后在新的 dex 文件中添加恶意代码，重新签名，并通过 APKPure 分发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.apkpure.com/">APKPure: Download APK on Android with Free APK Downloader</a></li>

</ul>
</details>

**标签**: `#security`, `#spyware`, `#Telegram`, `#APKPure`, `#mobile malware`

---

<a id="item-2"></a>
## [内存成本占 AI 芯片组件近三分之二](https://epoch.ai/data-insights/ai-chip-component-cost-shares) ⭐️ 8.0/10

这一成本结构变化对 AI 硬件定价影响重大，表明一旦 DRAM 供应赶上需求，AI 推理和训练可能实现约 3 倍的硬件成本降低。 HBM 每 GB 消耗的晶圆产能约是 DDR5 的三倍，且制造复杂性导致良率偏低。社区讨论指出，即使没有新技术突破，等待供应赶上需求也能大幅降低成本。

hackernews · intelkishan · May 24, 16:31 · [社区讨论](https://news.ycombinator.com/item?id=48258684)

**背景**: AI 芯片（如 GPU 和 NPU）依赖高带宽内存（HBM）来为数千个并行核心提供数据。HBM 将 DRAM 芯片垂直堆叠，提供高带宽和低功耗，但制造成本高昂。AI 需求的激增使内存成本占比从很小一部分升至近三分之二。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.tomshardware.com/pc-components/ram/hbm-is-eating-your-ram">Here's why HBM is coming for your PC's RAM — HBM consumes around three times the wafer capacity of DDR5 per gigabyte, as AI supercharges demand for chips and advanced packaging | Tom's Hardware</a></li>
<li><a href="https://www.appliedmaterials.com/us/en/semiconductor/markets-and-inflections/memory/hbm.html">High Bandwidth Memory (HBM)</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出 RAM 价格飙升，有用户提到两年前 96GB DDR4 只需 250 美元，现在却要 1200 美元。一些人认为 DRAM 容量年增长 20-25%不足以满足 AI 需求，另一些人则表示会推迟硬件升级直到价格回落。

**标签**: `#AI hardware`, `#memory pricing`, `#chip costs`, `#supply chain`

---

<a id="item-3"></a>
## [约束衰减：LLM 智能体在架构规则下的脆弱性](https://arxiv.org/abs/2605.06445) ⭐️ 8.0/10

一项新的系统性研究发现，LLM 智能体表现出“约束衰减”现象：在多文件后端代码生成过程中，随着约束数量增加，其对显式架构规则的遵守程度会下降。 这一发现突显了使用 LLM 智能体进行生产级后端开发时的关键可靠性缺陷：它们在无约束的原型设计中表现良好，但在必须遵循严格架构规则时变得不可靠。 研究发现，当约束数量增加时，模型会悄然丢弃最不突出的约束，且框架惯例比显式契约更早被舍弃。尽管因成本原因未全面测试前沿模型，但在测试模型上一致观察到了性能下降。

hackernews · wek · May 24, 12:55 · [社区讨论](https://news.ycombinator.com/item?id=48256912)

**背景**: LLM 智能体是使用大型语言模型自主生成代码的系统。约束衰减是一种新发现的失效模式，智能体在长时间交互中逐渐偏离最初确认的规则。本研究专门考察了在结构约束下进行多文件后端代码生成的任务，这是现实软件工程中的常见场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.06445">[2605.06445] Constraint Decay: The Fragility of LLM Agents in ... Constraint Decay in Backend Code Generation - agentpatterns.ai Constraint Decay: The Fragility of LLM Agents in Backend Code ... Constraint Decay: The Fragility of LLM Agents in Back End ... Constraint Collapse and Fidelity Decay: When Feedback Stops ... Constraint Decay: A New Failure Type in the Era of Large ...</a></li>
<li><a href="https://www.agentpatterns.ai/verification/constraint-decay-backend-agents/">Constraint Decay in Backend Code Generation - agentpatterns.ai</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认同研究发现，一位用户提到自己在实际项目中随着复杂度增加不得不添加更多约束。另一用户指出该研究未测试最新的前沿模型，这些模型可能表现更好，但整体讨论验证了约束衰减现象在实践中的存在。

**标签**: `#LLM agents`, `#code generation`, `#AI reliability`, `#software engineering`, `#constraint decay`

---

<a id="item-4"></a>
## [Vivado 2026.1 移除免费版 Linux 支持](https://adaptivesupport.amd.com/s/question/0D5Pd00001YQLdMKAX/why-is-vivado-20261-dropping-linux-support-for-free-tier-?language=en_US) ⭐️ 8.0/10

AMD 的 Vivado 2026.1 更新移除了免费基础版（Basic tier）对 Linux 的支持，而 Windows 版继续保留。AMD 在官方论坛帖子中确认了这一变更。 这一决定可能疏远依赖 Linux 进行 FPGA 开发的学生、爱好者和开发者，从而缩小 AMD/Xilinx 生态系统。它可能促使用户转向 Lattice 或 Intel 等竞争对手，后者提供对 Linux 更友好的免费工具。 只有免费基础版失去 Linux 支持，付费的标准版和企业版仍保留 Linux 功能。免费版对于学习和小型项目至关重要，取消 Linux 支持对许多用户构成了重大障碍。

hackernews · zdw · May 24, 04:14 · [社区讨论](https://news.ycombinator.com/item?id=48254309)

**背景**: Vivado 是 AMD 用于 FPGA（现场可编程门阵列）和自适应 SoC 的集成设计环境。FPGA 是可重新配置的芯片，用于硬件加速、通信和嵌入式系统。免费版（前身为 WebPACK）允许免费使用某些器件系列的全部功能，对教育和爱好者采用至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.amd.com/en/products/software/adaptive-socs-and-fpgas/vivado.html">Vivado Overview - AMD</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vivado">Vivado - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Field-programmable_gate_array">Field-programmable gate array - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区反应普遍负面，用户称此举短视且不利于生态系统。许多人将其与 Lattice 对基本芯片免费的政策进行不利比较，并担心 AMD 优先考虑货币化而非用户增长。部分用户表示今后将更换供应商。

**标签**: `#AMD`, `#Xilinx`, `#Vivado`, `#FPGA`, `#Linux`

---

<a id="item-5"></a>
## [Armin Ronacher 批评 AI 生成的错误报告](https://simonwillison.net/2026/May/24/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Armin Ronacher 公开批评开源项目中越来越普遍的 AI 生成的错误报告，特别指出由 LLM 重写的问题常常包含不准确的结论和虚假的自信。他提出一个简单、人工观察的问题报告格式：描述运行的命令、预期行为、实际行为以及确切的错误或日志。 这很重要，因为 AI 生成的错误报告降低了问题追踪的质量，浪费了维护者处理误导性或无关信息的时间。随着 LLM 越来越多地融入开发者工作流程，这个问题将影响开源维护的可持续性和效率。 Ronacher 将这些报告称为“垃圾问题”，指出它们通常包含“虚假的最小复现”、错误根本原因猜测和不相关的错误列表。他提出的三步格式旨在去除 AI 生成的噪声，专注于直接的人工观察。

rss · Simon Willison · May 24, 18:46

**背景**: 生成式 AI 工具的兴起导致用户提交的 bug 报告越来越多地经过 LLM 自动重写或扩充。这些报告听起来自信满满，但事实往往不可靠，给维护者增加了额外的工作量，他们必须解析和验证内容。Ronacher 是 Python 和开源社区中的知名人物，以创建 Flask 和 Click 而闻名。

**标签**: `#open source`, `#bug reports`, `#LLMs`, `#software engineering`

---

<a id="item-6"></a>
## [华为提出'韬定律'：以时间缩微替代几何缩微](https://www.peopleapp.com/column/30052220655-500007509895) ⭐️ 8.0/10

华为在上海举行的 2026 国际电路与系统研讨会上提出'韬定律'，以时间缩微替代几何缩微。该公司声称过去六年已据此设计量产 381 款芯片，今年秋季将推出采用逻辑折叠技术的新麒麟手机芯片。 该定律可能为摩尔定律逼近物理极限后的半导体发展提供新路径，有望重塑行业研发方向。若经验证，它或许能在不追求极限微缩的情况下继续提升性能，使整个电子生态系统受益。 韬定律致力于在器件、电路、芯片和系统层级系统性地降低时间常数τ。华为预计，到 2031 年基于该定律的芯片晶体管密度可达 1.4 纳米制程同等水平。

telegram · zaihuapd · May 25, 01:35

**背景**: 摩尔定律指出芯片上晶体管数量大约每两年翻一番，几十年来一直推动着半导体进步。然而，随着晶体管尺寸接近原子尺度，几何缩微变得越来越困难和昂贵。传统的 Dennard 缩微等方法也面临限制。韬定律提出通过优化时间性能而非减小物理尺寸来实现范式转变。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/5/ieee-iscas-tau-scaling">HUAWEI Presents the Tau (τ) Scaling Law, Enabling Breakthroughs in ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Moore's_law">Moore's law - Wikipedia</a></li>
<li><a href="https://www.globaltimes.cn/page/202605/1361841.shtml">Huawei unveils new semiconductor law, charting fresh path for ...</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#Huawei`, `#Moore's Law`, `#chip design`, `#innovation`

---

<a id="item-7"></a>
## [Epic 公布虚幻引擎 6，首款游戏《火箭联盟》](https://www.pcgamer.com/gaming-industry/epic-reveals-first-unreal-engine-6-game-and-its-not-fortnite/) ⭐️ 8.0/10

Epic Games 在巴黎火箭联盟冠军系列赛上宣布了虚幻引擎 6，并确认《火箭联盟》将从虚幻引擎 3 直接升级到 UE6。 这标志着一个广泛使用的游戏引擎的重大新版本，表明了 Epic 的战略方向，对游戏开发潜在影响重大，尤其是虚幻引擎 5 面临优化批评之际。 《火箭联盟》自发布以来一直运行在 UE3 上，因此升级到 UE6 相当于跨越数代，堪比续作。UE6 预告片还包含了《堡垒之夜》等游戏的镜头，暗示了统一的元宇宙推进。

telegram · zaihuapd · May 25, 02:20

**背景**: 虚幻引擎是 Epic Games 开发的 3D 游戏引擎，最初用于 1998 年的游戏《虚幻》。它被视为提供游戏开发核心功能的中间件。Epic 此前于 2022 年发布 UE5，被广泛采用，但因 PC 端性能问题受到批评。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unreal_Engine">Unreal Engine - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Game_engine">Game engine - Wikipedia</a></li>

</ul>
</details>

**标签**: `#unreal-engine`, `#game-development`, `#epic-games`, `#announcement`, `#engine-update`

---