---
layout: default
title: "Horizon Summary: 2026-05-25 (EN)"
date: 2026-05-25
lang: en
---

> From 33 items, 25 important content pieces were selected

---

1. [LLM Agents Show Constraint Decay in Backend Code Generation](#item-1) ⭐️ 8.0/10
2. [Microsoft open-sources earliest DOS source code](#item-2) ⭐️ 8.0/10
3. [Scammers abuse internal Microsoft account for spam](#item-3) ⭐️ 8.0/10
4. [16-Byte Demo Creates Audiovisual Magic](#item-4) ⭐️ 8.0/10
5. [AMD to Drop Linux Support for Free Vivado Tier in 2026.1](#item-5) ⭐️ 8.0/10
6. [Armin Ronacher criticizes AI slop in bug reports](#item-6) ⭐️ 8.0/10
7. [PapersWithCode Revival Adds Multi-Metric Support](#item-7) ⭐️ 8.0/10
8. [BitCPM-CANN: First Native 1.58-Bit LLM Training on Ascend NPU](#item-8) ⭐️ 8.0/10
9. [DeepSeek Releases Reasonix: A Cost-Efficient Native Coding Agent](#item-9) ⭐️ 7.0/10
10. [Memory now accounts for ~66% of AI chip component costs](#item-10) ⭐️ 7.0/10
11. [Greg Brockman Interview Discusses OpenAI and AI Industry](#item-11) ⭐️ 7.0/10
12. [CBP Tightens Electronic Device Searches at Borders](#item-12) ⭐️ 7.0/10
13. [Usborne 1980s Computer Books Inspire Generations of Coders](#item-13) ⭐️ 7.0/10
14. [Community compares Qwen3.6 and Gemma4 models](#item-14) ⭐️ 7.0/10
15. [Uncensored Models Serve Practical Needs Beyond Roleplaying](#item-15) ⭐️ 7.0/10
16. [Tesla Renames FSD to 'Tesla Assisted Driving' in China](#item-16) ⭐️ 7.0/10
17. [Vision LLMs Underperform OCR in Long Document QA Benchmark](#item-17) ⭐️ 7.0/10
18. [Mastering Dyalog APL: Interactive Book Released](#item-18) ⭐️ 6.0/10
19. [Nostalgic Look at Early Computing Experiences](#item-19) ⭐️ 6.0/10
20. [Ruby for Good: A Gathering for Social Good Maintainers](#item-20) ⭐️ 6.0/10
21. [Datasette 1.0a30 adds customizable Jump to menu with plugin hook](#item-21) ⭐️ 6.0/10
22. [AI Revives 1980s Usborne Game as Interactive Web App](#item-22) ⭐️ 6.0/10
23. [Questioning NVIDIA's dominance for local LLMs in 2026](#item-23) ⭐️ 6.0/10
24. [Qwen3.6-35B-A3B Uncensored Model Runs 200k Context on Mini PC](#item-24) ⭐️ 6.0/10
25. [Exploring Specialized Database Engines Beyond SQL and NoSQL](#item-25) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [LLM Agents Show Constraint Decay in Backend Code Generation](https://arxiv.org/abs/2605.06445) ⭐️ 8.0/10

A systematic study reveals that LLM agents' performance drops by about 30 points in assertion pass rates when constrained by architectural rules, a phenomenon termed 'constraint decay'. This highlights a critical reliability gap for using LLM agents in production backend development, where strict architectural constraints are common, undermining trust in AI-generated code for complex systems. The study tested LLM agents on multi-file backend generation tasks while progressively adding constraints such as ORM patterns and framework conventions, finding performance concentrated in convention-heavy frameworks.

hackernews · wek · May 24, 12:55 · [Discussion](https://news.ycombinator.com/item?id=48256912)

**Background**: LLM-based coding agents are AI systems that generate code from natural language prompts. While they excel at unconstrained tasks like prototyping, their reliability when adhering to specific architectural rules had been understudied. Constraint decay refers to the substantial decline in generation quality as the number of structural requirements increases.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.06445">[2605.06445] Constraint Decay : The Fragility of LLM Agents in...</a></li>
<li><a href="https://www.alphaxiv.org/overview/2605.06445v1">Constraint Decay : The Fragility of LLM Agents in Backend... | alphaXiv</a></li>
<li><a href="https://agentpatterns.ai/verification/constraint-decay-backend-agents/">Constraint Decay in Backend Code Generation - AgentPatterns.ai</a></li>

</ul>
</details>

**Discussion**: Commenters noted parallels to long-horizon task errors and suggested mitigation strategies like gradual constraint inclusion or external orchestrators. Some criticized the study for not using frontier models due to cost, limiting generality.

**Tags**: `#LLM agents`, `#code generation`, `#constraint decay`, `#backend development`, `#AI reliability`

---

<a id="item-2"></a>
## [Microsoft open-sources earliest DOS source code](https://arstechnica.com/gadgets/2026/04/microsoft-open-sources-the-earliest-dos-source-code-discovered-to-date/) ⭐️ 8.0/10

Microsoft has open-sourced the earliest known DOS source code, recovered from paper printouts via OCR by a team of historians and preservationists. This marks a significant preservation effort for a foundational piece of computing history. This release preserves a critical piece of software history that shaped the personal computer industry, making it available for study and preservation by the open-source community. It also demonstrates Microsoft's commitment to transparency and historical preservation. The source code was transcribed from paper printouts provided by Tim Paterson, the original developer of DOS, using modern OCR software that struggled with the decades-old print quality. The effort was led by Yufeng Gao and Rich Cini as part of the 'DOS Disassembly Group.'

hackernews · DamnInteresting · May 24, 01:21 · [Discussion](https://news.ycombinator.com/item?id=48253386)

**Background**: DOS (Disk Operating System) was the foundational operating system for early IBM PCs and compatibles, developed by Microsoft in the early 1980s. The source code had not been stored digitally and was only recoverable from physical printouts, making this open-sourcing a remarkable historical achievement.

**Discussion**: The community largely praised the effort, with one user thanking Microsoft and noting the simultaneous open-sourcing of the early BASIC code. Another user expressed envy at how a few thousand lines of assembly were enough to launch a successful software company. A comment highlighted the difficulty of OCR from old paper printouts.

**Tags**: `#open source`, `#DOS`, `#Microsoft`, `#history`, `#preservation`

---

<a id="item-3"></a>
## [Scammers abuse internal Microsoft account for spam](https://techcrunch.com/2026/05/21/scammers-are-abusing-an-internal-microsoft-account-to-send-spam/) ⭐️ 8.0/10

Scammers are exploiting a legitimate internal Microsoft email account to send spam and phishing links, bypassing traditional email security filters. This vulnerability undermines trust in Microsoft's email security, potentially leading to widespread phishing attacks that appear to come from a trusted source. The abused account is used for sending genuine account alerts, making it difficult for recipients to distinguish legitimate emails from spam.

hackernews · spike021 · May 24, 00:51 · [Discussion](https://news.ycombinator.com/item?id=48253186)

**Background**: Microsoft uses various domains for official communications, but managing a large portfolio of domain assets can lead to security gaps. Email authentication methods like SPF, DKIM, and DMARC are designed to prevent spoofing, but internal accounts may bypass these checks.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/05/21/scammers-are-abusing-an-internal-microsoft-account-to-send-spam/">Scammers are abusing an internal Microsoft account to send ...</a></li>
<li><a href="https://sesamedisk.com/microsoft-internal-account-abuse-2026-cybersecurity/">Microsoft Internal Account Abuse in 2026: Cybersecurity ...</a></li>

</ul>
</details>

**Discussion**: Comments on Hacker News expressed frustration with Microsoft's domain management, noting that even internal users are unsure of all legitimate domains. Some users shared personal experiences with phishing attempts and Microsoft's inadequate security responses.

**Tags**: `#security`, `#microsoft`, `#spam`, `#phishing`

---

<a id="item-4"></a>
## [16-Byte Demo Creates Audiovisual Magic](https://hellmood.111mb.de/wake_up_16b_writeup.html) ⭐️ 8.0/10

A writeup explains how a 16-byte executable demo, 'Wake up! 16b', generates audiovisual output through extreme code optimization and size coding techniques. This demo pushes the boundaries of size coding, demonstrating that complex audiovisual effects can be achieved in just 16 bytes, inspiring further innovation in the demoscene and low-level programming communities. The demo fits within 16 bytes, smaller than typical 64k or 4k intros, and produces both sound and visuals. The writeup details specific optimization tricks used to achieve this extreme compression.

hackernews · MaximilianEmel · May 24, 00:30 · [Discussion](https://news.ycombinator.com/item?id=48253060)

**Background**: The demoscene is a computer art subculture where programmers create self-contained audiovisual demos, often with strict size limits such as 64k or 4k bytes. Size coding is the practice of writing extremely compact code, using techniques like instruction overlapping and self-modifying code. This 16-byte demo represents an extreme achievement in that tradition.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Demoscene">Demoscene</a></li>
<li><a href="http://www.sizecoding.org/wiki/Main_Page">SizeCoding.org</a></li>

</ul>
</details>

**Discussion**: Community comments express awe and admiration, with one calling it 'witchcraft' and another noting it sent them on a rabbit hole. There is high engagement and appreciation for the technical feat, with some remarking it surpasses previous 32-byte demos and includes sound.

**Tags**: `#demoscene`, `#size coding`, `#optimization`, `#low-level programming`

---

<a id="item-5"></a>
## [AMD to Drop Linux Support for Free Vivado Tier in 2026.1](https://adaptivesupport.amd.com/s/question/0D5Pd00001YQLdMKAX/why-is-vivado-20261-dropping-linux-support-for-free-tier-?language=en_US) ⭐️ 8.0/10

AMD announced that the free tier of Vivado (Vivado ML Standard) will no longer support Linux starting from version 2026.1, while Windows support remains. This decision alienates students, hobbyists, and developers who rely on Linux for FPGA development, potentially shrinking the AMD/Xilinx ecosystem and driving users to competitors like Lattice. The free Vivado tier (formerly WebPACK) is the only no-cost option for AMD FPGAs; removing Linux support forces Linux users to either switch to Windows or purchase expensive paid licenses for full-featured versions.

hackernews · zdw · May 24, 04:14 · [Discussion](https://news.ycombinator.com/item?id=48254309)

**Background**: Vivado is AMD's (formerly Xilinx's) FPGA design suite. The free WebPACK/Standard edition provides limited features at no cost. Historically, Vivado has supported both Windows and Linux, with Linux being favored by many developers for server and automation workflows. AMD's acquisition of Xilinx has raised concerns about shifting priorities toward enterprise licensing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vivado">Vivado - Wikipedia</a></li>
<li><a href="https://wiki.archlinux.org/title/Xilinx_Vivado">Xilinx Vivado - ArchWiki</a></li>

</ul>
</details>

**Discussion**: Community comments express strong backlash: users criticize AMD for ignoring Linux users' needs, citing ecosystem harm and licensing hassles, with some switching to Lattice or Altera. Long-time AMD users feel the company no longer understands its customer base after the acquisition.

**Tags**: `#FPGA`, `#AMD`, `#Vivado`, `#Linux`, `#EDA tools`

---

<a id="item-6"></a>
## [Armin Ronacher criticizes AI slop in bug reports](https://simonwillison.net/2026/May/24/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Armin Ronacher, creator of Flask and other popular Python tools, published a blog post criticizing the influx of AI-generated bug reports on his open source project Pi, and advocates for a simple, human-observed format for issue submissions. This critique highlights a growing problem in open source maintenance where AI-generated issues waste maintainers' time with confident but inaccurate analysis. It calls for a return to concise, human-authored bug reports to preserve project health. Ronacher's proposed format requires only four elements: the command run, expected behavior, actual behavior, and the exact error or log. He emphasizes that AI rewrites strip away the human voice and inject speculative conclusions.

rss · Simon Willison · May 24, 18:46

**Background**: Bug reports are vital for open source maintenance, allowing developers to reproduce and fix issues. With the rise of AI coding assistants, many users now submit issues generated or enhanced by large language models (LLMs), which often produce verbose, inaccurate, and overconfident reports. This phenomenon, sometimes called 'slop,' burdens maintainers and undermines the collaborative process.

**Tags**: `#open-source`, `#bug reports`, `#AI`, `#software maintenance`, `#issue tracking`

---

<a id="item-7"></a>
## [PapersWithCode Revival Adds Multi-Metric Support](https://www.reddit.com/r/MachineLearning/comments/1tmawv5/paperswithcode_new_features_week_1_p/) ⭐️ 8.0/10

NielsRogge from Hugging Face announced new features for the revived PapersWithCode.co, including support for multiple metrics per benchmark and submission of papers from external sources like GitHub and blog posts. This update enhances the platform's utility for tracking state-of-the-art models by allowing richer comparisons across efficiency and accuracy metrics, and makes it easier for researchers to contribute non-Arxiv papers. Multi-metric leaderboards now support metrics like Word Error Rate (WER) and Inverse Real-Time Factor (RTFx) for ASR, and mAP plus FPS for object detection on COCO. External paper submission is enabled via a dedicated form with automatic enrichment.

reddit · r/MachineLearning · NielsRogge · May 24, 12:31

**Background**: PapersWithCode was a popular website for tracking state-of-the-art results in machine learning, but it was shut down by its previous owner. Hugging Face revived it as PapersWithCode.co, an open-source community-driven platform. Multi-metric leaderboards allow comparing models on both accuracy and efficiency, which is increasingly important for real-world deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/inverse-real-time-factor-rtfx">Inverse Real - Time Factor ( RTFx ) in ASR</a></li>
<li><a href="https://huggingface.co/spaces/hf-audio/open_asr_leaderboard">Open ASR Leaderboard - a Hugging Face Space by hf-audio</a></li>
<li><a href="https://arxiv.org/html/2510.06961v1">Open ASR Leaderboard: Towards Reproducible and Transparent ...</a></li>

</ul>
</details>

**Discussion**: The community is enthusiastic, with commenters praising the work and asking for help or features like a paper claiming mechanism to add missing GitHub links. One user asked about the advantage over Hugging Face's daily papers section.

**Tags**: `#paperswithcode`, `#open-source`, `#machine-learning`, `#leaderboard`, `#state-of-the-art`

---

<a id="item-8"></a>
## [BitCPM-CANN: First Native 1.58-Bit LLM Training on Ascend NPU](https://www.reddit.com/r/LocalLLaMA/comments/1tmf63y/bitcpmcann_native_158bit_large_language_model/) ⭐️ 8.0/10

Researchers from OpenBMB present BitCPM-CANN, a family of 1.58-bit ternary LLMs trained natively on Huawei Ascend NPU using CANN, MindSpeed, and Megatron-LM, achieving 4.5% training overhead and up to 8× memory savings at inference. This work demonstrates that extreme low-bit training is feasible outside the CUDA ecosystem, enabling efficient AI on alternative hardware like Ascend NPU, which could reduce reliance on Nvidia GPUs and lower deployment costs. The BitCPM-CANN models (0.5B to 8B) retain 90-97% of full-precision performance on reasoning benchmarks, with the 3B and 8B variants nearly matching full-precision on GSM8K and BBH. The QAT integration adds only 4.5% training throughput overhead, making ternary training a practical default.

reddit · r/LocalLLaMA · Aaaaaaaaaeeeee · May 24, 15:24

**Background**: 1.58-bit quantization, also known as ternary quantization, restricts weights to three values (-1, 0, +1), drastically reducing memory and computation. CANN (Compute Architecture for Neural Networks) is Huawei's heterogeneous computing platform for AI on Ascend NPUs. MindSpeed is a distributed training framework for Ascend NPU ecosystem, adapted from Megatron-LM. Prior 1.58-bit LLMs were mostly trained on CUDA, making this work a significant port to alternative hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/1.58-bit_large_language_model">1.58-bit large language model - Wikipedia</a></li>
<li><a href="https://www.hiascend.com/document/detail/en/canncommercial/800/quickstart/index/index.html">Overview-Quick Start- CANN commercial edition8.0.0开发文档-昇腾社区</a></li>
<li><a href="https://deepwiki.com/moguizhizi/MindSpeed-LLM">moguizhizi/ MindSpeed -LLM | DeepWiki</a></li>

</ul>
</details>

**Discussion**: The Reddit community expressed strong interest, with comments praising the minimal training overhead and memory savings, while noting that the 0.5B model underperforms on math. Some users tested the models and found limited intelligence at small scales, but acknowledged the achievement of running ternary models without Nvidia hardware. There is anticipation for larger models in this format.

**Tags**: `#LLM`, `#quantization`, `#Ascend NPU`, `#ternary`, `#efficient AI`

---

<a id="item-9"></a>
## [DeepSeek Releases Reasonix: A Cost-Efficient Native Coding Agent](https://esengine.github.io/DeepSeek-Reasonix/) ⭐️ 7.0/10

DeepSeek has launched Reasonix, a terminal-based AI coding agent that is natively designed to work with DeepSeek's API, featuring a cache-first loop to minimize token costs and support for local embeddings via Ollama or DeepSeek-hosted services. Reasonix directly addresses the key pain point of API costs for AI coding assistants by optimizing caching efficiency, which could significantly reduce expenses for developers using DeepSeek's models. It also signals a trend of AI labs creating custom tooling to better leverage their APIs' unique capabilities. The agent is designed around prefix-cache stability, aiming to keep token costs low across long sessions. It is available on GitHub and integrates directly with DeepSeek's API, but community comments have pointed out UX issues with the promotional website and questioned whether a dedicated agent is necessary given that existing tools can already benefit from DeepSeek's cache.

hackernews · Alifatisk · May 24, 13:02 · [Discussion](https://news.ycombinator.com/item?id=48256953)

**Background**: AI coding agents like GitHub Copilot and Codex use large language models to assist with code generation, typically incurring costs per token processed. Caching strategies, especially prefix caching, can reduce repeated computation and lower API expenses. DeepSeek is a prominent AI research lab known for its competitive pricing and high-performance models. Reasonix is built to maximize the caching benefits of DeepSeek's API.

<details><summary>References</summary>
<ul>
<li><a href="https://esengine.github.io/DeepSeek-Reasonix/">Reasonix — DeepSeek -native AI coding agent</a></li>
<li><a href="https://api-docs.deepseek.com/quick_start/agent_integrations/reasonix">Integrate with Reasonix | DeepSeek API Docs</a></li>
<li><a href="https://github.com/esengine/DeepSeek-Reasonix">GitHub - esengine/ DeepSeek - Reasonix : DeepSeek -native AI coding...</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some appreciate the cost optimization potential, while others criticize the website's UX (e.g., animated typing causing content shifts) and argue that existing open-source harnesses like opencode can already leverage DeepSeek's cache effectively. There is also debate about the best caching strategies and whether a dedicated agent is truly needed.

**Tags**: `#AI coding agent`, `#DeepSeek`, `#caching`, `#low cost`, `#software engineering`

---

<a id="item-10"></a>
## [Memory now accounts for ~66% of AI chip component costs](https://epoch.ai/data-insights/ai-chip-component-cost-shares) ⭐️ 7.0/10

Memory has risen to nearly two-thirds of total AI chip component costs, driven by the soaring demand for High Bandwidth Memory (HBM) in AI accelerators. This cost structure shift reveals a significant path for hardware cost reduction: as HBM supply catches up with demand, AI training and inference costs could drop by ~3x without any technical innovation. High Bandwidth Memory (HBM) stacks multiple DRAM dies vertically using through-silicon vias (TSVs) and mounts on an interposer, providing enormous bandwidth but consuming roughly three times the wafer capacity of DDR5 per gigabyte.

hackernews · intelkishan · May 24, 16:31 · [Discussion](https://news.ycombinator.com/item?id=48258684)

**Background**: HBM is a specialized DRAM designed for AI accelerators like NVIDIA H100 and B200, offering much higher bandwidth than conventional RAM. The unprecedented demand from AI has caused DRAM prices to surge—some exceeding 200% since early 2025—and memory has become the dominant cost in chip components.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/ram/hbm-is-eating-your-ram">Here's why HBM is coming for your PC's RAM — HBM consumes around three times the wafer capacity of DDR5 per gigabyte, as AI supercharges demand for chips and advanced packaging | Tom's Hardware</a></li>
<li><a href="https://introl.com/blog/ai-memory-supercycle-hbm-2026">The AI Memory Supercycle | Introl Blog</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted that waiting for DRAM supply to stabilize could yield a ~3x hardware cost reduction, while others noted personal hardware price pain (e.g., 96GB RAM cost rising from $250 to $1200). Some questioned whether DRAM capacity growth (~20-25%/year) can keep up with AI demand.

**Tags**: `#AI hardware`, `#memory costs`, `#DRAM`, `#semiconductor industry`, `#cost analysis`

---

<a id="item-11"></a>
## [Greg Brockman Interview Discusses OpenAI and AI Industry](https://fs.blog/knowledge-project-podcast/greg-brockman/) ⭐️ 7.0/10

Greg Brockman, co-founder of OpenAI, appeared on The Knowledge Project podcast to discuss OpenAI's journey, governance, and AI developments. This interview offers insights into OpenAI's internal dynamics and the broader AI industry, sparking community debate on corporate governance and non-profit integrity. The interview covers OpenAI's transition from non-profit to capped-profit, and references a personal diary made public in a lawsuit by Elon Musk, which Musk lost due to late filing.

hackernews · prakashqwerty · May 24, 08:29 · [Discussion](https://news.ycombinator.com/item?id=48255593)

**Background**: OpenAI was originally founded as a non-profit AI research lab, but later created a capped-profit arm to attract funding. This structure has been controversial, with critics arguing it undermines non-profit principles. The community discusses figures like Ilya Sutskever and corporate rivalries with Anthropic.

**Discussion**: Commenters expressed skepticism about non-profit integrity, with one user questioning how a non-profit was allowed to transform into a for-profit entity. Another noted the personal diary from Brockman revealed financial ambitions, fueling distrust. Some comments shifted focus to Anthropic as now more important.

**Tags**: `#Greg Brockman`, `#OpenAI`, `#AI interview`, `#AI industry`, `#Hacker News discussion`

---

<a id="item-12"></a>
## [CBP Tightens Electronic Device Searches at Borders](https://www.cbp.gov/document/directives/cbp-directive-no-3340-049b-border-search-electronic-devices) ⭐️ 7.0/10

The U.S. Customs and Border Protection (CBP) issued Directive 3340-049B in January 2025, updating procedures for searching electronic devices at U.S. borders, including the handling of passcode-protected and encrypted data. This directive significantly impacts travelers' digital privacy at U.S. borders, as it formalizes expansive search authorities while creating legal loopholes via 'national security' exceptions that remain undisclosed. The directive clarifies that travelers must provide access to their devices, but passcodes cannot be used to access data stored only remotely (5.3.2). It also states that CBP will not infringe on privacy unless national security requires it, and such cases need not be disclosed.

hackernews · Ember_Wipe · May 24, 19:12 · [Discussion](https://news.ycombinator.com/item?id=48260140)

**Background**: CBP operates under the 'border search exception' to the Fourth Amendment, which allows warrantless searches at international borders. This directive updates a 2009 policy (Directive 3340-049) and is meant to balance national security with privacy concerns amidst rising use of encrypted devices.

**Discussion**: Commenters express distrust, noting that the directive's national security clause effectively allows unlimited searches without accountability. Some criticize the vagueness of the exception, while others point out that similar practices have existed since 2009 and advise using burner devices when traveling.

**Tags**: `#privacy`, `#border search`, `#electronic devices`, `#CBP`, `#digital rights`

---

<a id="item-13"></a>
## [Usborne 1980s Computer Books Inspire Generations of Coders](https://usborne.com/us/books/computer-and-coding-books) ⭐️ 7.0/10

Usborne Publishing has made its classic 1980s computer books available as free PDF downloads, rekindling memories and appreciation among early coders. These books introduced many young readers to programming concepts through engaging illustrations and practical projects, shaping the early computing ecosystem and inspiring countless careers. The collection includes titles such as 'Practice Your BASIC', 'Machine Code for Beginners', and robot-building guides, all originally published in the 1980s and now freely accessible.

hackernews · ngram · May 24, 15:43 · [Discussion](https://news.ycombinator.com/item?id=48258194)

**Background**: In the 1980s, home microcomputers like the ZX Spectrum, Commodore 64, and Amstrad CPC became popular. Usborne's books taught generations how to program in BASIC and machine code, often serving as the only educational resource before the internet.

<details><summary>References</summary>
<ul>
<li><a href="https://retrocomputingforum.com/t/usborne-1980s-computer-books/275">Usborne 1980s computer books - Histories - Retro Computing</a></li>
<li><a href="https://news.ycombinator.com/item?id=32202822">Usborne computer and coding books from the 1980s | Hacker News</a></li>
<li><a href="https://hackaday.com/2017/03/20/usborne-release-more-1980s-computer-books/">Usborne Release More 1980s Computer Books | Hackaday</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News shared heartfelt stories of learning to code from these books, with many crediting them for their subsequent careers in software engineering. Some noted the books' visual appeal and clarity compared to modern programming texts.

**Tags**: `#retro computing`, `#programming education`, `#BASIC`, `#nostalgia`, `#hacker news`

---

<a id="item-14"></a>
## [Community compares Qwen3.6 and Gemma4 models](https://www.reddit.com/r/LocalLLaMA/comments/1tmbola/qwen3635ba3b_vs_gemma426ba4b/) ⭐️ 7.0/10

A Reddit user asked for experiences comparing Qwen3.6-35B-A3B and Gemma4-26B-A4B, and community responses revealed that Gemma runs faster but Qwen has more reliable tool calls, with Gemma preferred for non-coding tasks. This comparison provides actionable insights for practitioners selecting between two popular open-source Mixture-of-Experts (MoE) models for local inference, highlighting trade-offs between speed and tool call reliability. Both models are sparse MoE architectures: Qwen3.6-35B-A3B has 35B total parameters with 3B active, while Gemma4-26B-A4B has 26B total with 4B active. The discussion is based on local inference using llama.cpp on a Radeon 9070 XT GPU.

reddit · r/LocalLLaMA · MarcCDB · May 24, 13:05

**Background**: Sparse Mixture-of-Experts (MoE) models activate only a subset of parameters per token, enabling larger total parameter counts while maintaining inference efficiency. Tool calling (or function calling) is the ability of an LLM to invoke external tools or APIs, a critical capability for building AI agents. The comparison is relevant to users running models locally for tasks like coding and general text generation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.labellerr.com/blog/qwen3-6-35b-a3b-open-source-ai-model/">Qwen3.6-35B-A3B: The Small Model That Codes Like a Giant</a></li>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B-it">google/gemma-4-26B-A4B-it · Hugging Face</a></li>
<li><a href="https://medium.com/garantibbva-teknoloji/understanding-llm-tool-calling-traditional-vs-embedded-approaches-fc7e576d05de">Understanding LLM Tool Calling: Traditional vs. Embedded ...</a></li>

</ul>
</details>

**Discussion**: Community members reported that Qwen had significantly fewer issues with tool calls, while Gemma was faster and better for non-coding tasks. One user summarized the sentiment as "Love with your Gemma, use your Qwen for everything else."

**Tags**: `#LLM`, `#Qwen`, `#Gemma`, `#model comparison`, `#local inference`

---

<a id="item-15"></a>
## [Uncensored Models Serve Practical Needs Beyond Roleplaying](https://www.reddit.com/r/LocalLLaMA/comments/1tlzvfs/is_there_any_reason_for_an_uncensored_model_if/) ⭐️ 7.0/10

A Reddit user questioned the value of uncensored LLMs beyond roleplaying, sparking a discussion where the community highlighted real-world use cases such as financial advice, medical translation, coding debugging, historical analysis, and reverse engineering. This discussion clarifies that uncensored models are critical for tasks where alignment refusals hinder productivity, and highlights the growing demand for models that prioritize utility over safety guardrails in specialized domains. Users noted that uncensored models do not magically solve hallucination or accuracy issues, but they eliminate friction caused by refusals for sensitive topics, such as stock research or reverse engineering, as explicitly mentioned in the comments.

reddit · r/LocalLLaMA · vick2djax · May 24, 02:49

**Background**: Uncensored language models, also called heretic or abliterated models, are fine-tuned or modified versions that remove the built-in refusal behavior (alignment) typical of standard models. Tools like Heretic enable this without retraining. These models are popular among users who need unrestricted responses for research, creative writing, or technical tasks where safety filters are counterproductive.

<details><summary>References</summary>
<ul>
<li><a href="https://insiderllm.com/guides/best-uncensored-local-llms/">Best Uncensored Local LLMs (And Why You Might Want Them)</a></li>
<li><a href="https://github.com/FemaleGhost/heretic-AI">GitHub - FemaleGhost/ heretic - AI : Fully automatic censorship removal...</a></li>
<li><a href="https://huggingface.co/TheBloke/WizardLM-13B-Uncensored-GGUF">TheBloke/WizardLM-13B-Uncensored-GGUF · Hugging Face</a></li>

</ul>
</details>

**Discussion**: Top comments strongly argue uncensored models are essential for practical uses: one user praised them for stock advice without disclaimers, another listed many scenarios where censored models fail (e.g., medical advice, translation of strong language, debugging, historical questions). A third highlighted reverse engineering as a key use case. The overall sentiment supports uncensored models as a necessary tool, not just for roleplaying.

**Tags**: `#large language models`, `#uncensored models`, `#AI censorship`, `#model behavior`

---

<a id="item-16"></a>
## [Tesla Renames FSD to 'Tesla Assisted Driving' in China](https://electrek.co/2026/05/23/tesla-now-calls-fsd-tesla-assisted-driving-in-china-a-more-truthful-name/) ⭐️ 7.0/10

Tesla has rebranded its Full Self-Driving (FSD) system as 'Tesla Assisted Driving' in China, complying with Chinese regulatory demands for more accurate naming that reflects the system's true capabilities. This move highlights how Chinese regulations can enforce honest marketing, contrasting with corporate puffery often seen elsewhere, and sets a precedent for autonomous driving terminology globally. The name change applies only to the Chinese market, where regulators have pushed back against misleading terms like 'Full Self-Driving' that imply full autonomy not yet achieved.

reddit · r/electricvehicles · SpriteZeroY2k · May 24, 01:59 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1tlyt3e/tesla_now_calls_fsd_tesla_assisted_driving_in/)

**Background**: Tesla's 'Full Self-Driving' is an advanced driver-assistance system that requires active driver supervision, not true self-driving. The term has been criticized globally for overpromising capabilities. China's regulatory environment has shown willingness to enforce accurate labeling, as seen with similar demands for solid-state battery terminology.

**Discussion**: Commenters praised China's regulatory stance against corporate puffery, with one noting that the Chinese government will 'bring the fucking hammer down' for false advertising. Another felt the new name is more realistic and explicitly branded.

**Tags**: `#Tesla`, `#FSD`, `#China`, `#regulations`, `#autonomous driving`

---

<a id="item-17"></a>
## [Vision LLMs Underperform OCR in Long Document QA Benchmark](https://www.reddit.com/r/artificial/comments/1tlzy43/visioncapable_llms_vs_ocr_for_longdocument/) ⭐️ 7.0/10

A benchmark on 30 long, image-heavy PDFs from MMLongBench-Doc found that vision-capable LLMs (Claude Sonnet 4.5) achieved only 52.0% accuracy at $0.2552 per query, while OCR-based pipelines reached up to 59.6% accuracy at lower cost. This challenges the popular claim that vision LLMs can replace OCR for document understanding, showing that proper OCR with layout extraction still offers better accuracy and reliability, especially in production environments. The vision LLM arm had a 7% intrinsic failure rate due to PDF file size issues that persisted after retries, while OCR arms had 0% failure. Vision models particularly underperformed on chart- and table-heavy pages.

reddit · r/artificial · Uiqueblhats · May 24, 02:52

**Background**: MMLongBench-Doc is a benchmark for long-context, multimodal document understanding, containing over 1,000 expert-annotated questions. OCR extracts text from images, often combined with layout analysis to preserve document structure. Vision-capable LLMs can directly process PDFs as images, but may struggle with complex layouts and large file sizes.

<details><summary>References</summary>
<ul>
<li><a href="https://mayubo2333.github.io/MMLongBench-Doc/">MMLongBench - Doc</a></li>
<li><a href="https://pvsravanth.medium.com/mastering-paddleocr-for-layout-detection-d4edb26723d0">Mastering PaddleOCR for Layout Detection | by Sravanth | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters generally agreed with the findings, noting that vision LLMs still cannot match proper layout extraction for structured documents. One comment emphasized that system components like OCR and orchestration are crucial for production-grade reliability.

**Tags**: `#LLM`, `#OCR`, `#Document QA`, `#Benchmarking`, `#RAG`

---

<a id="item-18"></a>
## [Mastering Dyalog APL: Interactive Book Released](https://mastering.dyalog.com/README.html) ⭐️ 6.0/10

A comprehensive interactive book titled 'Mastering Dyalog APL' has been released, providing a modern, Jupyter Notebook-based learning experience for the APL array programming language. This resource lowers the barrier to learning APL, a powerful but niche language, by offering interactive examples that help build muscle memory with its unique symbolic notation, potentially attracting more programmers to explore array programming. The book is available online for free and includes executable code cells, making it easy to experiment with APL concepts directly in the browser. It is based on the original 'Mastering Dyalog APL' text but enhanced with interactive features.

hackernews · tosh · May 24, 11:42 · [Discussion](https://news.ycombinator.com/item?id=48256475)

**Background**: APL (A Programming Language) is a high-level, array-oriented programming language known for its concise use of special symbols to express complex operations on arrays. Dyalog APL is the most widely used modern implementation, offering enterprise-grade features and cross-platform support. Array programming is a paradigm where operations apply to entire arrays at once, enabling expressive and efficient code for data-intensive tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/APL_(programming_language)">APL (programming language) - Wikipedia</a></li>
<li><a href="https://www.dyalog.com/">Home - Dyalog</a></li>
<li><a href="https://aplwiki.com/wiki/Dyalog_APL">Dyalog APL APL (programming language) - Wikipedia A Dyalog workflow. Or two. — Learning APL - GitHub Pages TryAPL Welcome to Dyalog Videos Page Why Are More Engineers Discovering Dyalog APL in 2025?</a></li>

</ul>
</details>

**Discussion**: The community comments reflect appreciation for the interactive Jupyter Notebook format, with one user noting it helps build muscle memory for APL symbols. Some discussion also touches on the niche status of APL, its enterprise licensing model, and alternative learning resources like 'Learn APL' and solving problems on Kattis.

**Tags**: `#APL`, `#programming languages`, `#array programming`, `#interactive learning`

---

<a id="item-19"></a>
## [Nostalgic Look at Early Computing Experiences](https://susam.net/childhood-computing.html) ⭐️ 6.0/10

The article is a personal reflection on childhood computing, sharing sentimental memories and learning moments from the early days of personal computers. It resonates with many readers who grew up with early computers, highlighting the profound emotional and educational impact of hands-on computing experiences. The article does not provide specific technical details but evokes the sensory and cognitive aspects of using machines like the Commodore 64 and early Windows PCs.

hackernews · blenderob · May 24, 12:07 · [Discussion](https://news.ycombinator.com/item?id=48256597)

**Background**: In the 1980s and 1990s, home computers like the Commodore 64 and IBM PC compatibles introduced millions to programming and digital creativity. These machines had limited hardware but encouraged deep exploration and learning, often through trial and error without internet access.

**Discussion**: Commenters share nostalgic memories of their first computers, including a C64 with a misconfigured tape head and a Pentium 166 MHz machine. One user describes the epiphany of understanding variables in RPG Maker, while another expresses conflict over modern screen time policies for children.

**Tags**: `#nostalgia`, `#computing history`, `#programming`, `#childhood`

---

<a id="item-20"></a>
## [Ruby for Good: A Gathering for Social Good Maintainers](https://ti.to/codeforgood/rubyforgood) ⭐️ 6.0/10

Ruby for Good announced its in-person event, explicitly stating it is a gathering of open source maintainers working on social good projects, not a hackathon, and opened early-bird registrations. This event provides a dedicated space for maintainers to collaborate on long-running social good projects, fostering community and sustained impact beyond typical hackathons. The event is not a hackathon but a friendly gathering of open source maintainers working on existing projects, some of which have been running for over 10 years, according to founder Sean Marcia.

hackernews · mooreds · May 24, 15:49 · [Discussion](https://news.ycombinator.com/item?id=48258254)

**Background**: Ruby for Good is a community-driven initiative that brings together Ruby developers to work on open source projects for social good. Unlike hackathons which often start new projects, this event focuses on maintaining and improving existing applications that serve nonprofits and communities.

**Discussion**: The community expressed gratitude and support, with founder Sean Marcia clarifying the non-hackathon nature and opening early-bird registrations. Some users inquired about sponsors, reflecting interest in corporate support for social good.

**Tags**: `#Ruby`, `#open source`, `#social good`, `#conference`, `#community`

---

<a id="item-21"></a>
## [Datasette 1.0a30 adds customizable Jump to menu with plugin hook](https://simonwillison.net/2026/May/24/datasette/#atom-everything) ⭐️ 6.0/10

Datasette 1.0a30 introduces a new customizable 'Jump to' menu, activated by pressing the '/' key, and a new plugin hook `jump_items_sql()` for adding custom items to the menu. This update enhances navigation within Datasette, making it easier for users to quickly find databases, tables, and other items. The plugin hook empowers developers to extend the menu with custom searches, improving the tool's flexibility and ecosystem. The Jump to menu supports real-time filtering as the user types, and the `jump_items_sql()` hook allows plugins to contribute items via SQL queries. The release is an alpha version (1.0a30), indicating it is still in development.

rss · Simon Willison · May 24, 23:52

**Background**: Datasette is an open-source tool for exploring and publishing data, primarily using SQLite databases. It supports a plugin system based on the pluggy framework, where hooks allow plugins to customize behavior. The new Jump to menu builds on existing action menu patterns to provide a unified search experience across databases, tables, and custom plugin entries.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/stable/plugin_hooks.html">Plugin hooks - Datasette documentation</a></li>
<li><a href="https://github.com/simonw/datasette">GitHub - simonw/datasette: An open source multi-tool for ... datasette-plugins - Skill | Smithery Datasette Adds Semantic Column Types And Plugin Hook Datasette 1.0a8: JavaScript plugins, new plugin hooks and ... Datasette Plugins</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#release`, `#plugin`, `#open-source`, `#data exploration`

---

<a id="item-22"></a>
## [AI Revives 1980s Usborne Game as Interactive Web App](https://simonwillison.net/2026/May/24/usborne-mad-house/#atom-everything) ⭐️ 6.0/10

Simon Willison used Anthropic's Claude to convert the 1983 game 'Mad House' from a PDF of Usborne's 'Creepy Computer Games' book into a fully working JavaScript and HTML interactive version. This demonstrates how large language models can bridge vintage computing nostalgia with modern web development, making classic games accessible without requiring users to type in code manually. Willison provided Claude with the PDF and a prompt asking for a vanilla JS artifact with mobile-friendly design and a retro aesthetic, and the model generated the game's ASCII-style corridors, door controls, and scoring logic.

rss · Simon Willison · May 24, 17:14

**Background**: Usborne Publishing released free PDFs of their 1980s computer books, including 'Creepy Computer Games' (1983), which contained type-in games for platforms like the Commodore 64. Simon Willison is a well-known web developer who frequently experiments with AI tools like Claude. This project showcases the use of AI to reinterpret historical software.

**Tags**: `#retro computing`, `#AI`, `#JavaScript`, `#game development`, `#Claude`

---

<a id="item-23"></a>
## [Questioning NVIDIA's dominance for local LLMs in 2026](https://i.redd.it/pzq8x188q43h1.jpeg) ⭐️ 6.0/10

A Reddit post with 168 points and 89% upvotes questions whether NVIDIA remains the default best GPU choice for running local LLMs in 2026, sparking debate on pricing and alternatives. This discussion matters because NVIDIA's dominance affects consumer hardware decisions and competition in the AI hardware market, especially as local LLM inference grows in popularity. The post highlights that MSRP pricing is often outdated, and some users are combining NVIDIA and AMD GPUs, indicating that alternatives like AMD are becoming viable for local LLM inference.

reddit · r/LocalLLaMA · pmv143 · May 24, 18:34 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1tmkaua/is_nvidia_still_the_default_best_choice_for_local/)

**Background**: Local LLMs are large language models run on personal hardware rather than cloud servers. GPU choice is critical because model inference relies heavily on parallel processing and VRAM. NVIDIA has historically been the default due to its mature CUDA ecosystem and broad software support from tools like Ollama and LM Studio. However, rising GPU prices and the emergence of competitive hardware from AMD and Intel are challenging that default status.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.starmorph.com/blog/local-llm-inference-tools-guide">Local LLM Inference in 2026: The Complete Guide to Tools ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/CUDA">CUDA - Wikipedia</a></li>
<li><a href="https://www.aitooldiscovery.com/how-to/best-local-llm-models">Best Local LLM Models 2026: Benchmarks & Use Cases</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about NVIDIA's pricing, with one noting that MSRP is meaningless due to inflated market prices. Another user shared a mixed NVIDIA+AMD setup, suggesting that a combination of hardware from different vendors is a practical approach.

**Tags**: `#NVIDIA`, `#local LLMs`, `#GPU`, `#AI hardware`

---

<a id="item-24"></a>
## [Qwen3.6-35B-A3B Uncensored Model Runs 200k Context on Mini PC](https://www.reddit.com/r/LocalLLaMA/comments/1tm3toi/qwen3635ba3buncensoredgenesisapexmtp/) ⭐️ 6.0/10

A new uncensored, quantized version of Qwen3.6-35B-A3B called Genesis-V2-APEX-MTP has been released, featuring multi-token prediction (MTP) support and successful 200,000-token context tests on a Beelink GTR9 Pro mini PC using Q8_K_P MTP quantization. This release demonstrates that large language models with 35B parameters can run efficiently on consumer-grade hardware, challenging the assumption that such models require expensive data center GPUs. It also provides an uncensored variant with enhanced inference speed via MTP, beneficial for local AI applications and privacy. The model uses GGUF format with APEX quantization and MTP support. Safetensors versions are also available for Apple MLX conversion. The recommended quantizations are APEX and MTP-APEX, with custom system prompt and chat template provided.

reddit · r/LocalLLaMA · EvilEnginer · May 24, 06:08

**Background**: Large language models (LLMs) are typically too large to run on personal computers; quantization reduces model size by lowering numerical precision, and multi-token prediction (MTP) speeds inference by predicting multiple tokens at once. The Qwen3.6-35B-A3B model is a sparse mixture-of-experts (MoE) architecture with 35B total parameters but only 3B active, enabling efficient local inference. Safetensors is a secure, fast file format for storing model weights, while GGUF is optimized for CPU inference tools like llama.cpp.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hardware-corner.net/multi-token-prediction-llm-speed/">How Multi-Token Prediction Makes Local LLMs Faster – Without ...</a></li>
<li><a href="https://huggingface.co/docs/safetensors/index">Safetensors · Hugging Face Safetensors – PyTorch File Format | huggingface/safetensors | DeepWiki Safetensors File Format • safetensors - GitHub Pages Package 'safetensors' reference manual SAFETENSORS File - What is it and how do I open it?</a></li>
<li><a href="https://huggingface.co/docs/hub/gguf">GGUF · Hugging Face</a></li>

</ul>
</details>

**Discussion**: The community shows mixed reactions: one user celebrates running a 35B model with 200k context on a mini PC, contrasting with big tech's requirements for 8 H100s. Another user expresses skepticism about APEX quants in coding agents, reporting wrong tangents and looping issues despite using quality presets.

**Tags**: `#LLM`, `#Qwen`, `#Quantization`, `#Local Inference`, `#Uncensored`

---

<a id="item-25"></a>
## [Exploring Specialized Database Engines Beyond SQL and NoSQL](https://blog.gaborkoos.com/posts/2025-09-19-The-Database-Zoo-Exotic-Data-Storage-Engines/) ⭐️ 6.0/10

A blog post titled 'The Database Zoo: Exotic Data Storage Engines' argues that general-purpose databases cannot handle all modern workloads, prompting the rise of specialized engines for time-series, vector, and probabilistic data. This matters because it highlights a shift in the database landscape where specialized engines offer significant performance and efficiency gains for niche applications like IoT monitoring, AI-powered search, and uncertainty management. The post is the first in a series that will cover time-series databases (TSDBs), vector databases, and probabilistic databases in depth, emphasizing their unique optimizations over general-purpose systems.

reddit · r/programming · OtherwisePush6424 · May 24, 02:39 · [Discussion](https://www.reddit.com/r/programming/comments/1tlzo76/the_database_zoo_exotic_data_storage_engines_why/)

**Background**: Traditional SQL databases excel at structured data with complex queries, while NoSQL databases offer flexibility for semi-structured data. However, modern applications like real-time analytics (time-series data), AI-powered similarity search (vector data), and handling uncertain data (probabilistic data) demand specialized storage engines that trade off generality for targeted performance. For instance, time-series databases use specialized compression for timestamped data, vector databases enable efficient high-dimensional similarity search used in retrieval-augmented generation (RAG), and probabilistic databases manage data with associated probabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Time_series_database">Time series database - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vector_database">Vector database - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Probabilistic_database">Probabilistic database - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community reaction is mixed: some users jokingly argue that any database not using SQL is NoSQL, while others criticize the article for lacking rigor and being non-exhaustive for its 'zoo' title. A few express exhaustion with marketing jargon.

**Tags**: `#databases`, `#NoSQL`, `#SQL`, `#time-series`, `#vector databases`

---