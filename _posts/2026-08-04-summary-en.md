---
layout: default
title: "Horizon Summary: 2026-08-04 (EN)"
date: 2026-08-04
lang: en
---

> From 27 items, 6 important content pieces were selected

---

1. [OpenAI Highlights Ten AI-Assisted Advances in Mathematics](#item-1) ⭐️ 8.0/10
2. [MiniMax H3 Gets Day-0 ComfyUI Support with Open Weights and 2K Video](#item-2) ⭐️ 8.0/10
3. [Andy Pavlo joins ClickHouse to establish ClickHouse Labs](#item-3) ⭐️ 8.0/10
4. [DNA Analysis Flaw Could Allow Undetected Tampering with 30 Years of Evidence](#item-4) ⭐️ 8.0/10
5. [Nvidia CMP 170HX mining GPU exploit unlocks 80GB VRAM, sparks price surge](#item-5) ⭐️ 8.0/10
6. [UK Renews Demand for Apple Backdoor, Limits to UK Citizen Data](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI Highlights Ten AI-Assisted Advances in Mathematics](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 8.0/10

OpenAI published a post on its website highlighting ten AI-assisted advances in mathematics and theoretical computer science. The announcement has attracted widespread attention and discussion within the research community. This signals that AI is moving beyond routine computation into creative mathematical discovery, which could fundamentally change how research is conducted. Mathematicians and computer scientists will need to adapt to new AI-based tools and collaborative approaches. The post specifically lists ten advances, though the available content did not detail them. The announcement builds on wider industry efforts, including the Leiden Declaration, which mentions OpenAI, Google DeepMind, and Anthropic as key players in AI-assisted mathematical discovery.

hackernews · milkshakes · Aug 3, 16:27 · [Discussion](https://news.ycombinator.com/item?id=49157930)

**Background**: For centuries, mathematical discovery has relied on human intuition, conjecture, and proof. Recently, machine learning and large language models have begun to assist with generating hypotheses and searching for proofs, a field often called machine learning for theorem proving. The existence of tutorials at NeurIPS and ICML, and the recent Leiden Declaration, show how quickly this area is maturing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Leiden_Declaration_on_Artificial_Intelligence_and_Mathematics">Leiden Declaration on Artificial Intelligence and Mathematics</a></li>
<li><a href="https://www.nature.com/articles/s41567-025-03042-0">Mathematical discovery in the age of artificial intelligence</a></li>

</ul>
</details>

**Discussion**: Commenters are largely impressed but vary in their interpretation. Some see progress following an exponential curve, noting that mathematics may be 'consumed' by AI while other fields like writing lag behind. Others question the hype and point to the post's promotion on Hacker News. A recurring theme is concern for human mathematicians, with one commenter quoting Douglas Adams to suggest that many researchers' recent work could be upended by AI grind.

**Tags**: `#AI`, `#mathematics`, `#theoretical computer science`, `#OpenAI`, `#research`

---

<a id="item-2"></a>
## [MiniMax H3 Gets Day-0 ComfyUI Support with Open Weights and 2K Video](https://blog.comfy.org/p/minimax-h3-day-0-support-in-comfyui) ⭐️ 8.0/10

ComfyUI announced Day-0 support for MiniMax H3, an open-weights omni-modal model that generates video with native stereo audio at up to 2K resolution and 15 seconds in length. The integration enables local generation on consumer GPUs, including an RTX 3060 after memory optimizations. This marks a major step for open-weights video generation, bringing a state-of-the-art omni-modal model into ComfyUI's node-based workflow on day one. Hobbyists and professionals alike can run 2K video with audio locally instead of relying on closed APIs, which could accelerate experimentation and creative production. MiniMax H3 accepts mixed text, image, video, and audio inputs in a single request, and supports instruction-based editing that keeps unedited content stable. ComfyUI repackaged model files are available on Hugging Face, and a pruning technique removed roughly 40% of modulation weights to cut total memory from 123.6 GB to as low as 42.5 GB.

hackernews · vblanco · Aug 3, 13:34 · [Discussion](https://news.ycombinator.com/item?id=49155629)

**Background**: MiniMax H3 is a general-purpose omni-modal generation model from MiniMax that jointly understands text, images, video, and audio, generating video with native stereo audio. ComfyUI is an open-source, node-based GUI and backend for building modular diffusion-model workflows, widely used in the AI art and video community. 'Day-0 support' means the integration is available immediately when the model launches, so users can run it in ComfyUI from the first day without waiting for community adapters.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H 3 : An Open Model Breaking the Boundaries Between Tasks...</a></li>
<li><a href="https://huggingface.co/Comfy-Org/MiniMax-H3">Comfy-Org/ MiniMax - H 3 · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/ComfyUI">ComfyUI</a></li>

</ul>
</details>

**Discussion**: Commenters report strong results: one user generated a 10-second 480p clip on a 16 GB RTX 4070 Ti Super in 10 minutes, calling the output 'spectacular,' while another was shocked by how fast and well text-to-video ran. Some observed lingering 'AI smoothing' artifacts in complex shots, and one noted that unusual/parody scenarios still produce jank. Another commenter questioned whether pruning 40% of weights with 'no loss in output quality' could generalize to LLMs.

**Tags**: `#ComfyUI`, `#MiniMax`, `#video generation`, `#open weights`, `#AI/ML`

---

<a id="item-3"></a>
## [Andy Pavlo joins ClickHouse to establish ClickHouse Labs](https://clickhouse.com/blog/andy-pavlo-joins-clickhouse) ⭐️ 8.0/10

Andy Pavlo, a prominent database researcher and Carnegie Mellon professor, is joining ClickHouse to establish ClickHouse Labs, a new database research lab announced on the ClickHouse blog. The move brings a leading academic voice directly into the company's engineering organization. This is significant because it shows a commercial database company investing in fundamental research beyond AI, potentially bridging academic ideas and production systems. It could influence the direction of OLAP architectures, particularly the industry-wide shift toward decoupled compute and storage. ClickHouse is a columnar OLAP database known for highly compressed columnar storage and distributed query processing. Community commentators also noted that competitors like StarRocks and query engines like Trino are converging on decoupled compute/storage models using object storage such as S3.

hackernews · nikolay_sivko · Aug 3, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49156011)

**Background**: OLAP databases are optimized for analytical queries over large datasets, often using columnar storage to improve compression and scan performance. Decoupled compute and storage separates durable storage (like S3) from stateless compute resources, enabling independent scaling and lower costs, but poses challenges for ingestion, indexing, and join execution. ClickHouse has been a major beneficiary of the AI wave, and this lab is a way to give back to fundamental infrastructure research.

<details><summary>References</summary>
<ul>
<li><a href="https://premvishnoi.medium.com/unlocking-the-potential-of-clickhouse-olap-db-architecture-use-cases-and-cost-analysis-56b1aa82bd85">Unlocking the Potential of ClickHouse OLAP DB: Architecture , Use...</a></li>
<li><a href="https://medium.com/@manik.ruet08/decoupling-compute-and-storage-in-modern-data-platforms-0a13f6100613">Decoupling Compute and Storage in Modern Data Platforms | Medium</a></li>
<li><a href="https://clickhouse.com/resources/engineering/unifying-oltp-and-olap">Unifying OLTP and OLAP : HTAP... | ClickHouse Resource Hub</a></li>

</ul>
</details>

**Discussion**: The community reaction was largely positive, with praise for corporate research labs in a non-AI area and hopes that Andy Pavlo's CMU lecture series would continue in a sponsored form. Several commenters raised substantive concerns, including the decline of academic database funding and the technical implications of decoupled compute/storage for ingestion, indexing, and join performance.

**Tags**: `#databases`, `#clickhouse`, `#research`, `#olap`, `#industry-news`

---

<a id="item-4"></a>
## [DNA Analysis Flaw Could Allow Undetected Tampering with 30 Years of Evidence](https://www.wsj.com/tech/cybersecurity/security-flaw-placed-30-years-of-dna-evidence-at-risk-of-hacking-1932775a) ⭐️ 8.0/10

Researchers discovered a vulnerability in DNA analysis devices used by most U.S. crime labs, enabling nearly undetectable tampering with forensic DNA files dating back to 1995. Thermo Fisher Scientific acknowledged the flaw in July and released a security advisory and software update with digital signatures. The vulnerability threatens the integrity of decades of forensic DNA evidence used in criminal investigations and court cases. It highlights the need for stronger security and regulation across the more than 200 U.S. labs that lack uniform standards. The researchers used AI-generated code from Anthropic's Claude to modify DNA scan data; the first tampering attempt took about 45 minutes and evaded common analysis software alerts. The flaw is tracked as CVE-2026-17583 and affects Applied Biosystems DNA files in Thermo Fisher's HID software products.

telegram · zaihuapd · Aug 3, 05:15

**Background**: Forensic DNA analysis relies on specialized instruments and software to produce genetic profiles used in criminal justice. DNA data files are typically created by capillary electrophoresis instruments, and maintaining their integrity is crucial for chain of custody. Digital signatures can help verify that files have not been altered. The company is working with the U.S. Cybersecurity and Infrastructure Security Agency (CISA), and no actual exploitation has been reported.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/thermo-fisher-patches-flaw-that-could.html">Thermo Fisher Patches Flaw That Could Make DNA File Tampering Nearly Undetectable</a></li>
<li><a href="https://cybersecuritynews.com/dna-test-software-vulnerability/">DNA Test Software Vulnerability Allows Attackers to Alter Analysis Data</a></li>
<li><a href="https://www.hindustantimes.com/technology/security-flaw-placed-30-tears-of-dna-evidence-at-risk-of-hacking-101785681888060.html">Security flaw placed 30 tears of DNA evidence at risk of hacking | Technology News (HT Tech)</a></li>

</ul>
</details>

**Tags**: `#cybersecurity`, `#DNA analysis`, `#forensic science`, `#vulnerability`, `#supply chain`

---

<a id="item-5"></a>
## [Nvidia CMP 170HX mining GPU exploit unlocks 80GB VRAM, sparks price surge](https://finance.sina.com.cn/tech/roll/2026-08-03/doc-inikzqsf4659769.shtml) ⭐️ 8.0/10

Researchers at Arizona State University publicly disclosed a stack overflow exploit in the Falcon security coprocessor of Nvidia CMP 170HX mining GPUs. The exploit bypasses OTP fuse locks, expanding VRAM to 80GB and boosting FP32 performance from 0.39 to 94 TFLOPS. This security bypass turns a cheap, low-performance mining card into a capable AI inference accelerator, causing secondary-market prices to jump from 300–500 RMB to 3000–4000 RMB and $1,500 overseas. It demonstrates that Nvidia's hardware locking on GPUs can be reversed, with significant implications for hardware security and AI hardware supply. The exploit targets an unbounded DMA overflow in the Falcon security coprocessor to hijack privileges and modify registers one by one, releasing restrictions on compute, memory, and PCIe. Community validation shows unlocked cards can run AI image generation and LLM inference on Windows and Linux, but long-term stability and per-batch unlock limits remain uncertain.

telegram · zaihuapd · Aug 3, 11:29

**Background**: The CMP 170HX is a dedicated cryptocurrency mining card released by Nvidia in 2021, built on the same GA100 die as the A100 but with OTP fuse-based hardware locks on hashrate, VRAM, and PCIe bandwidth. These one-time-programmable fuses permanently set hardware configurations and were previously considered irreversible; the researchers' stack overflow exploit instead modifies runtime registers to unlock the hardware. The card's full HBM2e memory bus could already rival an A100 in FP32 workloads, making it attractive for AI after the unlock.

<details><summary>References</summary>
<ul>
<li><a href="https://niconiconi.neocities.org/tech-notes/nvidia-cmp-170hx-review/">All GB/s without FLOPS - Nvidia CMP 170HX Review, Performance Lockdown Workaround, Teardown, Watercooling, and Repair</a></li>
<li><a href="https://www.youtube.com/shorts/cIZpgNeolvU">Embedded 101: What Are OTP Fuses? #zephyrrtos #podcast #nvmem - YouTube</a></li>

</ul>
</details>

**Tags**: `#hardware-security`, `#GPU`, `#exploit`, `#AI-inference`, `#Nvidia`

---

<a id="item-6"></a>
## [UK Renews Demand for Apple Backdoor, Limits to UK Citizen Data](https://t.me/zaihuapd/42953) ⭐️ 8.0/10

In early September, the UK Home Office issued a new technical capability notice to Apple, demanding a backdoor into encrypted iCloud backups for UK citizens' data. This follows a January notice that sought global access and triggered a US-UK diplomatic row. This marks the latest escalation in government efforts to mandate encryption backdoors, with significant implications for global privacy and security. Apple's response could set a precedent for how tech firms handle state demands that undermine end-to-end encryption. The new notice is reportedly limited to UK citizens' data, unlike the earlier global demand. Apple had already withdrawn iCloud Advanced Data Protection from the UK in February rather than comply with the prior notice.

telegram · zaihuapd · Aug 3, 15:40

**Background**: The UK's Investigatory Powers Act 2016 allows the Home Office to issue technical capability notices requiring telecoms operators to provide capabilities to intercept data. iCloud Advanced Data Protection is Apple's optional end-to-end encryption feature that protects most iCloud data, including backups, so even Apple cannot access the keys. Opening a backdoor would mean weakening this encryption for law enforcement access.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Investigatory_Powers_Act_2016">Investigatory Powers Act 2016 - Wikipedia</a></li>
<li><a href="https://www.gov.uk/government/publications/investigatory-powers-amendment-bill-factsheets/investigatory-powers-amendment-bill-overview-of-the-notices-regime">Investigatory Powers (Amendment) Bill: Overview of the... - GOV. UK</a></li>
<li><a href="https://support.apple.com/en-us/108756">How to turn on Advanced Data Protection for iCloud - Apple Support</a></li>

</ul>
</details>

**Tags**: `#encryption`, `#privacy`, `#UK government`, `#Apple`, `#backdoor`

---