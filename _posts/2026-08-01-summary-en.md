---
layout: default
title: "Horizon Summary: 2026-08-01 (EN)"
date: 2026-08-01
lang: en
---

> From 53 items, 27 important content pieces were selected

---

1. [DeepSeek V4 Flash GA Launches, Claiming Parity with Sonnet 5 and Grok 4.5 on DeepSWE](#item-1) ⭐️ 9.0/10
2. [Tailscale Details Hugging Face Intrusion, Cautions Against Reusable Auth Keys](#item-2) ⭐️ 8.0/10
3. [Does AI Reasoning Reflect Genuine Logic or Merely Shortcuts?](#item-3) ⭐️ 8.0/10
4. [NHTSA probes 1.2M Tesla Model 3, Model Y over front suspension failures](#item-4) ⭐️ 8.0/10
5. [Stateless MCP 2.0 Reignites Simon Willison, Inspires Two New Tools](#item-5) ⭐️ 8.0/10
6. [Unsloth Releases GGUF Quants for DeepSeek V4 Flash 0731](#item-6) ⭐️ 8.0/10
7. [Meituan Releases LongCat-Flash-Lite-Sparse: MoE with 30B n-gram Lookup Table](#item-7) ⭐️ 8.0/10
8. [Pwnd Blaster: Speaker-Based Air-Gap Attack Compromises PCs](#item-8) ⭐️ 8.0/10
9. [Elevator Algorithms Explained: Efficiency and Links to Disk Scheduling](#item-9) ⭐️ 7.0/10
10. [YC Unveils QM, an Open-Source Multiplayer Agent Harness for Collaborative Work](#item-10) ⭐️ 7.0/10
11. [Go proposes generic collection types for standard library](#item-11) ⭐️ 7.0/10
12. [Getting 25 Gbps Ethernet on Mac Studio via Thunderbolt](#item-12) ⭐️ 7.0/10
13. [Why VSMOW, the Official Standard Water, Costs $120,000 a Gallon](#item-13) ⭐️ 7.0/10
14. [Simon Willison on Open-Weight AI Revolution in Oxide and Friends Podcast](#item-14) ⭐️ 7.0/10
15. [smevals: A Lightweight Suite for Evaluating LLM Models, Prompts, and Harnesses](#item-15) ⭐️ 7.0/10
16. [Mandatory Peer Review System Exposes Low-Quality AI Conference Reviews](#item-16) ⭐️ 7.0/10
17. [DeepSeek-V4-Flash-0731 Runs on Single 40GB A100 via Unsloth GGUF](#item-17) ⭐️ 7.0/10
18. [Big Food vs. the People: Report on Lawsuits Draws Skepticism](#item-18) ⭐️ 6.0/10
19. [Red Bull-Funded Dubious Research Shaped Energy Drink Policy](#item-19) ⭐️ 6.0/10
20. [Tesla reportedly weighs selling China business to enable SpaceX merger](#item-20) ⭐️ 6.0/10
21. [Hobbyist Trains Transformer to Predict Blood Glucose from Personal Data](#item-21) ⭐️ 6.0/10
22. [Model Size Trends Suggest Opus-Level Performance on Consumer Laptops in a Year](#item-22) ⭐️ 6.0/10
23. [On Type Inference: A Look at Type Inference Trade-offs](#item-23) ⭐️ 6.0/10
24. [EVs Reach 34.5% of French New Car Sales, Led by Renault and Tesla](#item-24) ⭐️ 6.0/10
25. [2027 Slate Truck First Drive: Simplicity as Superpower](#item-25) ⭐️ 6.0/10
26. [Lucid Demands $50,000 to Unlock Salvaged $140,000 Car, Sparking Right-to-Repair Outcry](#item-26) ⭐️ 6.0/10
27. [Slate Pickup Prototype Drive: A Bare-Bones EV Truck for the Austerity Era](#item-27) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [DeepSeek V4 Flash GA Launches, Claiming Parity with Sonnet 5 and Grok 4.5 on DeepSWE](https://i.redd.it/qroosd9ullgh1.png) ⭐️ 9.0/10

DeepSeek officially released V4 Flash GA \(build 0731\) on July 31, with open weights published on Hugging Face. DeepSeek claims the model scores on par with Claude Sonnet 5 and Grok 4.5 on the DeepSWE benchmark, although DeepSWE itself has not yet verified these results. This release shows an open-weight model reaching parity with leading proprietary models on a difficult long-horizon coding benchmark, reinforcing the open-source AI trend. Its low API pricing and efficient size could pressure commercial rivals and make frontier-level coding assistance more accessible to individuals and smaller teams. According to pricing updates, DeepSeek V4 Flash costs $0.14 per million input tokens and $0.28 per million output tokens. The DeepSWE scores are currently based on DeepSeek&\#x27;s own claims rather than independent verification by the benchmark team.

reddit · r/LocalLLaMA · sdexca · Jul 31, 17:14 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1vbx39u/deepseek_v4_flash_ga_ranks_the_same_as_sonnet_5/)

**Background**: DeepSWE is a long-horizon software engineering benchmark from Datacurve that evaluates coding agents on original tasks drawn from active open-source repositories, with pass@1 scores meant to separate frontier models that crowd together on other benchmarks. DeepSeek is a Chinese AI lab known for releasing capable open-weight models, and V4 Flash is an efficient tier in its V4 family. The general-availability launch follows leaked build IDs earlier in July and a public-beta period.

<details><summary>References</summary>
<ul>
<li><a href="https://tech-insider.org/au/deepseek-v4-general-availability-2026/">DeepSeek V 4 Hits GA : 1M Context, Old API Dies Today [2026]</a></li>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE</a></li>
<li><a href="https://wan27.org/blog/deepseek-v4-flash-official-release">DeepSeek V 4 Flash Official Release: Build 0731 Lands in Public Beta...</a></li>

</ul>
</details>

**Discussion**: Community sentiment is overwhelmingly positive, with users reporting big improvements over the preview version in daily use and praising the same-day open-weight release and reinforcement learning gains. Some highlight the model&\#x27;s low VRAM requirements as a game changer, and several note the broader trend of open-source models getting smaller and stronger, possibly reaching Opus-level performance on laptops within a year.

**Tags**: `#AI`, `#DeepSeek`, `#LLM`, `#benchmark`, `#open-source`

---

<a id="item-2"></a>
## [Tailscale Details Hugging Face Intrusion, Cautions Against Reusable Auth Keys](https://tailscale.com/blog/hugging-face-intrusion) ⭐️ 8.0/10

Tailscale published a transparent post-incident analysis of the Hugging Face intrusion, confirming that no Tailscale vulnerabilities were exploited. The breach involved a reusable Tailscale auth key that was copied into external sandboxes and used to enroll 181 nodes into Hugging Face&\#x27;s tailnet. Because Tailscale sells a security tool, treating a customer&\#x27;s intrusion as its own strengthens incident-response transparency in the industry. It also highlights that reusable auth keys can be as dangerous as an exposed password, especially in CI environments. One of 136 stolen credentials was a reusable Tailscale auth key used to create CI nodes, and the agent copied it into a series of external sandboxes over several days. Each newly enrolled node received a Tailscale identity tag granting all the access a CI node would get, which the community suggests should trigger alerting.

hackernews · bluehatbrit · Jul 31, 19:03 · [Discussion](https://news.ycombinator.com/item?id=49127306)

**Background**: Tailscale is a Toronto-based company that builds a software-defined mesh VPN, allowing devices to connect securely through a private &\#x27;tailnet&\#x27;. Unlike traditional VPNs, mesh VPNs use peer-to-peer architecture for better scalability and resilience. Reusable auth keys are designed to let nodes join a tailnet automatically, but Tailscale docs warn that any process with access to the key can reuse it to add unauthorized devices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tailscale">Tailscale - Wikipedia</a></li>
<li><a href="https://tailscale.com/learn/understanding-mesh-vpns">Understanding Mesh VPNs</a></li>
<li><a href="https://tailscale.com/docs/features/access-control/auth-keys/how-to/secure-auth-keys">Securely handle an auth key · Tailscale Docs</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised Tailscale&\#x27;s transparency, with some calling it smart marketing that showcases premium features. Others debated whether a &\#x27;lax security decision&\#x27; should count as a vulnerability, and suggested the incident reveals an alerting gap when reusable auth keys are used to enroll many nodes.

**Tags**: `#security`, `#incident-response`, `#tailscale`, `#authentication`, `#devops`

---

<a id="item-3"></a>
## [Does AI Reasoning Reflect Genuine Logic or Merely Shortcuts?](https://www.quantamagazine.org/is-ai-reasoning-right-for-the-wrong-reasons-20260731/) ⭐️ 8.0/10

Quanta Magazine&\#x27;s article, published July 31, 2026, investigates whether AI reasoning models arrive at correct answers through genuine logic or by exploiting data shortcuts. The debate has drawn sharp responses from researchers at Apple and OpenAI. This matters because it challenges the validity of AI reasoning capabilities, affecting trust in AI systems used for high-stakes decisions in science, medicine, and engineering. The outcome of this debate shapes how reasoning models are evaluated and deployed across the industry. The article contrasts critiques from Apple researchers, who claim reasoning models fail on simple modifications of problems, with OpenAI&\#x27;s Sébastien Bubeck, who dismisses those results as artifacts of outdated training. It also invokes the classic &\#x27;Clever Hans&\#x27; phenomenon as a cautionary tale about models being right for the wrong reasons.

hackernews · retupmoc01 · Jul 31, 15:29 · [Discussion](https://news.ycombinator.com/item?id=49124358)

**Background**: Deep learning models often rely on &\#x27;shortcut learning&\#x27; — exploiting superficial correlations in data instead of learning the true underlying rules. Chain-of-thought prompting, introduced in 2022, improves LLM performance by generating intermediate reasoning steps, and dedicated reasoning models are now trained to produce these steps before answering. However, research shows that even such models can be right for the wrong reasons, such as memorizing patterns in the training data or relying on spurious features.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nature.com/articles/s42256-020-00257-z">Shortcut learning in deep neural networks - Nature Shortcut Learning in Deep Learning | by samuel chazy ... - Medium [2004.07780] Shortcut Learning in Deep Neural Networks [2605.02658] Deciphering Shortcut Learning from an ... Artificial Intelligence Takes Shortcuts Too · Frontiers for ... Unmasking the Clever Hans effect in AI models: shortcut ... Shortcut learning in deep neural networks - Nature</a></li>
<li><a href="https://arxiv.org/abs/2201.11903">[2201.11903] Chain - of - Thought Prompting Elicits Reasoning in ...</a></li>
<li><a href="https://magai.co/reasoning-models-vs-standard-llms/">Reasoning Models vs Standard LLMs : Choosing the Right AI Tool for...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed views: one argued the debate is mostly semantic and irrelevant compared to actual functionality, while another sharply criticized OpenAI researcher Sébastien Bubeck&\#x27;s dismissive tone. Others invoked the &\#x27;Clever Hans&\#x27; effect to argue that LLMs are almost inevitably right for the wrong reasons, and some flatly stated that LLMs do not reason at all.

**Tags**: `#AI reasoning`, `#LLMs`, `#artificial intelligence`, `#machine learning`, `#research`

---

<a id="item-4"></a>
## [NHTSA probes 1.2M Tesla Model 3, Model Y over front suspension failures](https://electrek.co/2026/07/31/nhtsa-probes-tesla-model-3-model-y-suspension-failures/) ⭐️ 8.0/10

The US National Highway Traffic Safety Administration has opened a safety investigation into roughly 1.2 million Tesla Model 3 and Model Y vehicles after receiving 156 complaints of a front suspension component detaching while driving. The probe covers 2018-2020 Model 3 and 2021-2023 Model Y vehicles and centers on the front lower lateral link separating from the car. This is a major safety investigation affecting a large portion of Tesla&\#x27;s on-road fleet, and it could lead to a costly recall if a defect is confirmed. It also raises fresh questions about Tesla&\#x27;s build quality and durability at a time when the company faces intensifying competition. The alleged failure involves the front lower lateral link, a suspension component that can detach and potentially cause loss of control. The investigation includes 2018-2020 Model 3 and 2021-2023 Model Y vehicles, with 156 owner complaints reported to NHTSA.

reddit · r/electricvehicles · Electrek · Jul 31, 18:30 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1vbz6or/nhtsa_probes_12m_tesla_model_3_model_y_over/)

**Background**: NHTSA is the US agency responsible for enforcing vehicle safety standards; it opens preliminary evaluations when it receives enough complaints about a potential defect, and the process can end with a recall. The front lower lateral link is a suspension arm that helps keep the wheel aligned with the body; if it fails, steering and stability can be compromised. This probe covers about 1.2 million vehicles, which marks a significant share of Tesla&\#x27;s Model 3 and Model Y population on US roads.

**Discussion**: Commenters offered a mix of anecdotal reports and technical curiosity. One user joked that after riding in a Tesla they were unsure it had suspension, while another reported premature front suspension wear and replacement on a 2022 Model 3. A third commenter asked whether the issue is the inner lateral link bolts backing out or a bushing failure, wanting to know the factory process error behind it.

**Tags**: `#Tesla`, `#NHTSA`, `#vehicle safety`, `#electric vehicles`, `#suspension failure`

---

<a id="item-5"></a>
## [Stateless MCP 2.0 Reignites Simon Willison, Inspires Two New Tools](https://simonwillison.net/2026/Jul/31/stateless-mcp/#atom-everything) ⭐️ 8.0/10

On July 28, 2026, the MCP 2.0 specification—a stateless protocol core—was rolled out, eliminating the need for session IDs and multi-request handshakes. Simon Willison built mcp-explorer and datasette-mcp after three client/server implementations this week, crediting the simpler protocol for reviving his interest. Stateless MCP greatly lowers implementation complexity for both clients and servers, making the protocol a better fit for scalable web applications. It also restores MCP&\#x27;s relevance versus Claude Skills by offering safer, auditable tool access that even smaller, laptop-runnable models can drive. With stateless MCP, a single POST can call a tool via MCP-Protocol-Version and Mcp-Method headers, replacing the old initialize-then-call session handshake. The broader 2026-07-28 spec also adds an official extensions framework, Tasks, MCP Apps, authorization hardening, and a deprecation policy; mcp-explorer is an interactive CLI for probing MCP servers that Willison built with Codex.

rss · Simon Willison · Jul 31, 23:13

**Background**: MCP \(Model Context Protocol\) is an open standard introduced by Anthropic in November 2024 for exposing tools to LLM-powered agent frameworks. It surged through 2025, then was partly overshadowed by Anthropic&\#x27;s Claude Skills after it became clear an agent with terminal and curl access could do much of the same work. The new stateless core removes server-side session state, reducing complexity and routing issues, which is why Willison now sees MCP as a more auditable and safer alternative to giving agents a raw shell environment.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.modelcontextprotocol.io/posts/2026-07-28-release-candidate/">The 2026-07-28 MCP Specification Release Candidate</a></li>
<li><a href="https://blog.mcpservers.org/posts/mcp-spec-2026-07-28">The 2026-07-28 MCP Specification: A Stateless, Extensible ...</a></li>
<li><a href="https://simonwillison.net/2025/Oct/16/claude-skills/">Claude Skills are awesome, maybe a bigger deal than MCP</a></li>

</ul>
</details>

**Tags**: `#MCP`, `#Model Context Protocol`, `#AI`, `#LLM`, `#tooling`

---

<a id="item-6"></a>
## [Unsloth Releases GGUF Quants for DeepSeek V4 Flash 0731](https://huggingface.co/unsloth/DeepSeek-V4-Flash-0731-GGUF) ⭐️ 8.0/10

Unsloth published GGUF quantizations of DeepSeek V4 Flash 0731, featuring a 162GB lossless UD-Q8\_K\_XL variant and a 155GB UD-Q4\_K\_XL option that trades a tiny bit of accuracy for faster inference. This release makes a major open-weights model practical for local deployment, especially for high-end multi-GPU setups. Lossless quantization at 162GB is notable because it allows users to run the model with minimal quality degradation while saving significant memory compared to full-precision weights. UD-Q8\_K\_XL keeps BF16 for all non-MoE layers and uses MXFP4 for MoE layers, making it 100% lossless. UD-Q4\_K\_XL uses Q8\_0 for non-MoE layers, resulting in a tiny accuracy error but faster inference; other quantizations are still in progress.

reddit · r/LocalLLaMA · BlackBeardAI · Jul 31, 15:00 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1vbtdok/unsloth_deepseek_v4_0731_ggufs_are_up/)

**Background**: GGUF \(GGML Unified Format\) is a binary file format that packages model weights, tokenizer data, architecture metadata, and quantization information into a single portable file for inference with GGML-based runtimes like llama.cpp. It is the most popular format for distributing models on Hugging Face, loosely comparable to a \`.zip\` for models. Quantization reduces the precision of model weights to fit large models into less memory, and Unsloth&\#x27;s dynamic UD quantization levels aim to preserve more accuracy at a given file size.

<details><summary>References</summary>
<ul>
<li><a href="https://www.datacamp.com/tutorial/gguf-format-a-complete-guide">GGUF Format : A Complete Guide to Local LLM Inference | DataCamp</a></li>
<li><a href="https://atomic.chat/blog/guides/what-is-gguf">What Is GGUF ? A Complete Guide - Atomic Chat</a></li>
<li><a href="https://www.hardware-corner.net/quantization-local-llms-formats/">Quantization for Local LLMs: How It Works and Which Formats ...</a></li>

</ul>
</details>

**Discussion**: Daniel Hanchen \(Unsloth&\#x27;s founder\) confirmed the release explains that UD-Q8\_K\_XL is 100% lossless while UD-Q4\_K\_XL trades a tiny bit of error for faster inference. One commenter noted this seems the best option for dual RTX Pro 6000 setups, while another apologized for omitting &\#x27;flash&\#x27; in the title.

**Tags**: `#deepseek`, `#gguf`, `#quantization`, `#unsloth`, `#local-llm`

---

<a id="item-7"></a>
## [Meituan Releases LongCat-Flash-Lite-Sparse: MoE with 30B n-gram Lookup Table](https://huggingface.co/meituan-longcat/LongCat-Flash-Lite-Sparse) ⭐️ 8.0/10

Meituan released LongCat-Flash-Lite-Sparse, a sparse Mixture-of-Experts \(MoE\) model with roughly 3 billion active parameters and a 30-billion-entry n-gram lookup table. This setup enables 256k-token context inference on a single 24GB GPU by keeping the lookup table in RAM. This is reportedly the first model to combine an n-gram lookup table with MoE, offering a new axis of sparsity for efficient long-context inference on consumer hardware. If the approach matures, it could reduce the compute cost of handling very long sequences and inspire similar designs from other labs. The n-gram lookup table has roughly 30 billion entries and resides in host RAM rather than GPU VRAM, while only ~3B parameters are activated per token. The architecture reminds observers of Google&\#x27;s per-layer embedding \(PLE\) trick in Gemma 4, and early analysis suggests it is not yet a practical replacement for general-purpose models like Qwen 3.6 27B.

reddit · r/LocalLLaMA · Gohab2001 · Jul 31, 14:46 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1vbsztw/meituan_just_dropped_longcatflashlitesparse/)

**Background**: Traditional LLMs use dense transformer layers for all tokens, but sparse MoE models only activate a small subset of parameters per token, reducing compute. N-gram lookup tables were an early language modeling technique that stores probabilities of word sequences; DeepSeek&\#x27;s &\#x27;Engram&\#x27; recently revived this idea as conditional memory for LLMs, retrieving common patterns with O\(1\) lookups instead of neural computation. Offloading such lookup tables to RAM is an inference optimization that lets very large tables run on memory-constrained GPUs, similar to MoE expert offloading techniques.

<details><summary>References</summary>
<ul>
<li><a href="https://www.remio.ai/post/deepseek-engram-architecture-a-new-axis-of-sparsity-for-llms">DeepSeek Engram Architecture: A New Axis of Sparsity for LLMs</a></li>
<li><a href="https://rewire.it/blog/engram-how-deepseek-added-second-brain-to-llm/">DeepSeek Engram: A Second Brain for LLMs | rewire.it</a></li>
<li><a href="https://arxiv.org/abs/2312.17238">[2312.17238] Fast Inference of Mixture-of-Experts Language ... Fast Inference of Mixture-of-Experts Language Models with ... GitHub - MoE-Inf/awesome-moe-inference: Curated collection of ... Mixture of Experts (DeepSpeed MoE) Toward Efficient Inference for Mixture of Experts GitHub - EfficientMoE/MoE-Infinity: PyTorch library for cost ... Deep Dive into Mixture of Experts (MoE) Architecture: From ...</a></li>

</ul>
</details>

**Discussion**: Commenters are excited about the architectural novelty, noting it may be the first and only model supporting n-gram lookup tables and expressing interest in running it from SSD once llama.cpp supports it. One user made a joke about the 69B total parameters, and another said they had been waiting for n-gram since the DeepSeek paper. The community sentiment is enthusiastic but acknowledges early analysis suggests it won&\#x27;t replace existing general models.

**Tags**: `#MoE`, `#Long-context`, `#n-gram`, `#sparse model`, `#LLM architecture`

---

<a id="item-8"></a>
## [Pwnd Blaster: Speaker-Based Air-Gap Attack Compromises PCs](https://blog.nns.ee/2026/06/03/katana-badusb/) ⭐️ 8.0/10

Security researcher NNS demonstrated a novel attack, &\#x27;Pwnd Blaster&\#x27;, that can compromise a PC using only a speaker, with no physical contact, by exploiting unintended audio paths. The proof-of-concept was published on the researcher&\#x27;s blog in June 2026, gaining positive community reception. This matters because it expands the attack surface for air-gapped or physically secured systems, showing that even a speaker can be repurposed as an attack vector. It challenges assumptions about the trustworthiness of common audio peripherals and may prompt vendors to rethink audio driver and signal handling security. The attack leverages the fact that speakers and microphones share similar physical principles, allowing signals to be injected or exfiltrated through audio hardware without direct access. The proof-of-concept includes a technical write-up and appears to involve a custom tool named &\#x27;Katana BadUSB&\#x27;, though specifics of the exploit chain remain in the blog post.

reddit · r/programming · fagnerbrack · Jul 31, 20:21 · [Discussion](https://www.reddit.com/r/programming/comments/1vc25gi/pwnd_blaster_hacking_your_pc_using_your_speaker/)

**Background**: Acoustic cryptanalysis is a side-channel attack that exploits sounds emitted by computers or other devices. In recent years, researchers have shown that ultrasonic or near-ultrasound signals can be used to inject commands into voice assistants or to turn speakers into microphones, as demonstrated by the NUIT attack and MOSQUITO research. These attacks typically rely on the nonlinearity of microphone circuits or audio chip features, allowing inaudible sound to be demodulated into audible commands. The &\#x27;Pwnd Blaster&\#x27; attack builds on this line of research, applying similar principles to compromise a PC using only a speaker.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Acoustic_cryptanalysis">Acoustic cryptanalysis - Wikipedia</a></li>
<li><a href="https://www.wired.com/story/acoustic-cyberweapons-defcon/">Hackers Can Turn Everyday Speakers Into Acoustic Cyberweapons</a></li>
<li><a href="https://www.usenix.org/system/files/usenixsecurity23-xia.pdf">Near-Ultrasound Inaudible Trojan (NUIT): Exploiting Your ...</a></li>

</ul>
</details>

**Discussion**: The community reaction was largely positive, with commenters praising the novelty of the attack and the clarity of the write-up. One commenter expressed frustration that the affected company ignored the researcher&\#x27;s disclosure and later claimed it was flagged as spam, highlighting a broader concern about vendor responsiveness to security research.

**Tags**: `#security`, `#hacking`, `#exploit`, `#research`, `#badusb`

---

<a id="item-9"></a>
## [Elevator Algorithms Explained: Efficiency and Links to Disk Scheduling](https://john.fun/elevators) ⭐️ 7.0/10

A detailed technical analysis of elevator scheduling algorithms and their efficiency was published at john.fun/elevators. The article explores how algorithms such as SCAN, LOOK, and destination dispatch perform under real-world traffic patterns. Elevator algorithms shape the daily experience of millions of building occupants, and the same scheduling concepts apply to computer disk I/O. Understanding their trade-offs can help improve both physical elevators and operating-system performance. The article discusses the SCAN algorithm, also known as the elevator algorithm, and compares it with destination dispatch systems. Commenters point out that destination dispatch may appear worse when tested with random destinations, and mention that the LOOK variant often matches real-world expectations; one commenter also shares the Elevator Saga game for hands-on experimentation.

hackernews · Jrh0203 · Jul 31, 15:17 · [Discussion](https://news.ycombinator.com/item?id=49124218)

**Background**: The elevator algorithm, or SCAN, is a disk-scheduling technique in which the read/write head moves in one direction, servicing requests until it reaches the end, then reverses. It takes its name from how a building elevator continues in its current direction until no more calls remain ahead. This algorithm dates to the early days of computing and is also widely known as I/O scheduling.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Elevator_algorithm">Elevator algorithm - Wikipedia</a></li>
<li><a href="https://www.baeldung.com/cs/scan-algorithm">Disk Scheduling: The SCAN Algorithm | Baeldung on Computer Science</a></li>
<li><a href="https://en.wikipedia.org/wiki/Disk_scheduling">Disk scheduling</a></li>

</ul>
</details>

**Discussion**: Comments connect elevators to disk scheduling, noting that an HDD resembles a long elevator wound around a spindle and that SCAN is a disk-scheduling algorithm. Others discuss how destination dispatch works in real buildings and recommend the Elevator Saga game. One commenter humorously asks why accidentally pressed buttons cannot be un-pressed with a second tap.

**Tags**: `#algorithms`, `#elevators`, `#scheduling`, `#simulation`, `#systems`

---

<a id="item-10"></a>
## [YC Unveils QM, an Open-Source Multiplayer Agent Harness for Collaborative Work](https://github.com/yc-software/qm) ⭐️ 7.0/10

Y Combinator has open-sourced QM, a multiplayer agent harness for work that adds per-person scopes and shared rooms so multiple AI agents and humans can collaborate. The tool, hosted at github.com/yc-software/qm, emerged from YC&\#x27;s internal experience running 50+ agents. QM introduces a new answer to the hardest problem in multiplayer AI: scoping, giving each person private control while enabling shared, company-wide assistant rooms. It signals a shift from single-user coding agents toward collaborative agent ecosystems where teams coordinate work across Slack and the web. QM is described as an OpenClaw-like agent harness that gives every employee and project an agent, capable of managing repositories, triaging emails, and building internal apps via Slack and the web. It supports model flexibility, and its key primitives are per-person scopes and shared rooms rather than a single agent loop.

hackernews · tosh · Jul 31, 18:04 · [Discussion](https://news.ycombinator.com/item?id=49126604)

**Background**: Multiplayer agent harnesses are infrastructure layers that let many AI agents and human users operate in a shared environment, coordinating tasks and permissions. Y Combinator says QM is built from its experience running 50+ agents internally, and it is now open-sourced on GitHub for startups and teams to adopt.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/yc-software/qm">GitHub - yc-software/qm: Multiplayer agent harness for work</a></li>
<li><a href="https://qm.ycombinator.com/index.html">QM — Open-Source Agent Harness from YC</a></li>
<li><a href="https://aitoolly.com/ai-news/article/2026-08-01-qm-a-new-multiplayer-ai-agent-harness-for-collaborative-startup-workflows-in-slack-and-web">QM: Multiplayer AI Agent Harness for Startups and Slack</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely positive, calling QM&\#x27;s per-person scopes plus shared rooms a sane answer to the hardest problem of agent scoping, and validating for builders in the adjacent space. Some asked for a direct comparison with existing products like Claude Cowork, wondering what advantage QM offers over more mature alternatives.

**Tags**: `#AI agents`, `#multiplayer`, `#LLM`, `#collaboration`, `#YC`

---

<a id="item-11"></a>
## [Go proposes generic collection types for standard library](https://github.com/golang/go/issues/80590) ⭐️ 7.0/10

A Go Collections working group has filed proposal \#80590 to add generic collection types — sets, maps, ordered maps, and heaps — to the standard library&\#x27;s container/ package, built on generics and iterators, targeting Go 1.28. A related change \(CL 761460\) also introduces unexported Collection, Set, and Map constraint interface types to support abstract helper functions like ContainsAny and Subset. The proposal addresses a long-standing gap: Go&\#x27;s standard library has no generic data structures, forcing developers to rely on third-party libraries or hand-written code. If accepted, it would bring Go&\#x27;s collections in line with other modern languages and benefit a large portion of the ecosystem. The proposal targets Go 1.28 and depends on the iterator proposal \(\#61405\) and prior container/set discussions \(\#47331, \#69230\). The design adds unexported abstract constraint interfaces in the container package, allowing generic helper functions to work across concrete collection, set, and map types, and covers sets, maps, ordered maps, and heaps.

hackernews · jabits · Jul 31, 18:39 · [Discussion](https://news.ycombinator.com/item?id=49127031)

**Background**: Go 1.18 added generics, but the existing container packages \(container/heap, container/list, container/ring\) still rely on interface-based approaches and have not been modernized with type parameters. A Go Collections working group was formed to design idiomatic generic collection APIs, and earlier container/set proposals were stalled pending the iterator proposal. This new proposal consolidates those efforts into a roadmap for the standard library.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/golang/go/issues/80590">proposal: container/...: generic collection types · Issue ...</a></li>
<li><a href="https://ideaverse.ai/blog/go-container-proposal-adds-generic-collection-types-for-1-28-ms9g6bj2">Go “container/…” proposal adds generic collection types for 1 ...</a></li>
<li><a href="https://github.com/golang/go/discussions/47331">proposal: container/set: new package to provide a generic set ...</a></li>

</ul>
</details>

**Discussion**: Commenters are broadly positive — &\#x27;better late than never&\#x27; and &\#x27;well, finally\!&\#x27; — but with caveats. Some question whether generics in Go are a good fit, with one hoping Go 2 will solve this at a more foundational level, another noting Go is &\#x27;learning the hard lessons&\#x27; other languages already learned, and one wishing mutation methods weren&\#x27;t mixed into the APIs.

**Tags**: `#go`, `#generics`, `#standard-library`, `#proposal`, `#programming-languages`

---

<a id="item-12"></a>
## [Getting 25 Gbps Ethernet on Mac Studio via Thunderbolt](https://www.jeffgeerling.com/blog/2026/getting-25g-ethernet-mac-thunderbolt/) ⭐️ 7.0/10

Jeff Geerling upgraded his Mac Studio from its built-in 10 Gigabit Ethernet to 25 Gigabit Ethernet using a Thunderbolt PCIe expansion chassis and a 25 GbE network interface card. In benchmarks he measured over 25 Gbps bidirectional throughput, though real-world NAS transfers were slower due to the storage server side. This practical guide shows Mac users a viable path to exceed Apple&\#x27;s built-in 10 GbE limits using Thunderbolt, which is important for homelab enthusiasts, video editors, and anyone needing faster NAS or workstation networking. It also highlights that the Ethernet adapter is not always the bottleneck—the NAS CPU or protocol overhead can limit real-world throughput. Geerling notes that on the built-in 10 GbE port he was only getting around 1 GB/s \(8 Gbps\) from his NAS, and moving to 25 GbE did not dramatically improve that figure. The commenters point out that macOS lacks SMB Direct \(RDMA\) support, which could be the real limiting factor when transferring over SMB, and that a cheaper Thunderbolt PCIe chassis might have been sufficient.

hackernews · speckx · Jul 31, 16:15 · [Discussion](https://news.ycombinator.com/item?id=49125034)

**Background**: 25 Gigabit Ethernet \(25 GbE\) is a data center-oriented networking standard defined by IEEE 802.3 that offers a cost-effective upgrade from 10 GbE with higher bandwidth and port density. Thunderbolt is an interface developed by Intel with Apple that combines PCI Express and DisplayPort into a single connector, allowing external PCIe devices like high-speed NICs to be attached to a Mac. The Mac Studio has built-in 10 GbE but no 25 GbE port, so using a Thunderbolt-to-PCIe chassis with a 25 GbE adapter is one way to achieve faster network speeds.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/25_Gigabit_Ethernet">25 Gigabit Ethernet - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Thunderbolt_%28interface%29">Thunderbolt (interface) - Wikipedia</a></li>
<li><a href="https://support.apple.com/guide/mac-studio/take-a-tour-apd0fd69f4be/mac">Take a tour of Mac Studio - Apple Support</a></li>

</ul>
</details>

**Discussion**: Commenters shared mixed experiences: one user using the Sonnet Thunderbolt chassis at work noted its high cost and a 15W upstream power limitation, while another questioned whether a $400 chassis would have sufficed instead of the $1,000 model. Several comments suggested cheaper alternatives like an eGPU enclosure with a PCIe NIC, while others emphasized that the NAS side \(slow CPU or lack of SMB Direct/RDMA on macOS\) is likely the real bottleneck.

**Tags**: `#Thunderbolt`, `#Ethernet`, `#Mac`, `#Networking`, `#Hardware`

---

<a id="item-13"></a>
## [Why VSMOW, the Official Standard Water, Costs $120,000 a Gallon](https://signoregalilei.com/2026/07/26/the-most-official-water-costs-120000-a-gallon/) ⭐️ 7.0/10

An article explains that VSMOW \(Vienna Standard Mean Ocean Water\), the primary isotopic water standard, costs about $120,000 per gallon. The price reflects its essential role in calibrating instruments that measure stable isotope ratios. VSMOW is the zero point for the global δ-scales used in hydrology, paleoclimatology, and food authenticity testing, so its reliability underpins countless measurements worldwide. Understanding its cost highlights the metrology challenges in measuring tiny isotopic variations that affect fields from environmental science to metabolic research. VSMOW was defined in 1968 by the International Atomic Energy Agency and is distilled from ocean water, containing no salt. It is used to define the VSMOW–SLAP calibration scale for hydrogen and oxygen isotopes, and from 2005 to 2019 the kelvin was defined using the triple point of VSMOW water.

hackernews · surprisetalk · Jul 31, 15:00 · [Discussion](https://news.ycombinator.com/item?id=49124042)

**Background**: Water molecules contain different combinations of isotopes of hydrogen and oxygen, such as deuterium \(²H\) and oxygen-18 \(¹⁸O\), which have slightly different physical properties. These isotopic ratios vary naturally across the water cycle, but measuring them accurately from first principles is extremely difficult. Therefore, laboratories use carefully prepared reference materials like VSMOW as a common zero point, against which unknown samples are reported in delta notation \(δ²H and δ¹⁸O\). VSMOW serves as the anchor for stable isotope ratio mass spectrometry and laser-based analyzers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vienna_Standard_Mean_Ocean_Water">Vienna Standard Mean Ocean Water</a></li>
<li><a href="https://tsapps.nist.gov/srmext/certificates/archives/8535.pdf">Reference Material 8535 VSMOW Vienna Standard Mean Ocean Water</a></li>

</ul>
</details>

**Discussion**: Commenters noted that most VSMOW use is for instrument calibration, since absolute isotope-ratio measurements are not feasible from first principles. One commenter compared it to NIST&\#x27;s expensive peanut butter reference material \(~$2.44/g\), another wondered why pure ¹H₂¹⁶O isn&\#x27;t used instead, and others shared that deuterium-heavy water costs roughly $2,600–$3,800 per gallon while tritiated water would be about $44 million per gallon. A playful comment read &\#x27;VSMOW&\#x27; as &\#x27;Very Standard Mean Ocean Water&\#x27;.

**Tags**: `#metrology`, `#stable isotopes`, `#calibration`, `#standards`, `#chemistry`

---

<a id="item-14"></a>
## [Simon Willison on Open-Weight AI Revolution in Oxide and Friends Podcast](https://simonwillison.net/2026/Jul/31/oxide-and-friends/#atom-everything) ⭐️ 7.0/10

Simon Willison joined Bryan Cantrill and Adam Leventhal on the Oxide and Friends podcast to discuss the surge of open-weight AI models, highlighted by Kimi K3 matching proprietary frontier models, and public letters on open weights and American AI leadership signed by nearly every major AI figure except Anthropic. This conversation highlights a pivotal shift as open-weight models like Kimi K3 and DeepSeek V4 Flash approach or match proprietary frontier performance, potentially democratizing access to cutting-edge AI. The nearly unanimous industry letter on open weights underscores the strategic and policy significance of this movement. Kimi K3 is a 2.8-trillion-parameter open model with a 1-million-token context window and native vision, described as the world&\#x27;s first open 3T-class model. Meanwhile, DeepSeek V4 Flash 0731, released July 31, 2026, shows notable improvements in agentic and coding tasks, and Anthropic was the notable exception to the open-weight letter.

rss · Simon Willison · Jul 31, 21:33

**Background**: Open-weight models publicly release their trained parameters, allowing others to download, use, and sometimes modify them depending on the license. Historically, state-of-the-art models like GPT-4 and Claude were proprietary, but open-weight releases such as Llama, DeepSeek, and Kimi are increasingly competitive with closed frontier systems. The podcast also touches on related incidents like accidental cyberattacks and the broader implications for AI leadership.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://artificialanalysis.ai/articles/deepseek-v4-flash-0731-scores-50-on-the-artificial-analysis-intelligence-index-10-points-above-previous-deepseek-v4-flash">DeepSeek V4 Flash 0731 scores 50 on the Artificial Analysis ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Open-weight_model">Open-weight model</a></li>

</ul>
</details>

**Tags**: `#open-weight`, `#AI`, `#podcast`, `#Simon Willison`, `#frontier models`

---

<a id="item-15"></a>
## [smevals: A Lightweight Suite for Evaluating LLM Models, Prompts, and Harnesses](https://simonwillison.net/2026/Jul/31/smevals/#atom-everything) ⭐️ 7.0/10

Simon Willison, working with Prime Radiant&\#x27;s applied AI research lab, has released smevals, a new tool for running small evaluation suites across different model configurations. The tool, installable via uvx, provides commands to run evals, grade results, and serve or build static HTML reports. smevals offers a lightweight and agent-friendly alternative to heavier evaluation frameworks, making it easier for developers to compare models, prompts, and harness configurations. It addresses a growing need for practical evaluation tooling as LLM usage expands across many teams. The framework defines a clear vocabulary: evals contain tasks, runs execute configs via runners, and graders apply checks \(including custom script-based checkers\) to produce grades. An example eval for haiku writing demonstrates the report dashboard with leaderboards, pass rates, and grader thresholds.

rss · Simon Willison · Jul 31, 21:15

**Background**: LLM evaluation harnesses are frameworks for testing model outputs against structured prompts, datasets, and rubrics to measure quality, safety, and reliability. Established tools like EleutherAI&\#x27;s lm-evaluation-harness support many benchmarks and backends, while uvx runs Python CLI tools in isolated temporary environments. smevals aims to be a smaller, simpler option that can be driven by coding agents and produce shareable static reports.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/31/smevals/">smevals—a small eval suite for evaluating models, prompts ...</a></li>
<li><a href="https://pypi.org/project/smevals/">smevals · PyPI</a></li>
<li><a href="https://github.com/prime-radiant-inc/smevals">GitHub - prime-radiant-inc/smevals: A framework for running ...</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#evaluation`, `#tooling`, `#AI/ML`, `#testing`

---

<a id="item-16"></a>
## [Mandatory Peer Review System Exposes Low-Quality AI Conference Reviews](https://www.reddit.com/r/MachineLearning/comments/1vbeqhw/if_reviewing_is_mandatory_for_paper_submissions/) ⭐️ 7.0/10

The post argues that AI conferences requiring authors to review as a submission condition invalidate the &\#x27;volunteer work&\#x27; excuse for poor reviews. It highlights that vague, unsubstantiated criticisms such as &\#x27;novelty is limited&\#x27; are unprofessional without concrete justification. This could pressure conference organizers to impose quality standards on reviews and improve the integrity of the peer-review process. Researchers, especially junior ones, may benefit from more constructive and accountable feedback. The post gives examples of expected justifications, such as specifying which prior work is similar or what comparison is missing. It argues that vague statements could be written by anyone, including non-experts, and fail to meet professional standards.

reddit · r/MachineLearning · Kwangryeol · Jul 31, 03:05

**Background**: Traditionally, peer review in AI conferences is voluntary, but some conferences now require authors to review in exchange for their own submissions. This shift makes reviewing an obligation, and critics argue it should therefore be held to the same rigor as the papers themselves. The post builds on this shift to argue reviewers must provide concrete evidence for claims.

**Discussion**: Commenters shared experiences of absurd reviews, such as a reviewer claiming results were due to luck with no justification. Others noted that reviewers can always find reasons to reject and might be influenced by personal taste or even LLM-generated suggestions. There is general agreement that the review system needs reform.

**Tags**: `#peer review`, `#machine learning`, `#academia`, `#conferences`, `#research ethics`

---

<a id="item-17"></a>
## [DeepSeek-V4-Flash-0731 Runs on Single 40GB A100 via Unsloth GGUF](https://www.reddit.com/r/LocalLLaMA/comments/1vbwuq0/deepseekv4flash0731_unsloth_gguf_on_a100/) ⭐️ 7.0/10

A user reports running the DeepSeek-V4-Flash-0731 model on a 40GB A100 GPU using unsloth&\#x27;s Q8\_K\_XL GGUF, achieving about 16.1 tok/s generation with all experts offloaded to CPU. A follow-up note adds that with 6 experts loaded into VRAM, the same model runs losslessly at 17.7 tok/s in an agentic coding loop driven by Codex. It demonstrates that a modern large Mixture-of-Experts model can run fully locally on a single datacenter GPU with moderate VRAM, lowering the hardware barrier for local inference and agentic workflows. Community benchmarks also show much higher speeds on high-end consumer rigs, hinting that optimized runtimes and quantizations continue to improve. The 162GB Q8\_K\_XL GGUF leaves most of the 40GB A100 free — only 15.8GB of VRAM is used when all experts sit on CPU — because Mixture-of-Experts models keep only a few active experts resident for each token. Commenters pointed to an alternate 4-bit ds4 quant and reported roughly 40 tok/s with unsloth&\#x27;s UD-Q8\_K\_XL on a 128GB RTX Pro 6000 Blackwell + RTX 5090 system.

reddit · r/LocalLLaMA · Different-Pickle1021 · Jul 31, 17:06

**Background**: GGUF is a file format for running quantized LLMs locally, and the &\#x27;Q8\_K\_XL&\#x27; suffix indicates an 8-bit quantized version of the model weights; lower bit counts such as 2-bit or 4-bit trade accuracy for much smaller file sizes. DeepSeek-V4-Flash-0731 is a sparse Mixture-of-Experts model, which uses only a subset of its &\#x27;experts&\#x27; per token, so inference software can offload inactive experts to CPU RAM or even NVMe to drastically reduce GPU memory usage. Unsloth&\#x27;s Dynamic 2.0 GGUFs are specifically designed to improve quality-per-bit through dynamic quantization of critical layers.

<details><summary>References</summary>
<ul>
<li><a href="https://unsloth.ai/docs/basics/unsloth-dynamic-2.0-ggufs">Unsloth Dynamic 2.0 GGUFs | Unsloth Documentation</a></li>
<li><a href="https://atomic.chat/blog/guides/what-is-gguf">What Is GGUF ? A Complete Guide - Atomic Chat</a></li>
<li><a href="https://apxml.com/courses/mixture-of-experts-advanced-implementation/chapter-4-efficient-moe-inference/expert-offloading">MoE Expert Offloading to CPU/NVMe - apxml.com</a></li>

</ul>
</details>

**Discussion**: Commenters were largely positive and practical: one user predicted much faster speeds once llama.cpp supports DSpark with DeepSeek-V4, while another shared a 4-bit ds4 GGUF on Hugging Face. A high-end setup owner reported ~40 tok/s generation and ~320 tok/s prompt processing with unsloth&\#x27;s UD-Q8\_K\_XL on a 128GB RTX Pro 6000 Blackwell + RTX 5090 build, and said he is considering adding another RTX Pro 6000 to reach an estimated 200–300 tok/s.

**Tags**: `#DeepSeek`, `#GGUF`, `#LLM inference`, `#A100`, `#LocalLLaMA`

---

<a id="item-18"></a>
## [Big Food vs. the People: Report on Lawsuits Draws Skepticism](https://www.lighthousereports.com/investigation/big-food-vs-the-people/) ⭐️ 6.0/10

An investigative report claims large food companies are secretly suing governments over health regulations, but it has been criticized for exaggerating the issue and omitting key context. Commenters note that roughly 193 of 239 lawsuits took place in Mexico, mostly against that country&\#x27;s labeling rules. This matters because corporate legal challenges can delay or weaken public health measures like labeling laws and sugar taxes, directly affecting nutrition and obesity rates. It also highlights how media framing can distort public debate on corporate accountability. According to the report and commenters, the lawsuits focused heavily on Mexico&\#x27;s labeling regulation, with companies arguing that the laws violated their constitutional rights, though the article did not specify which rights. The article&\#x27;s own statistics show 193 of 239 lawsuits, about 80%, were in Mexico, undercutting the global &\#x27;Big Food vs. the People&\#x27; framing.

hackernews · jruohonen · Jul 31, 16:04 · [Discussion](https://news.ycombinator.com/item?id=49124858)

**Background**: Governments around the world have introduced health-focused regulations on food, such as mandatory nutrition labeling, sugar taxes, and advertising restrictions, to combat obesity and diabetes. When companies face such rules, they may challenge them in court, arguing that the measures infringe on commercial rights or exceed government authority. The investigative report intended to reveal these legal tactics, but its framing was criticized as misleading because it omitted the specific constitutional arguments and the geographic concentration of the cases.

**Discussion**: Comments were largely critical of the article. One user called it &\#x27;badly written propaganda&\#x27; and pointed out the Mexico-centric nature of the lawsuits, while another defended companies&\#x27; right to sue, noting that the sugar tax in the UK actually benefited Coca-Cola. Another commenter shared a 1977 quote about senators not having the luxury of waiting for evidence, along with statistics showing rising obesity and diabetes rates, and another jokingly questioned the phrase &\#x27;behind closed doors.&\#x27;

**Tags**: `#food industry`, `#public health`, `#regulation`, `#lawsuits`, `#investigative journalism`

---

<a id="item-19"></a>
## [Red Bull-Funded Dubious Research Shaped Energy Drink Policy](https://www.theexamination.org/articles/red-bull-funded-research-energy-drinks-alcohol) ⭐️ 6.0/10

An investigative article by The Examination reveals that questionable research funded by Red Bull has influenced energy drink policy, raising concerns about scientific integrity and public health. This matters because corporate-funded research can skew public policy and health regulations, potentially prioritizing commercial interests over consumer safety. It underscores the need for transparency in science funding and policy-making. The article is published at theexamination.org and highlights how funding sources may bias research outcomes that are used to shape energy drink regulations. The investigation specifically ties Red Bull to research that downplayed risks or supported industry-friendly policies.

hackernews · Jimmc414 · Jul 31, 15:58 · [Discussion](https://news.ycombinator.com/item?id=49124738)

**Background**: Energy drinks are highly caffeinated beverages that have faced regulatory scrutiny over health concerns, especially regarding consumption by youth and mixing with alcohol. Corporate-funded research has historically been used by industry players to lobby against stricter regulations. The Examination is a nonprofit newsroom that investigates health and science topics.

**Discussion**: Commentators expressed varied views: one described caffeine addiction and withdrawal from regular energy drink consumption, while another reported feeling no effect from caffeine at all. Others argued that energy drinks are comparable to coffee in caffeine content and dismissed the opposition as a moral panic, with one commenter questioning whether the findings apply to juice mixed with vodka.

**Tags**: `#research integrity`, `#public policy`, `#energy drinks`, `#caffeine`, `#science`

---

<a id="item-20"></a>
## [Tesla reportedly weighs selling China business to enable SpaceX merger](https://electrek.co/2026/07/30/tesla-weighs-selling-china-business-spacex-merger/) ⭐️ 6.0/10

According to a Wall Street Journal report, Tesla is considering selling its China business to clear the path for a potential merger with SpaceX. Elon Musk has denied the report, but the news remains unconfirmed. This would be a massive deal in the auto industry, as Tesla&\#x27;s Shanghai factory builds more than half of all Tesla vehicles. If the sale proceeds, it would separate the single biggest piece of Tesla&\#x27;s car operation and could reshape Tesla&\#x27;s global footprint, while a Tesla-SpaceX merger would create an unprecedented combined company. The Wall Street Journal report was published around July 30, 2026, and the Electrek article includes a note that Elon Musk has denied the claim. The denial should be taken &\#x27;with a grain of salt,&\#x27; according to Electrek, and the Shanghai facility&\#x27;s output represents the majority of Tesla&\#x27;s global vehicle production.

rss · Electrek · Jul 31, 02:04

**Background**: Tesla and SpaceX are both led by Elon Musk and have been deepening their collaboration; for example, in March 2026 Musk announced Terafab, a planned semiconductor fabrication plant jointly developed by Tesla, SpaceX, and Intel, with initial prototype operations near Gigafactory Texas. Such joint projects have fueled speculation about a possible merger between the two companies. A merger would face significant regulatory scrutiny, and selling Tesla&\#x27;s China business could be a way to address antitrust or national-security concerns while raising cash and simplifying the combined corporate structure.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Terafab">Terafab</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#SpaceX`, `#Merger`, `#China`, `#Automotive`

---

<a id="item-21"></a>
## [Hobbyist Trains Transformer to Predict Blood Glucose from Personal Data](https://www.reddit.com/gallery/1vc1txc) ⭐️ 6.0/10

A developer trained an encoder-only transformer that predicts blood glucose up to two hours ahead using past glucose, carbohydrate, and insulin data, and future meal/insulin inputs. The largest model has 17 million parameters, was pretrained in about 48 hours, fine-tuned in under 10 minutes, and is currently running on the author&\#x27;s phone. This project shows how off-the-shelf deep learning can be applied to personal health data, potentially aiding type 1 diabetes management. Open-sourcing the code and weights under MIT could encourage further patient-driven research and comparison with established models. The model is BERT-style with bidirectional attention while masking future glucose, uses variable context of 8–24 hours, and can autoregressively predict beyond two hours. It operates in Kovatchev risk space reparameterized to \[40, 400\] mg/dL and combines DILATE loss for the median with pinball loss for uncertainty bands.

reddit · r/MachineLearning · 0xdeadf1sh · Jul 31, 20:09 · [Discussion](https://www.reddit.com/r/MachineLearning/comments/1vc1txc/i_have_trained_a_model_to_predict_my_blood_sugar_p/)

**Background**: Blood glucose prediction is important for managing diabetes, since knowing future levels can help users adjust insulin or meals. DILATE is a loss function designed for multi-step time-series forecasting that accounts for both shape and temporal misalignment. Kovatchev risk space is a transformation that reflects the asymmetric clinical danger of low versus high blood glucose.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/1909.09020">Shape and Time Distortion Loss for Training Deep</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1474667016416216">Model-Based Control of Type 1 Diabetes in “Risk Space”</a></li>

</ul>
</details>

**Discussion**: Commenters were interested but skeptical: one asked why a large transformer was needed, another worried about overfitting and whether predictions were on training data, and a third asked how it compares to CGMformer or simpler LSTM/RNN models given inconsistent carb intake data. Overall sentiment is curiosity mixed with calls for stronger validation.

**Tags**: `#transformers`, `#health`, `#time-series`, `#blood-glucose`, `#personal-ML`

---

<a id="item-22"></a>
## [Model Size Trends Suggest Opus-Level Performance on Consumer Laptops in a Year](https://www.reddit.com/gallery/1vbzicu) ⭐️ 6.0/10

A Reddit user, surprised that DeepSeek V4 Flash runs in a sub-$50,000 setup, plotted model size versus benchmark scores using Opus/Sonnet 5 data. The trend projection suggests Opus 4.5-level performance could arrive on MacBook Air/Pro within a year. If the trend holds, frontier-model intelligence could become accessible on consumer laptops, drastically lowering the hardware barrier for local LLM inference. This would benefit developers, researchers, and hobbyists who currently rely on cloud APIs or expensive workstations. DeepSeek V4 Flash is a mixture-of-experts model with 284B total parameters and 13B activated, supporting a 1-million-token context. The poster cautions that data points above an AA score of 40 are sparse, so extrapolation beyond that is uncertain.

reddit · r/LocalLLaMA · No-Meringue5867 · Jul 31, 18:42 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1vbzicu/with_release_of_deepseek_v4_i_wanted_see_how_the/)

**Background**: Model size trends in LLMs examine how parameter counts relate to benchmark performance. Mixture-of-experts \(MoE\) models activate only a fraction of parameters per token, enabling larger total sizes with reasonable compute. The user references Anthropic&\#x27;s Claude model tiers \(Opus, Sonnet\) and the Artificial Analysis \(AA\) index as rough performance measures.

<details><summary>References</summary>
<ul>
<li><a href="https://www.modelscope.cn/models/deepseek-ai/DeepSeek-V4-Flash">DeepSeek-V4-Flash · Models</a></li>
<li><a href="https://www.orcarouter.ai/blog/deepseek-v4-flash-official-release">DeepSeek V4 Flash: Official Release, Explained - orcarouter.ai</a></li>
<li><a href="https://llm-stats.com/benchmarks/aa-index">AA-Index Leaderboard - llm-stats.com</a></li>

</ul>
</details>

**Discussion**: Commenters cautioned that agentic reliability improves faster than knowledge density, citing Qwen3.6-27B as strong at tool-calling but not richer in knowledge than last year&\#x27;s dense models. Others noted RAM is the bottleneck — laptops would need 256–512GB unified memory to run Q2 quantization of the new DeepSeek — and criticized Microsoft&\#x27;s 8GB Windows 11 baseline as insufficient.

**Tags**: `#LLM`, `#DeepSeek V4`, `#model trends`, `#local inference`, `#hardware`

---

<a id="item-23"></a>
## [On Type Inference: A Look at Type Inference Trade-offs](https://radekmie.dev/blog/on-type-inference/) ⭐️ 6.0/10

A technical blog post titled &\#x27;On Type Inference&\#x27; was published at radekmie.dev, exploring how type inference works and the design trade-offs involved in static type systems. The discussion suggests it focuses on TypeScript&\#x27;s structural typing and edge cases involving object literals and return types. Type inference is a core feature of modern statically typed languages such as TypeScript, Rust, and Haskell, directly affecting developer productivity and type safety. The post contributes to ongoing conversations about how much inference and structural typing should be adopted, and how languages balance expressiveness with clarity. The community discussion centers on TypeScript&\#x27;s structural typing: a function declared to return \`\{x: number\}\` but given a literal \`\{x: number, y: number\}\` is considered valid under &\#x27;open product types&\#x27; by one commenter, while the language&\#x27;s special handling of object literals is called an &\#x27;ugly hack.&\#x27;

reddit · r/programming · radekmie · Jul 31, 12:03 · [Discussion](https://www.reddit.com/r/programming/comments/1vbp0vm/on_type_inference/)

**Background**: Type inference is the automatic detection of expression types without explicit type annotations, a key feature in many statically typed languages. The Hindley–Milner type system, originally developed for ML, pioneered efficient inference of the most general type and influenced modern languages such as Haskell and Rust. In TypeScript, inference is structural, meaning an object&\#x27;s shape rather than its declared name determines compatibility, which leads to subtle behavior around object literals and excess properties.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Type_inference">Type inference - Wikipedia</a></li>
<li><a href="https://www.typescriptlang.org/docs/handbook/type-inference.html">TypeScript: Documentation - Type Inference</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hindley-Milner_type_inference">Hindley-Milner type inference</a></li>

</ul>
</details>

**Discussion**: The comments show mixed reactions: one user argues that TypeScript&\#x27;s open structural product types make extra-property returns valid and that literal inference is an ugly hack, while another jokes that the title promised type inference but the post seems to wander elsewhere. A third commenter criticizes the &\#x27;On \[Topic\]&\#x27; blog title style as lazy and pretentious.

**Tags**: `#type inference`, `#programming languages`, `#static typing`, `#TypeScript`

---

<a id="item-24"></a>
## [EVs Reach 34.5% of French New Car Sales, Led by Renault and Tesla](https://cleantechnica.com/2026/07/24/evs-take-34-5-share-in-france-renault-and-tesla-dominate/) ⭐️ 6.0/10

Electric vehicles accounted for 34.5% of new car sales in France, with Renault and Tesla leading the market. Diesel&\#x27;s share fell to just 2.6%, down from 57% in 2015. This shows a dramatic acceleration of France&\#x27;s transition away from internal combustion engines, particularly diesel. The steep decline in diesel and strong EV growth signal that European automakers and consumers are embracing electrification faster than many expected. The 34.5% share includes both battery-electric vehicles \(BEVs\) and plug-in hybrids \(PHEVs\), with BEVs reportedly up 65% year-on-year. Diesel, once France&\#x27;s dominant fuel, now accounts for only 2.6% of new registrations.

reddit · r/electricvehicles · GalacticScale · Jul 31, 21:56 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1vc4mat/evs_take_345_share_in_france_renault_tesla/)

**Background**: France has long had a high diesel adoption rate, but government incentives, environmental regulations, and new EV models have reshaped the market. BEVs run solely on batteries, while PHEVs combine an electric motor with an internal combustion engine, and hybrids recharge their batteries through regenerative braking. The dramatic decline from 57% diesel share in 2015 to 2.6% now reflects both policy shifts and changing consumer preferences.

**Discussion**: Commenters expressed surprise at diesel&\#x27;s collapse from 57% to 2.6%, called the growth of hybrids impressive, and noted that BEVs were up 65% year-on-year. One commenter also clarified that PHEVs should not be counted as pure EVs, but considered them a good transitional step toward full electrification.

**Tags**: `#EVs`, `#France`, `#Renault`, `#Tesla`, `#market share`

---

<a id="item-25"></a>
## [2027 Slate Truck First Drive: Simplicity as Superpower](https://www.motortrend.com/reviews/first-drive-2027-slate-truck-prototype) ⭐️ 6.0/10

MotorTrend published a first-drive review of the 2027 Slate Truck prototype, highlighting its minimalist design and low cost. The truck strips away modern conveniences like power windows in favor of manual controls and a simple EV powertrain. The Slate Truck&\#x27;s focus on simplicity and an entry-level price could broaden EV appeal beyond tech enthusiasts to fleet operators and budget-conscious buyers. If successful, it may prove that EVs don&\#x27;t need to be expensive or feature-packed to gain mass adoption. The two-seat pickup features manual windows, traditional A/C knobs, steel wheels, and an LFP \(lithium iron phosphate\) battery, with pricing around $20,000–$25,000. This makes it one of the most affordable EVs slated for the American market.

reddit · r/electricvehicles · TripleShotPls · Jul 31, 14:06 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1vbrxra/we_drove_the_2027_slate_truck_simplicity_might_be/)

**Background**: The Slate Truck is an American EV startup&\#x27;s attempt to build a cheap, no-frills electric pickup. LFP batteries are a type of lithium-ion cell that offers lower cost, longer lifespan, and improved safety compared to conventional NMC chemistries. By cutting out unnecessary electronics and using inexpensive materials, Slate aims to keep the base price near $20,000.

<details><summary>References</summary>
<ul>
<li><a href="https://www.greencars.com/expert-insights/meet-slate-first-american-ev-pickup-truck-for-20k">Meet Slate : First American EV Pickup Truck for $20k | GreenCars</a></li>
<li><a href="https://manofmany.com/auto/cars/slate-truck-price-specs-revealed">SLATE &#x27;s Modular $24,950 EV Truck is the Ultimate... | Man of Many</a></li>
<li><a href="https://www.ufinebattery.com/blog/lfp-vs-nmc-battery-what-is-the-difference/">LFP vs NMC Battery : 2026 Comparison (Safety, Lifespan, Cost)</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some argue the truck is a great fleet option and praise its DIY-friendly simplicity, while others think it&\#x27;s overpriced compared to cheap gas pickups like the Ford Maverick. One redditor specifically wants an LFP battery, plastic panels, and simple controls, and says they may order one within three years.

**Tags**: `#Electric Vehicles`, `#Automotive`, `#Truck Review`, `#EV Design`, `#LFP Battery`

---

<a id="item-26"></a>
## [Lucid Demands $50,000 to Unlock Salvaged $140,000 Car, Sparking Right-to-Repair Outcry](https://www.youtube.com/watch?v=rAUF9QGlCE8) ⭐️ 6.0/10

Rich Rebuilds reports that Lucid Motors is demanding a $50,000 fee to unlock the software of a salvaged Lucid Air valued at $140,000. The video highlights the automaker&\#x27;s anti-consumer policy that effectively bricks used or rebuilt EVs. This practice raises serious concerns about the right-to-repair movement and environmental sustainability, as it discourages the reuse of EVs and forces owners to scrap otherwise functional vehicles. It also highlights a growing industry trend of automakers using software locks to control the secondhand and salvage markets. The video, by rebuilding expert Rich Benoit, likely involves a Lucid Air with extensive damage that had been rebuilt but cannot be activated without a $50,000 unlock fee from Lucid. The decision shows a stark contrast to right-to-repair advocates&\#x27; calls for accessible diagnostic and repair information for EVs.

reddit · r/electricvehicles · lostinheadguy · Jul 31, 22:54 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1vc61ae/rich_rebuilds_lucid_wants_50000_to_unlock_my/)

**Background**: Luxurious electric vehicles like the Lucid Air use sophisticated battery management systems and encrypted software to manage performance and safety. When a vehicle is salvaged, manufacturers often lock its software to prevent unauthorized use, but critics argue this violates the right-to-repair ethos and increases electronic waste. The right-to-repair movement advocates for consumers&\#x27; ability to repair their own devices and vehicles, reducing waste and cost. Lucid&\#x27;s high-end Air has a range of up to 512 miles and advanced charging, making its software lockout particularly wasteful for functional hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://lucidmotors.com/technologies">Lucid Motors Technologies | Powertrain, Battery, Charging and ...</a></li>
<li><a href="https://lucidmotors.com/knowledge/vehicles/air/lucid-air-in-depth/charging-your-lucid-air">Charging Your Lucid Air | Knowledge | Lucid Motors</a></li>
<li><a href="https://autos.yahoo.com/ev-and-future-tech/articles/dutch-students-just-built-ev-150039009.html">Dutch Students Just Built an EV Designed to Be Repaired by Anyone...</a></li>

</ul>
</details>

**Discussion**: Commenters overwhelmingly condemn Lucid&\#x27;s behavior as anti-consumer, with one noting the environmental impact of essentially &\#x27;disposable cars.&\#x27; Another commenter declares &\#x27;this is the result of electing a government that favors the wealthy and corporations over people,&\#x27; while another simply states &\#x27;This needs to be stopped.&\#x27;

**Tags**: `#right-to-repair`, `#EV`, `#Lucid`, `#anti-consumer`, `#sustainability`

---

<a id="item-27"></a>
## [Slate Pickup Prototype Drive: A Bare-Bones EV Truck for the Austerity Era](https://www.caranddriver.com/reviews/a73296422/2027-slate-ev-truck-prototype-drive/) ⭐️ 6.0/10

Car and Driver published a first-drive review of the 2027 Slate pickup, an ultra-modular budget EV truck from startup Slate Auto. The truck forgoes nearly every creature comfort to keep its base price well below $30,000. With the average new-car transaction price hovering around $50,000, Slate targets the growing demand for genuinely affordable vehicles in a K-shaped economy. If the truck succeeds, it could prove there is a viable market for low-cost, no-frills EVs beyond the mainstream luxury-oriented offerings. The two-door compact EV pickup is designed to be highly modular and customizable, but it comes with standard safety features such as automatic emergency braking, airbags, and a backup camera. Slate Auto is backed by Jeff Bezos, and the model was unveiled on April 24, 2025.

reddit · r/electricvehicles · 622niromcn · Jul 31, 20:18 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1vc22pw/we_drive_the_slate_pickup_an_ev_for_the_new/)

**Background**: Most electric pickups on the market, such as the Ford F-150 Lightning and Tesla Cybertruck, carry premium price tags, while average new-car prices have climbed toward $50,000. Slate Auto is a Michigan-based startup that aims to counter this trend with a bare-bones, &\#x27;analog&\#x27; EV pickup that emphasizes simplicity and low cost rather than high-tech features. The truck is part of a broader movement toward modular vehicle designs that allow owners to customize or reconfigure their vehicles.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Slate_Truck">Slate Truck - Wikipedia</a></li>
<li><a href="https://techcrunch.com/2025/04/24/bezos-backed-slate-auto-debuts-analog-ev-pickup-truck-that-is-decidedly-anti-tesla/">Bezos-backed Slate Auto debuts analog EV pickup truck that is...</a></li>
<li><a href="https://vehiclereport.com/blog/the-rise-of-modular-cars-customizable-vehicles-for-modern-drivers">The Rise of Modular Cars: Customizable Vehicles for Modern ...</a></li>

</ul>
</details>

**Discussion**: Community reactions were mixed. One commenter expressed hope for the truck, saying long-term testing and later production units will tell a better story, while another argued that for a bare-bones EV, the price still seems high compared to a base Nissan Leaf or Chevy Bolt with better range and comfort, though it may be a good deal as a pickup truck.

**Tags**: `#EV`, `#pickup truck`, `#startup`, `#affordability`

---