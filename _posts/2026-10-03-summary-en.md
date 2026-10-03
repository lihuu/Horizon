---
layout: default
title: "Horizon Summary: 2026-10-03 (EN)"
date: 2026-10-03
lang: en
---

> From 51 items, 20 important content pieces were selected

---

1. [AI Beats Top Human Stratego Player With 34x Less Training](#item-1) ⭐️ 8.0/10
2. [Zig v0.17.0 release notes spark strong Hacker News discussion](#item-2) ⭐️ 8.0/10
3. [Greg Kroah-Hartman Dissects an LLM&\#x27;s 79 Kernel Bug Claims](#item-3) ⭐️ 8.0/10
4. [Antirez, creator of Redis, releases ds4 local LLM inference engine](#item-4) ⭐️ 7.0/10
5. [Show HN: Opus 5.5 Paints on a Simulated Oil Canvas in Rust](#item-5) ⭐️ 7.0/10
6. [arXiv caps submissions at two per calendar month](#item-6) ⭐️ 7.0/10
7. [iPhone 17 Pro Max turned into a second GPU for a 24 GB MacBook](#item-7) ⭐️ 7.0/10
8. [llama.cpp adds support for decision models](#item-8) ⭐️ 7.0/10
9. [Microsoft releases FrogNano-4B, a 4B agentic coding model built on Qwen3.5-4B](#item-9) ⭐️ 7.0/10
10. [Percepta&\#x27;s Spotlight decouples intelligence from memory to grow knowledge without weight updates](#item-10) ⭐️ 7.0/10
11. [Two 96 GB Huawei Ascend Cards Run Qwen3.8 Flash-Next at 30 tok/s](#item-11) ⭐️ 7.0/10
12. [Apple Launches Official Web-Based Pass Designer for Wallet](#item-12) ⭐️ 6.0/10
13. [12-Year Telescope Sequence Shows a Star and Four Orbiting Exoplanets](#item-13) ⭐️ 6.0/10
14. [Paul Halmos&\#x27;s 1973 Essay &\#x27;The Legend of von Neumann&\#x27; Resurfaces](#item-14) ⭐️ 6.0/10
15. [AllenAI Open-Sources AstaBrief, an 8B Model for Fast Cited Scientific Reports](#item-15) ⭐️ 6.0/10
16. [ServiceNow AI&\#x27;s AutoSynthData Generates Synthetic Training Data for Enterprise Agents](#item-16) ⭐️ 6.0/10
17. [Micro Center Reportedly Requires ID and No-Export Declaration for RTX 5090 Buys](#item-17) ⭐️ 6.0/10
18. [Qwen3.8-27B Humanlike-Chat 2.0 LoRA adds tool calls and better instruction following](#item-18) ⭐️ 6.0/10
19. [NVIDIA Adds 64GB DGX Spark at $5,000, Raises 128GB Model to $6,950](#item-19) ⭐️ 6.0/10
20. [Strata hits 150-200 tok/s decode on a power-limited RTX 5090](#item-20) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [AI Beats Top Human Stratego Player With 34x Less Training](https://arstechnica.com/science/2026/10/ai-finally-beat-the-best-stratego-player-in-history-and-did-it-on-a-budget/) ⭐️ 8.0/10

Researchers published a paper in Nature, with an accompanying arXiv preprint \(2511.07312\), describing an AI system that defeated the best human Stratego player in history. The system reportedly trained roughly 34 times more efficiently than DeepMind&\#x27;s DeepNash, playing far fewer games while ending up stronger. Stratego is an imperfect-information game in which the value of a move depends on facts the player cannot observe, which breaks the lookahead search and credit-assignment machinery that made chess and Go bots so successful. Demonstrating sample-efficient learning here suggests techniques that could transfer to other hidden-information problems such as negotiation, security games, and real-world sequential decision making. The headline technical claim is efficiency: the new algorithm played about 34 times fewer games than DeepNash yet still ended up much stronger, which matters because imperfect-information games make it impossible to simply search ahead over the opponent&\#x27;s hidden setup. DeepMind&\#x27;s DeepNash \(2022\) was a model-free multiagent reinforcement learning approach that was widely described as having &quot;mastered&quot; Stratego, so this result reframes how complete that earlier mastery really was.

hackernews · PaulHoule · Oct 2, 14:11 · [Discussion](https://news.ycombinator.com/item?id=49933740)

**Background**: Stratego is a chess-like two-player board wargame played on a 10x10 board, in which each side secretly places 40 ranked pieces plus bombs and a flag. Because you cannot see the opponent&\#x27;s piece identities and only infer them from combat outcomes, the game is a classic imperfect-information challenge, a category where poker has long served as the standard benchmark for AI research. This hidden information is precisely what makes Stratego fundamentally harder for AI than chess or Go, where the full board state is visible to both players.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stratego">Stratego - Wikipedia</a></li>
<li><a href="https://medium.com/illumination/can-ai-beat-humans-in-games-deepnash-says-yes-27237778127c">Can AI Beat Humans in Games? DeepNash Says Yes! | ILLUMINATION</a></li>
<li><a href="https://boardgamegeek.com/boardgame/1917/stratego">Stratego | Board Game | BoardGameGeek Top Stories Amazon.com: Stratego Original - strategy game Amazon.com: Stratego Board Game Stratego Rules – How to Play, Setup, Strategy, and Winning Stratego Classic Board Game - Target How to Play Stratego: Rules and Tips for Beginners - wikiHow</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely thoughtful rather than dismissive: janalsncm argued that the 34x efficiency gain is the critical piece, since with hidden information the best move depends on facts you cannot know, making lookahead search and credit assignment fundamentally hard. smokel noted that this puts DeepMind&\#x27;s 2022 &quot;mastering the game of Stratego&quot; claim in perspective, since the new approach actually appears to surpass humans. Others added nostalgic anecdotes, including a childhood opponent who subtly marked his pieces and a player who crushed everyone he knew but never imagined serious competitive Stratego existed.

**Tags**: `#AI/ML`, `#game-playing AI`, `#imperfect information`, `#reinforcement learning`, `#research breakthrough`

---

<a id="item-2"></a>
## [Zig v0.17.0 release notes spark strong Hacker News discussion](https://ziglang.org/download/0.17.0/release-notes.html) ⭐️ 8.0/10

The Zig project published the release notes for Zig v0.17.0 on its official download page, marking another point release of the systems programming language and toolchain. The announcement drew 188 upvotes and 98 comments on Hacker News, where developers discussed the language&\#x27;s design quality, its unusually broad target support, and the tooling roadmap. Zig is one of the fastest-growing challengers to C for low-level systems work, so each release signals how quickly it is closing the gap in portability and tooling. The discussion also highlights a maturing ecosystem story: strong language design and target coverage, but still an unstable language and a small library ecosystem that limits near-term production adoption. Commenters singled out Zig&\#x27;s target support as possibly the only serious competitor to C in that regard, and pointed to the new build integration as something that could unlock tooling improvements. The features most anticipated for upcoming releases are a new stackless coroutine IO implementation and first-class fuzzing tooling, while questions remain about the state of evented IO and io\_uring in this version.

hackernews · ErenayDev · Oct 2, 20:56 · [Discussion](https://news.ycombinator.com/item?id=49938521)

**Background**: Zig is a general-purpose systems programming language and toolchain created by Andrew Kelley and first announced in 2016, designed as a general-purpose improvement on C. It avoids macros and preprocessor instructions, requires manual memory management, and adds compile-time generics, arbitrary-width integers and multiple pointer types; development is funded by the Zig Software Foundation through corporate sponsorships and donations. Because Zig emphasizes portability and a self-contained toolchain that can also compile C and C++, its release notes are closely watched by systems and embedded developers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_%28programming_language%29">Zig (programming language)</a></li>
<li><a href="https://ziglang.org/">Home ⚡ Zig Programming Language</a></li>

</ul>
</details>

**Discussion**: Sentiment was strongly positive: one developer with a year of Zig experience called it the best-designed language they had tried, while acknowledging it is still unstable with a small ecosystem. Others praised the target support and build integration, noted that Andrew Kelley is warming up to using LLMs for bug discovery inspired by SQLite&\#x27;s results, and asked about the project&\#x27;s stance on AI and the status of evented IO/io\_uring.

**Tags**: `#zig`, `#programming-languages`, `#systems-programming`, `#compilers`, `#release-notes`

---

<a id="item-3"></a>
## [Greg Kroah-Hartman Dissects an LLM&\#x27;s 79 Kernel Bug Claims](https://www.youtube.com/watch?v=NnV_cWeoo5Q) ⭐️ 8.0/10

In a Kernel Recipes 2026 talk titled &quot;Security in the LLM Age,&quot; Linux kernel maintainer Greg Kroah-Hartman walked through a slide-by-slide breakdown of an LLM \(referred to as &quot;Mythos&quot;\) that claimed to have found 79 Linux kernel vulnerabilities, showing that only 20 actually required fixes and that the entire exercise amounted to roughly one hour of real kernel development work. The talk was posted as a video and quickly became a focal point on Hacker News. This is a data-backed rebuttal from one of the most credible figures in the kernel community, directly challenging the way AI-safety marketing frames LLM vulnerability discovery. It pushes the industry to ask harder questions about attribution, reproducibility, and how LLM-driven security research should actually be evaluated. The slide breakdown was: 24 reports with no detail beyond &quot;something crashed,&quot; 14 that were not bugs at all, 3 with fabricated data, 15 already fixed in the latest release \(11 by others, 4 by Anthropic\), and only 20 that genuinely needed fixes — of which 7 assumed a malicious filesystem image and 2 assumed attacker-controlled input. Kroah-Hartman also characterized the method as pattern matching, taking fix patterns from decades of past kernel patches and applying them elsewhere to see whether they had been universally applied.

hackernews · usernomdeguerre · Oct 2, 02:51 · [Discussion](https://news.ycombinator.com/item?id=49929391)

**Background**: Linux kernel developers receive a constant stream of bug reports, many of which are assigned CVE \(Common Vulnerabilities and Exposures\) identifiers and then triaged, fixed, and backported to stable kernel releases. In recent years LLMs have been increasingly applied to automated code scanning and vulnerability discovery, a fast-growing research area catalogued in resources such as &quot;Awesome-LLM4Cybersecurity.&quot; Kernel Recipes is an annual technical conference for kernel developers, and Greg Kroah-Hartman is one of the longest-serving Linux kernel maintainers, responsible for the stable kernel series.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/tmylla/Awesome-LLM4Cybersecurity">GitHub - tmylla/Awesome-LLM4Cybersecurity: An overview of ...</a></li>
<li><a href="https://arxiv.org/html/2505.01177v1">LLM Security: Vulnerabilities, Attacks, Defenses, and ...</a></li>
<li><a href="https://securityhome.eu/mailings/mailing.php?mid=25179">SecurityHome.eu [USN-7683-1] Linux kernel vulnerabilities</a></li>

</ul>
</details>

**Discussion**: Commenters broadly praised Kroah-Hartman&\#x27;s candor, transcribing the slide data and noting that the &quot;79 vulnerabilities&quot; claim collapsed into roughly one hour of kernel work. Several criticized Anthropic for not crediting the kernel developers who originally fixed those CVEs, while others argued that specialized models trained on kernel-specific code and coding standards could still make bug discovery, analysis, and fixing faster and more accurate in the future.

**Tags**: `#security`, `#llm`, `#linux-kernel`, `#ai-safety`, `#vulnerability-research`

---

<a id="item-4"></a>
## [Antirez, creator of Redis, releases ds4 local LLM inference engine](https://dwarfstar.sh/) ⭐️ 7.0/10

Salvatore Sanfilippo \(&quot;antirez&quot;\), the creator of Redis, has released ds4, a native C inference engine for running large language models locally on Metal, CUDA and ROCm, initially optimized for DeepSeek V4 Flash and later extended to DeepSeek V4.1 Flash, GLM 5.x and Qwen3.8 Flash Next. The project&\#x27;s site dwarfstar.sh hosts documentation, benchmarks and setup notes, and the release has sparked an active Hacker News thread about performance, forks and use cases. Local inference has quietly become one of the most consequential layers of the open-source AI stack, and a well-known systems programmer like antirez entering the space lends it credibility and attention. ds4 lets users run frontier-class open-weight models on high-end consumer hardware without cloud APIs, subscriptions or sending data off-device. ds4 is a small, model-specific engine written in C that targets high-end consumer hardware such as the DGX Spark or AMD Ryzen machines, with experimental vision-model support alongside text inference. Because it is a specialized runner rather than a general-purpose one, its model coverage is narrower than llama.cpp&\#x27;s, and community forks have extended it with shared libraries, FFI bindings and ports to other hardware.

hackernews · fibo · Oct 2, 18:01 · [Discussion](https://news.ycombinator.com/item?id=49936575)

**Background**: Redis is a widely used open-source in-memory data store created by Salvatore Sanfilippo, who is known in the community as &quot;antirez&quot;. Local LLM inference means running open-weight models on your own machine instead of calling a cloud API, using tools such as llama.cpp, Ollama, vLLM and SGLang. ds4 belongs to this ecosystem but takes a different approach: instead of supporting every model format, it is tuned specifically for a handful of large MoE model families to squeeze out speed and long-context performance.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/antirez/ds4">GitHub - antirez/ds4: DeepSeek 4 Flash and PRO local ...</a></li>
<li><a href="https://dwarfstar.sh/">DwarfStar 4 (ds4): Local DeepSeek V4.1, Qwen and GLM</a></li>
<li><a href="https://blog.starmorph.com/blog/local-llm-inference-tools-guide">Local LLM Inference in 2026: The Complete Guide to Tools ...</a></li>

</ul>
</details>

**Discussion**: Commenters are broadly enthusiastic: one maintainer of a fork describes shipping ds4 as shared libraries with FFI bindings and a Go wrapper \(ds4go\), while a user reports it is the best launcher they have tried on an M5 Max with 128GB, running Qwen 3.8 Flash Next with very long context windows. Others note occasional model forgetfulness that may stem from the agent harness rather than ds4, and one developer was inspired to build a separate inference engine \(xenolith\) for Intel Xe-LP laptops.

**Tags**: `#LLM`, `#local inference`, `#ds4`, `#Redis`, `#open source`

---

<a id="item-5"></a>
## [Show HN: Opus 5.5 Paints on a Simulated Oil Canvas in Rust](https://stillwet.art/) ⭐️ 7.0/10

A new Show HN project hosted at stillwet.art gives Claude Opus 5.5 a simulated physical oil-paint canvas — a Rust-based paint simulator paired with an easel — so the model paints by issuing brush strokes through code instead of generating pixels directly. The post drew roughly 180 upvotes and 60 comments on Hacker News, with the underlying code published as the claude-paint repository. It demonstrates a growing alternative to diffusion-based image generation, where AI output is an inspectable, editable source file rather than an opaque raster image — a property that matters for provenance, human learning, and forums that ban generative AI images. It also showcases the agentic coding strengths Anthropic is pushing with Opus 5.5, turning a language model into a tool-using artist. According to the project description, every mark is made the way a painter makes it: simulated bristles carry wet paint over a primed linen canvas, the paint levels and dries on a clock, and layers combine using Kubelka–Munk optics. The code also exposes a &quot;look&quot; tool that lets the model view its own canvas at the provider&\#x27;s best image resolution, which commenters noted is essential for the results to be believable.

hackernews · alstonite · Oct 2, 00:27 · [Discussion](https://news.ycombinator.com/item?id=49928566)

**Background**: Claude Opus 5.5 is Anthropic&\#x27;s flagship model, released on September 22, 2026, positioned as leading in agentic coding and knowledge work while costing about 40% less to run than Opus 5 on typical workloads. Most AI image tools today use diffusion models, which generate pictures by iteratively denoising random noise and give users little insight into how an image was constructed. This project instead has the LLM emit code and tool calls that drive a physics-based paint simulation, so the &quot;painting&quot; is really a program. Kubelka–Munk theory, referenced in the simulator, is a classic model of how light scatters and is absorbed inside pigmented layers such as paint.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49928566">Show HN: Giving Opus 5.5 a simulated paint canvas | Hacker News</a></li>
<li><a href="https://www.anthropic.com/claude-opus-5-5">Introducing Claude Opus 5.5 \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/models/opus-5-5/overview">Claude Opus 5.5 - Claude Platform Docs</a></li>

</ul>
</details>

**Discussion**: Commenters were largely impressed but split on the aesthetics: one noted the landscapes are &quot;ruined&quot; by nonsensical clusters of churches, an uncanny-valley artifact, while another highlighted that the technique can bypass forums that ban generative AI by submitting a process rather than an image. Several participants framed the project as part of a broader shift in which LLMs encroach on diffusion models&\#x27; territory — one speculated Anthropic runs tens of thousands of RL environments recreating famous paintings in code — and others praised the idea that AI artifacts should be inspectable source code, drawing a parallel to music generated as project files.

**Tags**: `#AI art`, `#LLM`, `#Show HN`, `#creative coding`, `#generative AI`

---

<a id="item-6"></a>
## [arXiv caps submissions at two per calendar month](https://blog.arxiv.org/2026/10/01/updated-rate-limit-policy/) ⭐️ 7.0/10

arXiv has announced an updated rate-limit policy that restricts each submitter to at most two submissions per calendar month, published on its official blog. The change applies to the act of submitting to the preprint server rather than to any specific subject area or paper type. arXiv is the primary venue where machine learning and AI researchers share preprints, so a hard cap on monthly submissions directly reshapes how quickly labs and individuals can publicize their work. It is also an explicit attempt to curb the flood of low-quality and AI-generated papers that has strained the server&\#x27;s moderation capacity. The limit is counted per submitter per calendar month, which means large labs could potentially sidestep it by rotating which co-author performs the submission. It follows earlier arXiv measures such as requiring first-time posters to be endorsed by an established arXiv author in their field.

reddit · r/MachineLearning · Nunki08 · Oct 2, 00:47 · [Discussion](https://www.reddit.com/r/MachineLearning/comments/1wvg7yc/arxiv_now_limits_submitters_to_up_to_two/)

**Background**: arXiv is a free, open-access preprint server hosting nearly 2.4 million scholarly articles across physics, mathematics, computer science, quantitative biology and related fields. A preprint is a version of a scholarly paper that is made public before formal peer review and journal publication, which lets results circulate quickly. In recent years the server has faced a surge of AI-generated and low-effort submissions, prompting a series of moderation and eligibility changes.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/">arXiv .org e- Print archive</a></li>
<li><a href="https://en.wikipedia.org/wiki/Preprint">Preprint - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/frommholz_arxiv-preprint-server-clamps-down-on-ai-slop-activity-7422368432240676864-Z6el">ArXiv preprint server clamps down on AI slop | Ingo Frommholz</a></li>

</ul>
</details>

**Discussion**: The reaction was overwhelmingly positive, with commenters calling the change sensible and joking that producing even one paper a month is already a stretch. The main caveat raised was that large &\#x27;paper mill&\#x27; labs will likely game the rule by rotating authorship across their headcount, limiting its real-world effect.

**Tags**: `#arXiv`, `#academic-publishing`, `#research-policy`, `#machine-learning`, `#preprints`

---

<a id="item-7"></a>
## [iPhone 17 Pro Max turned into a second GPU for a 24 GB MacBook](https://v.redd.it/2c6hq3vn33th1) ⭐️ 7.0/10

A developer split Qwen 3.8 27B across a 24 GB M4 Pro MacBook and an iPhone 17 Pro Max, running layers 1–40 on the Mac and layers 41–64 on the phone&\#x27;s A19 Pro GPU over a 10 Gb/s USB-C link. The setup delivered 29–44% faster end-to-end prefill on a 2,000-token file and, past 64k context, moves the oldest KV pages onto the phone so the Mac can keep all 64 layers resident. It demonstrates a practical way to work around the unified-memory ceiling that limits local LLM inference on Apple Silicon, by recruiting idle phone silicon instead of buying more RAM. If the approach generalizes, it could spawn a class of ad-hoc distributed inference setups across consumer Apple devices that users already own. The A19 Pro&\#x27;s GPU matrix units, accessed through Metal 4 tensor ops, make the phone&\#x27;s half of the model 2.4x faster than the same phone without them; measured prefill went from 132 to 177 tok/s at 8k context \(+35%\), 109 to 157 at 16k \(+44%\), 101 to 130 at 32k \(+29%\) and 87 to 113 at 48k \(+30%\), while a cold 27k-token agent session dropped from 245 s on stock llama.cpp to 168 s with the phone. The author also disclosed a metric bug: the prefill TPS displayed on the phone was computed only for the layers it holds, not end-to-end, and is being fixed.

reddit · r/LocalLLaMA · StayLameBro · Oct 2, 16:59 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1wvz1ex/i_made_my_iphone_a_second_gpu_for_my_24_gb/)

**Background**: Apple Silicon uses unified memory shared between CPU and GPU, so a 24 GB MacBook can barely hold a 27B-parameter model at 4-bit precision plus a long context window — the author notes only 64k of 8-bit context fits next to Qwen 3.8 27B in IQ4\_XS, an importance-matrix quantization format in llama.cpp that packs weights at roughly 4.25 bits per weight. Prefill is the compute-heavy phase in which the model ingests the whole prompt before generating tokens, which is why it dominates the wait when an agent reads large files. Metal 4 exposes GPU matrix units through tensor operations in the Metal Shading Language, giving Apple GPUs hardware-accelerated matrix math that the phone exploits here.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/qwen/qwen3.8-27b">Qwen 3.8 27 B - API Pricing &amp; Benchmarks | OpenRouter</a></li>
<li><a href="https://www.local-llm.net/learn/quantization-explained/">Understanding LLM Quantization : GGUF, GPTQ, AWQ... | local-llm.net</a></li>
<li><a href="https://arxiv.org/pdf/2609.32237">Bandwidth, Not FLOPS: FFT Kernels, Matrix Units and SAR Imaging...</a></li>

</ul>
</details>

**Discussion**: The discussion was overwhelmingly positive but mostly humorous rather than technical: the top comment joked that phone prices will skyrocket thanks to the author, and another praised it as an &quot;amazing use of free will.&quot; No substantive technical objections or counterarguments appeared in the provided comments.

**Tags**: `#local-llm-inference`, `#distributed-inference`, `#apple-silicon`, `#metal`, `#gpu-offloading`

---

<a id="item-8"></a>
## [llama.cpp adds support for decision models](https://huggingface.co/blog/ggml-org/decision-models-in-llamacpp) ⭐️ 7.0/10

The GGML team published a blog post on Hugging Face announcing that llama.cpp now supports decision models, a recently emerged class of models. The announcement drew heavy community engagement, with 350 upvotes and a 99% approval ratio. llama.cpp is the de facto core of nearly all local inference tooling such as Ollama and LM Studio, so adding a new model class there makes it immediately runnable on consumer hardware for a very large user base. It also illustrates how quickly model ideas commoditize: a concept hyped as &quot;the next big thing&quot; can be replicated and absorbed into mainstream tooling within weeks. The post comes from the ggml-org account on Hugging Face, and the feature is an incremental addition to llama.cpp rather than a new architecture or benchmark breakthrough. Community members note that &quot;Jev-like&quot; models proliferated in under a month while the original Jev faded away, and users are already asking whether decision models can keep local roleplay characters consistent.

reddit · r/LocalLLaMA · paf1138 · Oct 2, 14:25 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1wvv6im/new_in_llamacpp_decision_models/)

**Background**: llama.cpp is an open-source C/C++ library for running large language models locally, started by Georgi Gerganov in March 2023 and co-developed with the GGML tensor library; it has become the de facto standard core behind most local inference tools, including Ollama and LM Studio. &quot;Decision models&quot; here refers to a recently popularized family of LLM-based models \(exemplified by &quot;Jev&quot;\) rather than the classical decision-theory concept of the same name. Because llama.cpp largely defines what can run on ordinary hardware, support for a new model type is often the moment that type becomes practically usable for hobbyists and small teams.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Llama.cpp">Llama.cpp</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp">GitHub - ggml-org/llama.cpp: LLM inference in C/C++</a></li>
<li><a href="https://en.wikipedia.org/wiki/Decision_model">Decision model</a></li>

</ul>
</details>

**Discussion**: The top comment \(299 points\) argues that Jev is a case study in a hyped idea with no moat: competitors shipped their own versions within weeks, so &quot;Jev-like&quot; models are everywhere while Jev itself is nowhere. Other commenters are more practical, asking whether decision models can stop local roleplay characters from going off the rails mid-scene, and one admits they still don&\#x27;t know what to do with this kind of model.

**Tags**: `#llama.cpp`, `#local LLMs`, `#decision models`, `#open-source AI`, `#model architectures`

---

<a id="item-9"></a>
## [Microsoft releases FrogNano-4B, a 4B agentic coding model built on Qwen3.5-4B](https://huggingface.co/microsoft/FrogNano-4B-2609) ⭐️ 7.0/10

Microsoft published FrogNano-4B-2609 on Hugging Face, a 4B agentic coding model derived from Qwen/Qwen3.5-4B and additionally post-trained for repository-level software engineering. The extra training used reinforcement learning over roughly 1,500 synthetic SWE task environments generated and calibrated against the evolving policy with TaskPilot, with the five-tool Leaf harness and executable test-based rewards over complete multi-turn coding trajectories. It shows that a compact 4B model can be aimed at long-horizon, repository-level software engineering, making agentic coding workflows usable by people with limited GPU resources rather than only by those running large frontier models. It is also notable that Microsoft is fine-tuning a Qwen base model instead of one of its own, and that it deliberately avoids distilling solution traces from stronger models. The additional post-training is text-only, so the multimodal abilities of the Qwen3.5-4B base are not carried over, and the model inherits that base&\#x27;s dense 32-layer hybrid Gated DeltaNet plus gated-attention architecture. Microsoft warns that performance is sensitive to the Leaf harness and test quality, that training data are Python-heavy and primarily English, and that generated patches may be incorrect or insecure even when they pass the available tests.

reddit · r/LocalLLaMA · jacek2023 · Oct 2, 20:16 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1ww40o2/microsoftfrognano4b2609_hugging_face/)

**Background**: Gated DeltaNet is a linear-attention architecture introduced by NVIDIA Labs \(NVlabs\) and published at ICLR 2025; it applies a gated delta rule for memory management and reports better results than Mamba2 and DeltaNet on language modeling, commonsense reasoning, in-context retrieval and long-context tasks. An &quot;agentic coding model&quot; is a language model that runs in a loop with tools — reading and editing files, running shell commands and executing tests — to modify a real code repository. Community quantizations such as GGUF and MLX shrink these models so they can run on consumer GPUs or Apple silicon laptops.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2412.06464">[2412.06464] Gated Delta Networks: Improving Mamba2 with ... GitHub - NVlabs/GatedDeltaNet: [ICLR 2025] Official PyTorch ... Architecture | NVlabs/GatedDeltaNet | DeepWiki [2412.06464] Gated Delta Networks: Improving Mamba2 with ... NVlabs/GatedDeltaNet | DeepWiki [2605.22791] Gated DeltaNet-2: Decoupling Erase and Write in ... Gated DeltaNet | Sebastian Raschka, PhD</a></li>
<li><a href="https://arxiv.org/html/2609.07925">FrogNano: Training a 4B Coding Agent via Online Task Synthesis</a></li>
<li><a href="https://github.com/NVlabs/GatedDeltaNet">GitHub - NVlabs/GatedDeltaNet: [ICLR 2025] Official PyTorch ...</a></li>

</ul>
</details>

**Discussion**: Commenters found the Microsoft-fine-tunes-Qwen combination a &quot;peculiar timeline,&quot; and one user complained that good models now cluster either below 8B or above 27B, leaving a gap in the 14–24B range. Another user quickly published MLX quantizations \(oQ8e, oQ6e, oQ5e\) for Apple silicon, showing immediate practical interest, though the thread stayed light on deep technical evaluation.

**Tags**: `#LLM`, `#agentic coding`, `#Microsoft`, `#Qwen`, `#local models`

---

<a id="item-10"></a>
## [Percepta&\#x27;s Spotlight decouples intelligence from memory to grow knowledge without weight updates](https://v.redd.it/h35la1omc3th1) ⭐️ 7.0/10

Percepta announced Spotlight, a new neural network architecture that replaces attention with a writable, unbounded memory which the model sparsely indexes, so each token reads from and writes to only a small number of memory cells regardless of how large the memory grows. The company says the intelligence module stays the same size and its weights do not change as memory expands, allowing new facts and even new skills to be added without retraining. If the claims hold up, this could reshape long-context and continual-learning research by breaking the usual trade-off between memory capacity and access cost, letting a fixed-size model keep acquiring knowledge and capabilities over time. It also offers a different scaling path from mixture-of-experts and retrieval-augmented generation, which are the dominant approaches today for adding capacity without proportional compute. Percepta claims Spotlight is &quot;arbitrarily sparse&quot;: unlike a mixture-of-experts model, which always activates a fixed number of experts from a fixed set, Spotlight touches the same number of cells no matter how much memory exists, so the fraction of memory used can shrink arbitrarily. The memory is writable and the model itself decides token by token what to load and when to overwrite it, but the announcement is a company blog post with no released paper, code, or benchmark numbers yet.

reddit · r/LocalLLaMA · Recoil42 · Oct 2, 17:47 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1ww09ab/new_architecture_from_percepta_spotlight/)

**Background**: Standard transformer attention compares every token against every other token, so cost grows quickly with context length, which is why long-context work relies on tricks like retrieval-augmented generation, KV caches, or mixture-of-experts layers. Mixture-of-experts models scale parameters cheaply by activating only a fixed subset of experts per token, but that subset size is fixed by design. Spotlight instead splits the system into an intelligence module that performs computation and a separate memory that holds knowledge, procedures, and working state, with the model learning to index individual memory cells so it can retrieve and overwrite them selectively.

<details><summary>References</summary>
<ul>
<li><a href="https://www.percepta.ai/blog/spotlight-memory">Spotlight Memory | Percepta</a></li>
<li><a href="https://korshunov.ai/en/article/30831-percepta-introduces-spotlight-architecture-with-unbounded-memory/">Percepta introduces Spotlight architecture with unbounded ...</a></li>
<li><a href="https://agihunt.info/en/p/1a0fdc811e643b882ab79e36a97">Percepta unveils Spotlight architecture… · AGI Hunt</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion is short and mostly skeptical rather than deeply technical: one commenter asks whether this is essentially just a read/write engram, another shares that they have been experimenting with sparse adaptors on a small lab setup and hopes the research proves useful, and a third simply asks where the claims can be tested.

**Tags**: `#LLM architecture`, `#memory`, `#attention`, `#sparse models`, `#long-context`

---

<a id="item-11"></a>
## [Two 96 GB Huawei Ascend Cards Run Qwen3.8 Flash-Next at 30 tok/s](https://www.reddit.com/r/LocalLLaMA/comments/1wvt1m4/two_96_gb_ascend_cards_crun_qwen38flashnext/) ⭐️ 7.0/10

A builder documented taking a two-card Huawei Atlas 300I Duo machine \(96 GB of device memory per card\) from roughly 1 generated token per second with incoherent output to about 30 tok/s for a single request and roughly 61 tok/s aggregate at four-way concurrency on Qwen3.8 Flash-Next. The same setup also completed the full 198-question GPQA Diamond benchmark, and the post is framed as the start of a guide covering hardware, cooling, memory semantics, vLLM/vLLM-Ascend changes, and remaining open problems. It offers rare, concrete evidence that large-model local inference is viable on non-CUDA Huawei Ascend NPUs, which matters for users priced out of high-VRAM NVIDIA cards. Because the Atlas 300I Duo reportedly sells for under $1500 with 96 GB of memory, a working software recipe could make these surplus cards a practical option for the local-LLM community rather than a paperweight. Each Atlas 300I Duo card actually enumerates as two Ascend 310P3 devices, so two physical cards appear as four NPUs, and the author notes that the nameplate 96 GB per card does not equal the memory actually visible at runtime. The bulk of the work was software-side: ubuntu-26.04 driver support, model architecture support, memory layout, custom operators, and getting every asynchronous state transition exactly right.

reddit · r/LocalLLaMA · matteiuspi · Oct 2, 12:54

**Background**: Huawei&\#x27;s Atlas 300I Duo is a passive, dual-accelerator PCIe inference card built on the Ascend architecture, and it is not a drop-in replacement for CUDA GPUs — it relies on Huawei&\#x27;s own CANN software stack instead. vLLM Ascend \(vllm-ascend\) is a community-maintained hardware plugin that lets the popular vLLM inference server run on Ascend NPUs through vLLM&\#x27;s hardware-pluggable interface. GPQA Diamond is a widely used benchmark of 198 extremely difficult graduate-level biology, physics, and chemistry questions, on which PhD experts score about 65% while skilled non-experts with web access reach only about 34%.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hardware-corner.net/huawei-atlas-300i-duo-96gb-llm-20250830/">Huawei’s Atlas 300I Duo offers 96GB VRAM for local LLMs under ...</a></li>
<li><a href="https://docs.vllm.ai/projects/ascend/en/latest/index.html">vLLM Ascend</a></li>
<li><a href="https://epoch.ai/benchmarks/gpqa-diamond">GPQA Diamond - epoch.ai</a></li>

</ul>
</details>

**Discussion**: Commenters were largely positive but practical: one noted the post is packed with good information yet very long, while others asked how much the setup cost and whether the author will publish the code and modifications so less experienced developers can use these cards more easily. The request for shared code reflects a concern that the optimization work may be too advanced for the average user to reproduce alone.

**Tags**: `#local-llm-inference`, `#huawei-ascend`, `#vllm`, `#hardware-benchmarks`, `#npu-optimization`

---

<a id="item-12"></a>
## [Apple Launches Official Web-Based Pass Designer for Wallet](https://developer.apple.com/pass-designer/) ⭐️ 6.0/10

Apple has released Pass Designer, an official web-based tool at developer.apple.com/pass-designer/ that lets developers visually build Apple Wallet passes instead of hand-authoring the underlying pass files. It is Apple&\#x27;s first first-party design surface for Wallet passes, a task that previously required third-party wizards or manual JSON editing. Wallet passes are widely used for tickets, boarding passes, loyalty cards and event badges, yet creating them has long been a painful, poorly documented process, so an official designer lowers the barrier for the many developers who ship passes. It also signals that Apple is finally investing in the Wallet pass toolchain, though the reaction suggests the move is seen as catch-up rather than innovation. The tool is a browser-based designer rather than a new runtime capability, so it does not by itself change what a pass can do on-device; developers still work with the PKPass format and its associated JSON metadata and images. Notably, the release does not appear to address long-requested framework features such as semantically defined barcode regions for HDR brightness control.

hackernews · soheilpro · Oct 2, 19:06 · [Discussion](https://news.ycombinator.com/item?id=49937276)

**Background**: A Wallet pass is packaged as a .pkpass file, a format Apple developed for storing and exchanging digital passes in its Wallet app; it bundles JSON describing the pass plus images and barcode data, and is cryptographically signed so Wallet will accept it. Because the format was sparsely documented and signing was fiddly, developers historically relied on community-built web wizards and libraries to generate passes. Pass Designer is Apple&\#x27;s attempt to provide an official, first-party path for that same job.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PKPASS">PKPASS - Wikipedia</a></li>
<li><a href="https://www.passcreator.com/en/features/ultimate-guide/pkpass-files-the-apple-wallet-file-format">pkpass Files : The Apple Wallet File Format</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely unimpressed, with several calling the tool roughly a decade too late and pointing to free existing web wizards such as walletwallet.alen.ro. An ex-Apple engineer said he had pushed hard for exactly this tool a dozen years ago and welcomed it as better late than never, while others raised substantive wishes, notably the ability to semantically define a barcode region so Wallet can light up only that rectangle at blinding brightness on HDR displays instead of the whole screen.

**Tags**: `#Apple Wallet`, `#PKPass`, `#Developer Tools`, `#iOS`, `#Design Tools`

---

<a id="item-13"></a>
## [12-Year Telescope Sequence Shows a Star and Four Orbiting Exoplanets](https://bsky.app/profile/theplanetaryguy.com/post/3mwucf5ert22f) ⭐️ 6.0/10

A widely shared animation posted by the account &quot;The Planetary Guy&quot; on Bluesky stitches together roughly 12 years of telescope images into a looping sequence showing a star and four planets orbiting it. The post triggered a discussion among astronomers and enthusiasts about how the visualization was assembled and what it implies for the future of direct exoplanet imaging. Directly imaging planets around other stars is one of the hardest problems in observational astronomy, so a clear, long-baseline visualization helps the public grasp that these worlds are real, moving objects rather than abstract data points. It also builds momentum for next-generation instruments such as the Roman Coronagraph and the Habitable Worlds Observatory, which aim to image fainter, smaller planets. Commenters stressed that this is not a real video: it is built from about 10 static images with a few hundred interpolated &quot;fake&quot; frames filling the gaps. The original creator also mixed data from several different telescopes and wavelengths, whereas one commenter produced an alternative animation using only Keck data at a single near-infrared wavelength of 3.5 microns.

hackernews · mariuz · Oct 2, 11:07 · [Discussion](https://news.ycombinator.com/item?id=49932147)

**Background**: Most of the more than 5,600 known exoplanets were found indirectly, by measuring how a planet dims or tugs on its star. Direct imaging, also called high-contrast imaging, instead tries to block out the overwhelming glare of the star with a coronagraph and sharpen the view with adaptive optics so the faint planet light can be seen. Because planets are millions of times dimmer than their host stars, only a small number of systems have been imaged this way, and the resulting pictures are sparse, requiring interpolation to turn them into smooth animations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/List_of_directly_imaged_exoplanets">List of directly imaged exoplanets - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2404.05797">[2404.05797] Direct imaging of exoplanets - arXiv.org</a></li>
<li><a href="https://science.nasa.gov/mission/roman-space-telescope/direct-imaging/">Direct Imaging - Science@NASA</a></li>

</ul>
</details>

**Discussion**: The discussion was largely appreciative but technically careful: one commenter clarified that the animation is 10 static images plus hundreds of interpolated frames, and another shared a self-made version using only Keck data at a single wavelength for a more consistent comparison. Others expressed excitement about the Roman Coronagraph, which is designed to detect planets 100 million times fainter than their stars \(100 to 1,000 times better than existing space-based coronagraphs\), and about the Habitable Worlds Observatory planned for the 2040s, while several wished there were more such visualizations of nebulae and the galactic center.

**Tags**: `#astronomy`, `#exoplanets`, `#scientific-visualization`, `#telescopes`, `#space`

---

<a id="item-14"></a>
## [Paul Halmos&\#x27;s 1973 Essay &\#x27;The Legend of von Neumann&\#x27; Resurfaces](https://gwern.net/doc/math/1973-halmos.pdf) ⭐️ 6.0/10

Paul Halmos&\#x27;s 1973 essay &quot;The Legend of von Neumann,&quot; hosted as a PDF on gwern.net, was posted to Hacker News and drew 234 points with 136 comments. Nothing new was announced — the item is a resurfacing of a decades-old biographical essay that sparked a fresh round of discussion about von Neumann&\#x27;s influence. Von Neumann is one of the few figures whose work directly shaped modern computing, game theory, quantum mechanics and economics, so retrospectives on him remain relevant to anyone working in those fields. The renewed discussion also shows how the Hacker News community uses classic essays as anchors for debating who really drove 20th-century science. Halmos was himself a prominent mathematician known for work in measure theory and ergodic theory, and the essay is a personal, legend-focused portrait rather than a technical survey of von Neumann&\#x27;s results. The item is a repost: Hacker News previously hosted the same essay in June 2010 \(4 comments\) and August 2014 \(65 comments\), as noted by moderator dang in the thread.

hackernews · suopspaces · Oct 2, 13:18 · [Discussion](https://news.ycombinator.com/item?id=49933235)

**Background**: John von Neumann \(1903–1957\) was a Hungarian-American mathematician whose name is attached to the von Neumann architecture that underlies most computers, to the foundations of game theory, and to key contributions in quantum mechanics, set theory and numerical computing. He was also a member of the informally named &quot;The Martians,&quot; a group of prominent Hungarian Jewish scientists — including Eugene Wigner, Leo Szilard and Edward Teller — who emigrated from Europe to the United States and played outsized roles in 20th-century physics and mathematics. Paul Halmos \(1916–2006\) was a Hungarian-born American mathematician and a well-known expositor, so his essay blends mathematical biography with personal recollection and the mythology that grew up around von Neumann.

**Discussion**: Commenters largely agreed on von Neumann&\#x27;s exceptional stature: one quoted Edward Teller&\#x27;s remark that von Neumann would converse with Teller&\#x27;s three-year-old son &quot;as equals,&quot; while another argued he was more influential in 20th-century science and mathematics than either Einstein or Planck, even if less of an obvious symbol. Others recommended Ananyo Bhattacharya&\#x27;s biography &quot;The Man from the Future&quot; as an accessible longer read and shared a Wikipedia link on &quot;The Martians,&quot; the Hungarian scientist cohort von Neumann belonged to.

**Tags**: `#von-neumann`, `#mathematics`, `#history-of-computing`, `#biography`, `#hackernews-discussion`

---

<a id="item-15"></a>
## [AllenAI Open-Sources AstaBrief, an 8B Model for Fast Cited Scientific Reports](https://huggingface.co/blog/allenai/astabrief) ⭐️ 6.0/10

AllenAI \(Ai2\) has open-sourced AstaBrief, an 8B open-weights model that generates cited scientific reports and now powers the &quot;Fast mode&quot; of the Asta research assistant&\#x27;s report-generation feature. Alongside the model weights, Ai2 released the training data so others can study, reproduce, and build on the approach, with the model available on Hugging Face as allenai/AstaBrief\_8B. The release shows that a small, specialized open model can approach the quality of a proprietary pipeline while running faster and at lower cost, giving researchers and developers a self-hostable alternative to closed APIs for literature-grounded report writing. It also strengthens Ai2&\#x27;s broader Asta ecosystem of scientific AI agents and benchmarks by making a core component reproducible and customizable. AstaBrief is an 8B-parameter model offered both as a hosted &quot;Fast mode&quot; inside Asta and as downloadable weights \(including an SFT variant\) that can be run on your own infrastructure, for example via transformers or vLLM. It sits alongside the Claude-powered &quot;Thinking mode&quot; in Asta, which uses a slower multi-step pipeline that summarizes retrieved snippets, clusters them by theme, and writes the report section by section.

rss · HuggingFace Blog · Oct 2, 15:19

**Background**: Asta is Ai2&\#x27;s scholarly research assistant, announced in August 2025, which draws on more than 108 million abstracts and 12 million full-text papers to find, summarize, and analyze scientific evidence. Its report-generation feature originally ran entirely on a Claude-powered multi-step pipeline, which produced high-quality output but was relatively slow and costly. AstaBrief was built to handle the same task with a much smaller open model, trading a small amount of quality for speed and the ability to run locally.

<details><summary>References</summary>
<ul>
<li><a href="https://allenai.org/blog/astabrief">Open -sourcing AstaBrief , the fast report - generation model in Asta</a></li>
<li><a href="https://huggingface.co/allenai/AstaBrief_8B">allenai / AstaBrief _8B · Hugging Face</a></li>
<li><a href="https://allenai.org/asta">Asta: Advancing Scientific AI with Agents &amp; Benchmarks</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#LLM`, `#report-generation`, `#AI-research`, `#HuggingFace`

---

<a id="item-16"></a>
## [ServiceNow AI&\#x27;s AutoSynthData Generates Synthetic Training Data for Enterprise Agents](https://huggingface.co/blog/ServiceNow-AI/autosynthdata) ⭐️ 6.0/10

ServiceNow CoreAI published AutoSynthData on the Hugging Face blog, a pipeline that turns a target agent&\#x27;s failures and a stronger teacher model&\#x27;s successes into validated synthetic training tasks. The write-up, authored by Esakkivel Esakkiraja, describes how the method decides what the model should learn next and then generates and validates new tasks that exercise those capabilities. Enterprise agent teams often struggle with a shortage of high-quality, domain-specific training data, so a method that automatically converts agent failures into new training tasks could make iterative improvement far cheaper than manual annotation. It reflects a broader industry trend of using synthetic data and teacher-student pipelines to close capability gaps in LLM-based agents. The approach is a two-part loop: it mines failures from the target model and successes from a stronger teacher to select learning targets, then generates and validates new tasks before they enter training. As a vendor blog post on Hugging Face, it has not been peer reviewed and no community discussion or benchmark comparison was provided alongside it.

rss · HuggingFace Blog · Oct 2, 04:01

**Background**: Enterprise AI agents are LLM-driven systems that carry out multi-step tasks inside business workflows, such as IT service management or customer support. Training or fine-tuning them requires task-specific data, but such data is scarce because enterprise environments are private and highly domain-specific. Synthetic data generation addresses this by having models create training examples, often through teacher-student distillation, where a stronger model produces data used to improve a weaker one.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/ServiceNow-AI/autosynthdata">AutoSynthData : Generating Training Data for Enterprise Agents</a></li>
<li><a href="https://www.aiassistantstore.com/blogs/latest-news/servicenow-s-autosynthdata-turns-agent-failures-into-training-gold">aiassistantstore.com/blogs/latest-news/ servicenow -s- autosynthdata ...</a></li>

</ul>
</details>

**Tags**: `#synthetic-data`, `#enterprise-agents`, `#LLM-training`, `#data-generation`, `#AI-agents`

---

<a id="item-17"></a>
## [Micro Center Reportedly Requires ID and No-Export Declaration for RTX 5090 Buys](https://wccftech.com/buying-rtx-5090-at-micro-center-now-requires-paperwork/) ⭐️ 6.0/10

Micro Center has reportedly begun requiring customers buying an Nvidia GeForce RTX 5090 — whether as a standalone card or inside a pre-built system — to present government-issued photo ID for scanning and sign a no-export declaration. Store staff described the process as new, starting roughly two days before the reports, and the form appears to be an &quot;Advanced Computing Product Purchaser Declaration&quot; that collects contact and ID details and states &quot;No exports, No exceptions.&quot; This is one of the first signs that US export controls, which have long targeted data-center AI accelerators like the H100 and H200, are now reaching flagship consumer GPUs. Because the RTX 5090&\#x27;s 32 GB of VRAM makes it popular for local LLM inference, tighter retail-level restrictions could affect hobbyists, small AI startups, and researchers who rely on consumer cards rather than datacenter hardware. The requirement reportedly applies both to standalone cards and to systems with an RTX 5090 pre-installed, and it is enforced at the point of sale rather than through a formal licensing regime. The declaration is a retailer-level document, so it is unclear whether it stems from a government directive, distributor policy, or Nvidia&\#x27;s own compliance push, and whether other retailers will follow.

reddit · r/LocalLLaMA · Boomfrag · Oct 2, 20:35 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1ww4hne/buying_rtx_5090_at_micro_center_reportedly_now/)

**Background**: The GeForce RTX 5090 is Nvidia&\#x27;s flagship consumer GPU, launched in January 2025 as part of the RTX 50 series built on the Blackwell architecture, with 32 GB of GDDR7 memory and a 575 W power rating. US export controls on advanced chips have historically focused on datacenter-class accelerators sold to China and other restricted markets, with licensing rules covering parts such as the H20 and Blackwell datacenter products. Consumer graphics cards were largely exempt from those rules, which is why a retail no-export declaration is notable. The large memory capacity of the 5090 makes it a common choice for running local AI models, blurring the line between gaming hardware and AI compute.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techpowerup.com/353333/micro-center-reportedly-requires-id-and-a-signed-no-export-declaration-for-rtx-5090-sales">Micro Center Reportedly Requires ID and a Signed No - Export ...</a></li>
<li><a href="https://www.tweaktown.com/news/113861/micro-center-starts-asking-rtx-5090-buyers-for-id-and-a-no-export-declaration/index.html">Micro Center starts asking RTX 5090 buyers for ID and a &#x27; No Export ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/RTX_5090">RTX 5090</a></li>

</ul>
</details>

**Discussion**: Commenters reacted with a mix of sarcasm and concern: one joked about needing &quot;FFL-style paperwork&quot; at a &quot;certified Superintelligence dealer&quot; to transfer an old RTX 4090, while another predicted the requirement will spread to all GPUs and AI hardware and eventually extend to locking chips out of running local models. A third commenter expressed hope that China will eventually produce the best GPUs and AI chips so the world can &quot;breathe again,&quot; reflecting a broader frustration with escalating restrictions.

**Tags**: `#export-controls`, `#gpu-hardware`, `#nvidia`, `#ai-hardware`, `#policy`

---

<a id="item-18"></a>
## [Qwen3.8-27B Humanlike-Chat 2.0 LoRA adds tool calls and better instruction following](https://www.reddit.com/gallery/1wvxl4n) ⭐️ 6.0/10

The creator of a Qwen3.8-27B LoRA that makes the model &quot;talk like a person instead of an assistant&quot; released version 2.0 after three weeks of work, directly targeting the three criticisms of v1: replies that were only a few words long, a single default personality that prompting could not change, and tool calls that did not work at all. Version 2.0 now performs working tool calls \(asking for missing information instead of inventing it\), supports character cards, and can switch to formal emails, numbered steps or full explanations on request before returning to casual texting. It shows how cheaply and quickly a small community LoRA can reshape a mid-size open-weight model&\#x27;s behavior, giving local-LLM users a middle ground between robotic assistant speak and a model that refuses to be useful. Working tool calls in particular move such fine-tunes from a novelty into something usable in real agent or automation pipelines. The author reports that v1 accumulated 700+ upvotes, 248 comments and 44k downloads, and that v2 keeps lowercase texting as the default unless the user says &quot;from now on write in full sentences&quot; or puts that in the system prompt — a persistent instruction v1 ignored completely. The post itself is light on technical specifics, offering no training data, hyperparameters or benchmark numbers, so the improvements are currently self-reported rather than independently measured.

reddit · r/LocalLLaMA · kvyb · Oct 2, 16:00 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1wvxl4n/qwen3827bhumanlikechat_20_texts_like_a_human_now/)

**Background**: LoRA \(Low-Rank Adaptation\) is a parameter-efficient fine-tuning technique introduced by Microsoft researchers in 2021 that inserts small trainable matrices into a model&\#x27;s layers, letting you adapt a large model to a new style or task while training only a tiny fraction of the parameters. Qwen3.8-27B is Alibaba&\#x27;s open-weight mid-size multimodal model, designed for coding, visual understanding, tool use and structured output, and it can be run locally through llama.cpp, Ollama or LM Studio. Tool calling \(also called function calling\) is the mechanism where the model outputs a structured request that the surrounding application actually executes — for example a weather lookup — and then feeds the result back to the model to continue reasoning.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/ Qwen 3 . 8 - 27 B · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/LoRA_%28machine_learning%29">LoRA (machine learning) - Wikipedia</a></li>
<li><a href="https://zaingz.medium.com/understanding-tool-calling-how-llms-interact-with-the-real-world-2cd9088b99a8">Understanding Tool Calling : How LLMs Interact with the... | Medium</a></li>

</ul>
</details>

**Discussion**: The comment thread is overwhelmingly playful rather than technical: the top reply jokes about how lonely the model must be, another mocks up a GGUF filename as &quot;hey,you-up-3.8-27b-gguf&quot;, and a third says it &quot;texts like a teenager&quot;. The sentiment is affectionate and engaged, but there is almost no substantive discussion of the fine-tuning itself, which is why the item stays modest in overall value.

**Tags**: `#LocalLLaMA`, `#LoRA`, `#Qwen`, `#fine-tuning`, `#tool-calling`

---

<a id="item-19"></a>
## [NVIDIA Adds 64GB DGX Spark at $5,000, Raises 128GB Model to $6,950](https://i.redd.it/j43l3sia33th1.jpeg) ⭐️ 6.0/10

NVIDIA has introduced a new 64GB configuration of its DGX Spark personal AI computer priced at $5,000, while simultaneously raising the price of the original 128GB model to $6,950 USD. The move marks a notable price increase from the device&\#x27;s earlier positioning, which the community recalls as being announced around $3,000 and launched around $4,000. The pricing shift matters directly to the local-LLM community, since DGX Spark competes with AMD Strix Halo mini-PCs that offer 128GB of unified memory at roughly the same or lower cost. If NVIDIA&\#x27;s entry price rises while a cheaper 64GB variant cannot hold large models, buyers may increasingly favor Strix Halo-based alternatives for running local models. The 64GB variant is seen by community members as limited for large local models, since unified memory capacity is the key constraint for loading big weights. Commenters also note that DGX Spark performance depends heavily on NVFP4 quantization, which requires expensive training to produce good weights, whereas Strix Halo setups running GGUF can reach roughly 50-60 tokens/s decode and 1200-1600 tokens/s prefill.

reddit · r/LocalLLaMA · Norwood\_Reaper\_ · Oct 2, 16:55 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1wvyxzg/new_64gb_dgx_spark_significantly_higher_price_for/)

**Background**: DGX Spark is NVIDIA&\#x27;s compact desktop &\#x27;personal AI supercomputer&\#x27; built on the GB10 Grace Blackwell Superchip, combining an Arm-based Grace CPU with a Blackwell GPU and a large pool of unified memory so that AI models and agents can run locally instead of in the cloud. AMD&\#x27;s Strix Halo \(Ryzen AI Max\) is a competing APU platform that also offers up to 128GB of unified memory in small machines, making it a popular choice for local LLM inference. Quantization formats such as GGUF and NVFP4 determine how model weights are compressed to fit in memory and how fast they run, and the quality of the quantized weights strongly affects output quality.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/products/workstations/dgx-spark/">Personal AI Supercomputer Powered by Blackwell | NVIDIA DGX Spark</a></li>
<li><a href="https://grokipedia.com/page/NVIDIA_DGX_Spark">NVIDIA DGX Spark</a></li>
<li><a href="https://d33gy59ovltp76.cloudfront.net/news/amd-slides-claim-strix-halo-can-beat-the-rtx-4070-laptop-gpu-by-up-to-68-in-modern-games">AMD slides claim Strix Halo can beat the RTX 4070</a></li>

</ul>
</details>

**Discussion**: Sentiment is overwhelmingly negative, with top comments mocking the $5,000 price as ungracious and calling the trajectory from a $3,000 announcement to a $7,000 product a &\#x27;scam.&\#x27; A widely upvoted comment argues that two 128GB Bosgame Strix Halo machines can be bought for $5,000 and, using custom engines like strix-llama, gufo and halogen, match Spark performance when both run GGUF, while also warning that the 64GB Spark is &\#x27;pretty much useless&\#x27; for large models.

**Tags**: `#nvidia`, `#dgx-spark`, `#local-llm`, `#hardware-pricing`, `#strix-halo`

---

<a id="item-20"></a>
## [Strata hits 150-200 tok/s decode on a power-limited RTX 5090](https://i.redd.it/hmr77h6in2th1.png) ⭐️ 6.0/10

A local-inference performance report shows Strata, a standalone local LLM inference engine, running Qwen3.8-Flash-Next at IQ3\_S quantization with a 128k-token context \(8-bit KV cache\) and delivering roughly 150-200 tokens/sec decode and 5-6k tokens/sec prefill on a power-limited RTX 5090 paired with 96GB of DDR5-6400 system memory. It suggests that a single consumer GPU plus system RAM can now serve a large-context model at genuinely interactive speeds, which matters for local-LLM users who want responsive agentic or chat sessions without cloud APIs and who are looking for alternatives to llama.cpp. The run uses IQ3\_S, an importance-matrix-guided 3-bit GGUF quantization, with the KV cache stored at 8-bit precision to keep 128k context within memory limits, and the GPU is explicitly power-limited, so the numbers reflect a deliberately constrained rather than maximum-performance configuration.

reddit · r/LocalLLaMA · z0\_o6 · Oct 2, 15:29 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1wvwssq/strata_on_a_power_limited_5090_and_96gb_of/)

**Background**: Strata is a standalone local inference engine that offers one-click installation on Windows and Linux and exposes OpenAI/Anthropic-compatible APIs on localhost, positioning itself as an alternative to established local runners such as llama.cpp. Qwen3.8-Flash-Next is a Qwen model that uses a hybrid GDN + QSA attention architecture and is distributed in GGUF form by quantizers like Unsloth. IQ3\_S is part of the GGUF quantization family, where the &\#x27;I&\#x27; indicates importance-matrix-based calibration that tries to preserve quality at very low bit widths. In LLM serving, &\#x27;prefill&\#x27; is the prompt-processing phase and &\#x27;decode&\#x27; is the per-token generation phase, so high prefill numbers mean long prompts are ingested quickly while decode numbers determine how fast text streams out.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Niko1221/Strata">GitHub - Niko1221/Strata: Qwen3.8-Flash-Next on any consumer ...</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-Flash-Next">Qwen/Qwen3.8-Flash-Next · Hugging Face</a></li>
<li><a href="https://gist.github.com/Artefact2/b5f810600771265fc1e39442288e8ec9">GGUF quantizations overview · GitHub</a></li>

</ul>
</details>

**Discussion**: Commenters largely corroborate the claim: MindfulMan1984 says Strata is legit after testing it on a 24GB VRAM GPU with 128GB of system RAM, praising its system-detecting setup script and calibration routine as well-optimized for an NVMe SSD + GPU + CPU combination, though noting they have not yet tried whole-repository coding. giveen, who uses nvfp4 for serving Qwen3.8-Flash in their own engine, says they are impressed with Strata&\#x27;s speed, and leonbollerup simply calls it &\#x27;damn nice&\#x27; — the thread is affirming rather than debate-driven.

**Tags**: `#local-llm`, `#inference-engine`, `#quantization`, `#gpu-performance`, `#llama-cpp-alternatives`

---