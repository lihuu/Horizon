---
layout: default
title: "Horizon Summary: 2026-11-09 (EN)"
date: 2026-11-09
lang: en
---

> From 68 items, 30 important content pieces were selected

---

1. [Goldman Sachs revokes Claude Code access for bankers and traders](#item-1) ⭐️ 8.0/10
2. [Nvidia Board Probes Spying Operation Targeting CEO Jensen Huang](#item-2) ⭐️ 8.0/10
3. [2.8T Kimi-K3.1-Pro-Coder compressed to 775GB via tiered quantization](#item-3) ⭐️ 8.0/10
4. [Consumer Gemini quietly routes Drive and Gmail content to human reviewers](#item-4) ⭐️ 8.0/10
5. [Dux: Open-source Wayland desktop shell adds file manager and theming](#item-5) ⭐️ 7.0/10
6. [Outlook.com Quietly Rejects Inbound Email From Domains Without DMARC](#item-6) ⭐️ 7.0/10
7. [Developer switches from Claude to Pi coding agent harness](#item-7) ⭐️ 7.0/10
8. [C vs Rust: Benchmarking a parse\_number\(\) SQLite Extension](#item-8) ⭐️ 7.0/10
9. [Nace releases Drex Max v1.1 multimodal decision model with open weights](#item-9) ⭐️ 7.0/10
10. [Hobbyist Trains Playable Diffusion World Model of Pokémon Red With System 1/2 Agent Harness](#item-10) ⭐️ 7.0/10
11. [Open-source tool maps LLM answers on censorship by country](#item-11) ⭐️ 7.0/10
12. [Tencent Releases DSpine Draft Model Promising 3x Faster Decoding for Qwen3.8-27B](#item-12) ⭐️ 7.0/10
13. [Intel Arc Pro B70 32GB hits ~half RTX 5090 speed for one-fifth the price on Qwen3-27B](#item-13) ⭐️ 7.0/10
14. [Fine-tuned Qwen3.5-0.8B turns English into bash, beats larger stock models](#item-14) ⭐️ 7.0/10
15. [PyTorch 2.7.1 and Native CUDA Mamba-1 Ported to Legacy NVIDIA GPUs](#item-15) ⭐️ 7.0/10
16. [r/LocalLLaMA asks what local models are actually useful for](#item-16) ⭐️ 7.0/10
17. [Sem86: An x86 Full-System Emulator With Runtime-Loaded Instruction Semantics](#item-17) ⭐️ 7.0/10
18. [C64 Demoscener Explains Bumpmapped Rain Effect in Lunatico](#item-18) ⭐️ 7.0/10
19. [Stroustrup presents C++ profiles for simplicity and safety guarantees](#item-19) ⭐️ 7.0/10
20. [Spectre: design-by-contract language with allocator-centric API claims up to 6x faster than Zig](#item-20) ⭐️ 7.0/10
21. [GPT-6 Astra edits 0.016% of Qwen weights, critics dispute framing](#item-21) ⭐️ 7.0/10
22. [Repo claims 284B DeepSeek on 64GB RAM without a GPU](#item-22) ⭐️ 6.0/10
23. [Blogger Argues Writing Is a Thinking Tool, Not Just Output](#item-23) ⭐️ 6.0/10
24. [How I Fight AI Brain Fry: Managing Parallel AI Coding Sessions](#item-24) ⭐️ 6.0/10
25. [Blog post argues agent memory needs an OpenTelemetry-style standard](#item-25) ⭐️ 6.0/10
26. [GRFNet: Open-source PyTorch model for multichannel time-series classification](#item-26) ⭐️ 6.0/10
27. [Local Qwen3.8 Flash Next Generates 15-Second Three.js Motion Graphics Video on an RTX 4080](#item-27) ⭐️ 6.0/10
28. [Six GPUs \(4x Radeon AI PRO R9700 + 2x RTX 3090\) Run Off One x16 PCIe Slot via a Switch](#item-28) ⭐️ 6.0/10
29. [4x Radeon R9700 Build Serves 8 Users at 128K Context](#item-29) ⭐️ 6.0/10
30. [Hands-On QUBO Tutorial Runs End-to-End on D-Wave Quantum Annealer](#item-30) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Goldman Sachs revokes Claude Code access for bankers and traders](https://www.thestateofai.com/news/goldman-sachs-claude-code-traders-bankers) ⭐️ 8.0/10

Goldman Sachs is reportedly pulling Claude Code access from its bankers and traders, according to a report discussed widely on Hacker News \(542 points, 329 comments\). The rollback applies specifically to front-office finance staff rather than to engineers, who are said to keep using the tool. This is a high-profile case study of agentic AI stalling inside a regulated enterprise, showing that the blockers are security exposure, unpredictable consumption billing and auditability rather than model quality. It signals to other financial institutions and AI vendors that coding agents must be packaged with entitlement controls, cost governance and audit trails before front-office deployment is viable. Commenters point to the &\#x27;lethal trifecta&\#x27; risk of running semi-autonomous agents on workstations that already hold client, trade and proprietary data plus email and internet access, and to chronic billing overages under token-based consumption pricing. Notably, the restriction targets traders specifically — the only staff permitted to send orders — while Gemini is cited as gaining ground because it offers flat-rate billing and handles overages by throttling access to higher-tier models.

hackernews · TheWiggles · Nov 8, 18:16 · [Discussion](https://news.ycombinator.com/item?id=50415628)

**Background**: Claude Code is Anthropic&\#x27;s agentic coding tool that runs in the terminal, IDE or browser and can read a codebase, edit files and execute shell commands on the user&\#x27;s machine. Because it acts rather than merely suggests, deploying it on production workstations in finance raises data-exposure and audit problems that a chat assistant does not. Regulated banks must also be able to show who accessed which data and which approvals were granted, and consumption-based LLM pricing makes per-seat cost forecasting hard compared with flat subscriptions.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI coding agent and assistant</a></li>
<li><a href="https://www.aba.com/news-research/analysis-guides/auditability-and-explainability">Auditability and Explainability: The Foundation for Responsible AI in...</a></li>
<li><a href="https://www.gartner.com/en/newsroom/press-releases/2026-06-24-gartner-predicts-ai-coding-costs-will-surpass-average-developer-salary-by-2028-as-token-consumption-surges">Gartner Predicts AI Coding Costs Will Surpass Average ...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion largely rejects &\#x27;the model wasn&\#x27;t good enough&\#x27; explanations, arguing instead that unattended agents on machines with client data, email and internet access form a security trifecta that regulated firms cannot accept. Others blame chronic billing overages and the lack of normalized pricing from Anthropic, contrasting it with Gemini&\#x27;s flat-rate throttling model, and several note the timing is odd given Goldman&\#x27;s role leading Anthropic&\#x27;s IPO, speculating that an operational incident may have forced the decision.

**Tags**: `#AI coding agents`, `#enterprise security`, `#LLM cost/billing`, `#finance industry AI adoption`, `#compliance and governance`

---

<a id="item-2"></a>
## [Nvidia Board Probes Spying Operation Targeting CEO Jensen Huang](https://nvidianews.nvidia.com/news/statement-from-nvidia-board-of-directors) ⭐️ 8.0/10

Nvidia&\#x27;s board of directors issued a statement confirming it is investigating an intelligence/spying operation that targeted CEO Jensen Huang, a case reportedly involving a Singapore-based firm alleged to be a Chinese front company as well as Huang&\#x27;s admitted infidelity. According to Bloomberg, the board opened the spying probe after the CEO acknowledged the affair. The probe touches two sensitive areas at once: whether any ties to an alleged Chinese front company compromised Nvidia&\#x27;s compliance with US semiconductor export controls, and how corporate governance works at one of the world&\#x27;s most valuable companies. Even without proof of wrongdoing, the case gives US authorities a reason to scrutinize Nvidia&\#x27;s China export-control processes. The board is investigating what happened to Huang, not investigating Huang himself — several social-media summaries misread the statement as the board targeting its own CEO. Much of the underlying reporting, including the alleged front-company link and the infidelity admission, remains unconfirmed by Nvidia beyond the short statement.

hackernews · vincentchau · Nov 8, 20:26 · [Discussion](https://news.ycombinator.com/item?id=50416801)

**Background**: US chip export controls are rules administered by the Commerce Department&\#x27;s Bureau of Industry and Security \(BIS\) that restrict which advanced AI chips and related technology can be sold to countries such as China. A &quot;front company&quot; is an entity set up to conceal who really controls it, often used by intelligence services or to disguise illicit trade; in the semiconductor world, Singapore has recently become a focus of investigations into Nvidia chips being routed to China, including a roughly $390 million smuggling case and a US probe of freight forwarder Apex Logistics. Because decisions about which chips go where are worth billions, a CEO of Huang&\#x27;s stature is a natural target for foreign intelligence services.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Front_organization">Front organization - Wikipedia</a></li>
<li><a href="https://neuralwired.com/2026/06/05/nvidia-chip-export-controls-china-2026/">Nvidia &amp; US Chip Export Controls: Complete 2026 Guide</a></li>
<li><a href="https://www.straitstimes.com/business/spore-based-apex-logistics-fully-cooperating-in-us-probe-over-alleged-smuggling-of-nvidia-chips">Apex Logistics under US probe for alleged Nvidia chip ...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters pushed back hard on the submission&\#x27;s misleading title, clarifying that Nvidia is investigating an operation against Huang rather than investigating Huang. Others explained the export-control stakes — if Huang knew the Singapore firm was really a Chinese front, that could imply complicity in evading US export controls — while several cautioned that nothing has been proven and that great-power intelligence services routinely study figures of Huang&\#x27;s consequence.

**Tags**: `#nvidia`, `#corporate-governance`, `#export-controls`, `#semiconductors`, `#geopolitics`

---

<a id="item-3"></a>
## [2.8T Kimi-K3.1-Pro-Coder compressed to 775GB via tiered quantization](https://www.reddit.com/r/LocalLLaMA/comments/1xr777l/kimik31procoder_28t_177_tb_775_gb_56_368_tps/) ⭐️ 8.0/10

A Reddit experiment applied a custom tiered quantization pipeline called Strata + dr-triton to the 2.8T-parameter Kimi-K3.1-Pro-Coder, cutting its footprint from 1.77 TB to 775 GB \(−56%\). The compressed model reportedly retained 96.7% on both AIME 2025 and LiveCodeBench while running across a single Blackwell GPU, 176 GB of RAM, and NVMe storage. This matters because a 2.8T-parameter MoE model would normally require roughly 22 80GB GPUs just to hold its weights in VRAM, so running it on one GPU plus RAM and NVMe sharply lowers the hardware barrier for local experimentation. It also offers reusable tooling and a stress test for tiered offloading and mixed-precision MoE quantization, though the setup remains experimental rather than a production-ready release. The routed MoE experts were quantized across three tiers at 2.81, 2.56, and 1.44 bits per weight \(averaging about 1.92 bpw\), while shared experts, attention, and embeddings stayed in native BF16/F32. The custom packed tensor layout means the shards cannot be dropped directly into vanilla llama.cpp or vLLM, and the measured throughput was 36.8 tok/s batch/prefill and 10.8 tok/s single-stream decode on an RTX PRO 6000 Blackwell with 176 GB RAM.

reddit · r/LocalLLaMA · /u/Grawnch · Nov 8, 19:45

**Background**: Mixture-of-Experts \(MoE\) models contain many routed expert subnetworks but activate only a small subset per token, which keeps compute lower than a dense model of the same total parameter count while still requiring enormous memory to store all weights. Quantization reduces memory by storing weights at lower precision, and &\#x27;bits per weight&\#x27; \(bpw\) describes the average storage cost; MXFP4 is a 4-bit micro-scaling format, while BF16 is a 16-bit format commonly used for higher-fidelity weights. Tiered offloading places frequently used experts in GPU VRAM, less-used ones in pinned system RAM, and the rest on NVMe, trading speed for capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2509.02512">MoPEQ: Mixture of Mixed Precision Quantized Experts Automated Fine-Grained Mixture-of-Experts Quantization GitHub - chenzx921020/MoEQuant AUTOMATED FINE-GRAINED MIXTURE-OF-EXPERTS QUANTIZATION apex-quant/paper/APEX_Technical_Report.md at main - GitHub ICLR Poster Efficient Quantization of Mixture-of-Experts with ...</a></li>
<li><a href="https://modal.com/llm-almanac/block-quants/nvidia-fp4">LLM Engineer&#x27;s Almanac - What is NVFP4? | Modal</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#quantization`, `#mixture-of-experts`, `#inference-optimization`, `#large-language-models`

---

<a id="item-4"></a>
## [Consumer Gemini quietly routes Drive and Gmail content to human reviewers](https://www.reddit.com/r/artificial/comments/1xr1o9g/consumer_gemini_autonomously_ingests_drive/) ⭐️ 8.0/10

A detailed Reddit analysis reports that Google has reversed its 2023 commitment that personal content from Gmail, Docs, and Drive connected to Gemini &quot;is not seen by human reviewers.&quot; Google now states this explicitly in the updated Help Answer 16836988 and in an October 16 edit to its original 2023 blog post, warning users not to connect apps containing confidential information they wouldn&\#x27;t want a reviewer to see. Testing described in the post shows that ingestion happens autonomously when users casually mention personal topics, without requiring @Drive or @Gmail tags. This reverses a public trust guarantee from a major AI vendor, affecting anyone who has enabled Connected Apps in consumer Gemini, including users who linked their Workspace accounts specifically because of the earlier privacy assurance. It also raises broader questions about whether assistant products can be trusted with ambient access to email and files, and is likely to draw scrutiny from regulators and enterprise buyers evaluating Google&\#x27;s AI offerings. Because LLM tool-calling and context injection are probabilistic, the same query can yield one of four outcomes: no retrieval, a metadata or generic summary, a partial unredacted quotation containing PII, or full-file ingestion into session context — so a single test showing no retrieval does not disprove the pipeline. The author also argues Google&\#x27;s regex and NER scrubbing cannot adequately de-identify narrative data such as account numbers, confirmation numbers, and transaction dates.

reddit · r/artificial · /u/tlislo · Nov 8, 15:58

**Background**: Gemini Apps can be linked to Google Workspace through &quot;Connected Apps&quot; \(formerly Workspace extensions\), which lets the model locate and incorporate data from a user&\#x27;s Gmail, Docs, and Drive when answering a request. Normally such retrieval is expected to be an explicit action, such as an @-mention of a specific file or app, but modern assistants also make autonomous tool calls based on inferred intent. Separately, AI providers commonly use sampled conversations for human review to improve quality and safety, which is why the scope of that review — and whether connected-app data is included — matters to privacy-conscious users.

<details><summary>References</summary>
<ul>
<li><a href="https://workspaceupdates.googleblog.com/2024/07/gemini-workspace-extensions-beta.html">Google Workspace Updates: Google Workspace extensions for ...</a></li>
<li><a href="https://support.google.com/gemini/answer/13695044?hl=en&amp;co=GENIE.Platform=Desktop">Use &amp; manage Connected Apps in Gemini - Computer - Gemini ...</a></li>
<li><a href="https://www.skilldrop.ai/blog/google-gemini-extensions-tools-guide">Google Gemini Extensions and Tools: The Complete 2026 Guide</a></li>

</ul>
</details>

**Tags**: `#AI privacy`, `#Google Gemini`, `#data governance`, `#LLM products`, `#trust and safety`

---

<a id="item-5"></a>
## [Dux: Open-source Wayland desktop shell adds file manager and theming](https://duxlabs.dev/) ⭐️ 7.0/10

Dux, the rebranded successor to Dank Material Shell, has released version 2.0 as a free, open-source Wayland desktop shell that now includes a file manager and theming, along with official support for atomic Linux distributions such as Bazzite. The release matters because long-term users describe Dux as polished enough to help mainstream the Niri compositor, and its official atomic-distro support removes a notable adoption gap for users of immutable Fedora-based systems. Dux is built with Quickshell and Go and is designed for Niri, Hyprland, Sway, MangoWC, labwc, Scroll, Miracle WM, and other Wayland compositors, replacing tools such as waybar, swaylock, swayidle, mako, fuzzel, and polkit with one shell. However, its curl \| sh installation method has drawn trust and distro-packaging concerns from commenters.

hackernews · indigodaddy · Nov 8, 19:08 · [Discussion](https://news.ycombinator.com/item?id=50416053)

**Background**: Wayland is the modern Linux display protocol, and a compositor such as Niri handles window management and rendering; a desktop shell supplies the panel, launcher, notifications, lock screen, and other everyday desktop pieces on top. Niri is a Rust-written scrollable-tiling compositor that arranges windows in columns on an infinite horizontal strip. Dux began as Dank Material Shell, a Quickshell- and Go-based shell intended to serve a role similar to GNOME Shell or KDE Plasma.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/duxlabs-dev/dux-shell">GitHub - duxlabs-dev/dux-shell: Desktop shell for wayland ...</a></li>
<li><a href="https://danklinux.com/docs/dankmaterialshell/overview">Overview &amp; Architecture | Dank Linux</a></li>
<li><a href="https://github.com/niri-wm/niri">GitHub - niri-wm/niri: A scrollable-tiling Wayland compositor.</a></li>

</ul>
</details>

**Discussion**: Commenters who have used it for nearly a year praise Dux/DMS as extremely slick and stable, with some saying it could help mainstream Niri. Others raise concerns about its Android-like look and the curl \| sh installer, arguing such a project should be distro-packaged and reviewed, while another user says it is becoming too all-encompassing and mentions alternatives such as Noctalia with the River-based Triad compositor.

**Tags**: `#wayland`, `#linux-desktop`, `#open-source`, `#desktop-shell`, `#niri`

---

<a id="item-6"></a>
## [Outlook.com Quietly Rejects Inbound Email From Domains Without DMARC](https://mailroute.net/blog/outlook-rejecting-email-without-dmarc) ⭐️ 7.0/10

Since November 5, Outlook.com, Hotmail and Live.com have been rejecting inbound messages from domains that publish no DMARC record, returning 550 5.7.1 bounces to senders without any public announcement from Microsoft. The change hits small senders and self-hosted mail servers hardest, since many of them have never published a DMARC policy. A single major mailbox provider turning DMARC into a hard entry requirement effectively makes the standard mandatory for anyone who wants to reach Outlook users, raising the bar for small businesses, hobbyist mail servers and transactional senders. It also reinforces a broader trend of Google, Yahoo and Microsoft tightening authentication rules and shifting deliverability power toward a handful of large platforms. The documented fix is a single DNS TXT record at \_dmarc.example.com containing something as minimal as &quot;v=DMARC1; p=none;&quot;, which declares a policy without demanding that failing mail be quarantined or rejected. Because the rejection is not accompanied by a clear public notice and the bounce is generic, senders often only discover the problem when recipients report missing mail.

hackernews · xmddmx · Nov 8, 19:20 · [Discussion](https://news.ycombinator.com/item?id=50416158)

**Background**: DMARC \(Domain-based Message Authentication, Reporting and Conformance\) is an email authentication protocol layered on top of SPF and DKIM: SPF checks whether the sending IP is authorized by the domain, DKIM cryptographically signs messages, and DMARC tells the receiving server what to do when those checks fail and where to send aggregate reports. Historically DMARC was a recommendation that improved trust and spam filtering; mailbox providers are now increasingly treating its mere presence as a precondition for accepting mail at all. Self-hosting a mail server means owning that entire chain — DNS records, reverse DNS, IP reputation and authentication — which is why small operators are the most exposed to policy shifts like this one.

<details><summary>References</summary>
<ul>
<li><a href="https://mailroute.net/blog/outlook-rejecting-email-without-dmarc">Outlook.com Is Quietly Rejecting Email From Domains Without DMARC</a></li>
<li><a href="https://en.wikipedia.org/wiki/DMARC">DMARC - Wikipedia</a></li>
<li><a href="https://tosend.com/articles/outlook-rejects-email-without-dmarc/">Outlook.com now rejects email from domains without DMARC</a></li>

</ul>
</details>

**Discussion**: Commenters are split: some welcome strict DMARC enforcement as long overdue and blame late adopters for being lazy, while self-hosters describe years of Outlook silently dropping legitimate mail even with SPF, DKIM and DMARC correctly configured. Others complain that Microsoft&\#x27;s non-public blocklists make appeals essentially impossible, and a few argue the episode shows email&\#x27;s bolted-on security model is beyond patching and should be replaced outright.

**Tags**: `#email`, `#dmarc`, `#deliverability`, `#self-hosting`, `#infrastructure`

---

<a id="item-7"></a>
## [Developer switches from Claude to Pi coding agent harness](https://caleb.software/posts/claude-to-pi.html) ⭐️ 7.0/10

A developer published a post titled “Goodbye Claude, hello Pi” describing a switch from Anthropic’s Claude coding agent to Pi, an open-source, minimal coding-agent harness; the Hacker News submission drew 675 points and 424 comments. The discussion shows that harness design can matter as much as the underlying model for coding-agent performance, and that choosing a third-party harness is now entangled with subscription terms-of-service risk. It affects developers who pay for Claude or Codex subscriptions and highlights growing competition among agent harnesses. Commenters describe Pi as a minimal, token-efficient harness with a small system prompt and customizability, but warn that using Anthropic subscription models through it may risk account bans and that Claude’s native harness relies on custom headers, hidden flags, and undocumented API features that shape model behavior. Users also report that heavy multi-project use pushes them toward GUI desktop apps over terminal UIs for cleaner history and richer text.

hackernews · karagenit · Nov 8, 03:11 · [Discussion](https://news.ycombinator.com/item?id=50410107)

**Background**: An agent harness is the software layer around an LLM that supplies prompts, tools, memory, and orchestration, which is why the same model can behave differently in different coding agents. Pi is an open-source, terminal-based harness designed to be minimal and extensible, while Claude is Anthropic’s subscription-based assistant and coding agent. As developers seek more control and lower costs, swapping harnesses has become common, raising questions about terms of service and native-harness behavior.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness - Wikipedia</a></li>
<li><a href="https://github.com/earendil-works/pi">GitHub - earendil-works/ pi : AI agent toolkit: unified LLM API, agent ...</a></li>
<li><a href="https://theagentwire.ai/p/mm-8-anthropic-openclaw-ban-ai-agents-more-expensive">MM-8 — Anthropic Just Raised My Rent</a></li>

</ul>
</details>

**Discussion**: The overall sentiment is positive toward Pi and alternative harnesses, with some users calling Pi the best harness because it gives them full control and reduces frustration. At the same time, experienced commenters caution that Anthropic subscription models are risky to use outside Claude’s native harness due to possible ToS enforcement, missing custom headers and undocumented API behavior, and weaker compaction. A separate thread of discussion favors GUI clients over TUIs for managing many long-running sessions and cleaner history.

**Tags**: `#AI coding agents`, `#LLM tooling`, `#Anthropic Claude`, `#developer tools`, `#Hacker News discussion`

---

<a id="item-8"></a>
## [C vs Rust: Benchmarking a parse\_number\(\) SQLite Extension](https://simonwillison.net/2026/Nov/8/sqlite-parse-number-c-vs-rust/) ⭐️ 7.0/10

Simon Willison published a research report comparing a parse\_number\(\) SQLite loadable extension written in C versus the same function implemented in Rust, all generated through Claude chat sessions \(Opus 5.5\). The first C version was only 14 KB versus 321 KB with Rusqlite and 298 KB with sqlite-loadable-rs, but Rust was initially faster; after prompting Claude to hand-write a faster C number parser, the new C version dropped to 19 ns per row on mixed data versus 46 ns for Rusqlite and 41 ns for sqlite-loadable-rs. For developers writing SQLite extensions, this is a concrete data point on the trade-off between Rust&\#x27;s safety and tooling versus C&\#x27;s tiny binaries and, with careful tuning, superior raw speed. It also illustrates a workflow where an LLM drafts competing implementations, benchmarks them, and then iterates on the slow one until it wins. The benchmarks measure net cost per row over 2 million rows: the original C version took 67 ns on mixed data, 25 ns on integers and 106 ns on decimals, while the rewritten C version reached 19/16/18 ns, beating both Rust frameworks in every category. The initial Rust advantage came from Rust&\#x27;s equivalent of C&\#x27;s strtod being roughly twice as fast, which the hand-rolled C parser then overtook.

rss · Simon Willison · Nov 8, 22:26

**Background**: SQLite supports run-time loadable extensions, which are shared libraries \(.so files\) compiled against the SQLite C API that register new scalar functions, virtual tables, or file systems when loaded. Custom scalar functions are typically registered with the sqlite3\_create\_function\(\) family of interfaces; the Rust wrappers rusqlite and sqlite-loadable-rs wrap these same C APIs, which is why they add binary size and some call overhead. Writing an extension in C keeps the binary minimal, but pushing maximum speed often requires replacing the standard library&\#x27;s strtod parsing routine with a purpose-built parser.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Nov/8/sqlite-parse-number-c-vs-rust/">Research: parse_number () as a SQLite extension: C vs Rust</a></li>
<li><a href="https://github.com/asg017/sqlite-loadable-rs">GitHub - asg017/sqlite-loadable-rs: A framework for writing ...</a></li>
<li><a href="https://sqlite.org/appfunc.html">Application-Defined SQL Functions - SQLite</a></li>

</ul>
</details>

**Tags**: `#SQLite`, `#Rust`, `#C`, `#extensions`, `#performance`

---

<a id="item-9"></a>
## [Nace releases Drex Max v1.1 multimodal decision model with open weights](https://www.reddit.com/r/MachineLearning/comments/1xr4hkm/artificial_analysis_multimodal_decision_model/) ⭐️ 7.0/10

Nace announced Drex Max v1.1, which it claims reaches state-of-the-art performance and sits on the Pareto frontier for decision models on the Artificial Analysis leaderboard. The company released Drex Max v1 weights on Hugging Face under an Open RAIL-M license, published a training paper titled &quot;Towards Foundation Decision Models: Drex&quot; \(arXiv 2611.07854\), and said v1.1 open weights are coming soon once local-inference optimization is finished. Decision models are an emerging category where most competitors are closed, so a release that pairs open weights with a public training playbook and a custom local inference engine gives researchers a reproducible baseline to build on. If Nace&\#x27;s cost claim holds, an 8x cheaper open model could pressure pricing across the category and make decision-model workloads viable for smaller teams. The model supports roughly a 256k context window, versus 64k for Glide1.2 and 16k for Mammoth, matching pplxdecider&\#x27;s 256k, and can run locally on a Mac via Nace&\#x27;s Kapitsa inference engine. Caveats worth noting: only v1 weights are actually downloadable today, the v1.1 release is still pending, and the SOTA and Pareto-frontier claims come from the company itself.

reddit · r/MachineLearning · /u/m4rkGS · Nov 8, 17:54

**Background**: A &quot;decision model&quot; is a model that outputs an action or choice rather than free-form text, and the category is being tracked by independent benchmark sites such as Artificial Analysis, which ranks models on quality-versus-cost trade-offs; models on the &quot;Pareto frontier&quot; are those that no other model beats on both axes simultaneously. Kapitsa, mentioned in the announcement, is Nace&\#x27;s inference engine for Apple Silicon that runs models such as Qwen and Nemotron locally and exposes OpenAI- and Anthropic-compatible APIs. Open RAIL-M is a Responsible AI License that allows commercial use but attaches behavioral use restrictions to the model and its derivatives.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/nace-ai/kapitsa">Apple Silicon Inference Engine: Kapitsa - GitHub</a></li>
<li><a href="https://www.licenses.ai/ai-licenses">AI Licenses — Responsible AI Licenses ( RAIL )</a></li>

</ul>
</details>

**Tags**: `#multimodal-models`, `#decision-models`, `#open-weights`, `#model-release`, `#llm-inference`

---

<a id="item-10"></a>
## [Hobbyist Trains Playable Diffusion World Model of Pokémon Red With System 1/2 Agent Harness](https://www.reddit.com/r/MachineLearning/comments/1xqt0pk/i_trained_a_playable_diffusion_world_model_of/) ⭐️ 7.0/10

A developer trained a 16.7M-parameter DIAMOND-style EDM U-Net diffusion world model that renders the next 72×80 greyscale frame of Pokémon Red from the last four screens plus a button press, letting a player walk around inside the generated &quot;dream.&quot; The model was paired with a System 1/System 2 agent harness modeled on Krafton&\#x27;s PUBG Ally, where a RAM-reading planner picks goals and ten 1.58M-parameter executor policies do the walking, all trained for a total of 50 GPU-hours on a single RTX 4090. It is a concrete, fully open demonstration that a home-scale diffusion world model can be played interactively and, more importantly, serve as an imagination-only training ground whose policies transfer to the real game — the executor policies win the first gym badge in 30 out of 30 real runs despite never taking a real-game step. This speaks directly to world-model reinforcement learning and to the System 1/System 2 agent design that commercial AI teammates like PUBG Ally are built on. The world model runs autonomously but re-syncs on four real frames every 10 steps, and battles remain scripted because the dream tends to end battles early; two extra tiny nets \(a 0.72M-parameter upsampler and a 1.91M-parameter colorizer with 99.27% accuracy on held-out frames\) make the tiny greyscale output watchable, each trained in about 25 minutes. The author reports no benchmarks, baselines, or ablations, and the best local LLM planner needed a median 7,144.5 button presses versus 8,779.5 for hand-written rules — so the evaluation evidence is anecdotal rather than comparative.

reddit · r/MachineLearning · /u/priyanshu123sah · Nov 8, 07:48

**Background**: DIAMOND \(DIffusion As a Model Of eNvironment Dreams\), a NeurIPS 2024 spotlight, models the next frame as a continuous pixel-space diffusion process conditioned on stacked past frames and past actions, which lets an RL agent be trained entirely inside the generated environment. Krafton&\#x27;s PUBG Ally, an AI teammate for PUBG: BATTLEGROUNDS, uses a System 1/System 2 split: a fast reactive layer plus a slow language-model planner operating through a bounded tool interface. ICLR workshops are smaller satellite venues with later deadlines and shorter-format papers, often used to showcase promising early-stage or applied work.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/eloialonso/diamond">GitHub - eloialonso/diamond: DIAMOND (DIffusion As a Model Of ...</a></li>
<li><a href="https://www.krafton.ai/blog/pubg_ally_nemotron/">From Workflow-Based SLM to Autonomous Agent: Evolving PUBG ...</a></li>
<li><a href="https://arxiv.org/html/2609.29837v1">PUBG Ally: A Conversational Embodied Agent as an AI Teammate</a></li>

</ul>
</details>

**Tags**: `#diffusion-models`, `#world-models`, `#game-ai`, `#llm-agents`, `#reinforcement-learning`

---

<a id="item-11"></a>
## [Open-source tool maps LLM answers on censorship by country](https://www.reddit.com/r/LocalLLaMA/comments/1xr09nq/does_censorship_exist_in_country_according_to/) ⭐️ 7.0/10

Developer p-e-w published llm-beliefs, a small open-source program that asks a language model the same Yes/No question about censorship for every country and renders the answers as an SVG world map, and said the results surprised him. The project turns a much-debated issue — how LLMs answer politically sensitive questions differently depending on the country involved — into a reproducible, visual experiment, giving the LocalLLaMA community a concrete artifact for arguing about alignment bias and geographic inconsistency in model behavior. The probe is a single Yes/No question per country, so the resulting map reflects prompt phrasing, query language and training-data artifacts as much as any real-world condition; it is a lightweight visualization rather than a controlled benchmark, and maps are published in the repo under maps/.

reddit · r/LocalLLaMA · /u/-p-e-w- · Nov 8, 14:56

**Background**: Large language models absorb geopolitical and cultural viewpoints from their training corpora, so their answers on politically sensitive topics can vary by country and by the language used to ask. Prior research \(such as ACL 2025 work on geopolitical and cultural bias\) separates &quot;model bias&quot; baked in during training from &quot;inference bias&quot; induced by the language of the query, which is exactly the kind of effect a per-country yes/no probe can surface.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/p-e-w/llm-beliefs/tree/master/maps">llm-beliefs/maps at master · p-e-w/llm-beliefs · GitHub</a></li>
<li><a href="https://aclanthology.org/2025.acl-srw.38/">A Dual-Layered Evaluation of Geopolitical and Cultural Bias ...</a></li>

</ul>
</details>

**Tags**: `#llm-bias`, `#censorship`, `#model-evaluation`, `#visualization`, `#open-source`

---

<a id="item-12"></a>
## [Tencent Releases DSpine Draft Model Promising 3x Faster Decoding for Qwen3.8-27B](https://www.reddit.com/r/LocalLLaMA/comments/1xr2aaa/tencentqwen3827bdspineb16_hugging_face/) ⭐️ 7.0/10

Tencent published a Hugging Face checkpoint named tencent/Qwen3.8-27B-DSpine-b16, a five-layer DSpine draft model built to accelerate speculative decoding for Qwen3.8-27B, with block size 16 and an 8,192-token sliding window. A post on r/LocalLLaMA highlights the release as reportedly delivering roughly 3x faster decoding for 27B-class models. Speculative decoding is one of the few inference optimizations that speeds up generation without degrading output quality, so a working 3x decode speedup on a 27B model directly affects latency and cost for anyone self-hosting large models. It is also notable that Tencent is shipping an optimized drafter for Qwen, a model family from Alibaba, signaling that acceleration checkpoints are becoming reusable cross-lab artifacts rather than lab-internal tricks. DSpine drafts in parallel: at every draft layer each position receives the predicted feature of its predecessor, so the causal chain unfolds over network depth while all positions are still drafted in a single backbone pass, which avoids the inconsistent continuations that hurt acceptance length in naive parallel drafting. The checkpoint is only a five-layer drafter with block size 16 and an 8,192-token sliding window, meaning it must be paired with the matching Qwen3.8-27B target model, and community GGUF conversions are already appearing for llama.cpp users.

reddit · r/LocalLLaMA · /u/emdeka87 · Nov 8, 16:23

**Background**: Speculative decoding pairs a small, fast draft model with the large target model: the drafter proposes several tokens ahead, and the target model verifies them in parallel, accepting those that match its own predictions. Because only the accepted tokens cost a full forward pass and rejected ones are discarded, output is identical to normal decoding while wall-clock latency drops. Classic draft-model approaches are inherently sequential, so newer methods such as EAGLE and now DSpine \(Draft in Parallel, Condition Through Depth\) try to generate multiple draft candidates in a single backbone pass to push acceptance rates and speedups higher.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/tencent/Qwen3.8-27B-DSpine-b16">tencent/ Qwen 3 . 8 - 27 B - DSpine - b 16 · Hugging Face</a></li>
<li><a href="https://github.com/tencent/dspine/">GitHub - Tencent/DSpine</a></li>
<li><a href="https://handbook.modular.com/inference-optimization/speculative-decoding/">Speculative decoding | LLM Inference Handbook</a></li>

</ul>
</details>

**Tags**: `#speculative decoding`, `#LLM inference`, `#Tencent`, `#Qwen`, `#optimization`

---

<a id="item-13"></a>
## [Intel Arc Pro B70 32GB hits ~half RTX 5090 speed for one-fifth the price on Qwen3-27B](https://www.reddit.com/r/LocalLLaMA/comments/1xr78s5/intel_arc_pro_b70_32gb_1299_vs_nvidia_rtx_5090/) ⭐️ 7.0/10

A user on r/LocalLLaMA benchmarked a $1,299 32GB Intel Arc Pro B70 \(bought from ASRock&\#x27;s official Amazon store\) against an RTX 5090 selling for $6,550+ on Newegg, running Qwen3.8-27B at Q6 quantization with a ~3k-token prompt and MTP enabled. After tuning, the Intel card reached ~960 tok/s prefill and ~52 tok/s generation versus ~2,830 tok/s and ~98 tok/s for the RTX 5090 — roughly half the generation speed and one-third the prefill speed at about one-fifth the price \($41/GB vs $200+/GB of VRAM\). Local LLM buyers have been stuck paying steep NVIDIA premiums for large-VRAM cards, so first-hand price/performance data on non-NVIDIA alternatives directly informs hardware purchasing decisions. The post also documents the specific software stack needed to make an Intel Arc card usable, which fills a documentation gap that has kept many hobbyists and small studios on CUDA. The card is reportedly poor out of the box — base ollama on Ubuntu 24.04&\#x27;s Mesa 25.2 managed only 137 tok/s prefill and 6.8 tok/s generation at 16k context — and required kernel 6.17+, Resizable BAR with CSM disabled, Intel&\#x27;s compute runtime PPA and Mesa 26.x to become competitive. On Vulkan, quantized KV caches \(q8\_0/q4\_0\) cause severe generation slowdowns, so the author recommends building llama.cpp with SYCL to use q8\_0 KV cache and \`--spec-type draft-mtp --spec-draft-n-max 4\`; the 5090 figures come from other users&\#x27; Hugging Face posts, not the author&\#x27;s own machine.

reddit · r/LocalLLaMA · /u/maikerukonare · Nov 8, 19:46

**Background**: Local LLM inference splits into two phases: prefill, where the model ingests the whole prompt and builds the KV cache \(compute-bound and slow for long prompts\), and generation/decode, where tokens are produced one at a time \(memory-bandwidth-bound\). Multi-token prediction \(MTP\) uses built-in prediction heads in compatible models to draft several future tokens at once, speeding up generation. The Intel Arc Pro B70 is a workstation GPU with 32GB of GDDR6 on a 256-bit memory interface and a 230W TDP, positioning it as a high-VRAM alternative to consumer NVIDIA cards for workloads that need capacity more than raw speed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.intel.com/content/www/us/en/products/sku/245797/intel-arc-pro-b70-graphics/specifications.html">Intel® Arc™ Pro B70 Graphics Specifications</a></li>
<li><a href="https://www.techpowerup.com/gpu-specs/arc-pro-b70.c4388">Intel Arc Pro B70 Specs | TechPowerUp GPU Database</a></li>
<li><a href="https://www.datacamp.com/tutorial/how-llm-inference-works">How LLM Inference Works: A Practical Guide to Serving... | DataCamp</a></li>

</ul>
</details>

**Tags**: `#local-llm-inference`, `#gpu-hardware`, `#intel-arc`, `#price-performance`, `#benchmarks`

---

<a id="item-14"></a>
## [Fine-tuned Qwen3.5-0.8B turns English into bash, beats larger stock models](https://www.reddit.com/r/LocalLLaMA/comments/1xr0ykk/i_finetuned_qwen3508b_to_turn_plain_english_into/) ⭐️ 7.0/10

A developer released dale, an offline terminal helper built by fine-tuning Qwen3.5 models from 0.8B to 9B to convert natural-language requests into bash commands. On 471 held-out English and Spanish requests, the 529 MB dale-0.8b running on CPU scored 79.4% versus 62.8% for stock Qwen3.5-9B and 14.9% for stock Qwen3.5-0.8B. The result shows that a carefully fine-tuned sub-1B model can outperform much larger prompt-only models on a narrow command-generation task, while remaining fast enough for CPU-only laptops. That has practical implications for offline developer tools and edge deployments, where latency, privacy, and binary size matter more than broad general capability. On a 2020 laptop without a GPU, the 0.8B model answers in a median 1.7 s, and a deterministic risk checker labels each command safe, caution, or danger before anything runs. The author also reports that adding about 9k requests matching the longer, stacked-constraint test style raised the 0.8B from 348 to 375 correct \(p=0.001\), while cautioning that baselines are untuned 8-shot prompted models and the synthetic test is judged by two LLMs.

reddit · r/LocalLLaMA · /u/AlternativeEnough352 · Nov 8, 15:26

**Background**: Qwen3.5-0.8B is the smallest model in Alibaba Cloud&\#x27;s Qwen3.5 small-model series, which also includes 2B, 4B, and 9B variants aimed at local and edge deployment. llama.cpp is a C++ inference engine for running LLMs locally, and GGUF is its model file format; Q4\_K\_M is a 4-bit quantization recipe that shrinks weights with modest quality loss. Fine-tuning adapts a pretrained model to a specific task, while DPO and distillation are alternative training methods the author tried when the small model plateaued.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.5-0.8B">Qwen/Qwen3.5-0.8B · Hugging Face</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/blob/master/tools/quantize/README.md">llama.cpp/tools/quantize/README.md at master · ggml ... - GitHub</a></li>
<li><a href="https://apidog.com/blog/use-qwen-3-5-small-models/">How to Use Qwen 3.5 Small Model Series - apidog.com</a></li>

</ul>
</details>

**Tags**: `#local LLMs`, `#fine-tuning`, `#code generation`, `#shell/bash`, `#small language models`

---

<a id="item-15"></a>
## [PyTorch 2.7.1 and Native CUDA Mamba-1 Ported to Legacy NVIDIA GPUs](https://www.reddit.com/r/LocalLLaMA/comments/1xr97iz/resurrecting_2013_ewaste_native_cuda_mamba1/) ⭐️ 7.0/10

Developer theIvanR released four repositories — torch-on-clunkers, conv-on-clunkers, mamba-on-clunkers, and nccl-on-windows — that bring a modern LLM training stack to legacy NVIDIA GPUs spanning SM 3.5 through SM 7.5. The port includes a custom PyTorch 2.7.1 build compiled with CUDA 11.8 that retains legacy SASS, causal-conv1d v1.7.0, Mamba-1 with pure native CUDA kernels, and a Windows NCCL backend for multi-GPU DDP training, with Mamba-1 verified on a 2013 Tesla K40c at a maximum absolute error of 3.8e-06 against the PyTorch reference. Modern AI frameworks routinely drop support for older GPU architectures, so this project can extend the usable life of Kepler, Maxwell, Pascal, and Turing cards that would otherwise be e-waste or landfill. It also opens a cheap path to real multi-GPU LLM training experiments for hobbyists and resource-constrained researchers who only have second-hand hardware. Mamba-2 and Mamba-3 depend on Triton and TileLang, so they only run natively on Turing \(SM 7.5\) and newer; on older cards the package detects the missing modules and automatically falls back to the pure-CUDA Mamba-1 implementation. Local testing has so far been limited to Kepler, and the author is explicitly asking for Maxwell and Pascal benchmark and profiling reports from the community.

reddit · r/LocalLLaMA · /u/TheSpicyBoi123 · Nov 8, 21:09

**Background**: Mamba is a sequence-modeling architecture based on selective state space models \(SSMs\), introduced by Albert Gu and Tri Dao in late 2023, that scales linearly rather than quadratically with sequence length like Transformer attention. causal-conv1d is a small CUDA kernel implementing depthwise causal convolution, a component Mamba relies on for its local mixing. SASS is the compiled machine code actually executed by NVIDIA GPUs, and CUDA 11.8 was the last toolkit release to retain Kepler-era support, which is why a custom PyTorch build is needed. NCCL is NVIDIA&\#x27;s collective-communication library that PyTorch&\#x27;s DistributedDataParallel \(DDP\) uses to synchronize gradients across multiple GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mamba_%28deep_learning_architecture%29">Mamba (deep learning architecture) - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2312.00752">[2312.00752] Mamba: Linear-Time Sequence Modeling with ... What Is a Mamba Model? Complete Guide to SSM Architecture What is a Mamba model? - IBM state-spaces/mamba | DeepWiki State Space Models and Mamba | LLM Learning</a></li>
<li><a href="https://github.com/Dao-AILab/causal-conv1d">Dao-AILab/ causal - conv 1 d : Causal depthwise conv 1 d in CUDA , with...</a></li>

</ul>
</details>

**Tags**: `#CUDA`, `#Mamba`, `#Legacy GPUs`, `#PyTorch`, `#LLM Training`

---

<a id="item-16"></a>
## [r/LocalLLaMA asks what local models are actually useful for](https://www.reddit.com/r/LocalLLaMA/comments/1xr4iv0/what_are_people_finding_local_models_actually/) ⭐️ 7.0/10

A Reddit post by u/prestodigitarium in r/LocalLLaMA asks practitioners to share concretely what they use locally hosted LLMs for, seeding the thread with his own setup: DeepSeek V4.1 Flash 1017 served through Fraser Price&\#x27;s BRRR recipe on 4x RTX PRO 6000 Blackwells, reaching roughly 550 tokens/sec at concurrency 1 and a couple thousand at c=16. He lists live use cases including local &quot;scout&quot; web-research agents called by frontier models, &quot;mason&quot; sub-agents that build code stubs specified by a frontier model, a Hacker News/YouTube news filter, an events crawler that emails a weekly top-10, a terminal-and-browser activity summarizer, and local speech-to-text. The thread pushes the local-LLM conversation past benchmark tables toward reproducible real-world workflows, and the described orchestration pattern—frontier models delegating cheap, high-volume subtasks to local models—can meaningfully cut API token spend while keeping latency low. It matters for self-hosters deciding whether their GPU investment pays off, and for agent builders looking for ways to split work between expensive cloud models and owned hardware. The throughput numbers are self-reported and specific to the BRRR recipe, which layers fused decode kernels, speculative decoding, and SSD ngram offload on top of the b12x base image and is tuned primarily for single-stream code-generation decode speed. The author also admits the setup is bottlenecked by his own involvement, and that repeated attempts at a more autonomous &quot;software factory&quot; have not yet produced anything compelling.

reddit · r/LocalLLaMA · /u/prestodigitarium · Nov 8, 17:56

**Background**: Local LLMs are open-weight models run on your own hardware instead of a vendor API; DeepSeek V4.1 Flash 1017 is an MIT-licensed model with a very large context window that can be self-hosted on sufficiently large GPU setups. The RTX PRO 6000 Blackwell is a 96 GB workstation GPU, and four of them are what makes hosting a model of this size feasible. In the agent orchestration pattern described, a frontier API model acts as planner and calls the local model for sub-tasks, while figures like &quot;c=1&quot; and &quot;c=16&quot; refer to the number of simultaneous requests being served and tokens per second \(tps\) measures generation throughput.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/fraserprice/DeepSeek-4.1-Flash-1017-BRRR">DeepSeek-4.1-Flash-1017-BRRR - GitHub</a></li>
<li><a href="https://theddari.com/en/learn/deepseek-v4-1-flash-1017-api-local-guide">DeepSeek V4.1 Flash 1017: Specs, API Pricing, Local Setup</a></li>
<li><a href="https://llmconfigurator.com/en/gpu/rtx-pro-6000-blackwell">RTX PRO 6000 Blackwell: Tokens per Second &amp; 96 GB VRAM</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#llm-agents`, `#self-hosting`, `#inference-throughput`, `#community-discussion`

---

<a id="item-17"></a>
## [Sem86: An x86 Full-System Emulator With Runtime-Loaded Instruction Semantics](https://www.reddit.com/r/programming/comments/1xr4v4f/sem86_a_fullsystem_emulator_without_hardcoded/) ⭐️ 7.0/10

A Reddit r/programming post highlights Sem86, an x86 full-system emulator that contains no hard-coded instruction semantics and instead loads them at runtime from an input file, making it trivial to switch between different semantics. The work is documented in a paper \(QRS26\) and a public GitHub repository under the libLISA project. x86 does not define a single behavior for every instruction and operand combination, so an emulator that bakes in one fixed semantics cannot faithfully reproduce CPU-specific quirks or undocumented instructions. Turning semantics into swappable data could let researchers plug in formally derived or machine-synthesized models, which matters for reverse engineering, malware analysis, and verification of x86 binaries. Instruction semantics are encoded in a simple format that can be converted to and from SMT-LIB, and the project&\#x27;s stated motivation is accurately emulating undefined behavior and undocumented instructions, with automatic generation of semantics listed as a long-term goal. The related-work discussion notes that emulators such as Bochs and QEMU do not aim to accurately implement undefined behavior, which is precisely the gap Sem86 targets.

reddit · r/programming · /u/mttd · Nov 8, 18:09

**Background**: An emulator must know what every machine instruction does, and this knowledge — the instruction semantics — is normally written directly into the emulator&\#x27;s source code. That approach is awkward on x86, where some instruction and operand combinations are officially undefined, so real CPUs from different vendors or generations can produce different results for the same code. SMT-LIB is a standard, solver-agnostic format used by formal verification and symbolic execution tools, which makes it a natural interchange format for machine-readable semantics. Sem86 comes out of the libLISA research project and packages these ideas as a runnable full-system emulator rather than a purely theoretical model.

<details><summary>References</summary>
<ul>
<li><a href="https://ssrg.ece.vt.edu/papers/qrs26-sem86.pdf">Sem86: A Full-System Emulator Without Hard-Coded Semantics</a></li>
<li><a href="https://github.com/libLISA/sem86">Sem86 - A full-system x86 emulator without hardcoded semantics</a></li>
<li><a href="https://liblisa.nl/publications/sem86-qrs26/02-related-work/">Related Work - Sem 86 : A Full - System Emulator Without Hard-Coded...</a></li>

</ul>
</details>

**Tags**: `#emulation`, `#systems`, `#formal-semantics`, `#x86`, `#programming`

---

<a id="item-18"></a>
## [C64 Demoscener Explains Bumpmapped Rain Effect in Lunatico](https://www.reddit.com/r/programming/comments/1xrbciy/c64_demo_effect_explained_the_bumpmapped_rain_in/) ⭐️ 7.0/10

Linus Åkesson, the programmer behind the Commodore 64 demo Lunatico released in 2016, has published an explanation and video walking through how the demo&\#x27;s bumpmapped rain effect was implemented. The write-up and video detail the inner workings of an effect that appears trivial on modern hardware but is highly demanding on a stock C64. It offers a rare, code-level look at how demoscene programmers achieve modern-looking visuals on hardware with roughly a 1 MHz CPU and no framebuffer, making it valuable to retrocomputing, demoscene, and graphics-programming audiences. Such explanations preserve and spread optimization techniques that are otherwise locked inside binaries and hard to learn from. Lunatico was released on 30 October 2016 and took second place in the C64 demo competition at the X&\#x27;2016 demoparty, with code, graphics, and music all by Lft. The explanation focuses specifically on the rain effect&\#x27;s implementation on stock hardware rather than on accelerated or expanded C64 configurations.

reddit · r/programming · /u/jailbird · Nov 8, 22:43

**Background**: The Commodore 64, released in 1982, runs a 6510 CPU at about 1 MHz with 64 KB of RAM and displays graphics through the VIC-II chip, which has no linear framebuffer and imposes tight character-cell and color limitations. Bump mapping is a per-pixel lighting technique normally associated with far more powerful machines, so recreating it on a C64 requires extreme trickery and cycle-level optimization. The demoscene is a subculture devoted to pushing such vintage hardware beyond its documented limits, and Lunatico is a well-known example of that craft.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linusakesson.net/scene/lunatico/rain.php">Rain Effect Explained - linusakesson.net</a></li>
<li><a href="https://csdb.dk/release/?id=151273">[CSDb] - Lunatico by Lft (2016) - Commodore 64 Scene Database</a></li>
<li><a href="https://en.wikipedia.org/wiki/Commodore_64_demos">Commodore 64 demos - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Commodore 64`, `#Demoscene`, `#Retrocomputing`, `#Graphics Programming`, `#Optimization`

---

<a id="item-19"></a>
## [Stroustrup presents C++ profiles for simplicity and safety guarantees](https://www.reddit.com/r/programming/comments/1xqs5vb/profiles_for_simplicity_and_guarantees_bjarne/) ⭐️ 7.0/10

Bjarne Stroustrup presents C++ profiles as a language mechanism for improving simplicity and providing stronger safety guarantees in C++. The linked talk/article frames profiles as a way to address long-standing C++ safety and complexity concerns. This matters because C++ faces persistent criticism over memory safety and complexity, and profiles could offer a standardized, incrementally adoptable path to safer code without abandoning existing codebases. The work affects C++ developers, compiler and toolchain vendors, and the ISO C++ standardization community. Profiles are envisioned as named sets of guarantees plus detailed rules, with the C++ Core Guidelines serving as an initial proving ground; the approach emphasizes gradual adoption, incremental improvements to guarantees, and portability of guarantees across toolchains.

reddit · r/programming · /u/\_telesis · Nov 8, 06:53

**Background**: C++ profiles are a proposed language-level framework for bundling safety and style rules into enforceable profiles. The idea responds to growing pressure for memory safety in systems programming languages and to C++&\#x27;s reputation for complexity. Rather than replacing C++, profiles aim to let developers opt into stricter guarantees over time.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/BjarneStroustrup/profiles">GitHub - BjarneStroustrup/profiles: site for discussing ...</a></li>
<li><a href="https://cpp-profiles.org/">C++ Profiles: language-level safety</a></li>
<li><a href="https://www.open-std.org/jtc1/sc22/wg21/docs/papers/2025/p3589r2.pdf">C++ Profiles: The Framework - open-std.org</a></li>

</ul>
</details>

**Tags**: `#C++`, `#programming languages`, `#software safety`, `#language design`, `#Bjarne Stroustrup`

---

<a id="item-20"></a>
## [Spectre: design-by-contract language with allocator-centric API claims up to 6x faster than Zig](https://www.reddit.com/r/programming/comments/1xraxrk/spectre_a_designbycontract_language_with_an/) ⭐️ 7.0/10

A Reddit post on r/programming introduced Spectre, a statically typed, design-by-contract programming language that pairs language-level contract semantics with an explicit, allocator-centric API for memory management. The submission claims Spectre outperforms Zig by up to 6x on general-purpose benchmarks, though the post itself contains only a title and link with no benchmark methodology or source code. If the performance claims hold up, Spectre would show that language-level contract checking and low-level manual memory control can coexist without a garbage collector, an unusual combination that could interest systems programmers currently choosing between Zig, Rust, and C++. It also adds a new entrant to the small but growing group of languages competing on explicit allocator APIs and compile-time safety guarantees. Spectre is described as having no garbage collector, instead using a custom-allocator-based approach to memory management with ownership semantics, and it is statically typed. The 6x figure against Zig comes from a single Reddit headline with no published benchmark harness, hardware details, or reproducibility instructions, so the comparison should be treated as an unverified vendor-style claim rather than a measured result.

reddit · r/programming · /u/Top\_Marionberry\_4413 · Nov 8, 22:24

**Background**: Design by contract is a software design approach in which functions declare preconditions, postconditions, and invariants that the compiler or runtime can check, making responsibilities between caller and callee explicit. An allocator-centric API means heap allocation is never implicit: functions receive allocator handles explicitly and pass them down the call stack, a style popularized by Zig, which forces programmers to reason about every allocation and makes memory use visible in type signatures. Zig itself is a low-level systems language known for manual memory management, comptime metaprogramming, and C interoperability, so it is a natural baseline for a new language making performance claims in this space.

<details><summary>References</summary>
<ul>
<li><a href="https://spectrelang.org/">Spectre Programming Language</a></li>
<li><a href="https://dev.to/navidm/spectre-programming-language-39ff">Spectre Programming Language - DEV Community</a></li>
<li><a href="https://en.wikipedia.org/wiki/Design_by_contract">Design by contract - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#programming languages`, `#performance`, `#Zig`, `#memory allocation`, `#design-by-contract`

---

<a id="item-21"></a>
## [GPT-6 Astra edits 0.016% of Qwen weights, critics dispute framing](https://www.reddit.com/r/artificial/comments/1xr8gei/mit_csail_gpt6_astra_edited_0016_of_a_small_qwen/) ⭐️ 7.0/10

MIT CSAIL researchers \(Rikiya Takehi, Jayden Teoh, Alex Zhang and Omar Khattab\) published &quot;Sparks of Weight-Space Programming&quot; on Nov 2, reporting that GPT-6 Astra was given the raw weights of Alibaba&\#x27;s Qwen3.5-0.8B plus a Python environment and traced its math-problem looping to a single direction in the MLPs of layers 15 and 19, subtracting it from 64 output columns in each layer. That changed 131,072 weights \(0.016% of the total\) with no training run or gradient descent, lifting MATH-500 accuracy from 7.9% to 48.1%. If the result holds, it suggests an LLM can maintain another model at the weight level — diagnosing and patching a behavioral bug the way a programmer patches source code — which would point to a new workflow sitting between interpretability probing and conventional fine-tuning. Hugging Face&\#x27;s Ahsen Khaliq independently rebuilt the edited checkpoint from the published logs and scored 51.0%, giving the claim early external support. The pushback came within a day: spaCy creator Matthew Honnibal called the write-up &quot;massively misleading&quot; because the &quot;raw weights, no tools&quot; setup only applied to tiny networks of 17k–172k weights, while every real-language-model experiment used Python and the Qwen run could also test the model on up to 50 batches of practice problems. The work is a blog post with logs rather than a peer-reviewed paper, and the authors themselves describe the results as &quot;exciting but still limited&quot;, citing context length and tooling as constraints.

reddit · r/artificial · /u/winer666 · Nov 8, 20:36

**Background**: Weight-space programming is the idea that a model can read and directly rewrite another model&\#x27;s parameters instead of only prompting it or retraining it. The edits here resemble activation steering — a known technique where a direction in a model&\#x27;s internal representations is identified and added or subtracted to shift behavior — except the intervention is baked into the weights themselves rather than applied at inference time. Qwen3.5-0.8B is Alibaba&\#x27;s ultra-compact 0.8B-parameter multimodal model aimed at edge deployment, and MATH-500 is a widely used 500-problem curated subset of the MATH competition benchmark that serves as a standard test of step-by-step mathematical reasoning.

<details><summary>References</summary>
<ul>
<li><a href="https://rikiyat.github.io/blog/weight-space-programming/">Sparks of Weight - Space Programming : LLMs can natively read...</a></li>
<li><a href="https://huggingface.co/prithivMLmods/Qwen3.5-0.8B-weight-space-programming-GGUF">prithivMLmods/Qwen3.5-0.8B- weight - space - programming -GGUF...</a></li>
<li><a href="https://explainx.ai/blog/weight-space-programming-gpt-6-astra-edits-qwen3-5-0-8b-weights-math-7-9-to-48-1-mit-csail-2026">GPT-6 Astra Edits Qwen Weights : MATH-500 7.9% to... | explainx.ai</a></li>

</ul>
</details>

**Discussion**: Commenters are split: some see a genuinely new capability in an LLM maintaining another model, while others — echoing Honnibal and Sean Goedecke — describe the Qwen fix as a well-executed application of existing steering techniques dressed up as &quot;reading weights&quot;. A recurring counterpoint is that the distinction may matter less than the practical outcome, since a targeted edit producing a roughly 6x benchmark jump appears to replicate.

**Tags**: `#AI research`, `#LLM weight editing`, `#interpretability`, `#model steering`, `#research criticism/reproducibility`

---

<a id="item-22"></a>
## [Repo claims 284B DeepSeek on 64GB RAM without a GPU](https://github.com/synchopate/llama-modchip) ⭐️ 6.0/10

A GitHub project called llama-modchip \(by user synichopate\) claims it can run a 284-billion-parameter DeepSeek model on a machine with only 64GB of RAM and no GPU at all. The repo drew 343 points and 143 comments on Hacker News, where users tried to reproduce the claim and debated what the project actually adds beyond stock llama.cpp. The claim touches a nerve in the local-inference community, where falling memory and GPU prices are not keeping pace with demand for running large models on consumer hardware. If the approach generalizes, it would let hobbyists and small teams run frontier-scale Mixture-of-Experts models on ordinary workstations, though the discussion suggests the headline is more about aggressive quantization than a new engine. The trick is not a new inference engine but extreme low-bit quantization combined with mmap/disk offload, and testers report the default modchip app installs Nemotron and says nothing about DeepSeek, with performance on a Ryzen 7945HX with 96GB DDR5 roughly matching plain llama.cpp on CPU except for faster prefill. Commenters also note quantization performance is non-linear and generally peaks around 4 bits per weight, so quality at the bit-widths needed to fit 284B parameters into 64GB is a serious open question.

hackernews · joshcsimmons · Nov 8, 10:22 · [Discussion](https://news.ycombinator.com/item?id=50411961)

**Background**: DeepSeek-V4-Flash is a 284-billion-parameter Mixture-of-Experts model, meaning only a fraction of its weights activate for each token, which makes it cheaper to run than a dense model of the same size. Even so, the full weights at 16-bit precision would need hundreds of gigabytes, so community GGUF builds quantize them down to formats like IQ1\_S-XL or Q2\_K\_XL, trading accuracy for size. llama.cpp is the widely used open-source C++ inference engine that supports these GGUF files and can run models on CPU plus RAM when no GPU is available.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=50411961">Llama-modchip: 284 B DeepSeek on 64 GB RAM , no GPU</a></li>
<li><a href="https://github.com/synchopate/llama-modchip/blob/main/ARCHITECTURE.md">llama - modchip /ARCHITECTURE.md at main...</a></li>
<li><a href="https://huggingface.co/persadian/DeepSeek-V4-Flash-GGUF">persadian/ DeepSeek -V4-Flash-GGUF · Hugging Face</a></li>

</ul>
</details>

**Discussion**: Sentiment is split between practical hardware advice and skepticism. kennywinker argues a sub-$800 E5 workstation with 96GB-ish RAM and a cheap GPU already delivers usable ~20 tok/s output, armcat warns that quantization below 4 bits sharply degrades quality, and antirez points to 128GB unified RAM running coding agents acceptably fast, while aappleby openly asks whether this &quot;AI-generated repo actually does anything&quot; beyond stock llama.cpp.

**Tags**: `#local-llm-inference`, `#quantization`, `#deepseek`, `#hardware`, `#hackernews-discussion`

---

<a id="item-23"></a>
## [Blogger Argues Writing Is a Thinking Tool, Not Just Output](http://muratbuffalo.blogspot.com/2026/11/writing-as-thinking-tool.html) ⭐️ 6.0/10

A post on Murat Buffalo&\#x27;s blog argues that writing is not merely the final step of recording results but a core part of the thinking and discovery process itself, and the essay reached the front page of Hacker News with 258 points and 77 comments. Commenters quickly extended the thesis beyond prose to design, programming, and system diagramming. The piece lands at a moment when AI drafting tools make producing text cheap, pushing practitioners to re-examine what the human act of composing actually contributes to clarity and insight. For engineers and designers, it reframes everyday artifacts like design files, code, and whiteboard sketches as cognitive instruments rather than mere deliverables. The post is a short reflective essay rather than a study, offering no empirical data, benchmarks, or tooling; its value lies mainly in the discussion thread, where practitioners describe tight loops between thinking and making. Several commenters note the feeling of insight differs markedly from prompt-driven generation, though no one presents evidence beyond personal experience.

hackernews · jruohonen · Nov 8, 10:41 · [Discussion](https://news.ycombinator.com/item?id=50412067)

**Background**: The idea that writing is a mode of thinking rather than a transcription of thought is an old one, often summarized by the observation that one does not know what one thinks until one sees what one has said. It underlies practices like drafting multiple revisions, keeping a lab notebook, and rubber-duck debugging, where articulating a problem aloud or on paper exposes gaps in reasoning. The Hacker News thread extends this to modern tools, contrasting hands-on work in Figma or a code editor with prompt-based generation.

**Discussion**: Commenters broadly agreed and extended the thesis: one described how the writing phase of a PhD turned out to shape the science itself, another argued that Figma prototyping remains essential for novel UX problems because the thinking-and-craft loop has no real substitute in prompting, and others added that coding and paper system diagrams function as external storage for thought. The tone was enthusiastic consensus rather than debate, with no notable counterarguments raised.

**Tags**: `#writing`, `#cognition`, `#software-engineering-practice`, `#design`, `#hackernews-discussion`

---

<a id="item-24"></a>
## [How I Fight AI Brain Fry: Managing Parallel AI Coding Sessions](https://sergeykuhne.com/blog/fighting-ai-brain-fry) ⭐️ 6.0/10

Sergey Kuhne published a blog post describing his personal tactics for avoiding &quot;AI brain fry&quot; — the cognitive overload that comes from juggling several AI-assisted coding sessions at once — and the piece sparked a Hacker News discussion with 128 points and 112 comments. As developers move from typing code to orchestrating multiple AI agents in parallel, human attention and code-review capacity rather than model throughput are becoming the limiting factor, which shapes how individuals and teams should structure AI-assisted workflows. The recommended approach is to cap the number of concurrent AI sessions \(commenters suggest two or three at most\) and accept idle time as a recharge period rather than always starting &quot;just one more session&quot;; the practical caveat is that parallelism multiplies the review burden, since each session can produce diffs of 10,000+ lines whose context is hard to hold simultaneously.

hackernews · kyunez · Nov 8, 19:37 · [Discussion](https://news.ycombinator.com/item?id=50416363)

**Background**: AI-assisted coding tools such as chat-based assistants and terminal or editor-integrated agents can each run long autonomous tasks, which makes it tempting to launch several at once and treat them like parallel workers. &quot;Brain fry&quot; is the informal term for the mental fog and decision fatigue that follows from rapidly context-switching among many such sessions. Hacker News is a widely read technology forum where practitioners frequently compare notes on emerging developer workflows like this one.

**Discussion**: Commenters largely agree that unbounded parallelism backfires: some cap themselves at two or three concurrent sessions and accept idle time as more productive overall, while others \(docheinestages\) reject running parallel threads at all and argue for breaking a task into steps and finishing one thing. The sharpest counterpoint comes from sollewitt, who says the real bottleneck is code review — three 10k-line changelists dilute context and understanding, making multi-session review far worse than single-threaded work — and others report that brokering sessions through markdown notes or Linear quickly became tedious, out of sync, and token-expensive.

**Tags**: `#AI-assisted-development`, `#developer-productivity`, `#cognitive-load`, `#workflow`, `#code-review`

---

<a id="item-25"></a>
## [Blog post argues agent memory needs an OpenTelemetry-style standard](https://www.lorekit.io/blog/open-agent-memory-format) ⭐️ 6.0/10

A post on the LoreKit blog \(lorekit.io\) argues that AI agent memory should have a standardized, interoperable format, drawing an explicit analogy to how OpenTelemetry became the common standard for telemetry data. The proposal was submitted to Hacker News, where it drew a substantive but largely skeptical discussion rather than adoption momentum. Agent memory is currently a fragmented space where every framework invents its own storage schema, so a shared format could make memory portable across tools, vendors, and agent runtimes the way OpenTelemetry made telemetry vendor-neutral. However, the community pushback suggests the industry may not yet know what such a standard should encode, meaning any early spec risks locking in the wrong abstractions. The post frames the problem as interoperability rather than capability, arguing that without a common memory format agents remain locked into single-vendor or single-framework stores. The critique in the comments notes that concrete efforts in this direction already exist — projects such as the Agent Memory Protocol and the Universal Memory Protocol publish schemas covering memory-store structure, node types, link semantics, indexing, import/export, and versioning — which weakens the claim that nothing exists yet.

hackernews · mthines · Nov 8, 08:40 · [Discussion](https://news.ycombinator.com/item?id=50411467)

**Background**: LLM agents are stateless at their core: an LLM&\#x27;s only real memory is the context window sent with each request, so anything remembered across sessions must be written to and re-read from external storage. Developers therefore build memory layers — flat files, vector stores, hierarchical summaries — to persist facts, plans, and project context between runs. OpenTelemetry is the reference point here because it is a vendor-neutral open standard for traces, metrics, and logs that is supported by more than 90 observability vendors and integrated into many libraries and services, showing what a successful ecosystem-wide standard looks like.

<details><summary>References</summary>
<ul>
<li><a href="https://opentelemetry.io/">OpenTelemetry</a></li>
<li><a href="https://arxiv.org/abs/2603.07670">[2603.07670] Memory for Autonomous LLM Agents:Mechanisms ... Agent Memory Architecture — Optimized Memory for LLM Agents Agent Memory Systems: The Complete Guide (2026) A Practical Guide to Memory for Autonomous LLM Agents AI Agent Memory Management System Architecture Design ... Architecture and Orchestration of Memory Systems in AI Agents</a></li>
<li><a href="https://universalmemoryprotocol.io/">Universal Memory Protocol</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly skeptical: several argued the need is overstated because agents are already good at reading whatever memory format a project uses, and LLMs excel at interpreting informal natural language, so a rigid schema adds little. Others warned that standardizing now could produce another SOAP or SGML — a premature abstraction built before anyone understands how long memory should last or how context should be structured — and some questioned whether cross-user memory sharing is even desirable; a further complaint was that the post itself reads as LLM-generated.

**Tags**: `#AI agents`, `#agent memory`, `#standards`, `#OpenTelemetry`, `#LLM tooling`

---

<a id="item-26"></a>
## [GRFNet: Open-source PyTorch model for multichannel time-series classification](https://www.reddit.com/r/MachineLearning/comments/1xqqj67/grfnet_pytorch_model_for_multichannel_timeseries/) ⭐️ 6.0/10

A Reddit post by /u/joekrry introduces GRFNet, an open-source PyTorch model for multichannel time-series classification that combines ROCKET-style random convolutional kernels, learned spatial filters, dilated convolutions, and gated summary statistics. The default configuration handles 22 channels and 4 classes with only 3,847 parameters, accepts variable input lengths, and is being prepared for subject-independent EEG evaluation. EEG decoding often suffers from small datasets and high inter-subject variability, so a model with fewer than 4,000 parameters that can adapt to different channel layouts and sampling rates could be attractive for low-resource or subject-independent brain-computer interface applications. However, the project has no published benchmark results yet, so its practical value remains unproven. If sensor positions are supplied, the learned spatial filters are initialized from the electrode layout rather than random noise; most dilated kernels are frozen random filters with only a few learnable kernels. The author plans comparisons against EEGNet and ShallowConvNet on PhysioNet EEGMMIDB with 109 subjects and subject-wise train/test splits, plus scalp topographies, confusion matrices, saliency maps, speed benchmarks, and four architecture variants.

reddit · r/MachineLearning · /u/joekrry · Nov 8, 05:13

**Background**: ROCKET \(RandOm Convolutional KErnel Transform\) showed that random, untrained convolutional kernels combined with a simple linear classifier can deliver strong time-series classification accuracy at low computational cost. EEG decoding models commonly use spatial filters to mix electrode channels before temporal feature extraction, which is important because EEG datasets are typically small, noisy, and highly variable across subjects. GRFNet applies these ideas to multichannel EEG-like signals and plans to use PhysioNet EEGMMIDB, a widely used 109-subject EEG dataset, for evaluation.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/1910.13051">ROCKET: Exceptionally fast and accurate time series ... ROCKET: Exceptionally fast and accurate time series ... ROCKET: exceptionally fast and accurate time series ... ROCKET: exceptionally fast and accurate time series ... ROCKET: Exceptionally fast and accurate time series ... Time series classification with random convolution kernels ... ROCKET: exceptionally fast and accurate time series ...</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11199199/">EEG decoding with spatiotemporal convolutional neural network ...</a></li>

</ul>
</details>

**Tags**: `#EEG`, `#time-series classification`, `#PyTorch`, `#ROCKET`, `#deep learning`

---

<a id="item-27"></a>
## [Local Qwen3.8 Flash Next Generates 15-Second Three.js Motion Graphics Video on an RTX 4080](https://www.reddit.com/r/LocalLLaMA/comments/1xr3qes/motion_graphics_video_made_with_qwen38_flash_next/) ⭐️ 6.0/10

A Reddit user \(u/Yhojm\) produced a 15-second, 1920×1080, 60fps motion-graphics showcase of a Japanese Shinkansen train entirely with the quantized Qwen3.8 Flash Next GSQ RCO IQ3\_XXS model running locally on a 16GB RTX 4080 with 64GB DDR5-5600, served through strata and driven by the opencode coding agent at roughly 95 tok/s decode and 3000 tok/s prefill. The first render took about 40 minutes, and roughly three follow-up prompts to fix a dark frame, missing buildings and broken text brought the total to around two hours. It shows that a single consumer GPU can now drive a full agentic code-generation pipeline that writes Three.js scenes, renders them frame by frame with Playwright, and encodes MP4 via ffmpeg — a workflow that previously required frontier proprietary models like Opus. The concrete throughput numbers and the copyable prompt &quot;recipe&quot; make it a practical reference point for the local-LLM community rather than just a demo. The user notes the output is not comparable to Opus in quality, and that the pipeline has no inherent duration limit so videos can be arbitrarily long. Quality is highly dependent on iteration: the first attempt came out dark, lacked buildings and contained too much on-screen text, requiring the three follow-up prompts; the model&\#x27;s VRAM footprint is held down by the IQ3\_XXS \(~3-bit\) quantization of a large MoE model.

reddit · r/LocalLLaMA · /u/Yhojm · Nov 8, 17:23

**Background**: Qwen3.8 Flash Next is a large Mixture-of-Experts \(MoE\) model, and the &quot;GSQ RCO IQ3\_XXS&quot; suffix refers to the quantized GGUF weights published by ISTA-DASLab, which trade file size and VRAM usage against output quality across several precision levels. Strata is an open-source local inference engine that makes such massive MoE models fit on consumer GPUs by dynamically swapping dormant expert layers between VRAM, system RAM and NVMe storage, while opencode is an open-source terminal-based AI coding agent that can call models from many providers or a local endpoint. The rendering half of the recipe relies on Three.js \(a JavaScript 3D library\) for the animation, Playwright for headless browser frame capture, and ffmpeg for encoding the frames into an MP4.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/ISTA-DASLab/Qwen3.8-Flash-Next-GSQ-RCO-GGUF">ISTA-DASLab/ Qwen 3 . 8 - Flash - Next - GSQ - RCO -GGUF · Hugging Face</a></li>
<li><a href="https://github.com/Niko1221/Strata">GitHub - Niko1221/Strata: Qwen3.8-Flash-Next on any consumer ...</a></li>
<li><a href="https://opencode.ai/docs/cli/">Intro | OpenCode</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#qwen`, `#code-generation`, `#three.js`, `#video-generation`

---

<a id="item-28"></a>
## [Six GPUs \(4x Radeon AI PRO R9700 + 2x RTX 3090\) Run Off One x16 PCIe Slot via a Switch](https://www.reddit.com/r/LocalLLaMA/comments/1xr2a6y/4x_radeon_ai_pro_r9700_2x_rtx_3090_on_one_x16/) ⭐️ 6.0/10

A Reddit user \(bolts98\) on r/LocalLLaMA posted a build that runs four AMD Radeon AI PRO R9700 cards and two RTX 3090s simultaneously through a single x16 PCIe slot by using a PCIe switch, rather than relying on one physical slot per GPU. The configuration puts roughly 176 GB of combined VRAM behind one host link, targeting multi-GPU local LLM inference. Consumer and most prosumer platforms offer far too few PCIe lanes for four-to-six GPU builds, so a working switch-based configuration is a concrete real-world datapoint for homelab and local-LLM users who want maximum VRAM without buying server-class motherboards or CPUs. It also shows that AMD&\#x27;s 32 GB workstation cards are being taken seriously as inference hardware alongside used RTX 3090s. The switch fans out a single upstream x16 link to all six GPUs, so aggregate host bandwidth is capped at whatever that one link provides and each card effectively gets a fraction of it — usually acceptable for layer-split llama.cpp inference, where bandwidth mostly matters during model load, but a real constraint for tensor-parallel workloads with heavy per-token synchronization. Because the build mixes AMD and Nvidia cards, expect separate driver stacks \(ROCm and CUDA\), meaning a single model is typically not split across both vendors at once.

reddit · r/LocalLLaMA · /u/bolts98 · Nov 8, 16:23

**Background**: A PCIe switch chip acts like a small network switch for PCIe: the host sees one upstream link, and the chip fans it out to multiple downstream devices, letting several GPUs share lanes that the CPU would otherwise have to arbitrate itself. Mainstream desktop CPUs typically expose around 20–24 PCIe lanes, which is why multi-GPU builders either move to HEDT/server platforms or add a switch card. The Radeon AI PRO R9700 is AMD&\#x27;s RDNA 4-based workstation card launched in July 2025 with 32 GB of GDDR6 and a 300 W power envelope, positioned for local AI inference; the RTX 3090 remains popular in the local-LLM community for its 24 GB of VRAM.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techpowerup.com/gpu-specs/radeon-ai-pro-r9700.c4290">AMD Radeon AI PRO R9700 Specs | TechPowerUp GPU Database</a></li>
<li><a href="https://www.amd.com/en/products/graphics/workstations/radeon-ai-pro/ai-9000-series/amd-radeon-ai-pro-r9700.html">AMD Radeon™ AI PRO R9700</a></li>
<li><a href="https://aikaboom.com/01_physical_realm/chapter_1/1.5c_15c_pcie_slots_risers_and_switch_chips/">1.5c PCIe slots, risers, and switch chips: how multiple GPUs ...</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#gpu-hardware`, `#pcie-switch`, `#multi-gpu`, `#homelab`

---

<a id="item-29"></a>
## [4x Radeon R9700 Build Serves 8 Users at 128K Context](https://www.reddit.com/r/LocalLLaMA/comments/1xrcia4/joined_the_4x_r9700_club_initial_benchmarks_for/) ⭐️ 6.0/10

A user on r/LocalLLaMA shared a roughly $16,000 CAD local inference server built from four AMD Radeon AI PRO R9700 GPUs \(three Gigabyte, one XFX, all power-limited to 210W\) on an EPYC 7402P platform with 128GB DDR4. Running Qwen3.8-Flash-Next through Radiance v1.17.0 on ROCm 10.1, the rig posted about 190 tok/s single-user decode, roughly 6,800 tok/s aggregate prefill regardless of user count, and 80–225 tok/s per user with eight concurrent 128K-context sessions. Real-world concurrency data for AMD&\#x27;s RDNA 4 workstation cards is still scarce, so this gives the local-LLM community a practical reference point for multi-user agent serving on AMD hardware. It also suggests a four-card 128GB AMD setup can handle privacy-sensitive business inference workloads as an alternative to NVIDIA&\#x27;s lineup. At tensor parallelism of 4, the model&\#x27;s 17.4 GiB of weights per card fit entirely in VRAM, the KV cache gets 11.6 GiB per card \(about 1.6M tokens, or eight full 200K sessions\), and a 47.7 GiB n-gram/PLE table is pinned in host RAM. The worst case measured — eight users each firing a fresh 128K prompt simultaneously — waits about 2.5 minutes for the first token, and the report is an anecdotal personal benchmark without published scripts or full methodology.

reddit · r/LocalLLaMA · /u/Anarchaotic · Nov 8, 23:36

**Background**: The Radeon AI PRO R9700 is AMD&\#x27;s RDNA 4 \(Navi 48\) workstation GPU with 32GB of GDDR6 and roughly 640 GB/s of memory bandwidth, positioned for local AI work rather than gaming. LLM inference splits into two phases: prefill, which processes all prompt tokens in parallel and determines time-to-first-token, and decode, which generates output tokens one at a time and determines streaming speed. ROCm is AMD&\#x27;s open software stack analogous to CUDA, and the EPYC 7402P is a 24-core Zen 2 server CPU launched in 2019, which this builder bought used on eBay.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/gpus/amd-launches-radeon-ai-pro-r9700-to-challenge-nvidias-ai-market-dominance">AMD launches Radeon AI Pro R 9700 to challenge... | Tom&#x27;s Hardware</a></li>
<li><a href="https://runaihome.com/blog/amd-radeon-ai-pro-r9700-local-ai-hardware-guide-2026/">AMD Radeon AI PRO R 9700 for Local AI in 2026: 32GB, a $1,299...</a></li>
<li><a href="https://llm-speed.com/blog/decode-vs-prefill-tokens-per-second">Decode vs prefill tok/s: what speed numbers mean · llm-speed</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#gpu-benchmarks`, `#amd-rdna4`, `#inference-performance`, `#multi-gpu`

---

<a id="item-30"></a>
## [Hands-On QUBO Tutorial Runs End-to-End on D-Wave Quantum Annealer](https://www.reddit.com/r/programming/comments/1xqqoz3/quantum_optimization_solve_qubo_on_dwave_quantum/) ⭐️ 6.0/10

A new Python tutorial walks developers through solving a Max-Cut/QUBO problem end to end on a real D-Wave quantum annealer, covering Leap access, QUBO-to-BQM conversion, embedding, SampleSet interpretation, QPU timing, and a local neal simulated-annealing fallback. It lowers the barrier for Python developers and optimization practitioners to experiment with quantum annealing by showing what actually happens after calling sampler.sample\(...\) and how logical variables map onto physical hardware. The tutorial is educational rather than a novel breakthrough, but it fills a practical gap for developers who want hands-on exposure to real QPU workflows. The tutorial emphasizes practical mechanics rather than quantum advantage: it explains minor embedding and qubit chains, physical-qubit usage, the meaning of energy and num\_occurrences, and QPU annealing, sampling, programming, and access times. It also provides a local neal simulated-annealing fallback so the same workflow can be tested without hardware access.

reddit · r/programming · /u/Future\_Ad7567 · Nov 8, 05:22

**Background**: QUBO is an NP-hard combinatorial optimization formulation used in finance, machine learning, and graph problems, and many quantum annealers accept QUBO or equivalent Ising models. D-Wave systems are programmable quantum annealers that map problems onto a transverse-field Ising Hamiltonian using superconducting flux qubits. Because hardware connectivity is sparse, minor embedding maps each logical variable to a chain of physical qubits, which is a key practical step in running real problems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/D-Wave_Systems">D - Wave Systems - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Quadratic_unconstrained_binary_optimization">Quadratic unconstrained binary optimization - Wikipedia</a></li>
<li><a href="https://arxiv.org/html/2507.16004v1">Minor Embedding for Quantum Annealing with Reinforcement Learning</a></li>

</ul>
</details>

**Tags**: `#quantum-computing`, `#D-Wave`, `#QUBO`, `#optimization`, `#python-tutorial`

---