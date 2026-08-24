---
layout: default
title: "Horizon Summary: 2026-08-24 (ZH)"
date: 2026-08-24
lang: zh
---

> From 26 items, 5 important content pieces were selected

---

1. [1998 年经典论文《复杂系统如何失效》仍影响可靠性工程](#item-1) ⭐️ 9.0/10
2. [拥有我全部设备：逆向工程与 WebUSB 风险](#item-2) ⭐️ 8.0/10
3. [超 17 万非营利组织数据全失，微软应否担责？](#item-3) ⭐️ 8.0/10
4. [英伟达斥资 60 亿美元获 Poolside 授权，打造美国开源 AI 模型对标中国](#item-4) ⭐️ 8.0/10
5. [阿里拟配售 800 亿港元新股，募资全部投入 AI 建设](#item-5) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [1998 年经典论文《复杂系统如何失效》仍影响可靠性工程](https://how.complexsystems.fail/) ⭐️ 9.0/10

Richard Cook 于 1998 年发表的经典论文《How Complex Systems Fail》正在 Hacker News 上引发广泛讨论，其核心论点重新受到关注。讨论表明，该文对根本原因分析的批判至今仍对现代可靠性工程具有重要启示。 这篇论文是事件分析与可靠性工程的奠基之作，指出复杂系统的失效方式无法简单归因于单一根本原因。其观点持续影响着工程师处理故障、安全与系统设计的方式。 论文提出了诸如“复杂系统以残缺状态运行”和“灾难需要多重失效而非单点失效”等原则。它还认为，对复杂系统进行根本原因分析往往是误导性的，这一观点在 Hacker News 评论中既有支持也有质疑。

hackernews · shortcrct · Aug 23, 15:13 · [社区讨论](https://news.ycombinator.com/item?id=49409473)

**背景**: 这篇论文借鉴了社会学家 Charles Perrow 提出的常态事故理论，该理论认为在复杂且紧耦合的系统中，故障是不可避免的。在可靠性工程领域，这一视角挑战了传统的根本原因分析——后者假设存在可识别并修复的单一原因。Hacker News 的讨论还将论文与混沌工程等实践联系起来，即通过刻意引入故障来构建系统的韧性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://how.complexsystems.fail/">How Complex Systems Fail</a></li>
<li><a href="https://news.ycombinator.com/item?id=25550685">How Complex Systems Fail (1998) | Hacker News</a></li>
<li><a href="https://en.wikipedia.org/wiki/Normal_Accidents">Normal Accidents - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者大多称赞这篇论文；tptacek 称其至关重要，并说只有亲历复杂系统失效后才能体会其对根本原因分析的批判。然而，elisbce 不同意“灾难需要多重失效”的说法，指出现实世界存在许多单点故障，只是因故障率极低而尚未引发灾难。jedberg 则表示该文启发了混沌工程，即通过主动注入故障来让系统做好准备。

**标签**: `#complex systems`, `#reliability engineering`, `#incident analysis`, `#software engineering`, `#root cause`

---

<a id="item-2"></a>
## [拥有我全部设备：逆向工程与 WebUSB 风险](https://schlarp.com/posts/everything-i-own-owned/) ⭐️ 8.0/10

作者记录了一个个人项目：对拥有的每台设备进行逆向工程并取得“所有权”，首先是通过修补固件移除 ASUS ROG Swift PG42UQ 显示器上的“像素清洁”弹窗。文章强调，如今 WebUSB、WebHID 和 WebBluetooth 可能让用户在一次粗心的权限提示点击后，就使外接设备被永久植入后门。 这件事很重要，因为它突显了一个日益明显的矛盾：固件修补让消费级硬件真正归用户所有，而 WebUSB 等 Web API 则扩大了恶意网站的攻击面。对于安全研究人员和普通用户而言，理解这两方面对于保护外部设备都至关重要。 作者承认这台显示器很贵，且自己尚未真正刷入修改后的固件；有评论者则讲述了在尝试向引导分区添加 TFTP 启动路径时变砖一台路由器的经历。文章总结道，只有写入可用补丁后设备才算真正“被拥有”，而变砖风险仍是关键障碍。

hackernews · schlarpc · Aug 23, 22:41 · [社区讨论](https://news.ycombinator.com/item?id=49413320)

**背景**: WebUSB 是一组让网页与非标准 USB 设备通信的浏览器 API；WebHID 则向 Web 应用暴露键盘、游戏手柄等人机接口设备。这些 API 需要用户点击权限提示，之后网站就能向设备发送任意命令，从而带来安全风险。在硬件破解语境中，“拥有”设备意味着在其上运行修改过的固件，通常涉及反汇编、修补分支并刷写新镜像——这一过程中一旦出错就可能让硬件变砖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebUSB">WebUSB - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/WebUSB_API">WebUSB API - Web APIs | MDN</a></li>
<li><a href="https://wicg.github.io/webhid/">WebHID API</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了实用经验和观点：有人从 ASUS PG42UQ 显示器的“像素清洁”弹窗入手；有人承认在修固件时变砖了路由器，并呼吁更好的 glitching 工具和安全迭代修补方法；teddyh 引用了关于 WebUSB/WebHID/WebBluetooth 的核心要点；philips 报告称一个 LLM 智能体在数小时内逆向出了 Supernote 文件格式；compiler-devel 则称赞 LLM 带来了开源运动梦寐以求的软件与硬件自由。

**标签**: `#security`, `#reverse-engineering`, `#firmware`, `#hardware`, `#webusb`

---

<a id="item-3"></a>
## [超 17 万非营利组织数据全失，微软应否担责？](https://slate.com/technology/2026/08/microsoft-software-nonprofit-data-delete.html) ⭐️ 8.0/10

据 Slate 2026 年 8 月报道，超过 17 万个非营利组织因微软软件而丢失了全部数据，引发对云可靠性的争论。这一事件也让人们质疑企业责任，以及对云服务安全性的依赖。 非营利组织高度依赖微软云服务存储捐赠记录、财务数据和运营文件，数据全部丢失可能造成毁灭性影响。此次事件还引发了对厂商责任、数据保留政策，以及非营利部门是否需要独立备份的更广泛担忧。 数据丢失的确切原因尚不清楚；有评论者指出微软文档规定许可证到期后 90 天内不应删除数据，暗示可能是政策执行或技术故障。此事也提醒人们，云存储和 SSD 本身并不能可靠地用于长期归档。

hackernews · tchalla · Aug 23, 18:55 · [社区讨论](https://news.ycombinator.com/item?id=49411395)

**背景**: 微软 365 在非营利组织中广泛使用，通常通过捐赠或折扣许可获得。订阅到期后，微软的保留政策本应在一定期限内保存数据，但系统性故障或混乱的政策执行仍可能导致永久丢失。云服务不能替代备份，机构应为关键数据保留独立副本。

**社区讨论**: 评论者整体持批评态度：有人称微软“不是一家严肃的公司”并指责整个行业缺乏严肃性，也有人质疑问微软明文规定 90 天保留期为何还会删除数据。还有人分享个人经历，提醒云存储和 SSD 不适合长期归档。

**标签**: `#Microsoft`, `#Data Loss`, `#Cloud Computing`, `#Nonprofits`, `#Reliability`

---

<a id="item-4"></a>
## [英伟达斥资 60 亿美元获 Poolside 授权，打造美国开源 AI 模型对标中国](https://www.wsj.com/tech/ai/nvidia-is-spending-6-billion-to-build-a-powerful-u-s-alternative-to-chinese-ai-c51c38cc) ⭐️ 8.0/10

英伟达以 120 亿美元投前估值向 AI 初创公司 Poolside 投资 10 亿美元，并同意支付 60 亿美元获得其技术授权及吸纳大部分工程师。这些工程师将加入英伟达的开源权重模型项目 Nemotron，目标打造全球最强开源权重模型之一，与 DeepSeek、Kimi K3 等中国模型竞争。 这笔交易标志着英伟达迄今在开源权重 AI 模型领域最大的一次布局，加剧了与 DeepSeek 等中国开源实验室以及 OpenAI、Anthropic 等美国闭源头部企业的竞争。这可能加速高性能开源模型的普及，重塑 AI 行业的竞争格局。 根据协议，Poolside 的投前估值为 120 亿美元，英伟达的 60 亿美元授权费用不计入该估值。Poolside 逾百名工程师中的大部分将加入英伟达的 Nemotron 项目，该项目是一系列面向推理、编码和智能体应用的开源权重模型。

telegram · zaihuapd · Aug 23, 04:20

**背景**: 开源权重模型会发布训练好的神经网络参数，使他人能够运行、微调并在此基础上构建，但完整的训练数据和代码可能不会公开。英伟达的 Nemotron 系列包括 Nemotron 3.5 Lightning 等开源模型，这是一款 30B 参数的 MoE 模型，激活参数为 3B。Poolside 是一家专注于软件开发大语言模型的美国初创公司。这笔交易是英伟达在 AI 芯片与软件生态中进一步布局的一部分，同时应对中国开源模型竞争力的上升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/NVIDIA_Nemotron">NVIDIA Nemotron</a></li>
<li><a href="https://money.udn.com/money/story/123398/9708183">輝達斥資60億美元 取得 Poolside 模型授權 壯大 AI ... | 經濟日報</a></li>
<li><a href="https://www.ofweek.com/ai/2025-02/ART-201700-8420-30657041.html">3分钟看懂大 模 型 开 闭 源 战争，谁将主宰未来？ - OFweek 人工智能网</a></li>

</ul>
</details>

**标签**: `#Nvidia`, `#AI`, `#open-source`, `#Poolside`, `#investment`

---

<a id="item-5"></a>
## [阿里拟配售 800 亿港元新股，募资全部投入 AI 建设](https://www.jwview.com/jingwei/html/m/08-23/684731.shtml) ⭐️ 8.0/10

阿里巴巴 8 月 23 日宣布，拟向美国境外的非美国人士配售新股，募资总额 800 亿港元，这是其 2019 年港股上市以来首次启动的新股配售。配售所得款项净额将 100%用于投资全栈 AI 能力，加强 AI 基础设施建设。 这是中国科技公司规模最大的 AI 专项融资之一，表明阿里巴巴正大力加码 AI 基础设施，以与全球云和 AI 巨头展开竞争。此举也凸显了超大规模云厂商之间日益激烈的 AI 资本开支竞赛，将对 AI 芯片需求、云服务定价以及更广泛的 AI 生态产生影响。 本次配售面向美国境外的非美国人士，是阿里巴巴 2019 年港股上市以来首次启动的新股配售。公司表示所得款项净额将全部用于全栈 AI 能力建设，而全栈通常涵盖底层算力（芯片、服务器、数据中心）、模型层与应用层。

telegram · zaihuapd · Aug 23, 08:19

**背景**: “全栈 AI”通常指企业具备覆盖整个 AI 技术栈的能力，从底层算力（自研芯片、服务器、数据中心）到模型层再到应用层。阿里巴巴承诺将募资全部投入全栈 AI 能力与 AI 基础设施建设，意味着资金将投向算力、数据中心、模型研发，甚至可能包括自研芯片。AI 基础设施一般包括 AI 芯片、GPU 集群和数据中心网络，是大规模模型训练与推理的物理基础。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.qbitai.com/2024/02/119135.html">全栈智能才能兑现AI红利？</a></li>
<li><a href="https://m.c114.com.cn/w5339-1301043.html">全栈式AI:巨头的“战略逻辑”及未来生态博弈 - C114通信网</a></li>

</ul>
</details>

**标签**: `#Alibaba`, `#AI infrastructure`, `#investment`, `#fundraising`

---