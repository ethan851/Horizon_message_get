---
layout: default
title: "Horizon Summary: 2026-06-01 (EN)"
date: 2026-06-01
lang: en
---

> From 23 items, 4 important content pieces were selected

---

1. [Cloudflare Turnstile Uses WebGL Fingerprinting](#item-1) ⭐️ 8.0/10
2. [Dav2d: Open-Source AV2 Decoder Achieves Real-Time Software Decoding](#item-2) ⭐️ 8.0/10
3. [Linux Restartable Sequences (rseq) Enable Lock-Free Critical Sections](#item-3) ⭐️ 8.0/10
4. [AI distraction leads to subscription cancellation consideration](#item-4) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Cloudflare Turnstile Uses WebGL Fingerprinting](https://hacktivis.me/articles/cloudflare-turnstile-webgl-fingerprinting) ⭐️ 8.0/10

Cloudflare Turnstile, a privacy-focused CAPTCHA alternative, now requires WebGL fingerprinting to detect bots, as revealed in a recent analysis. This undermines Turnstile's privacy promise and shows how even privacy-oriented services may resort to browser fingerprinting, impacting user anonymity and transparency. WebGL fingerprinting exploits the unique rendering capabilities of a device's graphics hardware to generate a stable identifier, even when other fingerprinting protections are enabled.

hackernews · HypnoticOcelot · May 31, 14:13 · [Discussion](https://news.ycombinator.com/item?id=48345840)

**Background**: Turnstile is Cloudflare's alternative to CAPTCHAs like reCAPTCHA, designed to verify users without intrusive challenges. WebGL fingerprinting is a technique that uses the WebGL API to extract device-specific characteristics. The combination raises concerns because fingerprinting can be used to track users across sites without consent.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cloudflare.com/products/turnstile/">Cloudflare Turnstile - Easy CAPTCHA Alternative</a></li>
<li><a href="https://developers.cloudflare.com/turnstile/">Overview · Cloudflare Turnstile docs</a></li>
<li><a href="https://browserleaks.com/webgl">WebGL Browser Report - WebGL Fingerprinting - BrowserLeaks</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Cloudflare is known for fingerprinting (e.g., JA3), and some defended fingerprinting as necessary for bot detection. Others criticized the war on bots as leading to internet walled gardens, while a minority browser maintainer reported real user impact.

**Tags**: `#privacy`, `#fingerprinting`, `#cloudflare`, `#web-security`, `#anti-bot`

---

<a id="item-2"></a>
## [Dav2d: Open-Source AV2 Decoder Achieves Real-Time Software Decoding](https://jbkempf.com/blog/2026/dav2d/) ⭐️ 8.0/10

VideoLAN has announced dav2d, a new open-source CPU-based decoder for the AV2 video codec, capable of real-time software decoding on current hardware despite AV2's significantly increased complexity. This makes AV2 a viable candidate for practical use, offering a 25% reduction in bitrate over AV1 while maintaining quality, though software decoding remains challenging for older devices without hardware acceleration. AV2 decoding is roughly five times more complex than AV1, but dav2d achieves real-time performance through careful architecture-specific optimizations for x86, ARM, and RISC-V. The project is cross-platform and prioritizes correctness first, with further performance improvements expected.

hackernews · captain_bender · May 31, 11:44 · [Discussion](https://news.ycombinator.com/item?id=48344961)

**Background**: AV2 is the next-generation open and royalty-free video codec from the Alliance for Open Media, succeeding AV1. VideoLAN is known for VLC media player and previously developed dav1d, the optimized AV1 decoder. The dav2d project builds on that experience to bring efficient software decoding to AV2.

<details><summary>References</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Dav2d-Open-Source-AV2-Decode">VideoLAN Publishes Dav2d For Open-Source AV2 Decoder - Phoronix</a></li>
<li><a href="https://videocardz.com/newz/videolan-publishes-dav2d-an-early-cpu-decoder-for-av2-video-codec">VideoLAN publishes dav2d, an early CPU decoder for AV2 video codec - VideoCardz.com</a></li>
<li><a href="https://en.wikipedia.org/wiki/AV2_(codec)">AV2 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed feelings: some are worried that AV2's 5x complexity over AV1 will obsolete current hardware decoders, while others suggest neural decoding via tensor cores as an alternative. Overall, there is cautious optimism about dav2d's performance but concerns about hardware compatibility.

**Tags**: `#video codecs`, `#AV2`, `#decoding`, `#performance`, `#open-source`

---

<a id="item-3"></a>
## [Linux Restartable Sequences (rseq) Enable Lock-Free Critical Sections](https://justine.lol/rseq/) ⭐️ 8.0/10

An article explains how the Linux kernel's restartable sequences (rseq) feature, available since version 4.18, allows user-space code to perform atomic-like operations on per-CPU data without locks or memory barrier instructions by coordinating with the scheduler to restart critical sections if interrupted. This technique dramatically reduces overhead for thread-safe data structures on multi-core systems, especially important for high-performance computing and real-time applications. The rseq() system call registers a restartable sequence with the kernel; if the sequence is preempted, the kernel restores the CPU state to the beginning of the sequence and retries. The ABI is documented in kernel source and selftests, and glibc 2.35 added support.

hackernews · grappler · May 31, 14:38 · [Discussion](https://news.ycombinator.com/item?id=48346019)

**Background**: In concurrent programming, critical sections are code regions that must be executed atomically to prevent race conditions. Traditionally, mutexes or atomic operations are used, but they introduce overhead and scalability issues on many-core CPUs. Restartable sequences provide a lightweight alternative by letting the kernel automatically restart user-space critical sections if interrupted, avoiding locking.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.kernel.org/next/userspace-api/rseq.html">Restartable Sequences — The Linux Kernel documentation</a></li>
<li><a href="https://lwn.net/Articles/883104/">Restartable sequences in glibc - LWN.net</a></li>

</ul>
</details>

**Discussion**: Commenters praised the article but noted missing references, such as the librseq library for higher-level helpers. Some criticized the article's intro about expensive workstations as off-putting. Others discussed broader applications of introspection windows and potential use for load-link/store-conditional in user-space.

**Tags**: `#linux`, `#concurrency`, `#kernel`, `#performance`, `#rseq`

---

<a id="item-4"></a>
## [AI distraction leads to subscription cancellation consideration](https://simonwillison.net/2026/May/31/the-solution-might-be-cancelling-my-ai-subscription/#atom-everything) ⭐️ 8.0/10

David Wilson detailed 16+ abandoned projects created with AI tools, calling AI a 'thermonuclear ADHD amplifier', and is considering canceling his AI subscription. This critique resonates with many developers who find AI tools hurt attention and productivity, fueling a necessary debate on sustainable AI usage in creative work. Wilson notes that each AI session often starts with a simple request but ends hours later with unfinished projects and little value, and he hopes discipline is the skill needed to manage AI effectively.

rss · Simon Willison · May 31, 16:31

**Background**: AI coding agents like Claude can rapidly turn vague ideas into fully-fledged projects with tests and documentation, but this ease of creation can lead to a proliferation of abandoned work. The technology lowers friction so much that users may lose commitment, making attention management a critical issue.

**Discussion**: Hacker News comments show a split: some with ADHD report that AI helps them achieve focus and complete projects for the first time, while others echo Wilson's concern about distraction. One commenter described AI as a 'salve for my mind', enabling inbox zero and cross-project engagement.

**Tags**: `#AI`, `#productivity`, `#attention`, `#developer experience`, `#critique`

---