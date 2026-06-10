---
layout: default
title: "Horizon Summary: 2026-05-13 (EN)"
date: 2026-05-13
lang: en
---

> From 63 items, 34 important content pieces were selected

---

1. [CERT Releases Six CVEs for Serious Dnsmasq Vulnerabilities](#item-1) ⭐️ 9.0/10
2. [Instructure Paid Ransom After Canvas Breach](#item-2) ⭐️ 9.0/10
3. [Transformer language model runs on stock Game Boy Color](#item-3) ⭐️ 9.0/10
4. [750x speedup for minimum line cover of prime points solver](#item-4) ⭐️ 9.0/10
5. [Dennis Ritchie's Lost Dissertation Discovered](#item-5) ⭐️ 9.0/10
6. [Needle: 26M Tool-Calling Model Distilled with Pure Attention](#item-6) ⭐️ 8.0/10
7. [Quack: DuckDB's New Client-Server Protocol](#item-7) ⭐️ 8.0/10
8. [Curated guide on learning software architecture principles](#item-8) ⭐️ 8.0/10
9. [Canada's Bill C-22 Revives Encryption Backdoor Threat](#item-9) ⭐️ 8.0/10
10. [BYD launches Seagull EV with roof LiDAR at $13,000](#item-10) ⭐️ 8.0/10
11. [Tesla Robotaxi convenience issues mask safety validation bottleneck](#item-11) ⭐️ 8.0/10
12. [TabPFN-3 Released: Tabular Foundation Model for 1M Rows](#item-12) ⭐️ 8.0/10
13. [Power Limiting RTX 4090 to 40% Saves Electricity Without Performance Loss](#item-13) ⭐️ 8.0/10
14. [llama-eval tool added to llama.cpp for local model evaluation](#item-14) ⭐️ 8.0/10
15. [Mass npm Supply Chain Attack Hits 170+ Packages](#item-15) ⭐️ 8.0/10
16. [Why Senior Developers Struggle to Communicate Expertise](#item-16) ⭐️ 7.0/10
17. [Rendering Realistic Skies, Sunsets, and Planets with Shaders](#item-17) ⭐️ 7.0/10
18. [DeepMind reimagines mouse pointer with AI and voice](#item-18) ⭐️ 7.0/10
19. [Obsidian Announces Automated Plugin Review System](#item-19) ⭐️ 7.0/10
20. [California deploys 500 MWh sodium-ion battery storage](#item-20) ⭐️ 7.0/10
21. [Rivian Launches 'Hey Rivian' AI Assistant with Full Vehicle Control](#item-21) ⭐️ 7.0/10
22. [Hashimoto Blasts TDM Risk Aversion](#item-22) ⭐️ 7.0/10
23. [MagicQuant v2.0: Hybrid GGUF Quantization Pipeline](#item-23) ⭐️ 7.0/10
24. [Hugging Face Reaches 1 Million Datasets Milestone](#item-24) ⭐️ 7.0/10
25. [Hyundai Integrates EV Powertrain into Modular Units](#item-25) ⭐️ 7.0/10
26. [Waymo Recalls 3,791 Robotaxis Over Flooded Road Incident](#item-26) ⭐️ 6.0/10
27. [Tesla Invests $250M More in Giga Berlin Battery Cells](#item-27) ⭐️ 6.0/10
28. [LLM 0.32a2 adds OpenAI /v1/responses endpoint support and reasoning tokens display](#item-28) ⭐️ 6.0/10
29. [LoRA Meme Sparks ML Community Humor](#item-29) ⭐️ 6.0/10
30. [vLLM vs llama.cpp: Worth It for Single-User Inference?](#item-30) ⭐️ 6.0/10
31. [DIY Tap Water Cooling for DGX AI Hardware](#item-31) ⭐️ 6.0/10
32. [Mazda delays dedicated EV to 2029, pivots to hybrids](#item-32) ⭐️ 6.0/10
33. [Ford TX Plan Offers 15 Hours Free EV Charging Daily](#item-33) ⭐️ 6.0/10
34. [Daily Brief Agentic System for Kids with Receipt Printer](#item-34) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [CERT Releases Six CVEs for Serious Dnsmasq Vulnerabilities](https://lists.thekelleys.org.uk/pipermail/dnsmasq-discuss/2026q2/018471.html) ⭐️ 9.0/10

CERT has disclosed six Common Vulnerabilities and Exposures (CVEs) for serious security vulnerabilities in dnsmasq, a widely-used lightweight network services daemon. The announcement, made on the dnsmasq mailing list, has prompted urgent discussion about patching and memory safety. These vulnerabilities affect a core component of many routers, IoT devices, and Linux systems, putting millions of devices at risk of remote compromise. The disclosure reignites the debate on memory safety in network infrastructure software written in C. The six CVEs cover issues such as buffer overflows and other memory corruption bugs, which can lead to denial of service or arbitrary code execution. Given dnsmasq's role as a DNS forwarder and DHCP server, these vulnerabilities are especially dangerous in home routers and embedded systems.

hackernews · chizhik-pyzhik · May 12, 18:12 · [Discussion](https://news.ycombinator.com/item?id=48112042)

**Background**: Dnsmasq is a free, lightweight software that provides DNS caching, DHCP server, TFTP server, and network boot features for small networks. It is widely used in home routers, Android devices, and many Linux distributions due to its low resource requirements. The software is written in C, a memory-unsafe language, which has historically been a source of vulnerabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dnsmasq">Dnsmasq</a></li>
<li><a href="https://thekelleys.org.uk/dnsmasq/doc.html">Dnsmasq - network services for small networks.</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the urgency of moving to memory-safe languages, with one user proposing Rust or Go as replacements for dnsmasq. Others criticize Debian's slow patching practices and express frustration over the complexity of backporting fixes. Meanwhile, OpenWRT is reportedly working on updated builds to address the CVEs.

**Tags**: `#dnsmasq`, `#security`, `#CVE`, `#network infrastructure`, `#memory safety`

---

<a id="item-2"></a>
## [Instructure Paid Ransom After Canvas Breach](https://www.insidehighered.com/news/tech-innovation/administrative-tech/2026/05/11/instructure-pays-ransom-canvas-hackers) ⭐️ 9.0/10

Instructure, the developer of the Canvas learning management system, confirmed it paid a ransom to hackers who breached its systems and received digital confirmation of data destruction on May 11, 2026. This incident highlights the security risks facing widely used educational platforms and reignites the debate over whether paying ransoms incentivizes further cyberattacks, potentially affecting millions of students and educators. Instructure stated it received digital confirmation of data destruction (shred logs), but security experts caution that such assurances are often unreliable. The breach affected Canvas, a web-based LMS used by thousands of institutions worldwide.

hackernews · Cider9986 · May 12, 02:56 · [Discussion](https://news.ycombinator.com/item?id=48103668)

**Background**: Canvas is a web-based learning management system (LMS) developed by Instructure, widely used by schools and universities for online course delivery. Ransomware attacks typically involve hackers encrypting or stealing data and demanding payment for its return or destruction. Paying ransoms is controversial because it may fund criminal activities and encourage further attacks, though some organizations pay to protect sensitive data from public exposure.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Instructure">Instructure - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters debated the ethics of ransom payments: some argued it fuels the ransomware industry, while others noted that ransomware groups need to maintain credibility to stay in business. Several users expressed skepticism about the reliability of data destruction confirmations, with one calling it 'shockingly naive.' Another suggested creating a public list of organizations that have paid ransoms to inform consumer choices.

**Tags**: `#Security`, `#Ransomware`, `#Education`, `#Canvas`, `#Instructure`

---

<a id="item-3"></a>
## [Transformer language model runs on stock Game Boy Color](https://i.redd.it/1hl9id7ghs0h1.jpeg) ⭐️ 9.0/10

A transformer language model, TinyStories-260K, has been successfully run locally on a stock Game Boy Color using INT8 quantization, fixed-point math, and bank-switched cartridge ROM. This demonstrates that even highly constrained hardware from 1998 can execute a modern transformer model, pushing the limits of edge computing and model compression. The model uses a 260K parameter TinyStories variant, runs via a GBDK-2020 ROM on MBC5 cartridge, and stores the KV cache in cartridge SRAM due to the Game Boy Color's tiny work RAM.

reddit · r/LocalLLaMA · maddiedreese · May 12, 23:15 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1tbi2n3/i_got_a_real_transformer_language_model_running/)

**Background**: The Game Boy Color (1998) has an 8-bit CPU at ~8 MHz, 32 KB work RAM, and no floating-point unit. Transformers typically require powerful GPUs. INT8 quantization reduces model size and enables integer-only arithmetic, while bank switching allows the cartridge to access more than 32 KB of ROM by paging 16 KB banks.

<details><summary>References</summary>
<ul>
<li><a href="https://hackaday.io/project/205074-on-chip-lm-tinystories-260k-on-cortex-m7">On-Chip LM: TinyStories 260K on Cortex-M7 | Hackaday.io</a></li>
<li><a href="https://en.wikipedia.org/wiki/Game_Boy">Game Boy - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/not-lain/kv-caching">KV Caching Explained: Optimizing Transformer Inference Efficiency</a></li>

</ul>
</details>

**Discussion**: The community expressed awe and excitement, with comments like 'Wow just wow' and 'This makes me wanna run a model on my N64.' A user also shared a related joke project running a model on a Game Boy Advance.

**Tags**: `#machine learning`, `#edge computing`, `#hardware`, `#retro computing`, `#LLM`

---

<a id="item-4"></a>
## [750x speedup for minimum line cover of prime points solver](https://prime-line-cover.vercel.app/?article) ⭐️ 9.0/10

A C++ solver using an arithmetic-aware incremental architecture has achieved a world record by reducing the time to solve the minimum line cover for prime points from 282 hours to 22 minutes for N=861, and up to N=1024 in under 40 hours, certifying 20 new awkward primes. This breakthrough demonstrates that domain-specific algorithmic optimizations can dramatically outperform general-purpose solvers, even for NP-complete problems. It also enables the certification of new awkward primes, advancing number theory and computational mathematics. The solver uses 12,162 heavy lines (through 3+ primes) stored as 1024-bit bitmasks to keep the working set in L2 cache, achieves 60% of steps without search via witness propagation, and applies Lagrangian relaxation with projected subgradient descent for lower bounds.

reddit · r/programming · jespergran · May 12, 17:27 · [Discussion](https://www.reddit.com/r/programming/comments/1tb8gv6/i_built_a_world_record_exact_solver_for_the/)

**Background**: The minimum line cover of prime points problem asks for the smallest number of straight lines that can cover all points (i, p_i) for the first N primes. It is NP-complete, meaning exact solutions become exponentially harder as N grows. Previously, Max Alekseyev solved N=861 using an industrial MIP solver over 282 hours. The new solver replaces MIP with custom bitmask-based branch-and-bound, leveraging arithmetic-aware heuristics.

<details><summary>References</summary>
<ul>
<li><a href="https://prime-line-cover.vercel.app/">Prime Line Cover — OEIS A373813</a></li>
<li><a href="https://www.numberphile.com/videos/party-pooper-prime">4211 - The Party Pooper Prime — Numberphile</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lagrangian_relaxation">Lagrangian relaxation - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments express admiration for the work, with user _kelvindecosta praising the website design and interactive visuals. User walen questions whether the speedup is just due to caching previous results, prompting a clarification (implied) that the solver uses fundamentally different algorithms. There is also mention of some downplaying due to perceived AI assistance.

**Tags**: `#optimization`, `#number theory`, `#C++`, `#computational mathematics`, `#prime numbers`

---

<a id="item-5"></a>
## [Dennis Ritchie's Lost Dissertation Discovered](https://computerhistory.org/blog/discovering-dennis-ritchies-lost-dissertation/) ⭐️ 9.0/10

A previously lost dissertation by Dennis Ritchie, co-creator of C and Unix, has been discovered, offering new insights into his early work. This discovery provides a rare glimpse into the foundational thinking behind two of computing's most influential technologies: C and Unix. The dissertation was found by the Computer History Museum and is expected to be digitized and made publicly available.

reddit · r/programming · someone-very-cool · May 12, 15:12 · [Discussion](https://www.reddit.com/r/programming/comments/1tb4jtk/discovering_dennis_ritchies_lost_dissertation/)

**Background**: Dennis Ritchie was a pioneering computer scientist who co-created the C programming language and the Unix operating system at Bell Labs in the 1970s. These innovations became foundational to modern computing, influencing everything from personal computers to the internet. A dissertation from his early career was thought lost for decades.

**Tags**: `#Dennis Ritchie`, `#computer history`, `#dissertation`, `#Unix`, `#C`

---

<a id="item-6"></a>
## [Needle: 26M Tool-Calling Model Distilled with Pure Attention](https://github.com/cactus-compute/needle) ⭐️ 8.0/10

Cactus open-sourced Needle, a 26M parameter function-calling model that uses only cross-attention and gating (no MLPs), achieving 6000 tok/s prefill and 1200 tok/s decode on consumer devices. Needle demonstrates that small, efficient models can outperform larger ones in tool calling, enabling agentic AI on budget phones, wearables, and other edge devices without relying on cloud APIs. The model was pretrained on 200B tokens and post-trained on 2B tokens of synthetic function-calling data generated by Gemini across 15 tool categories. It is MIT-licensed and available on GitHub and Hugging Face.

hackernews · HenryNdubuaku · May 12, 18:03 · [Discussion](https://news.ycombinator.com/item?id=48111896)

**Background**: Tool calling allows AI models to interact with external services (e.g., APIs) by generating structured JSON outputs. Model distillation transfers knowledge from large models to smaller ones. Cross-attention enables the model to focus on relevant input parts, which the authors argue is sufficient for tool calling without need for feed-forward networks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Transformer_(deep_learning)">Transformer (deep learning) - Wikipedia</a></li>
<li><a href="https://ai-sdk.dev/docs/ai-sdk-core/tools-and-tool-calling">AI SDK Core: Tool Calling</a></li>
<li><a href="https://en.wikipedia.org/wiki/Model_distillation">Model distillation</a></li>

</ul>
</details>

**Discussion**: Community comments show interest in browser integration via ONNX, CLI usage for natural language tool parsing, and the push for tiny models. Suggestions include publishing a live demo and clarifying the model size notation (26M vs 0.026B).

**Tags**: `#small models`, `#tool calling`, `#open source`, `#distillation`, `#agentic AI`

---

<a id="item-7"></a>
## [Quack: DuckDB's New Client-Server Protocol](https://duckdb.org/2026/05/12/quack-remote-protocol) ⭐️ 8.0/10

DuckDB has announced Quack, a custom client-server protocol that enables remote connections, horizontal scaling, and multi-user support for the embedded OLAP database. This development transforms DuckDB from a single-user embedded database into a networked database system, allowing teams to share and scale analytical workloads across multiple machines. Quack is a lightweight, purpose-built protocol that communicates over TCP and is designed to leverage DuckDB's columnar engine for efficient OLAP query execution. It does not use standard protocols like PostgreSQL wire protocol.

hackernews · aduffy · May 12, 17:54 · [Discussion](https://news.ycombinator.com/item?id=48111765)

**Background**: DuckDB is an open-source, in-process SQL OLAP database management system designed for fast analytical queries on large datasets. Traditionally, it operates as an embedded database within a single process, limiting it to single-user scenarios. The Quack protocol introduces a server mode, enabling remote clients to connect and execute queries concurrently.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DuckDB">DuckDB - Wikipedia</a></li>
<li><a href="https://duckdb.org/">DuckDB – An in-process SQL OLAP database management system</a></li>

</ul>
</details>

**Discussion**: Community response is generally positive, with users like rglover and ashkankiani expressing excitement about horizontal scaling and remote querying. However, simlevesque questioned DuckDB's evolving identity, and hermitcrab asked whether Quack is suitable for low-concurrency multi-user applications, indicating some uncertainty about best use cases.

**Tags**: `#duckdb`, `#database`, `#client-server`, `#protocol`, `#scaling`

---

<a id="item-8"></a>
## [Curated guide on learning software architecture principles](https://matklad.github.io/2026/05/12/software-architecture.html) ⭐️ 8.0/10

A blog post by a Hacker News reader curates key principles and resources for learning software architecture, emphasizing hands-on experience and minimizing coupling. This high-scoring discussion (514 points, 103 comments) brings together community-validated insights from experienced engineers, offering a practical roadmap for both newcomers and seasoned developers aiming to improve architectural skills. The post recommends resources like 'A Philosophy of Software Design' and 'Architecture of Open Source Applications,' and highlights the importance of maintaining large, multi-team projects to truly learn architecture.

hackernews · surprisetalk · May 12, 09:30 · [Discussion](https://news.ycombinator.com/item?id=48106024)

**Background**: Software architecture refers to the high-level structure of a software system, including its components and their interactions. Coupling, a key concept in software design, measures the degree of interdependence between modules; loose coupling is generally desirable to improve maintainability and flexibility. The discussion builds on these foundational ideas by offering practical advice and curated resources for learning architecture beyond theory.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Loose_coupling">Loose coupling - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/software-engineering/software-engineering-coupling-and-cohesion/">Coupling and Cohesion - Software Engineering - GeeksforGeeks</a></li>
<li><a href="https://codeopinion.com/solid-nope-just-coupling-and-cohesion/">SOLID? Nope, just Coupling and Cohesion - CodeOpinion</a></li>

</ul>
</details>

**Discussion**: Commenters emphasized key principles such as 'coupling is the root of most evil' and 'isolate data transformation from usage,' while recommending classic texts like Shaw/Garlan's 'Software Architecture' and the 'Architecture of Open Source Applications' series. Some pointed out that the original post's recommendations are more about general software development than architecture specifically.

**Tags**: `#software architecture`, `#design principles`, `#learning`, `#engineering culture`

---

<a id="item-9"></a>
## [Canada's Bill C-22 Revives Encryption Backdoor Threat](https://www.eff.org/deeplinks/2026/05/canadas-bill-c-22-repackaged-version-last-years-surveillance-nightmare) ⭐️ 8.0/10

Canada has reintroduced Bill C-22, which includes mandatory data retention and encryption backdoor requirements, effectively repackaging last year's controversial surveillance legislation. If passed, Bill C-22 could force encrypted messaging services like Signal and WhatsApp to block Canadian users or weaken security, threatening global privacy norms and setting a dangerous precedent for other governments. The bill mandates that telecommunications providers retain metadata for two years and requires companies to provide decrypted communications upon request, effectively creating an encryption backdoor.

hackernews · Brajeshwar · May 12, 17:35 · [Discussion](https://news.ycombinator.com/item?id=48111531)

**Background**: Encryption backdoors are covert methods that bypass normal authentication to access encrypted data. Mandatory data retention laws require service providers to store user metadata for law enforcement access. Similar legislation in Australia has faced criticism for undermining privacy and security.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Encryption_backdoor">Encryption backdoor</a></li>
<li><a href="https://www.internetsociety.org/blog/2025/05/what-is-an-encryption-backdoor/">What Is an Encryption Backdoor? - Internet Society</a></li>
<li><a href="https://en.wikipedia.org/wiki/Data_retention">Data retention - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments express strong opposition, with users urging contact with MPs and the Minister of Public Safety. Some note a pattern of repeated legislative attempts, while others see it as a catalyst for innovation in censorship circumvention. A request for a French translation of the EFF article was made to aid local advocacy.

**Tags**: `#privacy`, `#encryption`, `#surveillance`, `#Canada`, `#legislation`

---

<a id="item-10"></a>
## [BYD launches Seagull EV with roof LiDAR at $13,000](https://electrek.co/2026/05/12/byd-launches-seagull-ev-with-lidar-for-13000-first-in-its-class/) ⭐️ 8.0/10

BYD has launched the 2026 Seagull EV, the first A00-class electric vehicle to feature a roof-mounted LiDAR, with a starting price of approximately $13,000. This milestone brings advanced driver-assistance technology (LiDAR) to the entry-level EV segment, potentially accelerating the adoption of smart driving features in affordable cars and challenging industry norms. The LiDAR sensor is mounted on the roof of the vehicle, enabling features like adaptive cruise control and automated parking. The Seagull remains BYD's most affordable EV, now with enhanced autonomous driving capabilities.

rss · Electrek · May 12, 19:24

**Background**: A00-class refers to the smallest segment of microcars, typically with short wheelbases and low prices, popular in China for urban commuting. LiDAR, or Light Detection and Ranging, uses laser pulses to create high-resolution 3D maps of the surroundings and is usually reserved for premium EVs. BYD's move to equip an entry-level model with LiDAR is unprecedented and could pressure other automakers to follow suit.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tesevo.com/blogs/tesla-news/byd-s-cheapest-ev-now-features-roof-mounted-lidar-starting-at-just-13-000">BYD’s Cheapest EV Now Features Roof-Mounted LiDAR Starting at Just $13</a></li>

</ul>
</details>

**Tags**: `#BYD`, `#Electric Vehicles`, `#LiDAR`, `#Autonomous Driving`, `#Affordable EV`

---

<a id="item-11"></a>
## [Tesla Robotaxi convenience issues mask safety validation bottleneck](https://electrek.co/2026/05/12/tesla-robotaxi-convenience-issues-hide-safety-bottleneck/) ⭐️ 8.0/10

A Reuters investigation reveals that Tesla's Robotaxi service suffers from long wait times, surface-street-only routing, and near-zero vehicle availability, which are symptoms of an unresolved safety validation bottleneck that prevents scaling. This matters because it reveals that Tesla's autonomous driving deployment is fundamentally limited by safety validation, not just user experience issues, and highlights a critical barrier to commercial viability of robotaxis. Elon Musk confirmed on the Q1 2026 earnings call that safety validation is the limiting factor, linking degraded user experience directly to safety constraints.

rss · Electrek · May 12, 13:43

**Background**: Autonomous vehicle safety validation involves proving that the system can operate safely in countless edge cases, requiring massive real-world testing and simulation. Scaling a robotaxi service requires passing rigorous safety benchmarks, and if validation is incomplete, operators must limit the service to safe conditions, resulting in poor user experience.

<details><summary>References</summary>
<ul>
<li><a href="https://electrek.co/2026/05/12/tesla-robotaxi-convenience-issues-hide-safety-bottleneck/">Tesla Robotaxi 's 'convenience issues' are hiding the real safety ....</a></li>
<li><a href="https://www.notateslaapp.com/news/3862/tesla-starts-using-cabin-cameras-to-assess-driver-age">Tesla Highlights 2,700-Mile FSD Trip With Zero Interventions</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#Robotaxi`, `#autonomous driving`, `#safety`, `#scalability`

---

<a id="item-12"></a>
## [TabPFN-3 Released: Tabular Foundation Model for 1M Rows](https://www.reddit.com/r/MachineLearning/comments/1tb3fh5/tabpfn3_just_released_a_pretrained_tabular/) ⭐️ 8.0/10

TabPFN-3, the latest iteration of the tabular foundation model originally published in Nature, extends support to 1 million rows on a single H100 GPU, achieves 10-1000x faster inference, and introduces a thinking mode for test-time compute. This release significantly raises the scale and performance bar for tabular machine learning, making foundation models competitive with classical methods like gradient boosting on larger datasets. Practitioners can now handle up to 1M rows without training or hyperparameter tuning, potentially democratizing high-quality tabular prediction. The model uses a reduced KV cache (~8GB per million rows per estimator) and row-chunked inference to scale practically on a single GPU. The thinking mode (API only) outperforms AutoGluon 1.5 extreme by over 200 Elo on TabArena, with a gap of 420 Elo on larger datasets.

reddit · r/MachineLearning · rsesrsfh · May 12, 14:33

**Background**: TabPFN is a transformer-based foundation model for tabular data that performs predictions in a single forward pass without training or hyperparameter tuning. The model leverages KV caching and chunked inference to manage large datasets efficiently. Test-time compute, also known as 'thinking mode,' allocates extra computational resources during inference to improve predictions, similar to techniques used in large language models like OpenAI's o1.

<details><summary>References</summary>
<ul>
<li><a href="https://mbrenndoerfer.com/writing/kv-cache-transformer-attention-optimization">KV Cache Explained: Efficient Attention for LLM Generation - Interactive</a></li>
<li><a href="https://huggingface.co/blog/Kseniase/testtimecompute">What is test - time compute and how to scale it?</a></li>
<li><a href="https://mni-ml.github.io/articles/inference/">LLM Inference | mni-ml</a></li>

</ul>
</details>

**Discussion**: One user noted that TabPFN often outperforms gradient boosting on small-to-medium datasets without feature engineering, and the 1M row support is a big leap. Another expressed skepticism about the trend of applying foundation models to every domain, suggesting it may not always be appropriate.

**Tags**: `#tabular data`, `#foundation model`, `#machine learning`, `#TabPFN`, `#AI`

---

<a id="item-13"></a>
## [Power Limiting RTX 4090 to 40% Saves Electricity Without Performance Loss](https://www.reddit.com/gallery/1tayu5t) ⭐️ 8.0/10

A Reddit user demonstrated that power limiting an RTX 4090 to 40% of its maximum (using nvidia-smi -pl) significantly reduces power consumption during LLM inference with llama.cpp, without any drop in tokens-per-second performance. This practical optimization can reduce electricity costs and heat output for users running large language models locally, and extends GPU lifespan. It also provides a data-driven baseline for power efficiency on high-end GPUs. The user ran llama-server with a 27B Q4_K_XL model, using flash attention and quantization flags. They observed the GPU constantly hitting the power limit, so the actual consumption matches the set limit. Power was set via sudo nvidia-smi -pl <wattage>.

reddit · r/LocalLLaMA · OkFly3388 · May 12, 11:32 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1tayu5t/stop_wasting_electricity/)

**Background**: Power limiting a GPU reduces its maximum power draw, which typically lowers clock speeds and performance, but for some workloads like LLM inference, the GPU may not fully utilize its power budget. nvidia-smi is a command-line tool from NVIDIA to manage GPU settings. llama.cpp is an open-source library for running LLMs efficiently on consumer hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.nvidia.com/deploy/nvidia-smi/">nvidia-smi</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp">GitHub - ggml-org/llama.cpp: LLM inference in C/C++ · GitHub</a></li>
<li><a href="https://huggingface.co/docs/text-generation-inference/en/conceptual/flash_attention">Flash Attention · Hugging Face</a></li>

</ul>
</details>

**Discussion**: One user asked about prefill performance, indicating interest in detailed benchmarks. Another user with an RTX 5090 mentioned capping power out of fear of melting and suggested they should explore further power reduction based on this graph.

**Tags**: `#GPU power optimization`, `#LLM inference`, `#efficiency`, `#RTX 4090`

---

<a id="item-14"></a>
## [llama-eval tool added to llama.cpp for local model evaluation](https://github.com/ggml-org/llama.cpp/pull/21152) ⭐️ 8.0/10

A new tool called llama-eval has been added to the llama.cpp repository via Pull Request #21152, supporting local evaluation of quantized models on standard benchmarks including AIME, GSM8K, and GPQA. This enables developers and researchers to easily benchmark their local quantized models without relying on external APIs or complex setups, addressing a common pain point in the community and facilitating more accessible model comparison and optimization. The tool supports datasets AIME, AIME2025, GSM8K, and GPQA, and is designed to integrate seamlessly with llama.cpp's existing infrastructure for quantized model inference.

reddit · r/LocalLLaMA · jacek2023 · May 12, 12:57 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1tb0uln/examples_add_llamaeval_by_ggerganov_pull_request/)

**Background**: AIME (American Invitational Mathematics Examination) benchmarks test mathematical reasoning, GSM8K is a dataset of grade-school math word problems, and GPQA (Graduate-Level Google-Proof Q&A) evaluates general question-answering at a graduate level. These are widely used standards for assessing LLM performance. llama.cpp is a popular open-source inference engine optimized for running LLMs locally on consumer hardware, often with quantization to reduce memory usage.

<details><summary>References</summary>
<ul>
<li><a href="https://www.vals.ai/benchmarks/aime">AIME</a></li>
<li><a href="https://klu.ai/glossary/GSM8K-eval">GSM8K Benchmark — Klu</a></li>
<li><a href="https://www.vals.ai/benchmarks/gpqa">GPQA</a></li>

</ul>
</details>

**Discussion**: Community members expressed strong approval, with one noting that many benchmarks only support API keys without local server options, making llama-eval a welcome addition. Another user highlighted the flexibility of running benchmarks at home while tinkering, though they joked about the extreme parameters shown (-c 4194304 -np 256) not being typical for home setups. A third user who struggled with lm-eval eagerly anticipates the elegance of this new tool.

**Tags**: `#llama.cpp`, `#model evaluation`, `#benchmarking`, `#local LLM`, `#tools`

---

<a id="item-15"></a>
## [Mass npm Supply Chain Attack Hits 170+ Packages](https://safedep.io/mass-npm-supply-chain-attack-tanstack-mistral/) ⭐️ 8.0/10

A massive npm supply chain attack published malicious versions of over 170 packages, including TanStack and Mistral AI, without compromising any maintainer accounts. This attack highlights the ongoing vulnerability of the npm ecosystem to supply chain attacks, affecting widely-used open-source libraries and potentially millions of downstream users. Over 400 malicious versions were published across 170+ packages, with no maintainer accounts compromised, suggesting the attackers exploited other vectors such as typosquatting or dependency confusion.

reddit · r/programming · BattleRemote3157 · May 12, 03:29 · [Discussion](https://www.reddit.com/r/programming/comments/1tapmvi/mass_npm_supply_chain_attack_hits_tanstack/)

**Background**: Supply chain attacks on npm occur when attackers inject malicious code into packages that are then distributed to users via package managers. Past attacks like event-stream (2018) and axios (2024) have shown how such exploits can target specific applications or cryptocurrency wallets. The lack of maintainer compromise in this attack suggests a different attack vector, possibly through automated bots or compromised CI/CD pipelines.

<details><summary>References</summary>
<ul>
<li><a href="https://apidog.com/blog/axios-attack/">axios@1.14.1 Supply Chain Attack : What to Do Now</a></li>
<li><a href="https://blog.openreplay.com/npm-supply-chain-defense/">A Simple Defense Against npm Supply Chain Attacks</a></li>

</ul>
</details>

**Discussion**: Community comments emphasize proactive mitigation strategies: using private artifactory with a delay, setting `min-release-age=3` in `.npmrc`, and disabling `preinstall/postinstall` scripts via `ignore-scripts=true`. Users generally agree that npm should disable scripts by default to prevent simple exploits.

**Tags**: `#security`, `#npm`, `#supply chain`, `#JavaScript`, `#open source`

---

<a id="item-16"></a>
## [Why Senior Developers Struggle to Communicate Expertise](https://www.nair.sh/guides-and-opinions/communicating-your-expertise/why-senior-developers-fail-to-communicate-their-expertise) ⭐️ 7.0/10

An article explores why senior developers find it difficult to articulate their deep, intuitive expertise, attributing this to an internal 'world model' and proposing methods to bridge the communication gap. This matters because ineffective communication of expertise hinders team productivity, mentorship, and decision-making in software engineering, affecting both individual growth and organizational success. The article introduces the concept of a 'world model' as a mental representation of systems shaped by experience, contrasting it with the mistaken belief that all knowledge can be easily verbalized.

hackernews · nilirl · May 12, 15:08 · [Discussion](https://news.ycombinator.com/item?id=48109460)

**Background**: Senior developers often possess tacit knowledge gained through years of experience, which is hard to convey explicitly. The 'world model' refers to an internalized understanding of how systems work, influencing intuitive decisions. Developing structured communication techniques can help bridge this gap.

**Discussion**: Community comments show mixed reactions: some agree with the world model concept, while others criticize blanket statements. Concerns about AI accelerating codebase complexity and the need for better communication strategies were also raised.

**Tags**: `#senior developers`, `#communication`, `#expertise`, `#soft skills`, `#software engineering`

---

<a id="item-17"></a>
## [Rendering Realistic Skies, Sunsets, and Planets with Shaders](https://blog.maximeheckel.com/posts/on-rendering-the-sky-sunsets-and-planets/) ⭐️ 7.0/10

Maxime Heckel published a detailed blog post explaining how to render realistic skies, sunsets, and planets in real-time in the browser using shaders, raymarching, Rayleigh and Mie scattering, and ozone absorption. This article provides a practical, step-by-step guide for graphics practitioners to implement atmospheric scattering effects on the web, making advanced rendering techniques more accessible and inspiring further experimentation in real-time planet and sky rendering. The implementation is done entirely in the browser using shaders without external libraries, covering both single scattering and multiple scattering approximations; the demo allows interactive parameter adjustments for sun position, atmospheric density, and planet properties.

hackernews · ibobev · May 12, 13:26 · [Discussion](https://news.ycombinator.com/item?id=48107997)

**Background**: Atmospheric scattering is the physical phenomenon where light interacts with air molecules (Rayleigh scattering) and larger particles (Mie scattering), causing the sky to appear blue and sunsets to look red. In computer graphics, these effects are simulated by integrating the scattering along a view ray, often precomputed or approximated in shaders. Ray marching is a technique to sample points along a ray to compute the accumulated light.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.maximeheckel.com/posts/on-rendering-the-sky-sunsets-and-planets/">On Rendering the Sky, Sunsets, and Planets - The Blog of Maxime Heckel</a></li>
<li><a href="https://developer.nvidia.com/gpugems/gpugems2/part-ii-shading-lighting-and-shadows/chapter-16-accurate-atmospheric-scattering">Chapter 16. Accurate Atmospheric Scattering | NVIDIA Developer</a></li>

</ul>
</details>

**Discussion**: Community members praised the post and shared related references: one noted that the sunset demo misses post-sunset twilight (sky turns black too early), another linked Sebastian Lague's planetary atmosphere video, and a third referenced the classic 1993 paper by Nishita et al. on atmospheric scattering.

**Tags**: `#graphics`, `#rendering`, `#atmospheric scattering`, `#computer graphics`, `#planet rendering`

---

<a id="item-18"></a>
## [DeepMind reimagines mouse pointer with AI and voice](https://deepmind.google/blog/ai-pointer/) ⭐️ 7.0/10

DeepMind has proposed a new AI-enhanced mouse pointer that combines voice commands with contextual awareness to simplify cursor-based tasks, allowing users to interact with on-screen elements through natural language. This concept could significantly change human-computer interaction by making complex tasks accessible to non-technical users, while challenging the dominance of traditional keyboard shortcuts and menus. The pointer uses voice prompts like 'add to prompt' and contextual understanding to execute actions such as rearranging elements or applying filters, but it relies on cloud-based AI processing, raising privacy and latency concerns.

hackernews · devhouse · May 12, 17:40 · [Discussion](https://news.ycombinator.com/item?id=48111581)

**Background**: The traditional mouse pointer has remained largely unchanged for decades. DeepMind's proposal integrates LLM-based voice control with visual context, aiming to create a more intuitive interface that understands user intent beyond simple point-and-click.

**Discussion**: Community reactions are mixed. Some users express skepticism, noting that voice commands can be slower and socially awkward, and that existing context menus already achieve similar results. Others see potential for less technical users who struggle with standard shortcuts.

**Tags**: `#AI`, `#human-computer interaction`, `#voice control`, `#pointer`, `#DeepMind`

---

<a id="item-19"></a>
## [Obsidian Announces Automated Plugin Review System](https://obsidian.md/blog/future-of-plugins/) ⭐️ 7.0/10

Obsidian launched a new community site and automated review system to handle the plugin submission backlog, with CEO kepano detailing the roadmap and future improvements. This addresses a major scaling bottleneck in the Obsidian plugin ecosystem, reducing developer frustration and preventing team burnout, while setting a precedent for community-driven security review. The system uses automated checks to assess plugin security, but some community members remain skeptical about its ability to catch malicious code without full sandboxing.

hackernews · xz18r · May 12, 15:45 · [Discussion](https://news.ycombinator.com/item?id=48109970)

**Background**: Obsidian is a popular note-taking app built on Markdown files, known for its extensible plugin system. Previously, all plugins required manual review by the small team, leading to long delays and developer frustration as the volume of submissions grew, especially with AI-assisted plugin development.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Obsidian_(software)">Obsidian (software) - Wikipedia</a></li>
<li><a href="https://obsidian.md/">Obsidian - Sharpen your thinking</a></li>

</ul>
</details>

**Discussion**: CEO kepano expressed excitement about the launch and invited feedback, noting it was a challenging project for a 7-person team. Some users welcomed the relief of the bottleneck, while others questioned the effectiveness of automated security checks and asked about iOS code execution policies.

**Tags**: `#Obsidian`, `#plugins`, `#software engineering`, `#security`, `#scalability`

---

<a id="item-20"></a>
## [California deploys 500 MWh sodium-ion battery storage](https://electrek.co/2026/05/12/california-bets-on-sodium-ion-batteries-for-extreme-heat-regions/) ⭐️ 7.0/10

California has partnered with Juniper Energy and Alsym Energy to deploy 500 MWh of sodium-ion battery storage projects in regions prone to extreme heat. Sodium-ion batteries are safer and more heat-tolerant than lithium-ion, making them ideal for hot climates. This deployment could accelerate adoption of alternative battery chemistries and reduce reliance on lithium supply chains. The 500 MWh projects will be located in California's hottest regions, using Alsym Energy's sodium-ion battery technology. Specific locations and timelines have not been disclosed.

rss · Electrek · May 12, 20:03

**Background**: Sodium-ion batteries use abundant sodium instead of lithium, reducing cost and supply chain risks. They perform better at high temperatures and are less prone to thermal runaway. However, they have lower energy density than lithium-ion, making them more suitable for stationary storage than electric vehicles.

<details><summary>References</summary>
<ul>
<li><a href="https://www.technologyreview.com/2023/05/11/1072865/how-sodium-could-change-the-game-for-batteries/">How sodium could change the game for batteries | MIT Technology</a></li>
<li><a href="https://www.technologyreview.com/2026/01/12/1129991/sodium-ion-batteries-2026-breakthrough-technology/">Sodium-ion batteries: 10 Breakthrough Technologies 2026 | MIT</a></li>

</ul>
</details>

**Tags**: `#energy storage`, `#sodium-ion batteries`, `#renewable energy`, `#California`

---

<a id="item-21"></a>
## [Rivian Launches 'Hey Rivian' AI Assistant with Full Vehicle Control](https://electrek.co/2026/05/12/rivian-hey-rivian-ai-assistant-vehicle-control/) ⭐️ 7.0/10

Rivian has released its new AI-powered voice assistant, 'Hey Rivian,' to all Gen 1 and Gen 2 R1 owners via an over-the-air software update, enabling full vehicle control through voice commands. This move puts Rivian ahead of Tesla, whose Grok assistant still lacks full vehicle control capabilities, and enhances the user experience for Rivian owners with more intuitive interaction. The assistant is activated by saying 'Hey Rivian' or holding the left steering wheel button, and requires an active Connect+ subscription.

rss · Electrek · May 12, 18:15

**Background**: Over-the-air (OTA) updates allow car manufacturers to add features remotely without requiring a dealer visit. Voice assistants in vehicles have become common, but most only handle infotainment tasks; Rivian's integration extends to core vehicle functions like climate control and driving modes.

<details><summary>References</summary>
<ul>
<li><a href="https://rivian.com/connect-plus">Rivian Connect+ - Ever-evolving connectivity for your Rivian</a></li>
<li><a href="https://newslinker.co/tesla-integrates-grok-ai-assistant-with-vehicles-expands-connectivity-options/">Tesla Integrates Grok AI Assistant with Vehicles, Expands</a></li>

</ul>
</details>

**Tags**: `#Rivian`, `#AI assistant`, `#vehicle control`, `#OTA update`, `#EV`

---

<a id="item-22"></a>
## [Hashimoto Blasts TDM Risk Aversion](https://simonwillison.net/2026/May/12/mitchell-hashimoto/#atom-everything) ⭐️ 7.0/10

Mitchell Hashimoto, in a Lobste.rs comment, sharply criticized Technical Decision Makers (TDMs) for being primarily motivated by not getting fired, rather than genuine innovation or technical excellence. This commentary resonates widely in the software industry, highlighting the disconnect between risk-averse enterprise culture and the open-source, meritocratic values of the developer community. Hashimoto specifically cited Gartner and McKinsey as examples of analysts whose trends TDMs follow to justify decisions, using the phrase 'Context Engine for AI Apps' as a satirical example of a buzzword-driven product.

rss · Simon Willison · May 12, 22:21

**Background**: Technical Decision Makers (TDMs) are roles in organizations that choose which technologies, vendors, and architectures to adopt. Hashimoto, co-creator of Vagrant and Terraform, is a well-known figure in the DevOps and infrastructure communities, often offering candid insights.

**Tags**: `#technical-decision-making`, `#industry-commentary`, `#risk-aversion`, `#enterprise-software`

---

<a id="item-23"></a>
## [MagicQuant v2.0: Hybrid GGUF Quantization Pipeline](https://www.reddit.com/r/LocalLLaMA/comments/1tb3sja/magicquant_v20_hybrid_mixed_gguf_models_unsloth/) ⭐️ 7.0/10

MagicQuant v2.0 has been released, introducing a pipeline that automatically creates hybrid GGUF quant mixes by learning from models like Unsloth, and provides benchmark tables showing improved Kullback-Leibler divergence and model size trade-offs. This addresses the critical need for benchmark-driven quantization choices, enabling users to select optimal quant mixes for their available VRAM, which can significantly enhance local LLM deployment efficiency and performance. MagicQuant employs dominance, premium, nonlinear subspace winners, and collapse logic to test and identify the best quantization configurations; it also handles model-specific quirks, such as those found in Qwen3.6 27B, to optimize performance.

reddit · r/LocalLLaMA · crossivejoker · May 12, 14:46

**Background**: Quantization reduces the memory footprint of large language models by lowering the precision of weights, typically from 16-bit to lower bit widths. GGUF is a single-file format for storing quantized models, commonly used with llama.cpp. Kullback-Leibler divergence measures the information loss between the original and quantized model, with lower values indicating better fidelity.

<details><summary>References</summary>
<ul>
<li><a href="https://technewshaven.com/quantizing-llms-step-by-step-converting-fp16-models-to-gguf/">Quantizing LLMs Step-by-Step: Converting FP16 Models to GGUF -</a></li>
<li><a href="https://unsloth.ai/docs/basics/unsloth-dynamic-2.0-ggufs">Unsloth Dynamic 2.0 GGUFs | Unsloth Documentation</a></li>

</ul>
</details>

**Discussion**: The community reacted positively, with one user requesting visualizations similar to Unsloth's balloon graphs for dominance assertion. Another commenter noted that KLD benchmarks are now more common thanks to Unsloth's regular publications, contrasting the earlier lack of benchmarks.

**Tags**: `#quantization`, `#GGUF`, `#LLM`, `#Unsloth`, `#open-source-tools`

---

<a id="item-24"></a>
## [Hugging Face Reaches 1 Million Datasets Milestone](https://i.redd.it/0hc0psqvcq0h1.png) ⭐️ 7.0/10

Hugging Face has announced that its platform now hosts over 1 million publicly available datasets, a significant milestone for open-source AI resources. This milestone underscores the rapid growth of open data in the AI community, enabling more accessible model training and research for developers worldwide. The dataset count covers a wide range of modalities including text, image, audio, and video, contributed by the community. Hugging Face Datasets library provides standardized APIs for easy access.

reddit · r/LocalLLaMA · qlhoest · May 12, 16:07 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1tb64km/1m_datasets_on_hf/)

**Background**: Hugging Face is a leading platform for open-source machine learning, offering hosting for models, datasets, and spaces. The Datasets library is a popular tool that allows users to download and preprocess thousands of datasets with a few lines of code. Reaching 1 million datasets indicates a thriving ecosystem of shared data for AI.

**Discussion**: The comments are lighthearted and not deeply analytical, with users making jokes about 'gooner' datasets and a mention of the anti-AI crowd's criticism of data usage. The overall sentiment is positive but lacks substantive technical discussion.

**Tags**: `#Hugging Face`, `#open datasets`, `#AI`, `#milestone`

---

<a id="item-25"></a>
## [Hyundai Integrates EV Powertrain into Modular Units](https://insideevs.com/news/795470/hyundai-160kw-modular-ev-motor/) ⭐️ 7.0/10

Hyundai has announced a new modular powertrain approach that integrates the motor, inverter, reduction gear, and cooling into a single unit. There will be three power variants: 120kW, 160kW, and 250kW, which can be used in RWD or combined for AWD configurations. This standardization reduces manufacturing complexity and costs, allowing Hyundai to scale EV production across multiple models. It also improves assembly efficiency and serviceability, as components are interchangeable. The modular units cover a power range from 120kW to 500kW when using dual motors for AWD. However, integrating multiple functions into one unit creates a single point of failure, a concern noted by the community.

reddit · r/electricvehicles · willyolio · May 12, 17:26 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1tb8foi/hyundai_is_standardizing_and_integrating_ev/)

**Background**: An inverter converts DC from the battery to AC for the motor, and a reduction gear reduces motor speed while increasing torque. Traditionally, these components are separate, but Hyundai's integrated approach simplifies packaging and cooling.

<details><summary>References</summary>
<ul>
<li><a href="https://industrial.panasonic.com/ww/ds/ss/technical/ap6">What Is an Inverter in an Electric Vehicle? - DC/AC converter efficiently supplying power to motor - - Panasonic</a></li>
<li><a href="https://www.torquetrends.com/">Heavy Duty EV Gearbox Manufacturer, EGSE, 1.90... - Torque Trends</a></li>

</ul>
</details>

**Discussion**: Community comments are generally positive, highlighting the benefits of modularity and interchangeability. One user expressed excitement about swapping high-power motors into smaller used cars for drag racing, while another noted the trade-off of creating a single point of failure.

**Tags**: `#electric vehicles`, `#Hyundai`, `#powertrain`, `#modularity`, `#EV engineering`

---

<a id="item-26"></a>
## [Waymo Recalls 3,791 Robotaxis Over Flooded Road Incident](https://electrek.co/2026/05/12/waymo-recalls-3791-robotaxis-flooded-road-ota-software-fix/) ⭐️ 6.0/10

Waymo voluntarily filed a recall with NHTSA covering 3,791 robotaxis after one vehicle drove into a flooded road in San Antonio last month, with no injuries reported. The fix will be deployed over-the-air (OTA) with no need for physical service visits. This incident highlights ongoing challenges in autonomous vehicle perception of adverse conditions, but the OTA fix demonstrates the industry's ability to address safety issues rapidly without disrupting operations. It reinforces regulatory scrutiny on AV safety while showing that software-defined vehicles can mitigate risks efficiently. Waymo has already implemented interim constraints on its fleet while finalizing the full software remedy. The recall covers all 3,791 vehicles in Waymo's fleet at the time, and no human injuries occurred.

rss · Electrek · May 12, 15:09

**Background**: Autonomous vehicles rely on sensors and AI to navigate, but unusual conditions like flooded roads can pose challenges. OTA updates allow manufacturers to patch software remotely, similar to smartphone updates. NHTSA oversees vehicle safety recalls in the US.

**Tags**: `#Waymo`, `#autonomous vehicles`, `#OTA update`, `#safety recall`

---

<a id="item-27"></a>
## [Tesla Invests $250M More in Giga Berlin Battery Cells](https://electrek.co/2026/05/12/tesla-giga-berlin-250-million-battery-cell-investment-18-gwh/) ⭐️ 6.0/10

Tesla announced an additional $250 million investment in battery cell production at its Giga Berlin factory, more than doubling planned capacity to 18 GWh per year and creating over 1,500 jobs. This investment signals Tesla's commitment to localizing battery production in Europe, reducing reliance on imports, and scaling up output for its electric vehicles. The expansion also comes amid labor disputes, highlighting the intersection of corporate growth and workforce relations. The investment follows a contentious works council election where CEO Elon Musk previously threatened to halt expansion if unions gained control. The new capacity of 18 GWh is expected to supply batteries for Tesla's Model Y production at the same site.

rss · Electrek · May 12, 14:33

**Background**: Giga Berlin is Tesla's first European gigafactory, currently producing the Model Y and ramping up battery cell manufacturing. Battery cells are the core energy storage units for EVs, and Tesla aims to produce them in-house to reduce costs and secure supply chains. The factory has faced regulatory hurdles and labor tensions since its opening.

**Tags**: `#Tesla`, `#battery cells`, `#Giga Berlin`, `#investment`, `#electric vehicles`

---

<a id="item-28"></a>
## [LLM 0.32a2 adds OpenAI /v1/responses endpoint support and reasoning tokens display](https://simonwillison.net/2026/May/12/llm/#atom-everything) ⭐️ 6.0/10

LLM 0.32a2, an alpha release, now uses OpenAI's /v1/responses endpoint for reasoning-capable models and displays reasoning tokens in a different color. Users can hide reasoning output with the -R or --hide-reasoning flag. This update enables interleaved reasoning across tool calls for GPT-5 class models, improving transparency into model thinking. It is a useful incremental improvement for users of the LLM tool who work with OpenAI's reasoning models. The change applies to most reasoning-capable OpenAI models. Reasoning tokens are shown in a different color from standard output, and can be suppressed with the --hide-reasoning flag. This is an alpha release, so it may have instability.

rss · Simon Willison · May 12, 17:45

**Background**: LLM is a command-line tool and Python library for interacting with large language models, created by Simon Willison. OpenAI's /v1/responses endpoint is a newer API that supports advanced agentic workflows, structured outputs, and chain-of-thought reasoning beyond the traditional chat completions endpoint. Reasoning tokens represent the model's internal step-by-step reasoning process, which can now be surfaced to users.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.openai.com/docs/api-reference/responses">platform. openai .com/docs/api-reference/ responses</a></li>
<li><a href="https://wisdom-docs.juheapi.com/api-reference/text/responses">OpenAI Responses API - Wisdom Gate Docs</a></li>

</ul>
</details>

**Tags**: `#llm`, `#openai`, `#reasoning`, `#tool`, `#release`

---

<a id="item-29"></a>
## [LoRA Meme Sparks ML Community Humor](https://i.redd.it/a6oq8jzitr0h1.jpeg) ⭐️ 6.0/10

A Reddit meme puns on the LoRA fine-tuning technique, comparing a child's name 'Lora' to the method, with community comments adding jokes about posterior collapse, Muon optimizer, and Qwen models. While not technically groundbreaking, the meme reflects how machine learning concepts like LoRA have entered common humor among practitioners, indicating the growing cultural footprint of AI. The meme is a play on the term LoRA (Low-Rank Adaptation), with the punchline that the sister's name is Lora. Comments reference posterior collapse (a VAE issue) and the Muon optimizer, linking to recent ML developments.

reddit · r/LocalLLaMA · rwitz4 · May 12, 21:01 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1tbemwa/dad_why_is_my_sisters_name_lora/)

**Background**: LoRA is a parameter-efficient fine-tuning method that injects trainable low-rank matrices into pre-trained models, reducing memory usage. Posterior collapse occurs in variational autoencoders when the latent variable becomes uninformative. Muon is a newer optimizer that applies orthogonalization to momentum updates to accelerate training.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@dsh.2065/fine-tuning-llms-with-lora-and-qlora-from-confusion-to-kinda-working-results-89b348bcce71">Fine-Tuning LLMs with LoRA and QLoRA: From Confusion to (Kinda) Working Results | by Deepesh Sharma | Medium</a></li>
<li><a href="https://arxiv.org/abs/2301.00537">[2301.00537] Posterior Collapse and Latent Variable Non-identifiability</a></li>
<li><a href="https://kellerjordan.github.io/posts/muon/">Muon: An optimizer for hidden layers in neural networks | Keller Jordan blog</a></li>

</ul>
</details>

**Discussion**: Community members engaged humorously: one comment joked about an aunt named 'posterior collapse,' another called for Muon fans, and a third suggested a sibling named Qwen (a model name). The humor leverages specialized ML knowledge.

**Tags**: `#LoRA`, `#fine-tuning`, `#large language models`, `#community humor`

---

<a id="item-30"></a>
## [vLLM vs llama.cpp: Worth It for Single-User Inference?](https://www.reddit.com/r/LocalLLaMA/comments/1tbftlt/is_using_vllm_actually_worth_it_if_you_arent/) ⭐️ 6.0/10

A Reddit debate explores whether vLLM benefits single-user local inference compared to llama.cpp, with users reporting faster prompt processing and better multi-GPU scaling. This discussion matters for local LLM users deciding between vLLM and llama.cpp, highlighting that vLLM's advantages (like batched inference and multi-node support) may still matter for single users with non-trivial workloads. vLLM dynamically allocates VRAM per batch as needed, while llama.cpp pre-allocates for maximum batch size and context. vLLM also offers significantly faster prompt processing on CUDA and supports tensor parallelism across nodes and GPUs.

reddit · r/LocalLLaMA · ayylmaonade · May 12, 21:45

**Background**: llama.cpp is a popular C/C++ library for running LLMs locally with minimal setup, supporting various backends like Vulkan. vLLM is a high-throughput inference engine designed for serving many requests simultaneously, using advanced scheduling and memory management. Both are open-source and widely used in the LLM community.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.vllm.ai/2025/09/05/anatomy-of-vllm.html">Inside vLLM: Anatomy of a High-Throughput LLM Inference System</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp">GitHub - ggml-org/llama.cpp: LLM inference in C/C++ · GitHub</a></li>
<li><a href="https://docs.bentoml.com/en/latest/examples/vllm.html">LLM inference: vLLM - BentoML</a></li>

</ul>
</details>

**Discussion**: Comments highlight that vLLM's batched inference and multi-node support are key advantages for multi-GPU setups, with one user noting it made serving a 397B model across two nodes possible. Another user emphasized that prompt processing speed on CUDA alone makes vLLM worth it, even for single users.

**Tags**: `#vLLM`, `#llama.cpp`, `#local inference`, `#LLM serving`

---

<a id="item-31"></a>
## [DIY Tap Water Cooling for DGX AI Hardware](https://i.redd.it/pmlz1ysv5m0h1.jpeg) ⭐️ 6.0/10

A Reddit user demonstrated a DIY cooling system using tap water for an NVIDIA DGX AI server, keeping GPU temperatures below 68°C at 95% utilization while running the Qwen3.5-122B-A10B model at Q6_K quantization. This shows a low-cost cooling alternative for high-end AI hardware, enabling sustained performance for local LLM inference without expensive liquid cooling systems, and highlights growing community interest in affordable AI infrastructure. The user reports 110 GB memory usage, an 80k context window, and 18.77 tokens/second for continuous vision analysis, but notes uncertainty about water change frequency and long-term reliability.

reddit · r/LocalLLaMA · OldEffective9726 · May 12, 02:05 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1tansuo/found_a_way_to_cool_the_dgx/)

**Background**: DGX systems are NVIDIA's high-performance AI servers designed for deep learning, typically requiring robust cooling. The Qwen3.5-122B-A10B is a large multimodal MoE model with 122B total parameters and only 10B active, optimized for efficiency. Q6_K is a quantization method that uses 6-bit precision for most weights while preserving higher precision for key weights, balancing model size and accuracy. Tap water cooling is unconventional due to risks of corrosion and mineral deposits.

<details><summary>References</summary>
<ul>
<li><a href="https://www.siliconflow.com/models/qwen3-5-122b-a10b">Qwen3.5-122B-A10B - Model Info, Parameters, Benchmarks -</a></li>
<li><a href="https://joshua8.ai/local-llm-benchmark-part2-quantization-ladder/">The Quantization Ladder Has Broken Rungs (Part 2) | Joshua8.AI</a></li>

</ul>
</details>

**Discussion**: Comments praise the creativity with 'finally some art on r/LocalLLaMA' and include a sarcastic remark about water usage, with overall sentiment positive and light-hearted.

**Tags**: `#cooling`, `#AI hardware`, `#DGX`, `#water cooling`, `#local LLM`

---

<a id="item-32"></a>
## [Mazda delays dedicated EV to 2029, pivots to hybrids](https://www.autonews.com/mazda/an-mazda-delays-ev-launch-pivots-to-hybrids-4q-earnings-financial-results-profit-0512/) ⭐️ 6.0/10

Mazda announced it is delaying its first dedicated electric vehicle launch to 2029 and reducing its EV investment, instead focusing on hybrid models. This move highlights Mazda's cautious approach to electrification, contrasting with many automakers accelerating EV plans, and could affect its competitiveness in the growing EV market. The delay pushes the dedicated EV platform to 2029, with reduced investment in EV technology, while Mazda plans to expand its hybrid lineup in the near term.

reddit · r/electricvehicles · TripleShotPls · May 12, 20:56 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1tbehmf/mazda_delays_own_ev_to_2029_slashes_investment/)

**Background**: Mazda has been one of the slowest Japanese automakers to adopt full electrification, historically favoring internal combustion engines and rotary technology. The company's strategy shift mirrors broader industry trends where some automakers are reassessing EV timelines due to infrastructure, cost, and demand challenges.

**Discussion**: Community comments express skepticism, with one user noting the delay is unsurprising given Mazda's slow electrification pace, while another questions why the company is not moving faster. A third comment draws a comparison to Ford, suggesting Ford will outpace Mazda in EV adoption.

**Tags**: `#EV`, `#automotive`, `#Mazda`, `#hybrids`, `#industry strategy`

---

<a id="item-33"></a>
## [Ford TX Plan Offers 15 Hours Free EV Charging Daily](https://www.utilitydive.com/news/txu-energy-ev-charging-program-could-work-in-other-competitive-markets-cha/819483/) ⭐️ 6.0/10

Ford partnered with TXU Energy to offer a retail electricity plan in Texas providing 15 hours per day of free home EV charging. The automaker reports shifting 515 MWh of energy to off-peak periods in 2025. This plan demonstrates innovative EV charging incentives in deregulated markets, potentially influencing utility plans nationwide. However, commenters raise concerns about cost-effectiveness compared to standard time-of-use rates. The plan's standard rate is 17.2 cents per kWh plus 4 cents in TDU charges, totaling over 21 cents per kWh. In contrast, some co-op TOU plans offer off-peak rates as low as 8.6 cents per kWh.

reddit · r/electricvehicles · cleantechguy · May 12, 11:40 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1taz0ra/utility_dive_ford_electric_vehicle_drivers_get_15/)

**Background**: Time-of-use (TOU) plans charge different rates for electricity based on the time of day, encouraging off-peak usage. Texas has a deregulated retail electricity market where consumers can choose among various providers and plans. Free charging periods aim to shift EV load to times of low grid demand.

**Discussion**: Commenters express skepticism about the plan's cost-effectiveness, noting that TXU is generally one of the more expensive providers. One user shares details showing the effective rate is over 21 cents per kWh, while their own TOU plan offers off-peak rates around 8.6 cents. Another raises concerns about Texas road taxes for EVs.

**Tags**: `#electric vehicles`, `#charging infrastructure`, `#energy policy`, `#utility plans`

---

<a id="item-34"></a>
## [Daily Brief Agentic System for Kids with Receipt Printer](https://v.redd.it/20fmi4ed5r0h1) ⭐️ 6.0/10

A developer built an agentic system that uses cron-triggered agents to gather and curate data, renders it into templates, converts to 1-bit dithered images, and prints daily briefs for each child on a phenol-free receipt printer when a button is pressed. This project demonstrates a creative integration of agentic workflows, IoT, and home automation for a personalized, engaging experience for children. It highlights the potential of agentic systems in consumer applications while prompting safety considerations regarding receipt paper chemicals. The system uses a cron job at 1:00am to generate data for three kids, a sidecar web service for rendering and conversion, and HomeAssistant to connect button presses to printing. Button-to-print delay is 2-5 seconds, and the demo uses mock data.

reddit · r/artificial · Boydbme · May 12, 18:46 · [Discussion](https://www.reddit.com/r/artificial/comments/1tbasiz/i_made_an_agentic_daily_brief_for_my_kids_with_a/)

**Background**: Agentic systems are AI systems that perform tasks autonomously using multiple specialized agents coordinated through orchestration. The sidecar pattern is an architectural approach where a helper service runs alongside the main application, sharing resources and lifecycle. 1-bit dithering converts images to black-and-white with patterns to simulate shades, suitable for receipt printers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/agentic-ai">What is Agentic AI? | IBM</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/architecture/patterns/sidecar">Sidecar Pattern - Azure Architecture Center | Microsoft Learn</a></li>
<li><a href="https://niftyutils.com/en/imagetools/image-1bit-dither/">Image to 1-Bit Converter: Retro Pixel Art Dithering Tool</a></li>

</ul>
</details>

**Discussion**: Commenters raised safety concerns about hormone-disrupting chemicals in receipt paper, even non-BPA variants. One commenter suggested using BPA/BPS/phenol-free rolls and provided hardware recommendations. Another suggested an app format to avoid paper waste.

**Tags**: `#agentic`, `#IoT`, `#receipt printer`, `#home automation`, `#children`

---