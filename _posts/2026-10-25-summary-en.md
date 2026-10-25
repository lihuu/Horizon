---
layout: default
title: "Horizon Summary: 2026-10-25 (EN)"
date: 2026-10-25
lang: en
---

> From 49 items, 22 important content pieces were selected

---

1. [Brotli RCE CVE-2026-111497 rebranded from Node2Shell to HTTP2Shell](#item-1) ⭐️ 8.0/10
2. [gpu-unlock: UEFI Exploit Lifts FP/BF16 Issue Rate Caps on RTX 3000 Cards](#item-2) ⭐️ 8.0/10
3. [rqlite Creator Reflects on Twelve Years of Distributed SQLite](#item-3) ⭐️ 8.0/10
4. [Minecraft Runs Inside Bannerlord: Bridging Two Unmodified Engines via Shared Memory](#item-4) ⭐️ 8.0/10
5. [Show HN: &quot;Steal My Bitcoin&quot; Puts a $502 Wallet Behind a PHP RCE](#item-5) ⭐️ 7.0/10
6. [Goose: A Memory-Safe Systems Language With Multiple Data Stacks](#item-6) ⭐️ 7.0/10
7. [HN Debates Why AI Payoff Stays Inside Tech](#item-7) ⭐️ 7.0/10
8. [Live MIDI jam with a pretrained music transformer via logit steering](#item-8) ⭐️ 7.0/10
9. [Kimi K3.1 Open-Weight Release Strips Cyberattack Training Data](#item-9) ⭐️ 7.0/10
10. [Reddit Post Argues KL Divergence Is Misused as a Quantization Ranking Metric](#item-10) ⭐️ 7.0/10
11. [Meta distills Llama 3 8B into 1B byte-level models, predicting they eventually beat token models](#item-11) ⭐️ 7.0/10
12. [8GB GPU Runs 262K-Context Qwen-Flash-Next Coder at 70 T/s via llama.cpp](#item-12) ⭐️ 7.0/10
13. [ANEMLL Forge 0.2.1 runs Qwen3.8-27B on M6 Neural Engine with 192K context](#item-13) ⭐️ 7.0/10
14. [ISTA Ships 1.75–2.25 bpw GSQ/RCO GGUFs of 763B DeepSeek-V4.1-Flash](#item-14) ⭐️ 7.0/10
15. [Roku moves its developer repositories from GitHub to GitLab](#item-15) ⭐️ 6.0/10
16. [FreeDNS Resurfaces on Hacker News, Sparking Public Suffix List Security Debate](#item-16) ⭐️ 6.0/10
17. [2018 Essay on Why Quantum Mechanics Defies Intuition Resurfaces on HN](#item-17) ⭐️ 6.0/10
18. [Unverified Tool Claims 30x/40x Compute Unlock on RTX 30/40 GPUs](#item-18) ⭐️ 6.0/10
19. [Open-Source Browser Rhythm Game Runs Four ONNX Audio Models Locally](#item-19) ⭐️ 6.0/10
20. [Chinese Labs Strip RTX 5090s for Dies and 32GB VRAM to Build AI Servers](#item-20) ⭐️ 6.0/10
21. [Boston Dynamics Employees Petition to Cancel $1.3M Spot Sale to ICE](#item-21) ⭐️ 6.0/10
22. [Reddit Post Claims AWS AI Cloud Capacity Sold Out Through 2027](#item-22) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Brotli RCE CVE-2026-111497 rebranded from Node2Shell to HTTP2Shell](https://www.aikido.dev/blog/python-packages-vulnerable-node2shell-brotli-cve-2026-111497) ⭐️ 8.0/10

A critical Brotli decompression vulnerability tracked as CVE-2026-111497 — an out-of-bounds write that can lead to unauthenticated remote code execution — has been rebranded from &quot;Node2Shell&quot; to &quot;HTTP2Shell&quot; as researchers mapped its blast radius beyond Node.js to Bun, Python, Ruby, Envoy and many other HTTP libraries and applications. Fixes ship in Brotli 1.0.10, 1.1.1 and 1.2.1, with patched runtimes including Node.js 22.23.4, 24.22.1 and 26.12.1. Because Brotli is bundled into so many language runtimes and HTTP stacks, a single decoder flaw becomes a cross-ecosystem RCE risk for anyone terminating or forwarding HTTP traffic, including reverse proxies, load balancers and application middleware. The slow, months-long path from report to coordinated patching also raises questions about how unauthenticated RCE reports are triaged and automated. The bug is an out-of-bounds write triggered when a vulnerable decoder processes specially crafted Brotli data, and it is not strictly HTTP-specific — any code path that manually decodes Brotli, such as decompressing a file or a message payload, can trigger it. The most practical stopgap is to reject incoming requests carrying Content-Encoding: br at the reverse proxy, load balancer or application middleware until the underlying Brotli library is upgraded.

hackernews · theanonymousone · Oct 24, 08:06 · [Discussion](https://news.ycombinator.com/item?id=50219177)

**Background**: Brotli is a general-purpose lossless compression algorithm developed by Google and widely used on the web; HTTP servers and clients negotiate it through the Content-Encoding: br header, and it is also used for static assets and compressed payloads. Because decompression libraries are typically written in C for speed and are fed untrusted input, memory-safety bugs in them are especially dangerous — a malformed compressed stream can corrupt memory before any application-level authentication or validation happens. This CVE was originally reported in February as an unauthenticated bidirectional RCE but was not treated as a security issue at the time, and no release shipped with the fix until now.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aikido.dev/blog/node2shell-nodejs-brotli-rce-cve-2026-111497">Node2Shell: Node.js Brotli vulnerability allows remote code execution...</a></li>
<li><a href="https://brandefense.io/blog/http2shell-brotli-cve-2026-111497/">HTTP2Shell Fixed Versions by Stack - Brandefense</a></li>
<li><a href="https://thehackernews.com/2026/10/nodejs-brotli-decoder-bug-could-allow.html">Node.js Brotli Decoder Bug Could Allow Remote Code Execution ...</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News were largely critical of the &quot;HTTP2Shell&quot; branding, calling it meaningless and overly broad, and several preferred names like &quot;Brotli2Shell&quot; or &quot;Broccoli2Shell&quot;; they also stressed that the flaw is not HTTP-specific since manual Brotli decoding triggers it too. Others questioned how an unauthenticated bidirectional RCE reported in February went unrecognized for so long — speculating about AI-driven automation with &quot;nobody at the wheel&quot; — and expressed surprise at how many projects support Brotli-compressed request bodies at all, with the general mood being &quot;patch your stuff and move on.&quot;

**Tags**: `#security`, `#vulnerability`, `#brotli`, `#http`, `#cve`

---

<a id="item-2"></a>
## [gpu-unlock: UEFI Exploit Lifts FP/BF16 Issue Rate Caps on RTX 3000 Cards](https://github.com/Zagitta/gpu-unlock) ⭐️ 8.0/10

Developer Zagitta has published gpu-unlock 1.0.0, a UEFI-based firmware module that removes the FP/BF16 instruction issue rate cap on Nvidia GeForce RTX 3000-series \(GA102\) consumer cards, bringing their matrix-math throughput closer to professional-grade equivalents. Instead of patching the Nvidia driver, it exploits a classic stack buffer overflow in the card&\#x27;s booter and uses Return Oriented Programming \(ROP\) to apply the unlock before the OS driver ever loads. If the gains hold, owners of consumer GeForce cards could get substantially higher FP16/BF16 matrix throughput for machine-learning workloads without paying for pro-grade hardware, undercutting a segmentation boundary Nvidia enforces in firmware. It also reinforces a growing pattern of community firmware-level unlocks — following the earlier turing-unlock project and the open-gpu-kernel-modules P2P patch — that bypass restrictions Nvidia imposes on cheaper cards. The reported gains come from doubling the FP/BF16 FMA-into-FP32 instruction issue rate on GA102 chips, and community testers say outputs before and after the unlock were bit-identical, so correctness is not affected. The trade-offs are real: the card runs hotter, realizing the full payoff on some cards requires raising the power limit to around 450W — well beyond what the stock cooler was designed for — and the whole approach depends on exploiting a firmware vulnerability, which carries bricking risk.

hackernews · fragebogen · Oct 24, 09:58 · [Discussion](https://news.ycombinator.com/item?id=50219700)

**Background**: Nvidia&\#x27;s consumer GeForce cards often use the same silicon as its professional RTX A-series parts, but firmware and driver restrictions keep certain throughput paths — such as how many FP16/BF16 fused-multiply-add operations can be issued per cycle — below what the hardware can physically do. FP16 and BF16 are the low-precision number formats used heavily in AI training and inference, so instruction issue rate directly affects matrix-multiplication speed. Because the cap is applied at the firmware level, a UEFI module that runs before the operating system and its GPU driver can lift it in a way a driver patch cannot easily be reverted. Similar standalone UEFI unlock modules previously circulated for Nvidia&\#x27;s CMP 90/50 HX mining cards on Windows.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Zagitta/gpu-unlock">GitHub - Zagitta/gpu-unlock: Unlock FP/BF16 instruction issue ...</a></li>
<li><a href="https://daily.dev/posts/gpu-unlock-fp-bf16-instruction-issue-rate-on-nvidia-3000-s-cards-kbbkhu5nr">GPU-unlock: FP/BF16 instruction issue rate on Nvidia...</a></li>
<li><a href="https://aiweekly.co/alerts/zagitta-releases-gpu-unlock-lifts-fp16bf16-caps-on-rtx-3000s">Zagitta Releases gpu-unlock, Lifts FP16/BF16 Caps on RTX ...</a></li>

</ul>
</details>

**Discussion**: The author \(Zagitta\) joined the thread, credited the underlying exploits to others, and explained the project mainly repackages the technique so users don&\#x27;t have to patch the Nvidia driver, inspired by the CMP 90/50 Windows unlocks. Commenters linked related work — nlzy&\#x27;s turing-unlock for Turing-generation cards and aikitoria&\#x27;s open-gpu-kernel-modules patch that restores roughly 20% card-to-card P2P bandwidth on consumer GPUs — while jacquesm flagged practical caveats about heat and the 450W power ceiling. Tiberium reported independently verifying the results and called them legitimate but risky, and noted ports exist for the RTX 4090 and 4070 Ti Super.

**Tags**: `#GPU`, `#Nvidia`, `#firmware-exploitation`, `#hardware-modding`, `#performance`

---

<a id="item-3"></a>
## [rqlite Creator Reflects on Twelve Years of Distributed SQLite](https://philipotoole.com/twelve-years-of-distributed-sqlite/) ⭐️ 8.0/10

Philip O&\#x27;Toole published a twelve-year retrospective on building rqlite, the distributed relational database he created on top of SQLite, tracing the project&\#x27;s evolution and the engineering lessons behind it. The post drew heavy attention on Hacker News \(359 points, 62 comments\), turning into a broader debate about how distributed SQLite engines should be built and operated. rqlite is one of the most widely used ways to get high availability out of SQLite, so a long-horizon retrospective from its creator is a rare, first-hand account of the trade-offs in replicating an embedded database. The discussion it triggered highlights that the &quot;distributed SQLite&quot; space is now crowded — Raft-based systems, WAL-replication experiments, and managed offerings like Cloudflare D1 — with meaningfully different guarantees. rqlite pairs SQLite with the Raft consensus algorithm to provide leader election, log replication, quorum commits, and split-brain prevention across a cluster. A recurring caveat raised in the thread is that rqlite does not officially support SQLite&\#x27;s BEGIN/COMMIT multi-statement transactions, which is a hard dividing line for applications that depend on them.

hackernews · otoolep · Oct 24, 01:16 · [Discussion](https://news.ycombinator.com/item?id=50217500)

**Background**: SQLite is an embedded, single-file relational database used on billions of devices, but it ships with no built-in replication, so every node is on its own. Distributed SQLite projects solve this by wrapping the SQLite engine in a consensus layer — typically Raft — that replicates writes to a quorum of nodes before acknowledging them, giving a cluster that survives node failures while keeping SQLite&\#x27;s simplicity. rqlite is the best-known implementation of this pattern, packaging the whole thing as a single lightweight binary that is easy to install and operate.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/rqlite/rqlite">GitHub - rqlite/rqlite: The lightweight, fault-tolerant ...</a></li>
<li><a href="https://rqlite.io/">rqlite</a></li>
<li><a href="https://www.sqliteforum.com/p/distributed-sqlite-with-raft">Distributed SQLite with Raft for High Availability</a></li>

</ul>
</details>

**Discussion**: Commenters pushed back on managed alternatives, with one practitioner calling Cloudflare D1 &quot;not very reliable&quot; in production and citing a D1 developer&\#x27;s remark that Durable Objects storage is often the better choice. Others asked for a comparison table across engines covering external dependencies, single-leader versus any-node writes, and library versus server shape, arguing that transaction support is the key dividing line since rqlite lacks official BEGIN/COMMIT. Several shared their own designs — a Paxos-based multi-master SQLite using WAL replication \(zaxonlite\) benchmarked against rqlite, and an Odin-language variant — while one commenter argued that with modern tooling it is now easier to just run PostgreSQL than to work around SQLite&\#x27;s SQL limitations.

**Tags**: `#distributed-systems`, `#sqlite`, `#rqlite`, `#databases`, `#replication`

---

<a id="item-4"></a>
## [Minecraft Runs Inside Bannerlord: Bridging Two Unmodified Engines via Shared Memory](https://www.reddit.com/r/programming/comments/1xemwgr/bridging_two_unmodified_game_engines_at_runtime/) ⭐️ 8.0/10

A developer published an MIT-licensed side project that lets Minecraft&\#x27;s player fight inside Mount &amp; Blade II: Bannerlord, linking the two completely unmodified engines through five named shared-memory blocks. The system consists of a C\# Bannerlord module built on Harmony patches, a Java 25 Fabric mod using Mixin and the Foreign Function &amp; Memory API, and a C++ ReShade add-on whose HLSL shader composites Minecraft&\#x27;s rendered frame into Bannerlord&\#x27;s. It demonstrates that runtime interop between two closed, unmodified game engines is practical without source access or engine forks, relying only on OS-level IPC, function hooking, and shader-stage compositing. For systems and graphics engineers it works as a concrete reference design covering lock-free cross-process synchronization, cross-engine depth-buffer reprojection, and overlay-based frame compositing. Synchronization uses seqlocks and single-writer ring buffers so that neither game ever blocks waiting on the other, and the compositor must compare two different reversed-Z depth buffers per pixel while reprojecting a Minecraft frame that is one or two frames stale. Cross-game combat is achieved by spawning invisible, frozen stand-in mobs so Minecraft&\#x27;s own unmodified attack code registers hits on Bannerlord soldiers, and Bannerlord&\#x27;s terrain is rebuilt around the player as invisible Minecraft blocks without stuttering while flying; the repository includes byte-level protocol documentation.

reddit · r/programming · /u/psicodart\_games · Oct 24, 23:23

**Background**: Shared memory is an OS facility that lets two processes map the same physical memory pages, making it one of the fastest ways to pass data between separate programs such as a Java game and a C\# game. A seqlock is a lock-free synchronization pattern in which a writer bumps a counter before and after updating data, so readers can detect a torn read and retry instead of blocking the writer. ReShade is a generic post-processing injector for DirectX/OpenGL/Vulkan games that loads add-ons and runs HLSL shaders over the final frame, which is how Minecraft&\#x27;s output is blended into Bannerlord&\#x27;s. Reversed-Z is a depth-buffer convention that stores near values with high precision; two engines using it with different projections still produce depth values that must be reconciled before per-pixel occlusion can be resolved.

<details><summary>References</summary>
<ul>
<li><a href="https://reshade.me/docs">Add-on Documentation - Reshade</a></li>
<li><a href="https://deepwiki.com/crosire/reshade/5.3-creating-add-ons">Creating Add-ons | crosire/reshade | DeepWiki</a></li>
<li><a href="https://github.com/JohannesLorenz/ringbuffer">GitHub - JohannesLorenz/ringbuffer: A small lock-free, multi ...</a></li>

</ul>
</details>

**Tags**: `#game-engines`, `#shared-memory`, `#lock-free`, `#graphics-programming`, `#interop`

---

<a id="item-5"></a>
## [Show HN: &quot;Steal My Bitcoin&quot; Puts a $502 Wallet Behind a PHP RCE](https://stealmybitcoin.com/) ⭐️ 7.0/10

A developer launched stealmybitcoin.com, a public challenge site that hides a Bitcoin private key worth roughly $502 on a server running a PHP version predating the PHP2SHELL remote code execution flaws, with the key readable by the PHP user account through a \`print-flag\` binary. The first person to exploit the box and claim the wallet wins the funds, and the post drew 354 points and 199 comments on Hacker News. The site turned into an accidental live experiment for claims that autonomous AI agents can mass-exploit vulnerable systems: if swarms of agents really were scanning and compromising every exposed box, the wallet should have vanished within minutes. Its survival became the central evidence in a broader argument about how much offensive capability AI agents actually have today. The challenge is deliberately shallow — a CTF-style PHP box with a known RCE class rather than a novel exploit — and the author explicitly frames it as a test of whether anyone can actually weaponize the recently disclosed PHP2SHELL flaws \(CVE-2026-109618 and CVE-2026-109619, CVSS 9.2, patched in PHP 8.5.12, 8.4.27, 8.3.36 and 8.2.35 on October 21, 2026\). The site&\#x27;s own counter read &quot;0.65 hours without a successful hack&quot; before traffic overwhelmed the server.

hackernews · cloudlandsdev · Oct 24, 20:30 · [Discussion](https://news.ycombinator.com/item?id=50224916)

**Background**: PHP2SHELL refers to a pair of critical, unauthenticated remote code execution vulnerabilities in PHP disclosed in October 2026, which allow an attacker to run arbitrary code on web-facing PHP installations; exploits began circulating within hours of the patch. A CTF \(Capture the Flag\) is a security exercise in which participants hunt for hidden &quot;flags&quot; inside intentionally vulnerable software, normally in a safe and legal setting. This site borrows that format but attaches real money, which raises questions about honeypots, disclosure ethics, and whether LLM-based agents can autonomously perform the same exploitation steps a human researcher would.

<details><summary>References</summary>
<ul>
<li><a href="https://securitylabs.datadoghq.com/articles/php2shell-critical-vulnerabilities-in-php/">PHP2Shell - Critical vulnerabilities in PHP (CVE-2026-109618 ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Capture_the_flag_%28cybersecurity%29">Capture the flag (cybersecurity) - Wikipedia</a></li>
<li><a href="https://arxiv.org/html/2602.02595">To Defend Against Cyber Attacks, We Must Teach AI Agents to Hack</a></li>

</ul>
</details>

**Discussion**: Sentiment was split between skepticism of AI-hacking hype and caution about the site itself: researcher dguido called it &quot;a trap,&quot; saying he has a working RCE but won&\#x27;t demonstrate it because it could leak his team&\#x27;s work while others still need time to patch. Commenter technion argued the wallet remaining unclaimed an hour later &quot;ends the narrative&quot; of swarms of autonomous agents compromising sites, while scottydelta reported that only two of five AI agents he asked even agreed to attempt the challenge \(GLM-5.3 and GLM-5.3-Flash\), with GPT-6.1-Sol refusing it as a cybersecurity request.

**Tags**: `#security`, `#PHP RCE`, `#CTF`, `#AI agents`, `#vulnerability exploitation`

---

<a id="item-6"></a>
## [Goose: A Memory-Safe Systems Language With Multiple Data Stacks](https://aardappel.github.io/goose/) ⭐️ 7.0/10

Wouter van Oortmerssen \(aardappel\), creator of FlatBuffers and the Lobster language, published Goose, an experimental systems programming language built around multiple data stacks, resizable fields, and share-nothing worker threads. He announced it on Hacker News and answered questions directly in a 139-comment thread, with John Carmack publicly praising the design. Goose proposes a third path to memory safety that avoids both a garbage collector and Rust-style lifetime annotations, which makes it relevant to systems programmers who find Rust&\#x27;s borrow checker burdensome or C++&\#x27;s manual memory management unsafe. Endorsement from a figure like Carmack, plus the volume of substantive technical debate, suggests the design ideas could influence future language work even if Goose itself stays experimental. The language has no heap allocator, garbage collector, or lifetime annotations, and its repository benchmarks claim it runs faster than C++ and Rust while using less memory. Workers are compiled as separate programs with their own memory, and flat values cross typed queues via memcpy, so data races, locks, atomics, and memory orderings simply do not exist in the language; the main caveat is that it remains an experimental project whose documentation drew criticism for appearing AI-generated.

hackernews · bobbydigitales · Oct 24, 19:06 · [Discussion](https://news.ycombinator.com/item?id=50224100)

**Background**: Most mainstream languages manage dynamic memory either through a garbage collector \(Java, Go\) or through compile-time ownership and lifetime analysis \(Rust\). Goose instead explores using several separate data stacks rather than one call stack plus a heap, with resizable fields allowing a struct member to grow in place by shifting data between stacks, and an automatic analysis deciding what goes where. Its share-nothing threading model resembles Dart isolates and the actor model, where concurrent units communicate only by copying messages rather than sharing memory.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/aardappel/goose">GitHub - aardappel/ goose : The Goose Programming Language</a></li>
<li><a href="https://www.besthub.dev/articles/why-share-nothing-should-be-the-default-concurrency-model-for-modern-servers-3255b32da121">Why ‘Share Nothing’ Should Be the Default Concurrency Model ...</a></li>

</ul>
</details>

**Discussion**: The author opened the thread with an explicit AMA, and discussion was largely substantive: one commenter said the AI-generated documentation alone was enough to make them lose interest, another raised a concrete technical objection about how a fixed number of stacks can represent an arbitrary number of dynamically sized values such as a hash table of strings, and others compared the share-nothing workers to Dart isolates. A frequently quoted comment was John Carmack&\#x27;s praise that multiple data stacks and resizable fields take the approach from &\#x27;lots of work can be done this way&\#x27; to &\#x27;basically everything can be&\#x27;, and that built-in binary structure validation enables direct memory mapping of network data.

**Tags**: `#programming languages`, `#language design`, `#concurrency`, `#memory management`, `#hacker news`

---

<a id="item-7"></a>
## [HN Debates Why AI Payoff Stays Inside Tech](https://www.apollo.com/wealth/insights-news/insights/daily-spark/no-signs-of-ai-payoff-outside-the-tech-sector) ⭐️ 7.0/10

An Apollo wealth-insights note titled &quot;No signs of AI payoff outside the tech sector&quot; triggered a large Hacker News discussion \(433 points, 425 comments\) about why measurable AI-driven productivity gains have not yet shown up in the broader economy. Commenters pushed back on and refined the article&\#x27;s framing, offering historical analogies and economic arguments rather than disputing the underlying observation. If AI is genuinely a general-purpose technology, the absence of visible productivity gains outside tech affects forecasts for GDP growth, inflation, labor demand, and the justification for the hundreds of billions of dollars in annual AI capital expenditure. It also shapes policy debates over whether the current investment boom is justified or speculative. The most-cited explanation is the electrification precedent: early factories were built around water power and shaft-driven machinery, so simply swapping in an electric motor delivered little until plants were physically redesigned around unit drive, a process that took roughly a decade or more. A second argument holds that AI vendors are pricing their products to capture nearly all of the productivity gain as revenue, so the benefit shows up in AI company earnings rather than in customer productivity statistics.

hackernews · the-mitr · Oct 24, 19:47 · [Discussion](https://news.ycombinator.com/item?id=50224463)

**Background**: Economists have seen this pattern before. In 1987 Robert Solow famously quipped that &quot;you can see the computer age everywhere but in the productivity statistics,&quot; and it took years of organizational change before IT investment translated into measured output. General-purpose technologies such as electricity, the internal combustion engine, and computers typically spread over decades, because institutions, infrastructure, business processes, and worker skills all have to be rebuilt around them before the gains materialize.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fernandohermida.com/posts/the-ai-productivity-paradox-we-have-been-here-before/">The AI Productivity Paradox: We&#x27;ve Been Here Before</a></li>
<li><a href="https://cs.stanford.edu/people/eroberts/cs201/projects/productivity-paradox/lag.html">Productivity Paradox: Lagging Investments - Computer Science</a></li>
<li><a href="https://maseconomics.com/the-ai-productivity-paradox-hundreds-of-billions-spent-zero-measurable-gdp-impact/">The AI Productivity Paradox – MASEconomics</a></li>

</ul>
</details>

**Discussion**: Sentiment was broadly skeptical of expecting quick economy-wide gains, with several distinct arguments emerging. One camp leaned on the electrification analogy, noting that factories had to be rebuilt around electric motors and that a decade of apparently flat growth followed; another argued that AI vendors are deliberately capturing nearly all the surplus as revenue, so gains appear in their earnings rather than in customer productivity; a third pointed out that shipping more software features does not automatically raise output elsewhere and that the enabling models are still very new. Others offered counterexamples such as education, where decades of computer investment have coincided with rising costs and falling scores, suggesting some sectors may see little change at all.

**Tags**: `#AI economics`, `#productivity`, `#technology adoption`, `#industry analysis`, `#Hacker News discussion`

---

<a id="item-8"></a>
## [Live MIDI jam with a pretrained music transformer via logit steering](https://www.reddit.com/r/MachineLearning/comments/1xe4pex/got_a_pretrained_music_transformer_to_jam_with_me/) ⭐️ 7.0/10

A practitioner \(Riccardo Cataldi, /u/GGAllin43\) released &quot;duetto,&quot; a system that jams live with a human MIDI keyboard player by steering the sampling logits of the pretrained Anticipatory Music Transformer \(music-medium-800k\) in real time, with no fine-tuning whatsoever. While the human plays, the system tracks the current key, the held chord and the player&\#x27;s tempo, and adds hand-tuned biases to the logits before sampling; code and a demo video are on GitHub, running on a Jetson Orin Nano. It demonstrates that inference-time control alone can turn a static, pretrained symbolic music model into a responsive improvising partner, without any dataset curation or training cost. That lowers the barrier for interactive music AI and human-AI co-creation tools, and offers a reproducible engineering recipe for real-time musical agents on edge hardware. The model samples roughly one second ahead, and whenever the player changes chord the already-planned output is discarded and resampled so the accompaniment stays harmonically aligned. Biases push down out-of-key notes and notes in the register right around the player&\#x27;s hands, push up chord tones and tensions, lift the register when the player stops \(as if a melody should enter\), and slightly boost continuation of the intervals of the player&\#x27;s last phrase; all offsets are hand-tuned by ear, and the author asks whether a small learned conditioning head or guidance-style methods would be more principled.

reddit · r/MachineLearning · /u/GGAllin43 · Oct 24, 09:58

**Background**: The Anticipatory Music Transformer \(Thickstun, Hall, Donahue and Liang, 2023\) is trained with an &quot;anticipation&quot; objective, meaning it learns to generate music conditioned on events that come later in time, which makes it well suited to accompaniment and infilling rather than plain left-to-right generation. Symbolic music models operate on discrete MIDI-like event tokens instead of audio waveforms, so they are cheap enough to run interactively. Logit steering \(or logit bias\) is a training-free inference-time technique in which values are added to a model&\#x27;s unnormalized output scores before sampling, nudging generation toward desired properties without changing any model weights.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/jthickstun/anticipation">GitHub - jthickstun/anticipation: Anticipatory Autoregressive ...</a></li>
<li><a href="https://arxiv.org/html/2306.08620v1">Anticipatory Music Transformer</a></li>
<li><a href="https://crfm.stanford.edu/2023/06/16/anticipatory-music-transformer.html">Anticipatory Music Transformer: A Controllable Infilling ...</a></li>

</ul>
</details>

**Tags**: `#music-generation`, `#transformer`, `#inference-time-steering`, `#real-time-systems`, `#logit-bias`

---

<a id="item-9"></a>
## [Kimi K3.1 Open-Weight Release Strips Cyberattack Training Data](https://www.reddit.com/r/LocalLLaMA/comments/1xecgrf/kimi_k31_removes_cyberattack_training_data_from/) ⭐️ 7.0/10

According to a LocalLLaMA post, Moonshot AI&\#x27;s Kimi K3.1 open-weight release reportedly excludes training data related to cyberattack capabilities, a change the poster attributes primarily to China&\#x27;s new export restrictions and secondarily to growing caution about cybersecurity exploits appearing in released models. This is an early concrete example of export-control policy directly reshaping what ships inside an open-weight model rather than just who can access it, which matters for anyone building on Chinese open models and for the wider debate over how much dangerous capability should be published in downloadable weights. The claim comes from a short community post rather than an official Moonshot statement, and no technical documentation has been provided on exactly which data was filtered or how capability was measured before and after removal; Kimi K3 itself is a 2.8-trillion-parameter open-weight multimodal model with a 1-million-token context window, and K3.1 Pro was released as a paid API tier with weights slated to follow.

reddit · r/LocalLLaMA · /u/zxyzyxz · Oct 24, 16:05

**Background**: Open-weight models are published as downloadable files that anyone can run and fine-tune locally, unlike closed services such as ChatGPT or Claude that are only reachable through an API or subscription. China has recently introduced export restrictions aimed at overseas transfer of open models with accessible weights, while leaving official APIs, apps and cloud platforms outside the scope. At the same time, safety researchers have grown concerned that openly downloadable models can be stripped of safety tuning or trained further for offensive cyber tasks, which is why labs increasingly filter hazardous training data before release.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MoonshotAI/Kimi-K3">GitHub - MoonshotAI/Kimi-K3: Open Frontier Intelligence</a></li>
<li><a href="https://www.nytimes.com/2026/10/21/world/asia/china-exports-ai-controls.html">China ’s Free A . I . Models Are Thrown Into Uncertainty - The New York...</a></li>
<li><a href="https://www.yottalabs.ai/post/kimi-k3-1-pro-specs-price-open-weights-benchmarks">Kimi K3.1 Pro: Specs, Price, Open Weights Date, and ...</a></li>

</ul>
</details>

**Tags**: `#open-weight models`, `#AI regulation`, `#cybersecurity`, `#LLM safety`, `#Kimi`

---

<a id="item-10"></a>
## [Reddit Post Argues KL Divergence Is Misused as a Quantization Ranking Metric](https://www.reddit.com/r/LocalLLaMA/comments/1xeim3m/kld_is_misunderstood/) ⭐️ 7.0/10

A post on r/LocalLLaMA argues that KL Divergence \(KLD\) is being treated as a universal leaderboard for quantized LLMs when it cannot support that role, and lays out two concrete failure modes: computing KLD on static text corpora such as Wikipedia articles instead of on tokens the model itself generates, and trivially gaming the number by evaluating on data that overlaps with the quantization calibration set. The author recommends generating an evaluation set with the base model and computing KLD only on the generated tokens, giving zero weight to prompt tokens. KLD numbers are routinely published alongside GGUF, MLX and other quantized model releases, so practitioners use them to decide which quant to download and run; if those numbers are easy to manipulate and weakly predictive of real task performance, users may be picking quantizations on the basis of noise. The post pushes the community toward task-based benchmarks and self-generated evaluation data instead of a single cheap-to-game scalar. The critique notes that even a nominally held-out evaluation set can be untrustworthy if it comes from the same source or a very similar distribution as the calibration data, and that some quantization methods do end-to-end fine-tuning of the quantization scale parameters on that same data, producing models that beat much larger ones on KLD while barely generalizing. The author stresses that a higher KLD does not imply the quantized model will fail at your tasks, and that unlike benchmark gaming, which needs serious hardware and compute, making a KLD number look excellent is extremely cheap.

reddit · r/LocalLLaMA · /u/Positive-Resource922 · Oct 24, 20:12

**Background**: Quantization compresses a model&\#x27;s weights \(and sometimes activations\) to lower precision, such as 4-bit, so it fits in less memory and runs faster, at the cost of some quality loss. KL Divergence measures how much one probability distribution diverges from another; in this context, the same text is fed to both the full-precision base model and the quantized model, and the divergence between their next-token probability distributions \(derived from the logits via softmax\) is averaged across tokens. Many quantization methods also rely on calibration data — a sample of text used to choose scaling factors — which is why overlap between calibration and evaluation data is a known source of inflated scores.

<details><summary>References</summary>
<ul>
<li><a href="https://fireworks.ai/research/llm-quantization-quality-kl-divergence">Measuring LLM Quantization Quality With KL Divergence | Fireworks</a></li>
<li><a href="https://apxml.com/courses/quantized-llm-deployment/chapter-3-performance-evaluation-quantized-llms/evaluating-accuracy-degradation">Assessing Accuracy Loss in Quantized LLMs</a></li>
<li><a href="https://ai-tldr.dev/learn/llm-fundamentals/text-generation/logits-explained/">Logits Explained: The Logits Probability Distribution | AI/TLDR</a></li>

</ul>
</details>

**Tags**: `#quantization`, `#KL-divergence`, `#LLM-evaluation`, `#model-metrics`, `#LocalLLaMA`

---

<a id="item-11"></a>
## [Meta distills Llama 3 8B into 1B byte-level models, predicting they eventually beat token models](https://www.reddit.com/r/LocalLLaMA/comments/1xe88ja/meta_trained_small_ai_models_to_read_raw_bytes/) ⭐️ 7.0/10

Researchers at Meta trained roughly 1B-parameter language models directly on raw bytes — one character at a time rather than on tokens — partly by distilling knowledge from the token-based Llama 3 8B teacher. In their runs the token models won early and clearly, but their gains flattened with more training while the byte models kept improving, and the byte models reportedly needed about 6x less text to reach the same level. If the trend holds, dropping the tokenizer could make small on-device models meaningfully stronger at the same parameter count, and it would eliminate tokenizer artifacts such as models miscounting letters in a word. That matters most for phones and laptops, where squeezing more quality out of a fixed model size is the central constraint. The headline claim that byte models beat Llama 3.2 1B and Gemma 3 1B by a few points is an extrapolation of fitted curves beyond what was actually trained, not an observed result, and in the real runs the token model was still ahead. Byte-level inference is also slower per unit of text — a token covers roughly 4-5 characters, so the same passage takes about 5x more steps — and the study only covers small models, so behavior at larger scale is unknown.

reddit · r/LocalLLaMA · /u/DotaMate · Oct 24, 13:08

**Background**: Mainstream language models do not read text character by character; a tokenizer first chops text into subword tokens \(roughly 4-5 characters each\) drawn from a fixed vocabulary, and the model predicts the next token. Byte-level models skip that step and operate on raw bytes, which makes them language- and script-agnostic and removes vocabulary limits, but lengthens the sequence the model must process. Knowledge distillation — training a smaller student to mimic a larger teacher&\#x27;s outputs — is the standard way to make small models punch above their weight, and here it is complicated by the teacher thinking in tokens while the student reads bytes, requiring a mapping between the two tokenizations.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2602.01007v1">Distilling Token -Trained Models into Byte -Level Models</a></li>
<li><a href="https://dev.to/danielsamfdo/tokens-are-a-crutch-why-byte-models-win-the-long-game-4fdd">Tokens Are a Crutch: Why Byte Models Win the... - DEV Community</a></li>
<li><a href="https://www.activeloop.ai/resources/glossary/byte-level-language-models/">What is Byte - Level Language Models ? | Activeloop Glossary</a></li>

</ul>
</details>

**Tags**: `#tokenization`, `#byte-level-models`, `#knowledge-distillation`, `#small-language-models`, `#scaling-laws`

---

<a id="item-12"></a>
## [8GB GPU Runs 262K-Context Qwen-Flash-Next Coder at 70 T/s via llama.cpp](https://www.reddit.com/r/LocalLLaMA/comments/1xebdzl/8_gb_gpu_262k_context_35_bpw_qwenflashnext_coder/) ⭐️ 7.0/10

A Reddit user \(u/jonathanx37\) published a working recipe for running ISTA DASLab&\#x27;s 3.5 BPW GSQ-RCO quant of Qwen-Flash-Next Coder on a machine with only 8GB of VRAM and 24GB of RAM, at a 262K context window. The trick is to keep most Mixture-of-Experts \(MoE\) layers in system RAM — placing only the smallest experts in VRAM — while pushing the model&\#x27;s n-gram embedding data to the fastest available SSD, yielding roughly 70 T/s prompt processing and 8 T/s token generation. It shows that sparse MoE architectures plus aggressive offloading let consumer-grade hardware run a model whose full checkpoint is far larger than the available VRAM, with a 262K context that would normally demand enormous memory. For the local-inference community this is a concrete, reproducible template for squeezing large coder models onto budget GPUs rather than renting cloud capacity. The author stresses that this is not a 1-bit quant: half of the experts are pruned and the retained weights are stored at 3.5 BPW, so the advertised 1.89 bits per parameter is an effective rate amortising pruning over the original parameter count. Selective MoE offloading via regex outperforms the simpler --n-cpu-moe flag \(which is bottlenecked by PCIe 3.0 here\), the first run is slower because of mmap so a second run gives accurate throughput, CUDA reportedly struggles at 8GB so the Vulkan backend is recommended, and the Qwen &quot;sharp&quot; chat template is advised to reduce overthinking.

reddit · r/LocalLLaMA · /u/jonathanx37 · Oct 24, 15:21

**Background**: Qwen-Flash-Next is an open-weight preview of the architecture behind Qwen 4: a 125B-parameter main model plus a separate 51B n-gram embedding table, with only about 6B parameters activated per token. Because a Mixture-of-Experts model only routes each token through a small subset of its experts, the inactive experts can sit in slower, cheaper memory without killing throughput — which is exactly what llama.cpp&\#x27;s offloading options exploit. The quant comes from ISTA DASLab, whose GSQ method performs accurate low-bit scalar quantization per tensor while RCO assigns quantization types across tensors under a total size budget, producing a non-uniform GGUF at a target file size.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/ISTA-DASLab/Qwen3.8-Flash-Next-GSQ-RCO-GGUF">ISTA-DASLab/Qwen3.8-Flash-Next- GSQ - RCO -GGUF · Hugging Face</a></li>
<li><a href="https://github.com/qwenlm/qwen3.8-flash-next">GitHub - QwenLM/ Qwen 3.8- Flash - Next : Qwen 3.8- Flash - Next is the...</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/discussions/10879">Performance of llama . cpp with Vulkan · ggml-org llama . cpp ...</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#llama.cpp`, `#mixture-of-experts`, `#quantization`, `#gpu-memory-offloading`

---

<a id="item-13"></a>
## [ANEMLL Forge 0.2.1 runs Qwen3.8-27B on M6 Neural Engine with 192K context](https://www.reddit.com/r/LocalLLaMA/comments/1xejv61/m6_mac_mini_owners_32gb_now_you_can_run_qwen3827b/) ⭐️ 7.0/10

ANEMLL Forge 0.2.1 now runs Qwen3.8-27B on the M6 Apple Neural Engine with context up to 192K on 32GB machines, adding an INT8 K/V cache that halves FP16 memory use and a smaller drafter model that shares the target model&\#x27;s output head, saving 0.86 GB of ANE memory at the same speed. The release also ships detailed benchmarks of the speed/memory tradeoffs across context lengths. It demonstrates that a 27B dense model can run entirely on-device on Apple&\#x27;s NPU with very long context, which matters for privacy-preserving local inference where no data leaves the machine. It also gives the Apple-silicon local LLM community a concrete alternative to the GPU-based MLX and llama.cpp paths, with published numbers rather than vague claims. Decode speed depends heavily on content: 35–62 tok/s for JSON, 18–32 for code, and 10–17 for prose, while prefill is 260 tok/s at short context but drops to 62 tok/s at 192K, where the tool switches to a smaller prefill batch \(32 instead of 64 rows\) to stay within the memory budget. The first full 192K compile takes about 2 hours on an M6 \(cached afterwards\), though \`--ctx\` exports only the needed entries so a 16K setup takes roughly 10 minutes, and the author considers 96K the sweet spot on 32GB at 123 tok/s prefill, ~27 tok/s decode and ~21.4 GB total memory.

reddit · r/LocalLLaMA · /u/Competitive-Bake4602 · Oct 24, 21:05

**Background**: The Apple Neural Engine \(ANE\) is the dedicated neural processing unit inside Apple silicon chips, accessed indirectly through Core ML rather than through general-purpose GPU APIs. ANEMLL is an open-source project that ports large language models to the ANE, and ANEMLL Forge is its research-oriented companion focused on inference of large dense models on the M6 ANE, sharing quantization and conversion workflows plus notes on compiler behavior. The K/V cache stores the attention keys and values for every token already processed, so its size grows with context length; storing it in INT8 instead of FP16 halves that memory, which is what makes long contexts feasible on a 32GB machine. The release also builds on the project&\#x27;s three-bit MLP vector quantization work, which compresses the model&\#x27;s feed-forward matrices to fit the ANE&\#x27;s constraints.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Anemll/anemll-forge">ANEMLL Forge - GitHub</a></li>
<li><a href="https://github.com/Anemll/Anemll">GitHub - Anemll/Anemll: Artificial Neural Engine Machine ...</a></li>
<li><a href="https://theaivibe.org/edge/a-27b-ai-hits-an-iphones-neural-engine-at-3-bits-while-a-14m-llm-keeps-2026-10-18">A 27B AI Hits an iPhone&#x27;s Neural Engine at 3 Bits While a 14M LLM</a></li>

</ul>
</details>

**Tags**: `#Apple Neural Engine`, `#local LLM inference`, `#quantization`, `#Qwen`, `#ANEMLL`

---

<a id="item-14"></a>
## [ISTA Ships 1.75–2.25 bpw GSQ/RCO GGUFs of 763B DeepSeek-V4.1-Flash](https://www.reddit.com/r/LocalLLaMA/comments/1xe2wg8/release_ista_gsqrco_ggufs_for_deepseekv41flash1017/) ⭐️ 7.0/10

The ISTA Deep Algorithms and Systems Lab released three GSQ/RCO-quantized GGUFs of DeepSeek-V4.1-Flash-1017 — a 763.2B-parameter sparse MoE with 384 routed experts \(6 active per token\) and a 1M-token context — at IQ1\_M \(1.75 bpw\), IQ2\_XXS \(2.00 bpw\) and IQ2\_XS \(2.25 bpw\), with backbones ranging from 120.7 GB to 155.2 GB. The builds share a single 110.6 GB Engram file holding the model&\#x27;s two lookup tables \(196.6B parameters\) at IQ4\_NL, which only needs to be downloaded once. At 2.00 bpw the quantized model reportedly matches the base model on every benchmark evaluated, meaning a frontier-scale 763B MoE can be squeezed into roughly 138 GB of backbone weights without measurable loss. Combined with the Strata runtime&\#x27;s claim of serving every build on a single 12 GB GPU, this pushes locally runnable frontier-class models well beyond what consumer hardware could previously attempt. The stated bit-widths are averages over the 551.9B backbone parameters that the search actually controls, and the Engram tables are read one row per token so they can stay memory-mapped on disk rather than resident in VRAM. Notably, llama.cpp does not yet support DeepSeek-V4.1, so these GGUFs currently run only in Strata, and results for the IQ2\_XS \(2.25 bpw\) build are still pending.

reddit · r/LocalLLaMA · /u/Loginhe · Oct 24, 08:05

**Background**: Mixture-of-experts \(MoE\) models keep total parameter counts huge but activate only a small subset of experts per token, so compute stays modest while memory requirements balloon — which is why quantization matters so much for local use. GGUF is the file format used by llama.cpp and related runtimes, and &quot;bits per weight&quot; \(bpw\) measures how many bits each parameter occupies, with values below 3 bpw considered extreme low-bit compression. GSQ \(Gumbel-Softmax Quantization\) is a post-training scalar quantization method that jointly learns per-coordinate grid assignments and per-group scales, while RCO \(Riemannian Constrained Optimization\) assigns a quantization type to each tensor so the whole model fits an exact size budget. DeepSeek&\#x27;s Engram is a conditional-memory mechanism that augments the Transformer with a large static lookup table, letting the network retrieve factual associations in O\(1\) time instead of storing them in expensive weights.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2604.18556">GSQ : Highly-Accurate Low-Precision Scalar Quantization for LLMs via...</a></li>
<li><a href="https://github.com/IST-DASLab/GSQ">IST-DASLab/ GSQ : Gumbel - Softmax post-training quantization for...</a></li>
<li><a href="https://www.remio.ai/post/deepseek-engram-architecture-a-new-axis-of-sparsity-for-llms">DeepSeek Engram Architecture: A New Axis of Sparsity for LLMs</a></li>

</ul>
</details>

**Tags**: `#quantization`, `#GGUF`, `#local-llm`, `#mixture-of-experts`, `#low-bit-inference`

---

<a id="item-15"></a>
## [Roku moves its developer repositories from GitHub to GitLab](https://blog.roku.com/developer/gitlab-move) ⭐️ 6.0/10

Roku announced on its developer blog that it is moving its developer repositories from GitHub to GitLab, without publicly stating a reason for the migration. The move drew a Hacker News thread of roughly 242 points and 159 comments debating the tradeoffs between the two platforms. A mid-size platform company leaving GitHub is a visible data point for teams weighing whether GitHub&\#x27;s dominance still justifies its workflow assumptions, especially as GitLab pitches an all-in-one DevSecOps stack. The migration also affects third-party Roku developers who follow sample code, SDKs, and issue trackers hosted in those repositories. Roku has not disclosed whether existing GitHub Actions pipelines will be ported to GitLab CI, nor how issues, pull requests, and access permissions will be handled during the transition. Commenters also noted that GitHub&\#x27;s recent outages are largely driven by heavier overall usage rather than by any single engineering failure, suggesting a platform switch may not address root causes.

hackernews · cxr · Oct 24, 16:06 · [Discussion](https://news.ycombinator.com/item?id=50222622)

**Background**: GitHub and GitLab both host Git repositories and the collaboration tooling around them, but they have diverged in emphasis: GitHub, owned by Microsoft since 2018, became the default home for open-source projects and social-style collaboration, while GitLab bundles source control, CI/CD, security scanning, and issue tracking into a single application that can also be self-hosted. Migrating repositories is more than a \`git remote\` change — it typically involves moving issues, merge/pull requests, CI configuration, webhooks, and team permissions. GitHub Actions and GitLab CI use different configuration formats, so pipelines usually need to be rewritten rather than copied.

**Discussion**: The dominant sentiment is that GitLab fits &quot;regular&quot; company and organization projects better than GitHub, which one commenter said drifted toward being an &quot;open source dev social network&quot; that has been &quot;Microsofted.&quot; Others are skeptical that switching platforms solves anything, arguing GitHub&\#x27;s outages stem from every user demanding more from the system, and several commenters simply wish Roku would &quot;spill some tea&quot; and explain its reasoning; one also claimed, without substantiation, that Roku is being acquired by Fox.

**Tags**: `#GitHub`, `#GitLab`, `#developer-tools`, `#platform-migration`, `#source-control`

---

<a id="item-16"></a>
## [FreeDNS Resurfaces on Hacker News, Sparking Public Suffix List Security Debate](https://freedns.afraid.org/) ⭐️ 6.0/10

A Hacker News thread about FreeDNS \(freedns.afraid.org\), a free DNS hosting service that has been running for roughly two decades, reached 239 points and 61 comments. The discussion focused less on new features than on long-standing caveats, notably that FreeDNS-hosted domains are absent from the Public Suffix List, plus comparisons to alternatives such as nic.eu.org and dns.he.net. FreeDNS is one of the oldest continuously operating free DNS providers, so many hobbyists, test setups, and small projects still depend on it, and the thread is a useful reminder that free shared-domain hosting carries security trade-offs. The Public Suffix List issue affects how browsers isolate cookies, meaning a shared parent domain can expose users to cookie-injection or session-fixation risks if the suffix is not properly registered. Commenters noted that getting a free subdomain provider added to the Public Suffix List is difficult and may not happen, so users should treat FreeDNS subdomains as shared infrastructure rather than security-isolated domains. Others highlighted FreeDNS&\#x27;s backup/secondary DNS feature, which lets someone run authoritative DNS on a single personal server with FreeDNS as a fallback, and pointed to nic.eu.org as another no-cost option.

hackernews · esher · Oct 24, 15:20 · [Discussion](https://news.ycombinator.com/item?id=50222133)

**Background**: DNS \(Domain Name System\) is the internet&\#x27;s directory that translates human-readable domain names into IP addresses, and DNS hosting services store and serve those records. The Public Suffix List is a community-maintained registry, originally a Mozilla initiative, of every suffix under which anyone can directly register a name — such as com, co.uk, or a hosting provider&\#x27;s shared subdomain zone. Browsers and other software use the list to decide which part of a domain is the registrant-controlled portion, which is why it governs cookie scoping and same-site boundaries. FreeDNS offers free static and dynamic DNS hosting, including subdomains under shared domains, which is why the list matters to its users.

<details><summary>References</summary>
<ul>
<li><a href="https://publicsuffix.org/">Public Suffix List</a></li>
<li><a href="https://freedns.afraid.org/?ref=mgrove.uk">FreeDNS - Free DNS - Dynamic DNS - Static DNS subdomain and...</a></li>
<li><a href="https://www.namecheap.com/domains/freedns/">Free DNS Hosting - Best FreeDNS Hosting Server by Namecheap</a></li>

</ul>
</details>

**Discussion**: Sentiment was broadly positive and nostalgic: one user called it &quot;one of the most solid and longest lasting services online&quot; after nearly two decades, and another described themselves as a happy free user for about 15 years. The main criticism was the Public Suffix List omission and its cookie security implications, while others recommended nic.eu.org and dns.he.net as alternatives and one commenter questioned whether FreeDNS&\#x27;s interface was copied from dns.he.net.

**Tags**: `#DNS`, `#free services`, `#web infrastructure`, `#security`, `#Hacker News`

---

<a id="item-17"></a>
## [2018 Essay on Why Quantum Mechanics Defies Intuition Resurfaces on HN](https://www.southampton.ac.uk/~doug/quantum_physics/index.html) ⭐️ 6.0/10

A pedagogical essay by a University of Southampton physics instructor, titled &quot;I don&\#x27;t understand quantum physics&quot; and originally posted in 2018, resurfaced on Hacker News and climbed to 267 points with 203 comments. The essay argues that quantum mechanics is hard to grasp not because the math is inaccessible but because the standard teaching sequence buries learners in conceptual baggage. The thread has become a practical reading list for self-taught learners, with commenters pointing to alternative entry points that skip the classical-physics-first approach. It also reflects a broader, ongoing debate in physics education about whether the traditional wave-particle and double-slit curriculum actually helps or hinders understanding. The value of the submission lies mostly in the comments rather than the essay itself, which offers no technical or research novelty; one commenter also flagged the author&\#x27;s disclaimer that images pulled from the internet were assumed to be public domain and left unreferenced. Recommended alternatives include learning the linear algebra of one- and two-qubit systems first, L. V. Tarasov&\#x27;s &quot;Basic Concepts of Quantum Mechanics,&quot; and Bob Coecke&\#x27;s &quot;Picturing Quantum Processes.&quot;

hackernews · rramadass · Oct 24, 09:53 · [Discussion](https://news.ycombinator.com/item?id=50219666)

**Background**: Quantum mechanics describes matter and light at atomic and subatomic scales, and its predictions routinely conflict with everyday intuition — particles behave like waves, measurement outcomes are probabilistic, and observing a system changes it. Standard university courses usually begin with classical waves and particles, the double-slit experiment, and the Schrödinger equation before introducing the abstract state-vector formalism of Hilbert spaces. Qubits, the basic unit of quantum computing, are two-level quantum systems whose behavior can be described with ordinary matrix algebra, which is why some educators argue they make a gentler first exposure than infinite-dimensional wave mechanics.

**Discussion**: Commenters largely agreed that the classical-physics-first curriculum is the real obstacle: one non-physicist said quantum mechanics only clicked after learning the linear algebra of one- and two-qubit systems, which is accessible at a pre-calculus level. Others shared books that worked for them, including Tarasov&\#x27;s dialogue-driven introduction and Coecke&\#x27;s visual &quot;Picturing Quantum Processes,&quot; and one commenter linked an interactive self-study guide built to help non-physicists &quot;feel&quot; the equations. A separate thread of criticism targeted the essay author&\#x27;s casual assumption that internet images are public domain.

**Tags**: `#quantum-computing`, `#physics`, `#education`, `#pedagogy`, `#hackernews-discussion`

---

<a id="item-18"></a>
## [Unverified Tool Claims 30x/40x Compute Unlock on RTX 30/40 GPUs](https://www.reddit.com/r/LocalLLaMA/comments/1xelhpj/cmp170hx_inspiration_unlocks_30x40x_also_up_to_2x/) ⭐️ 6.0/10

A Reddit post on r/LocalLLaMA claims that a new unlock tool, inspired by CMP 170HX mining-card modifications, delivers &quot;30x/40x&quot; compute gains and up to 2x prefill speedup on NVIDIA RTX 30 and RTX 40 GPUs for LLM workloads. The post itself is only a one-line hype message urging readers to &quot;buy, sell, but hurry,&quot; with no tool link, benchmarks, or methodology attached. If the claim holds up, extra usable compute and faster prefill on consumer RTX cards would directly benefit local LLM hobbyists and small-scale self-hosted deployments, where time-to-first-token on long prompts is a common bottleneck. Because the claim is unverified and framed as a market tip, it is more likely to move used-GPU prices than to change anyone&\#x27;s inference stack today. The post provides no benchmark numbers, no description of what is actually being unlocked \(compute units, power limits, PCIe lanes, or memory\), and no reproducibility information, so the 30x/40x and 2x figures cannot be evaluated. The only concrete technical lineage cited is the CMP 170HX, a GA100-based mining card that modders have previously unlocked for PCIe bandwidth and memory capacity via hardware and firmware patches.

reddit · r/LocalLLaMA · /u/chemist\_slime · Oct 24, 22:16

**Background**: The CMP 170HX is an NVIDIA GA100-based card built for cryptocurrency mining, and the modding community has used tools such as the NVIDIA-patcher project plus physical modifications like capacitor rework to lift its artificial limits on PCIe lanes and memory capacity. In LLM inference, the prefill phase is where the model ingests the entire prompt at once to populate the KV cache; it is compute-bound, so additional compute translates fairly directly into lower time-to-first-token. The decode phase that follows generates tokens one at a time and is typically bound by memory bandwidth instead, which is why a prefill-only speedup would not necessarily improve overall generation throughput.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/dartraiden/NVIDIA-patcher/issues/73">170 hx （any cmp hx card ） can run higher and higher fp32 flops than...</a></li>
<li><a href="https://www.youtube.com/watch?v=HNxKJvFtHcA">The MONSTER 170 HX UNLOCKED CAP MODDED x16... - YouTube</a></li>
<li><a href="https://redis.io/blog/prefill-vs-decode/">Prefill vs Decode: LLM Inference Phases Explained</a></li>

</ul>
</details>

**Tags**: `#NVIDIA GPUs`, `#LLM inference`, `#hardware modding`, `#RTX 4090`, `#performance optimization`

---

<a id="item-19"></a>
## [Open-Source Browser Rhythm Game Runs Four ONNX Audio Models Locally](https://www.reddit.com/r/LocalLLaMA/comments/1xeia9o/made_a_rhythm_game_where_4_small_neural_nets/) ⭐️ 6.0/10

A developer released Struna, an MIT-licensed browser rhythm runner that turns any user-supplied MP3 into a playable level using four small neural networks running entirely on-device via onnxruntime-web \(WASM, each model in its own web worker\): BeatNet \(~1.6 MB\) for beat and downbeat tracking, Spotify&\#x27;s Basic Pitch \(~0.2 MB\) for note transcription, Spleeter&\#x27;s vocal separation net \(~20 MB\), and SwiftF0 \(~0.1 MB\) for vocal pitch tracking. Nothing is uploaded — the four models total roughly 22 MB and are cached after the first load. It is a concrete, working demonstration that a full audio-understanding pipeline — beat tracking, transcription, source separation and pitch tracking — can run inside a browser tab with no server and no uploads, which is the same privacy-preserving, on-device inference pattern increasingly used for local LLMs. For anyone building browser-based audio or ML tools, it shows that a handful of sub-25 MB ONNX models are enough to drive real interactive applications. Each model&\#x27;s output maps directly to gameplay: BeatNet&\#x27;s beats form the grid every obstacle and jump sits on, Basic Pitch&\#x27;s held notes become swingable bars and solos become rings at each note&\#x27;s pitch, and SwiftF0&\#x27;s 16 ms pitch frames let the player fly through rings on the singer&\#x27;s syllables. If a device cannot keep up, the game falls back to plain DSP \(onsets, per-bar loudness, drop detection\), and the same song always generates the same world so levels can be learned; the author also notes his beat tracker still sometimes reads a fast song at half its tempo.

reddit · r/LocalLLaMA · /u/MrFelliks · Oct 24, 19:59

**Background**: onnxruntime-web is Microsoft&\#x27;s runtime for executing ONNX models in the browser, typically compiled to WebAssembly so inference runs locally without a GPU server. BeatNet is a CRNN plus particle-filter system for joint beat, downbeat, tempo and meter tracking; Basic Pitch is Spotify&\#x27;s lightweight audio-to-MIDI transcription model; and Spleeter is Deezer&\#x27;s TensorFlow-based source separation library whose pretrained models split a mix into stems such as vocals and accompaniment. Running these normally requires Python and TensorFlow, so porting them to small ONNX graphs that fit in a browser tab is the notable engineering step here.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/mjhydri/BeatNet">GitHub - mjhydri/BeatNet: BeatNet is state-of-the-art (Real ...</a></li>
<li><a href="https://huggingface.co/spotify/basic-pitch">spotify / basic - pitch · Hugging Face</a></li>
<li><a href="https://github.com/deezer/spleeter">GitHub - deezer/ spleeter : Deezer source separation library including...</a></li>

</ul>
</details>

**Tags**: `#local-inference`, `#onnxruntime-web`, `#browser-ml`, `#audio-processing`, `#open-source-game`

---

<a id="item-20"></a>
## [Chinese Labs Strip RTX 5090s for Dies and 32GB VRAM to Build AI Servers](https://www.reddit.com/r/LocalLLaMA/comments/1xe1zsr/the_rtx_5090_isnt_gone_its_in_chinese_labs_where/) ⭐️ 6.0/10

A post on r/LocalLLaMA reports that RTX 5090 graphics cards are being disassembled in Chinese labs, where technicians remove the GPU die and its 32GB of VRAM so the parts can be re-used in custom-built AI servers. Rather than running the cards as-is, the labs reportedly harvest the two most valuable components and rebuild them into multi-GPU machines. The story illustrates how demand for local AI compute and export controls on datacenter accelerators are pushing users toward unconventional supply chains, effectively turning a consumer gaming card into a source of salvaged AI hardware. If the practice is widespread, it could tighten retail availability and pricing for RTX 5090s while giving Chinese labs a cheaper path to high-VRAM inference boxes. The report is an unverified community anecdote with no photos, part numbers, or cost figures attached, so the scale of the practice is unknown. Harvesting a bare die and GDDR7 memory and re-mounting them onto custom boards requires advanced re-balling and PCB engineering, and it voids any warranty while discarding the card&\#x27;s cooler, power delivery and display outputs.

reddit · r/LocalLLaMA · /u/chemist\_slime · Oct 24, 07:09

**Background**: The RTX 5090 is NVIDIA&\#x27;s flagship consumer GPU, built on the Blackwell architecture and equipped with 32GB of GDDR7 memory — an unusually large amount of VRAM for a consumer card, which is why it is popular with the local LLM community for running large models. Successive US export controls have restricted sales of high-end datacenter accelerators such as NVIDIA&\#x27;s H100 and B200 to China, and the RTX 5090 has also been caught up in those restrictions. As a result, Chinese researchers and small labs often have to improvise, sourcing consumer cards or salvaged components to assemble the multi-GPU servers that local inference and fine-tuning require.

<details><summary>References</summary>
<ul>
<li><a href="https://petronellatech.com/blog/how-to-build-custom-ai-workstation-2026/">AI Workstation Build 2026: RTX 5090, DGX Spark &amp; Real Prices</a></li>
<li><a href="https://www.reddit.com/r/LocalLLaMA/about/">r/LocalLLaMA - Reddit</a></li>
<li><a href="https://abuz8ai.com/blog/run-ai-agents-on-rtx-5090">Run AI Agents on an RTX 5090: The Local AI Workstation Guide ...</a></li>

</ul>
</details>

**Tags**: `#GPU hardware`, `#AI infrastructure`, `#export controls`, `#LocalLLaMA`, `#supply chain`

---

<a id="item-21"></a>
## [Boston Dynamics Employees Petition to Cancel $1.3M Spot Sale to ICE](https://www.reddit.com/r/artificial/comments/1xe5pqg/boston_dynamics_employees_petition_to_cancel_13m/) ⭐️ 6.0/10

Employees at Boston Dynamics have reportedly circulated an internal petition urging the company to cancel a $1.3 million sale of its Spot quadruped robots to U.S. Immigration and Customs Enforcement \(ICE\). The petition frames the deal as a direct test of the company&\#x27;s stated ethical commitments about how its robots are used once they leave the factory. Spot is one of the most widely deployed commercial legged robots, so a staff revolt over a government customer signals how employee activism is now reaching hardware and robotics firms, not just AI labs and defense contractors. The outcome could shape how robotics companies structure contracts with law-enforcement and immigration agencies, and whether internal ethics review becomes a standard step before such sales. Spot is a payload-carrying mobile platform equipped with cameras and onboard perception software for inspecting, mapping and monitoring sites, which is precisely why surveillance concerns attach to police or agency deployments even though the robot itself is not a weapon. The petition&\#x27;s specific demands, the number of signatories, and any official response from Boston Dynamics management were not detailed in the available material, so the fate of the $1.3 million order remains unclear.

reddit · r/artificial · /u/VectorWireAI · Oct 24, 10:59

**Background**: Boston Dynamics is the robotics firm known for legged machines such as Spot, a four-legged robot that walks through industrial and outdoor environments carrying sensors to inspect and monitor sites. &quot;Dual-use&quot; technology refers to tools designed for civilian purposes that can also serve military, security or surveillance applications — a debate long applied to nuclear and aerospace tech and now increasingly to AI and robotics. ICE is the U.S. federal agency responsible for immigration enforcement and customs investigations, and its use of technology has been a recurring subject of public controversy. Employee petitions against such contracts have become a common way for tech workers to pressure management over who their products serve.

<details><summary>References</summary>
<ul>
<li><a href="https://bostondynamics.com/products/spot/">Spot | Boston Dynamics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Dual-use_technology">Dual-use technology - Wikipedia</a></li>
<li><a href="https://roboticsreports.com/spot-robot-explained-components-capabilities-and-use-cases/">Spot Robot Explained: Components, Capabilities, and Use Cases</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#tech ethics`, `#surveillance`, `#labor activism`, `#Boston Dynamics`

---

<a id="item-22"></a>
## [Reddit Post Claims AWS AI Cloud Capacity Sold Out Through 2027](https://www.reddit.com/r/artificial/comments/1xe1mos/aws_ai_cloud_capacity_sold_out_through_2027_2028/) ⭐️ 6.0/10

A Reddit post by user /u/VectorWireAI in r/artificial claims that AWS&\#x27;s AI cloud capacity is fully sold out through 2027, with bookings for 2028 already filling up quickly. The post itself contains no linked source article, figures, or supporting documentation, so the claim currently rests on an unsourced assertion. If accurate, a multi-year sell-out of AI compute at the world&\#x27;s largest cloud provider would signal that demand for GPU and accelerator capacity still far outpaces supply, reinforcing the capex boom in AI data centers. It would also mean startups and enterprises without long-term contracts could face higher prices, longer queues, or outright inability to secure capacity for years. The post provides no primary source, no specific capacity figures, no contract terms, and no indication of whether &quot;sold out&quot; refers to all AI instances or only specific high-end GPU types such as those used for large-scale model training. Readers should treat the claim as an unverified signal of sentiment rather than confirmed reporting until AWS or a credible outlet corroborates it.

reddit · r/artificial · /u/VectorWireAI · Oct 24, 06:47

**Background**: AWS is Amazon&\#x27;s cloud computing arm and the largest public cloud provider by market share, renting out compute, storage, and networking to companies on demand. In the AI era, the scarcest resource is not ordinary servers but GPU and custom accelerator capacity, such as NVIDIA chips and AWS&\#x27;s in-house Trainium and Inferentia silicon, which are needed to train and run large models. Because building data centers takes years and involves power, land, and chip supply constraints, cloud providers often pre-sell capacity through multi-year commitments, so &quot;sold out through 2027&quot; effectively means future supply is already contracted.

**Tags**: `#AWS`, `#AI infrastructure`, `#cloud computing`, `#compute capacity`, `#AI demand`

---