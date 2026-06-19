---
layout: default
title: "Horizon Summary: 2026-06-19 (EN)"
date: 2026-06-19
lang: en
---

> From 34 items, 6 important content pieces were selected

---

1. [10k GitHub repos spread Trojan malware](#item-1) ⭐️ 9.0/10
2. [Hospitals and universities repurposing drugs at 90% lower cost](#item-2) ⭐️ 8.0/10
3. [Tool checks if your name is 'in the weights' of LLMs](#item-3) ⭐️ 8.0/10
4. [Modos Color E-Paper Monitor Achieves 60Hz Refresh Rate](#item-4) ⭐️ 8.0/10
5. [Apple and Intel Reach Preliminary Foundry Chip Agreement](#item-5) ⭐️ 8.0/10
6. [China Seeks Public Comments on Distributed Digital Identity Rules](#item-6) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [10k GitHub repos spread Trojan malware](https://orchidfiles.com/github-repositories-distributing-malware/) ⭐️ 9.0/10

A researcher discovered over 10,000 GitHub repositories distributing Trojan malware, exploiting AI agents and developer trust by cloning legitimate repos and pushing malicious commits. This massive supply chain attack could infect numerous developers and end users, highlighting the growing risk of AI agents being tricked into trusting malicious repositories. The attacker targets new repositories instead of popular ones, and frequently deletes and pushes new commits to appear updated in search results, aiming to deceive AI agents that scrape repositories for dependencies.

hackernews · theorchid · Jun 18, 11:45 · [Discussion](https://news.ycombinator.com/item?id=48583928)

**Background**: A supply chain attack targets less secure elements in a software supply chain, such as cloned repositories injected with malware. Attackers hope developers or AI agents will download the malicious code, which then propagates through dependencies. The rise of AI coding agents that automatically fetch packages amplifies the risk of such attacks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack</a></li>
<li><a href="https://siliconangle.com/2025/06/02/sysdig-detects-ai-assisted-malware-exploiting-open-webui-misconfigurations/">Sysdig detects AI -assisted malware exploiting Open... - SiliconANGLE</a></li>

</ul>
</details>

**Discussion**: Commenters noted the attack targets AI agents, not humans, by appearing in searches. One user shared personal experience of their name attached to unrelated projects. Another referenced a Disney engineer who downloaded a malicious AI tool from GitHub. The discussion also observed that frequent commit updates help repos rank high in 'last updated' searches.

**Tags**: `#security`, `#malware`, `#GitHub`, `#supply chain attacks`, `#AI agents`

---

<a id="item-2"></a>
## [Hospitals and universities repurposing drugs at 90% lower cost](https://www.kcl.ac.uk/news/hospitals-and-universities-repurposing-drugs-at-90-lower-cost) ⭐️ 8.0/10

Hospitals and universities are repurposing existing drugs for new uses at a fraction of the cost, such as using the cancer drug Avastin to treat macular degeneration for about $50 per dose instead of $1,500 for Lucentis. This approach could dramatically reduce healthcare costs and improve access to treatments, especially for conditions like macular degeneration and rare diseases where new drug development is prohibitively expensive. Avastin and Lucentis are molecularly similar, but Avastin is not packaged for ocular injection, leading to cost differences. There is no clear regulatory pathway for extending drug use without manufacturer consent, posing a barrier to widespread adoption.

hackernews · giuliomagnifico · Jun 18, 10:33 · [Discussion](https://news.ycombinator.com/item?id=48583386)

**Background**: Drug repurposing involves researching new indications for already approved drugs. It is a cost-effective strategy because the safety profile of the drug is already known, reducing development time and expense. Common examples include using fluoxetine for age-related macular degeneration.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Drug_repurposing">Drug repurposing</a></li>
<li><a href="https://www.nih.gov/news-events/nih-research-matters/repurposing-drugs-treat-age-related-macular-degeneration">Repurposing drugs to treat age-related macular degeneration | National Institutes of Health (NIH)</a></li>

</ul>
</details>

**Discussion**: Community comments highlight real-world examples like Avastin vs Lucentis for macular degeneration, and the success of Cures Within Reach for rare diseases. They also point out regulatory and incentive challenges, such as the case of Spravato (esketamine) being patented as a modified version of ketamine, and the lack of a clear pathway for off-label use.

**Tags**: `#drug repurposing`, `#healthcare costs`, `#pharmaceuticals`, `#macular degeneration`

---

<a id="item-3"></a>
## [Tool checks if your name is 'in the weights' of LLMs](https://www.intheweights.com/) ⭐️ 8.0/10

A new website, 'Are You in the Weights?', allows users to query multiple large language models in parallel to see how strongly they recognize a given name or username, revealing traces of personal data in model weights. This tool highlights the growing concern about privacy and memorization in LLMs, as it demonstrates that models can retain personal information from training data without consent, potentially exposing users to identification or extraction attacks. The tool queries frontier and small models in parallel, clusters responses, and provides a recognition score. Users must use real names or usernames, raising privacy concerns; the site reports that scores are non-deterministic and improve with additional keywords.

hackernews · turtlesoup · Jun 18, 20:49 · [Discussion](https://news.ycombinator.com/item?id=48591348)

**Background**: Large language models (LLMs) are trained on vast amounts of text, including public data such as web pages and social media posts. During training, models may memorize specific pieces of information, including personal names and usernames, a phenomenon known as memorization. This can lead to privacy risks if an attacker can prompt the model to reveal such data. The website taps into this by directly asking models about a person's identity.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2410.02650v1">Undesirable Memorization in Large Language Models: A Survey</a></li>
<li><a href="https://www.scirp.org/journal/paperinformation?paperid=133625">Evaluating Privacy Leakage and Memorization Attacks on Large Language Models (LLMs) in Generative AI Applications</a></li>
<li><a href="https://proceedings.mlr.press/v202/yu23c/yu23c.pdf">Bag of Tricks for Training Data Extraction from Language Models</a></li>

</ul>
</details>

**Discussion**: Commenters shared mixed results: some found their username highly recognized after decades of use, while others with common names discovered the model prioritized a famous namesake. Privacy concerns were raised, leading many to avoid using their real names. One user noted that the score improves with more personal keywords, and the non-deterministic nature was observed.

**Tags**: `#LLMs`, `#privacy`, `#online identity`, `#AI recognition`, `#tool`

---

<a id="item-4"></a>
## [Modos Color E-Paper Monitor Achieves 60Hz Refresh Rate](https://spectrum.ieee.org/modos-e-paper-monitor) ⭐️ 8.0/10

Modos, a two-person startup, is developing a 13.3-inch color e-paper monitor with a native resolution of 3200x2400 and a 60Hz refresh rate, pushing e-paper technology closer to mainstream LCD performance. If successful, this could enable e-paper monitors that are comfortable for extended reading and usable outdoors, while consuming minimal power, opening new possibilities for auxiliary displays and portable devices. The monitor, named Modos Flow, includes touch input and aims for general usage responsiveness; however, the actual panel response time may still be slower than LCDs due to e-paper's physical particle movement limitations.

hackernews · Vinnl · Jun 18, 11:41 · [Discussion](https://news.ycombinator.com/item?id=48583897)

**Background**: E-paper displays use charged particles to reflect ambient light, offering low power and outdoor readability but historically suffered from slow refresh rates and limited color. Recent advances from E Ink and others have improved color and refresh, but 60Hz remains a milestone for e-paper.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Electronic_paper">Electronic paper - Wikipedia</a></li>
<li><a href="https://spectrum.ieee.org/e-paper-display-modos">E-Paper Display Reaches the Realm of LCD Screens - IEEE Spectrum</a></li>

</ul>
</details>

**Discussion**: Community comments are positive, with users calling it 'one of the more exciting developments' and noting it may be the first e-ink monitor responsive enough for general use. Some express curiosity about the impact of high refresh rate on e-panel longevity.

**Tags**: `#e-paper`, `#displays`, `#hardware`, `#alternative technology`

---

<a id="item-5"></a>
## [Apple and Intel Reach Preliminary Foundry Chip Agreement](https://t.me/zaihuapd/42031) ⭐️ 8.0/10

Apple and Intel have reached a preliminary agreement for Intel to manufacture some chips for Apple devices. The deal was finalized after over a year of negotiations. This agreement diversifies Apple's chip supply chain, reducing reliance on TSMC, and strengthens Intel's foundry business, which is key to U.S. semiconductor policy. It is unclear which Apple devices (iPhone, iPad, or Mac) will use Intel-made chips. The U.S. government, led by the Commerce Secretary, heavily pushed for this partnership, and Intel now has foundry deals with Nvidia, SpaceX, and Apple.

telegram · zaihuapd · Jun 18, 09:19

**Background**: A foundry agreement means one company manufactures chips designed by another. Apple currently relies heavily on TSMC for iPhone, iPad, and Mac chips. Intel is expanding its foundry services as part of a U.S. push to boost domestic semiconductor manufacturing.

**Tags**: `#Apple`, `#Intel`, `#Semiconductor`, `#Foundry`, `#Supply Chain`

---

<a id="item-6"></a>
## [China Seeks Public Comments on Distributed Digital Identity Rules](https://www.cac.gov.cn/2026-06/18/c_1783525605384124.htm) ⭐️ 8.0/10

On June 18, 2026, the Cyberspace Administration of China (CAC) released a draft regulation titled 'Regulations on Promoting the Interoperability and Mutual Recognition of Distributed Digital Identities' for public comment, with a deadline of July 18. The regulation defines distributed digital identities based on blockchain, consisting of identifiers, keys, verifiable credentials, and verifiable presentations, enabling user self-sovereign identity management for use cases like login authentication and data authorization. This is a significant policy move that establishes a regulatory framework for decentralized digital identity in China, potentially impacting blockchain adoption and cross-platform identity interoperability across finance, transportation, customs, taxation, and digital yuan. It could set a global precedent for government-led distributed identity systems. The regulation proposes building a public service system for distributed digital identities, leveraging the national blockchain network to construct an 'identity chain.' Domestically and internationally, individuals, institutions, and industrial devices can voluntarily apply for registration, and relevant entities must fulfill data security and personal information protection obligations.

telegram · zaihuapd · Jun 19, 01:39

**Background**: Distributed digital identity (DDID), also known as self-sovereign identity (SSI), shifts control of identity data from centralized providers to users. Verifiable credentials (VCs) are tamper-evident digital documents that follow W3C standards, allowing issuers, holders, and verifiers to interact trustworthily. The 'identity chain' concept leverages blockchain to create a decentralized backbone for identity verification across different platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reply.com/en/data-world/decentralised-digital-identity-will-change-everything">Decentralised Digital Identity ( DDID ) will change how we... | Reply</a></li>
<li><a href="https://en.wikipedia.org/wiki/Verifiable_credentials">Verifiable credentials</a></li>
<li><a href="https://chain.link/article/onchain-identity-verification">Onchain Identity Verification Explained | Chainlink</a></li>

</ul>
</details>

**Tags**: `#distributed identity`, `#blockchain`, `#regulation`, `#China`, `#digital identity`

---