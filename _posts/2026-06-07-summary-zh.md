---
layout: default
title: "Horizon Summary: 2026-06-07 (ZH)"
date: 2026-06-07
lang: zh
---

> From 21 items, 9 important content pieces were selected

---

1. [谷歌每月向 SpaceX 支付 9.2 亿美元租用 AI 算力](#item-1) ⭐️ 9.0/10
2. [全国首例侵入式脑机接口让失明 20 年患者重见光明](#item-2) ⭐️ 9.0/10
3. [Ntsc-rs：模拟电视和 VHS 效果的开源工具](#item-3) ⭐️ 8.0/10
4. [Unix fork()+exec() 模型面临审视](#item-4) ⭐️ 8.0/10
5. [Meta AI 聊天机器人漏洞导致 Instagram 账户被接管](#item-5) ⭐️ 8.0/10
6. [Zeroserve：零配置，用 eBPF 脚本化 Web 服务器](#item-6) ⭐️ 8.0/10
7. [Nvidia 推出 RTX Spark：面向 Windows PC 的 Arm 统一内存 CPU](#item-7) ⭐️ 8.0/10
8. [宝可梦绿宝石移植到 WebAssembly，帧率突破 10 万](#item-8) ⭐️ 8.0/10
9. [用 MicroPython 和 WASM 沙箱化 Python](#item-9) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [谷歌每月向 SpaceX 支付 9.2 亿美元租用 AI 算力](https://www.cnbc.com/2026/06/05/google-to-pay-spacex-920-million-a-month-for-xai-compute-capacity.html) ⭐️ 9.0/10

谷歌签署一项协议，从 2026 年 10 月到 2029 年 6 月每月向 SpaceX 支付 9.2 亿美元，以使用部署在 SpaceX 数据中心内的大约 11 万块 NVIDIA GPU。 两大行业巨头之间的巨额财务承诺凸显了对 GPU 算力的旺盛需求以及 AI 基础设施的战略重要性，可能改变 AI 计算资源的供应方式。 如果 SpaceX 未能在 2026 年 9 月 30 日前交付承诺数量的 GPU，谷歌可以终止协议。该交易旨在满足谷歌 Gemini Enterprise 代理平台超预期的算力需求。

telegram · zaihuapd · Jun 6, 04:15

**背景**: SpaceX 于 2026 年 5 月与 xAI 合并，继承了包括 Colossus 超级计算机和 Grok 聊天机器人等 AI 资产。这是 SpaceX 继 Anthropic 租用其孟菲斯数据中心全部算力后的第二项重大基础设施交易。SpaceX 第一季度资本支出达 101 亿美元，大部分投向 AI 领域，但 AI 业务仍录得 25 亿美元运营亏损。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/XAI_(company)">XAI (company)</a></li>
<li><a href="https://cloud.google.com/gemini-enterprise">Gemini Enterprise app: Best of Google AI for Business</a></li>

</ul>
</details>

**标签**: `#AI`, `#cloud computing`, `#GPU`, `#SpaceX`, `#Google`

---

<a id="item-2"></a>
## [全国首例侵入式脑机接口让失明 20 年患者重见光明](https://www.ithome.com/0/960/883.htm) ⭐️ 9.0/10

中南大学湘雅医院宣布一项侵入式脑机接口视觉重建临床试验取得突破：一名失明 20 年的 61 岁视网膜色素变性患者植入 IMIE 智能视网膜系统后，已能自主辨物、穿行房门，术后视力恢复至 0.03。该系统采用 256 通道柔性电极阵列，通道数是国外同类产品的四倍以上。 这是中国首例侵入式脑机接口成功恢复部分视力的病例，标志着中国在神经假体和脑机接口领域取得重大突破。该技术有望为全球数千万因视网膜疾病失明的患者带来复明希望。 患者术后视力恢复至 0.03，能够分辨物体轮廓和移动。系统通过外部摄像头捕获图像，转化为电刺激信号，无线传输至眼内植入的 256 通道柔性电极阵列，直接刺激视网膜神经细胞，绕过坏死的感光细胞。目前患者仍需持续康复训练以进一步提升视觉感知。

telegram · zaihuapd · Jun 6, 07:30

**背景**: 侵入式脑机接口通过手术将电极植入大脑或视网膜，直接与神经组织交互。视网膜色素变性是一种遗传性致盲疾病，导致感光细胞死亡，但内层视网膜和视神经功能通常完好。IMIE 系统“绕过”坏死的感光细胞，将视觉信号直接传递给视神经。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.chinanews.com/sh/shipin/cns/2020/10-16/news870379.shtml">湖南一医院成功实施智能视觉植入器手术 助失明多年患者重见光明-中新网视频</a></li>
<li><a href="https://www.sohu.com/a/1032751747_100180399">侵入式脑机接口“复明”手术在湘雅医院获重大突破_受试者_视觉_系统</a></li>
<li><a href="https://www.163.com/dy/article/KUOGHI1B0549HWZA.html">盲人福音！盲人凭脑机接口复明成功，是中国首例！机械飞升有望|手术|...</a></li>

</ul>
</details>

**标签**: `#brain-computer interface`, `#neural prosthetics`, `#visual restoration`, `#medical technology`, `#China innovation`

---

<a id="item-3"></a>
## [Ntsc-rs：模拟电视和 VHS 效果的开源工具](https://ntsc.rs/) ⭐️ 8.0/10

Ntsc-rs 是一个新发布的开源库，能够高精度地模拟模拟电视和 VHS 磁带效果，包括 NTSC 彩色编码、扫描线效果和信号噪声。 该工具使开发者和复古爱好者能够在现代软件中真实还原老式视频美学，为游戏、艺术和模拟保留了模拟媒体的视觉特征。它还促进了开源社区对模拟信号处理的深入理解。 该库支持 NTSC 和 PAL 两种标准，能模拟彩色副载波相位偏移和色同步检测失败等细微效果。它专为高性能设计，可集成到游戏模拟器和视频处理等实时应用中。

hackernews · gregsadetsky · Jun 6, 19:17 · [社区讨论](https://news.ycombinator.com/item?id=48428025)

**背景**: NTSC 和 PAL 是分别用于北美和欧洲的模拟电视标准，具有隔行扫描和特定的彩色编码方法。使用这些标准的 VHS 磁带会随时间老化，产生颜色渗色、跟踪误差和噪声等效果。模拟这些效果需要理解复杂的信号处理，包括色度解调和复合视频编码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/NTSC">NTSC - Wikipedia</a></li>
<li><a href="https://www.sony.com/electronics/support/articles/00006681">What are the NTSC, PAL, and SECAM video format standards? | Sony USA</a></li>
<li><a href="https://effect.app/effects/vhs">VHS Effect — Apply VHS to Images & Videos | Effect.app</a></li>

</ul>
</details>

**社区讨论**: 社区成员欣赏关于媒介签名的怀旧引言，并讨论了缺失的特性，如垂直振荡器漂移和 PAL 汉诺威条。一些人分享了他们自己在模拟效果方面的工作，例如像素分离 LED 效果，显示出对这一主题的浓厚兴趣。

**标签**: `#video emulation`, `#analog artifacts`, `#open-source`, `#retro computing`, `#signal processing`

---

<a id="item-4"></a>
## [Unix fork()+exec() 模型面临审视](https://lwn.net/SubscriberLink/1076018/16f01bbbb8e0d1f0/) ⭐️ 8.0/10

LWN.net 上的一篇文章探讨了传统 Unix fork()+exec() 进程创建模型的替代方案，指出了其局限性以及 posix_spawn 和 clone 等潜在替代品。 这一讨论挑战了数十年的操作系统设计，可能带来现代系统中更高效、更安全的进程创建方式，影响系统编程和应用性能。 文章指出，即使采用写时复制，fork() 仍因内存复制而代价高昂，而 posix_spawn 通过避免不必要的复制提供了轻量级替代方案。

hackernews · jwilk · Jun 6, 14:34 · [社区讨论](https://news.ycombinator.com/item?id=48425528)

**背景**: 几十年来，Unix 系统使用 fork() 通过复制父进程创建子进程，然后 exec() 加载新程序。该模型虽然有效，但若子进程立即执行 exec()，内存复制会被浪费，效率低下。替代方案如 posix_spawn 将创建和加载结合，而 Linux 的 clone() 提供了细粒度控制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pubs.opengroup.org/onlinepubs/9799919799/functions/posix_spawn.html">posix _ spawn</a></li>
<li><a href="https://www.man7.org/linux/man-pages/man2/clone.2.html">clone (2) - Linux manual page - man7.org</a></li>

</ul>
</details>

**社区讨论**: 评论者引用了论文《A fork() in the road》，反对使用 fork，并分享了因文件描述符问题导致的真实 bug。有人为 fork 在执行前配置的优雅性辩护，但也有人指出开销仍然很大。

**标签**: `#operating systems`, `#process creation`, `#unix`, `#systems programming`, `#fork`

---

<a id="item-5"></a>
## [Meta AI 聊天机器人漏洞导致 Instagram 账户被接管](https://this.weekinsecurity.com/meta-confirms-thousands-of-instagram-accounts-were-hacked-by-abusing-its-ai-chatbot/) ⭐️ 8.0/10

Meta 确认，由于安全漏洞，攻击者可以利用其 AI 聊天机器人在未经适当电子邮件验证的情况下重置 Instagram 密码，导致 2026 年 4 月 17 日至 6 月期间超过 20,000 个账户遭到入侵。 此次事件突显了一种新型攻击途径——具有账户恢复权限的 AI 聊天机器人可能被操纵，影响数千用户，并引发对 AI 客户支持系统安全性的担忧。 该聊天机器人拥有后端高级权限，可修改电子邮件地址并触发密码重置，且接受自然语言请求而不进行带外身份验证，从而使攻击者能够将自身的电子邮件关联到目标账户。

hackernews · speckx · Jun 6, 18:35 · [社区讨论](https://news.ycombinator.com/item?id=48427643)

**背景**: Meta 的 AI 聊天机器人（称为 Meta AI）被集成到 Instagram 的支持系统中，用于协助账户恢复。通常，密码重置需要验证账户绑定的电子邮件，但一个单独代码路径中的漏洞使得聊天机器人跳过了这一检查。此事件类似提示注入攻击，但涉及后端 API 的滥用，而非对 AI 模型的越狱。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/06/01/hackers-hijacked-instagram-accounts-by-tricking-meta-ai-support-chatbot-into-granting-access/">Hackers hijacked Instagram accounts by tricking Meta AI ...</a></li>
<li><a href="https://cybersecuritynews.com/instagram-meta-ai-vulnerability/">Instagram Meta AI Vulnerability Allegedly Enables Password Reset for Accounts</a></li>
<li><a href="https://blog.checkpoint.com/ai-security/the-meta-ai-account-recovery-incident-wasnt-just-a-chatbot-problem/">The Meta AI Account Recovery Incident Wasn’t Just a Chatbot ...</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Meta 将漏洞描述为“单独代码路径”问题表示怀疑，指出“按预期工作”的说法不准确。许多人震惊于超过 20,000 个账户的规模，并担心账户数据泄露可能导致的隐私侵犯。一些用户分享了因 Meta 自动化系统禁用账户而无法人工申诉的个人经历。

**标签**: `#security`, `#Instagram`, `#Meta`, `#AI chatbot`, `#vulnerability`

---

<a id="item-6"></a>
## [Zeroserve：零配置，用 eBPF 脚本化 Web 服务器](https://su3.io/posts/introducing-zeroserve) ⭐️ 8.0/10

Zeroserve 是一款新的零配置 Web 服务器，利用 eBPF 进行脚本编写，旨在通过基于 eBPF 程序的新型配置范式替代 nginx 和 Caddy 等传统 Web 服务器。 这种方法可以显著简化 Web 服务器配置，并实现 HTTP 请求的高性能内核级处理，可能改变开发者处理服务器设置和性能调优的方式。 Zeroserve 使用 Rust 编写，目前是单线程的，计划通过 SO_REUSEPORT 支持多线程。用户可以编写 C（或最终 Rust）的 eBPF 程序来定义请求处理逻辑。

hackernews · losfair · Jun 6, 14:59 · [社区讨论](https://news.ycombinator.com/item?id=48425723)

**背景**: eBPF（扩展的伯克利包过滤器）是一种 Linux 内核技术，允许在内核空间中安全高效地执行用户定义的程序。传统 Web 服务器如 nginx 使用声明式配置文件；Zeroserve 用 eBPF 脚本替代了这种配置，实现了对网络数据包的直接内核级操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/EBPF">EBPF</a></li>
<li><a href="https://ebpf.io/">eBPF - Introduction, Tutorials & Community Resources</a></li>

</ul>
</details>

**社区讨论**: 评论显示了兴趣但也存在质疑：一位用户注意到 Techempower 基准测试的衰落，但指出了一个新排行榜；另一位称赞 LLM 促成的创新；还有几位讨论了技术细节，如使用 Rust 文件而非 C 编写 eBPF，以及内核加速服务的潜力。

**标签**: `#eBPF`, `#web server`, `#Rust`, `#performance`, `#configuration`

---

<a id="item-7"></a>
## [Nvidia 推出 RTX Spark：面向 Windows PC 的 Arm 统一内存 CPU](https://twitter.com/lemire/status/2062880075117113739) ⭐️ 8.0/10

Nvidia 发布了 RTX Spark 超级芯片，这是一款基于 Arm 架构、采用统一内存设计的 Windows PC 处理器，专为本地 AI 代理和游戏打造。该芯片将于今年晚些时候出现在戴尔、惠普、华硕等品牌的笔记本电脑和迷你主机中。 这标志着 Nvidia 首次进入消费级 PC CPU 市场，在 Windows 生态中挑战 Intel 和 AMD，同时利用统一内存提升 AI 推理和游戏性能。它将直接与 Apple M 系列和 Qualcomm Snapdragon X 系列竞争，可能重塑 PC 市场格局。 RTX Spark 拥有 CPU 和 GPU 共享的统一内存池，组合峰值带宽为专用移动 GPU 的三分之二，总 TDP 也为三分之二。它采用 Arm 指令集，并集成了 Nvidia 的 RTX 图形核心，用于游戏和 AI 工作负载。

hackernews · tosh · Jun 6, 12:52 · [社区讨论](https://news.ycombinator.com/item?id=48424605)

**背景**: 统一内存架构（UMA）允许 CPU 和 GPU 访问同一内存池，无需复制数据，从而降低延迟并提高效率。Apple 的 M 系列芯片在消费设备中普及了这一方案。Nvidia 的 RTX Spark 将类似优势引入 Windows PC，结合了定制的 Arm CPU 和 Nvidia 的 GPU 技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvidianews.nvidia.com/news/nvidia-microsoft-windows-pcs-agents-rtx-spark">NVIDIA and Microsoft Reinvent Windows PCs for the Age of ...</a></li>
<li><a href="https://www.pcmag.com/news/nvidia-rtx-spark-reinvent-pc-computex-2026">Nvidia Unveils RTX Spark, an Arm-Based Superchip for Windows PCs</a></li>
<li><a href="https://www.cnbc.com/2026/05/31/nvidias-new-chip-to-power-fresh-line-of-windows-laptops-by-dell-hp.html">Nvidia's new chip to power fresh line of Windows laptops by ...</a></li>

</ul>
</details>

**社区讨论**: 评论者们就统一内存在游戏和 AI 方面的优劣展开了讨论，有人因带宽共享而质疑其游戏性能，也有人赞赏其对本地 AI 推理的潜力，并指出已上市的 Qualcomm Snapdragon X2 Elite 同样具备统一内存，是强劲对手。

**标签**: `#Nvidia`, `#CPU`, `#Unified Memory`, `#Windows PC`, `#AI`

---

<a id="item-8"></a>
## [宝可梦绿宝石移植到 WebAssembly，帧率突破 10 万](https://pokeemerald.com/) ⭐️ 8.0/10

一款完整的宝可梦绿宝石 WebAssembly 移植版已发布，实现了超过 10 万帧每秒的帧率，并支持保存功能。 这证明了复杂 GBA 游戏可以在浏览器中以极高速度模拟，为高性能复古游戏体验和 WebAssembly 新应用开辟了可能性。 部分 UI 元素显示不正确，例如物品名称位置出现数字；一个社区分支已经在致力于添加音频支持。

hackernews · tripplyons · Jun 6, 11:12 · [社区讨论](https://news.ycombinator.com/item?id=48423762)

**背景**: WebAssembly 是一种低级二进制指令格式，能在现代浏览器中以接近原生的速度运行，最初设计用于在 Web 上实现高性能应用。将宝可梦绿宝石这样的 GBA 游戏移植到 Wasm，需要将游戏的 C 源代码（此前已被反编译）编译为 Wasm 字节码，从而使其无需 JavaScript 模拟开销即可在浏览器中本地运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly - Wikipedia</a></li>
<li><a href="https://webassembly.org/">WebAssembly</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/WebAssembly">WebAssembly - MDN</a></li>

</ul>
</details>

**社区讨论**: 评论者确认保存功能正常，并对性能表示兴奋，同时也报告了显示错误和宝可梦菜单崩溃等 bug。一位用户正在开发支持音频的分支，另一位提到已将 FPS 游戏 Xonotic 移植到 Wasm。

**标签**: `#WebAssembly`, `#GameBoy Advance`, `#emulation`, `#Pokemon`

---

<a id="item-9"></a>
## [用 MicroPython 和 WASM 沙箱化 Python](https://simonwillison.net/2026/Jun/6/micropython-in-a-sandbox/#atom-everything) ⭐️ 8.0/10

Simon Willison 发布了 alpha 包 micropython-wasm，将 MicroPython 编译为 WebAssembly，从而在沙箱中运行 Python 代码。他已将其集成到 Datasette Agent 插件中，实现安全代码执行。 这提供了一个轻量级、受内存和 CPU 限制的沙箱，用于执行不受信任的 Python 代码，有可能在不使用完整操作系统级隔离的情况下，为 Python 应用程序实现更安全的插件系统和代码执行功能。它可以降低来自有缺陷或恶意插件的风险。 该沙箱使用通过 Emscripten 编译为 WebAssembly 的 MicroPython，并作为 Python 包提供，可通过 PyPI 安装并附带二进制 wheel。它施加了内存和 CPU 限制，但当前版本为 alpha，存在已知限制，不应完全信任。

rss · Simon Willison · Jun 6, 03:53

**背景**: MicroPython 是专为微控制器设计的 Python 3 精简实现，而 WebAssembly (WASM) 是一种在沙箱环境中运行的二进制指令格式。将两者结合，可以在限制主机资源访问权限的情况下执行 Python 代码。沙箱化是一种通过限制代码功能（如文件和网络访问）来安全运行不受信任代码的技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://micropython.org/">MicroPython - Python for microcontrollers</a></li>
<li><a href="https://github.com/ciresnave/wasm-sandbox">GitHub - ciresnave/wasm- sandbox : A secure WebAssembly sandbox ...</a></li>
<li><a href="https://agent.datasette.io/">Datasette Agent: an AI assistant for Datasette to help ...</a></li>

</ul>
</details>

**标签**: `#sandbox`, `#Python`, `#WebAssembly`, `#MicroPython`, `#security`

---