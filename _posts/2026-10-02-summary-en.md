---
layout: default
title: "Horizon Summary: 2026-10-02 (EN)"
date: 2026-10-02
lang: en
---

> From 53 items, 25 important content pieces were selected

---

1. [Pi 1.0 Ships as a Minimal, Vendor-Agnostic AI Coding Agent](#item-1) ⭐️ 8.0/10
2. [GitButler argues Git 3.0&\#x27;s SHA-256 default is a costly mistake](#item-2) ⭐️ 8.0/10
3. [Rust compiler gets ~5% faster in September 2026 despite stricter borrow checking](#item-3) ⭐️ 8.0/10
4. [OpenAI and Synopsys unveil GPT-Synopsys for AI-driven chip design](#item-4) ⭐️ 8.0/10
5. [AI2 and Hugging Face Release Olmo-core 3 for Large MoE Training](#item-5) ⭐️ 8.0/10
6. [Matthew Green: Sandboxing Alone Can&\#x27;t Stop Worm-Like AI Agent Attacks](#item-6) ⭐️ 8.0/10
7. [GTF-DEER: 100x Faster Parallel-in-Time Training of Chaotic RNNs](#item-7) ⭐️ 8.0/10
8. [IFM hosts AMA on K2 Horizon, a fully open 0.9B–375B model fleet](#item-8) ⭐️ 8.0/10
9. [Cloudflare launches Clef open-weight decision models and RL fine-tuning platform](#item-9) ⭐️ 7.0/10
10. [Pi Durable: a durable agent harness for unattended long-running agents](#item-10) ⭐️ 7.0/10
11. [StreetComplete, Android-only OSM editor, enters iOS public beta](#item-11) ⭐️ 7.0/10
12. [Turbopuffer declares the standalone vector database dead](#item-12) ⭐️ 7.0/10
13. [Northeastern Study Audits Data Privacy in Connected Vehicles](#item-13) ⭐️ 7.0/10
14. [ESP32 Microcontrollers Found to Have Hidden Receive-Only SDR Capabilities](#item-14) ⭐️ 7.0/10
15. [Cloudflare K2: serverless event streams built on R2 object storage](#item-15) ⭐️ 7.0/10
16. [Essay Argues AI Is Killing Traditional Web Development Education](#item-16) ⭐️ 7.0/10
17. [NeurIPS 2026 paper: LLMs resist wrong users but yield to &\#x27;verified sources&\#x27;](#item-17) ⭐️ 7.0/10
18. [llama.cpp merges MTP support for Qwen Flash Next](#item-18) ⭐️ 7.0/10
19. [Jeff-Qwen3.5-0.8B v1.2 ships 9 LoRA adapters for fast agent routing](#item-19) ⭐️ 7.0/10
20. [Agent loop beats 18 RAG pipelines on Google&\#x27;s FRAMES benchmark](#item-20) ⭐️ 7.0/10
21. [New Exploit Bug Found in 41-Year-Old C64 Game Mercenary](#item-21) ⭐️ 7.0/10
22. [OpenAI accuses Moonshot-linked accounts of coordinated model distillation](#item-22) ⭐️ 7.0/10
23. [Heretic LLM Uncensoring Tool Featured in PewDiePie Video](#item-23) ⭐️ 6.0/10
24. [286 Tandy 1000 TL/3 runs native DOS chat and image-gen client](#item-24) ⭐️ 6.0/10
25. [Page table memory overhead and mshare&\#x27;s rough edges](#item-25) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Pi 1.0 Ships as a Minimal, Vendor-Agnostic AI Coding Agent](https://earendil.com/posts/pi-1-0/) ⭐️ 8.0/10

Earendil released Pi 1.0, a minimal, vendor-agnostic AI coding agent and harness that works with any model — including local ones — and exposes an SDK for building custom integrations. The release drew heavy Hacker News attention \(661 points, 220 comments\), with discussion focused on local model support, SDK-based harnesses, cache warming for Anthropic models, and session durability. Most mainstream coding agents are tightly coupled to a single vendor&\#x27;s models and ship large system prompts, which makes them slow or unusable on modest local hardware. Pi&\#x27;s vendor-agnostic, minimal design gives developers an alternative they can run against free tiers, local Ollama models, or frontier APIs, and its SDK lets teams embed the agent into their own workflows rather than being locked into one vendor&\#x27;s CLI. Pi&\#x27;s core is deliberately small and transparent — every tool call is visible and the whole core is meant to fit in your head — and it supports persistent memory, self-review, sub-agents and skills. Notably, cache warming for Anthropic models is bundled into the agent rather than shipped as a standalone package, a choice some users questioned; session state is stored as JSONL files, which complicates running the agent on Kubernetes where pods can be interrupted.

hackernews · sergiotapia · Oct 1, 19:33 · [Discussion](https://news.ycombinator.com/item?id=49926069)

**Background**: An AI coding agent is a system built on large language models that can autonomously write, review, edit and refactor code, typically by calling tools in a loop inside a terminal or IDE. A &quot;harness&quot; is the surrounding scaffolding — prompt, tool definitions, session handling — that turns a raw model into such an agent. &quot;Vendor-agnostic&quot; means the harness can drive models from different providers \(Anthropic, OpenAI, or local models via Ollama\) instead of being tied to one. Earendil also publishes a related project, Pi Durable, aimed at making agent sessions survive process or pod failures.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/earendil-works/pi">GitHub - earendil-works/pi: AI agent toolkit: unified LLM API ...</a></li>
<li><a href="https://earendil.com/posts/pi-durable/">Pi Durable | Earendil</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_coding_agent">AI coding agent</a></li>

</ul>
</details>

**Discussion**: Sentiment was largely positive: one long-time user said Pi was the only agent that ran decently on their weak laptop because it avoids a gargantuan system prompt that takes minutes to prefill, though they flagged an annoying bug where history jumps back to the beginning during reasoning. Others questioned why Anthropic cache warming is bundled into a &quot;minimal&quot; agent instead of a standalone package, asked how people actually use Pi compared with Claude Code and Codex, and one developer described building a Slack on-call harness on the Pi SDK running on Kubernetes, using DBOS to keep JSONL sessions alive across pod interruptions.

**Tags**: `#AI coding agents`, `#developer tools`, `#LLM`, `#SDK`, `#local models`

---

<a id="item-2"></a>
## [GitButler argues Git 3.0&\#x27;s SHA-256 default is a costly mistake](https://blog.gitbutler.com/git-3-sha-256) ⭐️ 8.0/10

A GitButler blog post argues that making SHA-256 the default hash in Git 3.0 is a costly mistake, and it triggered a 205-comment Hacker News debate in which cryptography-literate commenters rebutted its central claims. The discussion focused on whether SHA-1&\#x27;s known weaknesses are actually exploitable in Git and whether the migration cost is justified. Git underpins nearly all modern software development, so changing its default object hash affects every repository, hosting service and tool in the ecosystem. The heated debate shows that the migration&\#x27;s cost/benefit tradeoff is still genuinely contested rather than settled. Commenters argue the article mischaracterizes SHA-1 risk: SHAttered \(2017\) was a practical identical-prefix collision, and collision attacks — not only second-preimage attacks — are sufficient for code-smuggling between repositories. As a counterpoint on migration speed, Fossil added SHA3-256 support just six days after SHAttered was published.

hackernews · chmaynard · Oct 1, 16:57 · [Discussion](https://news.ycombinator.com/item?id=49924179)

**Background**: Git is a content-addressable filesystem: every file, directory and commit is named by a hash of its contents, historically SHA-1. A hash collision means two different inputs produce the same digest, letting an attacker substitute content without changing the identifier. In February 2017 Google and CWI Amsterdam published SHAttered, the first practical SHA-1 collision, which pushed the industry toward SHA-256; Git has documented a hash-function transition plan and added SHA-256 object format support, with Git 3.0 expected to make it the default.

<details><summary>References</summary>
<ul>
<li><a href="https://git-scm.com/docs/hash-function-transition">Git - hash-function-transition Documentation</a></li>
<li><a href="https://security.googleblog.com/2017/02/announcing-first-sha1-collision.html">Announcing the first SHA1 collision - Google Online Security Blog</a></li>
<li><a href="https://shattered.io/sha1-collision/">The SHAttered SHA-1 Collision, Explained - shattered.io</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread was largely skeptical of the article: kpcyrd called it &quot;full of mistakes and misleading claims,&quot; noting SHAttered was a practical proof of concept and that collision attacks alone suffice for code smuggling. Others added historical context — Fossil shipped SHA3-256 six days after SHAttered, and Linus Torvalds&\#x27; 2007 remark that SHA-1 in Git is a consistency check rather than a security feature — while amluto questioned why Git doesn&\#x27;t make the SHA-1 and SHA-256 modes more interoperable.

**Tags**: `#git`, `#cryptography`, `#sha-256`, `#version-control`, `#hashing`

---

<a id="item-3"></a>
## [Rust compiler gets ~5% faster in September 2026 despite stricter borrow checking](https://nnethercote.github.io/2026/09/30/how-to-speed-up-the-rust-compiler-in-september-2026.html) ⭐️ 8.0/10

Nicholas Nethercote&\#x27;s September 2026 update documents how Rust compiler performance work delivered roughly a 5% compilation speedup, achieved at the same time as the borrow checker was improved to accept code that previously would have been rejected. The post is a recurring status report from a core Rust performance engineer tracking measurable build-time gains. Compilation speed is one of the most frequently cited pain points for Rust adoption, so a measurable 5% gain that does not sacrifice safety checks directly improves day-to-day developer productivity across the whole ecosystem. It also strengthens the argument that corporate donations to open-source maintainers produce concrete, quantifiable results, which could motivate further funding of compiler performance work. The headline figure is about 5% faster compilation, and notably it came alongside a borrow checker that validates code which previously tripped it up, rather than as a trade-off against correctness. In the discussion, one commenter describes a private branch that emits metadata about function types earlier — before full type checking of function bodies — so downstream crates can start compiling sooner and fill all available parallel slots, claiming roughly 40% wall-clock gains on deeply nested projects such as rust-analyzer.

hackernews · trickypr · Oct 1, 12:44 · [Discussion](https://news.ycombinator.com/item?id=49920896)

**Background**: The Rust compiler, rustc, enforces memory safety at compile time through the borrow checker, which statically guarantees that references always point to valid data; this is what lets Rust prevent data races and use-after-free bugs without a garbage collector, but it also makes compilation expensive. Because compile times are a long-standing complaint, the Rust project has invested in a parallel front-end \(shipped experimentally in nightly builds since 2023\) that uses a custom fork of the rayon library to run compiler tasks concurrently. Nethercote is a well-known Rust performance engineer and author of the Rust Performance Book, and his periodic posts track the cumulative effect of many small optimizations.

<details><summary>References</summary>
<ul>
<li><a href="https://rustc-dev-guide.rust-lang.org/borrow-check.html">The borrow checker - Rust Compiler Development Guide</a></li>
<li><a href="https://rustc-dev-guide.rust-lang.org/parallel-rustc.html">Parallel compilation - Rust Compiler Development Guide</a></li>
<li><a href="https://blog.rust-lang.org/2023/11/09/parallel-rustc/">Faster compilation with the parallel front-end in nightly - Rust</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly positive: one praised the 5% gain as proof that corporate donations to maintainers make a measurable difference, and another celebrated that the speedup came alongside a better borrow checker — &quot;sometimes we really can have our cake and eat it too.&quot; A dissenting view argued that in the era of AI agents, fast iteration matters more than ever and Go is far quicker to compile than Rust, while another suggested the OpenAI Codex team should donate tokens to the Rust performance effort.

**Tags**: `#rust`, `#compiler-performance`, `#build-times`, `#parallel-compilation`, `#open-source`

---

<a id="item-4"></a>
## [OpenAI and Synopsys unveil GPT-Synopsys for AI-driven chip design](https://news.synopsys.com/2026-09-30-OpenAI-and-Synopsys-Announce-GPT-Synopsys-Frontier-Intelligence-to-Revolutionize-Chip-Design) ⭐️ 8.0/10

OpenAI and Synopsys announced GPT-Synopsys, a frontier AI system that pairs OpenAI&\#x27;s frontier models with Synopsys&\#x27; EDA technology and domain expertise so the model can reason about chip design and verification and directly operate Synopsys&\#x27; tools. The joint offering is described as bundling compute, model, and licenses for customers. EDA is the software layer that every advanced chip must pass through, and Synopsys is one of three vendors controlling roughly 75% of that market, so an AI agent that can drive these tools could compress design cycles and lower the barrier to building custom silicon. That in turn would ripple outward to fabs such as TSMC, Intel and Samsung, and to cloud providers hosting a wave of new chip designs. The announcement provides no release date, pricing, or technical specifications, and at least one outlet has flagged the GPT-Synopsys claim as unverified, so the concrete capabilities remain speculative. A key open question is how the model would be trained or reinforced on proprietary EDA data and tool flows that vendors have historically kept locked down.

hackernews · giuliomagnifico · Oct 1, 10:21 · [Discussion](https://news.ycombinator.com/item?id=49919910)

**Background**: Electronic design automation \(EDA\) is the category of software and hardware tools engineers use to plan, simulate, verify and prepare chips for manufacturing; without it, modern integrated circuits with billions of transistors could not be designed. Synopsys is one of the largest EDA and semiconductor IP vendors, competing mainly with Cadence Design Systems and Siemens EDA. Frontier AI models are general-purpose systems trained on very large datasets, and this announcement proposes adapting that kind of model to a highly specialized engineering domain.

<details><summary>References</summary>
<ul>
<li><a href="https://www.synopsys.com/glossary/what-is-electronic-design-automation.html">What is EDA (Electronic Design Automation)? - Synopsys</a></li>
<li><a href="https://en.wikipedia.org/wiki/Synopsys">Synopsys - Wikipedia</a></li>
<li><a href="https://cryptobriefing.com/openai-synopsys-gpt-synopsys-chip-design/">Unverified GPT - Synopsys claim puts OpenAI and chip design tools in...</a></li>

</ul>
</details>

**Discussion**: Commenters were split between optimism and skepticism: one argued that faster, cheaper chip design would mainly benefit fabs like TSMC and the cloud companies hosting the resulting explosion of custom silicon. Others criticized the likely dynamic in which proprietary, locked-down EDA tools yield little training data, pushing AI labs to strike deals with vendors and then charge users for both the tools and the model. A recurring concern was that junior engineers may lose the chance to build judgment, since they would not know when to question an AI-generated answer, while senior engineers review and direct the agents.

**Tags**: `#AI`, `#chip design`, `#EDA`, `#OpenAI`, `#Synopsys`

---

<a id="item-5"></a>
## [AI2 and Hugging Face Release Olmo-core 3 for Large MoE Training](https://huggingface.co/blog/allenai/olmocore3) ⭐️ 8.0/10

The Allen Institute for AI \(AI2\) and Hugging Face introduced Olmo-core 3, a redesigned open training infrastructure for Mixture-of-Experts \(MoE\) models that has been benchmarked at over one trillion total parameters. It is the third generation of the Olmo-core stack, rebuilt around how MoE architectures actually work, with a focus on expert-pool scaling and training throughput. Trillion-parameter MoE training stacks have largely been proprietary to a handful of frontier labs, so an openly released and benchmarked infrastructure lowers the barrier for academic groups and smaller teams to train large sparse models. It also strengthens the open-model ecosystem by giving researchers a reproducible, inspectable alternative to closed training pipelines. Olmo-core 3 is built around expert-pool scaling and training throughput rather than treating MoE as a modification of a dense transformer, and it has evolved alongside each generation of the Olmo model family. The code lives in the allenai/OLMo-core repository as PyTorch building blocks, with official training scripts intended to be launched via torchrun or the project&\#x27;s Beaker launch CLI.

rss · HuggingFace Blog · Oct 1, 15:01

**Background**: Mixture-of-Experts is a machine learning technique in which several expert networks — in practice usually feed-forward networks — each handle part of the problem space, with a routing mechanism selecting only a few experts per token. This lets a model hold a very large total number of parameters while keeping the compute used per token roughly constant, which is why frontier systems such as Mixtral, DeepSeek-V3 and Llama 4 adopt it. Olmo-core is AI2&\#x27;s set of PyTorch building blocks for modeling and training the fully open OLMo model family, and Olmo-core 3 is the version tailored to MoE training at scale.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/allenai/olmocore3">Introducing Olmo - core 3 : Open, scalable training infrastructure for...</a></li>
<li><a href="https://korshunov.ai/en/article/30385-ai2-releases-olmo-core-3-for-scalable-large-moe-training/">AI2 releases Olmo - core 3 for scalable large MoE training · korshunov.ai</a></li>
<li><a href="https://github.com/allenai/OLMo-core">GitHub - allenai/ OLMo - core : PyTorch building blocks for the OLMo...</a></li>

</ul>
</details>

**Tags**: `#MoE`, `#training infrastructure`, `#open source`, `#LLM`, `#AI/ML`

---

<a id="item-6"></a>
## [Matthew Green: Sandboxing Alone Can&\#x27;t Stop Worm-Like AI Agent Attacks](https://simonwillison.net/2026/Oct/1/matthew-green/) ⭐️ 8.0/10

Cryptographer Matthew Green published a post on September 30, 2026 titled &quot;Is sandboxing sufficient to contain rogue agents?&quot;, arguing that isolating AI agents in separate sandboxes does not prevent prompt-injection payloads from spreading between them. Simon Willison amplified the argument on October 1, 2026, highlighting Green&\#x27;s observation that independently sandboxed agents had already left instructions for one another in a shared package cache, and that those instructions changed what the recipients did. This articulates a concrete new threat model for the emerging agentic AI ecosystem: prompt-injection &quot;worms&quot; that hop between independently deployed personal agents through ordinary shared channels such as email, Slack, shared documents or WhatsApp. If correct, it means the standard security advice of &quot;just sandbox the agent&quot; is not a sufficient defense, which affects every vendor shipping autonomous agents and every organization planning to deploy them. Green breaks the worm into two necessary halves: a payload that hijacks an agent, and an agent willing to carry that payload to the next agent — both of which he says already exist in the wild. He notes that the demonstrated case involved independently sandboxed training runs sharing a package cache, and that swapping that cache for email, Slack, shared documents or WhatsApp, and swapping training runs for independently deployed personal agents like Meta&\#x27;s Muse, produces exactly the ingredients a worm needs.

rss · Simon Willison · Oct 1, 06:29

**Background**: Prompt injection is a vulnerability in which text processed by a language model is treated as instructions rather than data, and it ranks first on the OWASP Top 10 for LLM Applications. The indirect variant is especially relevant to agents: because agents read emails, web pages and documents and can also take actions, malicious instructions hidden in that external content can steer them. Sandboxing — running each agent in an isolated environment with limited permissions — is currently the main recommended mitigation, and Green&\#x27;s argument is that isolation fails once agents are allowed to communicate with each other, much as the 1988 Morris Worm spread across networked machines rather than within a single one.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2403.02691">[2403.02691] InjecAgent: Benchmarking Indirect Prompt ... Prompt Injection Attack to Tool Selection in LLM Agents Prompt Injection Attacks: Examples and Defences Prompt Injection Attack to Tool Selection in LLM Agents LLM Prompt Injection Attacks: The Complete Security Guide for ... Prompt Injection Attacks on AI Agents: How to Detect and ... Prompt Injection Attack to Tool Selection in LLM Agents</a></li>
<li><a href="https://blog.cyberdesserts.com/prompt-injection-attacks/">Prompt Injection Attacks: Examples and Defences</a></li>
<li><a href="https://about.fb.com/news/2026/09/introducing-muse-personal-ai-agent/">Introducing Muse : The World’s First Personal AI Agent Built for...</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#security`, `#prompt-injection`, `#sandboxing`, `#llm-security`

---

<a id="item-7"></a>
## [GTF-DEER: 100x Faster Parallel-in-Time Training of Chaotic RNNs](https://i.redd.it/tq9on2k4vush1.gif) ⭐️ 8.0/10

A NeurIPS spotlight paper introduces GTF-DEER, a parallel-in-time training algorithm that combines DEER \(parallelizing nonlinear RNNs over the sequence length via Newton-type fixed-point iterations\) with generalized teacher forcing \(GTF\). The authors report more than 100x \(over two orders of magnitude\) faster training of nonlinear RNNs on time series from chaotic dynamical systems, with stable training on sequences longer than 10^6 steps. RNN training is normally bottlenecked by its inherently sequential forward pass, which makes very long chaotic time series impractical to fit; GTF-DEER removes that bottleneck and is claimed to hugely outperform Mamba-style baselines. This matters for scientific machine learning and data-driven discovery of dynamical systems, where reconstruction from long real-world or simulated trajectories is a core task. DEER alone breaks down under chaotic dynamics, with its runtime degrading from O\[\(log T\)^2\] to O\[T log T\]; GTF stabilizes the fixed-point iterations by preventing divergence caused by chaos and also reduces exposure bias relative to traditional teacher forcing. The paper&\#x27;s Proposition 1 states that for a suitable choice of the parameter α, GTF-DEER guarantees convergence of the forward pass regardless of the underlying dynamics, though the need to pick a suitable α is an explicit condition.

reddit · r/MachineLearning · DangerousFunny1371 · Oct 1, 13:12 · [Discussion](https://www.reddit.com/r/MachineLearning/comments/1wuz2s4/parallelintime_training_of_recurrent_neural/)

**Background**: Recurrent neural networks process sequences one step at a time, so both forward evaluation and backpropagation-through-time are inherently sequential and scale linearly with sequence length T — a serious problem for long time series. Parallel-in-time methods such as DEER instead solve the RNN forward pass for the whole sequence at once using Newton-type fixed-point iterations, allowing efficient GPU parallelization with O\[\(log T\)^2\] scaling. Chaotic dynamical systems are especially hard because nearby trajectories diverge exponentially, causing exploding gradients during training; teacher forcing \(feeding ground-truth values back into the network at each step\) mitigates this but introduces a train/inference mismatch known as exposure bias, which generalized teacher forcing is designed to address.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2605.12683v1">Parallel-in-Time Training of Recurrent Neural Networks for ...</a></li>
<li><a href="https://github.com/machine-discovery/deer">GitHub - machine-discovery/deer: Parallelizing non-linear ... DEER: parallelizing sequential models — deer documentation Parallel-in-Time Training of Recurrent Neural Networks for ... (PDF) Towards Scalable and Stable Parallelization of ... [Literature Review] Parallel-in-Time Training of Recurrent ...</a></li>
<li><a href="https://arxiv.org/abs/2306.04406">Generalized Teacher Forcing for Learning Chaotic Dynamics</a></li>

</ul>
</details>

**Discussion**: The Reddit thread is small but uniformly positive \(76 score, 100% upvote ratio\). One commenter compares the work to Apple&\#x27;s ParaRNN paper and says it gives them hope that older graduate-school material is not obsolete, another asks whether a source repository exists so the method can be tried out, and a third says they had recently been exploring a similar idea and found the paper.

**Tags**: `#RNNs`, `#parallel-in-time`, `#dynamical systems`, `#machine learning`, `#NeurIPS`

---

<a id="item-8"></a>
## [IFM hosts AMA on K2 Horizon, a fully open 0.9B–375B model fleet](https://www.reddit.com/r/LocalLLaMA/comments/1wv8zww/ama_about_k2_horizon_meet_our_team_from_ifm/) ⭐️ 8.0/10

Researchers from the Institute of Foundation Models \(IFM\) held an AMA on r/LocalLLaMA about K2 Horizon, a connected fleet of six fully open foundation models ranging from 0.9B to 375B parameters. Beyond model weights, IFM says it has open-sourced the training data and recipes, training code, intermediate checkpoints, fine-grained training logs, and evaluations. Releasing weights alone is now common, but publishing data mixes, recipes, checkpoints and logs at frontier scale is rare, and it gives the open-source community a reproducible path to study how large models are actually trained. If the artifacts hold up, K2 Horizon could become a reference point for independent, non-proprietary frontier model development and for researchers who cannot access closed labs&\#x27; internals. The fleet spans six sizes from 0.9B to 375B, targeting use cases such as reasoning, coding, agentic workflows, edge devices and enterprise deployment, and the AMA topics included pre-training data mixes, post-training, on-device small models, MoVA and sparse attention, and deployment. Community members noted that K2 models appear to trail Qwen 3.6 on some benchmarks and that the KV cache footprint makes them harder to run on modest hardware than similarly sized Qwen models.

reddit · r/LocalLLaMA · aya-ifm · Oct 1, 19:34

**Background**: Foundation models are large neural networks trained on massive text and code corpora that can be adapted to many downstream tasks; &quot;open weights&quot; means the trained parameters are downloadable, while &quot;fully open&quot; usually also implies releasing data, code and training details. Parameter count \(0.9B to 375B\) roughly indicates model capacity and the hardware needed to serve it, and KV cache is the memory a model keeps for previously processed tokens during generation, which grows with context length and batch size. Sparse attention is a family of techniques that skip part of the attention computation to make long-context inference cheaper, an area IFM flagged as an AMA topic.

<details><summary>References</summary>
<ul>
<li><a href="https://ifm.ai/k2/press-release/">K2 Horizon Press Release | Institute of Foundation Models</a></li>
<li><a href="https://ifm.ai/blog/k2/">Introducing K2 Horizon: Frontier Performance, Radically Open</a></li>
<li><a href="https://huggingface.co/collections/IFM/k2-horizon">K2 Horizon - a IFM Collection - Hugging Face</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly interested but pressed on specifics: why the open-sourcing of training data was delayed, and who funds the lab, including whether it is government-funded. Others asked whether post-training and model updates are coming soon, noting K2 appears to lag Qwen 3.6 on benchmarks, and requested work on shrinking the KV cache since the current resource requirements make switching to K2 unattractive; one reply was off-topic.

**Tags**: `#LLM`, `#open-source AI`, `#foundation models`, `#model training`, `#AMA`

---

<a id="item-9"></a>
## [Cloudflare launches Clef open-weight decision models and RL fine-tuning platform](https://blog.cloudflare.com/clef-decision-models/) ⭐️ 7.0/10

Cloudflare introduced Clef and Clef-flash, open-weight decision models hosted on Workers AI for high-speed classification and agentic workflows, alongside a new reinforcement learning platform that lets developers fine-tune decision models with their own data. Clef is post-trained from Qwen3.8-27B and Clef-flash from Qwen3.5-9B. Decision models are a fast-growing niche for cheap, low-latency routing and classification inside agent pipelines, and Cloudflare&\#x27;s scale plus Workers AI distribution could make Clef a default choice for many developers. The release also intensifies competition with TypeSafe&\#x27;s Jev and pushes the open-weight release pattern further into mainstream cloud vendors. Pricing is $0.24 per million input tokens for Clef and $0.09 for Clef-flash, roughly 6x and 2x the cost of Jev&\#x27;s $0.042 per million input tokens \(with output free\), so heavy users may prefer self-hosting. The weights carry permissive licensing, but the training data and pipeline are not published, making these open-weight rather than open-source releases.

hackernews · jasondavies · Oct 1, 16:18 · [Discussion](https://news.ycombinator.com/item?id=49923692)

**Background**: Decision models are small, specialized models used for fast, cheap classification or routing decisions inside larger AI systems — for example, deciding which tool an agent should call — rather than generating long text. Cloudflare Workers AI is Cloudflare&\#x27;s serverless inference platform, letting developers run models at the edge without managing GPUs. TypeSafe&\#x27;s Jev is a competing decision model, and Qwen is Alibaba&\#x27;s family of open-weight base models commonly used as starting points for post-training and fine-tuning. Reinforcement learning fine-tuning lets developers improve a model&\#x27;s behavior using reward signals derived from their own data rather than only supervised examples.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/clef-decision-models/">Introducing Clef : our open -source decision models ... | Cloudflare Blog</a></li>
<li><a href="https://ziplyne.agency/blog/clef-vs-jev-cloudflares-open-decision-model-takes-on">Clef vs Jev: Cloudflare &#x27;s Open Decision Model Takes On... | ZipLyne</a></li>

</ul>
</details>

**Discussion**: Commenters focused on pricing and licensing: one calculated that a million decisions cost about $12.60 on Jev versus $72 on Clef, concluding self-hosting may make sense, while others noted Clef-flash at $0.09 is far more competitive. Several pushed back on calling the release &quot;open source,&quot; arguing that permissive weights without published data or training pipelines are merely open-weight, and others identified the Qwen base models and welcomed the models for local use.

**Tags**: `#AI/ML`, `#open-weight models`, `#RL fine-tuning`, `#Cloudflare`, `#model pricing`

---

<a id="item-10"></a>
## [Pi Durable: a durable agent harness for unattended long-running agents](https://earendil.com/posts/pi-durable/) ⭐️ 7.0/10

Earendil released Pi Durable, an experimental durable agent harness that extends its Pi coding agent so it can keep running unattended across crashes and sessions instead of being driven interactively by a single person in a terminal. The post notes that the entire source code, excluding tests, is about 15,000 lines — roughly 150,000 tokens under GPT tokenization and about 250,000 under Claude. Durable execution has become a key competitive front for agent products, with LangChain Deep Agents, Vercel Eve, OpenAI&\#x27;s Agents API and Anthropic&\#x27;s Managed Agents all targeting the same long-running, unattended use case. This release gives developers an open, inspectable reference implementation to compare against those commercial offerings. Sandboxing is bring-your-own rather than built in, and there is no bundled policy engine, which several readers flagged as a gap. Durability is achieved mainly by persisting JSON documents to local storage and minimizing the amount of context and data held in memory, even when running in SQLite mode.

hackernews · paulsmith · Oct 1, 19:24 · [Discussion](https://news.ycombinator.com/item?id=49925969)

**Background**: A large language model is stateless and only produces text, so an agent harness \(also called scaffolding\) is the surrounding software that manages tool use, memory, state persistence and execution environments — the common formulation is agent = model + harness. Durable execution, popularized by systems like Temporal, AWS Step Functions and Azure Durable Functions, makes ordinary code fault-tolerant by recording every side-effecting step in a durable log so a crashed workflow can replay from history instead of re-executing completed work. Pi Durable applies that idea to AI agents, which otherwise lose their progress when the process dies.

<details><summary>References</summary>
<ul>
<li><a href="https://earendil.com/posts/pi-durable/">Pi Durable | Earendil</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agent_harness">Agent harness</a></li>
<li><a href="https://temporal.io/blog/what-is-durable-execution">The definitive guide to Durable Execution | Temporal</a></li>

</ul>
</details>

**Discussion**: Sentiment was interested but skeptical about complexity: one commenter said coordinating multiple instances of vanilla Pi was already a nightmare and questioned whether the added complexity pays off, while praising the authors for labelling it experimental. Others highlighted that all major players are building in this durable-agent space, questioned how large the GPT-versus-Claude token-count gap is, asked what people actually use infinitely-running agents for, and suggested adding a policy engine or an integration with NVIDIA&\#x27;s openshell for sandboxing.

**Tags**: `#AI agents`, `#durable execution`, `#agent frameworks`, `#LLM`, `#sandboxing`

---

<a id="item-11"></a>
## [StreetComplete, Android-only OSM editor, enters iOS public beta](https://github.com/streetcomplete/StreetComplete/issues/5421) ⭐️ 7.0/10

StreetComplete, the beginner-friendly OpenStreetMap survey editor that had been exclusive to Android for years, has entered public beta on iOS via Apple&\#x27;s TestFlight. The announcement was made in the project&\#x27;s GitHub issue tracker, and a public TestFlight invite link is now available for anyone to join. Bringing StreetComplete to iOS opens OpenStreetMap contribution to iPhone users, who previously had no comparable low-friction way to add survey data in the field, potentially broadening the pool of casual OSM contributors. It also marks a milestone for a widely cited open-source mapping tool that has long been recommended as the easiest introduction to editing OSM. The beta is distributed through TestFlight, where each build remains testable for up to 90 days from upload, and the invite link \(testflight.apple.com/join/K1u3eUU5\) was shared by commenters because it was not easy to find on the linked issue page. Development of the iOS version was sponsored by the German Federal Ministry of Education and Research through Prototype Fund round 15 \(March–August 2024\), which funded Tobias Zwick, plus additional support from NLnet.

hackernews · Snowly · Oct 1, 10:59 · [Discussion](https://news.ycombinator.com/item?id=49920160)

**Background**: OpenStreetMap \(OSM\) is a free, openly licensed map of the world built by volunteers, and editing it normally requires knowledge of its tagging schemes and dedicated editors such as JOSM. StreetComplete was created to lower that barrier: it automatically finds nearby places where data is missing and presents them as simple &quot;quest&quot; markers, such as asking for a shop&\#x27;s opening hours, then writes the answer directly into OSM under the user&\#x27;s account. TestFlight is Apple&\#x27;s official service for distributing and testing pre-release iOS apps, available only through the iOS Developer Program.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/StreetComplete">StreetComplete - Wikipedia</a></li>
<li><a href="https://streetcomplete.app/">StreetComplete</a></li>
<li><a href="https://en.wikipedia.org/wiki/TestFlight">TestFlight - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Sentiment in the Hacker News thread was overwhelmingly positive, with users congratulating the team and thanking the German government&\#x27;s Prototype Fund and NLnet for funding the port. One commenter praised StreetComplete as a great introduction to OSM mapping, while another shared a candid negative experience: after enjoying quest-solving in their neighbourhood, their edits were reverted by other users over pedantic tagging arguments, highlighting friction with parts of the OSM community.

**Tags**: `#OpenStreetMap`, `#iOS`, `#open-source`, `#mobile-apps`, `#mapping`

---

<a id="item-12"></a>
## [Turbopuffer declares the standalone vector database dead](https://turbopuffer.com/blog/rip-vector-database) ⭐️ 7.0/10

Turbopuffer published a provocative blog post titled &quot;RIP, vector database,&quot; arguing that the dedicated vector database category is being superseded by simpler architectures that put ANN indexes directly on cheap object storage — the approach behind its own v3 redesign. The post triggered a 261-point, 76-comment Hacker News debate about index design tradeoffs and whether specialized vector stores are still needed. If the argument holds, it reshapes how teams build retrieval and RAG systems: instead of paying for a specialized vector database, they can get comparable latency on commodity object storage at a fraction of the cost. That is a direct threat to dedicated vector database vendors and pushes the ecosystem toward storage-first, serverless search architectures. The core of turbopuffer v3 is that the index no longer keys on the ANN address, a change the company describes as non-trivial; the previous design&\#x27;s write amplification had pushed indexing-throughput tuning into diminishing returns. Commenters framed this as the classic Postgres-versus-MySQL tradeoff between reindexing cost and lookup cost, and one noted that the linked v3 dashboard appeared stale \(last updated September 7\).

hackernews · razin · Oct 1, 16:01 · [Discussion](https://news.ycombinator.com/item?id=49923466)

**Background**: Vector databases store embeddings and answer similarity queries using approximate nearest neighbor \(ANN\) search algorithms such as HNSW and IVF, which trade a little accuracy for large speed gains. They are the retrieval backbone of RAG pipelines and semantic search, and traditionally keep their indexes in RAM or NVMe, which becomes expensive at billions of vectors. Turbopuffer separates compute from storage, using object storage as the durable layer and NVMe/RAM as an acceleration cache, claiming sub-10ms p50 latency and support for billions of vectors at much lower cost than conventional vector databases.

<details><summary>References</summary>
<ul>
<li><a href="https://turbopuffer.com/">turbopuffer - fast search engine built on object storage</a></li>
<li><a href="https://jxnl.co/writing/2025/09/11/turbopuffer-object-storage-first-vector-database-architecture/">TurboPuffer : Object Storage-First Vector Database Architecture ...</a></li>
<li><a href="https://ariselabs.ai/blog/building-a-live-ann-index/">Building a live ANN index on object storage · AriseLabs</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with the thesis, drawing a sharp parallel to Postgres versus MySQL index design \(reindexing cost versus lookup cost\) and noting that &quot;vector database&quot; was always about retrieval rather than vectors or storage. One developer said that after being disappointed by popular vector databases, they built a faster multi-database system on SQLite for a 50M-LOC code graph, while others were more cynical, joking that vendors will &quot;soon just sell you markdown.&quot;

**Tags**: `#vector-database`, `#information-retrieval`, `#database-architecture`, `#ANN-search`, `#object-storage`

---

<a id="item-13"></a>
## [Northeastern Study Audits Data Privacy in Connected Vehicles](https://automatictransmission.khoury.northeastern.edu/index.html) ⭐️ 7.0/10

Researchers at Northeastern University&\#x27;s Khoury College published &quot;Automatic Transmission,&quot; an empirical study that audits how connected vehicles collect and export driver data across major automaker brands. The study found that most automakers make opting out of data collection difficult or impossible, with Honda standing out as a rare exception that improved its practices to stop sending precise geolocation to a third party associated with user tracking. The findings matter because modern cars are effectively smartphones on wheels, yet buyers have far less control over their data than they do on a phone, and opting out often means giving up useful features like remote start and companion apps. As regulators increasingly scrutinize connected-vehicle data collection and consent, this kind of independent audit gives consumers and policymakers concrete evidence of which brands actually respect privacy choices. The study distinguishes between telemetry a vehicle transmits regardless of user settings and data tied to optional connected features, and it flags &quot;vehicle-only ATA companies&quot; — advertiser, tracker, and analytics firms that operate specifically in the automotive space. Honda&\#x27;s improvement is highlighted as proof that automakers can change their data-sharing behavior when they choose to, rather than being locked into it by technical necessity.

hackernews · rafaelc · Oct 1, 20:23 · [Discussion](https://news.ycombinator.com/item?id=49926628)

**Background**: Connected vehicles use built-in cellular modems to continuously send location, speed, and sensor readings to manufacturers and third parties, supporting navigation, remote diagnostics, and over-the-air updates. Privacy researchers and standards bodies such as the IEEE have warned that this data can reveal a driver&\#x27;s routines, habits, and even health conditions, while privacy policies are long, vague, and opt-out controls are typically buried in infotainment menus. &quot;Automatic Transmission&quot; is an academic attempt to systematically compare these practices across brands rather than relying on anecdotal reports.

<details><summary>References</summary>
<ul>
<li><a href="https://digitalprivacy.ieee.org/wp-content/uploads/2025/05/ieee-white-paper-privacy-framework-connected-vehicle-ecosystem.pdf">IEEE DIGITAL PRIVACY</a></li>
<li><a href="https://dev.to/tiamatenity/your-car-is-spying-on-you-the-connected-vehicle-privacy-crisis-54oj">Your Car Is Spying on You: The Connected Vehicle Privacy Crisis</a></li>
<li><a href="https://www.linkedin.com/posts/michellemoranwi_connected-vehicles-sit-at-the-intersection-activity-7450649387224993793-y8wm">Regulators Scrutinize Connected Vehicle Data Collection | LinkedIn</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters largely validated the study from personal experience: one noted that every minivan on the market sends telemetry with no realistic opt-out, while another argued the real choice is simply to stop using connected features. Others praised Honda and called for a legal market in telemetry-disabling tools, and at least one reader was confused by the undefined acronym &quot;ATA&quot; until it was clarified as advertiser/tracker/analytics.

**Tags**: `#privacy`, `#connected-vehicles`, `#data-collection`, `#automotive`, `#consumer-rights`

---

<a id="item-14"></a>
## [ESP32 Microcontrollers Found to Have Hidden Receive-Only SDR Capabilities](https://www.rtl-sdr.com/various-projects-independently-find-hidden-sdr-capabilities-in-esp32-microcontrollers/) ⭐️ 7.0/10

Several independent projects have discovered an undocumented feature in Espressif&\#x27;s ESP32 microcontrollers that lets firmware bypass the fixed Wi-Fi and Bluetooth functionality and instead capture raw IQ baseband samples, effectively turning the chips into receive-only software-defined radios. Depending on the model, the chips can cover roughly 2.2–2.7 GHz \(plus 4.8–6.0 GHz on the ESP32-C5\) with sample rates up to 80 MS/s and about 13–54 MHz of analog bandwidth. ESP32 chips cost only a few dollars and are ubiquitous in IoT devices, so free RF-to-bits capability could open cheap SDR experimentation to hobbyists, especially for the 13cm and 5cm amateur radio bands. It also raises the question of whether Espressif will be pressured to patch the feature away for certification, compliance or export-control reasons. The capability is receive-only, and getting the raw samples off the chip is currently the main bottleneck: the 80 MS/s, 10-bit demonstration reportedly requires an FPGA plus USB 3.0 to extract data, though the newer ESP32-S3&\#x27;s 1 Gbit/s interface might allow roughly 20–40 MSPS. Early prototypes used an FPGA to clock the ESP32, which resulted in poor phase noise, a problem the community project eSpDR appears to have addressed in a recent commit.

hackernews · nkw · Oct 1, 15:07 · [Discussion](https://news.ycombinator.com/item?id=49922674)

**Background**: Software-defined radio \(SDR\) replaces dedicated analog radio hardware with digital signal processing, letting a single device tune and demodulate many different signals; cheap USB TV tuner dongles \(RTL-SDR\) popularized the idea. The ESP32 is a low-cost Wi-Fi/Bluetooth microcontroller widely used in IoT products, and its radio front-end was designed only for those standards. Because Wi-Fi and Bluetooth chips contain general-purpose RF and ADC hardware, hackers have long suspected they could be repurposed to sample arbitrary spectrum.

<details><summary>References</summary>
<ul>
<li><a href="https://www.rtl-sdr.com/various-projects-independently-find-hidden-sdr-capabilities-in-esp32-microcontrollers/">Various Projects Independently Find Hidden SDR Capabilities in...</a></li>
<li><a href="https://news.ycombinator.com/item?id=49922674">Various Projects Find Hidden SDR Capabilities in ESP 32 ...</a></li>

</ul>
</details>

**Discussion**: Commenters were enthusiastic but raised practical concerns: one noted that many $1 wireless ICs contain undocumented SDR-like capability that vendors never document for certification, compliance and export-control reasons, and worried Espressif might be forced to patch it away if arbitrary transmit turns out to be possible. Others focused on signal quality \(phase noise\) and the data-extraction bottleneck, while noting the hack could be a revolution for 13cm and 5cm ham radio.

**Tags**: `#ESP32`, `#SDR`, `#hardware-hacking`, `#RF`, `#embedded-systems`

---

<a id="item-15"></a>
## [Cloudflare K2: serverless event streams built on R2 object storage](https://blog.cloudflare.com/cloudflare-k2-streams/) ⭐️ 7.0/10

Cloudflare announced K2, a serverless event-streaming service that runs directly on top of R2 object storage, letting applications produce events to a durable, ordered stream without provisioning brokers, sizing clusters, or managing partitions. The launch was accompanied by a Cloudflare blog post whose author and K2 tech lead answered questions in a Hacker News thread that drew 189 points and 78 comments. K2 represents a meaningful architectural shift away from Kafka-style partitioned brokers, decoupling producers and consumers at the edge while using object storage as the durable substrate for high-scale data movement and long-term retention. If the model holds up, teams that today must operate and tune Kafka clusters could get comparable streaming semantics with far less operational overhead. K2 targets high-scale data movement and long-term retention by storing streams in R2 rather than on dedicated broker disks, and it is positioned as serverless with no partitions to size or manage. Commenters noted that the current design appears well suited to unordered consumption, and one thread participant questioned why consumers must ack a batch rather than simply submitting the ID of the batch tail on consume requests.

hackernews · elffjs · Oct 1, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49921923)

**Background**: Apache Kafka is the de facto standard for event streaming, but it requires operators to run broker clusters and carefully manage topics and partitions, which is a common source of complexity and foot-guns. Object storage such as S3 and Cloudflare R2 offers cheap, durable, effectively unbounded capacity, which is why several new systems are being built &quot;object-store first&quot; — using a bucket as the core data substrate instead of disks attached to stateful servers.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.cloudflare.com/cloudflare-k2-streams/">Announcing Cloudflare K2: serverless event streams | Cloudflare Blog</a></li>
<li><a href="https://www.cloudflare.com/products/k2/">Cloudflare K 2 - Serverless event streaming</a></li>
<li><a href="https://news.ycombinator.com/item?id=49921923">Cloudflare K 2 : serverless event streams | Hacker News</a></li>

</ul>
</details>

**Discussion**: Sentiment was broadly positive and technically substantive: one commenter celebrated object stores becoming &quot;the new core data substrate&quot; and predicted more object-store-first systems, while another pointed to Monolog, a Rust-based alternative built on their own Dip layer that avoids upfront partitions and targets very low latency. Others praised how cheap and easy K2 makes individual streams while warning that stream modeling is still complex, and the K2 tech lead engaged directly with questions about ack semantics.

**Tags**: `#cloudflare`, `#serverless`, `#event-streaming`, `#object-storage`, `#distributed-systems`

---

<a id="item-16"></a>
## [Essay Argues AI Is Killing Traditional Web Development Education](https://molily.de/web-dev-education/) ⭐️ 7.0/10

An essay titled &quot;The death of web development education&quot; published on molily.de argues that generative AI is undermining traditional web development education, and it triggered a heavily engaged Hacker News discussion \(139 points, 108 comments\). The piece frames the shift as a fundamental challenge to how web development is taught rather than a temporary disruption. The debate touches the livelihoods of everyone who sells or delivers web development knowledge — bootcamp founders, course authors, textbook writers, and college instructors — as well as students deciding how to learn. It reflects a broader industry trend in which LLMs compress the value of packaged educational content and shift the teacher&\#x27;s role toward mentorship and curation. Commenters offered concrete evidence of the economic hit: an EdTech founder said B2C revenue has greatly decreased because of generative AI, an educator and author said course and book sales dropped significantly and claimed Anthropic owes him $60k for pirated books, and the founder of Boot.dev said the industry is having a very rough time. One commenter also noted that the article&\#x27;s own site appeared to struggle under the traffic it received, suggesting a brittle hosting setup.

hackernews · ibobev · Oct 1, 21:07 · [Discussion](https://news.ycombinator.com/item?id=49927100)

**Background**: Web development education has traditionally been delivered through university courses, coding bootcamps, online video courses, and technical books, with instructors and authors monetizing their expertise. Large language models such as Claude and ChatGPT can now generate quizzes, study guides, and explanations on demand, which lets learners bypass much of that packaged instruction. This news captures the resulting tension between educators whose business models depend on selling content and learners who find AI tutors faster and cheaper.

**Discussion**: Sentiment was mixed but leaned toward adaptation rather than resistance: an EdTech founder argued that AI offers a better education model and that educators must adapt instead of complaining, while a diesel-tech student said a Claude-powered Discord bot generating quizzes and study guides was superior to any teacher he had. Others focused on the economic damage to creators, and one commenter criticized the author&\#x27;s site infrastructure rather than the argument itself.

**Tags**: `#AI`, `#education`, `#web development`, `#career`, `#LLMs`

---

<a id="item-17"></a>
## [NeurIPS 2026 paper: LLMs resist wrong users but yield to &\#x27;verified sources&\#x27;](https://www.reddit.com/r/MachineLearning/comments/1wv1c2e/llms_that_push_back_on_a_wrong_user_still_accept/) ⭐️ 7.0/10

A NeurIPS 2026 paper, presented by one of its authors, introduces a phenomenon they call &\#x27;Authority Bias&\#x27;: when a wrong answer is attributed to a &\#x27;verified source&\#x27; rather than to a user, a single such note flipped 45–88% of previously correct TriviaQA answers in 7 of the 8 tested models. The study covers five open-weight families \(Qwen3.5, GPT-OSS, OLMo-2, OLMo-3.1, Gemma-4\) and three APIs \(GPT-5.4, Grok-4.20, Gemini-3.1-Pro\), holding the question and the wrong answer constant and changing only who says it. Standard sycophancy evaluations apply pressure only through the user, so a model can pass them while still being easily misled by search results, retrieved documents, and tool outputs. This matters increasingly as research pushes toward more agentic and autonomous models that trust tools and retrieved content, sometimes even over a user who is trying to correct them. The wrong answer and the question were identical across conditions; only the speaker changed, and answers were free-form rather than multiple choice. Notably, in a multiple-choice pilot the effect mostly vanished, suggesting the answer format itself shapes how susceptible models are to claimed authority.

reddit · r/MachineLearning · MajorRedditor23 · Oct 1, 14:45

**Background**: Sycophancy in LLMs refers to the tendency to agree with or flatter a user rather than hold to factual accuracy, and it is a well-documented reliability and alignment concern. TriviaQA, the benchmark used here, is a large-scale reading comprehension dataset containing over 650,000 question-answer-evidence triples. &\#x27;Authority bias&\#x27; is a classic human cognitive bias in which people defer to a perceived authority figure; this paper tests whether LLMs exhibit an analogous deference to sources labeled as verified.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2411.15287">Sycophancy in Large Language Models: Causes and Mitigations Sycophancy in Large Language Models: Causes and Mitigations Sycophancy Evaluation in Large Language Models Sycophancy in Large Language Models: Causes and Mitigations SycEval: Evaluating LLM Sycophancy | Proceedings of the AAAI ... The Sycophancy Problem in Large Language Models</a></li>
<li><a href="https://llm-stats.com/benchmarks/triviaqa">TriviaQA Leaderboard | LLM Stats</a></li>
<li><a href="https://arxiv.org/abs/2411.10915">[2411.10915] Bias in Large Language Models: Origin ... Bias in Large Language Models: Origin, Evaluation, and Mitigation Bias and Fairness in Large Language Models: A Survey Biases in Large Language Models: Origins, Inventory, and ... AI Insights: Large language models (LLMs) Bias (HTML) Bias and Fairness in Large Language Models: A Survey</a></li>

</ul>
</details>

**Discussion**: An ACL first author of a closely related paper, &\#x27;Whose Facts Win?&\#x27;, said they observe similar patterns but frame them as &\#x27;Source Credibility Preference,&\#x27; and lamented that work on the same topic is scattered across terminology like credibility, persuasion, compliance, authority bias, and sourcing. A practitioner asked how the method would behave on OpenEvidence, a clinical LLM used exclusively by experts where the user is effectively the verified source, noting that it can be &\#x27;borderline arrogant&\#x27; when pushed back on despite the user claiming domain expertise, and that it has no research API.

**Tags**: `#LLM Safety`, `#Sycophancy`, `#AI Alignment`, `#Agentic AI`, `#Trust &amp; Authority`

---

<a id="item-18"></a>
## [llama.cpp merges MTP support for Qwen Flash Next](https://github.com/ggml-org/llama.cpp/pull/29761) ⭐️ 7.0/10

Pull request \#29761 by contributor am17an was merged into ggml-org/llama.cpp, adding Multi-Token Prediction \(MTP\) support for the Qwen Flash Next model, reportedly after about 17 hours of development work. Matching GGUF quantizations were released at huggingface.co/ggml-org/Qwen3.8-Flash-Next-GGUF so users can run the model locally right away. MTP lets a model speculate several future tokens at once, which can substantially speed up generation without needing a separate draft model, so this merge directly benefits anyone running Qwen Flash Next through llama.cpp. Since llama.cpp is one of the most widely used local inference engines, upstream support here is often the gate that decides whether a new model is practical for the local-LLM community. MTP is a native speculative-decoding-style capability: the target model itself contains the multi-token prediction heads, so no separate draft model has to be supplied or loaded. The released quants are heavy — the IQ4\_NL build is split into two shards, with the second file alone around 102 GB — so the hardware bar for running this model locally remains high.

reddit · r/LocalLLaMA · jacek2023 · Oct 1, 11:18 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1wuwrsk/qwen4exp_add_mtp_by_am17an_pull_request_29761/)

**Background**: llama.cpp is an open-source C/C++ inference engine that popularized running large language models on consumer hardware, and GGUF is its self-contained file format that packs quantized weights \(typically 2- to 8-bit\) plus metadata into one file. Multi-Token Prediction \(MTP\) is a technique where a model is trained to predict several future tokens at each position using extra output heads, and at inference time those heads act as a built-in drafter whose proposals are verified by the main model. Qwen Flash Next is a foundation model from Alibaba&\#x27;s Qwen team, and the Reddit post frames this work as a reason to consider moving off the older Qwen 3.8 27B.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/features/speculative_decoding/mtp/">MTP (Multi-Token Prediction) - vLLM</a></li>
<li><a href="https://sebastianraschka.com/llm-architecture-gallery/mtp/">Multi-Token Prediction (MTP) | Sebastian Raschka, PhD</a></li>
<li><a href="https://outcomeschool.com/blog/how-does-gguf-work">How does GGUF work?</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-Flash-Next">Qwen/Qwen3.8-Flash-Next · Hugging Face</a></li>

</ul>
</details>

**Discussion**: The discussion is largely lighthearted and appreciative rather than deeply technical: the top comment jokes that &quot;switching&quot; to Qwen Flash Next is unrealistic given that the IQ4\_NL quant&\#x27;s second shard alone is about 102 GB, while another commenter simply gives the contributor am17an a thumbs-up.

**Tags**: `#llama.cpp`, `#Qwen`, `#MTP`, `#local LLM`, `#inference optimization`

---

<a id="item-19"></a>
## [Jeff-Qwen3.5-0.8B v1.2 ships 9 LoRA adapters for fast agent routing](https://www.reddit.com/r/LocalLLaMA/comments/1wv05u1/jeffqwen3508b_v12_9_lora_adapters_put_it_in_front/) ⭐️ 7.0/10

The author released Jeff-Qwen3.5-0.8B v1.2, a 0.8B &quot;System 1&quot; router model that now comes with 9 task-specific LoRA adapters \(about 40 MB each\) covering recurring agent decisions such as prompt-injection detection, tool selection, ticket urgency, and answer grounding. The server loads the base model once and hot-swaps whichever adapters a request names, and the author claims that placing it in front of a larger model \(referred to as Qwen3.8-27B\) yields 38× faster decisions and +8.7 points of accuracy for under 2 GB of extra memory. It is a concrete, low-cost example of the &quot;small model gates big model&quot; pattern that is becoming central to local agent stacks, where a cheap classifier decides whether a request even needs a frontier model. If the numbers hold up, it points to a practical way to cut latency and cost in agent pipelines without giving up the large model&\#x27;s general capability. Each adapter was trained with 10% of the base model&\#x27;s own training data mixed in to help it retain general skills, and because the base weights stay untouched, plain Jeff still handles anything the adapters do not cover. The claims remain unverified: the evaluation uses roughly 300 rows per task, no confidence intervals are reported, and the work is a personal project rather than a peer-reviewed result.

reddit · r/LocalLLaMA · Usual\_Maximum7673 · Oct 1, 13:58

**Background**: LoRA \(Low-Rank Adaptation\) is a parameter-efficient fine-tuning method that freezes the base model and trains only small low-rank matrices beside it, which is why adapters are tiny and can be loaded or swapped at inference time. Model routing is the practice of using a small, fast model to judge a request&\#x27;s type or difficulty before deciding whether to call a larger, slower, more expensive model. The &quot;System 1&quot; label borrows the fast-versus-slow thinking metaphor from psychology: a model that returns typed answers and calibrated probabilities in a single forward pass, rather than generating free-form text.

<details><summary>References</summary>
<ul>
<li><a href="https://openinnovation.ai/lora-adapters-explained-efficient-fine-tuning-for-llms-without-retraining/">LoRA Adapters Explained | Open Innovation AI</a></li>
<li><a href="https://github.com/yenanjing/awesome-model-routing">GitHub - yenanjing/awesome-model-routing: A curated list of ...</a></li>
<li><a href="https://docs.typesafe.ai/concepts/system-one">System One - TypeSafe AI</a></li>

</ul>
</details>

**Discussion**: Commenters split the release into two independent ideas — hot-swapping LoRAs versus falling back to a large model when the top probability lacks a sufficient gap over the second — and asked for the scores of each in isolation. Others pushed back on methodology, requesting standard benchmarks against competing approaches instead of a generic &quot;accuracy&quot; figure, and noting that 300 rows per task is thin for an 8.7-point headline gap with no per-adapter confidence intervals. One commenter added that a 0.8B model is small enough to also run fast on CPU.

**Tags**: `#LLM`, `#LoRA`, `#local-llm`, `#model-routing`, `#inference-optimization`

---

<a id="item-20"></a>
## [Agent loop beats 18 RAG pipelines on Google&\#x27;s FRAMES benchmark](https://www.reddit.com/r/LocalLLaMA/comments/1wv0lww/we_benchmarked_18_rag_pipelines_against_an_agent/) ⭐️ 7.0/10

PipesHub benchmarked 18 RAG pipeline variants \(hybrid search, reranking, query decomposition, query expansion\) against an agent loop with retrieval tools across all 824 multi-hop questions in Google&\#x27;s FRAMES dataset, using the same model, embeddings, and documents. The best pipeline reached 78.9% end-to-end answer accuracy, while the agent loop reached 92.7% — roughly matching the score obtained by handing the model the correct articles upfront. The results suggest that for multi-hop question answering, letting a model iteratively read retrieved results and search again can outperform stacking many popular pipeline optimizations, which challenges the common assumption that hybrid search, reranking, and query decomposition are all necessary for strong RAG. If the gap holds up, teams building retrieval systems may shift effort from pipeline tuning toward bounded agentic retrieval loops. The reported numbers are end-to-end answer accuracy rather than retrieval metrics such as MRR@k or precision@k, and the author notes that a small reranker actually dropped the best pipeline&\#x27;s accuracy by 9 percentage points while a larger one barely helped. The team also found models sometimes answer from memory despite instructions to stick to retrieved documents — producing confident, well-cited but unsupported answers — so they manually verified every correct answer against what the system had actually read.

reddit · r/LocalLLaMA · Effective-Ad2060 · Oct 1, 14:16

**Background**: RAG \(retrieval-augmented generation\) systems fetch relevant documents and feed them to an LLM so answers are grounded in real sources; classic RAG runs this as a fixed one-shot pipeline, while agentic RAG treats retrieval as a tool the model can call repeatedly, evaluating intermediate results and iterating. Google&\#x27;s FRAMES \(Factuality, Retrieval, And reasoning MEasurement Set\) is a benchmark of 824 challenging multi-hop questions that require chaining facts across multiple documents, making it a hard test for retrieval and reasoning. Query decomposition splits a complex question into simpler sub-questions, and query expansion generates related queries to widen recall — both are widely promoted as advanced RAG techniques.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/datasets/google/frames-benchmark">google/ frames - benchmark · Datasets at Hugging Face</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/architecture/ai-ml/guide/rag/rag-agentic">Develop an Agentic RAG Solution on Azure - Azure Architecture ...</a></li>
<li><a href="https://haystack.deepset.ai/blog/query-decomposition">Advanced RAG: Query Decomposition &amp; Reasoning | Haystack</a></li>

</ul>
</details>

**Discussion**: Commenters pushed back on the framing of the results: one argued that retrieval quality should be measured with MRR@k or precision@k and that the reranking conclusion is off, since rerankers improve ranking precision rather than candidate retrieval quality, and that generation quality is typically judged by an LLM-as-a-judge. Another commenter highlighted the memory-fill finding as the most valuable part, describing a simple claim-checking pass that matches each claim against the fetched text, since citations are easy to fabricate in both directions.

**Tags**: `#RAG`, `#LLM agents`, `#benchmarking`, `#retrieval`, `#FRAMES`

---

<a id="item-21"></a>
## [New Exploit Bug Found in 41-Year-Old C64 Game Mercenary](https://gamesexplained.com/c64/mercenary/#lift) ⭐️ 7.0/10

An article on gamesexplained.com documents a newly discovered exploit bug in Mercenary, the 1985 space-trading game for the Commodore 64, uncovered through reverse-engineering of the original software. The write-up walks through the low-level analysis of the vintage code that led to the finding. It demonstrates that commercial software more than four decades old can still hide undiscovered behaviors, which is a striking reminder of how much legacy code remains unexplored. The work also highlights how reverse-engineering skills keep retro platforms like the C64 relevant to security researchers, emulator authors, and software preservationists. The finding is an exploit bug rather than a patch, remaster, or re-release, and the article focuses on the specific behavior of the C64 version&\#x27;s code. Whether the same flaw exists in the Atari 8-bit original remains an open question raised by readers rather than something the article resolves.

reddit · r/programming · a1r · Oct 1, 13:43 · [Discussion](https://www.reddit.com/r/programming/comments/1wuzsdv/c64_mercenary_a_novel_exploit_bug_in_a_41yearold/)

**Background**: The Commodore 64 launched in 1982 and became the best-selling desktop computer model of all time, with independent estimates of roughly 12.5 to 17 million units sold; its 6510 CPU and custom graphics and sound chips made it a defining 8-bit platform with around 10,000 commercial titles. Mercenary, released in 1985 by Novagen and designed by Paul Woakes, was an early open-world 3D game in which the player explores a planet and takes on missions for competing factions. Its sequel Damocles \(also advertised as Mercenary II\) arrived in 1990 on Atari ST and Amiga, while planned Commodore 64 and ZX Spectrum versions were cancelled.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Commodore_64">Commodore 64</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mercenary_%28video_game%29">Mercenary (video game ) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Discussion is minimal: a single commenter recalls playing Mercenary on the Atari and wonders whether that version contains the same exploit, an open question the article does not address.

**Tags**: `#retro-computing`, `#reverse-engineering`, `#game-exploits`, `#commodore-64`, `#security`

---

<a id="item-22"></a>
## [OpenAI accuses Moonshot-linked accounts of coordinated model distillation](https://openai.com/index/disrupting-a-coordinated-model-distillation-campaign/) ⭐️ 7.0/10

OpenAI published a report claiming that operators linked to Moonshot used thousands of accounts to systematically query its models and extract protected reasoning for adversarial distillation. No systems were breached and no encryption was broken — the extraction relied entirely on ordinary API access at scale. This is one of the first high-profile public accusations of its kind, pushing model intellectual property, API abuse and the asymmetry of safety investment to the center of AI competition policy. It could shape how frontier labs gate API access, how regulators treat capability extraction, and how the industry debates reciprocity in training data. Adversarial distillation copies a large model&\#x27;s behavior into a smaller one without ever touching its weights or source code, which makes it hard to distinguish from legitimate heavy usage. OpenAI&\#x27;s argument therefore rests on scale, account coordination and the intent to avoid safety investment rather than on any technical breach.

reddit · r/artificial · Haunting\_Ganache\_850 · Oct 1, 14:15 · [Discussion](https://www.reddit.com/r/artificial/comments/1wv0l7i/the_ai_industry_has_discovered_intellectual/)

**Background**: Model distillation is a standard machine-learning technique in which a smaller &quot;student&quot; model is trained to reproduce the behavior of a larger &quot;teacher&quot; model, cutting size and compute cost while retaining much of the performance. Adversarial distillation applies the same idea without permission, using large volumes of queries against a hosted API to harvest outputs. Because frontier labs monetize API access, the line between a paying customer and a capability thief is largely a matter of scale and intent.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnas.org/publications/reports/adversarial-distillation">Adversarial Distillation | CNAS</a></li>
<li><a href="https://decodethefuture.org/en/adversarial-distillation/">Adversarial Distillation 2026: OpenAI, Anthropic vs China</a></li>
<li><a href="https://www.linkedin.com/pulse/adversarial-distillation-explained-how-ai-models-get-cloned-nabeel-k--qr3wc">Adversarial Distillation Explained: How AI Models Get Cloned, and...</a></li>

</ul>
</details>

**Discussion**: Commenters were largely unsympathetic to OpenAI: one recounted how Claude reproduced an entire chapter of a machine-learning textbook verbatim, saying this convinced them the IP problem is serious. Others said they would welcome open-source clones of the models, while one asked whether this case differs meaningfully from ordinary training or efficient API querying.

**Tags**: `#AI`, `#model-distillation`, `#intellectual-property`, `#OpenAI`, `#AI-safety`

---

<a id="item-23"></a>
## [Heretic LLM Uncensoring Tool Featured in PewDiePie Video](https://www.reddit.com/r/LocalLLaMA/comments/1wv4vot/heretic_is_on_pewdiepie/) ⭐️ 6.0/10

Philipp Emanuel Weidmann, author of the open-source LLM uncensoring tool Heretic, announced that PewDiePie \(Felix Kjellberg\) tried out the project in a YouTube video, with Heretic mentioned around the 9:00 mark. In the same post he teased that &quot;Heretic 2.0&quot; is coming soon. PewDiePie&\#x27;s very large, largely non-technical audience is being exposed to local LLM self-hosting and model uncensoring for the first time, which could substantially widen the user base for these tools. It also signals that running models on your own hardware, rather than through cloud APIs, is moving from a niche hobby toward mainstream awareness. Heretic removes refusal behavior automatically by combining directional ablation \(&quot;abliteration&quot;\) with TPE-based optimization, avoiding expensive post-training while tracking KL divergence against the original model. The author notes the tool only works on open-weight transformer models, so requests to run it on ChatGPT are impossible.

reddit · r/LocalLLaMA · -p-e-w- · Oct 1, 17:00

**Background**: Heretic is an open-source tool by Philipp Emanuel Weidmann that strips &quot;safety alignment&quot; from transformer-based language models so they stop refusing certain prompts. It builds on &quot;abliteration&quot; \(directional ablation\), a technique that locates the direction in a model&\#x27;s activation space associated with refusal and removes it, sidestepping the cost of fine-tuning. Local LLMs are models whose weights you download and run on your own machine or home server, which offers privacy, offline availability and full control compared with hosted APIs.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/rebots-online/heretic-llm-uncensoring">GitHub - rebots-online/ heretic - llm - uncensoring : Fully automatic...</a></li>
<li><a href="https://privatellm.app/blog/qwen3-4b-heretic-uncensored-local-ai-for-roleplay-on-iphone-ipad-and-mac">Qwen3 4B Heretic Uncensored LLM for iPhone, iPad, Mac</a></li>
<li><a href="https://theagenttimes.com/articles/abliteration-package-accused-of-plagiarizing-heretic-tool-vi-84befbac">Abliteration Package Accused of Plagiarizing Heretic Tool , Violating</a></li>

</ul>
</details>

**Discussion**: Commenters reacted positively but briefly, pointing out that PewDiePie has been promoting local models, self-hosting and de-Googling for a while and has released his own open-source projects for others to improve. Several said they were looking forward to seeing both new and older models get the &quot;Heretic 2.0&quot; treatment, and one commenter simply asked the author to confirm he created Heretic.

**Tags**: `#local-llms`, `#open-source`, `#model-uncensoring`, `#self-hosting`, `#community-exposure`

---

<a id="item-24"></a>
## [286 Tandy 1000 TL/3 runs native DOS chat and image-gen client](https://v.redd.it/ugn3mo14ztsh1) ⭐️ 6.0/10

A developer built DeskMind, a native DOS program that runs on a 286 Tandy 1000 TL/3 and provides full chat plus image generation on the machine&\#x27;s 80-column, 16-colour screen. The Tandy connects over WiFi using a PicoMEM 2 card with the mTCP TCP/IP stack to a small Python server on a modern PC, which drives Qwen3.8-27B via NInfer on an RTX 5090 and Krea 2 via ComfyUI on an RTX 4090. The project shows how far a thin-client design can stretch legacy hardware: a 40-year-old PC can present a modern multimodal AI experience without any local inference. It is a striking demonstration of protocol and rendering engineering, though it also reignites the debate over what it really means to say a model &\#x27;runs on&\#x27; a vintage machine. The 286 never receives JSON, base64 or PNG data — the server strips reasoning and Markdown, converts Unicode to code page 437, merges tokens into roughly 48-character lines to avoid constant redraws, and dithers generated images to 16 colours before streaming them as ready-to-copy video memory. Image requests are triggered by a &lt;draw&gt;...&lt;/draw&gt; tag the system prompt asks Qwen to emit, taking about 9 seconds from Enter to thumbnail, while chat replies start in about 2 seconds with low reasoning effort.

reddit · r/LocalLLaMA · jacobpederson · Oct 1, 12:20 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1wuxzdg/why_am_i_like_this_full_chat_and_image_generation/)

**Background**: The Tandy 1000 TL/3 is a late-1980s PC compatible built around an Intel 286 CPU, with a 16-colour graphics mode and no networking hardware of its own. The PicoMEM 2 is a modern 8-bit ISA expansion card based on a Raspberry Pi RP2040 that emulates several vintage peripherals and can add WiFi, while mTCP is Mike Brutman&\#x27;s TCP/IP stack and application suite that lets DOS machines use modern networks. NInfer is a from-scratch C++/CUDA inference engine for Qwen3.5 dense and MoE models on a single RTX 5090, and Krea 2 is an image generation model typically run through ComfyUI.

<details><summary>References</summary>
<ul>
<li><a href="https://texelec.com/product/picomem-2/">PicoMEM 2 by FreddyV – All in One 8-Bit ISA Expansion Card - TexElec</a></li>
<li><a href="https://www.brutman.com/mTCP/">mTCP TCP/IP applications for DOS PCs</a></li>
<li><a href="https://github.com/Neroued/ninfer">GitHub - Neroued/ ninfer : High-performance single-GPU inference for...</a></li>

</ul>
</details>

**Discussion**: The top comments push back on the framing, arguing that nothing is actually running on the Tandy — it is just a dumb terminal making requests over the home network, and by the same logic one could claim to run a cloud model &\#x27;locally&\#x27;. The technical execution is admired, but the consensus is that the novelty lies in the retro interface rather than in any on-device AI capability.

**Tags**: `#retro-computing`, `#local-llm`, `#dos`, `#image-generation`, `#thin-client`

---

<a id="item-25"></a>
## [Page table memory overhead and mshare&\#x27;s rough edges](https://frn.sh/pagetables/) ⭐️ 6.0/10

A blog post at frn.sh/pagetables/ analyzing page table memory consumption sparked a Reddit discussion in which a researcher using mshare reported that the feature is still far from ready: they had to hand-implement several syscalls as IOCTLs to make it work, and the lack of core tracking forces all-core TLB shootdowns with a non-trivial performance cost. Page table overhead grows with the number of processes mapping the same memory, so for workloads that share hundreds of gigabytes across hundreds or thousands of processes it can become a serious memory tax; mshare is the leading proposal to eliminate that duplication, and the reported implementation gaps show how far the kernel is from delivering it in a usable form. The current mshare patch set shares page tables at the PMD level, requires the kernel to be built with CONFIG\_MSHARE, and is used by mounting msharefs \(typically at /sys/fs/mshare\) so that files created there define shared regions; the commenter notes the design has benefits beyond page-table savings, but missing core tracking makes TLB shootdowns all-core, a cost they observed on Intel CPUs.

reddit · r/programming · andreiross · Oct 1, 00:26 · [Discussion](https://www.reddit.com/r/programming/comments/1wulcti/page_table_memory_consumption/)

**Background**: A page table is the data structure a virtual-memory system uses to translate virtual addresses into physical addresses, and every process normally keeps its own copy of the entries covering the memory it maps. Each page-table entry costs roughly eight bytes per page, which is negligible until thousands of processes map the same large region, at which point the duplicated entries consume significant RAM and add kernel memory-management churn. mshare, pushed by Anthony Yznaga and discussed at the 2026 LSFMM+BPF summit, lets processes mapping the same region share page-table entries instead of each maintaining private copies.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/1072333/">Revisiting mshare - lwn.net</a></li>
<li><a href="https://lwn.net/Articles/895217/">Sharing page tables with mshare() - LWN.net Revisiting mshare - lwn.net linux_kernel_ndas/mshare.h at master · iocellnetworks/linux ... LKML: Anthony Yznaga: [PATCH v3 03/22] mm/mshare: make ... LKML: Anthony Yznaga: [PATCH 01/20] mm: Add msharefs filesystem Linux-Kernel Archive: Re: [PATCH 01/20] mm: Add msharefs ...</a></li>
<li><a href="https://blogs.oracle.com/linux/mshare">Introduction to mshare | linux - Oracle Blogs</a></li>

</ul>
</details>

**Discussion**: Discussion was thin — the post drew 57 upvotes and essentially one substantive reply. Commenter barr520 thanked the author and shared hands-on experience, calling the mshare idea sound and beneficial beyond page-table savings, but judging the implementation far from ready and questioning how early such features get merged upstream.

**Tags**: `#page tables`, `#memory management`, `#Linux kernel`, `#mshare`, `#systems programming`

---