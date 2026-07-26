---
layout: default
title: "Horizon Summary: 2026-07-26 (EN)"
date: 2026-07-26
lang: en
---

> From 21 items, 6 important content pieces were selected

---

1. [vLLM v0.26.0: Inkling Support and DeepSeek-V4 Optimization](#item-1) ⭐️ 8.0/10
2. [Open-weight AI is having its Kubernetes moment](#item-2) ⭐️ 8.0/10
3. [Android May Soon Restrict On-Device ADB](#item-3) ⭐️ 8.0/10
4. [Ruff v0.16.0 Expands Default Rules from 59 to 413](#item-4) ⭐️ 8.0/10
5. [Musk backs Cook on memory price spike, Micron blames Apple](#item-5) ⭐️ 8.0/10
6. [200 Silicon Valley Companies Oppose Ban on Chinese Open-Weight AI](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [vLLM v0.26.0: Inkling Support and DeepSeek-V4 Optimization](https://github.com/vllm-project/vllm/releases/tag/v0.26.0) ⭐️ 8.0/10

vLLM v0.26.0 is now available, featuring 411 commits from 212 contributors. It adds full support for the Inkling model family, significant performance optimizations for DeepSeek-V4 across vendors, and fp32 precision for lm_head via the head_dtype option. This update strengthens vLLM's position as a leading inference engine by supporting cutting-edge models like Inkling and pushing performance limits for DeepSeek-V4, which directly impacts deployment efficiency and accuracy for production AI systems. The Inkling support includes piecewise CUDA graphs, Hopper FA4 relative attention, MTP=1 speculative decoding, and NVFP4 quantization. DeepSeek-V4 optimizations yield a 2.94% end-to-end TPOT improvement via a specialized routing kernel and a 1.5–2x kernel speedup for fused_topk_bias.

github · khluu · Jul 25, 10:38

**Background**: vLLM is a popular open-source library for fast LLM inference, leveraging techniques like PagedAttention and continuous batching. The Inkling model, from Thinking Machines Lab, is a 975B-parameter MoE transformer with 41B active parameters, supporting text, image, and audio inputs. DeepSeek-V4 is a major LLM from DeepSeek that benefits from the optimizations in this release.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/introducing-inkling/">Inkling: Our Open-Weights Model - Thinking Machines Lab</a></li>
<li><a href="https://vllm.ai/blog/2026-07-15-inkling">TML Inkling on vLLM: Day-0 Support with Optimized Performance | vLLM Blog</a></li>

</ul>
</details>

**Tags**: `#vllm`, `#LLM inference`, `#release`, `#performance optimization`, `#DeepSeek`

---

<a id="item-2"></a>
## [Open-weight AI is having its Kubernetes moment](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

Open-weight AI models are increasingly seen as fundamental infrastructure, akin to Kubernetes, but face challenges in regulation, pricing, and collaborative development. If open-weight models become as ubiquitous as Kubernetes, they could democratize AI access, reduce inference costs, and foster a collaborative ecosystem, impacting startups, enterprises, and geopolitics. The article draws a parallel between the rise of Kubernetes for container orchestration and open-weight AI. Key challenges include the feasibility of banning models by origin, volatile 'tokenomics' pricing, and the need for collaborative model development akin to Linux.

hackernews · tknaup · Jul 25, 14:49 · [Discussion](https://news.ycombinator.com/item?id=49048034)

**Background**: Open-weight AI models make model parameters (weights) downloadable, allowing users to run and customize them, similar to Meta's Llama. This contrasts with fully open-source AI which also includes training code and data. Kubernetes is an open-source container orchestration platform that became the industry standard through community collaboration.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>
<li><a href="https://biz.chosun.com/en/en-it/2025/08/06/YNGJCP3ISNEUTGFKBXDS4OXY3I/">OpenAI launches open - weight AI models to enhance... - CHOSUNBIZ</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tokenomics">Tokenomics - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters debated the feasibility of banning Chinese open-weight models, with ozgung arguing it's impossible because weights are just numbers without country of origin. firasd criticized 'tokenomics' pricing volatility, while pianopatrick suggested that like Kubernetes, an AI model needs public training data and corporate collaboration to succeed.

**Tags**: `#open-weight AI`, `#Kubernetes analogy`, `#AI regulation`, `#tokenomics`, `#open source`

---

<a id="item-3"></a>
## [Android May Soon Restrict On-Device ADB](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 8.0/10

Android may soon restrict on-device ADB (Android Debug Bridge) usage, requiring users to connect via USB or wireless ADB from a computer instead of running ADB directly on the device. This change would impact developers and power users who rely on on-device ADB for debugging and sideloading apps, potentially increasing security but reducing flexibility on Android devices. The attack vector requires both enabling developer settings and enabling remote ADB, making it unrealistic for 99.9% of users, yet Google is still considering restrictions. The proposal also includes restricting access to certain IP addresses or interfaces.

hackernews · shscs911 · Jul 25, 06:57 · [Discussion](https://news.ycombinator.com/item?id=49045159)

**Background**: Android Debug Bridge (ADB) is a command-line tool that allows developers to communicate with Android devices for debugging, installing apps, and accessing a Unix shell. On-device ADB lets users run ADB commands directly on the device without a computer, which can be convenient but also poses a security risk if malicious apps gain access.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Android_Debug_Bridge">Android Debug Bridge - Wikipedia</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>
<li><a href="https://help.esper.io/hc/en-us/articles/12657625935761-Installing-the-Android-Debug-Bridge-ADB-Tool">Installing the Android Debug Bridge (ADB) Tool – Esper Help</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions: some argue the attack vector is too niche to justify restrictions, while others see it as an inevitable step toward locking down Android, comparing it to past sideloading restrictions. There is concern that Google's mindset is shifting away from openness, and technological workarounds may not help.

**Tags**: `#Android`, `#ADB`, `#Developer Tools`, `#Security`

---

<a id="item-4"></a>
## [Ruff v0.16.0 Expands Default Rules from 59 to 413](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0 was released on July 23, 2026, increasing the number of default rules from 59 to 413, causing immediate CI failures for projects with unpinned ruff dependencies. This dramatic expansion of default rules means many Python projects will now detect hundreds of previously unnoticed issues, significantly improving code quality and catching potential bugs early. It also breaks CI pipelines that use unpinned dependencies, forcing developers to either pin versions or update their code. The update brings the total number of rules from 708 to 968, with many new rules targeting syntax errors and runtime errors that were previously not enabled by default. The release includes tools like `ruff check --fix --unsafe-fixes` to help automatically resolve many of the new issues.

rss · Simon Willison · Jul 25, 22:44

**Background**: Ruff is an extremely fast Python linter and code formatter written in Rust, offering over 900 built-in rules with native re-implementations of popular Flake8 plugins. An 'unpinned dependency' means the version of a package (like ruff) is not exactly specified, so an upgrade like this automatically takes effect on the next install, which can cause unexpected CI failures when breaking changes are introduced.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/ruff/">Ruff</a></li>
<li><a href="https://github.com/astral-sh/ruff">GitHub - astral-sh/ruff: An extremely fast Python linter and code formatter, written in Rust. · GitHub</a></li>

</ul>
</details>

**Tags**: `#ruff`, `#python`, `#linting`, `#breaking changes`

---

<a id="item-5"></a>
## [Musk backs Cook on memory price spike, Micron blames Apple](https://t.me/zaihuapd/42761) ⭐️ 8.0/10

Elon Musk reposted Tim Cook's comments about unprecedented memory price increases, calling it the largest price rise he has ever seen. Musk advocated for massively increasing production and tied it to his Tesla Terafab project, while Micron's CCO suggested that Apple's aggressive supply chain pricing during the 2023 downturn contributed to the current shortage. This highlights a major supply chain tension in the memory industry, where aggressive buyer behavior can lead to long-term capacity shortages. The involvement of major figures like Musk and Cook signals that memory pricing is a critical issue for tech giants, potentially impacting product costs and availability. Musk specifically mentioned his Tesla Terafab chip factory project, which aims to integrate multiple memory upstream and downstream facilities in one campus. Micron CCO Sadana told the Wall Street Journal that during the 2023 downturn, some customers pressured prices so hard that Micron's profits turned negative, preventing investment in capacity expansion.

telegram · zaihuapd · Jul 25, 04:02

**Background**: Memory prices have experienced cyclical fluctuations, but the recent surge has been described as unprecedented. Tesla's Terafab is a planned $20 billion semiconductor fabrication facility in Austin, Texas, aimed at producing advanced AI chips for Tesla's products, including Cybercab and Optimus robots. The project was first teased in early 2026 and officially announced in March 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Terafab">Terafab - Wikipedia</a></li>
<li><a href="https://electrek.co/2026/06/30/tesla-intel-veteran-terafab-director/">Tesla poaches 17-year Intel veteran to lead its 'Terafab' chip plant | Electrek</a></li>

</ul>
</details>

**Tags**: `#memory`, `#supply chain`, `#Apple`, `#Elon Musk`, `#industry trends`

---

<a id="item-6"></a>
## [200 Silicon Valley Companies Oppose Ban on Chinese Open-Weight AI](https://t.me/zaihuapd/42772) ⭐️ 8.0/10

Nearly 200 Silicon Valley companies, including Proton and Y Combinator, have sent a letter to the Trump administration urging it not to ban Chinese open-weight AI models, warning that such a ban would harm U.S. startups. This coordinated opposition highlights the deep reliance of Silicon Valley startups on cost-effective Chinese AI models, and a ban could severely impact U.S. competitiveness in the AI ecosystem. The letter was organized by the Little Tech Association, which argues that a blanket ban would crush next-generation U.S. startups, while targeted security measures are a better alternative.

telegram · zaihuapd · Jul 26, 02:00

**Background**: Open-weight AI models release the trained neural network weights, allowing users to host, fine-tune, and deploy the model without relying on a cloud API. Unlike fully open-source models, open-weight models may withhold training data and code. Chinese open-weight models like those from DeepSeek and Alibaba are widely used by Silicon Valley startups for their low cost and customizability.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>
<li><a href="https://engineadvocacyfoundation.medium.com/ai-essentials-what-are-model-weights-2e5b47ec77a1">AI Essentials: What are model weights? | by Engine | Medium</a></li>

</ul>
</details>

**Tags**: `#AI policy`, `#US-China relations`, `#open-weight AI`, `#Silicon Valley`, `#startups`

---