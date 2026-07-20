---
layout: default
title: "Horizon Summary: 2026-07-20 (EN)"
date: 2026-07-20
lang: en
---

> From 27 items, 21 important content pieces were selected

---

1. [Alibaba Unveils Qwen 3.8: 2.4T Parameter Open-Weight LLM](#item-1) ⭐️ 9.0/10
2. [SRE replaces $120k bowling system with $1,600 ESP32s](#item-2) ⭐️ 8.0/10
3. [Minecraft Java Edition Switches to SDL3](#item-3) ⭐️ 8.0/10
4. [Claude Code adopts Bun rewritten in Rust](#item-4) ⭐️ 8.0/10
5. [Lessons from Selling 2,500 MIDI Recorders](#item-5) ⭐️ 8.0/10
6. [How fork() duplicates a process without copying its memory](#item-6) ⭐️ 8.0/10
7. [AI advice tripled confidence but slashed accuracy, study finds](#item-7) ⭐️ 7.0/10
8. [OpenAI Reduces Codex Context Window from 372k to 272k](#item-8) ⭐️ 7.0/10
9. [IndieWeb journey reveals benefits and barriers](#item-9) ⭐️ 7.0/10
10. [Moonshot AI pauses Kimi K3 subscriptions due to demand](#item-10) ⭐️ 7.0/10
11. [AI Mania Is Eviscerating Global Decision-Making](#item-11) ⭐️ 7.0/10
12. [Google's IDE Evolution: A Historical Retrospective](#item-12) ⭐️ 7.0/10
13. [Time Mismanagement in Distributed Systems: A Failure Mode](#item-13) ⭐️ 7.0/10
14. [Building Merkle Tree AIR Script in Plonky3](#item-14) ⭐️ 7.0/10
15. [Last MPEG-4 Visual Patent Expired, Freeing Xvid/DivX](#item-15) ⭐️ 6.0/10
16. [Home Server Rebirth: From Pi SD to SSD & Mini-PCs](#item-16) ⭐️ 6.0/10
17. [Wuling Bingo May Be Rebadged as Chevy for North America](#item-17) ⭐️ 6.0/10
18. [Transcribe.cpp: Open-Source C++ Speech-to-Text Library](#item-18) ⭐️ 6.0/10
19. [Commutative Complex Numbers in Plain C](#item-19) ⭐️ 6.0/10
20. [Real-World CPU Bottleneck Debugging Story](#item-20) ⭐️ 6.0/10
21. [Developing TUI in Go with Bubble Tea](#item-21) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Alibaba Unveils Qwen 3.8: 2.4T Parameter Open-Weight LLM](https://twitter.com/Alibaba_Qwen/status/2078759124914098291) ⭐️ 9.0/10

Alibaba announced Qwen 3.8, a 2.4-trillion-parameter open-weights large language model, as a competitive response to Moonshot AI's recently unveiled Kimi K3 (2.8T parameters). The model is expected to be released publicly soon, following the pattern of previous Qwen models. This announcement intensifies the competition in the open-weights LLM space, particularly between Chinese AI labs, and provides the community with another powerful alternative for local deployment. The 2.4T parameter size makes it one of the largest openly available models, potentially driving further interest in running large models on consumer hardware. Qwen 3.8 is a dense model with 2.4 trillion parameters, while the competing Kimi K3 has 2.8 trillion parameters and is set to be published on Hugging Face by July 27, 2026. The announcement includes a link to pricing plans for the Qwen cloud service, indicating a dual strategy of both open weights and commercial offerings.

hackernews · nh43215rgb · Jul 19, 08:44 · [Discussion](https://news.ycombinator.com/item?id=48966120)

**Background**: Open-weights LLMs are large language models whose pre-trained weights are publicly released, allowing others to fine-tune, deploy, or build upon them, though they are not fully open-source. Alibaba's Qwen series has been a prominent player in this space, with previous versions like Qwen 3.6 and 3.7 offering models of varying sizes, including MoE and dense architectures. The release of Qwen 3.8 follows shortly after Moonshot AI's Kimi K3, which itself was preceded by the open-weights Kimi K2 in July 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_K3">Kimi K3</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weights-llms-in-depth-analysis-adoption-usage-performance-jha-kymhc">Open - Weights LLMs: In-Depth Analysis of Adoption, Usage, and...</a></li>

</ul>
</details>

**Discussion**: Comments are largely positive, with users excited about the competition and eager to run the model locally. However, one user reported poor experience with Qwen 3.7 Pro for software engineering tasks, calling it 'unusable' and favoring DeepSeek V4 Pro. Others expressed hope for smaller sizes of Qwen 3.8 suitable for local use on consumer hardware.

**Tags**: `#AI`, `#LLM`, `#Open Weights`, `#Alibaba`, `#Qwen`

---

<a id="item-2"></a>
## [SRE replaces $120k bowling system with $1,600 ESP32s](https://news.ycombinator.com/item?id=48968606) ⭐️ 8.0/10

An SRE and bowling center owner reverse-engineered a legacy six-figure scoring system and built an open-source alternative using ESP32 microcontrollers and commodity hardware, reducing cost from over $100,000 to about $1,600. This demonstrates the massive cost-saving potential of retrofitting legacy industrial systems with modern open-source embedded technologies and could lower barriers for small bowling alleys to upgrade or maintain scoring systems. The system uses ESP32s communicating via ESPNow in a star-topology mesh with an RS485 wired fallback, and a Raspberry Pi as a lane computer running Redis and a state machine. The entire stack, called OpenLaneLink, is planned for open-source release.

hackernews · section33 · Jul 19, 14:41

**Background**: ESP32 is a low-cost, low-power microcontroller family with integrated Wi-Fi and Bluetooth, widely used in IoT applications. ESPNow is a proprietary communication protocol by Espressif that enables direct, low-latency, connectionless communication between ESP32 devices without a Wi-Fi router, forming a mesh network.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ESP32">ESP32</a></li>
<li><a href="https://www.espressif.com/en/products/socs/esp32">ESP32 Wi-Fi & Bluetooth SoC | Espressif Systems</a></li>

</ul>
</details>

**Discussion**: Comments share similar experiences: a mini bowling lane owner using an old Intel MCS-48 CPU, a mechanic's son recalling relay-based machines, and an engineer advocating for retrofitting old machine tools. The sentiment is positive and supportive, with added context about the prevalence of such retrofitting opportunities.

**Tags**: `#reverse-engineering`, `#IoT`, `#embedded-systems`, `#bowling`, `#cost-reduction`

---

<a id="item-3"></a>
## [Minecraft Java Edition Switches to SDL3](https://www.minecraft.net/en-us/article/minecraft-26-3-snapshot-4) ⭐️ 8.0/10

Minecraft: Java Edition has adopted the SDL3 library (Simple DirectMedia Layer 3) to improve cross-platform support, replacing its previous SDL2-based input and window management. This update enhances performance and compatibility across Windows, macOS, and Linux (including Wayland), benefiting millions of players. It also demonstrates the growing adoption of SDL3 in major game engines. Known issues include crashes in exclusive fullscreen mode on Windows with multiple monitors and on Wayland. The LWJGL bindings for SDL3 were contributed by a member of the GTNH modpack team.

hackernews · ObviouslyFlamer · Jul 19, 11:48 · [Discussion](https://news.ycombinator.com/item?id=48967256)

**Background**: Simple DirectMedia Layer (SDL) is a cross-platform library that provides low-level access to audio, keyboard, mouse, joystick, and graphics hardware. SDL3 is the latest major version, offering improved performance and new features. Minecraft's switch to SDL3 aligns with the broader trend of game engines adopting modern libraries for better cross-platform support.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Simple_DirectMedia_Layer">Simple DirectMedia Layer - Wikipedia</a></li>
<li><a href="https://www.studyplan.dev/sdl3/what-is-sdl">What is SDL? An Introduction for C++ Game Developers</a></li>

</ul>
</details>

**Discussion**: The community is largely positive about the technical update, with some expressing concerns about blocking bugs like the fullscreen crashes. There is appreciation for the LWJGL bindings contributed by the modding community, and helpful porting resources were shared. Some commenters noted that Minecraft is evolving into a game engine in its own right.

**Tags**: `#Minecraft`, `#SDL3`, `#game development`, `#cross-platform`, `#open source`

---

<a id="item-4"></a>
## [Claude Code adopts Bun rewritten in Rust](https://simonwillison.net/2026/Jul/19/claude-code-in-bun-in-rust/#atom-everything) ⭐️ 8.0/10

Simon Willison confirmed that Claude Code v2.1.181 and later use the Bun runtime that has been rewritten from Zig to Rust, resulting in a 10% startup improvement on Linux. This change demonstrates that a major AI tool is now powered by a Rust-based JavaScript runtime, highlighting the growing reliance on Rust for performance and safety in tooling. It also shows the feasibility of large-scale runtime rewrites using AI-assisted coding, as the rewrite was done with Claude Code. The Rust version of Bun is not yet publicly released as a stable version; Claude Code ships a preview with version number Bun v1.4.0, while the latest public release is v1.3.14. The rewrite was done using around 50 dynamic workflows in Claude Code over 11 days.

rss · Simon Willison · Jul 19, 03:54 · [Discussion](https://news.ycombinator.com/item?id=48966569)

**Background**: Bun is a fast all-in-one JavaScript runtime and toolkit that originally used Zig as its implementation language. Recently, the Bun team rewrote the runtime in Rust to leverage Rust's memory safety and tooling advantages. Claude Code is an AI-powered coding assistant by Anthropic that uses Bun as its underlying JavaScript runtime.

<details><summary>References</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://bun.com/blog/bun-in-rust">Rewriting Bun in Rust | Bun Blog</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed reactions: some question why a TUI needs a JavaScript runtime at all, while others appreciate the technical rationale for the Zig-to-Rust switch. There is also concern about the governance and transparency of Bun's development, especially given the rapid AI-assisted rewrite and lack of public consultation.

**Tags**: `#Claude Code`, `#Bun`, `#Rust`, `#runtime`, `#AI tools`

---

<a id="item-5"></a>
## [Lessons from Selling 2,500 MIDI Recorders](https://chipweinberger.com/articles/20260719-hardware-is-not-so-hard) ⭐️ 8.0/10

The article's author shares key takeaways from selling 2,500 MIDI recorders, arguing that hardware development difficulty depends on product complexity rather than being inherently hard. This provides practical insights for aspiring hardware entrepreneurs, challenging the common VC narrative that hardware is universally hard and offering a nuanced perspective on scaling and design. The author built a simple product with 25 components and off-the-shelf parts, keeping the design manageable. The article emphasizes that success depends on product complexity and careful planning rather than mystical difficulty.

hackernews · chipweinberger · Jul 19, 10:34 · [Discussion](https://news.ycombinator.com/item?id=48966713)

**Background**: Hardware startups often face challenges like scaling, logistics, and cash flow. MIDI recorders capture musical performances as MIDI data, a standard protocol for electronic instruments. The author's product, JamCorder, is a simple, affordable device that records MIDI to SD cards without requiring an app.

**Discussion**: Commenters generally agree that hardware difficulty varies by product complexity, with some pointing out that scaling, logistics, and cash flow are real challenges. One user praised the JamCorder as a perfect product with zero complaints. Another argued that the "hardware is hard" statement is a VC oversimplification.

**Tags**: `#hardware`, `#MIDI`, `#entrepreneurship`, `#product development`, `#lessons learned`

---

<a id="item-6"></a>
## [How fork() duplicates a process without copying its memory](https://www.reddit.com/r/programming/comments/1v0uqah/how_fork_duplicates_a_process_without_copying_its/) ⭐️ 8.0/10

A visual explainer demonstrates how Linux's copy-on-write mechanism allows fork() to duplicate a 10 GB process almost instantly by sharing physical pages and only copying on write. This efficiency is crucial for systems programming: it enables fast process creation, supports Redis snapshots without doubling memory, and underpins Android's Zygote for rapid app launches. The explainer covers fork()+exec(), Redis snapshotting via fork, Android Zygote which preloads common classes, lazy zero pages that defer allocation, and related CVEs.

reddit · r/programming · /u/Ok_Marionberry8922 · Jul 19, 16:16

**Background**: The fork() system call creates a new process by duplicating the calling process. Without copy-on-write, forking a large process would require copying all its memory, which is slow and wasteful. Copy-on-write defers the copy until one of the processes writes to a shared page, allowing fast fork() with minimal overhead.

<details><summary>References</summary>
<ul>
<li><a href="https://source.android.com/docs/core/runtime/zygote">About the Zygote processes | Android Open Source Project</a></li>
<li><a href="https://en.wikipedia.org/wiki/Demand_paging">Demand paging - Wikipedia</a></li>
<li><a href="https://lwn.net/Articles/517465/">Adding a huge zero page [LWN.net]</a></li>

</ul>
</details>

**Tags**: `#fork`, `#copy-on-write`, `#operating-systems`, `#linux`, `#memory-management`

---

<a id="item-7"></a>
## [AI advice tripled confidence but slashed accuracy, study finds](https://thenextweb.com/news/ai-advice-suppresses-critical-thinking-wrong-answers-study) ⭐️ 7.0/10

A recent study found that participants who received AI advice were three times less accurate but twice as confident in their answers compared to those who did not use AI. This highlights a dangerous overreliance on AI systems, where users become more confident in incorrect answers, potentially undermining critical thinking in real-world applications. The study used an LLM that was known to provide incorrect answers to specific questions, and participants were allowed to skip questions if unsure, yet still fell into the confidence trap.

hackernews · rbanffy · Jul 19, 21:18 · [Discussion](https://news.ycombinator.com/item?id=48971738)

**Background**: The study examined how AI-generated advice affects human decision-making, specifically accuracy and confidence. It involved participants answering questions with or without AI assistance. This research is part of a growing concern about AI's impact on critical thinking.

**Discussion**: Community comments were mixed, with some criticizing the study's methodology, noting that it tested AI systems giving known wrong answers rather than general AI reliability. Others expressed broader concerns about AI eroding critical thinking and creating echo chambers.

**Tags**: `#AI`, `#critical thinking`, `#study`, `#confidence`, `#accuracy`

---

<a id="item-8"></a>
## [OpenAI Reduces Codex Context Window from 372k to 272k](https://github.com/openai/codex/pull/33972/files) ⭐️ 7.0/10

OpenAI has reduced the context window size for its Codex model from 372,000 tokens to 272,000 tokens, as reflected in a pull request to the official repository. This change has sparked debate about the effectiveness of context compaction techniques and the trade-offs between context size and model performance. It highlights the ongoing tension between providing larger contexts and maintaining output quality, especially for complex tasks involving detailed documents or codebases. The reduction implies increased reliance on context compaction to fit more information into the smaller window, which some users find degrades detail retention. The pull request notes the new limit of 272k tokens, down from the previous 372k.

hackernews · AmazingTurtle · Jul 19, 07:54 · [Discussion](https://news.ycombinator.com/item?id=48965850)

**Background**: OpenAI Codex is a series of large language models specialized for coding tasks, built on top of GPT-3 and trained on GitHub repositories. Context compaction is a technique that compresses long conversation or document histories while trying to preserve essential information, enabling models to handle longer interactions within a finite context window. The trade-off is that compaction can lose subtle details, affecting performance on tasks requiring precise recall.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(language_model)">OpenAI Codex (language model) - Wikipedia</a></li>
<li><a href="https://kargarisaac.medium.com/the-fundamentals-of-context-management-and-compaction-in-llms-171ea31741a2">The Fundamentals of Context Management and Compaction in LLMs</a></li>

</ul>
</details>

**Discussion**: The community comments express mixed feelings: some users lament the loss of detail after compaction and criticize the reduction from 372k to 272k, noting that competitors like Anthropic offer larger contexts. Others argue that very long contexts degrade model intelligence and that it's better to stay under 300k, while some users report better results by clearing context and starting fresh rather than relying on compaction.

**Tags**: `#OpenAI`, `#Codex`, `#context size`, `#LLM`, `#model optimization`

---

<a id="item-9"></a>
## [IndieWeb journey reveals benefits and barriers](https://en.andros.dev/blog/0b8e451e/i-joined-the-indieweb-heres-what-i-learned/) ⭐️ 7.0/10

A personal blog post details the author's experience joining the IndieWeb movement, covering both the empowerment of owning one's content and the technical challenges of setting up POSSE (Publish on Your Own Site, Syndicate Elsewhere) protocols. This article highlights the ongoing tension between user empowerment and usability in decentralized social media, a critical issue as people seek alternatives to corporate platforms. The author implemented POSSE using tools like Indiekit, but notes that the setup still requires technical knowledge, limiting mainstream adoption.

hackernews · andros · Jul 19, 11:14 · [Discussion](https://news.ycombinator.com/item?id=48966984)

**Background**: The IndieWeb is a movement that advocates for individuals to own their data by publishing on personal websites and syndicating to social media silos. POSSE (Publish on Your Own Site, Syndicate Elsewhere) is a key practice where content is first posted on one's own site and then copied to other platforms, ensuring primary ownership remains with the author. This approach contrasts with corporate social media where platforms control content.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/IndieWeb">IndieWeb - Wikipedia</a></li>
<li><a href="https://indieweb.org/POSSE">POSSE - IndieWeb</a></li>
<li><a href="https://en.wikipedia.org/wiki/IndieWebCamp">IndieWebCamp - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters expressed mixed views: some criticized the IndieWeb's technical complexity as a barrier for most users, while others praised tools like Indiekit and Nostr as easier alternatives. There was also criticism of the IndieWeb's perceived elitism, with commenters noting that many personal sites include professional headshots and CVs, contradicting the anti-corporate ethos.

**Tags**: `#IndieWeb`, `#web development`, `#decentralization`, `#social media`, `#POSSE`

---

<a id="item-10"></a>
## [Moonshot AI pauses Kimi K3 subscriptions due to demand](https://twitter.com/kimi_moonshot/status/2078855608565207130) ⭐️ 7.0/10

Moonshot AI temporarily paused new subscriptions for its flagship Kimi K3 model due to overwhelming demand over 48 hours, prioritizing existing users over new growth. This decision signals a customer-first approach in AI, contrasting with firms that silently degrade service. It also highlights the intense demand for large-scale, open-source models like Kimi K3. Kimi K3 has 2.8 trillion parameters, uses Kimi Delta Attention (hybrid linear attention), and supports a 1M-token context window. Existing subscribers remain unaffected.

hackernews · serialx · Jul 19, 16:02 · [Discussion](https://news.ycombinator.com/item?id=48969291)

**Background**: Moonshot AI is a Beijing-based AI company founded in 2023, one of China's 'AI Tigers'. Kimi K3 is the world's first open-source model in the 3-trillion-parameter class, released in July 2026, designed for long-context coding, reasoning, and knowledge work.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kimi_K3">Kimi K3</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>

</ul>
</details>

**Discussion**: Commenters praised Moonshot's customer-first decision, with one noting it's a 'beautiful paragraph' to prioritize existing users. Some shared technical observations about Kimi K3's heavy use of RNN/linear attention layers, suggesting efficiency for long-context tasks.

**Tags**: `#AI`, `#Moonshot`, `#Kimi K3`, `#subscriptions`, `#demand`

---

<a id="item-11"></a>
## [AI Mania Is Eviscerating Global Decision-Making](https://simonwillison.net/2026/Jul/19/ai-mania/#atom-everything) ⭐️ 7.0/10

Nik Suresh published a blog post criticising how AI hype is leading to irrational decision-making in large companies, illustrated with anonymous anecdotes of executives endorsing AI strategies without using AI tools and engineers rewriting codebases in Zig to appear productive. This article highlights a pervasive issue in the tech industry where AI hype distorts decision-making, potentially wasting resources and undermining genuine innovation. It serves as a cautionary reminder for executives and engineers to ground AI adoption in reality. Notable anecdotes include a $2B+ revenue company's executive who never used ChatGPT but approved an AI-centric technical strategy, and an engineer who had an AI rewrite a Go repository in Zig to climb a 'token leaderboard'. Another story reveals vendors suppress honesty to avoid upsetting executives who believe in unrealistic productivity gains.

rss · Simon Willison · Jul 19, 05:06

**Background**: The article is part of ongoing criticism of AI hype in the tech industry. Zig is a system programming language similar to C, designed for performance and safety, often used as a replacement for C. ChatGPT is a widely known AI chatbot. The post was shared on Hacker News, a popular tech discussion platform, indicating community interest.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://ziglang.org/">Home Zig Programming Language</a></li>

</ul>
</details>

**Tags**: `#AI hype`, `#decision-making`, `#industry critique`, `#tech culture`

---

<a id="item-12"></a>
## [Google's IDE Evolution: A Historical Retrospective](https://www.reddit.com/r/programming/comments/1v0gkin/a_history_of_ides_at_google/) ⭐️ 7.0/10

A Reddit post shares a retrospective on the development and adoption of integrated development environments (IDEs) at Google over the years. This retrospective offers valuable insights into how a major tech company like Google shaped its internal development tooling, which can influence industry trends and best practices. The post details the evolution from early editors to modern IDEs, highlighting key decisions and trade-offs made by Google's engineering teams.

reddit · r/programming · /u/fagnerbrack · Jul 19, 04:17

**Background**: Integrated Development Environments (IDEs) combine code editing, debugging, and build tools into a single application. Google has developed several internal tools over the years, such as GoogleCL and internal variants of Eclipse and IntelliJ, before settling on modern solutions like IntelliJ IDEA-based IDEs.

**Tags**: `#IDE`, `#Google`, `#software engineering`, `#history`, `#development tools`

---

<a id="item-13"></a>
## [Time Mismanagement in Distributed Systems: A Failure Mode](https://www.reddit.com/r/programming/comments/1v0snnz/beyond_happy_path_engineering_time/) ⭐️ 7.0/10

This article explores how clock drift, deadline mismatches, retries, and TTL behavior cause real incidents in distributed systems, emphasizing that time-related assumptions often break in production. Understanding these failure modes is critical for engineers building reliable distributed systems, as ignoring time issues can lead to data corruption, performance degradation, and unexpected outages. The article describes specific scenarios where clock drift causes out-of-order events, deadline mismatches lead to task failures, retries amplify load, and TTL inconsistencies create stale data.

reddit · r/programming · /u/OtherwisePush6424 · Jul 19, 14:54

**Background**: Distributed systems rely on time for coordination, ordering, and failure detection. However, clocks on different machines inevitably drift due to hardware imperfections, and synchronizing them perfectly is impossible. Common mechanisms like NTP reduce drift but cannot eliminate it, and assumptions about bounded clock skew often fail. This makes time-based operations such as leases, heartbeats, and cache TTLs vulnerable to bugs that manifest only under real-world conditions.

<details><summary>References</summary>
<ul>
<li><a href="https://flowfuse.com/blog/2026/07/time-synchronization-edge-devices/">Handling Clock Drift in Distributed Edge Devices • FlowFuse</a></li>
<li><a href="https://www.geeksforgeeks.org/distributed-systems/clock-synchronization-in-distributed-system/">Clock Synchronization in Distributed Systems - GeeksforGeeks</a></li>

</ul>
</details>

**Tags**: `#distributed systems`, `#time`, `#fault tolerance`, `#reliability`

---

<a id="item-14"></a>
## [Building Merkle Tree AIR Script in Plonky3](https://www.reddit.com/r/programming/comments/1v0vext/a_tutorial_on_building_a_merkle_tree_air_script/) ⭐️ 7.0/10

A tutorial has been published that guides developers through creating a Merkle tree Algebraic Intermediate Representation (AIR) script using the Plonky3 zero-knowledge proof framework. This tutorial helps developers gain practical experience with Plonky3, a state-of-the-art ZK proving system, and demonstrates how to implement Merkle tree proofs using its modular architecture. The tutorial covers constructing an AIR that enforces Merkle tree opening constraints, leveraging Plonky3's polynomial IOP toolkit which supports multiple commitment schemes like Brakedown.

reddit · r/programming · /u/badcryptobitch · Jul 19, 16:43

**Background**: Plonky3 is an open-source toolkit by Polygon Zero for implementing polynomial IOPs like PLONK and STARKs, designed for high-performance recursive proofs. AIR (Algebraic Intermediate Representation) is a way to represent computations as polynomial constraints that connect rows of an execution trace, which is central to STARK-based proving.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Plonky3/Plonky3">GitHub - Plonky3/Plonky3: A toolkit for polynomial IOPs (PIOPs) Polygon Plonky3 is Production Ready GitHub - Plonky3/awesome-plonky3: A curated list of Plonky3 ... Open Source Polygon Plonky3 Is Once Again the Fastest ZK ... Breaking Down Proof Construction in Plonky3: The Fibonacci ... Production-Ready: Plonky3, Polygon's Advanced Zero-Knowledge ...</a></li>
<li><a href="https://polygon.technology/blog/polygon-plonky3-the-next-generation-of-zk-proving-systems-is-production-ready">Polygon Plonky3 is Production Ready</a></li>
<li><a href="https://deepwiki.com/Plonky3/Plonky3/6-air-(algebraic-intermediate-representation)">AIR (Algebraic Intermediate Representation) | Plonky3/Plonky3 ...</a></li>

</ul>
</details>

**Tags**: `#merkle-tree`, `#plonky3`, `#zero-knowledge-proofs`, `#tutorial`, `#cryptography`

---

<a id="item-15"></a>
## [Last MPEG-4 Visual Patent Expired, Freeing Xvid/DivX](https://www.phoronix.com/news/Last-MPEG-4-Patent-Expired) ⭐️ 6.0/10

The last patent covering MPEG-4 Visual (Part 2) has expired, removing patent restrictions on the Xvid and DivX codecs. This milestone was reached when the final active patent, held in Brazil, lapsed. This marks a significant milestone for legacy video codecs, enabling unrestricted use of Xvid and DivX for encoding and distribution. However, the impact is limited because the more widely used H.264 codec remains under patent protection for several more years. The expired patent was the only remaining one active in Brazil, as US and EU patents for MPEG-4 Part 2 had expired earlier. It is important to note that this applies to MPEG-4 Part 2 (based on H.263), not to H.264/AVC.

hackernews · LorenDB · Jul 19, 16:45 · [Discussion](https://news.ycombinator.com/item?id=48969635)

**Background**: MPEG-4 Visual is a video compression standard introduced in the late 1990s as part of the MPEG-4 suite. Xvid and DivX are popular codecs that implement MPEG-4 Part 2 Advanced Simple Profile (ASP). Patent restrictions previously hindered open-source use and distribution of these codecs, and their expiration allows free use without licensing fees.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MPEG-4">MPEG-4 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/MPEG-4_Part_2">MPEG-4 Part 2 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Xvid">Xvid - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters emphasize that this concerns MPEG-4 Part 2 (Xvid/DivX) and not H.264, criticizing Phoronix for potentially misleading reporting. Some users look forward to the eventual expiration of H.264 patents and the arrival of future codecs like MPEG-5.

**Tags**: `#patents`, `#video codecs`, `#MPEG-4`, `#Xvid`, `#DivX`

---

<a id="item-16"></a>
## [Home Server Rebirth: From Pi SD to SSD & Mini-PCs](https://sgt.hootr.club/blog/home-server-rebirth/) ⭐️ 6.0/10

A user documents their home server's transition from a Raspberry Pi with frequent SD card corruption to more reliable USB/SATA SSDs and ultimately a mini-PC, highlighting the common failure points of SD cards in 24/7 operation. This account underscores a widespread issue for hobbyist home servers: Raspberry Pi SD card failures due to constant writes. It validates the trend of moving to USB/SATA SSDs or low-power x86 mini-PCs for improved reliability and performance. The user's initial setup ran on a Raspberry Pi 4B with an SD card, which failed after repeated corruption. They upgraded to a Pi 5 with a Waveshare PoE+SSD HAT for SATA SSD boot, and later considered a mini-PC like an Intel NUC for better RAM capacity and NVMe support.

hackernews · steinuil · Jul 19, 10:44 · [Discussion](https://news.ycombinator.com/item?id=48966769)

**Background**: Raspberry Pis are popular for home servers but microSD cards have limited write endurance, often failing under constant logging or database writes typical of services like Home Assistant or Docker. USB/SATA SSDs offer greater reliability and performance, while x86 mini-PCs provide even more flexibility with standard RAM and storage interfaces. The Raspberry Pi bootloader now supports USB boot natively on recent models.

<details><summary>References</summary>
<ul>
<li><a href="https://raspberry.tips/en/calculate-raspberry-pi-sd-card-lifespan-test-now">Calculate Raspberry Pi SD Card Lifespan : Test Now!</a></li>
<li><a href="https://raspberrytips.com/raspberry-pi-storage-showdown/">Raspberry Pi Storage Options Compared: SD, USB, SSD & NVMe</a></li>

</ul>
</details>

**Discussion**: Commenters widely agree on SD card fragility, with some sharing workarounds like imaging multiple SD cards for quick swaps or using USB flash drives. Others recommend NVMe on Rockchip SBCs or the convenience of Waveshare HATs. A user notes that RAM prices make mini-PCs less attractive despite cheap other components.

**Tags**: `#home server`, `#Raspberry Pi`, `#SD card`, `#storage`, `#hobbyist`

---

<a id="item-17"></a>
## [Wuling Bingo May Be Rebadged as Chevy for North America](https://electrek.co/2026/07/19/chinese-wuling-bingo-could-come-to-north-america-as-an-entry-level-chevy-ev/) ⭐️ 6.0/10

Rumors indicate that the Chinese Wuling Bingo electric hatchback could be rebadged as a Chevrolet entry-level EV for global markets, potentially reviving the spirit of the Geo Metro. If confirmed, this would bring a low-cost electric vehicle to North America, leveraging GM's partnership with SAIC-GM-Wuling to offer an affordable EV option, potentially competing with other budget EVs and reviving the legacy of the fuel-sipping Geo Metro. The Wuling Bingo is a subcompact hatchback produced by SAIC-GM-Wuling (SGMW), a joint venture between SAIC, GM, and Liuzhou Wuling. The Geo Metro was a GM collaboration with Suzuki in the 1990s known for its fuel efficiency.

rss · Electrek · Jul 19, 22:28

**Background**: The Wuling Bingo, also known as the Binguo, is a battery electric subcompact hatchback launched in 2023 by SGMW in China. It is known for its retro-futuristic design and affordability. The Geo Metro was a compact car sold in North America from 1989 to 2001, co-developed by GM and Suzuki, and prized for its low cost and high fuel efficiency. Rebadging the Bingo as a Chevy would follow a similar strategy of offering an entry-level vehicle under a familiar brand.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wuling_Bingo_Plus">Wuling Bingo Plus</a></li>
<li><a href="https://en.wikipedia.org/wiki/Geo_Metro">Geo Metro - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Geo_(automobile)">Geo (automobile) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#electric vehicles`, `#Chevy`, `#Wuling`, `#automotive rumors`, `#North America`

---

<a id="item-18"></a>
## [Transcribe.cpp: Open-Source C++ Speech-to-Text Library](https://www.reddit.com/r/programming/comments/1v0woh5/transcribecpp/) ⭐️ 6.0/10

transcribe.cpp, a C/C++ speech-to-text inference library based on ggml, has been released, supporting 16 model families and over 60 variants with GPU backends including Metal, Vulkan, and CUDA, as well as a CPU path accelerated by tinyBLAS. This library makes it easier to integrate fast, local speech-to-text into applications without relying on cloud services, enhancing privacy and reducing latency. Its support for multiple model families provides flexibility for developers. The library uses GGUF model format for inference and has been numerically validated with word error rate (WER) testing to match reference implementations. It was developed by Mozilla.ai through their Builders in Residence program.

reddit · r/programming · /u/namanyayg · Jul 19, 17:32

**Background**: ggml is a tensor library for machine learning inference, optimized for CPU and GPU performance. Speech-to-text (STT) models transcribe audio into text. transcribe.cpp builds on ggml to support various STT models like Whisper, enabling local transcription without cloud dependencies.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/handy-computer/transcribe.cpp">GitHub - handy-computer/transcribe.cpp: ggml speech-to-text ...</a></li>
<li><a href="https://blog.mozilla.ai/announcing-transcribe-cpp/">Announcing transcribe.cpp</a></li>

</ul>
</details>

**Tags**: `#C++`, `#transcription`, `#machine learning`, `#open source`, `#tool`

---

<a id="item-19"></a>
## [Commutative Complex Numbers in Plain C](https://www.reddit.com/r/programming/comments/1v0of6b/commutative_complex_number_theory_in_plain_c/) ⭐️ 6.0/10

A C implementation demonstrates commutative properties of complex number arithmetic, exploring theoretical aspects within the language's constraints. This offers a novel pedagogical approach to understanding both complex numbers and C's type system, though it remains a niche academic exercise. The implementation likely uses structs and operator overloading via macros or functions to achieve commutativity, possibly with custom multiplication and addition routines.

reddit · r/programming · /u/DataBaeBee · Jul 19, 11:45

**Background**: Complex numbers are not natively supported in C, so developers often implement them as structs with real and imaginary parts. Commutativity means that a * b equals b * a, which holds for complex multiplication but can be tricky to enforce in code.

**Tags**: `#C`, `#complex numbers`, `#mathematics`, `#programming`

---

<a id="item-20"></a>
## [Real-World CPU Bottleneck Debugging Story](https://www.reddit.com/r/programming/comments/1v0llyh/finding_zombies_in_our_systems_a_realworld_story/) ⭐️ 6.0/10

A developer shares a real-world story about identifying and fixing CPU bottlenecks caused by zombie processes in a production system. This story provides practical insights into performance debugging and system monitoring, helping engineers avoid similar pitfalls in their own systems. The diagnosis involved tracking down zombie processes that accumulated and consumed CPU resources, highlighting the importance of proper process management and monitoring tools.

reddit · r/programming · /u/fagnerbrack · Jul 19, 09:04

**Background**: A zombie process is a terminated process that still has an entry in the process table because its parent has not read its exit status. In Linux, such processes appear with a 'Z' status in tools like ps. While typically short-lived, accumulated zombie processes can exhaust system resources and cause CPU bottlenecks.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@nirbhaysingh281/what-is-a-zombie-process-3576a4ac9bee">What is a zombie process ?. Definition of a Zombie Process | Medium</a></li>
<li><a href="https://www.geeksforgeeks.org/operating-systems/difference-between-zombie-orphan-and-daemon-processes/">Difference between Zombie , Orphan and Daemon Processes</a></li>

</ul>
</details>

**Tags**: `#performance`, `#debugging`, `#CPU`, `#systems`, `#real-world`

---

<a id="item-21"></a>
## [Developing TUI in Go with Bubble Tea](https://www.reddit.com/r/programming/comments/1v0xaws/developing_a_tui_in_go_with_bubble_tea/) ⭐️ 6.0/10

A tutorial on building terminal user interfaces (TUI) in Go using the Bubble Tea framework has been shared on Reddit, providing developers with a practical guide to creating interactive terminal applications. TUI applications are valuable for command-line tools and system utilities, and Bubble Tea's Elm-like architecture simplifies state management and event handling, making Go a stronger choice for terminal-based software. Bubble Tea operates on a model-update-view pattern inspired by The Elm Architecture, where messages are processed in Update() and the UI is rendered in View(), requiring these functions to be fast to avoid UI lag.

reddit · r/programming · /u/der_gopher · Jul 19, 17:56

**Background**: A terminal user interface (TUI) is a text-based interface that runs in a terminal emulator, using characters and colors to present interactive controls. Bubble Tea is a Go framework that implements The Elm Architecture (TEA), a pattern for building reactive UIs with immutable state and message passing. It is well-suited for both simple and complex terminal applications, supporting inline, full-window, or mixed modes.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/charmbracelet/bubbletea">GitHub - charmbracelet/ bubbletea : A powerful little TUI framework</a></li>
<li><a href="https://en.wikipedia.org/wiki/Text-based_user_interface">Text-based user interface - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Go`, `#TUI`, `#Bubble Tea`, `#Programming Tutorial`

---