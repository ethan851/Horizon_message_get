---
layout: default
title: "Horizon Summary: 2026-06-01 (ZH)"
date: 2026-06-01
lang: zh
---

> From 23 items, 4 important content pieces were selected

---

1. [Cloudflare Turnstile 使用 WebGL 指纹识别](#item-1) ⭐️ 8.0/10
2. [Dav2d：开源 AV2 解码器实现实时软件解码](#item-2) ⭐️ 8.0/10
3. [Linux 重启序列 (rseq) 实现无锁临界区](#item-3) ⭐️ 8.0/10
4. [AI 干扰导致考虑取消订阅](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Cloudflare Turnstile 使用 WebGL 指纹识别](https://hacktivis.me/articles/cloudflare-turnstile-webgl-fingerprinting) ⭐️ 8.0/10

Cloudflare Turnstile 是一款注重隐私的 CAPTCHA 替代方案，最近的分析显示，它现在需要使用 WebGL 指纹识别来检测机器人。 这削弱了 Turnstile 的隐私承诺，表明即使是注重隐私的服务也可能诉诸浏览器指纹识别，从而影响用户匿名性和透明度。 WebGL 指纹识别利用设备图形硬件的独特渲染能力来生成稳定的标识符，即使启用了其他指纹保护措施也是如此。

hackernews · HypnoticOcelot · May 31, 14:13 · [社区讨论](https://news.ycombinator.com/item?id=48345840)

**背景**: Turnstile 是 Cloudflare 提供的 CAPTCHA 替代方案，旨在无需侵入式挑战即可验证用户。WebGL 指纹识别是一种利用 WebGL API 提取设备特定特征的技术。这种结合引发了担忧，因为指纹识别可用于在未经用户同意的情况下跨网站追踪用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cloudflare.com/products/turnstile/">Cloudflare Turnstile - Easy CAPTCHA Alternative</a></li>
<li><a href="https://developers.cloudflare.com/turnstile/">Overview · Cloudflare Turnstile docs</a></li>
<li><a href="https://browserleaks.com/webgl">WebGL Browser Report - WebGL Fingerprinting - BrowserLeaks</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 Cloudflare 以指纹识别（如 JA3）闻名，一些人认为指纹识别是机器人检测所必需的。其他人批评打击机器人会导致互联网成为围墙花园，而一个少数派浏览器的维护者报告了给用户带来的实际影响。

**标签**: `#privacy`, `#fingerprinting`, `#cloudflare`, `#web-security`, `#anti-bot`

---

<a id="item-2"></a>
## [Dav2d：开源 AV2 解码器实现实时软件解码](https://jbkempf.com/blog/2026/dav2d/) ⭐️ 8.0/10

VideoLAN 发布了 dav2d，这是一个针对 AV2 视频编码格式的开源 CPU 解码器，能够在当前硬件上实现实时软件解码，尽管 AV2 的复杂度大幅提升。 这使得 AV2 成为实际应用的可行选择，相比 AV1 可节省 25% 的比特率同时保持质量，不过软件解码对于没有硬件加速的老旧设备仍具挑战。 AV2 解码的复杂度大约是 AV1 的五倍，但 dav2d 通过对 x86、ARM 和 RISC-V 等架构的针对性优化实现了实时性能。该项目是跨平台的，首先确保正确性，未来还有进一步的性能优化空间。

hackernews · captain_bender · May 31, 11:44 · [社区讨论](https://news.ycombinator.com/item?id=48344961)

**背景**: AV2 是开放媒体联盟（AOMedia）推出的新一代开放免版税视频编码格式，是 AV1 的继任者。VideoLAN 以 VLC 媒体播放器闻名，曾开发过优化的 AV1 解码器 dav1d。dav2d 项目基于该经验，为 AV2 带来高效的软件解码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Dav2d-Open-Source-AV2-Decode">VideoLAN Publishes Dav2d For Open-Source AV2 Decoder - Phoronix</a></li>
<li><a href="https://videocardz.com/newz/videolan-publishes-dav2d-an-early-cpu-decoder-for-av2-video-codec">VideoLAN publishes dav2d, an early CPU decoder for AV2 video codec - VideoCardz.com</a></li>
<li><a href="https://en.wikipedia.org/wiki/AV2_(codec)">AV2 - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论中观点不一：有人担心 AV2 相比 AV1 五倍的复杂度过高，会使现有硬件解码器过时；另有人提出通过张量核心进行神经解码的替代方案。总体来看，对 dav2d 的性能持谨慎乐观态度，但对硬件兼容性存在担忧。

**标签**: `#video codecs`, `#AV2`, `#decoding`, `#performance`, `#open-source`

---

<a id="item-3"></a>
## [Linux 重启序列 (rseq) 实现无锁临界区](https://justine.lol/rseq/) ⭐️ 8.0/10

一篇文章解释了 Linux 内核自 4.18 版本起提供的重启序列 (rseq) 特性，允许用户空间代码在无需锁或内存屏障指令的情况下，通过调度器协调来重启被中断的临界区，实现对每个 CPU 数据的原子类操作。 该技术大幅降低了多核系统上线程安全数据结构的开销，对高性能计算和实时应用尤为重要。 rseq() 系统调用向内核注册一个重启序列；如果序列被抢占，内核将 CPU 状态恢复至序列起点并重试。其 ABI 在内核源码和自测中有文档说明，glibc 2.35 已添加支持。

hackernews · grappler · May 31, 14:38 · [社区讨论](https://news.ycombinator.com/item?id=48346019)

**背景**: 在并发编程中，临界区是需要原子执行以防止竞态条件的代码区域。传统上使用互斥锁或原子操作，但它们在多核 CPU 上会引入开销和可伸缩性问题。重启序列提供了一种轻量级替代方案，通过让内核在用户空间临界区被中断时自动重启，避免了锁的使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.kernel.org/next/userspace-api/rseq.html">Restartable Sequences — The Linux Kernel documentation</a></li>
<li><a href="https://lwn.net/Articles/883104/">Restartable sequences in glibc - LWN.net</a></li>

</ul>
</details>

**社区讨论**: 评论者对文章表示赞赏，但指出缺少参考，如提供高级帮助函数的 librseq 库。一些人批评文章开头关于昂贵工作站的介绍令人反感。其他人讨论了自省窗口的更广泛应用以及在用户空间实现加载链接/存储条件的可能性。

**标签**: `#linux`, `#concurrency`, `#kernel`, `#performance`, `#rseq`

---

<a id="item-4"></a>
## [AI 干扰导致考虑取消订阅](https://simonwillison.net/2026/May/31/the-solution-might-be-cancelling-my-ai-subscription/#atom-everything) ⭐️ 8.0/10

David Wilson 详细列出了因使用 AI 工具而创建的 16 多个被遗弃的项目，称 AI 为‘热核 ADHD 放大器’，并正在考虑取消他的 AI 订阅。 这一批评引起了许多开发者的共鸣，他们发现 AI 工具损害了注意力和生产力，引发了关于在创造性工作中可持续使用 AI 的必要讨论。 Wilson 指出，每次 AI 会话通常从一个简单请求开始，但几小时后以未完成的项目和几乎无价值的结果告终，他希望自律是有效管理 AI 所需的关键技能。

rss · Simon Willison · May 31, 16:31

**背景**: 像 Claude 这样的 AI 编码代理可以迅速将模糊的想法转化为带有测试和文档的完整项目，但这种易创造性可能导致大量被遗弃的工作。该技术极大地降低了摩擦，用户可能失去承诺，使注意力管理成为关键问题。

**社区讨论**: Hacker News 上的评论出现了分歧：一些患有多动症的开发者表示，AI 帮助他们首次实现专注并完成项目，而另一些则认同 Wilson 关于干扰的担忧。一位评论者将 AI 描述为‘心灵的药膏’，使其实现了收件箱归零和跨项目参与。

**标签**: `#AI`, `#productivity`, `#attention`, `#developer experience`, `#critique`

---