---
layout: default
title: "Horizon Summary: 2026-06-15 (EN)"
date: 2026-06-15
lang: en
---

> From 25 items, 8 important content pieces were selected

---

1. [Gary Bernhardt's 2014 Talk Predicted JavaScript's Evolution](#item-1) ⭐️ 9.0/10
2. [Kobo Rejects Valid ePubs Due to Adobe RMSDK](#item-2) ⭐️ 8.0/10
3. [Rio's 'homegrown' LLM exposed as weighted merge](#item-3) ⭐️ 8.0/10
4. [Formal methods: Jane Street examines verification future](#item-4) ⭐️ 8.0/10
5. [Linux kernel 7.1 released with WiFi fix, new NTFS driver, old driver removals](#item-5) ⭐️ 8.0/10
6. [Why AI hasn't replaced software engineers yet](#item-6) ⭐️ 8.0/10
7. [Huawei Open-Sources Pangu 2.0 with Up to 505B Parameters](#item-7) ⭐️ 8.0/10
8. [US government orders Anthropic to block Mythos AI models](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Gary Bernhardt's 2014 Talk Predicted JavaScript's Evolution](https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript) ⭐️ 9.0/10

Gary Bernhardt's 2014 talk 'The Birth and Death of JavaScript' humorously predicted that JavaScript would become a universal compilation target and eventually be replaced by a better low-level language. This prediction has proven remarkably prescient with the rise of TypeScript and the advent of WebAssembly. The talk accurately forecasted major trends in web development, such as the emergence of compilation-to-JavaScript languages and the need for a performant low-level target. Its insights continue to influence how developers think about JavaScript's role and the future of web application performance. Delivered in 2014, the talk specifically referenced asm.js as a stepping stone toward a universal compilation target, which later influenced the development of WebAssembly. The talk also humorously predicted a global disaster between 2020-2025, though it got the type wrong.

hackernews · subset · Jun 14, 12:38 · [Discussion](https://news.ycombinator.com/item?id=48526661)

**Background**: A compilation target is a language or format that compilers translate source code into. Historically, JavaScript was only a source language until asm.js, a subset of JavaScript, emerged as a compilation target for C/C++ programs. WebAssembly (Wasm) is a low-level binary instruction format designed as a portable compilation target, enabling high-performance applications on web pages and beyond. It was announced in 2015 and first released in 2017, becoming a W3C recommendation in 2019.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Compiler">Compiler - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>

</ul>
</details>

**Discussion**: Commenters widely praise the talk's prescience, noting its accurate prediction of JavaScript's evolution and the rise of WebAssembly. Some reference the author's famous 'Wat' talk, and one comment humorously notes that 'every few years we invent a better JavaScript, then we transpile it to JavaScript.'

**Tags**: `#JavaScript`, `#programming languages`, `#compilation target`, `#Gary Bernhardt`, `#web development`

---

<a id="item-2"></a>
## [Kobo Rejects Valid ePubs Due to Adobe RMSDK](https://andreklein.net/your-epub-is-fine-kobo-disagrees-blame-adobe/) ⭐️ 8.0/10

The article reveals that ePubs passing validation are still rejected by Kobo devices because Adobe's RMSDK imposes stricter, opaque requirements beyond the EPUB standard, causing incompatibility despite standards compliance. This exposes a widespread compatibility problem in the ebook ecosystem, forcing publishers and developers to work around proprietary software like Adobe RMSDK, undermining the promise of open standards such as EPUB. Kobo uses Adobe's RMSDK for rendering, which has undocumented requirements beyond EPUB validation; community workarounds like kepubify can convert files to Kobo's own format to bypass the issue.

hackernews · sohkamyung · Jun 14, 22:54 · [Discussion](https://news.ycombinator.com/item?id=48533848)

**Background**: EPUB is a standard format for ebooks, with validation tools like epubcheck to ensure compliance. However, device manufacturers often implement proprietary rendering engines; Kobo uses Adobe's RMSDK, which adds extra constraints, leading to rejections of technically valid ePubs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.adobe.com/in/solutions/ebook/rmsdk/faq.html">Solutions - Ebook - rmsdk - FAQs</a></li>
<li><a href="https://medium.com/@jiminypan/five-interesting-facts-about-adobe-legacy-ebook-rmsdk-b7be0123c874">Five interesting facts about Adobe legacy eBook RMSDK | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters share frustrations with Adobe's poor QA and lack of support for RMSDK, noting that even indie developers cannot obtain access. Some suggest alternatives like PineNote or using kepubify to convert files, while others criticize the EPUB spec's reliance on living standards.

**Tags**: `#epub`, `#adobe`, `#kobo`, `#ebooks`, `#drm`

---

<a id="item-3"></a>
## [Rio's 'homegrown' LLM exposed as weighted merge](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

A community investigation revealed that the Rio-3.5-Open-397B model released by the municipality of Rio de Janeiro is actually a weighted merge of approximately 60% Nex-N2 Pro and 40% Qwen3.5-397B-A17B, rather than a fine-tuned homegrown model. This controversy highlights growing concerns about transparency and attribution in open-source AI development, especially when public entities claim credit for model creation without proper disclosure. Every weight tensor in the Rio model matches a 0.6/0.4 blend of Nex and Qwen across all 60 layers, with no evidence of additional fine-tuning or distillation.

hackernews · unrvl22 · Jun 14, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48528371)

**Background**: Model merging is a technique that combines weights from multiple fine-tuned models sharing the same base architecture, enabling a single model to inherit capabilities from all source models without additional training. Common methods include weighted averaging, SLERP, and TIES-Merging.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-model-merging-for-llms/">An Introduction to Model Merging for LLMs | NVIDIA Technical Blog</a></li>
<li><a href="https://www.linkedin.com/posts/tanveer-m-a13016a9_the-4-model-merging-techniques-how-to-combine-activity-7436097234850570241-JP8N">Model Merging : Combining Fine-Tuned AI Models for... | LinkedIn</a></li>

</ul>
</details>

**Discussion**: Commenters expressed disappointment and raised ethical concerns about profiting from others' work without attribution. Some speculated that the claimed distillation might not have been included in the uploaded model, causing confusion.

**Tags**: `#AI`, `#LLM`, `#open-source`, `#ethics`, `#model merging`

---

<a id="item-4"></a>
## [Formal methods: Jane Street examines verification future](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 8.0/10

Jane Street published an article on formal methods in programming, highlighting their growing importance and exploring historical tools like SAT solvers and the Boyer-Moore prover, as well as future implications including AI-assisted verification. As AI generates increasing amounts of code, shifting human effort from writing to verification becomes critical, and formal methods provide a rigorous mathematical foundation for ensuring correctness. The article references early work with the Oppen-Nelson simplifier and the Boyer-Moore prover, and discusses modern approaches like expressive type systems in Scala 3 that carry compile-time proofs.

hackernews · eatonphil · Jun 14, 12:35 · [Discussion](https://news.ycombinator.com/item?id=48526633)

**Background**: Formal methods are mathematical techniques for specifying and verifying software correctness. They use formal languages to describe system behavior and automated theorem provers or model checkers to prove properties. The field has evolved from manual proofs to modern SMT solvers that automate much of the verification process.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Formal_methods">Formal methods - Wikipedia</a></li>
<li><a href="https://web.mit.edu/16.35/www/lecturenotes/FormalMethods.pdf">Introducing Formal Methods - MIT</a></li>
<li><a href="https://www.microsoft.com/en-us/research/project/trusted-ai-assisted-programming/">Trusted AI-assisted Programming - Microsoft Research dafny-annotator: AI-Assisted Verification for Dafny The "Trust, But Verify" Pattern For AI-Assisted Engineering A Toolchain for AI-Assisted Code Specification, Synthesis and ... Towards AI-Assisted Synthesis of Verified Dafny Methods</a></li>

</ul>
</details>

**Discussion**: Community comments reflect diverse experiences: one user recalls early proof-of-correctness work with SAT solvers and the Boyer-Moore prover, while another discusses using expressive types in Scala 3 for compile-time proofs. Some express skepticism that formal specs just duplicate tests or implementation, while others highlight the challenge of AI code generation shifting human value to verification.

**Tags**: `#formal methods`, `#programming`, `#verification`, `#types`, `#software engineering`

---

<a id="item-5"></a>
## [Linux kernel 7.1 released with WiFi fix, new NTFS driver, old driver removals](https://lore.kernel.org/lkml/CAHk-=wi4BF4bMhZNZ1tqs+FFV4OuZRe3ZqdWB+LxRLmRweUzQw@mail.gmail.com/T/#u) ⭐️ 8.0/10

Linux kernel 7.1 has been released, featuring a fix for slow WiFi, a new NTFS driver, and the removal of obsolete drivers (ISDN, ham radio, ATM) motivated by AI-assisted bug report spam. This release demonstrates how AI is reshaping kernel maintenance by forcing the removal of rarely-used code to manage AI-generated bug reports, and provides better hardware support with a new NTFS driver and WiFi fix. The removal commit by Jakub Kicinski deletes 138,161 lines of code. The new NTFS driver replaces the previous ntfs3 driver from Paragon, aiming for better stability and performance.

hackernews · berlianta · Jun 14, 16:01 · [Discussion](https://news.ycombinator.com/item?id=48528729)

**Background**: Linux kernel versioning increments the major number (e.g., 7.1) after enough minor releases. AI-generated bug reports, especially from LLMs, have increased, causing maintainers to consider removing old subsystems to reduce the reporting burden.

<details><summary>References</summary>
<ul>
<li><a href="https://devtake.dev/article/linux-7-1-ham-radio-isdn-removal/">Linux 7.1 is yanking ham radio, ISDN, and ATM. The reason: AI …</a></li>
<li><a href="https://www.theregister.com/2026/03/26/greg_kroahhartman_ai_kernel/">Linux kernel czar says AI bug reports aren't slop anymore</a></li>
<li><a href="https://linux.slashdot.org/story/26/05/23/2041253/linus-torvalds-on-how-ai-is-impacting-the-hunt-for-linux-kernel-bugs">Linus Torvalds on How AI is Impacting the Hunt for Linux Kernel Bugs</a></li>

</ul>
</details>

**Discussion**: Community members expressed excitement about the WiFi fix and the new NTFS driver. Some praised the removal of old drivers as a positive consequence of AI bug reports, calling it 'trimming the fat'. Others noted that version 7.1 is just a normal increment and not particularly special.

**Tags**: `#Linux`, `#kernel`, `#open source`, `#AI`, `#bug reporting`

---

<a id="item-6"></a>
## [Why AI hasn't replaced software engineers yet](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan and Sayash Kapoor published an essay arguing that AI will not cause mass layoffs among software engineers, citing that no AI-related layoffs were reported in New York's first year of WARN Act disclosures. This challenges the prevailing narrative that AI will soon automate software engineering jobs, suggesting that the profession's core value lies in deep human understanding, not just code generation. The essay identifies three real bottlenecks in software engineering: deciding what to build, verifying delivered work, and the deep human understanding required for both. It notes that AI speeds up typing code but not these essential tasks.

rss · Simon Willison · Jun 14, 23:54

**Background**: The WARN Act (Worker Adjustment and Retraining Notification Act) requires U.S. employers to provide 60-day notice of mass layoffs. New York added an AI disclosure checkbox in March 2025. Software engineering involves far more than writing code—it requires understanding business needs, debugging, and communication.

**Tags**: `#AI`, `#software engineering`, `#job displacement`, `#labor market`, `#technology`

---

<a id="item-7"></a>
## [Huawei Open-Sources Pangu 2.0 with Up to 505B Parameters](https://t.me/zaihuapd/41948) ⭐️ 8.0/10

At the 2026 Huawei Developer Conference, Huawei released the open-source Pangu 2.0 model (openPangu 2.0), including a 505B-parameter Pro version and a 92B-parameter Flash version, both supporting a 512K context window. The company plans to open-source seven major components starting June 30. This significant open-source release of a large language model with competitive specs from a major Chinese tech company could accelerate AI development on Huawei's Ascend ecosystem and challenge global leaders. It also signals Huawei's commitment to open-source AI despite limited compute resources for internal use. The 505B-parameter Pro version and 92B Flash version both support a 512K token context window, placing them among the top-tier long-context models. The open-source release includes seven components such as pre-training code, and is optimized for Ascend computing power and HarmonyOS.

telegram · zaihuapd · Jun 14, 08:05

**Background**: Huawei's Ascend 950PR chip has become the primary AI chip for Chinese tech companies, replacing Nvidia's market share in China. Large language models with 512K context windows are increasingly common, with over a dozen models now supporting 1 million tokens or more. Huawei first released the Pangu model years ago when LLMs were still nascent.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huaweicentral.com/ascend-950pr-ai-chip-everything-you-need-to-know/">Ascend 950PR AI Chip: Everything you need to know - Huawei Central</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/huawei-expects-12-billion-in-ai-chip-revenue-this-year-as-nvidias-china-market-share-hits-zero">Huawei braces for $12 billion in AI chip revenue driven by homegrown AI model demand — Chinese fabs can barely keep up as Nvidia's market share craters within the region | Tom's Hardware</a></li>
<li><a href="https://www.morphllm.com/llm-context-window-comparison">LLM Context Window Comparison (2026): 20 Models From 200K to ...</a></li>

</ul>
</details>

**Discussion**: Community discussion from the Telegram source is limited, but the announcement has generated interest due to the competitive specs and open-source nature, though some may question the actual availability and performance on Ascend hardware.

**Tags**: `#open-source`, `#large language model`, `#Huawei`, `#Pangu`, `#AI`

---

<a id="item-8"></a>
## [US government orders Anthropic to block Mythos AI models](https://t.me/zaihuapd/41949) ⭐️ 8.0/10

The US Commerce Department, citing national security authorities, issued an export control directive ordering Anthropic to block access to its Fable 5 and Mythos 5 AI models for all customers, including foreign employees. Anthropic has complied by shutting down access to these two models while stating that other Claude models remain unaffected. This marks a significant escalation in US government intervention in AI model distribution, directly targeting advanced models that could pose national security risks if misused. It sets a precedent for export controls on AI model weights and may influence global AI regulation and the competitive landscape for frontier AI companies. The directive was triggered by concerns that the models could be jailbroken to bypass safety guardrails, posing risks in areas like cybersecurity and biology. Anthropic had previously released Fable 5 as a safer, publicly accessible version of Mythos 5, but the government ordered access blocked for both models entirely.

telegram · zaihuapd · Jun 14, 09:06

**Background**: Anthropic's Mythos models are highly capable AI systems that outperform humans in certain tasks, but they also pose potential safety risks. The US government has been tightening export controls on advanced AI technologies, particularly to prevent adversaries from accessing sensitive model weights. This action is part of a broader regulatory effort to balance AI innovation with national security, as seen in recent updates to the Entity List and export control policies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/mythos">Claude Mythos \ Anthropic</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/United_States_export_controls_on_AI_chips_and_semiconductors">United States export controls on AI chips and semiconductors</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#export controls`, `#national security`, `#Anthropic`, `#AI policy`

---