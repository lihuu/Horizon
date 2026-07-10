---
layout: default
title: "Horizon Summary: 2026-07-10 (EN)"
date: 2026-07-10
lang: en
---

> From 36 items, 19 important content pieces were selected

---

1. [OpenAI Releases GPT-5.6 with Three Model Sizes](#item-1) ⭐️ 9.0/10
2. [GLM 5.2 runs on 32GB RAM via int4 and disk streaming](#item-2) ⭐️ 8.0/10
3. [EU Parliament passes Chat Control 1.0 law](#item-3) ⭐️ 8.0/10
4. [US Army logistics too fragile for major war](#item-4) ⭐️ 8.0/10
5. [TLS certificates for internal services done right](#item-5) ⭐️ 8.0/10
6. [GLM 5.2 Approaches Human-Level Accuracy in Bookkeeping](#item-6) ⭐️ 8.0/10
7. [OpenAI Merges ChatGPT and Codex into 'ChatGPT Work'](#item-7) ⭐️ 8.0/10
8. [Google pays $250K for Linux KVM VM escape vulnerability](#item-8) ⭐️ 8.0/10
9. [Postgres is Enough for More Than We Admit](#item-9) ⭐️ 8.0/10
10. [Tencent's Hy3 LLM Stirs OpenRouter Debate](#item-10) ⭐️ 7.0/10
11. [Postgres Rewritten in Rust Using LLMs, Passes All Tests](#item-11) ⭐️ 7.0/10
12. [No leap second at end of December 2026, IERS announces](#item-12) ⭐️ 7.0/10
13. [Meta Releases Muse Spark 1.1 Agentic AI Model with API](#item-13) ⭐️ 7.0/10
14. [China's Gobi solar plant uses molten salt to generate power after dark](#item-14) ⭐️ 7.0/10
15. [New Jersey bill requires three sensor types, blocking Tesla's camera-only Robotaxi](#item-15) ⭐️ 7.0/10
16. [Bun Rust Rewrite Thoughts Shared by Developer](#item-16) ⭐️ 7.0/10
17. [AI-generated content floods social media, especially LinkedIn](#item-17) ⭐️ 6.0/10
18. [Developers abandon GitHub for Codeberg and self-hosted alternatives](#item-18) ⭐️ 6.0/10
19. [Pruning on Non-Partitioned Columns in PostgreSQL](#item-19) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI Releases GPT-5.6 with Three Model Sizes](https://openai.com/index/gpt-5-6/) ⭐️ 9.0/10

OpenAI released GPT-5.6, its latest flagship model available in three sizes: Luna, Terra, and Sol, with pricing starting at $1 per million input tokens for Luna. GPT-5.6 offers significant cost savings per task compared to competitors like Claude Opus and Fable, and sets a new state-of-the-art on the ARC-AGI-3 benchmark, demonstrating improved reasoning and agentic capabilities. The model sizes are Luna (smallest, $1/$6 per 1M input/output tokens), Terra ($2.50/$15), and Sol ($5/$30). Sol achieves 7.8% on ARC-AGI-3, the first verified frontier model to beat an ARC-AGI-3 game.

hackernews · logickkk1 · Jul 9, 17:04 · [Discussion](https://news.ycombinator.com/item?id=48849066)

**Background**: ARC-AGI-3 is an interactive reasoning benchmark that challenges AI agents to explore novel environments, infer goals, and plan actions. It is designed to measure human-like intelligence in AI agents. GPT-5.6's performance on this benchmark indicates progress toward more general reasoning.

<details><summary>References</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">[2603.24621] ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence</a></li>
<li><a href="https://arcprize.org/competitions/2026/arc-agi-3">ARC Prize 2026 - ARC-AGI-3 Competition</a></li>

</ul>
</details>

**Discussion**: Community comments highlight GPT-5.6's token efficiency and cost advantages, with Sol at $1.04 per task versus Opus 4.8 at $1.80 and Fable at $2.75. Developers also note semantic tips from OpenAI's guide, such as improved intent understanding. Some users discuss model comparisons in coding assistants like Claude Code vs Codex.

**Tags**: `#AI`, `#GPT-5.6`, `#OpenAI`, `#Language Models`, `#Machine Learning`

---

<a id="item-2"></a>
## [GLM 5.2 runs on 32GB RAM via int4 and disk streaming](https://github.com/JustVugg/colibri) ⭐️ 8.0/10

The author successfully ran the 744B-parameter MoE model GLM 5.2 on a 12-core laptop with 25GB RAM by converting to int4 and streaming routed experts from disk. The engine Colibrì achieves about 0.1 tokens per second on cold start. This demonstrates that massive LLMs can be run on consumer hardware without a GPU, enabling local AI inference for users with limited resources. It also shows innovative caching and streaming techniques that could be applied to other large models. The model has 744B parameters but activates only ~40B per token; the dense part (~17B params) stays in RAM at int4 (~9.9 GB), while 21,504 routed experts are streamed from disk (~370 GB) with an LRU cache. The engine is a single C file with no runtime dependencies.

hackernews · vforno · Jul 9, 08:05 · [Discussion](https://news.ycombinator.com/item?id=48842459)

**Background**: GLM 5.2 is a Mixture-of-Experts (MoE) model with 744B total parameters but only 40B active per token. int4 quantization reduces memory usage by half while preserving quality. MoE models route tokens to a subset of experts, enabling large capacity with manageable compute.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mindstudio.ai/blog/what-is-glm-5-2-open-weight-model">What Is GLM 5.2? The Open-Weight Model Beating GPT 5.5 on Design Benchmarks | MindStudio</a></li>
<li><a href="https://huggingface.co/docs/transformers/quantization/concept_guide">Quantization concepts · Hugging Face</a></li>
<li><a href="https://unsloth.ai/docs/models/glm-5.2">GLM-5.2 - How to Run Locally | Unsloth Documentation</a></li>

</ul>
</details>

**Discussion**: Community comments include a user working on similar optimization for macOS with Unsloth and Metal, another questioning practical token rates (e.g., 0.05–0.1 tok/s vs. 1 tok/s), and a suggestion to use mmap and Medusa. Overall sentiment is positive and collaborative, with shared technical insights.

**Tags**: `#LLM`, `#optimization`, `#local AI`, `#GLM`, `#quantization`

---

<a id="item-3"></a>
## [EU Parliament passes Chat Control 1.0 law](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 8.0/10

The European Parliament allowed Chat Control 1.0 to become law on July 9, 2026, permitting warrantless scanning of private messages until 2028, despite a majority of MEPs voting against it. This law enables mass surveillance of private communications, threatening end-to-end encryption and privacy rights, and sets a dangerous precedent for digital surveillance in the EU. The law was passed through a procedural trick: a motion to reject required an absolute majority of 361 votes, but only 314 MEPs opposed, with 276 in favor and 17 abstentions, while 113 were absent.

hackernews · rapnie · Jul 9, 11:03 · [Discussion](https://news.ycombinator.com/item?id=48843923)

**Background**: Chat Control 1.0 is a temporary EU regulation aimed at detecting child sexual abuse material (CSAM) through voluntary scanning by tech companies. Critics argue it effectively mandates mass surveillance of all private messages and undermines end-to-end encryption, violating fundamental rights to privacy.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control_1.0">Chat Control 1.0</a></li>
<li><a href="https://www.reddit.com/r/europe/comments/1urnadd/european_parliament_greenlights_chat_control_10/">r/europe on Reddit: European Parliament greenlights Chat Control 1.0, will now become law. 276 In Favour, 314 Against, 17 Abstentians.</a></li>

</ul>
</details>

**Discussion**: Community comments heavily criticize the parliamentary tactics used, calling it a 'stupid parliamentary trick' and a threat to democracy, with some warning that the EU is moving toward totalitarianism.

**Tags**: `#privacy`, `#surveillance`, `#EU legislation`, `#encryption`, `#civil liberties`

---

<a id="item-4"></a>
## [US Army logistics too fragile for major war](https://mwi.westpoint.edu/the-glass-backbone-why-the-armys-logistics-will-break-in-the-next-war/) ⭐️ 8.0/10

A detailed analysis from the Modern War Institute argues that the U.S. Army's logistics system, built on just-in-time principles, is dangerously fragile and likely to fail in a major conflict against a peer adversary. If the Army's logistics break down, frontline units could run out of ammunition, fuel, and food, leading to catastrophic operational failures. This critique challenges decades of cost-cutting efficiency at the expense of resilience. The article highlights the concept of 'tooth-to-tail ratio,' which measures combat forces versus support forces, and argues that modern logistics mirror fragile commercial supply chains. It warns that adversaries like Iran or China could target logistics nodes with long-range precision strikes.

hackernews · baud147258 · Jul 9, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48845442)

**Background**: Just-in-time logistics delivers supplies exactly when needed, reducing inventory costs but leaving little buffer for disruptions. The military adopted this approach for peacetime efficiency, but it becomes a vulnerability in contested environments where supply lines can be cut. The 'tooth-to-tail ratio' is an old metric that often leads to underinvestment in logistics.

<details><summary>References</summary>
<ul>
<li><a href="https://combataxis.com/just-in-time-logistics-in-warfare/">Enhancing Warfare Efficiency Through Just-in-Time Logistics ...</a></li>
<li><a href="https://www.forbes.com/sites/maryjohnstone-louis/2025/04/25/todays-most-crucial-leadership-skill-is-systems-thinking/">Today's Most Crucial Leadership Skill Is Systems Thinking - Forbes</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with the analysis, drawing parallels to historical strategies like Fabian tactics against Hannibal. Some note that Iran and Ukraine have shown how to target logistics in modern wars, while others argue that new technologies like SpaceX's Starship could revolutionize supply delivery.

**Tags**: `#logistics`, `#military`, `#systems-thinking`, `#supply-chain`, `#strategy`

---

<a id="item-5"></a>
## [TLS certificates for internal services done right](https://tuxnet.dev/posts/tls-for-internal-services/) ⭐️ 8.0/10

A new guide explains how to use split-horizon DNS with ACME to manage TLS certificates for internal services, offering an alternative to running an internal CA. This addresses a common operational challenge of managing TLS for internal services, reducing complexity and reliance on internal certificate authorities. The high community engagement underscores its relevance to practitioners. The guide recommends using the DNS-01 ACME challenge to avoid HTTP-01 limitations, and acknowledges that split-horizon DNS can introduce long-term complexity. Community comments advocate for DNS-01 and using Let's Encrypt over an internal CA.

hackernews · mrl5 · Jul 9, 14:57 · [Discussion](https://news.ycombinator.com/item?id=48846995)

**Background**: Split-horizon DNS is a technique where a DNS server returns different records based on the source of the query, often used to provide internal IP addresses to internal clients and public IPs to external ones. The ACME DNS-01 challenge proves domain control by requiring a specific TXT record placed in the domain's DNS zone, enabling certificate issuance for services not reachable via HTTP.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Split-horizon_DNS">Split-horizon DNS</a></li>
<li><a href="https://letsencrypt.org/docs/challenge-types/">Challenge Types - Let's Encrypt</a></li>

</ul>
</details>

**Discussion**: Commenters largely favor DNS-01 validation over split-horizon DNS to avoid complexity, with some suggesting using public DNS records with internal IPs behind a VPN. Others express frustration with the difficulty of configuring HTTPS clients to trust internal CAs, advocating for Let's Encrypt with wildcard certificates.

**Tags**: `#TLS`, `#certificates`, `#ACME`, `#DNS`, `#internal services`

---

<a id="item-6"></a>
## [GLM 5.2 Approaches Human-Level Accuracy in Bookkeeping](https://toot-books.pages.dev/blog/glm-5-2-vat-benchmark) ⭐️ 8.0/10

GLM 5.2 has achieved near-human accuracy on a VAT bookkeeping benchmark, correctly posting over 99% of transactions without error. However, the benchmark only tests a subset of a real bookkeeper's job, missing tasks like invoice retrieval and handling ambiguous situations. This milestone demonstrates that LLMs can perform core accounting tasks with high reliability, potentially reducing manual effort. However, liability and job scope limitations mean full automation of bookkeeping remains a future goal, not an immediate replacement. The model achieved 99.2% accuracy on the benchmark, with errors mostly from ambiguous tax rules or missing context. The benchmark used pre-prepared user notes, simplifying the real-world process where bookkeepers must find and organize invoices.

hackernews · adamkurkiewicz · Jul 9, 18:29 · [Discussion](https://news.ycombinator.com/item?id=48850414)

**Background**: GLM-5.2 is a large language model designed for long-horizon tasks with a 1M-token context window, built by Z.AI. Bookkeeping involves matching bank transactions with invoices and applying tax rules; LLMs like GLM can process text and perform reasoning, making them suitable for such structured tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://z.ai/blog/glm-5.2">GLM-5.2: Built for Long-Horizon Tasks - z.ai</a></li>
<li><a href="https://openlm.ai/glm-5.2/">GLM-5.2 - openlm.ai</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the benchmark underestimates the broader job scope (e.g., finding invoices, handling exceptions) and raised liability concerns if the LLM makes errors. Some expressed skepticism about the company's transparency and said they would continue using human accountants.

**Tags**: `#AI`, `#bookkeeping`, `#LLM`, `#automation`, `#accounting`

---

<a id="item-7"></a>
## [OpenAI Merges ChatGPT and Codex into 'ChatGPT Work'](https://openai.com/index/chatgpt-for-your-most-ambitious-work/) ⭐️ 8.0/10

OpenAI released 'ChatGPT Work', a unified app that merges the ChatGPT chatbot with the Codex coding agent, causing user confusion and criticism over UI changes. This unification blurs the line between casual conversation and coding tasks, potentially alienating users who prefer separate experiences. It signals OpenAI's push towards enterprise-focused features, but at the cost of UX clarity. The separate Codex app is replaced by ChatGPT Work; the old ChatGPT app is renamed 'ChatGPT Classic', implying eventual discontinuation. Users report that toggling between Work and Codex modes shows no visible changes, and casual chat is relegated to a small popup window.

hackernews · Tiberium · Jul 9, 17:03 · [Discussion](https://news.ycombinator.com/item?id=48849059)

**Background**: ChatGPT is a conversational AI chatbot launched by OpenAI in November 2022 for general text generation. Codex, introduced in May 2025, is an AI coding agent that can inspect repos, run commands, and complete coding tasks. The new 'ChatGPT Work' app aims to combine these two environments into a single interface, but the abrupt unification has led to confusion about which mode to use for different tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI</a></li>
<li><a href="https://openai.com/index/introducing-codex/">Introducing Codex - OpenAI</a></li>

</ul>
</details>

**Discussion**: User comments are overwhelmingly negative, with many expressing confusion about the product changes. Key complaints include the loss of a dedicated casual chat interface, unclear differences between Work and Codex modes, and the renaming of the old app to 'ChatGPT Classic' which suggests it will be deprecated. Some users urge OpenAI to leave well-functioning features alone and instead build new adjacent products.

**Tags**: `#OpenAI`, `#ChatGPT`, `#UX`, `#product-launch`, `#AI-tools`

---

<a id="item-8"></a>
## [Google pays $250K for Linux KVM VM escape vulnerability](https://www.reddit.com/r/programming/comments/1urt5ib/google_pays_250k_for_linux_vulnerability_allowing/) ⭐️ 8.0/10

Google awarded a $250,000 bounty through its kvmCTF program for a critical Linux kernel vulnerability (CVE-2026-53359) that allows guest virtual machines to escape their sandbox and gain root access on the host. This vulnerability, dubbed 'Januscape', affects KVM on both Intel and AMD x86 systems, posing a severe risk to multi-tenant cloud environments and virtualized infrastructures where a single malicious VM could compromise the entire host. The flaw existed for 16 years and corrupts the host kernel's shadow-page state from a guest VM, enabling full guest-to-host escape. Google's kvmCTF program offers up to $250,000 for such zero-day submissions.

reddit · r/programming · /u/CircumspectCapybara · Jul 9, 15:13

**Background**: KVM (Kernel-based Virtual Machine) is a Linux kernel module that allows the kernel to function as a hypervisor, hosting multiple virtual machines. A VM escape occurs when an attacker breaks out of the isolated guest environment and executes code on the host. Google's kvmCTF is a bug bounty program specifically targeting KVM vulnerabilities, with higher payouts for full host compromises.

<details><summary>References</summary>
<ul>
<li><a href="https://arstechnica.com/security/2026/07/high-severity-guest-vm-escape-is-1-of-2-linux-vulnerabilities-to-surface-this-week/">Google pays $250K for Linux vulnerability allowing guest VM ...</a></li>
<li><a href="https://threat-modeling.com/cve-2026-53359-januscape-linux-kvm-vm-escape-intel-amd/">CVE-2026-53359 'Januscape': 16-Year-Old Linux KVM Guest-to ...</a></li>
<li><a href="https://thehackernews.com/2026/07/16-year-old-linux-kvm-flaw-lets-guest.html">16-Year-Old Linux KVM Flaw Lets Guest VMs Escape to Host on ...</a></li>

</ul>
</details>

**Tags**: `#security`, `#Linux kernel`, `#virtualization`, `#vulnerability`, `#bounty`

---

<a id="item-9"></a>
## [Postgres is Enough for More Than We Admit](https://www.reddit.com/r/programming/comments/1us129c/postgres_is_enough_for_more_than_we_admit/) ⭐️ 8.0/10

A Reddit post and associated website (postgresisenough.dev) argue that many teams prematurely adopt specialized databases and services, when PostgreSQL's built-in features for queues, caches, full-text search, and pub/sub are often sufficient for real-world workloads. This challenges the trend of architectural complexity and suggests that teams can reduce operational overhead by leveraging Postgres's versatility, avoiding the cost and maintenance burden of multiple specialized services. The post highlights that Postgres is good enough for queues (e.g., using SKIP LOCKED), caching (using materialized views or UNLOGGED tables), and full-text search (using tsvector and GIN indexes), but admits that for very high throughput or specialized needs, dedicated services may still be required.

reddit · r/programming · /u/danieltabrizian · Jul 9, 19:52

**Background**: PostgreSQL is a powerful open-source relational database that includes features like full-text search, LISTEN/NOTIFY for pub/sub, and advisory locks. Many teams default to adding Redis for caching, Elasticsearch for search, and RabbitMQ for queues, even when Postgres's built-in capabilities could handle the load. The 'Postgres is enough' movement advocates for simpler, boring infrastructure that is easier to debug and maintain.

<details><summary>References</summary>
<ul>
<li><a href="https://leontrolski.github.io/postgres-as-queue.html">leontrolski - postgres as queue</a></li>
<li><a href="https://www.martinheinz.dev/blog/105">You Don't Need a Dedicated Cache Service - PostgreSQL as a ...</a></li>
<li><a href="https://www.postgresql.org/docs/current/textsearch.html">PostgreSQL: Documentation: 18: Chapter 12. Full Text Search</a></li>

</ul>
</details>

**Tags**: `#postgres`, `#database`, `#architecture`, `#simplicity`, `#infrastructure`

---

<a id="item-10"></a>
## [Tencent's Hy3 LLM Stirs OpenRouter Debate](https://hy.tencent.com/research/hy3) ⭐️ 7.0/10

Tencent released Hy3, an open-source Mixture-of-Experts (MoE) language model with 295B total parameters (21B active), alongside a preview version. It has topped OpenRouter rankings and sparked discussions over its pricing compared to DeepSeek Flash V4. Hy3 demonstrates that smaller models can rival much larger ones in capability, potentially reshaping cost efficiency in AI inference. Its availability on OpenRouter with competitive pricing challenges existing providers like DeepSeek. Hy3's effective input price on OpenRouter is now the same as DeepSeek-hosted DeepSeek Flash V4, which is a 284B-parameter MoE model with 13B active parameters. Hy3 includes an extra 3.8B MTP layer for speculative decoding.

hackernews · andai · Jul 9, 15:27 · [Discussion](https://news.ycombinator.com/item?id=48847552)

**Background**: Mixture-of-Experts (MoE) models activate only a subset of parameters per token, allowing large total capacity with efficient computation. Tencent's Hy3 is open-source and built with feedback from 50+ products. OpenRouter is a platform that aggregates AI models, providing rankings and pricing comparisons.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/tencent/Hy3">tencent/Hy3 · Hugging Face</a></li>
<li><a href="https://openrouter.ai/rankings">LLM Rankings | OpenRouter</a></li>
<li><a href="https://api-docs.deepseek.com/news/news260424/">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>

</ul>
</details>

**Discussion**: Commenters note Hy3's surprising capability for its small active parameter size, with some comparing it favorably to DeepSeek V4 Flash and even V4 Pro on benchmarks. However, others question its long-term value given pricing parity with DeepSeek Flash V4 and the free tier expiring soon.

**Tags**: `#AI model`, `#LLM`, `#Tencent`, `#pricing`, `#open-source`

---

<a id="item-11"></a>
## [Postgres Rewritten in Rust Using LLMs, Passes All Tests](https://github.com/malisper/pgrust) ⭐️ 7.0/10

A project called pgrust has rewritten PostgreSQL in Rust using large language models (LLMs) and now passes 100% of the PostgreSQL regression tests, as reported on Hacker News. This demonstrates that LLMs can be used to reimplement complex, decades-old systems like databases, potentially enabling faster innovation and safer rewrites. However, it also raises questions about code quality, licensing, and the need for rigorous testing beyond regression tests. The project changed the license from the PostgreSQL License to AGPL, and the code was generated using LLMs with 7101 commits in under a month, making manual review challenging. The author acknowledges ongoing work on a new version incorporating more advanced techniques.

hackernews · SweetSoftPillow · Jul 9, 06:18 · [Discussion](https://news.ycombinator.com/item?id=48841676)

**Background**: PostgreSQL is a mature, open-source relational database with a comprehensive regression test suite that has evolved over 30 years. Rewriting such a system in a memory-safe language like Rust could reduce bugs but is a massive undertaking. This project used LLMs to automate the translation and code generation, aiming to produce a clean Rust implementation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/regress.html">PostgreSQL: Documentation: 18: Chapter 31. Regression Tests</a></li>
<li><a href="https://arxiv.org/abs/2508.00083">A Survey on Code Generation with LLM-based Agents</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: some praise the technical achievement, while others demand rigorous verification like Jepsen testing and express concerns about the license change and the lack of human-verifiable commit history. The author responds by outlining future work on a rearchitected version.

**Tags**: `#Rust`, `#PostgreSQL`, `#database`, `#reimplementation`, `#LLM`

---

<a id="item-12"></a>
## [No leap second at end of December 2026, IERS announces](https://datacenter.iers.org/data/latestVersion/bulletinC.txt) ⭐️ 7.0/10

The International Earth Rotation and Reference Systems Service (IERS) announced that no leap second will be inserted at the end of December 2026, continuing a period without leap seconds since the last one in December 2016. This decision affects systems that rely on precise time synchronization, such as financial trading, telecommunications, and GPS. It also fuels ongoing debates about the practicality of leap seconds in an increasingly digital world. The UTC-TAI offset remains at -37 seconds, and the UTC-GPS offset at -18 seconds, as no leap second adjustment is needed. Earth's rotation has been relatively fast, reducing the need for leap seconds in the near term.

hackernews · ChrisArchitect · Jul 9, 14:16 · [Discussion](https://news.ycombinator.com/item?id=48846281)

**Background**: A leap second is a one-second adjustment to Coordinated Universal Time (UTC) to keep it close to mean solar time (UT1), which varies due to irregularities in Earth's rotation. Since 1972, 27 positive leap seconds have been added, all on June 30 or December 31. The IERS monitors Earth's rotation and decides about leap seconds about six months in advance. The unpredictability of Earth's rotation makes leap seconds difficult to forecast, posing challenges for time-sensitive digital systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Leap_second">Leap second</a></li>
<li><a href="https://en.wikipedia.org/wiki/International_Earth_Rotation_Service">International Earth Rotation Service</a></li>

</ul>
</details>

**Discussion**: Community members expressed curiosity about the causes of Earth's rotational unpredictability and asked how leap seconds affect UNIX timestamps, particularly for systems in maintenance mode. Some noted the constant offsets between UTC, TAI, and GPS, while others made lighthearted comments about the announcement's preamble and the cost of timekeeping.

**Tags**: `#leap second`, `#timekeeping`, `#UTC`, `#UNIX timestamps`, `#systems`

---

<a id="item-13"></a>
## [Meta Releases Muse Spark 1.1 Agentic AI Model with API](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 7.0/10

Meta has released Muse Spark 1.1, an upgraded agentic AI model, alongside a public API preview for developers. The model is priced at $1.25 per million input tokens and $4.5 per million output tokens, with cached input at $0.15. This release positions Meta as a direct competitor to OpenAI and Anthropic in the agentic AI space, offering a competitively priced model that could disrupt the market. The open-weight nature and API access encourage broad community experimentation, though evaluation methodology debates raise questions about benchmark integrity. According to the evaluation report, Muse Spark 1.1 uses a bash-tool-only agent harness with 6 CPU cores and 8GB RAM, which community members argue violates Terminal-Bench 2.1 task constraints. Developer Simon Willison demonstrated integration via an LLM plugin, and pricing is considered aggressive ($1.25/$4.5 per million tokens).

hackernews · ot · Jul 9, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48846184)

**Background**: Agentic AI models are AI systems capable of autonomously performing multi-step tasks by using tools and following goal-directed instructions. Meta first introduced Muse Spark in April 2026 as its most powerful model, and the 1.1 version now adds developer API access, allowing third-party applications to integrate the model for tasks like code generation and terminal automation.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.meta.com/blog/introducing-muse-spark-msl/">Introducing Muse Spark: Scaling Towards Personal ...</a></li>
<li><a href="https://www.reuters.com/business/meta-debuts-muse-spark-11-with-preview-open-developers-2026-07-09/">Meta debuts Muse Spark 1.1 model with preview open to ...</a></li>

</ul>
</details>

**Discussion**: Community feedback is mixed: some users praise the low pricing and competitive performance, while others criticize the evaluation methodology, noting that the benchmark setup deviates from standard constraints. Developer Simon Willison shared a positive integration experience, and a user suggested Meta could play a 'spoiler' role by commoditizing coding models.

**Tags**: `#AI`, `#Meta`, `#agentic model`, `#open-weight`, `#Hacker News discussion`

---

<a id="item-14"></a>
## [China's Gobi solar plant uses molten salt to generate power after dark](https://electrek.co/2026/07/09/china-hami-solar-molten-salt-storage/) ⭐️ 7.0/10

China Three Gorges Corporation has begun commercial trial operation of the world's largest solar PV-plus-concentrated solar hybrid plant in the Gobi Desert, which uses molten salt thermal storage to deliver electricity for up to eight hours after sunset without lithium batteries. This demonstrates a practical, large-scale alternative to battery storage for renewable energy, potentially reducing reliance on lithium batteries and enabling round-the-clock solar power. It could accelerate global deployment of similar hybrid plants in sunny regions. The 1-gigawatt Hami project in Xinjiang combines photovoltaic panels with concentrated solar power (CSP) towers that heat molten salt, which stores thermal energy for up to eight hours. The plant avoids lithium batteries entirely, relying instead on molten salt thermal energy storage.

rss · Electrek · Jul 9, 19:53

**Background**: Molten salt thermal energy storage works by heating salt to high temperatures (typically ~500°C) using sunlight concentrated by mirrors; the heat can later be used to generate steam and drive turbines. Concentrated solar power (CSP) plants have long used this technology, but combining it with photovoltaics in a hybrid system is relatively new. This hybrid approach allows for cost-effective, dispatchable renewable energy without expensive batteries.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Molten_salt_energy_storage">Molten salt energy storage</a></li>
<li><a href="https://en.wikipedia.org/wiki/Concentrated_solar_power">Concentrated solar power - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#solar energy`, `#molten salt storage`, `#China`, `#renewable energy`, `#energy storage`

---

<a id="item-15"></a>
## [New Jersey bill requires three sensor types, blocking Tesla's camera-only Robotaxi](https://electrek.co/2026/07/09/new-jersey-bill-tesla-camera-robotaxi/) ⭐️ 7.0/10

New Jersey lawmakers introduced bill S1677, which would mandate that driverless commercial vehicles carry cameras plus two additional sensor types (radar and lidar), effectively barring Tesla's camera-only Robotaxi from operating in the state. This bill could set a precedent for other states, potentially reshaping the competitive landscape between Tesla's vision-only approach and the multi-sensor strategies used by Waymo and others. It also reignites the debate over whether cameras alone are sufficient for safe autonomous driving. The proposed law requires cameras, radar, and lidar for any commercial driverless vehicle; Tesla's current Hardware 4.0 and planned Robotaxi lack lidar. Elon Musk has consistently argued that lidar is unnecessary, but many experts disagree.

rss · Electrek · Jul 9, 16:45

**Background**: Autonomous vehicles typically use a combination of cameras, radar, and lidar to perceive the environment. Cameras provide high-resolution color images but struggle in adverse weather and low light; lidar offers precise 3D depth data; radar works well in poor visibility but lacks detail. Tesla has pursued a 'pure vision' approach, relying solely on cameras and neural networks, while most other companies like Waymo use multi-sensor fusion.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Autopilot">Tesla Autopilot - Wikipedia</a></li>
<li><a href="https://insideevs.com/news/738204/tesla-pure-vision-camera-only/">Tesla Bet On 'Pure Vision' For Self-Driving. That's Why It's In Hot Water</a></li>

</ul>
</details>

**Tags**: `#autonomous vehicles`, `#regulation`, `#Tesla`, `#Waymo`, `#sensor technology`

---

<a id="item-16"></a>
## [Bun Rust Rewrite Thoughts Shared by Developer](https://www.reddit.com/r/programming/comments/1urmi6h/my_thoughts_on_the_bun_rust_rewrite/) ⭐️ 7.0/10

A developer on Reddit posted personal thoughts on the potential rewrite of the Bun JavaScript runtime in Rust, sparking discussion in the programming community. If Bun were rewritten in Rust, it could improve performance and reliability, impacting developers who use Bun as a Node.js alternative for faster startup and execution. The original post lacks detailed technical analysis, but the discussion highlights community interest in Bun's architecture. Bun currently uses JavaScriptCore and is written in Zig, not Rust.

reddit · r/programming · /u/simon_o · Jul 9, 10:36

**Background**: Bun is a fast all-in-one JavaScript runtime, package manager, and test runner, designed as a drop-in replacement for Node.js. It uses Safari's JavaScriptCore engine instead of V8 for better startup performance. Rewriting such a tool in a systems programming language like Rust could bring memory safety and concurrency benefits.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://bun.com/docs/runtime">Bun Runtime - Bun</a></li>

</ul>
</details>

**Tags**: `#Bun`, `#Rust`, `#Rewrite`, `#JavaScript`, `#Performance`

---

<a id="item-17"></a>
## [AI-generated content floods social media, especially LinkedIn](https://www.pangram.com/blog/ai-in-your-feed) ⭐️ 6.0/10

A recent blog post highlights the increasing prevalence of AI-generated content on social media platforms, with LinkedIn being a prime example where authenticity is being eroded. This trend matters because it undermines the trust and authenticity that social platforms rely on, potentially driving users away and degrading the overall quality of online discourse. The post is observational rather than groundbreaking, but it has garnered significant community engagement with 170 points and 149 comments, indicating strong resonance among users.

hackernews · mukmuk · Jul 9, 15:50 · [Discussion](https://news.ycombinator.com/item?id=48847940)

**Background**: Social media platforms like LinkedIn have long been places for professional networking and thought leadership. However, AI tools now allow easy generation of posts, leading to an influx of generic, AI-written content that often lacks personal voice and authenticity.

**Discussion**: Commenters express mixed feelings: some argue that AI writing erodes personal voice and authenticity, while others note that LinkedIn has always contained scripted or inauthentic content, and AI merely accelerates the trend. Some users also mention turning to RSS feeds and blogs to escape AI-generated noise.

**Tags**: `#AI`, `#social media`, `#LinkedIn`, `#content quality`, `#authenticity`

---

<a id="item-18"></a>
## [Developers abandon GitHub for Codeberg and self-hosted alternatives](https://www.reddit.com/r/programming/comments/1urm3mh/why_developers_are_ditching_github_for_codeberg/) ⭐️ 6.0/10

A growing number of developers are switching from GitHub to Codeberg, a non-profit Git hosting platform, or self-hosting their code repositories to gain more control and privacy. This shift reflects increasing concerns about vendor lock-in, privacy, and centralization in the software development ecosystem, potentially reshaping how open source projects choose their collaboration platforms. Codeberg is a German non-profit that uses Forgejo, a self-hosted Git service, and offers static pages, CI/CD, and translation tools, while self-hosting gives developers full control over their infrastructure.

reddit · r/programming · /u/Successful_Bowl2564 · Jul 9, 10:15

**Background**: GitHub, owned by Microsoft, is the dominant platform for code hosting, but some developers seek alternatives due to privacy concerns and desire for community governance. Codeberg, as a non-profit, emphasizes transparency and freedom. Self-hosting involves running one's own server, which requires technical expertise but offers maximum control.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Codeberg">Codeberg - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Self-hosting_(network)">Self-hosting (network) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#GitHub`, `#Codeberg`, `#self-hosting`, `#developer tools`, `#open source`

---

<a id="item-19"></a>
## [Pruning on Non-Partitioned Columns in PostgreSQL](https://www.reddit.com/r/programming/comments/1urmnow/how_to_achieve_pruning_when_querying_by/) ⭐️ 6.0/10

A Reddit post discusses techniques to achieve partition pruning in PostgreSQL when querying by non-partitioned columns, such as using constraint exclusion or expression indexes. The post aims to help users optimize queries on partitioned tables where the filter does not involve the partition key. This is significant because it extends the performance benefits of partition pruning to queries that do not filter on the partition key, potentially improving query performance in many real-world scenarios. PostgreSQL users with large partitioned tables can benefit from faster query responses without changing their application logic. The techniques may involve adding CHECK constraints on partitions that reference non-partitioned columns, enabling the query planner to use constraint exclusion to skip irrelevant partitions. However, this approach requires careful maintenance and may be less efficient than native partition pruning, which is based on the partition key.

reddit · r/programming · /u/be_haki · Jul 9, 10:44

**Background**: PostgreSQL's partition pruning automatically eliminates partitions that cannot satisfy the query's WHERE clause when the filter is on the partition key. Constraint exclusion is a similar mechanism that can skip tables or partitions based on CHECK constraints, but it is not as efficient and is often used in older PostgreSQL versions or specific use cases. Understanding both helps in designing optimal partitioning strategies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/ddl-partitioning.html">PostgreSQL: Documentation: 18: 5.12. Table Partitioning</a></li>
<li><a href="https://www.enterprisedb.com/postgres-tutorials/partition-pruning-during-executionpartition-pruning-during-execution">Partition Pruning During ExecutionPartition Pruning During Execution | EDB</a></li>

</ul>
</details>

**Tags**: `#PostgreSQL`, `#database optimization`, `#partitioning`

---