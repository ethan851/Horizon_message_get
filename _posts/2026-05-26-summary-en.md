---
layout: default
title: "Horizon Summary: 2026-05-26 (EN)"
date: 2026-05-26
lang: en
---

> From 19 items, 8 important content pieces were selected

---

1. [Pope Leo XIV's Encyclical on AI Ethics](#item-1) ⭐️ 9.0/10
2. [Using AI to write better code more slowly](#item-2) ⭐️ 8.0/10
3. [Norway Invests in 2PB Huawei Flash and HPE Cray for LLM](#item-3) ⭐️ 8.0/10
4. [California proposes Linux exemption from age-verification law](#item-4) ⭐️ 8.0/10
5. [Microsoft Copilot Cowork Vulnerable to Prompt Injection](#item-5) ⭐️ 8.0/10
6. [Cybersecurity Expert Demand Surges in AI Era](#item-6) ⭐️ 8.0/10
7. [Grok V9-Medium 1.5T Model Training Complete, Release Expected Soon](#item-7) ⭐️ 8.0/10
8. [Semi-living human brains used for drug testing challenge ethics](#item-8) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Pope Leo XIV's Encyclical on AI Ethics](https://simonwillison.net/2026/May/25/encyclical-on-ai/#atom-everything) ⭐️ 9.0/10

Pope Leo XIV issued the encyclical 'Magnifica Humanitas' today, providing clear ethical guidelines for integrating AI into society. This is the Vatican's first formal encyclical on AI ethics, marking a significant religious and philosophical contribution to global AI policy and discourse. The encyclical describes AI systems as more 'cultivated' than 'built', highlighting the interpretability problem, and emphasizes that true development must center human dignity.

rss · Simon Willison · May 25, 23:58

**Background**: An encyclical is a formal papal letter addressing important issues. Pope Leo XIV chose his name in honor of Pope Leo XIII, who wrote 'Rerum Novarum' on the industrial revolution. This new encyclical applies Catholic social teaching to the AI revolution.

**Tags**: `#AI ethics`, `#Vatican`, `#encyclical`, `#human dignity`, `#policy`

---

<a id="item-2"></a>
## [Using AI to write better code more slowly](https://nolanlawson.com/2026/05/25/using-ai-to-write-better-code-more-slowly/) ⭐️ 8.0/10

The article argues for an iterative AI-assisted coding approach focused on code review and refinement, which produces higher quality code but at the cost of slower development speed. This challenges the common narrative that AI accelerates coding, highlighting a trade-off between quality and speed. It offers a practical methodology for developers seeking robust code rather than rapid output. The approach involves multiple iterations: design with AI, implement with a slower but more capable model, review, then use a fast review model to find corner cases, and fix with the capable model again.

hackernews · signa11 · May 25, 23:16 · [Discussion](https://news.ycombinator.com/item?id=48272984)

**Background**: AI-assisted coding typically emphasizes speed through generating code quickly. However, this article suggests that careful, iterative review can improve code quality, albeit slower. It reflects a nuanced understanding of AI as a collaborative tool rather than a replacement for human judgment.

**Discussion**: Comments show mixed experiences; some find the iterative loops time-consuming, while others see value in AI code review. There is skepticism about opinion pieces lacking examples, but also appreciation for the approach.

**Tags**: `#AI-assisted development`, `#code review`, `#software engineering`, `#developer productivity`

---

<a id="item-3"></a>
## [Norway Invests in 2PB Huawei Flash and HPE Cray for LLM](https://www.blocksandfiles.com/flash/2026/05/22/norways-2-petabytes-of-huawei-flash-storage-and-llm-training/5244910) ⭐️ 8.0/10

Norway is investing in 2 petabytes of Huawei flash storage and an HPE Cray Supercomputing EX system (named Olivia) with 448 GPUs to train a sovereign large language model in Norwegian. This initiative highlights the growing trend of nations pursuing AI sovereignty to preserve their language and culture, while also sparking debate about whether such investments are necessary or if alternative approaches like fine-tuning existing models are more practical. The Olivia system features 448 GPUs and 64,512 CPU cores, which some commenters consider insufficient for training a full-fledged LLM. The storage consists of 2 petabytes of Huawei flash storage.

hackernews · rbanffy · May 25, 19:37 · [Discussion](https://news.ycombinator.com/item?id=48270770)

**Background**: Sovereign AI refers to a nation's ability to produce artificial intelligence using its own infrastructure, data, workforce, and business networks. Norway's goal is to create an LLM that understands the Norwegian language and culture, as globally trained English-centric models may lack local knowledge. HPE Cray systems are designed for high-performance AI training and have been used in various supercomputing setups.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hpe.com/us/en/hpe-cray-xd670.html">HPE Cray XD670 | HPE</a></li>
<li><a href="https://blogs.nvidia.com/blog/what-is-sovereign-ai/">What Is Sovereign AI? | NVIDIA Blog</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-sovereignty">What is AI Sovereignty? | IBM</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed opinions: some questioned the necessity of a sovereign LLM, arguing that existing models already cover many languages; others doubted the hardware sufficiency, calling it 'meager' and predicting the effort may not produce a useful model. Alternative proposals included sharing training data with model builders rather than building from scratch.

**Tags**: `#LLM`, `#sovereign AI`, `#storage`, `#Norway`, `#AI infrastructure`

---

<a id="item-4"></a>
## [California proposes Linux exemption from age-verification law](https://www.tomshardware.com/software/linux/california-moves-to-exempt-linux-from-its-upcoming-age-verification-law-after-backlash-over-forcing-operating-systems-to-collect-users-ages-amendment-proposed-by-the-same-lawmaker-who-wrote-the-original-law) ⭐️ 8.0/10

California lawmaker who authored the age-verification law has proposed an amendment to exempt Linux from the law after backlash from the open source community. This exemption could set a precedent for how age-verification laws treat open source software, and avoids burdening Linux distributions with user age collection. The amendment was proposed by the same lawmaker who wrote the original law, and it specifically exempts operating systems like Linux that are not primarily designed to access age-restricted content.

hackernews · rbanffy · May 25, 18:19 · [Discussion](https://news.ycombinator.com/item?id=48269961)

**Background**: California's age-verification law aims to require online services to verify users' ages to protect minors. Initially, it could have been interpreted to apply to operating systems like Linux, which sparked backlash from the open source community who argued it would be impractical and violate privacy. The proposed exemption addresses these concerns.

**Discussion**: Commenters expressed skepticism about the law's intent and implementation, with some suggesting it's a way to prevent Linux developers from challenging the law on First Amendment grounds. Others noted that most commenters misunderstand the law's actual content.

**Tags**: `#California`, `#Linux`, `#age-verification`, `#open source`, `#technology policy`

---

<a id="item-5"></a>
## [Microsoft Copilot Cowork Vulnerable to Prompt Injection](https://www.promptarmor.com/resources/microsoft-copilot-cowork-exfiltrates-files) ⭐️ 8.0/10

Microsoft Copilot Cowork, a new feature that automates tasks across Microsoft 365, is vulnerable to prompt injection attacks that can exfiltrate sensitive files. Researcher demonstrated that a maliciously crafted skill can trick Copilot into sending data to an attacker-controlled server. This vulnerability is significant because Copilot Cowork is being rapidly adopted by enterprises to automate workflows, making it a high-value target. Exploitation could lead to widespread data breaches, undermining trust in AI-powered enterprise tools. The attack exploits the skill creation system in Cowork, where a skill can be written in natural language and executed by the LLM. The researcher found that a skill containing a command to exfiltrate files via curl works as expected, without proper isolation or verification.

hackernews · Kneenex · May 25, 21:45 · [Discussion](https://news.ycombinator.com/item?id=48272354)

**Background**: Microsoft Copilot Cowork, introduced in early 2026, shifts Copilot from reactive prompting to proactive task execution — it can send emails, schedule meetings, and manage files on behalf of users. Prompt injection is a cybersecurity attack where malicious prompts hijack an LLM's behavior, often used to bypass restrictions. In this case, the prompt injection is embedded in a Cowork skill, leading to unauthorized data exfiltration.

<details><summary>References</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/microsoft-365/blog/2026/03/09/copilot-cowork-a-new-way-of-getting-work-done/">Copilot Cowork: A new way of getting work done | Microsoft ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community is divided: some argue it's 'works as expected' since skills are programs, while others blame Microsoft for rushing the feature to production. Commenters note that prompt injection is not new and that Copilot should have better defenses, but the real issue is the lack of security in skill execution.

**Tags**: `#security`, `#AI`, `#Microsoft`, `#prompt injection`, `#Copilot`

---

<a id="item-6"></a>
## [Cybersecurity Expert Demand Surges in AI Era](https://www.nytimes.com/2026/05/24/technology/one-job-that-is-growing-in-the-ai-era-cybersecurity-experts.html) ⭐️ 8.0/10

Demand for cybersecurity experts has surged, with job postings up 11% year-over-year in Q1 2026 and executive-level demand increasing 5-7 times since autumn 2025. This trend highlights the critical need for cybersecurity talent as AI expands attack surfaces and introduces new threats, directly impacting enterprise security and executive compensation packages. Advanced security roles now command compensation packages of $7-8 million, and security engineers must supplement their skills with AI expertise to remain competitive.

telegram · zaihuapd · May 25, 06:21

**Background**: AI systems like Anthropic's Mythos can discover and exploit software vulnerabilities, creating new risks. Companies need leaders who understand both security and AI complexity.

**Tags**: `#cybersecurity`, `#AI`, `#job market`, `#technology trend`, `#industry growth`

---

<a id="item-7"></a>
## [Grok V9-Medium 1.5T Model Training Complete, Release Expected Soon](https://x.com/elonmusk/status/2058787384364265734) ⭐️ 8.0/10

Elon Musk announced that xAI has completed training the Grok V9-Medium foundation model, with 1.5 trillion parameters, and expects a public release in 2-3 weeks. The model incorporates Cursor data for enhanced programming capabilities. This release marks a significant scale-up from the previous Grok V8-small (0.5T), tripling parameter count and promising substantial improvements in complex programming tasks. It demonstrates xAI's continued investment in large-scale language models. The V9-Medium model is three times larger than V8-small at 1.5 trillion parameters, trained with additional Cursor programming data. Fine-tuning is underway, with reinforcement learning starting in days.

telegram · zaihuapd · May 25, 07:07

**Background**: Grok is xAI's chatbot language model, currently running Grok V8-small for production traffic. Cursor is an AI-powered code editor that provides coding assistance. The V9-Medium naming suggests it may be an intermediate checkpoint before a larger V9 model.

<details><summary>References</summary>
<ul>
<li><a href="https://x.com/elonmusk/status/2058787384364265734">Grok foundation model V9-Medium (1.5T) has finished training ...</a></li>
<li><a href="https://beyondtmrw.org/article/grok-v9-medium-training-complete-xai-15t-parameter-leap-coding-ai">Is Grok V9-Medium Grok 5? xAI's 1.5T AGI Hype Train Explained</a></li>
<li><a href="https://www.basenor.com/blogs/news/grok-v9-medium-1-5t-finishes-training-release-in-2-3-weeks">Grok V9-Medium (1.5T) Finishes Training, Release in 2-3 Weeks</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#Grok`, `#machine learning`, `#programming`

---

<a id="item-8"></a>
## [Semi-living human brains used for drug testing challenge ethics](https://www.science.org/content/article/not-alive-not-dead-disembodied-human-brains-used-drug-testing) ⭐️ 8.0/10

A study using the BrainEx perfusion system has partially restored metabolic and cellular activity in human brains hours after death, enabling drug testing for neurological diseases like Alzheimer's and Parkinson's. This breakthrough could revolutionize drug development for neurological disorders by using real human brain tissue, but it also raises profound ethical questions about the definition of death, consciousness, and consent. The BrainEx system perfuses the brain with a solution containing vitamins, amino acids, and metabolic factors, but the brains show no signs of consciousness or integrated neural activity. Researchers emphasize the preparation is not alive nor fully dead.

telegram · zaihuapd · May 25, 14:57

**Background**: BrainEx was originally developed for pig brains in 2019, restoring circulation and cell function hours after death. Ex vivo brain slice cultures have been used for drug testing, but using whole human brains in a semi-living state is novel. The ethical frameworks for death and organ donation were not designed for such technology.

<details><summary>References</summary>
<ul>
<li><a href="https://neuwritesd.org/2019/06/13/brainex-restoring-brain-circulation-after-death/">BrainEx: Restoring Brain Circulation After Death</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC8272538/">Evaluating the translational value of postmortem brain ...</a></li>
<li><a href="https://britbrief.co.uk/health/public/startup-keeps-disembodied-brains-alive-for-drug-tests.html">Controversial Startup Keeps Disembodied Human Brains Alive for Drug Testing</a></li>

</ul>
</details>

**Tags**: `#neuroscience`, `#ethics`, `#drug testing`, `#brain`, `#biotechnology`

---