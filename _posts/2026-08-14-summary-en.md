---
layout: default
title: "Horizon Summary: 2026-08-14 (EN)"
date: 2026-08-14
lang: en
---

> From 27 items, 11 important content pieces were selected

---

1. [Cerebras and OpenAI's GPT-5.6 Sol Ultrafast Runs HLE 7x Faster](#item-1) ⭐️ 9.0/10
2. [Spaghettifying DRAM Attack Enables Hidden CPU Code Execution](#item-2) ⭐️ 9.0/10
3. [DeepSeek Releases Harness and Open-Sources V4-Pro-0813 Weights](#item-3) ⭐️ 9.0/10
4. [Google Launches Gemini 3.7 Flash, Its New Workhorse LLM](#item-4) ⭐️ 8.0/10
5. [Understanding Becomes the New Bottleneck in LLM-Driven Development](#item-5) ⭐️ 8.0/10
6. [Choose Boring Technology: Spend Limited Innovation Tokens Wisely](#item-6) ⭐️ 8.0/10
7. [Kubernetes on Oxide: Customer Needs Shape New Integrations](#item-7) ⭐️ 8.0/10
8. [Trump Signs Memo Allowing Private Firms to Conduct U.S.-Backed Offensive Cyber Operations](#item-8) ⭐️ 8.0/10
9. [DeepMind SL2T Brings Sign Language-to-Text AI to Pixel 11](#item-9) ⭐️ 8.0/10
10. [Google Unveils Gemini 3.6 Flash, Reveals Gemini 4 Pretraining](#item-10) ⭐️ 8.0/10
11. [X open-sources ranking algorithm, adds tool to check shadowbanning](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Cerebras and OpenAI's GPT-5.6 Sol Ultrafast Runs HLE 7x Faster](https://www.cerebras.ai/blog/accelerating-gpt-5-6-sol-ultrafast-with-openai) ⭐️ 9.0/10

Cerebras and OpenAI announced that GPT-5.6 Sol in Ultrafast mode answered all 2,500 Humanity's Last Exam questions in 11 hours and 11 minutes. This is nearly 7 times faster than Claude Fable 5, which required 78 hours and 27 minutes of continuous compute. This result highlights inference speed as a major competitive frontier in AI, potentially shifting the economic value from model weights to specialized inference hardware. Faster inference enables more iterative reasoning, which can significantly improve output quality and make frontier AI more practical for real-time applications. The benchmark used was Humanity's Last Exam, a dataset of 2,500 expert-crafted questions across over a hundred subjects. Notably, some commenters questioned whether the fast mode delivers exactly the same accuracy as the standard GPT-5.6 Sol, since neither company explicitly confirmed that in their posts.

hackernews · pr337h4m · Aug 13, 18:10 · [Discussion](https://news.ycombinator.com/item?id=49289844)

**Background**: Cerebras builds wafer-scale engines, the world's largest AI processors; its WSE-3 packs 4 trillion transistors and 900,000 AI-optimized cores with 44GB of on-chip SRAM, delivering enormous memory bandwidth for AI workloads. Humanity's Last Exam (HLE) is a frontier benchmark created by the Center for AI Safety and Scale AI, designed to be the final closed-ended academic benchmark with broad subject coverage. Cerebras and OpenAI have been collaborating on making frontier models run at ultra-fast inference speeds.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras_Systems">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Humanity's_Last_Exam">Humanity's Last Exam - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Product - Chip - Cerebras</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive but mixed. Some commenters predict that AI's economic value will shift from model weights to inference hardware, drawing an analogy to operating systems becoming free. Others praise the speed-to-iteration benefit of faster inference, while a few express skepticism about whether Ultrafast mode truly matches standard accuracy, noting that neither Cerebras nor OpenAI explicitly confirmed identical performance.

**Tags**: `#AI`, `#inference`, `#hardware`, `#OpenAI`, `#Cerebras`

---

<a id="item-2"></a>
## [Spaghettifying DRAM Attack Enables Hidden CPU Code Execution](https://github.com/xoreaxeaxeax/skitter-creek-bath-salts) ⭐️ 9.0/10

Security researcher Christopher Domas has released 'Spaghettifying DRAM,' a technique that manipulates the DRAM controller's address translation to scramble physical memory and access hidden processor regions such as the Platform Security Processor, System Management Mode, and CPU microcode. Demonstrated on AMD Family 16h CPUs (e.g., Jaguar), the attack operates below the OS, effectively at ring -1. This research exposes a new class of DRAM exploitation that bypasses all higher-level system protections, undermining hardware trust on affected CPUs. It has far-reaching implications for system security, impacting OS vendors, hardware manufacturers, and users of older AMD processors, and sparks broader concern about hidden hardware privilege levels. The technique uses linear algebra to reconstruct DRAM address mappings, and a single bit flip in the memory controller is enough to unlock hidden regions. According to the GitHub repository, the attack works on AMD Jaguar (2013), while Zen 3 has a different base address for its memory controller registers, leaving the attack's applicability to newer CPUs uncertain.

hackernews · matt_d · Aug 13, 14:17 · [Discussion](https://news.ycombinator.com/item?id=49286341)

**Background**: DRAM controllers translate physical addresses to actual memory locations, and this translation is normally invisible to software. 'Spaghettifying DRAM' exploits the ability to manipulate these translations, effectively rewiring the memory hierarchy to expose hidden regions. The term 'spaghettification' is borrowed from the tidal stretching effect near black holes, used here as a metaphor for scrambling memory. On x86 systems, privilege rings protect the OS (ring 0) from user applications (ring 3), but hypervisors and firmware operate at even higher privileges (ring -1), which is where this attack targets.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/xoreaxeaxeax/skitter-creek-bath-salts">Spaghettifying DRAM</a></li>
<li><a href="https://zeli.app/en/story/49286341">Spaghettifying DRAM: Unlock Everything on the CPU | Zeli</a></li>
<li><a href="https://en.wikipedia.org/wiki/Protection_ring">Protection ring - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong enthusiasm for Christopher Domas' upcoming Black Hat talk, praising his previous reverse engineering and hardware security presentations. Some questioned the attack's relevance to modern CPUs, noting that only AMD Jaguar is confirmed affected and asking about newer processors. Others observed that the growing complexity of DRAM expands the attack surface, and speculated that game console security teams, such as those for Xbox and PlayStation, might be concerned about gaining ring-0 access leading to full system compromise.

**Tags**: `#DRAM`, `#security`, `#hardware exploitation`, `#ring -1`, `#Christopher Domas`

---

<a id="item-3"></a>
## [DeepSeek Releases Harness and Open-Sources V4-Pro-0813 Weights](https://mp.weixin.qq.com/s/mANdGRI4fO_sEbC1ECEoZQ) ⭐️ 9.0/10

DeepSeek has released DeepSeek Harness, an open-source agent harness under the MIT license, and open-sourced the DeepSeek-V4-Pro-0813 model weights on Hugging Face. The harness uses an "everything is a plugin" architecture powered by Cordis, with four runtime modes: Standard, PTC, Minimal, and Creation. This is a milestone update for the open-source AI ecosystem, as DeepSeek not only releases model weights but also an extensible framework for building agent harnesses. The plugin-based design could make it easy for developers to customize every part of an AI agent, from model and tools to scheduling and UI, potentially influencing how agent frameworks are built. The harness became available as a developer preview, with the GitHub repository going live shortly after the initial announcement. The Hugging Face page for the V4-Pro-0813 weights briefly returned a 404 error before being restored. The architecture is powered by Cordis, a metaframework for hot-loading and unloading plugins without restarting a running process.

telegram · zaihuapd · Aug 13, 12:39

**Background**: Agent harnesses are frameworks that connect a language model to tools, memory, and execution environments, acting as the "backbone" of AI agents. DeepSeek Harness treats every capability — models, tools, skills, sessions, sandboxes, storage, loops, scheduling, and UI — as swappable plugins, making the system highly modular. Cordis, the underlying framework, has been used for years in the Koishi project and is designed for spatiotemporal composability, allowing plugin state to be reverted when unloaded.

<details><summary>References</summary>
<ul>
<li><a href="https://deepseek.com/harness/en/">DeepSeek Harness developer preview: Everything is a plugin</a></li>
<li><a href="https://github.com/deepseek-ai/deepseek-harness">GitHub - deepseek-ai/deepseek-harness: DeepSeek Harness ...</a></li>
<li><a href="https://github.com/cordiverse/cordis">GitHub - cordiverse/cordis: Meta-Framework of Spatiotemporal Composability · GitHub</a></li>

</ul>
</details>

**Discussion**: A DeepSeek Harness author acknowledged it is an early developer preview with rough edges and compatibility-breaking changes. Community members highlighted the traceability feature — append-only session logs for every model interaction — as a standout, noting US models keep traces encrypted. Others discussed the underlying Cordis framework and debated whether the heavy reliance on plugins creates "plugin fatigue" for developers.

**Tags**: `#DeepSeek`, `#AI模型`, `#开源`, `#模型权重`, `#工具`

---

<a id="item-4"></a>
## [Google Launches Gemini 3.7 Flash, Its New Workhorse LLM](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-3-7-flash/) ⭐️ 8.0/10

Google has introduced Gemini 3.7 Flash, the latest iteration in its Flash model line, based on Gemini 3.6 Flash and now powering Gemini Spark. The new model offers customizable thinking configurations and notable introductory pricing that is scheduled to rise in 2027. This release reinforces Google's push to offer strong performance at low cost in the competitive LLM market. Developers and enterprises relying on Gemini's Flash series for high-volume, vision-capable tasks will be directly affected by the new price-performance balance. Gemini 3.7 Flash is based on Gemini 3.6 Flash and adds algorithmic improvements to its core reasoning foundation. Its introductory pricing is set to double on December 31, 2026, with input tokens rising to $1.50 per million and output tokens to $7.50 per million starting January 1, 2027.

hackernews · thisisauserid · Aug 13, 17:23 · [Discussion](https://news.ycombinator.com/item?id=49289112)

**Background**: Gemini is a family of multimodal large language models (LLMs) developed by Google DeepMind, spanning Pro, Flash, and other variants. The Flash series is designed as a low-cost, high-volume workhorse for text-based and multimodal tasks such as summarization, parsing, and agentic workflows. Gemini 3.7 Flash continues that tradition while adding vision capabilities and configurable reasoning depth.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/models/model-cards/gemini-3-7-flash/">Gemini 3.7 Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://ai.google.dev/gemini-api/docs/models">Models - Gemini API | Google AI for Developers</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some praise the model’s vision-to-HTML performance relative to its price, while others question the unusual introductory pricing and rapid iteration cadence. Several commenters note that competitors like GPT-5.6 Luna offer better benchmarks and lower cost, undercutting the value proposition of the Flash series.

**Tags**: `#AI`, `#Google`, `#Gemini`, `#LLM`, `#model release`

---

<a id="item-5"></a>
## [Understanding Becomes the New Bottleneck in LLM-Driven Development](https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck) ⭐️ 8.0/10

Geoffrey Litt's essay 'Understanding is the new bottleneck' argues that as LLMs automate code generation, the key constraint in software development shifts from writing code to understanding code and systems. The essay has sparked active discussion on Hacker News with 197 points and 108 comments. This reframing matters because it challenges the assumption that more AI-generated code directly means more productivity. If engineers cannot comprehend the code they ship, review, and maintain, then understanding — not generation — becomes the limiting factor for scale, quality, and safety in software development. The essay centers on the shift in bottleneck: rather than spending effort writing code from scratch, developers now spend effort making sense of LLM-generated code, checking it against system architecture, and updating their mental models. Commenters also warn that relying on LLMs to generate 'understanding' is flawed, because a wrong model cannot reliably verify itself.

hackernews · sebg · Aug 13, 18:47 · [Discussion](https://news.ycombinator.com/item?id=49290299)

**Background**: Large language models (LLMs) can now auto-complete and generate substantial amounts of code, reducing the cost of writing code. However, code must still be reviewed, debugged, extended, and integrated into larger systems, tasks that require a human mental model of how the system behaves. The essay proposes that this human comprehension work is becoming the scarcer resource, and that tools and practices should be redesigned around supporting understanding rather than just generation.

**Discussion**: The discussion largely agrees that understanding was already a bottleneck before LLMs, but several note that LLMs change when understanding happens — moving it from 'frontloaded' (before writing code) to 'backloaded' (after code is generated). Some commenters criticize LLM-generated PR descriptions as mechanical and missing motivation, and warn against using an LLM to generate the very understanding needed to check the LLM.

**Tags**: `#LLMs`, `#software engineering`, `#code comprehension`, `#developer productivity`, `#program management`

---

<a id="item-6"></a>
## [Choose Boring Technology: Spend Limited Innovation Tokens Wisely](https://mcfunley.com/choose-boring-technology) ⭐️ 8.0/10

In this 2015 essay, Dan McKinley argues that engineering teams have a limited supply of "innovation tokens" and should spend them only on technologies that provide real competitive advantage, defaulting to boring, well-understood technology everywhere else. The essay gives engineering leaders a simple mental model for making and explaining technology tradeoffs, which is why it has remained influential for a decade. It is increasingly relevant as teams consider adopting AI agents and must decide where to take on risk. Under the model, "boring" does not mean outdated; it means well-understood and reliable. Each team gets a small fixed number of innovation tokens, and innovative choices cost a token, while boring choices are free.

hackernews · tosh · Aug 13, 17:48 · [Discussion](https://news.ycombinator.com/item?id=49289512)

**Background**: Dan McKinley wrote the essay in 2015 after spending six years as a software engineer at Etsy, where the engineering team was known for high productivity. The essay introduces the idea that every company effectively has a fixed supply of innovation tokens, and that spending them on non-critical tools leaves fewer for the areas that truly matter. The broader "boring technology" movement argues that proven technologies ship faster, break less, and are easier to maintain than trendy alternatives.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/technical-debt-innovation-tokens-case-boring-technology-jeffrey-henry-lhexe">Technical Debt, Innovation Tokens , and the Case for Boring...</a></li>
<li><a href="https://mattrickard.com/innovation-tokens">Innovation Tokens | Matt Rickard</a></li>
<li><a href="https://blog.glyph.im/2024/07/against-innovation-tokens.html">Deciphering Glyph :: Against Innovation Tokens</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised the essay; NickNaraghi called it "one of my favorite blog posts" and said the innovation-token concept is one of the most useful ideas he has had as a PM and engineering leader. theptip suggested that in the age of AI agents, teams should push all their innovation tokens into agents and choose boring, in-distribution technology for everything else. However, insanitybit pushed back, arguing that the innovation-token framing is arbitrary and unserious, and that engineers should evaluate actual risks and tradeoffs rather than rely on novelty as a weak proxy.

**Tags**: `#software engineering`, `#technology strategy`, `#engineering culture`, `#innovation`, `#essay`

---

<a id="item-7"></a>
## [Kubernetes on Oxide: Customer Needs Shape New Integrations](https://oxide.computer/blog/kubernetes-on-oxide) ⭐️ 8.0/10

Oxide Computer published a blog post detailing how customer requirements drove its Kubernetes integration work, including the oxide-cloud-controller-manager and Cluster API-based provisioning. The post explains the design and motivations behind these integrations. This matters because it shows Oxide's rack-scale cloud platform embracing standard Kubernetes ecosystem components, making it easier for enterprises to run Kubernetes workloads on Oxide hardware. The use of Cloud Controller Manager and Cluster API aligns with industry-standard approaches, reducing lock-in. The oxide-cloud-controller-manager is a Kubernetes control plane component that embeds Oxide-specific control logic, allowing clusters to integrate with the Oxide API via the Cloud Controller Manager architecture. Cluster API is a Kubernetes subproject focused on declarative APIs and tooling to simplify provisioning, upgrading, and operating multiple Kubernetes clusters.

hackernews · stevehipwell · Aug 13, 14:26 · [Discussion](https://news.ycombinator.com/item?id=49286485)

**Background**: Oxide Computer builds rack-scale cloud computers that integrate compute, storage, networking, and software into a single platform. Kubernetes is a popular container-orchestration system, and the Cloud Controller Manager is a standard Kubernetes component that allows cloud providers to integrate their APIs. Cluster API is part of the Kubernetes ecosystem that automates cluster lifecycle management.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/oxidecomputer/oxide-cloud-controller-manager">Oxide Cloud Controller Manager - GitHub</a></li>
<li><a href="https://docs.oxide.computer/guides/integrations/cloud-controller-manager">Cloud Controller Manager / Guides / Oxide</a></li>
<li><a href="https://github.com/kubernetes-sigs/cluster-api">GitHub - kubernetes -sigs/ cluster - api : Home for Cluster API ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong interest in the design of oxide-cloud-controller-manager, with one speculating about a karpenter-provider-oxide. Others praised Cluster API, noting its underappreciated role and enterprise-readiness, while some commented on wanting an Oxide rack at home or asking about how Oxide compares to kubevirt on bare metal.

**Tags**: `#Kubernetes`, `#Oxide`, `#Cloud-Controller-Manager`, `#ClusterAPI`, `#Infrastructure`

---

<a id="item-8"></a>
## [Trump Signs Memo Allowing Private Firms to Conduct U.S.-Backed Offensive Cyber Operations](https://www.bloomberg.com/news/articles/2026-08-13/trump-enlists-private-sector-to-boost-cyber-offensive-arsenal) ⭐️ 8.0/10

President Trump signed a memorandum permitting federally supervised private companies to conduct overseas surveillance and cyber attacks on behalf of the U.S. government. The Department of Homeland Security will run the program in coordination with the Department of Justice. This marks a major policy shift that expands the role of the private sector into offensive state-sanctioned cyber operations. It could reshape norms around government surveillance and cybersecurity, raising questions about accountability and the boundaries of corporate involvement in national security. Participating companies must maintain a bond or escrow of at least $1 million, which is forfeited if they fail to comply with contractual terms. The Department of Homeland Security will run the program, with oversight coordinated by the Department of Justice.

telegram · zaihuapd · Aug 13, 05:10

**Background**: Traditionally, offensive cyber operations against foreign criminal groups have been the domain of U.S. intelligence and military agencies. This memorandum appears to extend that authority to private companies, placing them under direct federal control and supervision. The requirement for a $1 million bond indicates a financial accountability mechanism, but the full scope of permissible actions is not detailed in the announcement.

**Tags**: `#cybersecurity`, `#surveillance`, `#policy`, `#private sector`, `#US government`

---

<a id="item-9"></a>
## [DeepMind SL2T Brings Sign Language-to-Text AI to Pixel 11](https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/) ⭐️ 8.0/10

Google DeepMind has introduced SL2T, a massively multilingual sign-language-to-text model, and deployed it in consumer products for the first time via Gboard and Live Transcribe on the Pixel 11. The initial rollout supports American Sign Language to English, with plans to expand to more languages and devices. This is a major accessibility breakthrough, marking the first time sign language AI has been built into everyday consumer devices. It could empower Deaf and hard-of-hearing users to compose messages, search the web, and access live captions using sign language, while also driving broader innovation in accessibility technology and NLP research. The model was trained on more than 100,000 hours of data spanning over 50 sign languages and achieves a zero-shot BLEURT score of 70 on the FLEURS-ASL benchmark, far surpassing previous records. To protect privacy, it processes only hand and body pose keypoints rather than raw video.

telegram · zaihuapd · Aug 13, 08:55

**Background**: Sign language translation is challenging due to the scarcity of large datasets and the inherently visual, continuous nature of signing. FLEURS-ASL extends the FLORES/FLEURS multilingual benchmarks to American Sign Language as video, while BLEURT is a reference-based neural metric that measures how well generated text matches a human-annotated reference. DeepMind's SL2T leverages these resources to train a model capable of zero-shot generalization to unseen sign languages. The on-device deployment demands efficiency, but the pose-keypoint approach helps keep processing lightweight and private.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/blog/putting-sign-language-ai-into-users-hands/">Putting sign language AI into users’ hands — Google DeepMind</a></li>
<li><a href="https://datanorth.ai/news/google-deepmind-releases-sl2t">Google DeepMind releases SL2T sign language AI - DataNorth</a></li>
<li><a href="https://arxiv.org/abs/2408.13585">[2408.13585] FLEURS-ASL: Including American Sign Language in Massively Multilingual Multitask Evaluation</a></li>

</ul>
</details>

**Tags**: `#sign language`, `#AI translation`, `#accessibility`, `#DeepMind`, `#consumer AI`

---

<a id="item-10"></a>
## [Google Unveils Gemini 3.6 Flash, Reveals Gemini 4 Pretraining](https://t.me/zaihuapd/43177) ⭐️ 8.0/10

Google has released Gemini 3.6 Flash, a new model that cuts output tokens by 17% versus Gemini 3.5 Flash while completing multistep tasks with fewer reasoning steps and tool calls. The company also disclosed that pretraining for Gemini 4 has already begun. This release signals Google's continued push to lower LLM inference costs and latency for real-world agents, affecting developers and enterprises building on Gemini APIs. The early disclosure of Gemini 4 pretraining sets expectations for the next major model generation and intensifies competition with OpenAI and Anthropic. The knowledge cutoff for Gemini 3.6 Flash is updated to March 2026, and the API is priced at $1.50 per million input tokens and $7.50 per million output tokens. Google is also offering Gemini 3.5 Flash for high-throughput, low-latency use cases.

telegram · zaihuapd · Aug 13, 17:32

**Background**: Tool calling lets large language models invoke external functions and APIs instead of only generating text, which is essential for automating workflows and performing multistep tasks. A knowledge cutoff defines the point after which a model has no training data, so an updated cutoff like March 2026 means the model has access to more recent information. Computer use refers to AI that interacts with software through the same interface a human uses, such as viewing screenshots and clicking, which Google and other labs are increasingly building into their models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/tool-calling">What Is Tool Calling? | IBM</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_cutoff">Knowledge cutoff - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/news/developing-computer-use">Developing a computer use model \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Google`, `#Gemini`, `#LLM`, `#API`

---

<a id="item-11"></a>
## [X open-sources ranking algorithm, adds tool to check shadowbanning](https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/) ⭐️ 8.0/10

X has expanded its open-source release to include the core 'For You' ranking engine on GitHub under an Apache 2.0 license, with the codebase roughly 10–15 times larger than its previous release. The company also launched a transparency tool in Settings that lets eligible users download a JSON file to check whether their account or posts have been flagged by the ranking system. This move is a significant step toward algorithmic accountability, as it lets users detect whether they have been shadowbanned and understand how content is ranked. However, because not all components are disclosed, the impact on full transparency is limited and may still leave room for criticism. The transparency tool is initially available to test users whose accounts are more than one year old, and who have posted at least 10 times in the past month. Notably, parts of the Grok system used to judge violating content were not open-sourced, and the ranking engine itself uses a transformer model to rank posts.

telegram · zaihuapd · Aug 14, 01:03

**Background**: X's 'For You' feed is powered by a ranking algorithm that filters content based on various inputs and ranks posts using a transformer model, a type of neural network widely used in modern AI. Shadowbanning refers to quietly limiting a user's content visibility without their knowledge, which has long been a source of user concern on social platforms. X previously open-sourced parts of its algorithm in 2023, and this release expands on that effort. Grok is xAI's AI model family, which X has integrated into its platform for content-related processes.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/xai-org/x-algorithm">GitHub - xai-org/x-algorithm: Algorithm powering the For You feed on X · GitHub</a></li>
<li><a href="https://techcrunch.com/2026/08/13/x-open-sources-its-ranking-algorithm-letting-users-see-if-theyve-been-shadowbanned/">X open sources its ranking algorithm, letting users see if they've been 'shadowbanned' | TechCrunch</a></li>
<li><a href="https://adlibrary.com/guides/x-twitter-algorithm-explained">X (Twitter) Algorithm Explained 2026: How For You Ranks Posts</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#algorithm`, `#transparency`, `#social-media`, `#ranking`

---