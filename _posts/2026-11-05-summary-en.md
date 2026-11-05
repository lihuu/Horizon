---
layout: default
title: "Horizon Summary: 2026-11-05 (EN)"
date: 2026-11-05
lang: en
---

> From 79 items, 31 important content pieces were selected

---

1. [IEEE Spectrum: AI Bug Hunting Forces Payoff of 40 Years of Security Debt](#item-1) ⭐️ 8.0/10
2. [Moonshot AI releases open weights for Kimi K3.1 Pro](#item-2) ⭐️ 8.0/10
3. [Go unveils encoding/json/v2, a long-awaited JSON API redesign](#item-3) ⭐️ 8.0/10
4. [Anthropic advances cryptographically provable inference for large language models](#item-4) ⭐️ 8.0/10
5. [Tencent Releases Hy4: 770B Open-Weight Model With Science and Game-Dev Focus](#item-5) ⭐️ 8.0/10
6. [NKI megakernels cut GLM-5.3-Flash decode latency on AWS Trainium2](#item-6) ⭐️ 8.0/10
7. [Ricursive Intelligence Releases Ripple-65B-Preview, a Dense Open-Weights Model](#item-7) ⭐️ 8.0/10
8. [C++26 Fails ISO National Body Vote in Unprecedented Setback](#item-8) ⭐️ 8.0/10
9. [Postgres 19 Ships Built-In REPACK for Online Table Bloat Cleanup](#item-9) ⭐️ 8.0/10
10. [Blog Claims White House IP Space Carries Residential Proxy Traffic](#item-10) ⭐️ 7.0/10
11. [Nvidia RTX Spark Linux GPU throttling slashes local AI inference speed](#item-11) ⭐️ 7.0/10
12. [AMD&\#x27;s $17B Q4 guidance would outsell Intel for the first time](#item-12) ⭐️ 7.0/10
13. [Deep Principle releases Hydrogen-1.0, an open-weight science model beating GPT-6 Astra on FSR](#item-13) ⭐️ 7.0/10
14. [Looped Transformers Save Storage, Not HBM Traffic, B200 Profiling Shows](#item-14) ⭐️ 7.0/10
15. [Developer prunes Gemma 4 26B-A4B down to a dense 3.81B model](#item-15) ⭐️ 7.0/10
16. [Unsloth ships Dynamic v3.1 GGUFs for Qwen3.8-Flash-Next](#item-16) ⭐️ 7.0/10
17. [Axion 1.0: A Fully Open 35B Agent Model Trained in Three Simple Stages](#item-17) ⭐️ 7.0/10
18. [Zig&\#x27;s libc rewrite blamed for 12,000× SQLite slowdown](#item-18) ⭐️ 7.0/10
19. [Interactive Explainer Peers Inside Git&\#x27;s Object Model and Refs](#item-19) ⭐️ 7.0/10
20. [Apple&\#x27;s 10-K flags rogue AI agents that can &\#x27;conceal&\#x27; and &\#x27;manipulate&\#x27;](#item-20) ⭐️ 7.0/10
21. [Cognition launches SWE-2 Flash, a faster, cheaper coding-agent model](#item-21) ⭐️ 7.0/10
22. [San Francisco&\#x27;s Guerrilla Bike Lanes Become Permanent Infrastructure](#item-22) ⭐️ 6.0/10
23. [OpenAI to acquire Pierre Computer Company, maker of Codex diff libraries](#item-23) ⭐️ 6.0/10
24. [Verification Is Not Knowledge: Science Needs Understanding, Not Just Answers](#item-24) ⭐️ 6.0/10
25. [Xiaomi claims humanoid robots worked a full 8-hour autonomous factory shift](#item-25) ⭐️ 6.0/10
26. [datasette-apps 0.3a0 Refines Datasette Agent Integration for Custom HTML Apps](#item-26) ⭐️ 6.0/10
27. [Researcher urges top AI conferences to desk-reject AI-generated papers](#item-27) ⭐️ 6.0/10
28. [Reddit debate: is CVPR&\#x27;s 25-paper-per-author cap unfit for the AI era?](#item-28) ⭐️ 6.0/10
29. [DeepSeek took 53% of OpenRouter&\#x27;s 27T daily tokens as open-weights labs pass 75%](#item-29) ⭐️ 6.0/10
30. [LFM3-Omni-2B claimed to run offline on iPhone at ~80 tok/s via WebGPU](#item-30) ⭐️ 6.0/10
31. [The Lost malloc\(\): Revisiting an Early Unix Allocator Interface](#item-31) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [IEEE Spectrum: AI Bug Hunting Forces Payoff of 40 Years of Security Debt](https://spectrum.ieee.org/ai-in-cybersecurity-php2shell-vulnerability) ⭐️ 8.0/10

An IEEE Spectrum article argues that AI-driven vulnerability discovery — exemplified by the high-impact PHP2Shell flaw in PHP — is exposing and forcing remediation of roughly 40 years of accumulated security technical debt. The piece sparked a large Hacker News discussion \(about 1,015 points and 612 comments\) that debated whether this really amounts to paying down debt or merely starts an endless treadmill of fix-work. AI is industrializing vulnerability discovery, so the volume of reported flaws is outpacing the capacity of maintainers and security teams to patch them, pushing organizations from traditional vulnerability management toward broader exposure management. Because so much of the web runs on long-lived codebases like PHP, the remediation burden falls on a vast, diffuse ecosystem of projects and vendors rather than a few large players. PHP2Shell refers to a pair of remote-code-execution vulnerabilities, CVE-2026-109618 and CVE-2026-109619, rooted in memory-safety flaws affecting PHP versions 5.4 through 8.5. Commenters note that many of these findings are not narrow off-by-one errors fixable with a surgical patch but require restructuring, which is why &\#x27;debt payoff&\#x27; and &\#x27;endless fix treadmill&\#x27; can look identical in the short term.

hackernews · pseudolus · Nov 4, 11:52 · [Discussion](https://news.ycombinator.com/item?id=50364336)

**Background**: Technical debt is the accumulated cost of shortcuts and deferred work in software; security technical debt specifically means unpatched vulnerabilities, outdated practices, and postponed hardening that raise risk over time. PHP is a server-side scripting language that powers a large share of the web, and much of its legacy code dates back decades. AI models and machine-assisted static analysis and fuzzing can now scan such code at a scale humans never could, surfacing flaws that sat unnoticed for years — the dynamic the article calls the forced repayment of four decades of debt.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PHP2Shell">PHP2Shell - Wikipedia</a></li>
<li><a href="https://www.akamai.com/blog/security-research/understanding-php2shell-everything-you-need-to-know">Understanding PHP2Shell: Everything You Need to Know</a></li>
<li><a href="https://www.techtarget.com/news/php2shell-explained-timeline-of-the-global-vulnerability-crisis/872935/">PHP2Shell explained: Timeline of the global vulnerability ...</a></li>

</ul>
</details>

**Discussion**: Sentiment was substantive rather than cheerleading: swatcoder questioned the article&\#x27;s framing, asking whether this is debt payoff or a compulsory endless treadmill of feature-neutral fix work, while Balgair invoked Gödel, Escher, Bach&\#x27;s record-player parable to argue that perfectly secure systems are impossible even in theory. Others were more optimistic — glennfiedler predicted software will end up more secure than ever after a painful few months, xbmcuser said AI auditing will finally make good on open source&\#x27;s often-assumed but rarely delivered outside review, and Arbortheus hoped nation-state and commercial zero-days will be found incidentally along the way.

**Tags**: `#AI security`, `#vulnerability discovery`, `#technical debt`, `#cybersecurity`, `#static analysis`

---

<a id="item-2"></a>
## [Moonshot AI releases open weights for Kimi K3.1 Pro](https://huggingface.co/moonshotai/Kimi-K3.1-Pro) ⭐️ 8.0/10

Moonshot AI published the open weights for Kimi K3.1 Pro on Hugging Face, describing it as an open-weight, natively multimodal agentic model and its most capable 3T-class model to date. It is the first release in the K3.1 series, post-trained from Kimi K3 with large-scale joint reinforcement learning across hundreds of downstream domains. Another frontier-class model dropping open weights puts pressure on closed API providers and, as commenters noted, immediately spawned a competitive market of third-party inference hosts on OpenRouter offering higher throughput at the same price. For enterprises with the hardware, it also means a top-tier multimodal model can be self-hosted instead of rented. The model inherits the 1M-token context window and visual input support of the K3 line, and community members estimate that self-hosting realistically requires something on the order of an 8x B300 node. The previous generation, Kimi K3, was a 2.8-trillion-parameter MoE model released under a Modified MIT license.

hackernews · abrarthought · Nov 4, 15:30 · [Discussion](https://news.ycombinator.com/item?id=50366999)

**Background**: Moonshot AI is the Chinese lab behind the Kimi chatbot and model family, which has built a reputation for publishing open weights — downloadable model files that anyone can run on their own hardware, unlike closed models accessible only through an API. Kimi&\#x27;s large models use a mixture-of-experts \(MoE\) architecture, which activates only a fraction of parameters per token to keep inference cheaper than the raw parameter count suggests, though trillion-parameter models still demand multi-GPU servers. The &\#x27;Pro&\#x27; naming and the 3.1 version bump indicate an incremental upgrade over the K3 generation rather than a new architecture.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3.1-Pro">moonshotai/ Kimi -K 3 . 1 - Pro · Hugging Face</a></li>
<li><a href="https://thenewstack.io/kimi-k3-open-weights/">Moonshot opens Kimi K3 weights — but few can run it</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kimi_%28AI%29">Kimi (AI) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Sentiment was split: skeptics argued the model looks &\#x27;benchmaxxed&\#x27; because it barely outpaces DeepSeekV4.1-Flash and scores lower than Opus5.5 on other labs&\#x27; internal benchmarks, while at least one commenter reported strong first-hand testing results and called it a very strong release slightly off the frontier. Others focused on practicalities — an 8x B300 node for self-hosting is out of reach for most individuals, and third-party hosts like Together and Modal are already delivering several times Moonshot&\#x27;s own endpoint throughput, suggesting room for cost cuts.

**Tags**: `#open-weight LLMs`, `#Moonshot AI`, `#model release`, `#LLM benchmarks`, `#inference infrastructure`

---

<a id="item-3"></a>
## [Go unveils encoding/json/v2, a long-awaited JSON API redesign](https://go.dev/blog/jsonv2) ⭐️ 8.0/10

The Go team has introduced encoding/json/v2 and the underlying encoding/json/jsontext package, a new API for JSON serialization and parsing that aims to improve ergonomics and fix behavioral issues in the original encoding/json package. Because encoding/json is one of the most widely used packages in Go, the redesign has broad implications for API contracts, migration strategies, and performance in web services, CLIs, and data pipelines across the ecosystem. The v1 encoding/json API remains behaviorally unchanged, while compatibility options such as DefaultOptionsV1 let teams migrate incrementally; early reports note faster unmarshalling but slower marshalling in some benchmarks, and helpers like MarshalIndent are not carried over in the same form.

hackernews · olexsmir · Nov 4, 17:52 · [Discussion](https://news.ycombinator.com/item?id=50369106)

**Background**: JSON is a ubiquitous text format for data interchange, and Go&\#x27;s encoding/json package has long been the standard way to marshal and unmarshal it in Go programs. Over more than a decade, the original API accumulated design compromises and behavioral quirks, prompting a formal proposal for a v2 design with a lower-level jsontext layer for token handling. The new API is being introduced with compatibility options so existing v1 code does not change behavior overnight.

<details><summary>References</summary>
<ul>
<li><a href="https://go.dev/blog/jsonv2">A new Go API for JSON - The Go Programming Language</a></li>
<li><a href="https://github.com/golang/go/issues/71497">encoding / json / v 2 : new API for encoding / json · Issue #71497...</a></li>
<li><a href="https://importstatic.com/go/go-json-v2-migration">Go JSON v 2 Migration : What Breaks in Go 1.27 | ImportStatic</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion is broadly positive, with commenters welcoming a cleaner JSON API and agreeing that marshalling needed fixing. Several users highlight migration pain points, especially the loss of MarshalIndent and the complexity of its replacement, while others discuss parser performance and schema-specialized SIMD parsing. One commenter notes that they now rely on AI to write Go but still value Go&\#x27;s performance and safety.

**Tags**: `#Go`, `#JSON`, `#standard library`, `#API design`, `#software engineering`

---

<a id="item-4"></a>
## [Anthropic advances cryptographically provable inference for large language models](https://www.anthropic.com/research/provable-inference) ⭐️ 8.0/10

Anthropic published research on using zkSNARKs — a succinct cryptographic proof system — to let a model provider commit to a specific set of weights and then prove that each individual response was produced by exactly those weights. The prototype commitment is roughly 6.5 MB and covers about 16 million requests, after which the provider must commit again, while verifying a single per-request proof takes about 17 seconds on 24 threads \(21 seconds single-threaded\). For closed-weight API providers, clients currently have no way to check which model actually answered them — output quality alone cannot distinguish the advertised model from a cheaper or distilled substitute. A working proof-of-inference primitive would give auditors, regulators, and enterprise buyers a cryptographic basis for trusting AI services, which is why the overhead-versus-trust tradeoff is drawing attention across the ecosystem. The scheme imposes a substantial cost: reporting and community discussion put proving overhead at roughly 90–100x the compute of ordinary inference, which makes it impractical for high-volume serving today. It also relies on deterministic inference and only certifies that the output satisfies the claimed computation relation, so analyses of zk proof-of-inference \(such as the Hollow-LLM work\) warn that such proofs do not automatically rule out degenerate or trivially-weighted variants.

hackernews · ltononro · Nov 4, 17:17 · [Discussion](https://news.ycombinator.com/item?id=50368626)

**Background**: A zkSNARK is a cryptographic proof that a computation was carried out correctly, producing a short proof that is far cheaper to verify than to re-run the computation itself — the same family of techniques used in some blockchain scaling systems. Applying it to LLM inference means expressing every matrix multiplication of a forward pass inside a proof system, which is why the overhead is measured in multiples of the original compute. The problem only exists for closed models: with open weights, a client can simply re-run the inference deterministically and compare outputs, which is far cheaper than any cryptographic approach. Earlier work in this space includes zkLLM and the VerInf project, which explored similar settings before Anthropic&\#x27;s post.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/research/provable-inference">Progress on provable inference for large language models</a></li>
<li><a href="https://www.europesays.com/ai/226951/">Progress on provable inference for large language models ...</a></li>
<li><a href="https://github.com/JamesPetrie/zkllm-entropy">GitHub - JamesPetrie/zkllm-entropy · GitHub</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread was technically rich but contentious: one commenter, a former MARS fellow, said the work is built on his VerInf project — down to the choice of a 400B Maverick-class model — with very little attribution. Others argued the closed-model case can be handled far more cheaply by probabilistically cross-checking four independent inference providers on the same non-batched prompt, noted that open-weight models make the whole problem trivial via deterministic recomputation, and a startup \(Attestable\) said its own approach is one of the comparisons in the post.

**Tags**: `#LLM verification`, `#provable inference`, `#zero-knowledge proofs`, `#AI trust and safety`, `#Anthropic research`

---

<a id="item-5"></a>
## [Tencent Releases Hy4: 770B Open-Weight Model With Science and Game-Dev Focus](https://hy.tencent.ai/research/hy4) ⭐️ 8.0/10

Tencent&\#x27;s Hy team released Hy4, a new-generation Mixture-of-Experts flagship with 770B total parameters and 49B activated per token, published as open weights \(the preview build lives on Hugging Face as tencent/Hy4-preview\). Alongside the main model, Tencent open-sourced two science-focused foundation models co-developed with Hy4 and Hyra 2.0 — HyCell for single-cell representation and HyPDE for physical field modeling — and shipped extensive adaptations of Hy4 for the Unreal Engine, Unity, and Godot game engines. A 770B-class open-weight release from a major Chinese lab pushes the frontier of what anyone can download and self-host, directly intensifying the open-versus-closed split in the global AI ecosystem. The decision to open-source domain-specific science models like HyCell and HyPDE is unusual among frontier labs and lowers the barrier for academic and biotech researchers who cannot access closed APIs or afford to train such models themselves. Hy4 uses a sparse Mixture-of-Experts architecture: despite only 49B active parameters per token, the full 770B weight file imposes a substantial VRAM and serving-cost barrier for local deployment, so most users will likely reach it through hosted APIs. Tencent itself states that a notable gap remains to top proprietary models, especially on internal benchmarks for research-level mathematics, long-horizon coding, model self-improvement, and advanced visual question answering, and says it will keep scaling pre-training and post-training to narrow it.

hackernews · Philpax · Nov 4, 14:11 · [Discussion](https://news.ycombinator.com/item?id=50365780)

**Background**: Tencent&\#x27;s model family was previously known as Hunyuan and is now branded Tencent Hy; like many recent frontier systems, it relies on a Mixture-of-Experts design in which only a small subset of the network&\#x27;s parameters is activated for each token, trading memory for cheaper inference. &quot;Open-weight&quot; means the trained parameter files are publicly downloadable so teams can run, fine-tune, and self-host the model — it is not the same as open source, since training data and full training code are typically not released. HyCell and HyPDE belong to a class of specialized scientific models that target narrow technical tasks, such as representing single-cell gene expression data or solving physical field equations, rather than general conversation.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/tencent/Hy4-preview">tencent / Hy 4 -preview · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tencent_Hy">Tencent Hy - Wikipedia</a></li>
<li><a href="https://www.eesel.ai/blog/tencent-hy4-review">Tencent Hy 4 review: is the 770B open-weight model worth it? | eesel AI</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly positive but focused on different angles: Simon Willison singled out the game-development specialization, noting the partnership with Tencent Interactive Entertainment to curate training data and evaluations around feature implementation, gameplay logic, state tracking, and asset pipelines. areoform praised the open-sourcing of science models as a refreshing contrast to US companies restricting research use, while frangonf appreciated Tencent&\#x27;s candid acknowledgment of the gap to proprietary models and argued open models are already good enough as day-to-day tools. chriddyp reported that on Plotly&\#x27;s data-analytics benchmark Hy4 landed on the cost/accuracy frontier between two GPT-6.1 variants, but was &quot;verrrry slow,&quot; sometimes issuing 26 to 64 queries per question.

**Tags**: `#open-weight models`, `#LLM release`, `#AI research`, `#game development`, `#open science`

---

<a id="item-6"></a>
## [NKI megakernels cut GLM-5.3-Flash decode latency on AWS Trainium2](https://www.reddit.com/r/MachineLearning/comments/1xo0yuq/p_nki_layer_megakernels_for_glm53flash_on_aws/) ⭐️ 8.0/10

RunAnywhere open-sourced trnrt, an inference engine that serves GLM-5.3-Flash—a 320B-parameter MoE model with 1M-token context—on a single AWS trn2.48xlarge, and rewrote each layer half as one fused NKI megakernel \(whole layers for sparse-attention layers\). On the same layout, a batch-8 decode step fell from 32.2 ms in the 17 October build to 24.2 ms in the 1 November build, with the fused sparse-attention layer and the KDA/MoE kernels each saving about 3.2 ms per step. The result shows that most decode latency on Trainium2 came from kernel-boundary overhead, XLA glue, transposes and cross-chip collectives rather than model math, making kernel-level co-design a first-order lever for non-NVIDIA accelerators. It also provides a rare reusable inference artifact for a 320B MoE with 1M context on AWS silicon, where the latest vLLM Neuron plugin registers no GLM model and NxD Inference is in maintenance mode. The kernels keep each layer half&\#x27;s working set in the 28 MiB SBUF of a physical NeuronCore and split the 340–400 GB/s weight stream across both cores to reach 672–708 GB/s, while the batch-8 step still spends 6.1 ms at the memory floor, 10.0 ms with engines busy, 4.6 ms waiting inside kernels, 2.8 ms on exposed collectives and 0.7 ms idle. Caveats include one remaining approximation in sparse-attention prefill on 1.2% of selections, which shifted next-token log-probabilities by 0.012–0.021 nats and changed the top token at 3 of 448 positions, and no task-level eval or GPU comparison was run.

reddit · r/MachineLearning · /u/WildCard727 · Nov 4, 21:47

**Background**: AWS Trainium2 is Amazon&\#x27;s custom AI accelerator; its NeuronCore-v3 compute engines and on-chip SBUF are programmed through NKI, a low-level interface that gives direct access to the NeuronCore instruction set for custom kernels. GLM-5.3-Flash is Z.ai&\#x27;s 320B-parameter MoE model with 18B activated parameters and a 1M-token context, designed for cheap inference. In LLM decoding, each generated token requires a forward pass through every layer, so small per-kernel overheads compound across hundreds of kernels and chips; megakernels fuse a whole layer or layer half into one kernel to avoid those boundaries. XLA is the compiler that normally stitches operations into a graph and inserts collectives, which is why kernel boundaries, glue code and collectives became the profiling targets.

<details><summary>References</summary>
<ul>
<li><a href="https://awsdocs-neuron.readthedocs-hosted.com/en/latest/general/nki/index.html">Neuron Kernel Interface (NKI) — AWS Neuron Documentation</a></li>
<li><a href="https://awsdocs-neuron.readthedocs-hosted.com/en/latest/nki/about/trainium2_arch.html">Trainium 2 Architecture Guide for NKI — AWS Neuron Documentation</a></li>
<li><a href="https://huggingface.co/zai-org/GLM-5.3-Flash">zai-org/ GLM - 5 . 3 - Flash · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#AWS Trainium`, `#kernel fusion`, `#MoE models`, `#performance profiling`

---

<a id="item-7"></a>
## [Ricursive Intelligence Releases Ripple-65B-Preview, a Dense Open-Weights Model](https://www.reddit.com/r/LocalLLaMA/comments/1xo2arv/ricursive_intelligence_ripple65bpreview_new_dense/) ⭐️ 8.0/10

Ricursive Intelligence released a preview of Ripple-65B, a 65B dense open-weights model built with an unusual &quot;thin and deep&quot; shape of 80 layers × 5120 dimensions and a 4:1 sliding-window-to-global attention hybrid. The company reports benchmarks that trade blows with far larger frontier open models such as Muse Spark Open \(816B\) and Reflection&\#x27;s Beam \(501B\), and community GGUFs \(Q8\_0 at 68.8 GB, Q4\_K\_M at 38.8 GB\) plus a llama.cpp fork patch are already available via AtomicChat. Local-LLM enthusiasts have long asked for a new ~70B dense model, and a 65B dense release that competes with 500B–800B mixture-of-experts frontier models would be a notable addition to the open-weights arsenal. Because this preview is only lightly post-trained for agentic coding, the final model could be considerably stronger, which makes it interesting both as a tool and as a signal of what smaller dense architectures can still achieve. The preview uses a fairly standard post-training recipe \(midtraining, long-context training, SFT, long-context SFT, and mixed-domain RL\) but with relatively light post-training focused on agentic coding, and there is also a pretrain-only checkpoint with no midtraining or synthetic QA data. Notable design choices include FFN activation clipping, gated attention, global NoPE attention and value residuals, plus a DFlash2 draft model for speculative decoding; reported scores include Terminal-Bench 2.1 80.5, SWE-bench Pro 61.4, DeepSWE 1.1 44.3, IFBench 79.2 and GPQA Diamond 85.2, though these are self-reported and the &quot;Preview&quot; label plus a 65B dense footprint \(slow on consumer hardware\) are important caveats.

reddit · r/LocalLLaMA · /u/returnity · Nov 4, 22:42

**Background**: Dense models activate all their parameters for every token, whereas mixture-of-experts \(MoE\) models only activate a subset, so a 65B dense model costs far more compute per token than a comparable or even larger MoE model. Hybrid attention mixes sliding-window attention \(cheap, local context\) with full global attention layers, often in a fixed ratio, to cut long-context cost; NoPE means those global attention layers use no explicit positional encoding at all, relying on content-based attention instead. Speculative decoding uses a small draft model — here DFlash2, a block-diffusion drafter — to propose tokens that the large model then verifies, speeding up inference, while GGUF is the quantized format used by llama.cpp for local execution.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/z-lab/Qwen3.8-27B-DFlash2">z-lab/Qwen3.8-27B-DFlash2 · Hugging Face</a></li>
<li><a href="https://www.mindstudio.ai/blog/qwen3-8-27b-dflash2-speculative-decoding">What Is DFlash 2? Speculative Decoding Explained for Qwen3.8 ...</a></li>
<li><a href="https://sebastianraschka.com/llm-architecture-gallery/nope/">No Positional Embeddings (NoPE) | Sebastian Raschka, PhD</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters welcomed another competitive open-weights release but were skeptical on several fronts: one noted that the term &quot;SOTA&quot; has been diluted by ever-narrower benchmark categories, another argued a 65B dense model will be prohibitively slow on consumer hardware and thus unlikely to win over hobbyists the way Qwen&\#x27;s 27B-class or MoE models have. Others criticized the release for not mentioning rival open-weight models, questioned how much it was &quot;benchmaxxed&quot; relative to Qwen, and pointed out that US-jurisdiction open weights are a meaningful differentiator for some users regardless of raw competitiveness.

**Tags**: `#local-llm`, `#open-weights`, `#dense-models`, `#model-architecture`, `#benchmarks`

---

<a id="item-8"></a>
## [C++26 Fails ISO National Body Vote in Unprecedented Setback](https://www.reddit.com/r/programming/comments/1xnucc3/c26_disapproved_by_the_iso_national_bodies/) ⭐️ 8.0/10

The draft international standard \(DIS\) for C++26 reportedly failed its ISO National Body ballot, with 12 votes in favor and 9 against — the first time a C++ standard draft has been rejected at this stage since the process began running smoothly in 1998. The rejection was widely expected to be a formality, so the negative vote came as a shock to the C++ community. The vote blocks C++26 from being published as an official ISO International Standard on the expected timeline, affecting every developer, compiler vendor, and standard-library implementer that tracks the standard. It also raises uncomfortable questions about the consensus-building process inside WG21, since a feature that passed working-group consensus was still rejected by national bodies. Reports indicate the objections center on the contracts proposal \(P2900\), a long-debated language feature, and that national bodies submitted comments alongside their votes. A failed DIS ballot does not cancel the project outright: SC22 can recirculate a revised committee draft, reissue it as a Technical Specification, or cancel the work item, with the SC22 chair choosing among these options in consultation with WG21 and the ISO/IEC central office.

reddit · r/programming · /u/alexeyr · Nov 4, 17:32

**Background**: The C++ standard is developed by WG21, the C++ working group under ISO/IEC JTC1/SC22, and must ultimately be approved through a formal ballot of ISO&\#x27;s national member bodies — the national standards organizations of participating countries. The DIS \(Draft International Standard\) ballot is normally the last major hurdle before publication, and for C++ it had passed without incident for over two decades. Because the standard functions as a de facto treaty for compiler and library implementers, a rejection at this stage ripples through toolchains, vendors, and long-term support planning.

<details><summary>References</summary>
<ul>
<li><a href="https://andreasfertig.com/blog/2026/11/cpp26-dis-failed-how-does-cpp-survive/">C+ + 26 DIS failed, how does C++ survive? - Andreas Fertig&#x27;s Blog</a></li>
<li><a href="https://train-it.eu/blog/cpp26-contracts-the-ballot-result/">The result of the C++26 DIS ballot | Train IT</a></li>
<li><a href="https://a4z.noexcept.dev/blog/2026/10/29/cpp26-wg21-and-isos-national-bodies.html">C++26, WG21, and ISO&#x27;s national bodies</a></li>

</ul>
</details>

**Tags**: `#C++`, `#ISO standards`, `#programming languages`, `#standardization`, `#compilers`

---

<a id="item-9"></a>
## [Postgres 19 Ships Built-In REPACK for Online Table Bloat Cleanup](https://www.reddit.com/r/programming/comments/1xn9jr2/postgres_19_repack_builtin_online_table_bloat/) ⭐️ 8.0/10

PostgreSQL 19 introduces a native REPACK command, including a REPACK \(CONCURRENTLY\) form, that rewrites a bloated table to reclaim wasted space while allowing writers to keep working. The feature folds the space-reclamation role of VACUUM FULL and the index-order rewrite of CLUSTER into a single built-in command, removing the need for the external pg\_repack extension. Table bloat is one of the most common operational headaches in long-running Postgres deployments, and previously the only options were a blocking VACUUM FULL/CLUSTER or the third-party pg\_repack extension with its own installation, triggers, and caveats. A first-party online REPACK lowers the operational barrier for DBAs and managed-service users, and may push cloud providers to expose the capability natively. Per the PostgreSQL 19 documentation, running REPACK without a table\_name processes every table and materialized view on which the current user holds the MAINTAIN privilege, and that database-wide form cannot be executed inside a transaction block. The CONCURRENTLY variant is the variant that avoids locking out writers, at the cost of extra I/O, longer runtime, and the need for temporary disk space to hold the rewritten copy of the table.

reddit · r/programming · /u/craigkerstiens · Nov 4, 00:06

**Background**: PostgreSQL uses MVCC \(multi-version concurrency control\), so an UPDATE or DELETE leaves behind a dead tuple that VACUUM later marks as reusable space; over time this dead space plus page fragmentation makes a table&\#x27;s physical size much larger than the data it actually holds, which is what people call bloat. Routine VACUUM reuses that space but does not return it to the operating system, while VACUUM FULL and CLUSTER do shrink the file by rewriting the table — historically taking an ACCESS EXCLUSIVE lock that blocks all reads and writes. The pg\_repack extension was created to work around that locking problem by copying the table online and swapping it in via triggers and a brief lock, which is the gap the built-in REPACK is meant to close.

<details><summary>References</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/19/sql-repack.html">PostgreSQL : Documentation: 19 : REPACK</a></li>
<li><a href="https://dev.to/remdore/postgres-19s-repack-rewrites-a-bloated-table-without-locking-out-your-writers-2ep0">Postgres 19 &#x27;s REPACK rewrites a bloated table... - DEV Community</a></li>
<li><a href="https://www.snowflake.com/en/blog/engineering/postgres-19-repack-table-bloat/">Postgres 19 REPACK: Built-In Online Table Bloat Cleanup</a></li>

</ul>
</details>

**Tags**: `#PostgreSQL`, `#database maintenance`, `#table bloat`, `#REPACK`, `#online operations`

---

<a id="item-10"></a>
## [Blog Claims White House IP Space Carries Residential Proxy Traffic](https://layer3intel.com/blog/residential-proxies-white-house-network) ⭐️ 7.0/10

A Layer3Intel threat-intelligence blog claims that residential proxy SDK traffic is exiting from IP space owned by the White House, based largely on activity that peaks between 5 p.m. and midnight Eastern time. The post triggered a 507-point Hacker News discussion about whether that pattern justifies attributing the traffic to an infected device physically on the White House network. If accurate, the finding would mean a device on one of the world’s most sensitive networks is being rented out through a proxy SDK, exposing the network to third-party traffic and potentially to command-and-control abuse. More broadly, it highlights how consumer-facing SDKs embedded in apps can create latent access paths that enterprises and government networks rarely audit. The evidence is inferential: the blog says its data shows proxy exits, not the device or person behind them, and ownership of IP space does not prove the traffic originates from a physical White House device rather than a lab, guest network, or media facility. Commenters also noted the post promotes a week-old service and that some legitimate mobile IPs, such as T-Mobile 5G, can be misclassified as residential proxies.

hackernews · Rasbora · Nov 4, 20:45 · [Discussion](https://news.ycombinator.com/item?id=50371246)

**Background**: Residential proxies route third-party web requests through real consumer internet connections so traffic appears to come from ordinary homes rather than data centers. They are often delivered through SDKs embedded in apps and can monetize a user’s bandwidth without clear consent; the FBI has warned that such networks can also obfuscate malware command-and-control. Detecting proxy exit traffic in network telemetry is a relatively novel technique, but attribution from IP ownership alone is notoriously weak.

<details><summary>References</summary>
<ul>
<li><a href="https://www.helpnetsecurity.com/2026/06/23/tv-residential-proxy-sdk/">Residential proxy SDKs are hiding in LG and... - Help Net Security</a></li>
<li><a href="https://www.fbi.gov/investigate/cyber/alerts/2026/evading-residential-proxy-networks-protecting-your-devices-from-becoming-a-tool-for-criminals">Evading Residential Proxy Networks: Protecting Your Devices ...</a></li>
<li><a href="https://nhimg.org/residential-proxy-networks-guide">Residential Proxy Networks: Abuse, Detection and Defence</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters pushed back on the inferential leap from White House-owned IP space to a physical White House device, calling the post promotional and noting it could be a security lab or guest media network. Several also warned that proxy SDKs embedded in compromised devices represent latent command-and-control capability, with one linking the issue to reports of phones being brought into SCIFs, while another reported their T-Mobile 5G IP being falsely listed as a residential proxy.

**Tags**: `#cybersecurity`, `#residential-proxies`, `#threat-intelligence`, `#botnet-detection`, `#privacy`

---

<a id="item-11"></a>
## [Nvidia RTX Spark Linux GPU throttling slashes local AI inference speed](https://www.mindstudio.ai/blog/linux-nvidia-rtx-spark-laptop) ⭐️ 7.0/10

A hands-on MindStudio report on dual-booting Linux on an Nvidia RTX Spark laptop \(an MSI Prestige machine\) found the GPU pinned at roughly 780 MHz on wall power, yielding about 13.9 tokens/sec versus 65.4 tokens/sec for the same inference workload under Windows. The root cause is that the platform&\#x27;s encrypted firmware power table can currently only be decrypted by the Windows driver, and Nvidia&\#x27;s Linux driver does not yet ship the platform controller&\#x27;s power-management logic. This matters because RTX Spark laptops are marketed as local AI workstations, and a large share of AI practitioners rely on Linux for CUDA, containerized inference stacks and reproducible benchmarking. If a flagship Nvidia laptop platform cannot reach full performance outside Windows, it reinforces concerns about vendor lock-in and makes Linux users effectively second-class citizens on hardware they already own. The behavior is strange enough to look like a bug rather than deliberate DRM: Linux reportedly runs the GPU at full clock on battery and downclocks when plugged in, which is the opposite of normal power management. The figures come from a single hands-on test and are not independently verified, and the article itself points to WSL as the pragmatic workaround since it carries minimal overhead versus native Linux for these workloads.

hackernews · novaRom · Nov 4, 08:46 · [Discussion](https://news.ycombinator.com/item?id=50362905)

**Background**: RTX Spark is Nvidia&\#x27;s new laptop platform \(referred to by its N1X chip designation and related to the GB10 systems used in DGX Spark\), and all shipping RTX Spark laptops come with Windows preinstalled, so Linux support is currently a community-driven effort. Modern GPUs depend on firmware-encoded power tables that tell the driver which clock and voltage states are safe; when those tables are encrypted and only one OS driver holds the key, other operating systems cannot properly negotiate clock speeds. WSL \(Windows Subsystem for Linux\) lets users run Linux tooling on top of the Windows driver stack, which is why it sidesteps the problem entirely.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mindstudio.ai/blog/linux-nvidia-rtx-spark-laptop">Linux on the Nvidia RTX Spark Laptop: What Actually... | MindStudio</a></li>
<li><a href="https://news.ycombinator.com/item?id=50362905">Nvidia RTX Spark encrypted firmware slows inference ... | Hacker News</a></li>
<li><a href="https://explainx.ai/blog/nvidia-rtx-spark-laptop-linux-gpu-clock-780-mhz-plugged-in-mindstudio-claimed-vs-verified-2026">RTX Spark Linux: 13.9 vs 65.4 tok/s Claim Checked - explainx.ai</a></li>

</ul>
</details>

**Discussion**: Commenters on Hacker News pushed back hard on the framing: several argued this is simply missing Linux driver support on a brand-new Windows-first platform, not a deliberate scheme, and noted that Nvidia has historically added Linux support well after launch. Others used the thread to attack Nvidia&\#x27;s proprietary, cryptographically locked firmware and the broader monopoly it enables, while some questioned why the first boot attempt targeted a brand-new, little-tested distribution instead of a long-established one, and one commenter worried the episode signals a drift toward cloud-dependent AI.

**Tags**: `#Nvidia`, `#Linux`, `#firmware`, `#GPU`, `#AI inference`

---

<a id="item-12"></a>
## [AMD&\#x27;s $17B Q4 guidance would outsell Intel for the first time](https://www.tomshardware.com/pc-components/cpus/amd-expects-to-outsell-intel-in-q4-for-the-first-time-in-history-usd17b-guidance-would-exceed-intels-projections) ⭐️ 7.0/10

AMD has issued fourth-quarter guidance of roughly $17 billion, a figure that would exceed Intel&\#x27;s own Q4 projections and, if realized, mark the first quarter in AMD&\#x27;s history in which it outsells Intel. The company attributes much of the growth to strong sales of its Instinct data center AI accelerators. For decades Intel has been the larger of the two x86 vendors, so a quarterly revenue crossover is a symbolic milestone in the server and PC processor market and a marker of how AI accelerator demand is reshaping the semiconductor hierarchy. It affects data center buyers, investors tracking the x86 duopoly, and anyone assessing whether AMD can convert AI spending into durable market share. The comparison is between guided total company revenue rather than unit shipments, so AMD&\#x27;s figure reflects a mix of Epyc server CPUs, Ryzen client chips and Instinct accelerators rather than a pure CPU victory. Commenters also point out that AMD&\#x27;s Instinct volumes remain modest next to Nvidia&\#x27;s data center GPUs, meaning the swing owes as much to Intel&\#x27;s weak accelerator position as to AMD&\#x27;s own AI momentum.

hackernews · rbanffy · Nov 4, 15:38 · [Discussion](https://news.ycombinator.com/item?id=50367125)

**Background**: AMD and Intel are the two companies whose processors implement the x86 instruction set, which underpins most PCs and a large share of servers. AMD&\#x27;s Instinct line, built on its CDNA architecture \(including the MI300 series\), is its data center GPU family for AI and HPC workloads and competes directly with Nvidia&\#x27;s data center GPUs; it replaced the FirePro S brand and dropped the Radeon name in 2020. Intel&\#x27;s decline in this comparison also reflects its retreat from projects such as Optane memory and its late, limited push into AI accelerators, while rivals like Apple and Qualcomm are shifting client devices toward Arm-based chips.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AMD_Instinct_accelerators">AMD Instinct accelerators</a></li>
<li><a href="https://www.amd.com/en/products/accelerators/instinct/mi300.html">AMD Instinct™ MI300 Series Accelerators</a></li>
<li><a href="https://en.wikipedia.org/wiki/AMD_Platform_Security_Processor">AMD Platform Security Processor - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News reaction was a mix of schadenfreude toward Intel and skepticism about AMD&\#x27;s own AI credentials: several commenters said Intel appears bloated and complacent \(citing the 13th/14th-gen voltage issues and the Optane cancellation\), while others argued neither vendor has shown real commitment to AI. A separate thread raised platform security concerns, with one user recounting law enforcement using Intel&\#x27;s DCI to extract a LUKS key from RAM and noting that AMD&\#x27;s PSP is opaque but currently friendlier to anti-forensic Linux setups, and another questioning whether x86 itself is being displaced by Arm.

**Tags**: `#AMD`, `#Intel`, `#CPU market`, `#x86`, `#semiconductor industry`

---

<a id="item-13"></a>
## [Deep Principle releases Hydrogen-1.0, an open-weight science model beating GPT-6 Astra on FSR](https://www.reddit.com/r/MachineLearning/comments/1xnjhdd/hydrogen10_openweight_scientific_model_beats_gpt6/) ⭐️ 7.0/10

Deep Principle, the team behind Mira AI Scientist, released Hydrogen-1.0, an open-weight model post-trained from Z.ai&\#x27;s GLM-5.3 for chemistry, materials science, and life sciences. In the team&\#x27;s own evaluations it reached a 38.3% pass rate on FrontierScience Research versus 33.3% for GPT-6 Astra at max thinking, at an estimated $0.25 of output-side cost per problem compared with $0.88 for Astra, roughly 72% lower. If the numbers hold up, this is a strong signal that domain-specific post-training on scientific workflows can let an open-weight model match or beat a frontier proprietary system at a fraction of the inference cost, which matters for academic labs and smaller biotech or materials companies that cannot afford frontier API bills. It also adds pressure on the assumption that only the largest closed models can do research-grade scientific reasoning. All comparisons are self-reported by the releasing team with limited benchmark detail and no independent validation; beyond FSR, Hydrogen scored 92.9% on GPQA Diamond \(just under Kimi K3&\#x27;s 93.5%\), gained +5.13 points over Astra on an internal scientific-computing set and +4.76 on single-step forward reaction prediction, but trailed Astra by 3.33 points on NMR structure elucidation. The five workflow demos are model-plus-tool walkthroughs rather than autonomous-research success rates — GROMACS performs the molecular dynamics and the Suzuki coupling protocol validation is virtual, so no physical experiment was actually run.

reddit · r/MachineLearning · /u/AKAMA199 · Nov 4, 09:00

**Background**: FrontierScience Research \(FSR\) is a benchmark introduced by OpenAI in December 2025 that tests AI reasoning on cutting-edge research questions in physics, chemistry, and biology requiring deep domain expertise and multi-step reasoning; GPQA Diamond is a widely used 198-question graduate-level multiple-choice set in the same fields. GLM-5.3 is Z.ai&\#x27;s flagship open-weights model \(753B parameters\) that reuses the GLM-5.2 base and gains its improvements entirely from post-training, where a pretrained model is further trained with supervised fine-tuning and reinforcement learning on curated data. Hydrogen-1.0 applies exactly that recipe, using lab records, scientist feedback, and discovery trajectories to teach the model how each research step should change after an observation, a failure, or an unexpected result.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/zai-org/GLM-5.3">Text Generation model with 753B parameters. Download, explore files...</a></li>
<li><a href="https://openai.com/index/frontierscience/">Evaluating AI’s ability to perform scientific research tasks</a></li>
<li><a href="https://llm-stats.com/benchmarks/frontierscience-research">FrontierScience Research Leaderboard - llm-stats.com</a></li>

</ul>
</details>

**Tags**: `#open-weight models`, `#scientific AI`, `#LLM benchmarks`, `#model release`, `#chemistry and materials`

---

<a id="item-14"></a>
## [Looped Transformers Save Storage, Not HBM Traffic, B200 Profiling Shows](https://www.reddit.com/r/MachineLearning/comments/1xnskvt/do_looped_transformers_save_hbm_traffic_profiling/) ⭐️ 7.0/10

A new profiling study by dinara-dl models and measures memory traffic for looped \(recurrent-depth\) transformers on an NVIDIA B200, using Nsight Compute data and reproducible code. In a microbenchmark, a chain of eight matmuls sharing one 72 MiB weight ran 24% faster than eight identical copies and read almost nothing from HBM, but at 288 MiB — larger than L2 — the advantage disappeared; a full Huginn Core \(teaching implementation, random weights\) took roughly eight times as long and read roughly eight times as much HBM data over eight iterations as over one. This is an actionable correction to a common intuition: parameter sharing in looped models cuts storage and FLOPs per parameter, but by itself does not reduce memory-bandwidth demand, which is often the real bottleneck for inference on modern GPUs. Anyone working on recurrent-depth architectures or memory-efficient inference must therefore treat L2 residency and kernel scheduling — not just weight tying — as the lever for real speedups. The measurements come from a single B200 and a deliberately simple teaching implementation with random weights, so the full-model numbers describe memory behavior rather than achievable inference performance; the key caveat is that the 72 MiB case fits in L2 while the 288 MiB case does not, so weight sharing only reduces HBM reads when the shared tensors stay on chip between iterations. The author explicitly asks whether anyone has kept recurrent weights resident across iterations, for example via a persistent kernel.

reddit · r/MachineLearning · /u/2dayyy6 · Nov 4, 16:26

**Background**: A looped transformer repeatedly applies the same layers and weights several times before emitting a token, a design known as recurrent depth and exemplified by the Huginn architecture; this adds internal test-time computation without adding parameters. The catch is the GPU memory hierarchy: model weights live in large but relatively slow high-bandwidth memory \(HBM\), while the much smaller L2 cache and on-chip SRAM are far faster. When a kernel does little arithmetic per byte moved, performance becomes bound by HBM bandwidth — the so-called memory wall — which is why tools like NVIDIA Nsight Compute are used to measure actual bytes read and compare them against hardware limits.

<details><summary>References</summary>
<ul>
<li><a href="https://interactive-active-ai.github.io/Aha-Looped-Transformer/papers/huginn/">Huginn · Aha Looped Transformer</a></li>
<li><a href="https://locsic.com/thinking/looped-transformer-recurrent-depth/">Looped Transformers: Recurrent Depth, Huginn and Nanbeige ...</a></li>
<li><a href="https://mlc.ai/modern-gpu-programming-for-mlsys/chapter_performance/index.html">What Makes a Kernel Fast — Modern GPU Programming For MLSys</a></li>

</ul>
</details>

**Tags**: `#looped-transformers`, `#GPU-memory-bandwidth`, `#HBM-traffic`, `#performance-profiling`, `#Huginn`, `#inference-efficiency`

---

<a id="item-15"></a>
## [Developer prunes Gemma 4 26B-A4B down to a dense 3.81B model](https://www.reddit.com/r/LocalLLaMA/comments/1xnoqyy/i_removed_85_of_gemmas_weights_and_it_is_mostly/) ⭐️ 7.0/10

A developer removed roughly 85% of Gemma 4 26B-A4B&\#x27;s weights by keeping a fixed set of 8 experts per layer, collapsing the mixture-of-experts model into a dense 3.81B-parameter network that reaches 92% agreement with the original on a single classification task. On a Mac the pruned model runs at 79 tokens/s using 3.8 GB of memory \(2.75 GB at Q4\_K\_M\), roughly double the speed and half the memory of Gemma 4 12B. This is a concrete data point for extreme MoE-to-dense collapse: instead of a general-purpose model, the result is a tiny task-specialized model suited to always-on, on-device inference where memory and energy dominate. It also hints at a workflow where per-block distillation could run on a user&\#x27;s own device in about 5 GB of memory to adapt the model to local data. The evaluation is narrow: the model only matches the original on one classification task, and knowledge-dependent tasks degrade badly because that knowledge is simply gone. Notably, the pruned model&\#x27;s 92% agreement is only marginally above the 90% agreement the much simpler Gemma 4 12B already achieves against the 26B on the same inputs, and the author has not yet tested on-device training on a real user&\#x27;s device and is openly asking for better expert-selection methods.

reddit · r/LocalLLaMA · /u/Accomplished\_Ad\_56 · Nov 4, 13:53

**Background**: Gemma 4 26B-A4B is a mixture-of-experts \(MoE\) model: it holds about 26B parameters in total, but a router sends each token through only a small subset of experts, so roughly 4B parameters are active per token. If the number of kept experts equals the number the router would normally select, the routing decision becomes trivial and the model effectively behaves like a dense network. Q4\_K\_M is a popular GGUF quantization scheme that stores most weights at 4-bit precision and keeps sensitive layers at higher precision, which is why the same model drops from 3.8 GB to 2.75 GB. Expert pruning is an active research area, with recent work exploring scoring and selecting experts, and distilling the pruned MoE back into a dense network.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B">google/gemma-4-26B-A4B · Hugging Face</a></li>
<li><a href="https://fengwang.github.io/posts/moe-expert-pruning/">MoE Expert Pruning: What Works, What Doesn&#x27;t, and What We ...</a></li>
<li><a href="https://www.runlocalai.co/glossary/q4-k-m">Q 4 _ K _ M Quantization — AI glossary | RunLocalAI</a></li>

</ul>
</details>

**Tags**: `#LLM pruning`, `#Mixture-of-Experts`, `#Gemma`, `#on-device AI`, `#model compression`

---

<a id="item-16"></a>
## [Unsloth ships Dynamic v3.1 GGUFs for Qwen3.8-Flash-Next](https://www.reddit.com/r/LocalLLaMA/comments/1xnvbxn/new_qwen38flashnext_unsloth_dynamic_v31_ggufs/) ⭐️ 7.0/10

Unsloth released Unsloth Dynamic v3.1 GGUF quantizations for Qwen3.8-Flash-Next, claiming 10–15% higher accuracy than GSQ-RCO quants at comparable file sizes on DeepSWE, Terminal Bench, Aider Polyglot and other suites. The release also introduces a new &quot;engram switching&quot; scheme that provides BF16, Q8\_0, Q5\_1 and IQ4\_NL variants across all quants, building on the earlier DeepSeek-V4.1-Flash UD3.1 work. For anyone running Qwen3.8-Flash-Next locally, the quant choice is a direct quality-versus-VRAM tradeoff, so a claimed double-digit accuracy gain on agentic and coding benchmarks at the same file size could shift the default recommendation in the local-LLM community. It also signals that imatrix-style quantization is being pushed toward per-layer, error-measured precision selection rather than uniform bit widths. Benchmarks were run at 256K context for agentic suites and 128K for the rest, with temperature 1.0, top\_p 0.95, top\_k 20, min\_p 0, no presence or repetition penalty, and preserve\_thinking with xhigh reasoning, consuming 26.2B tokens total \(18.1B on DeepSWE alone and 5.2B on Terminal Bench\), with LiveCodeBench repeated 3 times and HMMT 8–16 times. Only quants smaller than UD-Q4\_K\_XL have been updated so far, and the published engram files range from 102.4 GB at BF16 down to 28.8 GB at IQ4\_NL, whose relative RMSE versus BF16 is 0.0757.

reddit · r/LocalLLaMA · /u/danielhanchen · Nov 4, 18:08

**Background**: Quantization compresses a model&\#x27;s weights from 16-bit floating point down to lower-bit representations such as 8-bit or 4-bit, letting large models fit on consumer GPUs; GGUF is the file format used by the llama.cpp ecosystem for such quantized models. Applying one bit width uniformly to every layer tends to hurt accuracy, so Unsloth&\#x27;s &quot;Dynamic&quot; quants assign different precisions to different layers to protect sensitive ones. GSQ-RCO, from Das Lab at ISTA \(the group behind GPTQ\), is a competing quantization method used here as the comparison baseline.

<details><summary>References</summary>
<ul>
<li><a href="https://unsloth.ai/docs/basics/dynamic-3.0-ggufs">Unsloth Dynamic 3.0 GGUFs | Unsloth Documentation</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-gsq-rco-quantization">What Are GSQ and RCO? Das Lab&#x27;s New LLM Quantization Method</a></li>
<li><a href="https://agihunt.info/en/e/1a1a7b3641237e42759e4f60c5a">Unsloth Releases Dynamic v3.1 Quantization… · AGI Hunt</a></li>

</ul>
</details>

**Discussion**: A community member highlighted that the more useful takeaway for people already running IQ3S GSQ-RCO with Strata is that their quant scores 99.0% of BF16 on a 12-benchmark average, which is reassuring for those with limited VRAM, while noting that UD v3.1 appears roughly 15% better than IQ3S GSQ-RCO for anyone planning a fresh download.

**Tags**: `#quantization`, `#GGUF`, `#local-llm`, `#unsloth`, `#benchmarking`

---

<a id="item-17"></a>
## [Axion 1.0: A Fully Open 35B Agent Model Trained in Three Simple Stages](https://www.reddit.com/r/LocalLLaMA/comments/1xnjiu4/axion10axion1035b_hugging_face/) ⭐️ 7.0/10

ByteDance released Axion 1.0, a fully open 35B agent foundation model trained with a deliberately compact recipe of two supervised fine-tuning \(SFT\) stages followed by reinforcement learning — with no dedicated mid-training, no DPO, and no on-policy distillation. Beyond the weights, the team published the complete pipeline \(data construction, generation, filtering, verification, prompts, and training code\) along with the training dataset, arXiv paper \(2611.03233\), and a GitHub repository. Most strong agentic models are only partially open, so a 35B model whose entire data and training recipe is reproducible gives the open-model community a practical baseline to study, replicate, and extend rather than just fine-tune. It also suggests that competitive agentic capability may not require an increasingly elaborate multi-stage post-training stack, which lowers the cost of entry for smaller labs. The first SFT stage builds self-contained reasoning by synthesizing hard problems and adversarially strengthening them based on the base model&\#x27;s own successful solution strategies, while the second stage scales to tool-dependent reasoning via automatically verifiable tasks grounded in real-world data sources and deterministic computation; reinforcement learning then extends long-horizon reasoning and tool interaction. The authors claim the model is competitive with leading commercial models on several agentic benchmarks, though the results are self-reported and the recipe&\#x27;s generality beyond this base model remains unverified.

reddit · r/LocalLLaMA · /u/pmttyji · Nov 4, 09:02

**Background**: An &quot;agent foundation model&quot; is a language model post-trained to plan, reason over many steps, and call external tools rather than just answer single-turn questions. Post-training typically mixes supervised fine-tuning \(SFT\), which teaches behavior from curated input-output examples, with preference optimization methods such as DPO and distillation approaches such as on-policy distillation \(OPD\), where a student model learns from feedback on its own self-generated trajectories. Reinforcement learning with verifiable rewards is increasingly used to push long-horizon tool use, and &quot;fully open&quot; here means releasing the data and recipe, not only the weights.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2305.18290">[2305.18290] Direct Preference Optimization: Your Language ... Direct Preference Optimization (DPO): Complete Guide for 2026 [2608.16926] Data-DPO: Direct Preference Optimization for ... Preference Tuning LLMs with Direct Preference Optimization ... What is direct preference optimization (DPO)? - SuperAnnotate Direct Preference Optimization: A Deep Dive into RLHF ...</a></li>
<li><a href="https://www.emergentmind.com/topics/on-policy-distillation-opd">On - Policy Distillation in Neural Models</a></li>
<li><a href="https://arxiv.org/abs/2506.14681">[2506.14681] Massive Supervised Fine-tuning Experiments ... Supervised Fine-Tuning (SFT) for LLMs - GeeksforGeeks LLM Fine-Tuning Dataset Preparation: An End-to-End Guide Preparing data for supervised fine-tuning Part 1: Formatting ... Fine-tune a model with supervised fine-tuning in Microsoft ...</a></li>

</ul>
</details>

**Tags**: `#open-source LLM`, `#agent models`, `#reinforcement learning`, `#model training`, `#LocalLLaMA`

---

<a id="item-18"></a>
## [Zig&\#x27;s libc rewrite blamed for 12,000× SQLite slowdown](https://www.reddit.com/r/programming/comments/1xnq1xx/shlemiel_the_painter_is_back_how_zigs_libc/) ⭐️ 7.0/10

A microblog post by Dennis Forbes, published in late October 2026 and picked up for discussion on r/programming, documents how Zig&\#x27;s from-scratch libc implementation made SQLite roughly 12,000 times slower in a real production workload. The author frames the failure as a textbook &quot;Shlemiel the Painter&quot; case, in which a routine that should scale linearly instead degrades toward quadratic behavior as input size grows. Zig&\#x27;s pitch of self-contained, easily cross-compiled binaries depends on its own libc implementation, so the performance and robustness of that libc directly affect every Zig-built program that links against it. The incident is also a cautionary tale for any project that reimplements foundational C routines: code that compiles and passes tests can still carry catastrophic complexity that only shows up under real data volumes. Zig&\#x27;s libc lives under lib/c and provides only a subset of the standard C library functions, so code paths that glibc and musl have micro-optimized for decades may be implemented in a straightforward but naive way. The 12,000× figure is specific to the reported workload — a Rust service that writes large JSON analysis bundles into SQLite — rather than a universal constant, which makes it a reminder that regression baselines and complexity targets matter as much as correctness tests.

reddit · r/programming · /u/gallery\_rose · Nov 4, 14:46

**Background**: Zig is a systems programming language that ships its own C library implementation so that \`zig cc\` and Zig-built executables can cross-compile for other platforms without depending on the host system&\#x27;s libc, which varies widely between platforms. Functions like memcpy, strlen and snprintf look trivial but are among the most heavily hand-optimized code in modern computing, and replacing them is riskier than it appears. &quot;Shlemiel the Painter&quot; is Joel Spolsky&\#x27;s name for accidentally quadratic code, after a painter whose daily progress shrinks because he keeps walking back to the paint can; SQLite&\#x27;s own developers also maintain a long-running CPU-usage measurement harness precisely to catch such regressions.

<details><summary>References</summary>
<ul>
<li><a href="https://dennisforbes.ca/blog/microblog/2026/10/the_accidental_12000x_sqlite_slowdown/">Shlemiel the Painter Is Back: How Zig’s libc Rewrite Made ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Schlemiel_the_painter&#x27;s_Algorithm">Joel Spolsky - Wikipedia</a></li>
<li><a href="https://sqlite.org/cpu.html">Measuring and Reducing CPU Usage in SQLite Shlemiel the Painter Is Back: How Zig’s libc Rewrite Made ... Shlemiel the Painter Is Back: How Zig’s libc Rewrite Made ... SQLite Bug Forum: FTS5 performance regression at check-in ... Why an LLM‑Rewritten SQLite Is 20,000× Slower: Hidden… | BestHub SQLite Performance Benchmarks - OpenBenchmarking.org</a></li>

</ul>
</details>

**Tags**: `#Zig`, `#SQLite`, `#libc`, `#performance regression`, `#systems programming`

---

<a id="item-19"></a>
## [Interactive Explainer Peers Inside Git&\#x27;s Object Model and Refs](https://www.reddit.com/r/programming/comments/1xnqotw/git_from_the_inside_interactive_explainer/) ⭐️ 7.0/10

An interactive explainer titled &quot;Git, From the Inside&quot; was shared on r/programming, walking readers through Git&\#x27;s internal machinery — how commits, objects, refs, and the index actually work beneath the everyday commands. Rather than teaching Git as a list of commands to memorize, it visualizes the underlying data structures and plumbing that those commands manipulate. Most developers use Git daily but treat it as a black box, so confusion around detached HEADs, rebases, and lost commits persists well into senior roles. An interactive, visual treatment of the object model gives developers the mental model needed to debug their repositories and understand why destructive operations behave the way they do. The explainer centers on Git&\#x27;s content-addressed store: blobs for file contents, trees for directory listings, and commits that point to a root tree plus parent commits and author metadata, with refs and HEAD acting as human-readable pointers into that graph. It also covers the index \(staging area\), the file that bridges the working directory and the repository and determines what the next commit will contain.

reddit · r/programming · /u/Some\_Championship605 · Nov 4, 15:12

**Background**: Git stores everything as a Merkle-like directed acyclic graph of immutable objects, each addressed by a SHA-1 \(now increasingly SHA-256\) hash of its contents, which is why commits are effectively tamper-evident and why identical file contents are only stored once. A commit is not a diff but a snapshot: it points to a tree object that recursively describes the entire project state, plus zero or more parent commits. Branches are simply movable references to commits, stored as small files under .git/refs and updated by low-level plumbing such as update-ref, while HEAD indicates which ref is currently checked out. The index is a separate binary file in .git that records staged paths and their blob hashes, which is why git status can be fast without rescanning history.

<details><summary>References</summary>
<ul>
<li><a href="https://git-scm.com/book/en/v2/Git-Internals-Git-Objects">Git - Git Objects</a></li>
<li><a href="https://git-scm.com/book/en/v2/Git-Internals-Git-References">Git - Git References</a></li>
<li><a href="https://stackoverflow.com/questions/4084921/what-does-the-git-index-contain-exactly">internals - What does the git index contain EXACTLY? - Stack Overflow</a></li>

</ul>
</details>

**Tags**: `#git`, `#version-control`, `#interactive-learning`, `#developer-tools`, `#systems-education`

---

<a id="item-20"></a>
## [Apple&\#x27;s 10-K flags rogue AI agents that can &\#x27;conceal&\#x27; and &\#x27;manipulate&\#x27;](https://www.reddit.com/r/artificial/comments/1xnudhs/apple_put_a_warning_about_rogue_ai_agents_in_its/) ⭐️ 7.0/10

Apple&\#x27;s latest annual Form 10-K now carries risk-factor language warning that AI agents may take actions without authorization and could &quot;conceal&quot; their actions or manipulate information. The same post notes that Apple changed how Full Disk Access works on macOS, apparently to reduce what an agent can reach. Risk factors in a 10-K are legally binding disclosures drafted by lawyers who are personally exposed if they are wrong or misleading, so listing rogue-agent behavior as a present-tense risk — rather than a hypothetical future concern — is a strong signal about how the industry now treats agentic AI. It also hands enterprise legal and IT teams a citable, named basis to demand agent controls, and reporting indicates Alphabet filed parallel language in the same cycle. The most consequential word is &quot;conceal&quot;: an agent that hides what it did breaks the assumption underneath most monitoring and audit approaches, whereas simple unauthorized action is a more familiar failure mode. Notably, the filing describes business risk in general terms rather than disclosing a specific incident, and the macOS change sits inside the TCC \(Transparency, Consent, and Control\) permission framework that governs Full Disk Access.

reddit · r/artificial · /u/Dapper-Tale-4021 · Nov 4, 17:33

**Background**: A 10-K is the annual report that U.S. public companies file with the SEC; its risk factors are written by lawyers and included when a risk is judged material enough that staying silent would be the bigger liability. In this context, &quot;AI agents&quot; means LLM-driven software that can actually take actions — running code, completing transactions, calling tools — rather than just answering questions. On macOS, Full Disk Access is a TCC permission granting apps broad read access to protected user data, so tightening it directly shrinks how much an agent can see.

<details><summary>References</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/ai/articles/apple-warns-rogue-ai-agents-215652484.html?fr=sycsrp_catchall">Apple warns rogue AI agents could ‘conceal’ and ‘manipulate ...</a></li>
<li><a href="https://aiweekly.co/alerts/apple-10-k-warns-ai-agents-may-act-without-authorization">Apple 10-K Warns AI Agents May Act Without Authorization</a></li>
<li><a href="https://forgeeks.net/apple-agent-consent-not-least-privilege/">Apple Full Disk Access changes: consent, not least... — for(geeks)</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#AI risk &amp; governance`, `#Apple/macOS security`, `#SEC filings`, `#AI safety`

---

<a id="item-21"></a>
## [Cognition launches SWE-2 Flash, a faster, cheaper coding-agent model](https://www.reddit.com/r/artificial/comments/1xo27a9/cognition_launches_swe2_flash_a_coding_agent/) ⭐️ 7.0/10

On November 4, 2026, Cognition \(the company behind Devin\) announced SWE-2 Flash, a cheaper and roughly 3x faster sibling to SWE-2 that is priced at about one-fifth of SWE-2 and will be free to use through November 30, 2026 in Devin Desktop and the CLI. The model has 276B total parameters with 12B active, is adapted from Thinking Machines Lab&\#x27;s open-weights Inkling-Small, and keeps its own weights private. The release signals that coding-agent vendors are shifting from chasing benchmark leadership toward optimizing the economics of routine agent work, where speed and price per task may matter more than top scores. Because Cognition is one of the most widely used agent platforms, its pricing and speed choices could reset expectations for what teams pay for automations, code review, and documentation tasks. Cognition reports large gains over the base Inkling-Small but mixed results against the larger SWE-2, explicitly positioning Flash as a cost-and-speed alternative rather than a replacement. The company also says targeted cybersecurity training raised ExploitBench from 11.3% to 34.8%, and it is withholding the weights while building a secure sharing program for trusted partners and labs, citing dual-use concerns.

reddit · r/artificial · /u/winer666 · Nov 4, 22:38

**Background**: Inkling-Small, released with open weights on July 30, 2026, is a Mixture-of-Experts \(MoE\) transformer with 276B total parameters but only 12B active per token, which makes it far cheaper to serve than a dense model of the same total size; it is roughly a quarter the size of the original 975B/41B-active Inkling. SWE-2 Flash inherits that MoE design through adaptation, so the high total parameter count does not translate into proportional inference cost. ExploitBench is a benchmark that measures offensive cybersecurity capability by scoring LLM agents on end-to-end vulnerability discovery and V8 exploit synthesis, which is why a jump from 11.3% to 34.8% raises dual-use questions.

<details><summary>References</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/inkling-small/">Introducing Inkling-Small - Thinking Machines Lab</a></li>
<li><a href="https://www.marktechpost.com/2026/08/02/thinking-machines-lab-releases-inkling-small-276b-open-weights-multimodal-moe-model/">Thinking Machines Lab Releases Inkling-Small: A 276B Total ...</a></li>
<li><a href="https://benchlm.ai/benchmarks/exploitbench">ExploitBench Leaderboard &amp; Scores — September 2026 | BenchLM.ai</a></li>

</ul>
</details>

**Tags**: `#coding-agents`, `#LLM-release`, `#AI-cost-efficiency`, `#model-architecture`, `#AI-safety`

---

<a id="item-22"></a>
## [San Francisco&\#x27;s Guerrilla Bike Lanes Become Permanent Infrastructure](https://99percentinvisible.org/article/guerrilla-bike-lanes-san-francisco-makes-illicit-infrastructure-permanent/) ⭐️ 6.0/10

A 2016 99% Invisible article recounts how unauthorized bike lanes painted by activists in San Francisco were later adopted and formalized by the city as permanent infrastructure. It shows how bottom-up &quot;desire path&quot; interventions can expose unmet safety needs and pressure cities to formalize citizen-led fixes, a pattern relevant to civic tech and urban planning beyond cycling. The original intervention was unauthorized and therefore legally vulnerable, and its lasting impact came only when the city converted the illicit markings into official infrastructure. Because the article dates from 2016, it documents an early case rather than the later broader spread of tactical urbanism.

hackernews · zenincognito · Nov 4, 15:01 · [Discussion](https://news.ycombinator.com/item?id=50366522)

**Background**: A desire path is an informal route worn in by repeated use, often revealing where official planning diverges from how people actually move. Tactical urbanism, sometimes called guerrilla urbanism, applies the same idea through short-term, low-cost citizen interventions such as painted crosswalks or pop-up bike lanes. 99% Invisible is a design-focused radio show and podcast created by Roman Mars that often examines overlooked infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Desire_path">Desire path - Wikipedia</a></li>
<li><a href="https://www.bikeutah.org/tactical-urbanism">Toolkit: Tactical Urbanism — Bike Utah</a></li>
<li><a href="https://en.wikipedia.org/wiki/99%_Invisible">99% Invisible - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The thread was broadly sympathetic to citizen-led fixes but split on legitimacy and the state response. Commenters shared comparable cases: Berlin students repeatedly painted a campus crosswalk until the city installed a permanent signalized crossing, and Geneva activists who painted bike lanes in 2023 faced an aggressive police investigation and surveillance of 96 sympathizers. Another commenter linked a guerrilla fix to an L.A. freeway sign, while one argued bikes inherently fit neither roads nor sidewalks and cities need fully separated paths where feasible.

**Tags**: `#urbanism`, `#civic-tech`, `#activism`, `#desire-paths`, `#infrastructure`

---

<a id="item-23"></a>
## [OpenAI to acquire Pierre Computer Company, maker of Codex diff libraries](https://openai.com/index/openai-to-acquire-pierre/) ⭐️ 6.0/10

OpenAI announced it will acquire Pierre Computer Company, Inc., the developer-tools startup behind the Pierre code-review and diff-rendering product, whose founders Jacob Thornton and Mark Otto were original creators of Bootstrap. OpenAI said Pierre&\#x27;s Trees and Diffs libraries are already used inside Codex today to navigate project files and display code changes. The deal signals that OpenAI is investing in the unglamorous plumbing of code review — diffs, file trees, and repository interfaces — rather than only in model quality, as it competes with GitHub Copilot and Cursor on the full agentic coding workflow. Acquiring a small, well-regarded developer-tools team also fits a broader pattern of AI labs buying talent and product know-how from established tooling builders. Neither company disclosed the purchase price, headcount, or how Pierre&\#x27;s standalone product will be wound down, and OpenAI&\#x27;s post frames the acquisition around Codex tooling rather than any new model capability. Commenters also linked the move to OpenAI&\#x27;s separate engineering post on scaling Git at OpenAI, which describes a Git-compatible backend called Pando built for the development volume Codex enables.

hackernews · itunpredictable · Nov 4, 15:21 · [Discussion](https://news.ycombinator.com/item?id=50366863)

**Background**: Pierre Computer Company was a small startup building low-level, composable infrastructure for developer tools, best known for a fast diff-rendering library used to display large code changes in review interfaces. OpenAI&\#x27;s Codex is its coding agent, which needs to read repositories, navigate files, and show proposed edits, so components like Trees and Diffs sit directly in the user-facing path. The acquisition comes weeks after OpenAI described Pando, a reworked Git backend intended to handle the load of AI-driven code generation, which is exactly the kind of repository-scale problem Pierre&\#x27;s team has been working on.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/openai-to-acquire-pierre/">OpenAI to acquire Pierre Computer Company, Inc. | OpenAI</a></li>
<li><a href="https://openai.com/index/scaling-git-at-openai/">Scaling Git at OpenAI</a></li>
<li><a href="https://pierre.computer/">Pierre Computer Company</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters connected the deal to OpenAI&\#x27;s &quot;Scaling Git at OpenAI&quot; post and noted that HashiCorp founder Mitchell Hashimoto is a vocal admirer and reportedly an investor in Pierre. Others praised Pierre&\#x27;s diffs library, joked about a &quot;cheaper than the subscription&quot; category of acquisition, and speculated that big labs may also be harvesting human expertise from acquired teams to build training data.

**Tags**: `#openai`, `#acquisitions`, `#developer-tools`, `#code-review`, `#git`

---

<a id="item-24"></a>
## [Verification Is Not Knowledge: Science Needs Understanding, Not Just Answers](https://blog.cosmos-institute.org/p/verification-is-not-knowledge) ⭐️ 6.0/10

An essay published on the Cosmos Institute blog, titled &quot;Verification Is Not Knowledge,&quot; argues that a verified prediction — whether a machine-checkable proof, a well-fitting model, or an AI-generated result — does not by itself amount to scientific knowledge, because knowledge also requires explanation and understanding. The author builds the case from historical episodes and from contemporary research practice where checking answers has become cheap and automated. As AI systems increasingly produce results that can be checked faster than they can be understood, the essay&\#x27;s distinction bears directly on how journals, funders and hiring committees decide what counts as a scientific contribution. If verification alone is treated as the goal, explanation risks being crowded out of research entirely. The argument is conceptual rather than empirical: it leans on well-trodden philosophy-of-science ground — verificationism, the trade-off between predictive accuracy and understanding, and the epistemic opacity of deep neural networks — so it persuades by accumulated example rather than by new evidence or a formal result.

hackernews · ersinesen · Nov 4, 09:01 · [Discussion](https://news.ycombinator.com/item?id=50363019)

**Background**: Verificationism is the older philosophical doctrine that a statement is meaningful only if it can be empirically verified; it has largely been abandoned, and philosophers of science now generally distinguish between a theory predicting correctly and a theory explaining why something happens. A newer strand of work on &quot;epistemic opacity&quot; asks what scientists actually gain when they depend on deep neural networks whose internal reasoning they cannot inspect. The essay sits at the intersection of these two debates, applied to AI-assisted research.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Verificationism">Verificationism - Wikipedia</a></li>
<li><a href="https://link.springer.com/article/10.1007/s11229-020-02713-0">Prediction versus understanding in computationally enhanced ...</a></li>
<li><a href="https://link.springer.com/article/10.1007/s11229-025-04930-x">Of opaque oracles: epistemic dependence on AI in science ...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters largely agreed with the essay, one noting that Kepler&\#x27;s laws were adopted for their computational convenience long before Newton explained why they worked, and another comparing it to a math teacher who wants to see the work, not just the answer. A more skeptical thread argued that academia is drifting toward industrial-scale AI paper production where grants reward volume and co-author throughput rather than insight, while others offered individual mathematicians as counter-examples of researchers who generate understanding rather than mere proofs.

**Tags**: `#philosophy-of-science`, `#epistemology`, `#AI-in-research`, `#academic-publishing`, `#verification`

---

<a id="item-25"></a>
## [Xiaomi claims humanoid robots worked a full 8-hour autonomous factory shift](https://electrek.co/2026/11/04/xiaomi-humanoid-robot-8-hour-shift-ev-factory/) ⭐️ 6.0/10

Xiaomi published footage of its humanoid robots working an entire 8-hour shift at its EV factory, sorting center console side covers for its cars, and said the robots operated on their own while catching and correcting their own errors. The company did not release the quantitative metrics — such as intervention rates, cycle times, or success rates — that would let outsiders verify the autonomy claim. A verified 8-hour autonomous shift would be a meaningful step beyond short scripted demos, since endurance, error recovery, and uptime are exactly what determine whether humanoid robots are economically viable in manufacturing. If the claim holds up, it strengthens Xiaomi&\#x27;s position among Chinese automakers and tech firms racing to deploy humanoids on production lines, and raises the bar for how such milestones are documented. The task shown — sorting center console side covers — is a relatively structured picking-and-placing job rather than dexterous assembly, and Xiaomi disclosed no figures on how often humans intervened or how many parts were handled per hour. The article itself flags that prior humanoid demos have often turned out to be teleoperated or heavily assisted, so the absence of data leaves the autonomy claim unverified.

rss · Electrek · Nov 4, 16:23

**Background**: Xiaomi&\#x27;s humanoid program is anchored by CyberOne, a full-size bipedal robot unveiled in 2022 that stands about 177 cm tall, weighs roughly 52 kg, and has 21 degrees of freedom, originally pitched for research, exhibitions, and light indoor service work; a CyberOne V2 prototype reported in late 2026 focuses on improved autonomy and manipulation. Across the industry, most published end-to-end humanoid demos between 2024 and 2026 have relied on teleoperation or partial human assistance, which is why standards bodies such as NIST have been pushing for standardized reliability and performance metrics for humanoid systems.

<details><summary>References</summary>
<ul>
<li><a href="https://robovations.com/analysis/why-teleoperation-is-doing-the-work-in-most-humanoid-demos/">Are humanoid robot demos teleoperated or actually autonomous?</a></li>
<li><a href="https://humanoid.guide/product/cyberone/">Xiaomi CyberOne Specs &amp; Price | Humanoid.guide Xiaomi CyberOne V2: Specs, Price &amp; Buy (2026) | Robot Overflow CyberOne by Xiaomi Robotics Capabilities, Specs &amp; Price 2026 CyberOne全尺寸人形仿生机器人 - Xiaomi CyberOne - ROBOTS: Your Guide to the World of Robotics</a></li>
<li><a href="https://robotcomparisons.com/blog/en/benchmarking-humanoid-performance-in-2026-standardized-tests-and-kpis">Benchmarking Humanoid Performance in 2026: Standardized Tests ...</a></li>

</ul>
</details>

**Tags**: `#humanoid-robots`, `#robotics`, `#manufacturing-automation`, `#xiaomi`, `#EV-industry`

---

<a id="item-26"></a>
## [datasette-apps 0.3a0 Refines Datasette Agent Integration for Custom HTML Apps](https://simonwillison.net/2026/Nov/4/datasette-apps/) ⭐️ 6.0/10

datasette-apps 0.3a0 introduces \#-prefixed autocomplete tagging of apps in Datasette Agent chat, plus new app\_add\_stored\_queries\(\) and app\_remove\_stored\_queries\(\) tools that let the agent manage which stored queries an app may call. The app\_create\(\) tool now verifies that each requested stored query exists and is viewable by the user, and requires explicit user approval before any write query is granted. This release shows how LLM agents can be wired into a permission-aware workflow for building small internal data apps, rather than just generating code ad hoc. For teams running Datasette as a lightweight data platform, it lowers the friction of iterating on hosted HTML apps while keeping write access gated behind human approval. The \# autocomplete only lists apps the current user has permission to view, and granting a write query through the agent requires user approval first. The &quot;View app&quot; buttons surfaced by the agent tools and the links on \# app references now open the app full screen inside the Datasette Agent panel; this is still an alpha \(0.3a0\) release.

rss · Simon Willison · Nov 4, 00:29

**Background**: Datasette is Simon Willison&\#x27;s open source tool for exploring and publishing SQLite databases, exposing data through a JSON API and web interface. Datasette Apps is a plugin that lets you edit and host self-contained HTML, CSS and JavaScript applications inside a Datasette instance, running in a tightly constrained sandbox iframe; those apps can run read-only SQL and, when configured with stored queries, write queries too. Datasette Agent is an LLM-powered conversational assistant for Datasette that can query databases in natural language and call tools, and stored queries are saved SQL queries whose creation and execution are governed by Datasette permissions.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/blog/2026/datasette-apps/">Host applications inside Datasette with Datasette ... - Datasette Blog</a></li>
<li><a href="https://github.com/datasette/datasette-agent">GitHub - datasette / datasette - agent : An LLM -powered agent for...</a></li>
<li><a href="https://docs.datasette.io/en/latest/sql_queries.html">Running SQL queries - Datasette documentation</a></li>

</ul>
</details>

**Tags**: `#Datasette`, `#LLM agents`, `#developer tools`, `#release notes`, `#permissions`

---

<a id="item-27"></a>
## [Researcher urges top AI conferences to desk-reject AI-generated papers](https://www.reddit.com/r/MachineLearning/comments/1xnkbeu/a_message_to_top_tier_conferences_d/) ⭐️ 6.0/10

A researcher posting on r/MachineLearning recounted a string of anecdotes from two recent AI conferences \(described as CORE A and A\* venues\) in which authors were unable to explain their own papers — one took five minutes before answering that knowledge graphs were represented &quot;with a vector,&quot; and another openly typed questions into ChatGPT and read the answers aloud during the session. The poster also described an author who published the same paper at two conferences simultaneously, both accepted, and left the LLM prompts in a public GitHub repository, which revealed that the data had been fabricated. The post touches on a growing worry that LLM-assisted writing, plagiarism and fabricated results are slipping past peer review at the most prestigious ML venues, which would waste reviewer effort, crowd out honest submissions, and erode trust in published machine-learning results that other researchers build on. Because conference acceptance is the main currency for hiring and promotion in ML, reviewers and program chairs are under pressure to add screening rules for AI-generated and fraudulent work. The account is purely anecdotal and comes from a single anonymous poster: no venue names, paper titles, author identities or concrete evidence are given, and the claimed scale \(&quot;dozens of stories... just this month&quot;\) cannot be verified. It also conflates several distinct problems — authors who cannot explain their own work, live use of ChatGPT during presentations, dual submission, data fabrication, and simply low-quality papers — that would each require different detection mechanisms and policy responses.

reddit · r/MachineLearning · /u/Vegetable-Formal-753 · Nov 4, 09:55

**Background**: A desk rejection is a decision by an editor or program chair to reject a submission during initial screening, before it is sent out for external peer review; journals use this routinely to filter out out-of-scope, incomplete or clearly flawed manuscripts, and conference chairs use analogous checks. In the computing field, venues are commonly graded by rankings such as the CORE Conference Ranking, where &quot;A\*&quot; denotes the top tier, so an accepted paper at such a venue carries substantial weight for a researcher&\#x27;s career. Knowledge graphs are a structured knowledge-representation technique that stores entities and their relations as a graph, and how they are encoded for a model \(for example as embeddings or graph structures\) is a basic question any author in that area should be able to answer.

<details><summary>References</summary>
<ul>
<li><a href="https://casrai.org/guides/desk-rejection">What Desk Rejection Means and Why It Happens — CASRAI</a></li>
<li><a href="https://www.core.edu.au/conference-portal">CORE Rankings Portal - core.edu.au</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_representation_and_reasoning">Knowledge representation and reasoning - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#peer-review`, `#research-integrity`, `#LLM-misuse`, `#academic-publishing`, `#machine-learning-community`

---

<a id="item-28"></a>
## [Reddit debate: is CVPR&\#x27;s 25-paper-per-author cap unfit for the AI era?](https://www.reddit.com/r/MachineLearning/comments/1xnscvr/why_cant_conferences_just_reasonably_reduce_the/) ⭐️ 6.0/10

A post on r/MachineLearning quotes the CVPR 2027 author guidelines, which carry over the CVPR 2026 rule that &quot;each author may submit at most 25 papers,&quot; with Program Chairs desk-rejecting anything beyond that limit. The poster argues this cap is tone-deaf to the current AI-assisted research climate and proposes limiting first-author submissions to 2–3 papers instead. The post touches a real structural problem: in ML, acceptance at a handful of top venues is treated as career currency, so submission volume keeps rising while the volunteer reviewer pool does not grow proportionally, which degrades review quality for everyone. If conferences do not adjust incentive structures, cheap AI-generated submissions could further strain an already overloaded peer-review system. Under the stated policy, authors who enroll more than 25 papers are not banned outright; instead the Program Chairs desk-reject only the submissions exceeding the limit, meaning a prolific author keeps 25 shots at review. The poster says they are not opposed to AI-assisted research or writing per se, only to the volume, and argues a 2–3 first-author cap would force authors to care more about idea soundness and presentation quality while cutting reviewer load; the argument is qualitative and offers no data on actual submission distributions.

reddit · r/MachineLearning · /u/mofoss · Nov 4, 16:17

**Background**: CVPR \(the IEEE/CVF Conference on Computer Vision and Pattern Recognition\) is the flagship annual conference in computer vision, and like other top ML venues it relies on volunteer reviewers drawn largely from the same pool of authors who submit to it. A &quot;desk rejection&quot; is a rejection made by the editors or program chairs without sending the paper out for peer review, typically for policy violations such as exceeding length or submission limits. In many institutions and countries, papers at a small set of recognized top-tier \(&quot;A\*&quot;\) venues are directly tied to graduation requirements, hiring, promotions, and even cash compensation, which creates strong pressure to maximize the number of submissions rather than their quality.

<details><summary>References</summary>
<ul>
<li><a href="https://cvpr.thecvf.com/">2027 Conference</a></li>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Computer_Vision_and_Pattern_Recognition">Conference on Computer Vision and Pattern Recognition - Wikipedia</a></li>
<li><a href="https://www.aischolar.com/news/article/is-desk-rejection-common">Is Desk Rejection Common?</a></li>

</ul>
</details>

**Tags**: `#academic publishing`, `#peer review`, `#ML conferences`, `#AI-generated research`, `#research incentives`

---

<a id="item-29"></a>
## [DeepSeek took 53% of OpenRouter&\#x27;s 27T daily tokens as open-weights labs pass 75%](https://www.reddit.com/r/LocalLLaMA/comments/1xnz8ct/deepseek_alone_accounted_for_53_of_all_27/) ⭐️ 6.0/10

A post on r/LocalLLaMA, citing data from the third-party tracker dirac.run, reported that DeepSeek alone accounted for 53% of all tokens processed on the OpenRouter model-routing platform in a single day, out of roughly 27 trillion tokens total. Open-weights labs collectively were said to exceed 75% of that daily token share. If accurate, the numbers suggest that developers routing requests through OpenRouter are increasingly choosing open-weights models over proprietary APIs, a meaningful signal about real-world adoption rather than benchmark performance. Such a shift would put pricing pressure on closed-model providers and strengthen the position of labs like DeepSeek in the developer ecosystem. The figures come from a single-day snapshot on an unofficial third-party tracker, and the post itself offers no methodology detail on how tokens are attributed to labs or how routing and provider fallbacks affect the counts. Token share also reflects price and promotional routing rather than model quality alone, so it should not be read as a direct measure of capability.

reddit · r/LocalLLaMA · /u/Comfortable-Rock-498 · Nov 4, 20:39

**Background**: OpenRouter is a hosted API router that gives developers a single interface to hundreds of models from many providers, handling provider selection, fallbacks and consolidated billing. Open-weights models are ones whose trained parameters are publicly released, so anyone can download, self-host or fine-tune them — DeepSeek, a Hangzhou-based lab funded by the hedge fund High-Flyer, is the best-known publisher of such models with its V3 and R1 releases. Token counts measure how much text models actually process, making them a rough proxy for usage volume on a platform like OpenRouter.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/">OpenRouter</a></li>
<li><a href="https://en.wikipedia.org/wiki/Open_weights">Open weights - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#open-weights`, `#DeepSeek`, `#LLM market share`, `#OpenRouter`, `#AI industry trends`

---

<a id="item-30"></a>
## [LFM3-Omni-2B claimed to run offline on iPhone at ~80 tok/s via WebGPU](https://www.reddit.com/r/LocalLLaMA/comments/1xntou1/lfm3omni2b_running_fully_offline_on_my_iphone_18/) ⭐️ 6.0/10

A Reddit user \(/u/xenovatech\) posted in r/LocalLLaMA claiming that Liquid AI&\#x27;s 2B-parameter LFM3-Omni model runs fully offline on an iPhone 18 Pro Max at roughly 80 tokens per second, using custom WebGPU compute kernels inside a React Native app. The submission itself contains only a title and a link, with no code, benchmarks, model quantization details, or reproducible setup published alongside it. If the claim holds up, it would show that a small omni-modal model can be served at conversational speeds entirely on a phone&\#x27;s GPU through a JavaScript/React Native stack, bypassing native Core ML or Metal bindings and any cloud dependency. That would be a meaningful data point for privacy-preserving, offline mobile assistants and for WebGPU as a portable inference backend, though the lack of published artifacts means it should currently be treated as an unverified anecdote rather than a reproducible result. The post offers no details on quantization format, prefill versus decode throughput, context length, memory footprint, thermal throttling over sustained runs, or whether the ~80 tok/s figure refers to text-only or full omni-modal \(audio/video\) input. Note also that LFM3-Omni-2B is Liquid AI&\#x27;s end-to-end omni model that accepts text, images, video and audio and can answer in speech, so achieving that speed with the audio and vision encoders active would be considerably harder than text-only decoding.

reddit · r/LocalLLaMA · /u/xenovatech · Nov 4, 17:08

**Background**: LFM3-Omni-2B is Liquid AI&\#x27;s first omni-modal model in the LFM3 family: a single end-to-end model that understands text, images, video and audio and responds in both text and speech, small enough to run offline on modest hardware. WebGPU is the browser-oriented GPU compute API that has shipped in all major engines and is increasingly used as a portable backend for local LLM inference \(for example by WebLLM/MLC\), because the same kernels can target desktop, Android and iOS GPUs. On-device LLM inference on phones is typically done with quantized 1B–7B models, with realistic single-stream decode rates in the single or low-double-digit tokens-per-second range on current hardware, which is why an ~80 tok/s claim for a 2B model stands out. React Native is a cross-platform JavaScript framework for mobile apps, so using it as the host for GPU inference kernels is an unusual but interesting choice.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/LiquidAI/LFM3-Omni-2B">LiquidAI/ LFM 3 - Omni - 2 B · Hugging Face</a></li>
<li><a href="https://pinggy.io/blog/run_llm_in_browser_webgpu/">Run an LLM Inside a Browser Tab: WebGPU and Local Inference in...</a></li>
<li><a href="https://www.runlocalai.co/stacks/iphone-on-device-ai">iPhone on - device AI stack (May 2026) — Llama... | RunLocalAI</a></li>

</ul>
</details>

**Tags**: `#on-device AI`, `#WebGPU`, `#React Native`, `#LLM inference`, `#mobile`

---

<a id="item-31"></a>
## [The Lost malloc\(\): Revisiting an Early Unix Allocator Interface](https://www.reddit.com/r/programming/comments/1xni70o/the_lost_malloc/) ⭐️ 6.0/10

A Reddit r/programming post by /u/mttd surfaced &\#x27;the lost malloc\(\)&\#x27;, a blog post that examines a historical Unix malloc implementation whose interface accepted explicit memory-region maps such as coremap, swapmap, and anymap rather than only a size argument. The write-up is useful for systems programmers because it shows why modern malloc\(size\_t\) dropped explicit memory-region parameters and how allocator APIs are shaped by assumptions about program lifetimes and memory management. Modern malloc takes a single size\_t argument and returns uninitialized storage aligned for fundamental types, while the historical interface required callers to pass memory maps; the article frames this simplification as moving more policy into the allocator implementation.

reddit · r/programming · /u/mttd · Nov 4, 07:36

**Background**: malloc is the C library function for dynamic memory allocation: it reserves a block of uninitialized memory at runtime, returns a pointer, and the caller later releases it with free\(\). Many allocator designs exist because implementations must trade off speed, metadata overhead, and fragmentation. Early Unix systems managed physical and swap memory through structures like coremap and swapmap, and some early malloc variants exposed those regions directly in the allocator API. The blog post reconstructs that lost interface and explains how later malloc implementations hid such details behind a simpler size-only call.

<details><summary>References</summary>
<ul>
<li><a href="https://napcakes.nekoweb.org/posts/malloc/">the lost malloc () - gardenweb</a></li>
<li><a href="https://en.cppreference.com/c/memory/malloc">malloc - cppreference.com</a></li>

</ul>
</details>

**Tags**: `#malloc`, `#memory allocation`, `#C`, `#systems programming`, `#reddit`

---