---
layout: default
title: "Horizon Summary: 2026-09-09 (EN)"
date: 2026-09-09
lang: en
---

> From 34 items, 8 important content pieces were selected

---

1. [OpenAI claims Navier–Stokes breakthrough, faces plagiarism accusations](#item-1) ⭐️ 10.0/10
2. [AlphaGenome Atlas Maps Effects of Every Possible Human DNA Letter Change](#item-2) ⭐️ 9.0/10
3. [Meta Unveils Muse, a Personal AI Agent Prioritizing Speed and Security](#item-3) ⭐️ 8.0/10
4. [Terence Tao: AI Is Non-Renewably Mining Open Math Problems](#item-4) ⭐️ 8.0/10
5. [OpenAI Launches ChatGPT Images 2.5, Adds Sunburst and Flare API Models](#item-5) ⭐️ 8.0/10
6. [China Targets 9,800 EFLOPS Intelligent Computing Power by 2030](#item-6) ⭐️ 8.0/10
7. [OpenAI Unveils ChatGPT Images 2.0 with Better Text Rendering and Reasoning](#item-7) ⭐️ 8.0/10
8. [US Accuses Six Chinese AI Firms of Stealing Technology via Distillation](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [OpenAI claims Navier–Stokes breakthrough, faces plagiarism accusations](https://simonwillison.net/2026/Sep/8/on-navier-stokes/) ⭐️ 10.0/10

On September 8, 2026, OpenAI announced that an unreleased internal model produced a resolution to the Navier–Stokes existence and smoothness problem, one of the seven Millennium Prize Problems. The claim has not been verified by external mathematicians, and it is overshadowed by a priority dispute with NYU professor Tristan Buckmaster and Anthropic mathematician Levent Alpöge. If verified, this would be the first time an AI system has solved a Millennium Prize Problem, potentially transforming mathematical discovery. The accompanying controversy also raises urgent questions about competitive intelligence, data privacy, and the ethics of AI-driven research. OpenAI says its agents reached the result about 88 hours after launch, using roughly 130 billion output tokens for the Navier–Stokes problem, plus 17 hours of Lean formalization via GPT-6 Astra. Buckmaster and Alpöge had achieved a related breakthrough on August 15, and Buckmaster alleges OpenAI started its effort only after learning of their work; OpenAI acknowledges that it 'cannot rule out' that de-identified user data helped improve its models.

rss · Simon Willison · Sep 8, 23:55

**Background**: The Navier–Stokes equations describe the motion of fluids, and the question of whether smooth solutions always exist in three dimensions is one of the seven Millennium Prize Problems, each offering a $1,000,000 prize since 2000. Only the Poincaré conjecture has been officially solved so far, by Grigori Perelman, who declined the award. OpenAI's announced result is a counterexample showing a breakdown of smoothness, built on a method by Diego Cordoba and Luis Martinez Zoroa from 2023, but it still awaits independent verification by the Clay Mathematics Institute and the wider mathematical community.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Navier–Stokes_existence_and_smoothness_problem">Navier–Stokes existence and smoothness problem</a></li>
<li><a href="https://en.wikipedia.org/wiki/Millennium_Prize_Problems">Millennium Prize Problems</a></li>

</ul>
</details>

**Discussion**: Community comments are overwhelmingly critical of OpenAI, with users accusing it of looking at user data, stealing researchers' work, and attempting to intimidate them. Some highlight OpenAI's own admission that data leakage cannot be ruled out, while others frame the incident as a long-standing academic priority dispute that AI has intensified.

**Tags**: `#AI`, `#mathematics`, `#OpenAI`, `#Navier-Stokes`, `#Millennium Prize Problems`

---

<a id="item-2"></a>
## [AlphaGenome Atlas Maps Effects of Every Possible Human DNA Letter Change](https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/) ⭐️ 9.0/10

Google DeepMind has introduced AlphaGenome Atlas, a public database that predicts the functional impact of all ~9 billion possible single-nucleotide variants in the human genome. The predictions were pre-computed with the AlphaGenome AI model rather than measured experimentally. This is the first comprehensive predictive map of every single-letter change in human DNA, moving beyond reference genomes to variant effects. Researchers studying disease variants, regulatory genomics, and personalized medicine could use it to prioritize which mutations are most likely to matter. The catalog covers coding and non-coding DNA and assigns 'AVI' scores that estimate the molecular effect of each variant. It is freely accessible through an interactive web portal that does not require institutional affiliation.

hackernews · utiiiD · Sep 8, 14:55 · [Discussion](https://news.ycombinator.com/item?id=49611251)

**Background**: The human genome is a sequence of about 3 billion DNA letters; changing a single letter, a single-nucleotide variant (SNV), can alter gene regulation or protein function and contribute to disease. Interpreting these variants is hard because most sit in non-coding regions whose function is poorly understood. AlphaGenome is a deep-learning model that learns how DNA sequence influences molecular features such as chromatin and gene expression, enabling it to score unseen variants at genome scale.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/google-deepmind/alphagenome-atlas/">AlphaGenome Atlas: a high-resolution map of human DNA</a></li>
<li><a href="https://deepmind.google/blog/alphagenome-atlas-a-predictive-map-of-every-possible-dna-letter-change-in-the-human-genome/">AlphaGenome Atlas: Molecular predictions for 9 Billion human DNA variants — Google DeepMind</a></li>

</ul>
</details>

**Discussion**: Commenters were largely curious about practical use and coverage: some asked whether promoter sequences and regulatory regions are captured, and whether personal genomes such as 23andMe data could be screened for pathogenic mutations. Others pointed to tutorial videos and noted that no affiliation is required to access the Atlas. One commenter linked an external experimental study that exhaustively mutated a virus genome, framing it as a real-world benchmark that complements AlphaGenome's predictions.

**Tags**: `#AI`, `#Genomics`, `#DeepMind`, `#Biology`, `#DNA`

---

<a id="item-3"></a>
## [Meta Unveils Muse, a Personal AI Agent Prioritizing Speed and Security](https://ai.meta.com/muse/) ⭐️ 8.0/10

Meta has announced Muse, a personal AI agent, at ai.meta.com/muse, highlighting fast response times and layered defenses against prompt-injection attacks. Meta AI's David Singleton also shared technical details about the security architecture behind it. Muse marks Meta's push to capture mainstream, non-expert AI users, putting it in direct competition with consumer assistants like ChatGPT. The way Meta handles security and data privacy will influence how much trust people place in AI agents that manage personal information. The security strategy uses multiple layers: the model is trained to recognize and resist prompt injection, the harness marks anything from untrusted sources, deterministic code checks the result, and an ensemble of classifiers runs where the agent cannot reach them. Despite these claims, commenters remain skeptical about Meta's handling of personal data and whether the product truly solves a consumer need.

hackernews · yks · Sep 8, 19:25 · [Discussion](https://news.ycombinator.com/item?id=49615537)

**Background**: Prompt injection is a cybersecurity exploit that takes advantage of large language models' inability to distinguish between developer instructions, user inputs, and untrusted content such as web pages or files. For AI agents that can browse the web or access files, indirect prompt injection embedded in website content can cause unintended behavior. Personal agents like Muse become central hubs for data, making layered defenses important for protecting users.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://owasp.org/www-community/attacks/PromptInjection">Prompt Injection | OWASP Foundation</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some see Muse as Meta's bid for mainstream AI users and praise its speed as a standout feature, while a developer highlights its layered prompt-injection defenses. Others express strong distrust of Meta's data-privacy promises and argue the product falls into the 'nobody asked for this' category, saying consumer AI often tries to solve problems people were already handling fine.

**Tags**: `#AI`, `#Meta`, `#Personal Assistant`, `#Security`, `#Product Launch`

---

<a id="item-4"></a>
## [Terence Tao: AI Is Non-Renewably Mining Open Math Problems](https://mathstodon.xyz/@tao/117237320796901560) ⭐️ 8.0/10

On Mathstodon, Terence Tao wrote that open math problems are being non-renewably mined by AI: they can be consumed by machines without yielding new human insights. He added that identifying a promising problem has now become the scarce and precious resource. From one of the world's foremost mathematicians, this reframes AI's role in mathematics: progress may no longer be bottlenecked by solving ability but by the ability to ask meaningful questions. That could redirect how mathematical talent, prizes, and AI research efforts are allocated. Tao is not describing a specific conjecture being solved by a particular AI system; he is pointing to a structural consequence. Even if AI produces a symbolically verified solution, the goal of mathematical research is understanding, and a solved problem without insight permanently removes an interesting question from the field.

hackernews · _alternator_ · Sep 8, 21:00 · [Discussion](https://news.ycombinator.com/item?id=49616968)

**Background**: Terence Tao is a Fields Medal-winning mathematician who frequently discusses mathematics and AI on federated platforms like Mathstodon. "Open math problems" are unsolved questions that attract mathematicians' attention, such as the Riemann hypothesis or the Navier-Stokes regularity problem. Traditional mathematical culture values not just correct answers but proofs and concepts that illuminate new areas. With AI systems increasingly capable of symbolic reasoning, it has become realistic to ask what it means for a machine to "solve" such problems.

**Discussion**: Commenters largely engaged critically rather than simply agreeing. One invoked Asimov's Multivac story, arguing that asking the right questions is the real bottleneck; another joked about computing a staggeringly large digit of pi. Several pushed back on the idea that machine-solved problems automatically impede human knowledge, noting that an uninterpretable proof would simply be uninteresting; there was also surprise that open problems form a finite resource, plus a suggestion that AI's next frontier is posing good questions, perhaps incentivized by prizes.

**Tags**: `#AI`, `#mathematics`, `#research`, `#Terence Tao`, `#open problems`

---

<a id="item-5"></a>
## [OpenAI Launches ChatGPT Images 2.5, Adds Sunburst and Flare API Models](https://simonwillison.net/2026/Sep/8/introducing-chatgpt-images-25/) ⭐️ 8.0/10

OpenAI announced ChatGPT Images 2.5 on September 8, 2026, reporting that its image models have generated more than 3 billion images across ChatGPT and the API. The new release improves multi-turn instruction following, better preserves subjects in reference photos, and responds faster, with two new API model IDs introduced: gpt-image-2.5-sunburst and gpt-image-2.5-flare. This release strengthens OpenAI's position in AI image generation, where multi-turn editing and subject consistency are becoming increasingly important demands. Developers and creative professionals now get both a fast everyday model (Flare) and a precision-focused editing model (Sunburst), making high-quality iterative image editing more practical through the API. According to OpenAI's guidance, Sunburst is intended for workflows where editing precision matters most, while Flare is for fast, high-quality everyday image generation. The API update also supports passing one or more reference images, as shown by Simon Willison's updated openai_image.py CLI tool, which combines text prompts with input images.

rss · Simon Willison · Sep 8, 22:46

**Background**: ChatGPT Images is OpenAI's text-to-image generation system, accessible through ChatGPT and through the GPT-Image models in the API. Image generation models create images from text prompts and can also edit existing images by following instructions; a major challenge in this field is multi-turn editing, where users iteratively refine an image while the model must preserve context and subject identity.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.kanaries.net/articles/gpt-image-2-5">GPT Image 2.5: How to Use It, Flare vs Sunburst, and API ...</a></li>
<li><a href="https://www.callmissed.com/blog/gpt-image-flare-vs-sunburst-key-differences">GPT Image 2.5 Flare vs Sunburst: Key Differences | CallMissed</a></li>
<li><a href="https://www.orcarouter.ai/blog/gpt-image-2-5-flare-sunburst">GPT-Image-2.5 Flare vs Sunburst: New OpenAI Image APIs</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Image Generation`, `#API`, `#AI Models`

---

<a id="item-6"></a>
## [China Targets 9,800 EFLOPS Intelligent Computing Power by 2030](https://www.scmp.com/tech/policy/article/3366733/china-targets-fourfold-boost-ai-computing-capacity-2030-major-tech-push) ⭐️ 8.0/10

China's Ministry of Industry and Information Technology has issued a five-year industrial plan aiming to expand the country's intelligent computing capacity to 9,800 EFLOPS by 2030. The plan calls for cumulative investment of 3.8 trillion yuan in information infrastructure from 2026 to 2030 and orderly deployment of 10,000-card and 100,000-card-plus AI computing clusters. This policy represents a state-backed push to roughly quadruple China's AI computing capacity, potentially reshaping global competition in AI infrastructure. The scale of planned investment and cluster deployment could affect AI hardware supply chains and accelerate domestic adoption of Chinese-made AI chips. As of the end of June, China's intelligent computing power had reached 2,185 EFLOPS, up 177% year on year, meaning the 2030 target requires more than a fourfold increase. The plan also emphasizes adapting infrastructure to work with domestic AI chips, reflecting ongoing efforts to reduce reliance on imported accelerators.

telegram · zaihuapd · Sep 8, 11:23

**Background**: EFLOPS, or exa-FLOPS, is a measure of computing performance equal to one quintillion (10^18) floating-point operations per second, commonly used for AI workloads with lower-precision formats such as FP16. Intelligent computing power specifically refers to computational capacity optimized for AI tasks. Large AI clusters, such as 10,000-card or 100,000-card configurations, link thousands of AI accelerator chips using high-speed networking to train large models more efficiently. This concept has become central to what some describe as a global race to build intelligent infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Floating_point_operations_per_second">Floating point operations per second - Wikipedia</a></li>
<li><a href="https://baike.baidu.com/en/item/EFLOPS/3608460">EFLOPS（A performance unit used to measure the scale of ...</a></li>
<li><a href="https://www.scmp.com/tech/big-tech/article/3352200/supersized-and-scaling-china-pushes-10000-card-computing-clusters-ai-race">Supersized and scaling: China pushes 10,000-card computing clusters in AI race | South China Morning Post</a></li>

</ul>
</details>

**Tags**: `#China Tech Policy`, `#AI Infrastructure`, `#Computing Power`, `#EFLOPS`, `#State Investment`

---

<a id="item-7"></a>
## [OpenAI Unveils ChatGPT Images 2.0 with Better Text Rendering and Reasoning](https://t.me/zaihuapd/43693) ⭐️ 8.0/10

OpenAI has released ChatGPT Images 2.0, a new image generation model built on GPT Image 2, announced around April 21-22, 2026. It introduces reasoning capabilities, enabling web search, output verification, and generation of up to eight visually consistent images from a single prompt. This marks a 'step change' for AI image generation: models can now reason, search the web, and reliably render dense text, addressing long-standing weaknesses like garbled words and complex layouts. It should make AI-generated images far more useful for real-world tasks such as marketing materials, comics, and UI design. The model improves rendering of non-Latin scripts including Chinese, Japanese, Korean, Hindi, and Bengali, and supports multi-panel comics, UI elements, and marketing assets at up to 2K resolution. OpenAI says the system represents a major advance in following detailed instructions, rendering dense text, and placing or relating objects within a scene.

telegram · zaihuapd · Sep 8, 18:45

**Background**: ChatGPT Images is OpenAI's image generation feature inside ChatGPT, built on GPT Image models. Earlier image generation models struggled to render legible text, especially non-Latin scripts, and could not logically reason about prompts to validate visual outputs. The new version adds a reasoning capability that can check and verify results, improving accuracy and visual consistency.

<details><summary>References</summary>
<ul>
<li><a href="https://www.engadget.com/ai/chatgpt-images-20-is-better-at-rendering-non-latin-text-190000153.html">ChatGPT Images 2.0 is better at rendering non-Latin text - Engadget</a></li>
<li><a href="https://www.socialsamosa.com/news-2/chatgpt-images-20-accurac-style-non-english-text-support-11752887">ChatGPT launches Images 2.0 with better accuracy, style and non-English text support</a></li>
<li><a href="https://www.technology.org/2026/04/22/chatgpt-images-2-0-finally-nails-the-one-thing-ai-art-never-could-actual-words/">ChatGPT Images 2.0 Finally Spells Correctly - Technology Org</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#image generation`, `#GPT Image 2`, `#AI models`, `#text rendering`

---

<a id="item-8"></a>
## [US Accuses Six Chinese AI Firms of Stealing Technology via Distillation](https://www.reuters.com/technology/us-accuses-chinese-ai-firms-industrial-scale-theft-ai-technology-2026-09-08/) ⭐️ 8.0/10

On September 8, the U.S. government accused six Chinese AI companies, including DeepSeek, Moonshot AI, and Alibaba, of using model distillation to steal American AI intellectual property at industrial scale. The allegations name Anthropic, OpenAI, Google, and SpaceX as victims and claim the alleged theft was likely carried out with the Chinese government's knowledge. This accusation escalates US-China tensions in artificial intelligence just before Chinese leader Xi Jinping's planned visit to the US and the China-US AI safety dialogue. It could reshape cross-border AI collaboration, influence global AI regulation, and further restrict how Chinese companies access American AI tools and models. The U.S. government claims the alleged distillation lowered Chinese firms' research and development costs and strengthened China's military and cyberattack capabilities. The accusation comes days before Xi Jinping's scheduled US visit, tying the case directly to ongoing geopolitical and AI policy negotiations.

telegram · zaihuapd · Sep 9, 01:43

**Background**: Knowledge distillation is a machine learning technique where a smaller 'student' model is trained to replicate the behavior of a larger 'teacher' model, typically for improved efficiency and lower computational cost. It is widely used in AI research and development, but it becomes controversial when a company uses another firm's proprietary model outputs to train competing systems, raising intellectual property and licensing concerns. The US accusation treats this otherwise standard technique as a form of industrial-scale IP theft when applied across national borders without authorization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/knowledge-distillation">What is Knowledge distillation? | IBM</a></li>

</ul>
</details>

**Tags**: `#AI`, `#US-China`, `#intellectual property`, `#regulation`, `#geopolitics`

---