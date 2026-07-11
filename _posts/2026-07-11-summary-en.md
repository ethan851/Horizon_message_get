---
layout: default
title: "Horizon Summary: 2026-07-11 (EN)"
date: 2026-07-11
lang: en
---

> From 29 items, 11 important content pieces were selected

---

1. [Apple sues OpenAI over trade secret theft](#item-1) ⭐️ 9.0/10
2. [China's Long March 10B achieves world-first net-based sea recovery](#item-2) ⭐️ 9.0/10
3. [SGLang v0.5.15: 500+ tok/s/user for GLM-5.2 on Blackwell](#item-3) ⭐️ 8.0/10
4. [QuadRF: Open-Source RF Camera Visualizes WiFi and Drones](#item-4) ⭐️ 8.0/10
5. [GPT-5.6 Sol Ultra Claims Proof of Cycle Double Cover Conjecture](#item-5) ⭐️ 8.0/10
6. [New York City Bans Deceptive Subscription Practices](#item-6) ⭐️ 8.0/10
7. [Tencent in talks to acquire AI startup Manus from Meta](#item-7) ⭐️ 8.0/10
8. [OpenAI, Google Supply AI Models to Blacklisted Chinese Firms](#item-8) ⭐️ 8.0/10
9. [China Imposes Temporary Ban on Helium Exports](#item-9) ⭐️ 8.0/10
10. [Meta Faces $12B EU Fine Over Addictive Design](#item-10) ⭐️ 8.0/10
11. [SK Hynix CEO Warns of Worst Memory Shortage by 2027](#item-11) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Apple sues OpenAI over trade secret theft](https://9to5mac.com/2026/07/10/apple-sues-openai-trade-secret-theft/) ⭐️ 9.0/10

Apple filed a lawsuit accusing OpenAI of orchestrating a scheme to steal trade secrets through former employees, including directing candidates to bring actual Apple parts to interviews. This lawsuit could have major implications for the AI industry, highlighting the fierce competition for talent and intellectual property between tech giants. It also raises questions about OpenAI's ethics and could affect enterprise adoption of its products. Apple claims OpenAI instructed new hires not to notify Apple of their departure and used confidential hardware information to approach Apple suppliers. The lawsuit is backed by detailed evidence.

hackernews · stock_toaster · Jul 10, 20:47 · [Discussion](https://news.ycombinator.com/item?id=48865019)

**Background**: Trade secrets are confidential business information that gives a competitive advantage. Apple heavily invests in R&D and protects its product designs. Lawsuits over trade secret theft are common in Silicon Valley, especially when employees move between companies.

**Discussion**: Community comments express strong condemnation of OpenAI, with many users calling the evidence damning and predicting severe legal consequences. Some highlight the irony of OpenAI, which has faced allegations of content scraping, now being accused of theft itself.

**Tags**: `#Apple`, `#OpenAI`, `#trade secrets`, `#lawsuit`, `#corporate espionage`

---

<a id="item-2"></a>
## [China's Long March 10B achieves world-first net-based sea recovery](https://weibo.com/7340734455/R814of1Ki) ⭐️ 9.0/10

On July 10, 2026, China's Long March 10B rocket launched from Hainan Commercial Space Launch Site and successfully recovered its first stage at sea using a net-based system, marking the world's first net-based rocket recovery. This breakthrough significantly advances reusable rocket technology, reducing launch costs and increasing payload capacity, positioning China as a leader in rocket recovery alongside SpaceX. The net-based recovery uses pulley-driven cables to capture the first stage, simplifying onboard structure and reducing vehicle mass. Unlike traditional propulsive landing, this method does not require landing legs, saving weight.

telegram · zaihuapd · Jul 10, 04:36

**Background**: Rocket recovery is key to reusable launch systems, lowering the cost per launch by reusing expensive components. Previously, SpaceX's Falcon 9 used propulsive landing on droneships, while China's Long March 10B introduces a net capture method. The Long March 10B is a variant of the Long March 10 family, designed for crewed lunar missions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Long_March_10B">Long March 10B - Wikipedia</a></li>
<li><a href="https://www.globaltimes.cn/page/202607/1365624.shtml?id=12">China enters rocket recovery era as experts highlight... - Global Times</a></li>
<li><a href="https://www.youtube.com/watch?v=2D_GstQJp0U">World's first : China recovers rocket booster with net system at sea ...</a></li>

</ul>
</details>

**Tags**: `#rocket recovery`, `#aerospace`, `#long march 10b`, `#space technology`, `#china`

---

<a id="item-3"></a>
## [SGLang v0.5.15: 500+ tok/s/user for GLM-5.2 on Blackwell](https://github.com/sgl-project/sglang/releases/tag/v0.5.15) ⭐️ 8.0/10

SGLang v0.5.15 delivers optimized production serving for GLM-5.2 NVFP4 on Blackwell GPUs, achieving over 500 tokens per second per user on 8x B300. The release also introduces Spec V2 speculative decoding as default, IndexShare MTP optimizations, and support for new models like Hunyuan 3 and Qwen3.6. These performance gains make SGLang a compelling solution for serving large language models at scale, particularly for GLM-5.2 agents and long-context applications. The Spec V2 and IndexShare optimizations reduce latency and improve throughput, benefiting production deployments with lower costs and faster responses. Spec V2 achieves an 11% end-to-end throughput increase through zero-overhead scheduling and fused operations. IndexShare MTP reduces draft-step cost by up to 1.9x at long context by reusing the indexer top-k across draft steps. The release also enables breakable CUDA Graph by default and introduces linear-attention kernels for KDA and GDN.

github · Fridge003 · Jul 10, 22:58

**Background**: SGLang is an open-source inference framework for large language models. Speculative decoding accelerates generation by using a faster draft model to propose tokens that are then verified by the target model. NVFP4 is NVIDIA's 4-bit floating-point precision format that balances efficiency and accuracy. Blackwell refers to NVIDIA's next-generation GPU architecture (e.g., B300). IndexShare is a cross-layer reuse technique for sparse attention that reduces computation.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2211.17192">Fast Inference from Transformers via Speculative Decoding</a></li>
<li><a href="https://sebastianraschka.com/blog/2026/glm-5-2-indexshare.html">GLM-5.2 IndexShare Architecture Note | Sebastian Raschka, PhD</a></li>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision Inference | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Tags**: `#SGLang`, `#GPU inference`, `#speculative decoding`, `#production serving`, `#Blackwell`

---

<a id="item-4"></a>
## [QuadRF: Open-Source RF Camera Visualizes WiFi and Drones](https://www.jeffgeerling.com/blog/2026/quadrf-can-spot-drones-and-see-wifi-through-my-wall/) ⭐️ 8.0/10

QuadRF, an open-source modular 4x4 MIMO software-defined radio tile with an integrated Raspberry Pi 5, was demonstrated as an RF camera that can detect drones and map WiFi signals through walls. This tool democratizes phased array RF sensing, making advanced surveillance and spectrum monitoring accessible to hobbyists, security researchers, and educators, potentially increasing awareness of wireless privacy and security. QuadRF operates as a real-time RF camera with color-coded frequency visualization, identifying physical locations of transmitters like WiFi access points and drones. It is powered by a Raspberry Pi 5 and uses an open antenna architecture.

hackernews · speckx · Jul 10, 15:59 · [Discussion](https://news.ycombinator.com/item?id=48861717)

**Background**: Software-defined radio (SDR) is a radio communication system where traditionally analog components like mixers and filters are implemented via software. QuadRF extends SDR with phased array technology, using multiple antennas to spatially resolve signal sources. The open-source nature allows users to customize the UI and processing.

<details><summary>References</summary>
<ul>
<li><a href="https://www.crowdsupply.com/scale-rf/quadrf">QuadRF | Crowd Supply</a></li>
<li><a href="https://github.com/dustinbowers/QuadRF">GitHub - dustinbowers/QuadRF</a></li>
<li><a href="https://www.hackster.io/news/quadrf-the-open-source-rf-camera-that-lets-you-see-wi-fi-signals-141ad91f2a2d">QuadRF: The Open Source RF Camera That Lets You See Wi-Fi Signals</a></li>

</ul>
</details>

**Discussion**: The creator of QuadRF engaged in the comments, answering questions and noting improvements based on feedback. Some commenters were unclear about the 'see WiFi through walls' claim, while others discussed potential government surveillance capabilities and parallels with thermal cameras.

**Tags**: `#RF sensing`, `#software-defined radio`, `#drone detection`, `#open source hardware`, `#security`

---

<a id="item-5"></a>
## [GPT-5.6 Sol Ultra Claims Proof of Cycle Double Cover Conjecture](https://cdn.openai.com/pdf/04d1d1e4-bc75-476a-97cf-49055cd98d31/cdc_proof.pdf) ⭐️ 8.0/10

OpenAI released a preprint on July 10, 2026 claiming that their GPT-5.6 Sol Ultra model generated a proof of the Cycle Double Cover Conjecture, a long-standing open problem in graph theory. If verified, this would mark a significant milestone in AI's ability to autonomously produce novel mathematical proofs, potentially transforming research in mathematics and theoretical computer science. The proof is extremely concise, suggesting it exploits a clever trick missed by experts; the community remains skeptical pending peer review. The prompt included detailed instructions to reject status reports and vague optimism.

hackernews · scrlk · Jul 10, 18:29 · [Discussion](https://news.ycombinator.com/item?id=48863490)

**Background**: The Cycle Double Cover Conjecture asks whether every bridgeless undirected graph has a collection of cycles such that each edge appears exactly twice. It was posed by W.T. Tutte, Itai and Rodeh, George Szekeres, and Paul Seymour. The conjecture is equivalent to the circular embedding conjecture in graph embeddings.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover">Cycle double cover - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters noted the extensive hand-holding in the prompt, with one observing that much effort is spent telling the model to actually solve the problem. Another remarked that most commenters do not care about the conjecture itself, as evidenced by low past engagement. A third expressed skepticism, noting the proof's conciseness and the lack of autonomous theory-building.

**Tags**: `#AI`, `#graph theory`, `#proof`, `#LLM`, `#hype`

---

<a id="item-6"></a>
## [New York City Bans Deceptive Subscription Practices](https://www.theguardian.com/us-news/2026/jul/10/new-york-city-deceptive-subscriptions-ban) ⭐️ 8.0/10

New York City Mayor Mamdani announced a landmark law banning deceptive subscription practices and junk fees, requiring companies to make cancellations as easy as signing up. This law protects consumers from hidden fees and difficult cancellation processes, setting a precedent that could influence other jurisdictions and tech companies operating globally. The law includes a 'click-to-cancel' requirement and bans junk fees such as undisclosed service charges or resort fees, with no specific carveouts for restaurants unlike California.

hackernews · randycupertino · Jul 10, 18:26 · [Discussion](https://news.ycombinator.com/item?id=48863464)

**Background**: Subscription models are used by many businesses, from streaming services to gyms, often with automatic renewals and difficult cancellation processes. 'Drip pricing' and junk fees add hidden costs, leading to consumer frustration and regulatory action.

**Discussion**: Commenters expressed cautious optimism but raised enforcement concerns, noting California's similar laws have restaurant carveouts. Specific complaints included PayPal's old subscriptions and undisclosed hotel resort fees. Some praised the move as 'legitimate government' protecting consumers.

**Tags**: `#regulation`, `#consumer protection`, `#subscriptions`, `#New York City`, `#junk fees`

---

<a id="item-7"></a>
## [Tencent in talks to acquire AI startup Manus from Meta](https://www.reuters.com/technology/tencent-talks-become-ai-start-up-manus-largest-shareholder-ft-reports-2026-07-10/) ⭐️ 8.0/10

Tencent is negotiating to acquire the AI startup Manus from Meta, aiming to become its largest shareholder after Beijing ordered Meta to unwind its $2 billion acquisition. This deal marks a significant shift in the AI landscape, with Tencent gaining control of a promising AI agent startup amid geopolitical tensions between China and the US over technology acquisitions. Tencent will partner with original investors ZhenFund and HSG to repurchase Manus from Meta at a price of at least $2 billion, according to sources.

telegram · zaihuapd · Jul 10, 06:45

**Background**: Manus is an autonomous AI agent developed by Butterfly Effect, a company founded in China and based in Singapore. The startup gained attention for its ability to execute tasks beyond simple chatbots. Meta had previously agreed to acquire Manus for $2 billion, but the deal was blocked by Chinese regulators, leading to the current renegotiation with Tencent.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus (AI agent) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Manus_AI">Manus AI</a></li>

</ul>
</details>

**Tags**: `#Tencent`, `#AI startup`, `#acquisition`, `#Meta`, `#Manus`

---

<a id="item-8"></a>
## [OpenAI, Google Supply AI Models to Blacklisted Chinese Firms](https://www.ft.com/content/5d6aafa1-5d47-4585-aa95-6ec06a6cd20f) ⭐️ 8.0/10

OpenAI and Google have been providing advanced AI services to Singapore subsidiaries of Alibaba, Baidu, and Tencent, whose parent companies are on the US 1260H blacklist. These transactions are currently legal but have sparked renewed calls for stricter export controls on AI models. This news highlights a loophole in US export controls, as Chinese companies can access frontier AI models through overseas entities, raising national security concerns. It is likely to intensify the debate in Washington about regulating access to advanced AI software. OpenAI suspended API access for an Alibaba affiliate after detecting suspected model distillation and reported it to the US government. In contrast, Anthropic has a stricter policy, banning all Chinese companies and their overseas entities from accessing its frontier AI models.

telegram · zaihuapd · Jul 10, 09:59

**Background**: The 1260H list is a US Department of Defense list identifying Chinese military companies, often leading to economic sanctions. Model distillation is a machine learning technique where knowledge from a large 'teacher' model is transferred to a smaller 'student' model, making it easier to deploy on less powerful hardware. Understanding these concepts is crucial to grasping the implications of the news, as the US government is concerned that AI models could be misused for military purposes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/1260H_list">1260H list</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_distillation">Model distillation</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#export controls`, `#geopolitics`, `#OpenAI`, `#Google`

---

<a id="item-9"></a>
## [China Imposes Temporary Ban on Helium Exports](https://wms.mofcom.gov.cn/zcfb/wmgl/art/2026/art_2a795a0d55df4cada91c9fbd2a2cc13a.html) ⭐️ 8.0/10

On July 10, 2026, China's Ministry of Commerce and General Administration of Customs announced a temporary ban on the export of helium (HS code 2804290010), effective immediately, citing the Foreign Trade Law of the People's Republic of China. This ban could disrupt global helium supply chains critical for semiconductor manufacturing, medical imaging, and other high-tech industries, given China's role as a major helium producer. The ban applies to helium under customs code 2804290010, with no specified end date; adjustments will be announced separately. The announcement was jointly issued by the Ministry of Commerce and the General Administration of Customs.

telegram · zaihuapd · Jul 10, 13:27

**Background**: Helium is a non-renewable resource essential for cooling superconducting magnets in MRI machines, as a carrier gas in semiconductor manufacturing, and for space exploration. China is one of the world's largest helium producers, primarily through natural gas processing, and this export ban follows a trend of China restricting exports of strategic materials.

**Tags**: `#helium`, `#export ban`, `#trade policy`, `#supply chain`, `#semiconductor`

---

<a id="item-10"></a>
## [Meta Faces $12B EU Fine Over Addictive Design](https://www.theverge.com/policy/963872/meta-eu-addictive-design-200b-fine-risk-digital-services-act-dsa) ⭐️ 8.0/10

The European Commission has preliminarily found that Meta's Facebook and Instagram violate the Digital Services Act due to addictive design features, potentially leading to a $12 billion fine and a mandated redesign of the platforms. This action could set a major precedent for regulating addictive technology under the DSA, forcing Meta and other platforms to reduce engagement-driven features and better protect user mental health. The EU criticized Meta's limited tools as ineffective, and the proposed redesign includes disabling infinite scroll and autoplay by default, setting effective screen-time reminders, and reducing engagement-focused algorithmic recommendations.

telegram · zaihuapd · Jul 10, 14:47

**Background**: The Digital Services Act (DSA) is an EU regulation that imposes strict accountability and transparency requirements on large online platforms, especially Very Large Online Platforms (VLOPs) with over 45 million EU users. Addictive design refers to features like infinite scroll and autoplay that are intentionally crafted to maximize user engagement and time spent on platforms, often at the expense of user well-being. The DSA's risk assessment obligations require platforms to mitigate systemic risks such as negative effects on mental health.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Services_Act">Digital Services Act</a></li>
<li><a href="https://digital-strategy.ec.europa.eu/en/policies/digital-services-act">The Digital Services Act | Shaping Europe’s digital future</a></li>
<li><a href="https://algorithmwatch.org/en/dsa-explained/">A guide to the Digital Services Act, the EU’s law to rein in Big Tech - AlgorithmWatch</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#EU Regulation`, `#Digital Services Act`, `#Addictive Design`, `#Tech Policy`

---

<a id="item-11"></a>
## [SK Hynix CEO Warns of Worst Memory Shortage by 2027](https://www.reuters.com/world/asia-pacific/sk-hynix-ceo-sees-worst-ever-memory-supply-shortage-2027-says-demand-outstrip-2026-07-10/) ⭐️ 8.0/10

SK Hynix CEO Kwak Noh-jung warned that the global memory industry will face its worst-ever supply shortage in 2027, with demand outstripping supply into the 2030s despite aggressive expansion. This forecast from a major memory manufacturer signals potential price surges and supply constraints for AI, data centers, and consumer electronics, impacting the entire tech supply chain. SK Hynix is considering overseas fab sites in the US, Japan, and Southeast Asia, prioritizing land, electricity, and labor costs. The company reported a record operating profit of 47 trillion won in 2025.

telegram · zaihuapd · Jul 11, 00:45

**Background**: The memory chip industry is cyclical, with periods of oversupply and shortage driven by demand fluctuations and capacity investments. Recently, demand from AI and data centers has surged, straining supply. SK Hynix is a leading supplier of high-bandwidth memory (HBM) used in AI accelerators.

**Tags**: `#memory shortage`, `#semiconductor`, `#SK Hynix`, `#supply chain`, `#industry forecast`

---