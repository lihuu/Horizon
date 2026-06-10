---
layout: default
title: "Horizon Summary: 2026-06-04 (EN)"
date: 2026-06-04
lang: en
---

> From 32 items, 18 important content pieces were selected

---

1. [Elixir v1.20 Introduces Gradual Typing](#item-1) ⭐️ 9.0/10
2. [Google Releases Gemma 4 12B, an Encoder-Free Multimodal Model](#item-2) ⭐️ 9.0/10
3. [Soundbar Hacked via Bluetooth to Emulate Keyboard](#item-3) ⭐️ 9.0/10
4. [Let's Encrypt Plans Post-Quantum Migration with Merkle Tree Certificates](#item-4) ⭐️ 9.0/10
5. [ESP32-S31 Introduces RISC-V Cores with SIMD and BitScrambler](#item-5) ⭐️ 9.0/10
6. [DaVinci Resolve 21 Adds AI Tools and Photo Management](#item-6) ⭐️ 8.0/10
7. [Ted Chiang: AI Is Not Conscious Without Embodiment](#item-7) ⭐️ 8.0/10
8. [Uber Caps AI Coding Tool Usage to Control Costs](#item-8) ⭐️ 8.0/10
9. [Mathematicians Warn as AI Rapidly Gains Ground](#item-9) ⭐️ 8.0/10
10. [Memory Layout Optimization Deep Dive](#item-10) ⭐️ 8.0/10
11. [Tesla retroactively adds 'supervised' to FSD contracts](#item-11) ⭐️ 8.0/10
12. [PlayStation Hardware Deep-Dive Analysis](#item-12) ⭐️ 7.0/10
13. [Meta allows workers 30-minute opt-out from tracking](#item-13) ⭐️ 7.0/10
14. [Apple Doubles MacBook Neo Production Due to Demand](#item-14) ⭐️ 7.0/10
15. [Caterpillar BEPU: Plug-and-play electric engine swap](#item-15) ⭐️ 7.0/10
16. [Visual Studio Code 1.123 Released with Enhancements](#item-16) ⭐️ 6.0/10
17. [SEG Solar Announces Third Texas Factory](#item-17) ⭐️ 6.0/10
18. [Tesla expands Robotaxi to all Austin metro but fleet still tiny](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Elixir v1.20 Introduces Gradual Typing](https://elixir-lang.org/blog/2026/06/03/elixir-v1-20-0-released/) ⭐️ 9.0/10

Elixir v1.20, released on June 3, 2026, introduces gradual typing, allowing developers to optionally add type annotations. This marks a major milestone as it addresses a long-standing community request for static type checking in the dynamic language. This feature enhances code reliability and developer productivity by catching type errors at compile time, while maintaining backward compatibility. It could increase adoption of Elixir in larger codebases and critical systems where static typing is preferred. The gradual type system is built into the compiler and does not require external tools like Dialyzer. According to community discussion, it may affect runtime performance, but the exact trade-offs are still being evaluated.

hackernews · cloud8421 · Jun 3, 19:02 · [Discussion](https://news.ycombinator.com/item?id=48388324)

**Background**: Gradual typing is a type system that allows both statically and dynamically typed code within the same language, letting developers choose where to add type annotations. It bridges the gap between the flexibility of dynamic languages and the safety of static types. Elixir, traditionally dynamically typed, has long sought such a feature.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gradual_typing">Gradual typing</a></li>
<li><a href="https://jsiek.github.io/home/WhatIsGradualTyping.html">What is Gradual Typing | Jeremy Siek</a></li>

</ul>
</details>

**Discussion**: Comments reflect excitement and cautious optimism. A longtime Elixir developer (losvedir) is thrilled but curious about how it compares to Dialyzer's success typing. Another user (sestep) asks about asymptotic performance implications, referencing research showing gradual typing can sometimes make programs asymptotically slower. Some commenters express skepticism that gradually adding types to a dynamic language can match the experience of natively typed languages.

**Tags**: `#Elixir`, `#gradual typing`, `#programming languages`, `#static typing`, `#release`

---

<a id="item-2"></a>
## [Google Releases Gemma 4 12B, an Encoder-Free Multimodal Model](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemma-4-12b/) ⭐️ 9.0/10

Google introduced Gemma 4 12B, a multimodal model that eliminates the traditional vision encoder in favor of a lightweight embedding module consisting of a single matrix multiplication, positional embedding, and normalizations. This marks a shift towards encoder-free architectures in open-source AI. This release could lower the barrier for deploying multimodal AI on consumer hardware by reducing model complexity and memory requirements. It also demonstrates Google's commitment to open-source AI, potentially accelerating innovation in the field. The lightweight embedding module has only 35 million parameters, which may raise questions about its robustness compared to larger vision encoders like SigLIP. The model is open-source and available through Google's platforms.

hackernews · rvz · Jun 3, 16:04 · [Discussion](https://news.ycombinator.com/item?id=48385906)

**Background**: Traditional multimodal models like CLIP and LLaVA use a separate vision encoder (e.g., a Vision Transformer) to process images before combining with a language model. Gemma 4 12B's encoder-free design removes this separate component, making the model more efficient and easier to deploy. This is part of a broader industry trend toward unified, simpler architectures for multimodal AI.

<details><summary>References</summary>
<ul>
<li><a href="https://rocm.blogs.amd.com/software-tools-optimization/vllm-dp-vision/README.html">Accelerating Multimodal Inference in vLLM: The... — ROCm Blogs</a></li>
<li><a href="https://milvus.io/ai-quick-reference/what-are-lightweight-embedding-models">What are lightweight embedding models?</a></li>

</ul>
</details>

**Discussion**: Community reactions were mixed: user 'senko' tested the Q4 quant and found output decent but with minor syntax errors, while 'minimaxir' questioned the 'encoder-free' label, noting the embedding module still performs encoding. Others debated Google's strategic motives for releasing open models, with speculation ranging from ecosystem control to goodwill.

**Tags**: `#AI`, `#multimodal`, `#open-source`, `#google`, `#machine learning`

---

<a id="item-3"></a>
## [Soundbar Hacked via Bluetooth to Emulate Keyboard](https://blog.nns.ee/2026/06/03/katana-badusb/) ⭐️ 9.0/10

A security researcher remotely compromised the firmware of a Creative Sound Blaster Katana V2X soundbar via unauthenticated Bluetooth, enabling it to emulate a keyboard and send arbitrary keystrokes to the connected PC. This demonstrates a novel attack vector where a seemingly innocuous audio device can be weaponized to inject keystrokes, bypassing traditional security controls. It highlights the systemic risk of unauthenticated firmware updates in USB peripherals, potentially affecting millions of devices. The attack exploits the soundbar's unauthenticated Bluetooth firmware update mechanism, modifying the USB device descriptor to make it recognized as a keyboard. The researcher also released a third-party patch to fix the vulnerability, as the vendor did not acknowledge it as a security issue.

hackernews · xx_ns · Jun 3, 10:53 · [Discussion](https://news.ycombinator.com/item?id=48382310)

**Background**: Bluetooth supports HID profiles for wireless keyboards and mice, but devices like soundbars typically only use audio profiles. However, if a device connects via USB and has flashable firmware accessible over Bluetooth, an attacker can replace the firmware with one that enumerates as a keyboard. This is similar to earlier Bluetooth HID spoofing attacks, but here the attack propagates through the USB connection to the host computer.

<details><summary>References</summary>
<ul>
<li><a href="https://www.edgescan.com/bluetooth-and-the-invisible-security-threat-youre-probably-not-listening-to/">Bluetooth and the Invisible Security Threat You're... | Edgescan</a></li>
<li><a href="https://www.theverge.com/news/630647/samsung-q990d-soundbar-freezing-bricked-firmware-update">Samsung soundbar owners report major problems after latest ... Faulty firmware is bricking high-end Samsung soundbars An Automatic Update Is Breaking Samsung Soundbars Samsung admits a faulty software update bricked multiple ... Samsung admits a bad software update has been bricking its ... A buggy update is bricking Samsung soundbars—users left ... Samsung confirmed: Soundbars paralyzed by firmware update</a></li>
<li><a href="https://www.hackster.io/news/marc-newlin-s-keyboard-spoofing-attack-sends-arbitrary-commands-to-android-ios-macos-and-linux-21a738d6f548">Marc Newlin's Keyboard Spoofing Attack Sends... - Hackster.io</a></li>

</ul>
</details>

**Discussion**: Community comments express frustration that the vendor dismissed the issue as not a security risk, despite the clear attack vector. Some users speculate on wider implications, such as worm-like propagation through supply chains, while others applaud the researcher for publishing a fix.

**Tags**: `#security`, `#vulnerability`, `#IoT`, `#Bluetooth`, `#HID`

---

<a id="item-4"></a>
## [Let's Encrypt Plans Post-Quantum Migration with Merkle Tree Certificates](https://letsencrypt.org/2026/06/03/pq-certs) ⭐️ 9.0/10

Let's Encrypt announced plans to migrate to post-quantum certificates using Merkle Tree Certificates (MTCs), aiming to prepare for the threat of quantum computing to current cryptographic algorithms. This is significant because Let's Encrypt is the world's largest certificate authority, providing free TLS certificates to millions of websites. Their adoption of post-quantum cryptography will drive industry-wide migration and ensure long-term security against future quantum attacks. Merkle Tree Certificates integrate public logging directly into the certificate, reducing overhead and making the handshake smaller than current Web PKI even with post-quantum algorithms. This move comes after NIST standardized the first post-quantum cryptographic algorithms in 2024.

hackernews · SGran · Jun 3, 15:06 · [Discussion](https://news.ycombinator.com/item?id=48385114)

**Background**: Post-quantum cryptography (PQC) aims to develop algorithms secure against quantum computers, which could break widely used public-key systems using Shor's algorithm. The threat is considered urgent due to 'harvest now, decrypt later' attacks, where encrypted data is stored today for future decryption. Merkle Tree Certificates are a proposed new certificate format that combines issuance and transparency, addressing the size and performance challenges of large post-quantum signatures.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography</a></li>
<li><a href="https://www.ietf.org/archive/id/draft-davidben-tls-merkle-tree-certs-06.html">Merkle Tree Certificates - ietf.org</a></li>
<li><a href="https://blog.cloudflare.com/bootstrap-mtc/">Keeping the Internet fast and secure- introducing Merkle Tree Certificates</a></li>

</ul>
</details>

**Discussion**: The community expressed excitement and cautious optimism. User skmurphy noted the science-fiction nature of preparing for quantum threats, while BoppreH acknowledged the challenge of replacing decades of battle-tested infrastructure. Technical discussions focused on hybrid constructions and the advantages of MTCs, such as integrated transparency and smaller handshake sizes.

**Tags**: `#post-quantum cryptography`, `#TLS`, `#Let's Encrypt`, `#Merkle Tree Certificates`, `#certificate authority`

---

<a id="item-5"></a>
## [ESP32-S31 Introduces RISC-V Cores with SIMD and BitScrambler](https://www.espressif.com/en/products/socs/esp32-s31) ⭐️ 9.0/10

Espressif announced the ESP32-S31 SoC, which features RISC-V cores with SIMD instructions and a new BitScrambler peripheral for programmable data transformations during DMA transfers. This marks a significant shift toward open-source toolchains for embedded systems, enabling easy use of Rust (via `rustup target add riscv32imac-unknown-none-elf`) and reducing reliance on proprietary SDKs. The BitScrambler offers flexibility similar to the Raspberry Pi Pico's PIO, broadening the chip's applicability for custom protocols and signal processing. The ESP32-S31 includes SIMD instructions that accelerate parallel data processing, and the BitScrambler is a programmable peripheral integrated into the DMA stream for bit-level transformations. However, the naming expansion of the ESP32 family (with over 10 variants) has caused confusion among developers, as many associate "ESP32" only with the original WROOM-32E model.

hackernews · volemo · Jun 3, 16:10 · [Discussion](https://news.ycombinator.com/item?id=48385965)

**Background**: SIMD (Single Instruction, Multiple Data) allows a CPU to process multiple data points with one instruction, improving performance in media and signal processing tasks. The BitScrambler is a peripheral that transforms data formats during memory-to-peripheral or peripheral-to-memory transfers using a user-supplied program, offloading such work from the CPU. RISC-V is an open-standard instruction set architecture that enables customizable processor designs and broader toolchain support.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Single_instruction,_multiple_data">Single instruction, multiple data - Wikipedia</a></li>
<li><a href="https://docs.espressif.com/projects/esp-idf/en/stable/esp32p4/api-reference/peripherals/bitscrambler.html">BitScrambler Driver - ESP32-P4 - — ESP-IDF Programming Guide v6.0 documentation</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement about native RISC-V support simplifying Rust embedded development, with one noting that toolchain setup is now just a `rustup target add` command. The BitScrambler drew comparisons to the RP2040's PIO, seen as a powerful feature. However, several users voiced frustration over the proliferation of ESP32 model numbers, causing confusion about which chip is being referenced.

**Tags**: `#ESP32`, `#RISC-V`, `#Embedded Systems`, `#Espressif`, `#Microcontrollers`

---

<a id="item-6"></a>
## [DaVinci Resolve 21 Adds AI Tools and Photo Management](https://www.blackmagicdesign.com/products/davinciresolve/whatsnew) ⭐️ 8.0/10

Blackmagic Design has released DaVinci Resolve 21, introducing AI-powered features and integrated photo management capabilities, effectively merging video editing with photo workflow. This update positions DaVinci Resolve as a comprehensive all-in-one creative suite, challenging Adobe's dominance by offering a free version with professional-grade tools and now photo management, appealing to content creators and professionals alike. The new photo management module resembles Adobe Lightroom's functionality, and the AI features include motion graphics enhancements. However, the free version remains limited, requiring a Studio license ($299) for advanced AI and photo editing capabilities.

hackernews · pentagrama · Jun 3, 14:18 · [Discussion](https://news.ycombinator.com/item?id=48384482)

**Background**: DaVinci Resolve is a professional non-linear video editing, color grading, and audio post-production software developed by Blackmagic Design. It has a free version that is widely used, and a paid Studio version. The addition of photo management marks a significant expansion beyond traditional video editing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DaVinci_Resolve">DaVinci Resolve - Wikipedia</a></li>
<li><a href="https://www.blackmagicdesign.com/products/davinciresolve">DaVinci Resolve | Blackmagic Design</a></li>

</ul>
</details>

**Discussion**: Community comments are largely positive, with users praising the new features despite AI skepticism. One user highlights that the photo management addition alone is 'huge' and could be the best on Linux. Others appreciate AI tools for workflow improvements, while a user notes that Resolve requires a discrete GPU, unlike Blender's VSE.

**Tags**: `#video editing`, `#AI`, `#photo management`, `#Blackmagic`

---

<a id="item-7"></a>
## [Ted Chiang: AI Is Not Conscious Without Embodiment](https://www.theatlantic.com/philosophy/2026/06/no-artificial-intelligence-is-not-conscious/687378/) ⭐️ 8.0/10

Ted Chiang published an article in The Atlantic arguing that current artificial intelligence is not conscious because it lacks a physical body and sensory experience. This argument challenges growing narratives of AI sentience and underscores the need for embodiment in consciousness research, influencing public and scientific debate. Chiang outlines specific requirements for AI to be considered conscious, including having a body and sense organs, which enable desires and intentional language use.

hackernews · lordleft · Jun 3, 17:51 · [Discussion](https://news.ycombinator.com/item?id=48387270)

**Background**: Embodied cognition theory holds that cognitive processes are deeply dependent on the physical body and its interactions with the environment. The sensorimotor theory of consciousness further argues that perceptual experience arises from mastery of sensorimotor contingencies. These frameworks challenge the idea that disembodied algorithms can achieve consciousness.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Embodied_cognition">Embodied cognition - Wikipedia</a></li>
<li><a href="http://www.scholarpedia.org/article/Sensorimotor_theory_of_consciousness">Sensorimotor theory of consciousness - Scholarpedia</a></li>

</ul>
</details>

**Discussion**: Commenters drew analogies with Star Trek's 'Measure of a Man' and compared AI consciousness to airplanes vs. birds, arguing that AI can think without being alive. Others highlighted that LLMs are immutable and do not learn from experience, casting doubt on their consciousness.

**Tags**: `#AI`, `#consciousness`, `#philosophy`, `#Ted Chiang`, `#artificial intelligence`

---

<a id="item-8"></a>
## [Uber Caps AI Coding Tool Usage to Control Costs](https://simonwillison.net/2026/Jun/3/uber-caps-usage/#atom-everything) ⭐️ 8.0/10

Uber has implemented a monthly spending cap of $1,500 per employee per AI coding tool after blowing its 2026 AI budget in just four months. The cap applies to agentic coding software such as Cursor and Anthropic's Claude Code. This move highlights the real cost of AI coding agents and sets a precedent for enterprise AI cost management. With the cap equating to roughly 11% of a median Uber engineer's compensation, it underscores the need for sustainable pricing models. The cap is per tool, not aggregate, meaning employees can spend $1,500 on each of multiple tools. Simon Willison notes his own token usage is about $1,000/month per provider, which currently costs him only $100 due to subsidized individual plans not available to large companies.

rss · Simon Willison · Jun 3, 12:01 · [Discussion](https://news.ycombinator.com/item?id=48383056)

**Background**: AI coding tools like Claude Code use token-based pricing where costs scale with usage. Agentic coding tools autonomously edit files and run commands, consuming many tokens per task. Uber's 2026 AI budget was set in 2025 before the explosion of such tools, leading to rapid overspending.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Discussion**: Commenters debated the true cost of engineers (fully-loaded vs. compensation), the sustainability of pricing given competition from China, and whether flash models suffice for most tasks. Some noted tokenmaxxing behavior where employees intentionally maximize usage.

**Tags**: `#AI`, `#cost management`, `#Uber`, `#Claude Code`, `#coding agents`

---

<a id="item-9"></a>
## [Mathematicians Warn as AI Rapidly Gains Ground](https://www.science.org/content/article/mathematicians-issue-warning-ai-rapidly-gains-ground) ⭐️ 8.0/10

A group of mathematicians has issued a public warning about the rapid advancement of artificial intelligence in mathematical research, raising concerns about reliability, attribution, and the role of human proof verification. This warning highlights growing tensions between AI's potential to accelerate mathematical discovery and the need to preserve rigorous standards of proof, potentially reshaping how research is conducted in the field. The warning appears in a discussion on Science magazine, accompanied by community comments noting that AI often produces 'dumb' errors humans would never make, and drawing parallels to earlier disruptions in art and writing.

hackernews · pseudolus · Jun 3, 10:05 · [Discussion](https://news.ycombinator.com/item?id=48382052)

**Background**: Mathematicians have traditionally relied on human intuition and rigorous proof verification. Recent advances in AI, particularly large language models, have shown ability to generate conjectures and even proofs, but their unreliability raises questions about trust and accountability in mathematical outputs.

**Discussion**: Commenters expressed mixed views: some noted the long tail of AI stupidity beside its impressive output, others saw parallels with artist and author complaints during early generative AI, and a few argued that AI may inadvertently democratize access to mathematics but at the cost of eroding proper attribution and human verification.

**Tags**: `#AI`, `#mathematics`, `#research`, `#ethics`, `#community discussion`

---

<a id="item-10"></a>
## [Memory Layout Optimization Deep Dive](https://fzakaria.com/2026/06/01/every-byte-matters) ⭐️ 8.0/10

The article 'Every Byte Matters' presents a detailed analysis of how array-of-structs (AoS) versus struct-of-arrays (SoA) data layouts impact memory usage and performance, with a focus on JVM-specific overheads like object headers. This analysis is significant because memory layout optimization is critical for high-performance applications, and the JVM's current support for such optimization is limited; upcoming improvements like Project Valhalla could reduce overhead, making Java more competitive with AOT-compiled languages. The author demonstrates that reading a single byte across 1 million monsters actually reads 1 million bytes due to memory layout, and discusses the cost of JVM object headers (currently 12 bytes, soon to be 8) and how Project Valhalla plans to eliminate headers in some cases.

hackernews · ingve · Jun 3, 11:04 · [Discussion](https://news.ycombinator.com/item?id=48382382)

**Background**: Data-oriented design is an optimization approach that focuses on CPU cache efficiency by organizing data structure layouts to match access patterns. Array-of-structs (AoS) stores all fields of an object contiguously, while struct-of-arrays (SoA) stores each field in separate arrays, often improving spatial locality when iterating over a subset of fields. In the JVM, every object has a header (e.g., 12 bytes) that adds overhead not present in languages like C or Rust.

<details><summary>References</summary>
<ul>
<li><a href="https://hdembinski.github.io/posts/struct_of_arrays_vs_arrays_of_structs.html">Which data structure is faster: array of structs or struct of arrays ?</a></li>
<li><a href="https://en.wikipedia.org/wiki/Data-oriented_design">Data - oriented design - Wikipedia</a></li>
<li><a href="https://www.javacodegeeks.com/2026/01/performance-engineering-for-java-jvm-tuning-and-optimization.html">Performance Engineering for Java: JVM Tuning and Optimization</a></li>

</ul>
</details>

**Discussion**: Commenters had mixed reactions: some pointed out that 'every byte matters' is misleading because the focus is on large-scale patterns, not individual bytes. Others provided valuable context about JVM evolution, such as the reduction of object header size and Project Valhalla's off-heap memory tools. A user with a background in embedded systems noted the trade-off between micro-optimization and development time.

**Tags**: `#memory optimization`, `#JVM`, `#data structures`, `#performance`, `#systems programming`

---

<a id="item-11"></a>
## [Tesla retroactively adds 'supervised' to FSD contracts](https://electrek.co/2026/06/03/tesla-retroactively-modified-fsd-contracts-supervised/) ⭐️ 8.0/10

Tesla has retroactively modified Full Self-Driving (FSD) purchase agreements signed between 2016 and early 2024 to include the word 'supervised,' which was absent from the original contracts. This retroactive change could have significant legal and ethical implications, as it alters the original promise of full autonomy and may undermine consumer trust in Tesla's autonomous driving claims. Multiple owners have confirmed the issue, and in some cases, the original documents have been made entirely inaccessible through Tesla's online portal.

rss · Electrek · Jun 3, 12:54

**Background**: Tesla's 'Full Self-Driving Capability' package was marketed as enabling full autonomy without driver supervision. The term 'supervised' implies that the driver must remain attentive and ready to take control, which is a significant downgrade from the original promise. Retroactively altering contracts raises concerns about contract law and consumer protection.

**Tags**: `#Tesla`, `#Full Self-Driving`, `#contracts`, `#autonomous vehicles`, `#legal`

---

<a id="item-12"></a>
## [PlayStation Hardware Deep-Dive Analysis](https://www.copetti.org/writings/consoles/playstation/) ⭐️ 7.0/10

Rodrigo Copetti published a comprehensive technical analysis of the original PlayStation's hardware architecture, covering the CPU, GPU, SPU, memory mapping, and more. This analysis provides invaluable insights for retro gaming enthusiasts, emulator developers, and systems engineers, helping them understand the unique design choices that made the PlayStation a 3D gaming milestone. The CPU is a modified MIPS R3000A running at 33.8688 MHz with 5 KB L1 cache, and the GPU uses an integer coordinate model with no fractional coordinates. The SPU supports ADPCM with up to 24 channels and 512 KB RAM.

hackernews · gregsadetsky · Jun 3, 10:24 · [Discussion](https://news.ycombinator.com/item?id=48382142)

**Background**: The original PlayStation, released in 1994, was a revolutionary 32-bit console that used a RISC CPU from MIPS and dedicated hardware for graphics and sound. Its architecture was critical for enabling real-time 3D rendering at an affordable price.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PlayStation_technical_specifications">PlayStation technical specifications - Wikipedia</a></li>
<li><a href="https://www.copetti.org/writings/consoles/playstation/">PlayStation Architecture | A Practical Analysis</a></li>
<li><a href="https://www.psdevwiki.com/ps1/SPU">SPU - PS1 Developer wiki</a></li>

</ul>
</details>

**Discussion**: Commenters praised the article's depth and clarity, with some noting it was originally published in 2019. A technical discussion emerged about creative memory mapping tricks used by Konami in Metal Gear Solid, and recommendations for PS1 emulators were shared.

**Tags**: `#PlayStation`, `#hardware architecture`, `#retro gaming`, `#systems design`

---

<a id="item-13"></a>
## [Meta allows workers 30-minute opt-out from tracking](https://www.bbc.com/news/articles/c93x0k194yno) ⭐️ 7.0/10

Meta has introduced a policy allowing employees to opt out of workplace tracking for up to 30 minutes at a time, following internal backlash against its keystroke and mouse movement monitoring program for AI training. This move reflects growing tensions between employee privacy and corporate surveillance in the tech industry, and sets a precedent for how companies might balance AI training needs with worker autonomy. The opt-out window is limited to 30 minutes at a time, and employees cannot completely avoid monitoring on company-issued devices; the tracking program was part of Meta's Model Capability Initiative (MCI) to train AI.

hackernews · reconnecting · Jun 3, 12:42 · [Discussion](https://news.ycombinator.com/item?id=48383220)

**Background**: Meta had been tracking employees' keystrokes, mouse movements, and even capturing screenshots to train its AI models, a program that sparked significant internal opposition. The company initially stated there was no opt-out option, but after widespread backlash, it scaled back the program and introduced this limited opt-out feature.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bbc.com/news/articles/c93x0k194yno">Meta scales back plan to track workers' clicks and ... - BBC</a></li>
<li><a href="https://www.cnbc.com/2026/04/22/meta-tracks-employee-usage-on-google-linkedin-ai-training-project.html">Meta is tracking employee keystrokes on Google, LinkedIn ...</a></li>
<li><a href="https://finance.yahoo.com/sectors/technology/articles/meta-scales-back-employee-tracking-122523464.html?fr=sycsrp_catchall">Meta scales back employee tracking program after backlash</a></li>

</ul>
</details>

**Discussion**: Comments ranged from literary references to Snow Crash drawing parallels to dystopian tracking, to personal reflections on tech work culture and the irony of a surveillance company tracking its own employees. Some questioned why employees stay at Meta given the toxic environment, while others noted that IT pros rarely discuss the extent of monitoring.

**Tags**: `#privacy`, `#workplace surveillance`, `#Meta`, `#employee monitoring`, `#tech culture`

---

<a id="item-14"></a>
## [Apple Doubles MacBook Neo Production Due to Demand](https://www.macrumors.com/2026/06/03/macbook-neo-production-doubled-says-kuo/) ⭐️ 7.0/10

Apple has doubled production of the MacBook Neo following overwhelming demand, as reported by analyst Ming-Chi Kuo. This reflects strong market performance and Apple's ecosystem advantages, making it harder for competitors to catch up in the premium laptop segment. Despite the production ramp, some users have expressed concerns over the base 8GB memory configuration, though the overall reception has been positive.

hackernews · tosh · Jun 3, 16:33 · [Discussion](https://news.ycombinator.com/item?id=48386238)

**Discussion**: Commenters praise the MacBook Neo for its ecosystem ease and cost efficiency, with many noting that competitors struggle to match Apple's build quality and performance. Some users mention initial hesitation about 8GB RAM but find it sufficient for their needs.

**Tags**: `#Apple`, `#MacBook`, `#hardware`, `#business`, `#consumer tech`

---

<a id="item-15"></a>
## [Caterpillar BEPU: Plug-and-play electric engine swap](https://electrek.co/2026/06/03/caterpillar-bepu-makes-going-electric-as-easy-as-swapping-an-engine/) ⭐️ 7.0/10

Caterpillar announced the Battery Electric Power Unit (BEPU) in June 2026, a plug-and-play unit that fits into the same space and mounts as a diesel engine, enabling easy retrofitting of heavy machinery to electric power. The BEPU simplifies the electrification of heavy machinery by offering a direct retrofit option, reducing cost and downtime, which could accelerate adoption of electric power in industries like construction and mining. The integrated unit includes all powertrain components—battery, motor, inverter, onboard charging, cooling, and controls—and Doppstadt has already selected it for a zero-emission separator machine showcased at IFAT 2026.

rss · Electrek · Jun 3, 12:47

**Background**: Heavy machinery traditionally relies on diesel engines, and retrofitting to electric is complex due to space and integration challenges. Caterpillar's BEPU is designed as a drop-in replacement, maintaining compatibility with existing engine mounts and cooling systems. This approach allows OEMs to offer electric versions without redesigning their machines.

<details><summary>References</summary>
<ul>
<li><a href="https://electrek.co/2026/06/03/caterpillar-bepu-makes-going-electric-as-easy-as-swapping-an-engine/">Caterpillar BEPU makes going electric as easy as swapping an ...</a></li>
<li><a href="https://www.equipmentjournal.com/tech-news/doppstadt-selects-cats-bepu-as-alternative-to-diesel/">Doppstadt select’s Cat’s BEPU as alternative to diesel</a></li>
<li><a href="https://www.canadianminingjournal.com/news/caterpillars-electric-power-unit-powers-new-zero-emission-separator-at-ifat-2026/">Caterpillar’s electric power unit powers new zero-emission ...</a></li>

</ul>
</details>

**Tags**: `#electric vehicles`, `#heavy machinery`, `#retrofit`, `#battery technology`, `#sustainability`

---

<a id="item-16"></a>
## [Visual Studio Code 1.123 Released with Enhancements](https://github.com/microsoft/vscode/releases/tag/1.123) ⭐️ 6.0/10

Microsoft released Visual Studio Code version 1.123, which includes incremental updates and bug fixes to improve the editor's stability and performance. Even routine updates are important for developers who rely on VS Code daily for coding, as they ensure a smooth and secure development environment. The release includes various improvements across the editor, such as enhanced language support and refined user interface elements.

github · ulugbekna · Jun 3, 14:36

**Background**: Visual Studio Code is a free, open-source code editor developed by Microsoft, widely used for web development and other programming tasks. Regular monthly updates introduce new features, bug fixes, and performance improvements.

**Tags**: `#vscode`, `#release`, `#editor`, `#development`

---

<a id="item-17"></a>
## [SEG Solar Announces Third Texas Factory](https://electrek.co/2026/06/03/another-giant-solar-factory-is-coming-to-texas/) ⭐️ 6.0/10

SEG Solar announced plans to build a third solar module factory in the Houston, Texas area, further expanding its US manufacturing capacity. This expansion signals growing domestic solar manufacturing, which reduces reliance on imports and strengthens the US renewable energy supply chain. The new factory is in addition to SEG Solar's two existing US facilities, though specific capacity and timeline details were not disclosed in the announcement.

rss · Electrek · Jun 3, 22:55

**Background**: Solar module manufacturing in the US has been growing due to policy incentives like the Inflation Reduction Act and tariffs on imported panels. Texas has become a hub for solar factories due to its business-friendly environment and access to renewable energy resources.

**Tags**: `#solar energy`, `#manufacturing`, `#Texas`, `#renewables`, `#SEG Solar`

---

<a id="item-18"></a>
## [Tesla expands Robotaxi to all Austin metro but fleet still tiny](https://electrek.co/2026/06/03/tesla-robotaxi-expands-entire-austin-metro-only-20-vehicles/) ⭐️ 6.0/10

Tesla announced its unsupervised Robotaxi service now covers the entire Austin metro area, but the active fleet remains at only about 20 vehicles, a number that has been shrinking. This expansion is a notable milestone for Tesla's autonomous driving ambitions, but the tiny and shrinking fleet undermines the service's viability and raises questions about the company's ability to scale its robotaxi operations. The geofenced area now covers the entire Austin metro, but the fleet size of approximately 20 unsupervised vehicles is far smaller than needed for meaningful coverage, and recent data shows the fleet has been shrinking rather than growing.

rss · Electrek · Jun 3, 17:14

**Background**: A 'geofenced operating zone' is a virtual boundary that defines where an autonomous vehicle can operate; Tesla's Robotaxi service uses such zones to limit service areas. 'Unsupervised autonomous vehicles' refer to Level 4 or Level 5 systems that can drive without human intervention under specific conditions. Tesla's Robotaxi fleet in Austin is one of the first commercial deployments of unsupervised autonomy, but its small size contrasts with Musk's ambitious predictions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Geofence">Geofence - Wikipedia</a></li>
<li><a href="https://legalclarity.org/what-is-a-geofencing-restriction-and-how-does-it-work/">What Is a Geofencing Restriction and How Does It Work?</a></li>
<li><a href="https://www.teslaacessories.com/blogs/news/the-dawn-of-unsupervised-autonomy-—-inside-tesla's-fsd-v14-rollout-in-austin-and-palo-alto">The Dawn of Unsupervised Autonomy — Inside Tesla's FSD v14...</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#Robotaxi`, `#autonomous vehicles`, `#Austin`, `#fleet`

---