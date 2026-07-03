---
layout: default
title: "Horizon Summary: 2026-07-03 (EN)"
date: 2026-07-03
lang: en
---

> From 27 items, 10 important content pieces were selected

---

1. [Virginia Bans Sale of Geolocation Data](#item-1) ⭐️ 8.0/10
2. [Scott Aaronson Urges Action on US Privacy Emergency](#item-2) ⭐️ 8.0/10
3. [Linux 6.9 Bug Leaves LUKS Encryption Keys in Memory During Suspend](#item-3) ⭐️ 8.0/10
4. [Podman v6.0.0 Released with Networking Enhancements and Quadlet Support](#item-4) ⭐️ 8.0/10
5. [How to Ask Strangers for Help Effectively](#item-5) ⭐️ 8.0/10
6. [Immich 3.0: Major Update to Self-Hosted Photo Manager](#item-6) ⭐️ 8.0/10
7. [Cloudflare to block mixed-use AI crawlers from ad pages](#item-7) ⭐️ 8.0/10
8. [OpenAI Proposes 5% US Government Stake in Itself and Other AI Giants](#item-8) ⭐️ 8.0/10
9. [China approves Unitree Robotics IPO on STAR Market](#item-9) ⭐️ 8.0/10
10. [Companies Restrict Employee AI Use Due to Surging Costs](#item-10) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Virginia Bans Sale of Geolocation Data](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

On April 13, 2026, Virginia Governor Abigail Spanberger signed S.B. 388, amending the Virginia Consumer Data Protection Act (VCDPA) to prohibit the sale of consumers' precise geolocation data, effective July 1, 2026. This law makes Virginia the third state to ban the sale of geolocation data, reflecting growing momentum for privacy protections at the state level. It addresses concerns about sensitive location data being used for purposes like targeted advertising or tracking visits to medical facilities. The ban applies to 'precise geolocation data' as defined in the VCDPA, and violations may be enforced by the Virginia Attorney General. The law does not cover data collected within the state but sold from outside Virginia, raising jurisdictional questions.

hackernews · toomuchtodo · Jul 2, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48767347)

**Background**: Geolocation data is information that identifies the physical location of a device, often derived from GPS, Wi-Fi, or cellular signals. Such data can reveal sensitive details about individuals, such as visits to medical clinics or places of worship. Similar laws have been passed in other states, including California and Maine, as part of a broader push for consumer data privacy.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data">Virginia Bans Sale of Geolocation Data</a></li>
<li><a href="https://www.regulatoryoversight.com/2026/04/virginia-becomes-third-state-to-ban-sale-of-consumers-precise-geolocation-data/">Virginia Becomes Third State to Ban Sale of Consumers' Precise Geolocation Data | Regulatory Oversight</a></li>
<li><a href="https://therecord.media/virginia-enacts-ban-on-precise-geolocation-data">Virginia enacts ban on precise geolocation data sales as momentum for similar prohibitions builds | The Record from Recorded Future News</a></li>

</ul>
</details>

**Discussion**: Commenters generally support the ban but express concerns about enforcement and loopholes. For example, dv_dt questions how the law applies to out-of-state companies, while smalltorch wonders if automated license plate readers (ALPR) are exempt. danielrmay highlights a case where location data was used to target anti-abortion ads at Planned Parenthood visitors.

**Tags**: `#privacy`, `#legislation`, `#geolocation`, `#data protection`

---

<a id="item-2"></a>
## [Scott Aaronson Urges Action on US Privacy Emergency](https://scottaaronson.blog/?p=9902) ⭐️ 8.0/10

Scott Aaronson published a blog post calling attention to what he describes as an American privacy emergency and urging citizens to contact their legislators about the issue. This highlights a growing concern about privacy in the United States and the influence of corporate interests over legislation, potentially affecting millions of Americans' data protection rights. The post includes a high engagement score of 8.0/10 and 50 comments on the blog, indicating substantial community interest. A commenter provided a link to find your member of Congress.

hackernews · flowercalled · Jul 3, 00:01 · [Discussion](https://news.ycombinator.com/item?id=48768992)

**Discussion**: The comments express frustration with corporate influence in politics, with one user noting that parental leave is popular but not mandated due to corporate donations. Another user provided a direct link to contact legislators.

**Tags**: `#privacy`, `#politics`, `#surveillance`, `#legislation`

---

<a id="item-3"></a>
## [Linux 6.9 Bug Leaves LUKS Encryption Keys in Memory During Suspend](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 8.0/10

A bug in Linux kernel 6.9 prevents the `cryptsetup luksSuspend` command from wiping disk-encryption keys from memory, leaving them exposed during system suspend. This regression undermines the security guarantee of LUKS suspend, potentially allowing attackers with physical access to extract encryption keys from RAM during sleep, compromising full disk encryption. The `cryptsetup luksSuspend` operation is designed to suspend an active encrypted device and wipe the encryption key from kernel memory; this bug prevents the key wiping step. The issue appears to be specific to Debian's implementation of luksSuspend, which is not part of the mainline cryptsetup tool.

hackernews · IngoBlechschmid · Jul 2, 15:25 · [Discussion](https://news.ycombinator.com/item?id=48763035)

**Background**: LUKS (Linux Unified Key Setup) is a disk encryption specification for Linux. The `luksSuspend` command is an extension that pauses access to an encrypted device and removes the master key from memory, requiring the passphrase to be re-entered upon resume. However, the man page notes that luksSuspend does not clear plaintext data in caches. This bug was discovered and reported with a NixOS test that ensures the key is properly wiped.

<details><summary>References</summary>
<ul>
<li><a href="https://man.archlinux.org/man/core/cryptsetup/cryptsetup-luksSuspend.8.en">cryptsetup-luksSuspend (8) — Arch manual pages</a></li>
<li><a href="https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/8/html/security_hardening/encrypting-block-devices-using-luks_security-hardening">Chapter 9. Encrypting block devices using LUKS - Red Hat</a></li>

</ul>
</details>

**Discussion**: Commenters debated the severity and scope: some noted that the bug only affects Debian's unsupported extension, not mainline, and called the title clickbait. Others argued that suspend to RAM inherently keeps keys in memory, so the risk is limited, while a few highlighted the importance of testing (e.g., NixOS tests).

**Tags**: `#linux`, `#security`, `#encryption`, `#LUKS`, `#kernel`

---

<a id="item-4"></a>
## [Podman v6.0.0 Released with Networking Enhancements and Quadlet Support](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0 has been released, featuring new networking enhancements and improved Quadlet support for declarative container management via systemd unit files. This major version update strengthens Podman's position as a robust Docker alternative, particularly for users seeking daemonless, rootless container management with tighter system integration. The improvements may accelerate adoption among DevOps and homelab users. The exact changelog for v6.0.0 was not detailed, but community feedback highlights enhanced networking and Quadlet functionality. Podman remains daemonless and rootless; the new version may further ease migration from Docker by improving compatibility with docker-compose.yml files.

hackernews · soheilpro · Jul 2, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48762098)

**Background**: Podman is a daemonless, open-source container engine that manages OCI containers. Unlike Docker, it does not require a persistent background daemon, improving security and reducing resource usage. Quadlet, merged into Podman 4.4, allows users to define containers, pods, volumes, and networks declaratively using systemd unit files. This integration simplifies deployment on Linux without needing Kubernetes.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.podman.io/en/latest/markdown/podman-systemd.unit.5.html">podman-systemd.unit — Podman documentation</a></li>
<li><a href="https://www.redhat.com/en/topics/containers/what-is-podman">What is Podman? - Red Hat</a></li>
<li><a href="https://www.redhat.com/en/blog/quadlet-podman">Make systemd better for Podman with Quadlet - Enable Sysadmin</a></li>

</ul>
</details>

**Discussion**: The community is largely positive: users praise Podman's daemonless architecture and ease of migration from Docker, with one reporting seamless transition using docker-compose.yml. However, a significant complaint is the limited out-of-the-box installation support for popular distros like Ubuntu, which some argue hinders wider adoption. Quadlet is highlighted as a standout feature for rootless container hosting.

**Tags**: `#containerization`, `#podman`, `#docker`, `#open-source`, `#devops`

---

<a id="item-5"></a>
## [How to Ask Strangers for Help Effectively](https://pradyuprasad.com/writings/how-to-ask-for-help/) ⭐️ 8.0/10

The article provides a practical guide on asking for help from strangers, emphasizing showing proof of work and being concise. Community comments enrich the discussion with real-world experiences and additional strategies. Asking for help is a crucial skill for professional networking and career growth. This advice helps people overcome the hesitation of reaching out to strangers and increases the likelihood of receiving a positive response. The author and commenters stress that proof of work must be genuine and deep, not superficial. One commenter suggests offering to pay for the helper's time upfront, which often results in free interactions or discounted rates.

hackernews · FigurativeVoid · Jul 2, 13:19 · [Discussion](https://news.ycombinator.com/item?id=48761118)

**Background**: In this context, 'proof of work' means demonstrating that you have already invested significant effort to solve the problem yourself before asking for help. This shows respect for the helper's time and proves you are serious. The guide is relevant for anyone reaching out to professionals, potential mentors, or employers.

**Discussion**: The comments are positive and constructive, with users sharing personal lessons and additional tips. Jackconsidine emphasizes the importance of brevity over elaborate notes, while Aurornis warns that surface-level proof of work is insufficient. Mrtb suggests offering to pay as a sign of seriousness.

**Tags**: `#communication`, `#professional-networking`, `#career-advice`, `#asking-for-help`, `#soft-skills`

---

<a id="item-6"></a>
## [Immich 3.0: Major Update to Self-Hosted Photo Manager](https://github.com/immich-app/immich/discussions/29439) ⭐️ 8.0/10

Immich 3.0, a major version release of the self-hosted photo and video management platform, has been announced, sparking significant community discussion about new features and trade-offs. Immich is a popular open-source alternative to Google Photos and Apple Photos, and this major release highlights the growing demand for privacy-conscious, self-hosted media management solutions. The update includes numerous improvements and new features, though specific technical details were not provided in the announcement. Some users have reported ongoing issues with iOS photo sync performance.

hackernews · hashier · Jul 2, 14:13 · [Discussion](https://news.ycombinator.com/item?id=48761944)

**Background**: Immich is a self-hosted photo and video backup solution that allows users to store their media on their own servers, providing privacy and control. It offers features like automatic backup, organization, and search, similar to cloud services but without relying on third-party servers.

<details><summary>References</summary>
<ul>
<li><a href="https://immich.app/">Immich</a></li>

</ul>
</details>

**Discussion**: The community discussion is largely positive, with many praising Immich as a great substitute for Google/Apple Photos. However, there is debate about the lack of end-to-end encryption, with some users favoring services like Ente Photos for that feature. A user also raised ongoing issues with iOS photo sync, mentioning that the process can be slow and fill up storage.

**Tags**: `#self-hosting`, `#photography`, `#open-source`, `#privacy`

---

<a id="item-7"></a>
## [Cloudflare to block mixed-use AI crawlers from ad pages](https://techcrunch.com/2026/07/01/cloudflares-new-policy-pushes-ai-companies-to-pay-for-publishers-content/) ⭐️ 8.0/10

Cloudflare announced that starting September 15, it will default-block mixed-use crawlers—those used for both search and AI training—from accessing ads-supported pages, and specifically criticized Google for exploiting the loophole. This policy shift could force AI companies to pay for web content, addressing publisher concerns about unauthorized use of their data for AI training and potentially reshaping how AI firms access online data. The block applies to crawlers that serve both search indexing and AI model training, making it harder for companies like Google to use search crawler access to train AI without explicit permission.

telegram · zaihuapd · Jul 2, 05:37

**Background**: Web crawlers are automated programs that index pages for search engines. AI crawlers collect data to train large language models. Many websites block AI crawlers but allow search crawlers, creating a loophole that some AI companies like Google exploit to collect data for AI without additional payment.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-cn/網路爬蟲">网络 爬 虫 - 维基百科，自由的百科全书</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/678284279">下一代网络爬虫：爬虫级 AI agents - 知乎</a></li>

</ul>
</details>

**Discussion**: A common sentiment expressed is that many websites block AI crawlers but not Google search crawlers, allowing Google to exploit this loophole to train its AI.

**Tags**: `#Cloudflare`, `#AI crawlers`, `#web scraping`, `#Google`, `#AI policy`

---

<a id="item-8"></a>
## [OpenAI Proposes 5% US Government Stake in Itself and Other AI Giants](https://www.bloomberg.com/news/articles/2026-07-02/openai-proposes-giving-the-us-government-a-5-stake-ft-says) ⭐️ 8.0/10

OpenAI has proposed that the US government take a 5% equity stake in itself and other leading AI companies such as Google and Meta, as a way to share the benefits of AI with the public. This proposal could reshape the relationship between the US government and major AI firms, potentially setting a precedent for public benefit from AI-driven economic growth. It also raises significant questions about government control and conflicts of interest. The proposal includes a government entity holding 5% stakes in multiple AI companies, but it is unclear whether companies like Google and Meta have accepted. There are concerns about regulatory and governance issues.

telegram · zaihuapd · Jul 2, 06:02

**Background**: OpenAI is a leading AI research organization that developed GPT models. The proposal comes amid growing debate about how the benefits of AI should be distributed. The US government has been exploring various regulatory approaches to AI.

**Tags**: `#AI`, `#OpenAI`, `#Government Regulation`, `#Policy`, `#Tech Industry`

---

<a id="item-9"></a>
## [China approves Unitree Robotics IPO on STAR Market](https://www.csrc.gov.cn/csrc/c105906/c7642867/content.shtml) ⭐️ 8.0/10

On July 1, 2026, the China Securities Regulatory Commission (CSRC) approved Unitree Robotics' initial public offering (IPO) registration for listing on the Shanghai STAR Market. This approval marks a major financial milestone for Unitree, a leading robotics company, and signals regulatory confidence in the robotics and AI sectors, potentially encouraging more tech IPOs in China. Unitree must conduct the issuance strictly according to the prospectus and underwriting plan submitted to the Shanghai Stock Exchange, and must promptly report any material events from registration to issuance completion.

telegram · zaihuapd · Jul 2, 09:57

**Background**: The STAR Market, launched in July 2019, is China's Nasdaq-style board designed to attract innovative tech companies. Unitree Robotics, founded in 2016 by Wang Xingxing, specializes in quadruped and humanoid robots, gaining global recognition for its products.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unitree_Robotics">Unitree Robotics</a></li>
<li><a href="https://sjgrand.cn/star-market-shanghai-stock-exchange/">Star Market : Shanghai’s New Stock Exchange - S.J. Grand</a></li>

</ul>
</details>

**Tags**: `#IPO`, `#robotics`, `#regulation`, `#China`, `#finance`

---

<a id="item-10"></a>
## [Companies Restrict Employee AI Use Due to Surging Costs](https://www.404media.co/companies-are-throttling-employees-ai-use-because-its-too-expensive/) ⭐️ 8.0/10

Citibank has banned employees from using advanced AI models like GPT-5.5 and Claude Opus 4.6 and 4.7 due to excessive AI credit consumption, while Atlassian's monthly AI spend skyrocketed from $5M to $15M between August 2025 and May 2026. This trend reveals a critical friction point in enterprise AI adoption: usage-based pricing can lead to runaway costs, forcing companies to throttle AI use. It signals that current pricing models may be unsustainable for widespread internal deployment. Atlassian has ended unlimited AI usage and introduced a cost-tracking dashboard, while Adobe declined to renew its unlimited Claude contract. Amazon employees discovered previously unknown token usage caps after an internal leaderboard was shut down.

telegram · zaihuapd · Jul 2, 13:59

**Background**: AI models like GPT-5.5 and Claude Opus 4.6 are among the most powerful and expensive, with pricing per token (input and output). Many enterprises adopted usage-based billing from providers like OpenAI and Anthropic, resulting in costs that scale with employee usage, leading to budget overruns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-opus-4-6">Claude Opus 4 . 6 \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5 - Wikipedia</a></li>
<li><a href="https://stripe.com/billing/usage-based-billing">Usage - based billing software for AI | Metronome, a Stripe product</a></li>

</ul>
</details>

**Tags**: `#AI`, `#enterprise`, `#cost`, `#usage-tracking`, `#models`

---