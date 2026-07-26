---
layout: default
title: "Horizon Summary: 2026-07-26 (EN)"
date: 2026-07-26
lang: en
---

> From 36 items, 21 important content pieces were selected

---

1. [Inflect v2: Two Ultra-Tiny TTS Models Under 4M and 10M Parameters](#item-1) ⭐️ 9.0/10
2. [Anthropic&\#x27;s New Context Engineering Rules for Claude 5](#item-2) ⭐️ 8.0/10
3. [Open-weight AI is having its Kubernetes moment](#item-3) ⭐️ 8.0/10
4. [Growing vigilante movement disables Flock surveillance cameras](#item-4) ⭐️ 8.0/10
5. [The Dark Night of Mathematics: AI&\#x27;s Existential Challenge](#item-5) ⭐️ 8.0/10
6. [Ruff v0.16.0 Expands Default Rules from 59 to 413](#item-6) ⭐️ 8.0/10
7. [Claude Opus 5 Shows Strong Prompt Injection Resistance](#item-7) ⭐️ 8.0/10
8. [Android May Soon Restrict On-Device ADB](#item-8) ⭐️ 7.0/10
9. [Inside Fedora 45&\#x27;s Build Pipeline from Source to Release](#item-9) ⭐️ 7.0/10
10. [Google backs open-weight AI models](#item-10) ⭐️ 7.0/10
11. [Reddit users share practical small LLM use cases](#item-11) ⭐️ 7.0/10
12. [Llama.cpp Gains Full MCP Support for Agentic Chat](#item-12) ⭐️ 7.0/10
13. [Triton: New DirectX 11 Driver for QEMU](#item-13) ⭐️ 7.0/10
14. [Writing C Programs Without main\(\) Function](#item-14) ⭐️ 7.0/10
15. [Sebastian Lague Builds Graphics Library From Scratch](#item-15) ⭐️ 7.0/10
16. [Website Chronicles Recruiter Ghosting in Tech](#item-16) ⭐️ 6.0/10
17. [Show HN: Brolly – a minimalist plain-text weather site](#item-17) ⭐️ 6.0/10
18. [Bitchat Decentralized Messenger Now on Radicle](#item-18) ⭐️ 6.0/10
19. [IIHS: Waymo autonomous taxis 68% safer than human drivers, with caveats](#item-19) ⭐️ 6.0/10
20. [Massachusetts Bill Aims to Legalize 30-40 mph Electric Motorbikes](#item-20) ⭐️ 6.0/10
21. [Kimi Linear 48B A3B MoE Model Sparks Community Discussion](#item-21) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Inflect v2: Two Ultra-Tiny TTS Models Under 4M and 10M Parameters](https://i.redd.it/xqvybmopbafh1.png) ⭐️ 9.0/10

Developer released Inflect v2, which includes two complete text-to-speech models: Inflect-Nano-v2 at 3.96M parameters and Inflect-Micro-v2 at 9.36M parameters, both running entirely locally on CPU or CUDA without external dependencies. This breakthrough demonstrates that high-quality TTS can be achieved with extremely small models, enabling edge deployment on devices with limited memory and computational power, potentially expanding accessibility for on-device voice synthesis. The models include all inference components—text processing, timing prediction, speech generation, and waveform decoder—within a single package, with Nano being 21× smaller than Kokoro and over 1,000× smaller than Fish Audio S2 Pro.

reddit · r/LocalLLaMA · b111ue · Jul 25, 02:17 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1v5ve6v/i_released_inflect_v2_two_ultratiny_complete_tts/)

**Background**: Traditional neural TTS systems require separate models for text-to-acoustic mapping and a vocoder to convert acoustic features into audio waveforms, often resulting in hundreds of millions of parameters. Parameter count directly impacts model size and memory usage; FP32 format uses 32 bits per weight. Inflect v2 achieves a complete TTS pipeline with under 10M total parameters, making it suitable for resource-constrained environments.

<details><summary>References</summary>
<ul>
<li><a href="https://zilliz.com/ai-faq/what-is-the-function-of-a-vocoder-in-tts">What is the function of a vocoder in TTS? - Zilliz Vector ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Single-precision_floating-point_format">Single-precision floating-point format - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community reacted with disbelief and excitement, with one user admitting they didn&\#x27;t believe the claims until downloading and hearing the samples. Another user joked about running the model on a vintage 1997 Power Macintosh, reflecting enthusiasm for the tiny footprint.

**Tags**: `#TTS`, `#machine learning`, `#open source`, `#model compression`, `#efficiency`

---

<a id="item-2"></a>
## [Anthropic&\#x27;s New Context Engineering Rules for Claude 5](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models) ⭐️ 8.0/10

Anthropic published a blog post detailing new rules for context engineering tailored to the Claude 5 generation of models, moving beyond traditional prompt engineering to systematic context design. These rules signal a shift in how developers should interact with advanced LLMs, potentially improving reliability and task completion, but also raising concerns about vendor lock-in and reduced transparency. The blog post emphasizes structured instructions and context assembly, moving away from verbose prompting; community commenters note increased token usage and accidental deletions with the new models.

hackernews · mellosouls · Jul 25, 20:42 · [Discussion](https://news.ycombinator.com/item?id=49051361)

**Background**: Context engineering is a discipline that designs and optimizes all contextual inputs given to an AI model at inference time, including system prompts, tools, and memory. It extends prompt engineering by considering the entire information ecosystem the model operates within. Claude is Anthropic&\#x27;s family of large language models; the &\#x27;Claude 5 generation&\#x27; refers to the latest models like Opus 5 and Sonnet 4.6.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/context-engineering-ai">Context engineering (AI)</a></li>
<li><a href="https://www.anthropic.com/claude/sonnet">Claude Sonnet \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Some commenters find the advice to be common sense and note discrepancies with practical experience, while others criticize Anthropic&\#x27;s approach as an attempt to increase lock-in by moving harness optimization into proprietary tooling. There are also concerns about over-reliance on Claude&\#x27;s automemory, which makes opaque decisions and increases error rates.

**Tags**: `#claude`, `#context engineering`, `#ai`, `#llm`, `#prompt engineering`

---

<a id="item-3"></a>
## [Open-weight AI is having its Kubernetes moment](https://tobi.knaup.me/2026-07-25-open-weight-ai-is-having-its-kubernetes-moment/) ⭐️ 8.0/10

An article argues that open-weight AI models are becoming the default platform for AI development, analogous to Kubernetes in cloud computing, with significant implications for model regulation, inference pricing, and industry collaboration. This shift could democratize AI development by reducing barriers to entry and enabling community-driven innovation, while also complicating efforts to regulate models based on origin or safety. Open-weight models allow users to self-host and customize, providing a cost baseline that counteracts opaque pricing in proprietary APIs. The article suggests that a truly collaborative open model, akin to Linux, is still an aspirational goal.

hackernews · tknaup · Jul 25, 14:49 · [Discussion](https://news.ycombinator.com/item?id=49048034)

**Background**: Open-weight AI models make the trained neural network weights publicly available, enabling anyone to run, fine-tune, or study them, though the training data and code may remain proprietary. Kubernetes transformed cloud computing by providing a common platform for container orchestration, and the article argues that open-weight models could play a similar role for AI by becoming the standard infrastructure upon which applications are built.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/open-weight-ai-what-we-finally-opened-bonnet-nicolas-pistorio-n3ulf">Open - weight AI : what if we finally opened the bonnet ?</a></li>
<li><a href="https://openai.com/index/introducing-gpt-oss/">Introducing gpt-oss | OpenAI</a></li>

</ul>
</details>

**Discussion**: Commenters debate the feasibility of regulating models by origin \(e.g., Chinese vs American\), noting weights are just numbers. Some praise open-weight models for providing pricing baselines against proprietary API fluctuations. Others echo the need for a truly collaborative open model akin to Linux, while noting that some labs like OpenAI have released open-weight models but not updated them frequently.

**Tags**: `#AI`, `#open-weight models`, `#Kubernetes`, `#inference pricing`, `#model regulation`

---

<a id="item-4"></a>
## [Growing vigilante movement disables Flock surveillance cameras](https://www.theguardian.com/us-news/ng-interactive/2026/jul/25/flock-surveillance-cameras) ⭐️ 8.0/10

A grassroots movement of citizens is actively disabling Flock Safety surveillance cameras across the US, using methods like cardboard shields or pool skimmers, in protest of mass surveillance and perceived corruption. This vigilante action reflects deep public distrust in surveillance technology, challenging the assumption that automated license plate readers \(ALPRs\) are universally accepted for crime prevention. Flock cameras, like Falcon and Sparrow models, are AI-powered ALPR cameras that photograph the rear of all passing vehicles; the movement targets these cameras in tandem installations where one camera watches the other.

hackernews · bookofjoe · Jul 25, 19:02 · [Discussion](https://news.ycombinator.com/item?id=49050538)

**Background**: Flock Safety is a surveillance technology company that sells license plate recognition cameras to law enforcement and communities, claiming to reduce crime while protecting privacy. However, critics argue that such systems enable mass surveillance and lack oversight, exacerbating concerns about civil liberties. The movement echoes historical resistance to surveillance, as seen in community debates about &\#x27;who watches the watchers.&\#x27;

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://www.cnet.com/home/security/when-flock-comes-to-town-why-cities-are-axing-the-controversial-surveillance-technology/">When Flock Comes to Your Town: I Asked Experts What to Do ...</a></li>

</ul>
</details>

**Discussion**: Community comments show broad support for the vigilante actions, with users sharing stories of elderly citizens blocking cameras and debating tactics to defeat tandem installations. Some express distrust in the system, calling it a tool for criminals, while others highlight that opposition to mass surveillance unites people across political divides.

**Tags**: `#surveillance`, `#privacy`, `#civil liberties`, `#vigilantism`, `#protest`

---

<a id="item-5"></a>
## [The Dark Night of Mathematics: AI&\#x27;s Existential Challenge](https://kirwinhampshire.substack.com/p/the-dark-night-of-mathematics) ⭐️ 8.0/10

In this essay, the author explores the existential crisis mathematicians face as AI transforms their craft, urging a shift in how they relate to work and creativity. This discussion is significant because it addresses a growing anxiety among knowledge workers about the value of their skills in an age of increasingly capable AI, raising philosophical questions about the nature of creativity and discovery. The essay focuses on mathematics as a case study for knowledge work, noting that AI systems like automated theorem provers and machine learning for discovery are already changing how theorems are proven and new mathematics is created. The author argues that mathematicians must redefine their relationship with their work to avoid despair.

hackernews · rmdmphilosopher · Jul 25, 15:54 · [Discussion](https://news.ycombinator.com/item?id=49048681)

**Background**: Automated theorem proving has been a subfield of AI since the mid-20th century, with modern systems like Lean 4 enabling large-scale formalization of mathematics. Recently, AI-assisted mathematical discovery has emerged, integrating machine learning, LLMs, and symbolic reasoning to conjecture and prove results. This progress raises profound questions about the role of human mathematicians in an era where AI can autonomously derive new theorems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Automated_theorem_proving">Automated theorem proving - Wikipedia</a></li>
<li><a href="https://www.emergentmind.com/topics/ai-assisted-mathematical-discovery">AI-Assisted Math Discovery</a></li>

</ul>
</details>

**Discussion**: Community comments express a range of perspectives: some agree with the existential crisis while others find joy in mathematics regardless of AI; one welcomes the &\#x27;omniscient mathematician machine&\#x27; while another laments the loss of utility in learning programming languages due to LLMs.

**Tags**: `#mathematics`, `#artificial intelligence`, `#knowledge work`, `#philosophy`, `#professional identity`

---

<a id="item-6"></a>
## [Ruff v0.16.0 Expands Default Rules from 59 to 413](https://simonwillison.net/2026/Jul/25/ruff/#atom-everything) ⭐️ 8.0/10

Ruff v0.16.0, released on July 23, 2026, increases the number of rules enabled by default from 59 to 413, catching many severe issues previously missed. This change will likely break CI pipelines for projects using unpinned Ruff dependencies, but it also significantly improves code quality by catching syntax errors and runtime bugs early. The project&\#x27;s author reported that running the new defaults on sqlite-utils found 1618 errors, with 1538 auto-fixed using --fix --unsafe-fixes, leaving 80 remaining. The new rules include checks for timezone-naive datetime calls and blind exception catches.

rss · Simon Willison · Jul 25, 22:44

**Background**: Ruff is an extremely fast Python linter and code formatter written in Rust, developed by Astral \(now part of OpenAI\). It aims to provide high-performance tooling for the Python ecosystem. Previous defaults hadn&\#x27;t been updated since v0.1.0, while the total rule count grew from 708 to 968.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/ruff/linter/">The Ruff Linter | Ruff</a></li>
<li><a href="https://astral.sh/">Astral: High-performance Python tooling</a></li>
<li><a href="https://pypi.org/project/ruff/">An extremely fast Python linter and code formatter, written in Rust.</a></li>

</ul>
</details>

**Tags**: `#ruff`, `#python`, `#linting`, `#astral`

---

<a id="item-7"></a>
## [Claude Opus 5 Shows Strong Prompt Injection Resistance](https://simonwillison.net/2026/Jul/25/boris-cherny/#atom-everything) ⭐️ 8.0/10

Boris Cherny highlighted that Anthropic&\#x27;s Claude Opus 5 model is significantly more resistant to prompt injection attacks compared to previous models, as detailed in the system card released by Anthropic. This improvement marks a critical advancement in AI safety, as prompt injection is a major security vulnerability for large language models. Enhanced resistance can make LLM-based applications more trustworthy and secure. The system card \(page 73\) reports that across prompt injection evaluations and red teaming, Opus 5 proved very hard to prompt inject successfully. This represents the least prompt-injectable model from Anthropic to date.

rss · Simon Willison · Jul 25, 00:42

**Background**: Prompt injection is a cybersecurity exploit where malicious inputs trick a large language model into ignoring its instructions and performing unintended actions. System cards are structured documents that disclose details about an AI system&\#x27;s architecture, safeguards, and evaluations, akin to nutrition labels for AI systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://www.redhat.com/en/blog/security-beyond-model-introducing-ai-system-cards">Security beyond the model: Introducing AI system cards</a></li>

</ul>
</details>

**Tags**: `#prompt-injection`, `#claude`, `#anthropic`, `#ai-safety`, `#generative-ai`

---

<a id="item-8"></a>
## [Android May Soon Restrict On-Device ADB](https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/) ⭐️ 7.0/10

Android is planning to restrict on-device Android Debug Bridge \(ADB\) usage to improve security, limiting the ability to run ADB commands directly from the Android device itself. This change could impact developers who rely on on-device ADB for debugging and app development workflows, potentially forcing them to use a separate computer. It also affects tools like Shizuku and libadb that depend on this capability, and highlights the ongoing tension between security and developer flexibility in the Android ecosystem. The proposed restriction would prevent ADB from binding to all network interfaces when Wi-Fi debugging is enabled, and may require authentication or limit connections to specific IP addresses. This change is still under discussion and has not yet been implemented in any Android release.

hackernews · shscs911 · Jul 25, 06:57 · [Discussion](https://news.ycombinator.com/item?id=49045159)

**Background**: ADB \(Android Debug Bridge\) is a versatile command-line tool that lets developers communicate with an Android device for debugging, installing apps, and running shell commands. Traditionally, ADB works between two devices: a computer \(client\) and the Android device \(daemon\), but some developers use on-device ADB to run commands directly on the same device. While convenient, on-device ADB can expose the device to network attacks if remote debugging is enabled, which Google aims to mitigate.

<details><summary>References</summary>
<ul>
<li><a href="https://kitsumed.github.io/blog/posts/android-may-soon-restrict-on-device-adb/">Android May Soon Restrict On-Device ADB, Affecting Shizuku, libadb and Developers | Kitsumed Blog</a></li>
<li><a href="https://developer.android.com/tools/adb">Android Debug Bridge (adb) | Android Studio | Android Developers</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions. Some users question the security benefit, noting that on-device ADB requires already enabling developer options and remote debugging, so it affects few users. Others see it as a step toward locking down the platform, while some suggest better solutions like allowing IP restrictions instead of outright blocking.

**Tags**: `#Android`, `#ADB`, `#Security`, `#Developer Tools`, `#Google`

---

<a id="item-9"></a>
## [Inside Fedora 45&\#x27;s Build Pipeline from Source to Release](https://supakeen.com/weblog/the-fedora-45-sausage-factory/) ⭐️ 7.0/10

A comprehensive guide detailing the entire Fedora 45 build process from source code to final release has been published, providing end-to-end documentation of the pipeline. This documentation is invaluable for troubleshooting system behavior changes and understanding Fedora&\#x27;s internal build system, making it easier for users and contributors to debug issues and find where to contribute. The guide covers how filesystem images are produced, including file permission changes across versions, and references the Koji build system. It is highly detailed and includes references to specific Bugzilla issues.

hackernews · 6581 · Jul 25, 11:04 · [Discussion](https://news.ycombinator.com/item?id=49046525)

**Background**: Fedora is a popular Linux distribution that uses the Koji build system for building packages and composing releases. The build process involves multiple stages from source code to RPMs to installable images. This guide documents that pipeline for Fedora 45, which is the upcoming release planned for late 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.pagure.org/koji/using_the_koji_build_system/">Using the koji build system — Koji 1.36.1 documentation</a></li>
<li><a href="https://fedoraproject.org/wiki/Infrastructure/KojiBuildSystem">Infrastructure/KojiBuildSystem - Fedora Project Wiki</a></li>
<li><a href="https://docs.fedoraproject.org/or/releases/f45/">Fedora Linux 45 :: Fedora Docs</a></li>

</ul>
</details>

**Discussion**: Community comments express strong appreciation for the documentation, with one user citing it as helpful for debugging a root file permissions issue. Another user asks where to find areas needing volunteers for contribution, indicating interest in getting involved. Off-topic posts about bluewashing and &\#x27;Beefy Miracle&\#x27; were also present.

**Tags**: `#Fedora`, `#build system`, `#Linux distribution`, `#documentation`

---

<a id="item-10"></a>
## [Google backs open-weight AI models](https://x.com/sundarpichai/status/2081026488158040181) ⭐️ 7.0/10

Google CEO Sundar Pichai tweeted the company&\#x27;s support for open-weight AI models, positioning Google against Anthropic&\#x27;s push for more restrictive closed models. This endorsement from a major player could shift the balance in the open vs. closed source AI debate, potentially pressuring competitors like Anthropic and influencing regulatory perspectives. Open-weight models make trained parameters publicly available but may not be fully open-source; the tweet did not provide technical specifics or list which models Google considers open-weight.

reddit · r/LocalLLaMA · MysteryWra · Jul 25, 15:12 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1v6axx3/google_comes_out_in_favor_of_openweight_models_it/)

**Background**: Open-weight AI models refer to models whose trained parameters \(weights\) are publicly downloadable and usable, offering more transparency than fully closed models but less than open-source ones. The debate between open and closed models centers on safety, customizability, and commercial interests, with Anthropic often advocating for stricter controls to mitigate risks.

<details><summary>References</summary>
<ul>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>
<li><a href="https://allthings.how/what-is-an-open-weight-ai-model-and-how-to-use-one/">What is an Open Weight AI Model and How to Use One</a></li>
<li><a href="https://hellofuture.orange.com/en/a-typology-of-artificial-intelligence-models/">AI models explained: open source vs. open weight vs. closed - Hello Future</a></li>

</ul>
</details>

**Discussion**: Commenters made sarcastic remarks about Anthropic&\#x27;s IPO plans and called out the irony of &\#x27;evil tech giants&\#x27; embracing openness while smaller players like Anthropic push for safety restrictions.

**Tags**: `#AI`, `#open-source`, `#Google`, `#model weights`, `#industry debate`

---

<a id="item-11"></a>
## [Reddit users share practical small LLM use cases](https://i.redd.it/umoqmndkhffh1.jpeg) ⭐️ 7.0/10

A Reddit discussion reveals practical use cases for small LLMs, including using Qwen3 embedding 0.6B for local RAG, classification tasks, and vulnerability localization via Cisco&\#x27;s Antares models. 这突出了小型LLM可以在消费级硬件上有效处理RAG、分类和安全分析等特定任务，从而推动AI普及并保护隐私。 The Qwen3 0.6B embedding model is praised for balancing quality and VRAM usage in local RAG setups, while Cisco&\#x27;s Antares models are optimized for vulnerability localization in code.

reddit · r/LocalLLaMA · International-Car643 · Jul 25, 19:35 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1v6hosb/seriously_what_do_you_do_with_them/)

**Background**: Retrieval-augmented generation \(RAG\) enhances LLMs by retrieving external knowledge, making them more accurate for domain-specific queries. Small LLMs \(under 1B parameters\) can run locally on modest hardware, enabling privacy-sensitive applications. Vulnerability localization uses LLMs to automatically identify vulnerable code lines, aiding security auditing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Retrieval-augmented_generation">Retrieval-augmented generation - Wikipedia</a></li>
<li><a href="https://aws.amazon.com/what-is/retrieval-augmented-generation/">What is RAG? - Retrieval-Augmented Generation AI Explained - AWS</a></li>
<li><a href="https://arxiv.org/html/2404.00287">Evaluating Large Language Models for Line-Level Vulnerability Localization</a></li>

</ul>
</details>

**Discussion**: User maikerukonare recommends the Qwen3 0.6B embedding model for local RAG due to its low VRAM footprint. User muntaxitome simply states &\#x27;classification&\#x27; as a use case. User flower-power-123 shares a link to Cisco Antares, an open-weight model for vulnerability localization.

**Tags**: `#small LLM`, `#local RAG`, `#embedding models`, `#classification`, `#vulnerability localization`

---

<a id="item-12"></a>
## [Llama.cpp Gains Full MCP Support for Agentic Chat](https://www.reddit.com/r/LocalLLaMA/comments/1v6n33i/llamacpp_now_has_full_mcp_support/) ⭐️ 7.0/10

Llama.cpp has fully integrated the Model Context Protocol \(MCP\), enabling its WebUI to act as an agentic chat with tool use capabilities. The support was added via pull request \#26062, led by contributor ngxson, and covers both HTTP and stdio MCP servers. This integration allows users to run agentic workflows entirely locally without external dependencies, democratizing access to tool-using AI assistants. It significantly enhances llama.cpp&\#x27;s utility for developers and power users who value privacy and offline capabilities. MCP servers can be configured via a standard JSON config file or inline command-line arguments. For example, connecting the Serena MCP coding server enables a local-model-powered agentic coder without any additional dependencies.

reddit · r/LocalLLaMA · ilintar · Jul 25, 23:18

**Background**: The Model Context Protocol \(MCP\) is an open standard introduced by Anthropic in November 2024 for connecting AI models to external tools and data sources. Llama.cpp is a popular open-source library for running LLMs locally on consumer hardware. MCP supports two transport types: HTTP servers \(already supported in llama.cpp&\#x27;s client\) and stdio servers, which required deeper integration to pipe processes locally.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://github.com/oraios/serena">GitHub - oraios/serena: A powerful MCP toolkit for coding ...</a></li>
<li><a href="https://www.anthropic.com/news/model-context-protocol">Introducing the Model Context Protocol \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Users expressed excitement about the new capabilities, with one calling it &\#x27;nuts&\#x27; for enabling local agentic workflows. However, some noted that vLLM implemented MCP support about 11 months earlier, and others pointed to a lack of clear documentation, requiring community posts to clarify setup.

**Tags**: `#llama.cpp`, `#MCP`, `#local-llm`, `#agentic-chat`, `#tool-use`

---

<a id="item-13"></a>
## [Triton: New DirectX 11 Driver for QEMU](https://blog.getutm.app/2026/introducing-triton-directx-11-driver-for-qemu/) ⭐️ 7.0/10

Triton is a newly developed DirectX 11 driver for QEMU, enabling GPU virtualization with DirectX 11 support for guest operating systems. This driver significantly enhances QEMU&\#x27;s GPU virtualization, allowing Windows VMs to run DirectX 11 applications and games with improved performance. It expands the usability of QEMU for gaming and graphics-intensive workloads. Triton is the third GPU-related software to bear the name &\#x27;Triton&\#x27;, potentially causing naming confusion with NVIDIA&\#x27;s Triton Inference Server and the Triton language/compiler. The driver focuses on DirectX 11, which is widely used for Windows gaming and applications.

reddit · r/programming · NXGZ · Jul 25, 20:09 · [Discussion](https://www.reddit.com/r/programming/comments/1v6ijz9/introducing_triton_directx_11_driver_for_qemu/)

**Background**: QEMU is a popular open-source emulator and virtualizer that can run operating systems and programs for one machine on a different machine. GPU virtualization in QEMU has traditionally been limited, often requiring complex passthrough setups or relying on legacy graphics APIs. DirectX 11 is a key graphics API for Windows, and native support in QEMU reduces the need for translation layers like Wine or DXVK.

<details><summary>References</summary>
<ul>
<li><a href="https://wiki.archlinux.org/title/QEMU/Guest_graphics_acceleration">QEMU/Guest graphics acceleration - ArchWiki</a></li>
<li><a href="https://documentation.ubuntu.com/server/how-to/graphics/gpu-virtualization-with-qemu-kvm/">GPU virtualisation with QEMU/KVM - Ubuntu Server documentation</a></li>

</ul>
</details>

**Discussion**: Community feedback was mixed: one user pointed out the naming conflict with existing Triton projects, calling it a lack of research. Another user was excited to use QEMU for the first time, while a third user expressed appreciation despite not fully understanding the details.

**Tags**: `#QEMU`, `#DirectX`, `#GPU virtualization`, `#drivers`, `#virtualization`

---

<a id="item-14"></a>
## [Writing C Programs Without main\(\) Function](https://labs.iximiuz.com/tutorials/c-program-without-main-a1eea557) ⭐️ 7.0/10

A tutorial demonstrates how to write valid C programs that do not use the main function by defining custom entry points such as \_start, often requiring direct system calls or assembly code. This exploration deepens understanding of C program startup and linking, showing that main is not mandatory for a valid executable, which is valuable for systems programmers and those working on embedded or low-level code. The approach bypasses the standard C runtime initialization, requiring the programmer to handle tasks like setting up argc/argv or making direct system calls. The article notes that without main, one cannot rely on glibc and must interact with the kernel directly.

reddit · r/programming · iximiuz · Jul 25, 13:50 · [Discussion](https://www.reddit.com/r/programming/comments/1v68yb8/writing_a_valid_c_program_without_main/)

**Background**: In a typical C program, the entry point is main, called after the \_start function initializes the runtime. The \_start function is usually provided by the C runtime library \(crt0.o\). This tutorial explores writing programs that define \_start directly or use linker options to set a custom entry point, eliminating the need for main.

<details><summary>References</summary>
<ul>
<li><a href="https://labs.iximiuz.com/tutorials/c-program-without-main-a1eea557">Writing a (valid) C program without main() | iximiuz Labs</a></li>
<li><a href="https://stackoverflow.com/questions/29694564/what-is-the-use-of-start-in-c">gcc - What is the use of _start () in C? - Stack Overflow Code sample</a></li>
<li><a href="https://www.geeksforgeeks.org/c/write-running-c-code-without-main/">How to write a running C code without main()? - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: Community comments express surprise that the article delves into assembly code rather than a pure C trick, with some noting that using \_start directly is straightforward. Others mention linker options or C++ global constructors as alternative approaches.

**Tags**: `#C programming`, `#entry points`, `#linker`, `#assembly`, `#systems programming`

---

<a id="item-15"></a>
## [Sebastian Lague Builds Graphics Library From Scratch](https://youtu.be/_JGMgpyCTsY) ⭐️ 7.0/10

Sebastian Lague released a video documenting his journey of building a graphics library from scratch, starting with drawing a single triangle and progressing to complex terrain and cloud rendering. This video provides an accessible, hands-on look at the foundational concepts of computer graphics, making it a valuable educational resource for aspiring graphics programmers. The video demonstrates key rendering techniques including triangle rasterization, terrain generation using procedural noise, and volumetric cloud rendering, all built without relying on existing graphics APIs.

reddit · r/programming · Pink401k · Jul 25, 12:55 · [Discussion](https://www.reddit.com/r/programming/comments/1v67ohp/sebastian_lague_i_tried_coding_my_own_graphics/)

**Background**: A graphics library abstracts low-level hardware operations to simplify rendering tasks such as drawing shapes, handling lighting, and managing textures. Building one from scratch helps developers understand the rendering pipeline, including vertex processing, rasterization, and fragment shading. Terrain and cloud rendering often involve procedural generation and volumetric techniques, which are common in modern games and simulations.

<details><summary>References</summary>
<ul>
<li><a href="https://link.springer.com/article/10.1007/s00371-020-01953-y">A survey of modeling, rendering and animation of clouds in computer graphics | The Visual Computer | Springer Nature Link</a></li>
<li><a href="https://en.wikibooks.org/wiki/Blender_3D:_Noob_to_Pro/Landscape_Modeling_I:_Basic_Terrain">Blender 3D: Noob to Pro/Landscape Modeling I: Basic Terrain Create a terrain in Sketchup — From Sandbox to Google Earth ... terrain-rendering · GitHub Topics · GitHub Creating Photorealistic 3D Environments - The Gnomon Workshop Scratchapixel Home Page</a></li>

</ul>
</details>

**Discussion**: One top comment on the video humorously notes that progressing from drawing a triangle to a full countryside with clouds is &\#x27;peak imposter syndrome fuel,&\#x27; reflecting the inspiring yet intimidating nature of the tutorial.

**Tags**: `#graphics programming`, `#rendering`, `#tutorial`, `#software engineering`

---

<a id="item-16"></a>
## [Website Chronicles Recruiter Ghosting in Tech](https://didtheyghostyou.com/) ⭐️ 6.0/10

A new website called &\#x27;Did They Ghost You?&\#x27; collects personal anecdotes of recruiters ghosting job candidates, gaining high engagement on Hacker News with 197 points and 75 comments. This discussion highlights a widespread frustration in the tech job market, where candidates often face unanswered communications after interviews, eroding trust in the hiring process. The website appears to be &\#x27;vibe coded&\#x27; according to one commenter, and includes testimonials from users who were ghosted by major companies like Google and Amazon.

hackernews · mooreds · Jul 25, 20:18 · [Discussion](https://news.ycombinator.com/item?id=49051120)

**Background**: Ghosting refers to abruptly ending communication without any explanation. In the tech industry, recruiter ghosting has become a common complaint, where candidates invest time in interviews only to receive no response.

**Discussion**: Commenters shared personal stories of being ghosted by top tech companies, with some expressing frustration that the practice has worsened over time. One commenter noted the site&\#x27;s design may be &\#x27;vibe coded&\#x27;, suggesting it was created with minimal manual intervention.

**Tags**: `#recruiting`, `#job search`, `#tech industry`, `#ghosting`, `#career`

---

<a id="item-17"></a>
## [Show HN: Brolly – a minimalist plain-text weather site](https://brolly.sh/forecast/RWFP2qW8) ⭐️ 6.0/10

The creator launched Brolly \(brolly.sh\), a plain-text weather forecast site offering 7-day forecasts, hourly details, and previous day logs, built as a personal project in response to the UK MET office&\#x27;s redesign that reduced usability. Brolly demonstrates growing user demand for fast, minimalist, and accessible weather apps, and shows how plain-text interfaces can effectively convey complex data without heavy graphics or animations. The site uses PocketBase \(Go\) with backend-rendered HTML and minimal JavaScript, caches forecasts from Open-Meteo for 5 minutes, and encodes all page state in the URL for shareable and bookmarkable views.

hackernews · jsax · Jul 25, 17:34 · [Discussion](https://news.ycombinator.com/item?id=49049693)

**Background**: Plain-text weather services like wttr.in have long been popular among command-line users and minimalists for their speed and simplicity. Brolly extends this concept to a mobile-friendly, interactive web interface while keeping a text-based aesthetic, addressing frustrations with modern weather sites that prioritize visual design over quick information access.

**Discussion**: Commenters generally praised the site, comparing it favorably to wttr.in and noting its mobile usability. Suggestions included adding Unicode weather symbols, a terminal-friendly curl output, and more intuitive URL patterns. One user highlighted that the past-day log feature is underused in weather apps and works well with LLMs.

**Tags**: `#weather`, `#minimalist`, `#web development`, `#plain text`, `#UI/UX`

---

<a id="item-18"></a>
## [Bitchat Decentralized Messenger Now on Radicle](https://radicle.network/nodes/rosa.radicle.network/rad%3Az2v9tRJz1oknFAqCSY5W5c76nVvm6) ⭐️ 6.0/10

Bitchat, a decentralized messaging app using Bluetooth mesh and Nostr, is now hosted on Radicle, a peer-to-peer code collaboration platform. Community reports from Fusion Festival show low adoption, with only about 20 devices out of 80,000 attendees using the app. This marks a real-world test for decentralized messaging, highlighting the gap between concept and adoption. Radicle provides a censorship-resistant home for such projects, aligning with the ethos of decentralized infrastructure. Bitchat uses a hybrid architecture with Bluetooth mesh for local offline communication and the Nostr protocol for internet-based messaging. Radicle extends Git with conflict-free data types, enabling sovereign code collaboration without central servers.

hackernews · h1watt · Jul 25, 13:18 · [Discussion](https://news.ycombinator.com/item?id=49047365)

**Background**: Bitchat is a decentralized peer-to-peer messaging app that works entirely over Bluetooth mesh networks, allowing communication even when the internet is blocked or unavailable. Radicle is an open-source, peer-to-peer code collaboration platform built on Git, often described as a decentralized alternative to GitHub. Unlike centralized platforms, Radicle uses cryptographic identities and gossip protocols to replicate repositories across peers, giving developers full control over their code and data.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bitchat">BitChat - Wikipedia</a></li>
<li><a href="https://play.google.com/store/apps/details?id=com.bitchat.droid&amp;hl=en-US">bitchat - Apps on Google Play</a></li>
<li><a href="https://radicle.dev/">Radicle: the sovereign forge</a></li>

</ul>
</details>

**Discussion**: Community members shared mixed reactions: one user tested Bitchat at Fusion Festival and observed very low usage, noting only 20 devices and minimal message hops. Others praised the app&\#x27;s concept and Radicle&\#x27;s interface, with one suggesting users pre-download it for future use. A comment also noted Bitchat is an AOS project and wondered why it wasn&\#x27;t hosted on ngit.

**Tags**: `#decentralized-messaging`, `#radicle`, `#bitchat`, `#p2p`, `#real-world-testing`

---

<a id="item-19"></a>
## [IIHS: Waymo autonomous taxis 68% safer than human drivers, with caveats](https://electrek.co/2026/07/25/waymo-is-2-3-safer-than-a-human-driver-says-iihs-with-some-caveats/) ⭐️ 6.0/10

A study by the Insurance Institute for Highway Safety \(IIHS\) found that Waymo&\#x27;s autonomous electric taxis crash 68% less than the average human driver, with lower-severity crashes on average. However, the study includes important caveats regarding driving conditions and comparability. This provides strong evidence that autonomous driving technology can significantly improve road safety, but the caveats highlight that Waymo&\#x27;s limited operating domain \(urban areas, good weather\) may not be directly comparable to the full range of human driving. The findings could influence regulatory decisions and public trust in self-driving cars. The 68% reduction in crash rates refers to police-reported crashes per million miles driven, with Waymo vehicles having only 0.41 crashes versus 2.78 for human drivers. However, Waymos operate mostly in dense urban areas with lower speeds and less highway exposure, and the study did not account for differences in driving environments or weather conditions.

reddit · r/electricvehicles · Electrek · Jul 25, 21:41 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1v6kt0s/waymo_is_23_safer_than_a_human_driver_says_iihs/)

**Background**: The Insurance Institute for Highway Safety \(IIHS\) is an independent nonprofit organization that evaluates vehicle safety through crash tests and research. Waymo, a subsidiary of Alphabet Inc., develops autonomous driving technology and operates a commercial robotaxi service in several U.S. cities. Comparing autonomous vehicle safety to human drivers is challenging because of differences in operating domains and data limitations.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/IIHS">IIHS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Waymo">Waymo - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Some commenters criticized the phrasing &\#x27;2/3 safer&\#x27; as confusing or promotional. Others noted that Waymo&\#x27;s operating area differs significantly from where humans drive, making direct comparisons problematic; they suggested comparing Waymo to ride-share or taxi drivers who cover similar urban areas.

**Tags**: `#autonomous vehicles`, `#safety`, `#Waymo`, `#IIHS`, `#self-driving cars`

---

<a id="item-20"></a>
## [Massachusetts Bill Aims to Legalize 30-40 mph Electric Motorbikes](https://electrek.co/2026/07/25/another-state-may-legalize-electric-motorbikes-up-to-30-and-40-mph-under-sweeping-new-micromobility-bill/) ⭐️ 6.0/10

Massachusetts legislators are considering a comprehensive micromobility bill that would legalize electric motorbikes capable of reaching 30 mph, 40 mph, and beyond, creating a new regulatory framework for these vehicles. This bill could serve as a model for other states, clarifying rules for higher-speed electric motorbikes that currently fall into a legal gray area between e-bikes and mopeds, potentially accelerating micromobility adoption. The bill would establish a new vehicle class distinct from existing e-bike classes \(typically capped at 28 mph\), requiring registration, insurance, or a license for these faster motorbikes, while still classifying them as micromobility rather than full motorcycles.

rss · Electrek · Jul 25, 13:03

**Background**: Micromobility refers to lightweight, personal vehicles like bicycles and scooters used for short trips. In the US, e-bikes are typically classified into three classes: Class 1 \(pedal-assist up to 20 mph\), Class 2 \(throttle up to 20 mph\), and Class 3 \(pedal-assist up to 28 mph\). Vehicles exceeding these speeds are usually considered mopeds or motorcycles and require licensing and insurance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Micromobility">Micromobility - Wikipedia</a></li>
<li><a href="https://bikexchange.com/electric-bike-classes/">Electric Bike Classes Explained - 1 / 2 / 3 / 4 - Bikexchange Electric Bike Classes Explained (Class 1, 2 &amp; 3 Guide For ... WhatsMyBike | E-Bike Class Checker &amp; Information Checker Different Types of Electric Bikes Explained - Bikexchange What Is an E-Bike? A Guide to California E-Bike Classifications. E-Bike Classes Explained: Here&#x27;s Everything You Need to Know</a></li>

</ul>
</details>

**Tags**: `#micromobility`, `#electric motorbikes`, `#e-bikes`, `#legislation`, `#Massachusetts`

---

<a id="item-21"></a>
## [Kimi Linear 48B A3B MoE Model Sparks Community Discussion](https://www.reddit.com/gallery/1v6f5vf) ⭐️ 6.0/10

A Reddit user shared impressions of the Kimi Linear 48B A3B Instruct model, an experimental Mixture-of-Experts model with 1 million token context, noting fast performance but sometimes odd or minimal output behavior. This discussion highlights the community&\#x27;s interest in efficient long-context models using hybrid linear attention and MoE, potentially influencing future open-source model development from Moonshot AI. The model is a 48B total parameter MoE with only 3B active parameters per token, using a 3:1 ratio of linear attention layers to full attention layers for reduced KV-cache usage.

reddit · r/LocalLLaMA · Atretador · Jul 25, 17:58 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1v6f5vf/kimi_linear_48b_a3b/)

**Background**: Kimi Linear is a hybrid linear attention architecture introduced by Moonshot AI that outperforms full attention in various contexts. The 48B A3B variant is a Mixture-of-Experts \(MoE\) model that activates only 3B parameters per token, enabling efficient inference. Mixture-of-Experts divides a model into multiple specialized sub-networks to handle different input patterns, reducing compute costs.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MoonshotAI/Kimi-Linear">GitHub - MoonshotAI/Kimi-Linear</a></li>
<li><a href="https://huggingface.co/moonshotai/Kimi-Linear-48B-A3B-Instruct">moonshotai/Kimi-Linear-48B-A3B-Instruct · Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2510.26692">[2510.26692] Kimi Linear: An Expressive, Efficient Attention ... Top Stories Kimi Linear: An Expressive, Efficient Attention Architecture Kimi-Linear-A3B - a moonshotai Collection - Hugging Face Moonshot AI Kimi-Linear-48B-A3B-Instruct · Models</a></li>

</ul>
</details>

**Discussion**: Commenters expressed interest in a successor or larger MoE model \(100-200B range\). Some noted the model was experimental with limited training and lacked the AttnRes mechanism used in later Kimi models, while others reported that its long-context performance on benchmarks was strong but subjective performance seemed worse, possibly due to implementation issues.

**Tags**: `#Kimi Linear`, `#MoE`, `#LLM`, `#long context`, `#experimental model`

---