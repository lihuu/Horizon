---
layout: default
title: "Horizon Summary: 2026-09-17 (EN)"
date: 2026-09-17
lang: en
---

> From 47 items, 27 important content pieces were selected

---

1. [Nvidia brings native GPU programming to Rust](#item-1) ⭐️ 8.0/10
2. [Paper Cuts Ternary LLM Storage to 1.48 Bits per Weight](#item-2) ⭐️ 8.0/10
3. [Xiaomi Publishes Live Post-Training Dashboard for MiMo 2.6](#item-3) ⭐️ 8.0/10
4. [Mozilla and Mistral Partner for Private, Multilingual AI Browsing](#item-4) ⭐️ 8.0/10
5. [Dream-RSI: Recursive Self-Improvement via Evolving Worlds](#item-5) ⭐️ 8.0/10
6. [Flock Camera Security Flaws Expose Hardcoded Credentials](#item-6) ⭐️ 8.0/10
7. [DeepMind Launches Institute to Research AI&\#x27;s Societal Impact](#item-7) ⭐️ 8.0/10
8. [TMLR probes authors of desk-rejected papers, finds most can&\#x27;t explain their work](#item-8) ⭐️ 8.0/10
9. [China&\#x27;s open-weight AI models now 4 months behind US frontier, Mozilla report says](#item-9) ⭐️ 8.0/10
10. [Offloading KV Cache to RAM Enables 1M Context on 3x 3090 for Qwen3.8-Flash-Next](#item-10) ⭐️ 8.0/10
11. [BYD unveils 600 km electric truck with 1.5 MW megawatt charging](#item-11) ⭐️ 8.0/10
12. [4B LLM Trained to Generate Query Plans Claims 81% Speedup Over Postgres](#item-12) ⭐️ 7.0/10
13. [Small Programming Tricks: Habits and AI Insights](#item-13) ⭐️ 7.0/10
14. [BYD&\#x27;s Formula S EV undercuts Tesla Model 3 at under $29,000](#item-14) ⭐️ 7.0/10
15. [Anthropic Merges Claude Cowork and Chat into One Unified Claude](#item-15) ⭐️ 7.0/10
16. [Suleyman Warns Against Granting AI Models Rights](#item-16) ⭐️ 7.0/10
17. [Apple Reportedly Planning M8 AI Servers with Nvidia Networking](#item-17) ⭐️ 7.0/10
18. [Meta&\#x27;s Muse Spark weights still unreleased, Reddit criticizes broken promise](#item-18) ⭐️ 7.0/10
19. [Qwen3.8 Max \(0902\) tops China AI leaderboard with 45 score](#item-19) ⭐️ 7.0/10
20. [Qwen 3.5 4B with logits rivals TypeSafe&\#x27;s Jev model](#item-20) ⭐️ 7.0/10
21. [Qwen3.8 Flash Hits 15 tok/s on 12GB VRAM with Aggressive Quantization](#item-21) ⭐️ 7.0/10
22. [Git Worktree Gotchas: Common Pitfalls and Best Practices](#item-22) ⭐️ 7.0/10
23. [Hungary intensifies pressure on BYD and CATL over violations](#item-23) ⭐️ 7.0/10
24. [AI Voice Cloning: Treat Voice Samples as Sensitive Data](#item-24) ⭐️ 7.0/10
25. [Google&\#x27;s Vectorized Performance-Portable Quicksort Using SIMD](#item-25) ⭐️ 6.0/10
26. [LARA: Low-Rank Residual Adapters for Frozen LLMs](#item-26) ⭐️ 6.0/10
27. [Qwen 3.8 27B Runs 63 Hours on RTX 3090 Attempting Riemann Hypothesis](#item-27) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Nvidia brings native GPU programming to Rust](https://developer.nvidia.com/blog/introducing-cuda-rust-two-tracks-for-writing-gpu-kernels/) ⭐️ 8.0/10

Nvidia has announced native GPU programming in Rust, introducing two tracks for writing GPU kernels that let Rust developers leverage CUDA directly. This marks a major step for Rust in high-performance and GPU computing. This lowers the barrier for Rust adoption in GPU-accelerated computing and expands the Rust ecosystem into HPC and AI workloads. It also signals Nvidia&\#x27;s commitment to supporting modern systems languages beyond C and C++. The announcement describes two distinct tracks for writing GPU kernels, though specific implementation details are not provided in the summary. Community members are comparing it to existing Rust GPU tools such as Hugging Face&\#x27;s Candle and vectorware.

hackernews · nonmaskable · Sep 16, 11:15 · [Discussion](https://news.ycombinator.com/item?id=49724881)

**Background**: CUDA is Nvidia&\#x27;s proprietary parallel computing platform and API that allows software to use GPUs for general-purpose processing, originally released in 2007. GPU kernels are functions that execute on the GPU, typically written in C/C++ or via frameworks like OpenCL. Rust is a systems programming language focused on memory safety and performance, and this announcement enables Rust developers to write kernels natively without relying on C/C++ wrappers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/CUDA">CUDA</a></li>
<li><a href="https://modal.com/gpu-glossary/device-software/kernel">What is a CUDA Kernel? | GPU Glossary</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some developers express excitement about learning Rust and the new possibilities, while others criticize CUDA&\#x27;s proprietary nature and the difficulty of removing vendor lock-in. Comparisons are drawn to existing tools like Candle and vectorware, and one commenter notes the irony of Nvidia publishing an article that appears to be fully AI-written.

**Tags**: `#Rust`, `#GPU programming`, `#CUDA`, `#Nvidia`, `#HPC`

---

<a id="item-2"></a>
## [Paper Cuts Ternary LLM Storage to 1.48 Bits per Weight](https://arxiv.org/abs/2609.16338) ⭐️ 8.0/10

A new arXiv paper proposes reducing ternary LLM weight storage from 1.58 to 1.48 bits per weight by exploiting the fact that weights are zero about 51% of the time in practice. The technique uses a presence bitmap to encode which weights are non-zero rather than storing all three states explicitly. This addresses an important problem in model efficiency by further shrinking the memory footprint of ternary LLMs, which are already designed for computational efficiency. If practical, it could make ternary models even more attractive for edge deployment and custom silicon implementations, where memory bandwidth is a key bottleneck. The approach relies on a presence bitmap to mark non-zero weight positions, exploiting the observed sparsity of trained ternary weights. The work builds on the BitNet b1.58 line of research, where weights are restricted to the three values -1, 0, and +1, and the gain comes from information-entropy-based packing rather than changing the model itself.

hackernews · matt\_d · Sep 16, 20:59 · [Discussion](https://news.ycombinator.com/item?id=49732931)

**Background**: Ternary LLMs, such as Microsoft&\#x27;s BitNet b1.58, restrict weights to only three values \(-1, 0, +1\), which naively requires about 1.58 bits per weight. Because actual trained weights are zero roughly half the time, a presence bitmap can encode the non-zero positions and reduce the average storage cost to about 1.48 bits per weight. This is an information-theoretic packing improvement over the naive ternary representation, and it aligns with broader efforts to compress LLMs for efficient inference.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/1.58-bit_large_language_model">1.58-bit large language model - Wikipedia</a></li>
<li><a href="https://huggingface.co/microsoft/bitnet-b1.58-2B-4T">microsoft/bitnet-b1.58-2B-4T · Hugging Face</a></li>
<li><a href="https://github.com/microsoft/BitNet">GitHub - microsoft/BitNet: Official inference framework for 1-bit LLMs · GitHub</a></li>

</ul>
</details>

**Discussion**: The discussion is engaged and mixed. Some commenters are enthusiastic, noting that if ternary LLMs are baked into custom silicon they could be &\#x27;shockingly efficient,&\#x27; while another suggests using arithmetic coding to squeeze out even more centi-bits. However, one commenter is skeptical, arguing that ternary quantization doesn&\#x27;t make sense and that vector quantization and trellis-based methods are better for post-training quantization in this regime.

**Tags**: `#LLM`, `#quantization`, `#compression`, `#ternary`, `#arxiv`

---

<a id="item-3"></a>
## [Xiaomi Publishes Live Post-Training Dashboard for MiMo 2.6](https://mimo.xiaomi.com/rl/) ⭐️ 8.0/10

Xiaomi has launched a public, live dashboard at mimo.xiaomi.com/rl/ that streams the reinforcement-learning post-training runs for its MiMo 2.6 models \(mimo-v2.6-pro and mimo-v2.6-flash\) in real time, including reward curves and evaluation metrics straight from the trainer&\#x27;s logs. This is a notable transparency move in the open-source AI space, as most labs keep post-training details private. It lets the community observe model development in real time, which could build trust and set a new precedent for openness in model training, while also putting competitive pressure on closed labs like OpenAI and Anthropic. The dashboard streams live training metrics for both the pro and flash variants of MiMo 2.6. Community benchmarks reference DeepSWE 1.1, where MiMo-v2.5-Pro scored 19%, compared to competitors like Fable at 70%, Kimi K3 at 69%, and Astra at 74% on max effort.

hackernews · r/LocalLLaMA · krackers · Sep 16, 20:09 · [Discussion](https://news.ycombinator.com/item?id=49732270)

**Background**: Reinforcement learning \(RL\) post-training is a phase where a base model is further refined using reward signals to improve specific capabilities like coding or reasoning. Xiaomi&\#x27;s MiMo is an open-source family of LLMs, and the company has been building an ecosystem around it, including desktop apps and integrations with coding tools like Cursor, Cline, and Zed. By streaming training logs publicly, Xiaomi offers an unprecedented look into how its models are developed.

<details><summary>References</summary>
<ul>
<li><a href="https://mimo.xiaomi.com/rl/">mimo -v 2 . 6 RL</a></li>
<li><a href="https://aiweekly.co/alerts/xiaomi-publishes-live-post-training-dashboard-for-mimo-26-rl-run-streams-real">Xiaomi opens live RL post-training dashboard for Mimo 2.6</a></li>
<li><a href="https://github.com/XiaomiMiMo/MiMo-Code">GitHub - XiaomiMiMo/ MiMo -Code: MiMo Code: Where Models and...</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely positive, with users praising the transparency and the cost-effectiveness of MiMo models in real-world engineering work, with one user calling the ROI &\#x27;unbelievably low&\#x27; compared to Anthropic models. Some users noted the competitive threat this poses to closed labs&\#x27; IPOs, while others debated DeepSWE 1.1 benchmark scores and questioned why other providers don&\#x27;t offer similar transparency.

**Tags**: `#AI`, `#open-source`, `#LLM`, `#Xiaomi`, `#model training`

---

<a id="item-4"></a>
## [Mozilla and Mistral Partner for Private, Multilingual AI Browsing](https://mistral.ai/news/mistral-x-mozilla/) ⭐️ 8.0/10

Mozilla and Mistral announced a partnership to integrate private, multilingual AI browsing features into Firefox, including context-aware search, page summaries, and memory retrieval across browser tabs. The features are now live in France and North America, with launches in the UK and Germany planned for later this year. This partnership marks a notable step in AI-assisted browsing, positioning Firefox as a privacy-conscious alternative to Chrome&\#x27;s built-in AI features like Gemini Nano. It could reshape how users interact with AI in browsers and set a precedent for privacy-focused AI integration in the broader ecosystem. The partnership is built on a zero data retention policy, meaning conversations are not stored, and the system supports context-aware search, page summaries, and cross-tab memory retrieval. The rollout is currently limited to France and North America, with the UK and Germany expected later this year.

hackernews · vertigoruntime · Sep 16, 08:08 · [Discussion](https://news.ycombinator.com/item?id=49723408)

**Background**: Local inference runs AI models directly on the user&\#x27;s device, keeping data private but requiring more compute power, while cloud inference sends data to remote servers for processing, offering more power but raising privacy concerns. The core debate around this news centers on whether Mozilla should rely on local small models for privacy-sensitive browsing data instead of cloud inference. On-device AI is generally seen as offering faster responses and greater user privacy since data is processed locally, whereas cloud inference provides scalability and flexibility at the cost of data leaving the device.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/posts/andytillo_llm-inference-training-local-vs-cloud-activity-7253060953687130114-s-8s">LLM Inference training: Local vs . Cloud . | Andy Tillo</a></li>
<li><a href="https://openforge.io/on-device-ai-for-mobile-performance-privacy-and-cost-tradeoffs/">On-Device AI for Mobile: Performance, Privacy, and Cost Tradeoffs OpenForge: Mobile Academy</a></li>
<li><a href="https://arxiv.org/pdf/2605.29450">Protecting On-Device AI Inference: A Systematic Review of ...</a></li>

</ul>
</details>

**Discussion**: Community members expressed concerns that Mozilla is normalizing uploading private browsing history to the cloud, arguing that completely local small-model inference would be a better use case. Some noted similarities to Chrome&\#x27;s built-in Gemini Nano model, while others suggested technical improvements like using a tiny in-browser model to construct advanced search queries. There was also skepticism about the level of trust required for cloud inference, even with zero data retention policies, since end-users cannot easily verify compliance.

**Tags**: `#AI`, `#privacy`, `#web browsing`, `#Mozilla`, `#Mistral`

---

<a id="item-5"></a>
## [Dream-RSI: Recursive Self-Improvement via Evolving Worlds](https://arxiv.org/abs/2609.14858) ⭐️ 8.0/10

The paper introduces Dream-RSI, a framework for scalable and recursively self-improving exploration that uses accumulated discovery history as a replay simulator over the realized search space. It adds a lightweight orchestration layer while leaving the underlying coding agent unchanged. This addresses a key bottleneck in autonomous AI agents—managing and improving exploration strategies—which is critical for recursive self-improvement. It also fuels debate about what truly constitutes RSI and its safety implications. The key insight is that accumulated discovery history can serve as a replay simulator, avoiding expensive rollouts for off-policy evaluation. However, there are open questions about preventing the policy from overfitting to already-discovered branches as the search space expands.

hackernews · bananaflag · Sep 16, 13:44 · [Discussion](https://news.ycombinator.com/item?id=49726955)

**Background**: Recursive self-improvement \(RSI\) is a hypothesized process where an AI system improves its own capabilities, potentially leading to an intelligence explosion. Dream-RSI builds on Danijar Hafner&\#x27;s Dreamer line of work, applying the concept of evolving worlds to exploration in reinforcement learning. The framework makes exploration explicit and programmable, aiming for scalable self-improvement in complex domains.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2609.14858">[2609.14858] Dream-RSI: Recursive Self-Improvement through ...</a></li>
<li><a href="https://dream-rsi.com/">Dream-RSI: Recursive Self-Improvement through Evolving Worlds</a></li>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self - improvement - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters question whether this truly qualifies as RSI, with some calling it an optimization of current training methods rather than perpetual self-improvement. Others raise safety concerns about recursive self-improvement, while some praise the replay simulator idea for avoiding expensive rollouts and ask about overfitting risks. One commenter notes the paper&\#x27;s reference to Dreamer and provides related resources.

**Tags**: `#AI safety`, `#recursive self-improvement`, `#reinforcement learning`, `#research paper`, `#machine learning`

---

<a id="item-6"></a>
## [Flock Camera Security Flaws Expose Hardcoded Credentials](https://www.wired.com/story/hackers-flock-camera-data-shows-how-system-works/) ⭐️ 8.0/10

Security researchers disclosed that Flock Safety&\#x27;s ALPR cameras contain hardcoded credentials and other vulnerabilities, including cleartext storage of code and an enabled debug interface, potentially allowing unauthorized access to the system. The findings were published in collaboration with 404media, and Distributed Denial of Secrets released the camera partition images. Flock cameras are widely deployed in public spaces for law enforcement, making these vulnerabilities a serious public safety and privacy concern. The disclosure highlights systemic security weaknesses in IoT surveillance devices and raises questions about Flock&\#x27;s vulnerability disclosure policies. The hardcoded credential is an API key rather than a password, which can be used to request credentials stored in plaintext that may grant access to Flock&\#x27;s servers. Researchers identified 50+ vulnerabilities overall, including lack of encryption, unauthorized data collection, and physical access exploits, with field maintenance relying on unlocked bootloaders and open diagnostic modes.

hackernews · driverdan · Sep 16, 13:18 · [Discussion](https://news.ycombinator.com/item?id=49726586)

**Background**: Hardcoded credentials are secrets embedded directly into source code or configuration, rather than retrieved at runtime from a secure vault. They are considered a serious security flaw because the same credential is shared across all installations, and attackers who discover it can gain unauthorized access. Flock Safety is a company that deploys automated license plate recognition \(ALPR\) cameras in public spaces for law enforcement use, and inaccuracies in these cameras have previously resulted in wrongful arrests in several cities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://simeononsecurity.com/articles/flock-safety-camera-security-vulnerabilities-research-2026/">Flock Safety Camera Vulnerabilities: 50+ Flaws Found</a></li>
<li><a href="https://cwe.mitre.org/data/definitions/798.html">CWE - CWE-798: Use of Hard-coded Credentials (4.20)</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong criticism of Flock&\#x27;s security practices, calling hardcoded credentials a sign of incompetence and laziness driven by &\#x27;reduced time to market.&\#x27; Several noted that Flock&\#x27;s Vulnerability Disclosure Policy appears designed to create the appearance of responsible security posture while excluding meaningful testing, and pointed out that cameras deployed in unsecured public spaces mean the threat model must include local physical access.

**Tags**: `#security`, `#vulnerability`, `#IoT`, `#surveillance`, `#hardcoded credentials`

---

<a id="item-7"></a>
## [DeepMind Launches Institute to Research AI&\#x27;s Societal Impact](https://institute.deepmind.com/) ⭐️ 8.0/10

DeepMind has announced the launch of the DeepMind Institute, a new think tank dedicated to researching AI&\#x27;s societal impacts and shaping policy. The institute aims to influence AI governance discussions as the field approaches artificial general intelligence \(AGI\). This marks a major AI lab&\#x27;s formal entry into policy and societal-impact research, signaling that AI governance is becoming a core strategic priority. The institute&\#x27;s work could shape how governments and regulators approach AI safety, economics, and deployment. The institute will publish research on topics including economic policy, with proposals such as expanded unemployment insurance, Earned Income Tax Credit, and profit-sharing from AI. It also frames its mission around the approaching AGI, a claim some community members have questioned.

hackernews · vertigoruntime · Sep 16, 14:32 · [Discussion](https://news.ycombinator.com/item?id=49727659)

**Background**: DeepMind is one of the world&\#x27;s leading AI research laboratories, known for breakthroughs like AlphaGo and AlphaFold. Think tanks are research organizations that produce analysis and policy recommendations, often to influence public debate and government decisions. The DeepMind Institute represents a growing trend of AI companies establishing in-house policy research arms to shape the regulatory landscape around AI.

**Discussion**: Community members praised the institute&\#x27;s economic policy article for its sensible proposals, including expanded unemployment insurance and profit-sharing from AI. Others expressed skepticism about the institute&\#x27;s AGI claims and viewed it as an in-house think tank aimed at steering AI policy discussions. One commenter also raised concerns about the competitive pressure between AI labs like OpenAI and Anthropic regarding safety versus speed.

**Tags**: `#AI policy`, `#DeepMind`, `#think tank`, `#AI safety`, `#economics`

---

<a id="item-8"></a>
## [TMLR probes authors of desk-rejected papers, finds most can&\#x27;t explain their work](https://www.reddit.com/r/MachineLearning/comments/1wid67h/tmlr_reached_out_to_the_authors_of_10_papers/) ⭐️ 8.0/10

TMLR&\#x27;s Co-Editor-in-Chief contacted the authors of 10 papers slated for desk rejection and interviewed them about their own work. Of the ten, only one author could answer all questions, while three could not answer basic questions and three struggled with technical details. This finding exposes potential integrity issues in machine learning research submissions, suggesting some submitted papers may not be genuinely understood by their listed authors. It raises serious concerns about peer review practices and the quality of submissions in the ML community. Of the ten submissions, one paper was withdrawn, one author was unavailable, and one author scheduled a meeting but did not show up. The Co-EiC also identified a major flaw in the one paper whose author answered all questions.

reddit · r/MachineLearning · hihey54 · Sep 16, 23:20

**Background**: Desk rejection is a common practice in academic publishing where editors reject a manuscript before it goes to peer review, typically due to poor quality, lack of novelty, or non-compliance with journal scope. TMLR \(Transactions on Machine Learning Research\) is a peer-reviewed journal for machine learning research. This investigation suggests that some authors may be submitting papers they do not fully understand, which undermines research integrity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aischolar.com/news/article/is-desk-rejection-common">Is Desk Rejection Common?</a></li>
<li><a href="https://www.editage.com/insights/new_tags/desk-rejection">desk rejection Archives | Editage Insights</a></li>

</ul>
</details>

**Tags**: `#machine learning`, `#research integrity`, `#peer review`, `#academic publishing`, `#TMLR`

---

<a id="item-9"></a>
## [China&\#x27;s open-weight AI models now 4 months behind US frontier, Mozilla report says](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinas-open-weight-ai-models-are-now-just-4-months-behind-frontier-us-offerings-mozilla-report-claims-models-still-lag-in-some-benchmarks-but-are-drastically-cheaper-to-use) ⭐️ 8.0/10

A Mozilla report claims China&\#x27;s open-weight AI models are now only 4 months behind frontier US offerings, with significantly lower costs despite some benchmark gaps. The report highlights a narrowing gap in AI capability between the two countries. This development signals China&\#x27;s rapid progress in AI and its cost advantage, which could reshape the global AI competitive landscape and influence adoption decisions for businesses and developers. It also underscores the impact of export controls on GPU sales to China. The report notes that while Chinese models lag in some benchmarks, they are drastically cheaper to use, making them attractive for cost-sensitive applications. The 4-month gap represents a significant reduction from previous gaps, though GPU restrictions on China remain a limiting factor.

reddit · r/LocalLLaMA · DustNearby2848 · Sep 16, 17:02 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1wi32jg/chinas_openweight_ai_models_are_now_just_4_months/)

**Background**: Open-weight AI models provide access to the model&\#x27;s weights, allowing users to run, fine-tune, and customize them, unlike closed models. Frontier AI models are the most advanced general-purpose models, typically developed by leading US labs. The Mozilla report compares these two categories to assess the competitive gap.

<details><summary>References</summary>
<ul>
<li><a href="https://www.trustnoww.com/glossary/open-weight-model">Open - Weight Model — Definition | Trustnoww Glossary</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work | NVIDIA Glossary</a></li>

</ul>
</details>

**Discussion**: Reddit comments express that a 4-month gap is &\#x27;good enough&\#x27; for many users, with hopes for a price race to the bottom and more fine-tuning on agentic work. Some commenters argue that without GPU sales restrictions, China would be 4 months ahead, while others question the report&\#x27;s regional security findings and discuss the open-source gap.

**Tags**: `#AI`, `#open-source models`, `#China`, `#benchmarks`, `#cost`

---

<a id="item-10"></a>
## [Offloading KV Cache to RAM Enables 1M Context on 3x 3090 for Qwen3.8-Flash-Next](https://www.reddit.com/r/LocalLLaMA/comments/1whx5xi/you_can_offload_most_of_qwen38flashnexts_kv_cache/) ⭐️ 8.0/10

A Reddit user demonstrated that most of Qwen3.8-Flash-Next&\#x27;s KV cache can be offloaded to system RAM, achieving 1M-token context on three RTX 3090 GPUs with only a modest decode speed drop \(from ~80 to ~60 tok/s after the QSA budget is reached\). The implementation was made to work on vLLM, and the patches and model are available on the user&\#x27;s Hugging Face page. This technique enables running extremely long contexts \(1M tokens\) on consumer-grade hardware, potentially making long-context inference more accessible. Since the architecture is expected to underpin future Qwen models, this approach could be broadly applicable to upcoming local LLM deployments. Decode speed is bandwidth-bound: each step reads all weights and required attention state, so offloading works because the Qwen3-Next architecture \(qwen4\_exp\) uses sparse attention \(QSA\) that limits per-step KV reads. Prefill at 248k context reaches 3,701 tok/s, and throughput is ~150 tk/s at 4 concurrent requests.

reddit · r/LocalLLaMA · sadnessdevil · Sep 16, 13:24

**Background**: The KV cache stores intermediate key and value computations during autoregressive generation, avoiding redundant recomputation and speeding up inference. Normally it is kept in VRAM for fast access, but it grows with context length, often exceeding GPU memory. Qwen3.8-Flash-Next is a 125B-parameter MoE model with 6B active parameters per token, based on the architecture that will underpin Qwen 4. Its sparse attention mechanism \(QSA\) reduces the attention state read per step, making it feasible to store most of the KV cache in system RAM without significant decode slowdown.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-Flash-Next">Qwen / Qwen 3.8-Flash-Next · Hugging Face</a></li>
<li><a href="https://vllm.ai/">vLLM — Fast, Memory-Efficient LLM Inference &amp; Serving</a></li>
<li><a href="https://arxiv.org/html/2603.20397v1">KV Cache Optimization Strategies for Scalableand Efficient LLM Inference</a></li>

</ul>
</details>

**Discussion**: Community members expressed interest and asked for more details, such as the exact setup with three 3090s and prefill performance at lower GPU counts. One user speculated about whether Qwen 4 can improve long-range reasoning or if this architecture mainly benefits chat-based models. Overall sentiment is positive, with users eager to try the approach.

**Tags**: `#KV cache offloading`, `#Qwen`, `#local LLM inference`, `#context length`, `#vLLM`

---

<a id="item-11"></a>
## [BYD unveils 600 km electric truck with 1.5 MW megawatt charging](https://electrek.co/2026/09/14/byd-ett-44-electric-truck-megawatt-charging/) ⭐️ 8.0/10

BYD has unveiled a flagship electric truck offering a 600 km range and 1.5 MW megawatt charging capability. This announcement marks a major step in heavy-duty truck electrification, targeting fleet uptime and operational efficiency. This development directly addresses the critical issue of fleet uptime by enabling rapid charging, which could accelerate the adoption of electric trucks in freight and logistics. It also underscores the growing importance of megawatt charging infrastructure and battery chemistry choices for the commercial vehicle sector. The truck leverages the Megawatt Charging System \(MCS\) standard, which supports up to 3.75 MW per connector, though BYD&\#x27;s implementation is rated at 1.5 MW. The 1.5 MW rate allows a substantial range replenishment in about 20 minutes, and the vehicle is likely to use LFP battery chemistry, which offers longer cycle life and can be charged to 100% without significant degradation.

reddit · r/electricvehicles · i\_marketing · Sep 16, 03:28 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1whlsxs/byd_unveils_flagship_600_km_electric_truck_with/)

**Background**: The Megawatt Charging System \(MCS\) is a high-power DC fast-charging connector and protocol standard developed by CharIN, originally designed for heavy-duty electric trucks and commercial vehicles. It supports charge rates up to 3,000 kW \(3 MW\) at voltages up to 1,250V DC and currents up to 3,000A. LFP \(lithium iron phosphate\) batteries are increasingly favored for commercial EVs due to their longer cycle life, thermal stability, and ability to charge to 100% without degradation, compared to NCM \(nickel-cobalt-manganese\) batteries which typically require a lower charge limit to preserve lifespan.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Megawatt_Charging_System">Megawatt Charging System - Wikipedia</a></li>
<li><a href="https://www.sciencedirect.com/science/article/pii/S2590174526002448">Megawatt charging system for electric vehicles: Design ...</a></li>
<li><a href="https://autoedgeview.com/charging-guides/megawatt-charging-system-explained-ev-owners">Megawatt Charging System Explained: What MCS Means for EV ...</a></li>

</ul>
</details>

**Discussion**: Community comments reflect a mix of optimism and practical concerns. One user jokingly predicts diesel prices will force adoption, while another argues that LFP batteries will dominate open markets due to their superior cycle life and full-charge capability. A third commenter, working in traffic/ITS, highlights the real-world constraint of 1.5 MW per bay, noting that substation upgrades, utility coordination, and demand charges are significant hurdles for fleet deployment.

**Tags**: `#EV trucks`, `#megawatt charging`, `#BYD`, `#battery technology`, `#infrastructure`

---

<a id="item-12"></a>
## [4B LLM Trained to Generate Query Plans Claims 81% Speedup Over Postgres](https://rohanbansal.com/qorl) ⭐️ 7.0/10

A 4B-parameter LLM was trained via distillation from Astra trajectories to generate query plans, achieving a 1.81x geometric mean speedup and a 44.7% summed latency decrease compared to Postgres on an 8GB in-memory dataset with read-only SELECT queries. This work explores using LLMs for query optimization, a novel approach that could reshape database performance tuning. However, the narrow evaluation on a small in-memory dataset with read-only queries raises questions about its generalizability to real-world OLTP workloads. The training cost approximately $800 for renting a 2x H100 SXM node from Lambda for ~95 hours, plus ~$400 in OpenAI API fees for generating Astra trajectory demonstrations. The evaluation used an 8GB dataset that fits entirely in memory, with shared\_buffers constrained to a fraction of that, queries warmed before measuring, and only read-only SELECTs.

hackernews · polyphilz · Sep 16, 18:50 · [Discussion](https://news.ycombinator.com/item?id=49731285)

**Background**: A query plan is a sequence of steps a database uses to execute a SQL query, and query optimizers typically use cost-based heuristics to select the most efficient plan. This work instead trains an LLM to generate query plans directly, but the limited evaluation scope makes it unclear whether the approach would outperform traditional optimizers on larger, more realistic workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Query_plan">Query plan - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/dbms/query-optimization-in-relational-algebra/">Query Optimization - GeeksforGeeks</a></li>
<li><a href="https://www.ibm.com/think/topics/query-optimization">What Is Query Optimization? | IBM</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about the 81% claim, noting the evaluation used an 8GB in-memory dataset, read-only SELECTs, and warmed queries, which may lead to overfitting. Others raised reliability concerns, such as the LLM hallucinating and missing an index when a variable name changes, and suggested that AlphaGo-style neural heuristics might be a better direction than a blunt LLM approach.

**Tags**: `#LLM`, `#query optimization`, `#database`, `#machine learning`, `#performance`

---

<a id="item-13"></a>
## [Small Programming Tricks: Habits and AI Insights](https://will-keleher.com/posts/small-programming-tricks-matter/) ⭐️ 7.0/10

A blog post shares a collection of small programming and command-line tricks, sparking a lively discussion about habit formation and learning from AI-assisted workflows. The post has gained 362 points and 177 comments on Hacker News. This matters because it shows that even experienced developers often overlook simple shortcuts, and that AI can serve as a powerful teacher for discovering new techniques. The discussion highlights practical ways to boost productivity and encourages continuous learning in the developer community. The post covers command-line and SQL tricks, and commenters note that the real challenge is adopting new habits rather than just knowing the tricks. Some suggest that manually approving every command an AI runs can reveal novel uses of tools like \`perf\`.

hackernews · signa11 · Sep 16, 15:56 · [Discussion](https://news.ycombinator.com/item?id=49729000)

**Background**: Programming tricks are small efficiency hacks that can save time and reduce friction in daily workflows, but they often require deliberate practice to become habits. The discussion also touches on how AI-assisted workflows, where users observe AI&\#x27;s command choices, can serve as a learning opportunity for discovering lesser-known tool capabilities.

**Discussion**: Commenters shared mixed but generally positive views: phforms emphasized the difficulty of forming new habits, kccqzy recommended learning tricks by watching AI&\#x27;s commands, ozim noted that most people use computers inefficiently, GNOMES shared a directory navigation trick, and gnoack recommended O&\#x27;Reilly resources. The overall sentiment is that these tricks are useful but require conscious effort to adopt.

**Tags**: `#programming`, `#command-line`, `#productivity`, `#tips`, `#hackernews`

---

<a id="item-14"></a>
## [BYD&\#x27;s Formula S EV undercuts Tesla Model 3 at under $29,000](https://electrek.co/2026/09/16/byd-undercuts-tesla-new-formula-s-ev-starting-29000/) ⭐️ 7.0/10

BYD launched its new Formula S electric sedan under its Fang Cheng Bao brand, starting at under $29,000, making it cheaper than a Tesla Model 3. The Formula S series includes the brand&\#x27;s first sedan and a GT variant. This signals intensifying price competition in the EV market, as BYD continues to undercut Tesla on price. It could pressure Tesla to introduce more affordable models, especially in markets where BYD expands. The Formula S is only sold in China currently, and if it were sold in Western markets, the price could be significantly higher. The Fang Cheng Bao brand was launched in 2023 as BYD&\#x27;s off-road and personalization sub-brand, and the Formula S represents its first sedan.

rss · r/electricvehicles · Electrek · Sep 16, 16:58 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1wi4yy4/byd_undercuts_the_tesla_model_3_with_its_new/)

**Background**: Fang Cheng Bao is BYD&\#x27;s sub-brand introduced in June 2023, initially focused on rugged body-on-frame plug-in hybrid SUVs like the Bao 5 and Bao 8. The brand has since expanded with the Formula sub-range, including the Formula X supercar and now the Formula S sedan, marking its entry into the sedan segment. BYD uses multiple sub-brands to target different market segments and price points.

<details><summary>References</summary>
<ul>
<li><a href="https://www.techtimes.com/articles/325153/20260820/byds-fang-cheng-bao-formula-s-undercuts-porsche-96000-blade-battery-makes-it-possible.htm">BYD &#x27; s Fang Cheng Bao Formula S Undercuts Porsche by $96,000...</a></li>
<li><a href="https://www.yankodesign.com/2026/05/17/byds-boxy-off-road-brand-just-built-an-anti-minimalist-1000-hp-supercar/">BYD ’ s Boxy Off-Road Brand Just Built an... - Yanko Design</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the Formula S is only sold in China, and if it were sold in the West, it would likely cost around $90,000. Some questioned the need for another sub-brand, while others hoped that competition from other automakers would push Tesla to produce cheaper cars, as Tesla currently has no incentive to lower prices due to lack of competition for the Model Y.

**Tags**: `#EV`, `#BYD`, `#Tesla`, `#Automotive`, `#Pricing`

---

<a id="item-15"></a>
## [Anthropic Merges Claude Cowork and Chat into One Unified Claude](https://simonwillison.net/2026/Sep/16/one-claude/) ⭐️ 7.0/10

Anthropic is merging Claude Cowork and chat into a single unified Claude product, rolling out first to Pro and Max plans across web, desktop, and mobile apps over the coming weeks. The unified Claude will decide whether a request needs a quick answer or a full multi-step task. This signals Anthropic&\#x27;s strategic shift toward a general-purpose agent, where Claude handles tasks end-to-end rather than being split across separate product surfaces. It mirrors OpenAI&\#x27;s recent renaming of its Codex desktop app to ChatGPT, indicating a broader industry trend toward unified agentic interfaces. The merge is rolling out gradually to Pro and Max plans first, with more plans to follow, according to Anthropic&\#x27;s help center. Simon Willison notes that while the unification reduces confusion between Cowork and regular Claude, understanding the actual feature boundaries and surfaces of the new unified product will still require significant work.

rss · Simon Willison · Sep 16, 18:09

**Background**: Claude Cowork was a research preview feature from Anthropic that brought agentic AI capabilities to the Claude Desktop application, allowing users to hand off multi-step tasks that Claude completes from start to finish. Claude Code, by contrast, is Anthropic&\#x27;s agentic coding tool for developers that runs in the terminal, IDE, desktop app, and browser. The unification of Cowork and chat into one Claude represents a consolidation of Anthropic&\#x27;s agentic offerings, though Claude Code remains a separate developer-focused product.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/cowork">Claude Cowork | Claude by Anthropic</a></li>
<li><a href="https://support.claude.com/en/articles/13345190-get-started-with-claude-cowork">Get started with Claude Cowork | Claude Help Center</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>

</ul>
</details>

**Discussion**: No community discussion was provided with this news item, though it was shared via Hacker News.

**Tags**: `#AI`, `#Anthropic`, `#Claude`, `#Product Update`, `#Agents`

---

<a id="item-16"></a>
## [Suleyman Warns Against Granting AI Models Rights](https://simonwillison.net/2026/Sep/16/mustafa-suleyman/) ⭐️ 7.0/10

Mustafa Suleyman, a prominent AI leader, published a warning arguing that treating AI models as having feelings, preferences, or rights is not justified by evidence and would make the AI containment and alignment challenge harder. He explicitly states that consciousness is the foundation of our ethical, legal, and political systems. This perspective from a co-founder of DeepMind and current Microsoft executive adds significant weight to the ongoing debate about model welfare, potentially influencing industry practices and research priorities. It challenges the emerging movement that advocates for considering the moral status of AI systems, and could shape how companies approach AI safety and ethics. The quote comes from Suleyman&\#x27;s essay titled &quot;A warning about &\#x27;model welfare&\#x27;&quot; published on his personal website. He argues that inviting another entity to share any flavor of rights is not justified by evidence, and emphasizes that doing so will complicate the already difficult tasks of AI containment and alignment.

rss · Simon Willison · Sep 16, 16:00

**Background**: AI alignment is the field of research focused on steering AI systems toward human goals, values, and ethical principles, while AI containment refers to technical measures that prevent powerful AI systems from performing dangerous actions or interacting harmfully with the external environment. Model welfare is a research area, notably explored by Anthropic since April 2025, that investigates whether advanced AI systems might have morally relevant experiences such as suffering or wellbeing. Suleyman&\#x27;s stance represents a cautious counterpoint to those who argue for extending moral consideration to AI models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_alignment">AI alignment - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/research/exploring-model-welfare">Exploring model welfare \ Anthropic</a></li>
<li><a href="https://aidive.org/en/glossary/ethics-safety/ai-containment">AI Containment : meaning and practical use | AIDive</a></li>

</ul>
</details>

**Tags**: `#AI ethics`, `#model welfare`, `#AI alignment`, `#generative AI`, `#LLMs`

---

<a id="item-17"></a>
## [Apple Reportedly Planning M8 AI Servers with Nvidia Networking](https://www.macrumors.com/2026/09/16/apple-may-return-to-server-market/) ⭐️ 7.0/10

Apple is reportedly considering re-entering the server market with an AI server built around its future M8 chips, incorporating Nvidia&\#x27;s NVLink Fusion networking, with a potential 2029 release. The system would target companies running AI inference workloads on their own equipment. This marks Apple&\#x27;s potential return to the server business after discontinuing Xserve in 2011, signaling a push into AI infrastructure. It also suggests a possible collaboration between Apple and Nvidia despite historical tensions, which could reshape the AI hardware landscape. According to The Information, the arrangement is not finalized and could be canceled before 2029. The server would use M8 chips and Nvidia&\#x27;s NVLink Fusion for inter-chip communication, with a focus on inference rather than training.

reddit · r/LocalLLaMA · gappyvalley · Sep 16, 14:07 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1why9ao/apple_may_return_to_server_market_with_nvidia/)

**Background**: NVLink Fusion is Nvidia&\#x27;s program and silicon technology that opens its proprietary NVLink high-speed interconnect to third-party chips, allowing partners to connect their own CPUs and custom accelerators to Nvidia GPUs. Apple&\#x27;s M8 is an anticipated future generation of its custom silicon, expected to follow the M-series line. Apple previously sold servers with the Xserve line but discontinued it in 2011. The AI inference market is growing as companies seek to run trained models on their own hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://aiwiki.ai/wiki/nvlink_fusion">NVLink Fusion | AI Wiki</a></li>
<li><a href="https://www.linkedin.com/pulse/interconnect-computer-why-nvidias-nvlink-fusion-most-trojan-kannan-yoiec">The Interconnect Is the Computer: Why Nvidia ’s NVLink Fusion is the...</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed. One commenter recalls historical tensions between Apple and Nvidia over overheating issues in early unibody MacBooks, questioning whether financial incentives have overcome that rift. Another expresses deep skepticism, citing Apple&\#x27;s past discontinuation of Xserve and the Mac Pro &\#x27;trash can&\#x27; era, and stresses that long-term support and commitment are critical in server markets.

**Tags**: `#Apple`, `#Nvidia`, `#AI servers`, `#hardware`, `#inference`

---

<a id="item-18"></a>
## [Meta&\#x27;s Muse Spark weights still unreleased, Reddit criticizes broken promise](https://i.redd.it/9ka4k65h6uph1.png) ⭐️ 7.0/10

Over a month after Meta promised on August 10 to release the weights for its Muse Spark model, the weights remain unavailable, with the model now at version 1.3. A Reddit post highlights this delay and questions Meta&\#x27;s commitment to open weights. This matters because open weights are central to the open-source AI competition, especially against Chinese models that are typically released with open weights. Meta&\#x27;s delay undermines trust in its promises and contradicts its own stated urgency about not delaying model releases due to competition with China. The post notes the irony of Mark Zuckerberg&\#x27;s earlier statement that model releases should not be delayed &\#x27;even a month&\#x27; due to China competition, yet the weights have been withheld for over a month. It also questions whether Meta will release the 1.2 weights or the then-current version, and notes that no explanation has been provided.

reddit · r/LocalLLaMA · RishiFurfox · Sep 16, 07:46 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1whqm2c/hey_meta_wheres_those_muse_spark_weights/)

**Background**: Muse Spark is a large language model developed by Meta Superintelligence Labs, introduced in April 2026 and launched as version 1.1 on July 9, 2026. Open weights refer to the publicly released learned parameters of a trained AI model, allowing others to download and use it; Chinese companies like DeepSeek and Alibaba Cloud commonly release open weights, while many US labs favor proprietary models. The debate over open weights is tied to an AI arms race between the US and China.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Muse_Spark">Muse Spark - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Open_weights">Open weights</a></li>
<li><a href="https://ai.meta.com/blog/introducing-muse-spark-msl/">Introducing Muse Spark: Scaling Towards Personal Superintelligence</a></li>

</ul>
</details>

**Discussion**: Community comments express distrust in Mark Zuckerberg and Alexandr Wang, with one user saying they have no trust in them. Another comment points out that Grok has only open-sourced versions 1 and 2 despite being at 4.6, implying Meta may follow a similar pattern. A third comment jokes that the wait time is infinite, referencing Meta&\#x27;s logo.

**Tags**: `#Meta`, `#Muse Spark`, `#open weights`, `#AI community`, `#open-source`

---

<a id="item-19"></a>
## [Qwen3.8 Max \(0902\) tops China AI leaderboard with 45 score](https://www.reddit.com/r/LocalLLaMA/comments/1wi0dme/qwen38_max_0902_scores_45_on_the_artificial/) ⭐️ 7.0/10

Qwen3.8 Max \(0902\) scored 45 on the Artificial Analysis Intelligence Index, a 5-point improvement in a month, reclaiming the top spot on China&\#x27;s leaderboard ahead of GLM-5.3 \(44.9\) and Kimi K3 \(43.8\). This benchmark result signals intense competition among Chinese AI labs, with Qwen regaining leadership. The score improvement highlights rapid iteration cycles, though community concerns about pricing, speed, and open weights may affect adoption. The model is a 2.4-trillion-parameter Mixture-of-Experts \(MoE\) architecture, updated within 30 days. Despite the high score, it faces criticism for being expensive per task, slow inference, and lacking open weights, while the smaller Qwen3.8-Flash-Next scored 40 with better speed.

reddit · r/LocalLLaMA · UmpireBorn3719 · Sep 16, 15:26

**Background**: The Artificial Analysis Intelligence Index is a weighted average of production benchmark scores, scaled from 0 to 100, primarily text-based and in English. Mixture of Experts \(MoE\) is an architecture that activates only relevant sub-networks \(experts\) per token, enabling massive scale with lower compute than dense models. This context helps understand why the 2.4T MoE model can achieve high scores but may have trade-offs in speed and cost.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index v4.3 | Artificial Analysis</a></li>
<li><a href="https://researchaudio.io/p/mixture-of-experts-moe-in-large-language-models">Mixture of Experts ( MoE ) in Large Language Models</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: while some praise the benchmark improvement and the efficiency of the smaller Flash-Next variant, others criticize the high pricing, slow per-task latency, lack of open weights, and knowledge gaps in areas like physics. These concerns temper enthusiasm despite the top ranking.

**Tags**: `#AI models`, `#benchmarks`, `#Qwen`, `#LLM leaderboard`, `#China AI`

---

<a id="item-20"></a>
## [Qwen 3.5 4B with logits rivals TypeSafe&\#x27;s Jev model](https://www.reddit.com/r/LocalLLaMA/comments/1whzy7j/qwen35_4b_grabbing_logits_is_almost_jev_or_even/) ⭐️ 7.0/10

A Reddit user demonstrated that a small Qwen 3.5 4B model, by simply assigning each choice to a letter and reading the logit probabilities, can replicate or even outperform TypeSafe AI&\#x27;s new Jev &quot;System One Model&quot; which outputs calibrated probabilities for given choices. The implementation is open-sourced on GitHub \(openjev\) with a browser demo at openjev.com. This challenges the value proposition of dedicated &quot;System One&quot; probability-output models, suggesting that a small open-source model with logit extraction can achieve comparable or better results at a fraction of the cost. It could affect how developers approach probabilistic classification and choice-probability tasks in LLM applications. The approach assigns each option a letter token and reads the logit probabilities for those tokens rather than generating text. A community commenter noted the importance of comparing calibration \(whether confidence bins match observed correctness after temperature scaling\), not just accuracy, since rerankers can order choices well while producing overly sharp probabilities.

reddit · r/LocalLLaMA · theoleecj\_n · Sep 16, 15:10

**Background**: Logits are the raw, unnormalized outputs of a neural network&\#x27;s final layer, which are typically converted to probabilities via a softmax function. Reranker models are specialized AI systems used in information retrieval to re-order candidate documents by relevance. TypeSafe AI&\#x27;s Jev is a &quot;System One Model&quot; that returns typed decisions with calibrated probabilities instead of text, running 40-200x faster than frontier LLMs.

<details><summary>References</summary>
<ul>
<li><a href="https://typesafe.ai/">Home - TypeSafe AI</a></li>
<li><a href="https://docs.typesafe.ai/concepts/system-one">System One - TypeSafe AI</a></li>
<li><a href="https://stackoverflow.com/questions/41455101/what-is-the-meaning-of-the-word-logits-in-tensorflow">machine learning - What is the meaning of the word logits in ... Usage example</a></li>

</ul>
</details>

**Discussion**: Community reaction was largely positive and amused, with one commenter joking that &quot;there goes that seed funding round.&quot; Another user confirmed the Hugging Face version works. A substantive concern was raised about calibration: comparing confidence bins against observed correctness after temperature scaling, since rerankers may produce overly sharp probabilities even when ordering is accurate.

**Tags**: `#LLM`, `#logits`, `#Qwen`, `#reranker`, `#probabilistic-classification`

---

<a id="item-21"></a>
## [Qwen3.8 Flash Hits 15 tok/s on 12GB VRAM with Aggressive Quantization](https://www.reddit.com/r/LocalLLaMA/comments/1wi46on/qwen38_flash_on_12gb_vram_15_tokenss/) ⭐️ 7.0/10

A user reports running Qwen3.8-Flash-Next on a 12GB RTX 5070 SFF GPU at a steady 15 tokens/s output and 100-120 tokens/s prompt processing, using a 3 bpw IQ3\_XXS GGUF quantization with aggressive offloading to RAM and SSD. The setup achieved up to 128K context length in testing. This demonstrates that large frontier-class models can run at usable speeds on consumer hardware with limited VRAM, expanding what is practical for local LLM practitioners. The techniques shown — aggressive quantization combined with RAM/SSD offloading — offer a blueprint for running models that would otherwise require far more expensive hardware. The full GGUF is around 76GB, but only 47GB needs to be sharded across VRAM and RAM, with the remainder served from SSD. The user reports output quality matching Unsloth&\#x27;s Q6-Q8 level on their tests, with generation speeds ranging from 11.3 tok/s at 90-100K context to 14.6 tok/s at 8K, and plans to test a 2.40 bpw version next.

reddit · r/LocalLLaMA · KnownAd4832 · Sep 16, 17:41

**Background**: GGUF is a binary file format that packages model weights, tokenizer data, architecture metadata, and quantization information into a single portable file for inference with GGML-based runtimes like llama.cpp. Quantization reduces model precision \(e.g., IQ3\_XXS at roughly 3 bits per weight\) to shrink memory footprint at some cost to output quality. FreeToken is a local LLM runtime that brings datacenter-scale model serving to desktop machines, and the user used its CLI with llama for this benchmark.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/FlashML-org/FreeToken/blob/main/docs/cli.md">FreeToken/docs/cli.md at main · FlashML-org/FreeToken</a></li>
<li><a href="https://www.datacamp.com/tutorial/gguf-format-a-complete-guide">GGUF Format: A Complete Guide to Local LLM Inference</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/discussions/5063">Even more quantization types? · ggml-org llama.cpp · Discussion #5063</a></li>

</ul>
</details>

**Discussion**: Community members shared similar results and offered alternative approaches. One user reported achieving over 22 tok/s with a 91K context window on an RTX 5070 Ti 12GB using their own &\#x27;flyweight&\#x27; engine, while another noted that a 12GB card plus fast multi-channel RAM can run the model at full 262K context at 13-20 tok/s on a 5090 + 3060 setup. Another user said they were testing it as well and would share results later.

**Tags**: `#LocalLLM`, `#Qwen3.8`, `#VRAM optimization`, `#GGUF quantization`, `#Inference performance`

---

<a id="item-22"></a>
## [Git Worktree Gotchas: Common Pitfalls and Best Practices](https://www.olafalders.com/2026/09/16/git-worktree-gotchas/) ⭐️ 7.0/10

The blog post highlights common gotchas developers encounter when using git worktrees and offers practical solutions, sparking community discussion on best practices such as using bare repositories and handling real-world migration scenarios. Git worktrees are a powerful but often misunderstood feature that can significantly improve developer productivity by enabling parallel work on multiple branches. Understanding the pitfalls helps teams avoid data loss and workflow disruptions, especially in large-scale repository migrations. The post covers issues like the &\#x27;main working tree&\#x27; concept, path confusion, and the risk of accidentally deleting a worktree and losing the repository. The community recommends creating a bare repository and forking worktrees off of it, using \`git rev-parse --git-common-dir\` to locate the common repository shared by all worktrees.

reddit · r/programming · oalders · Sep 16, 15:46 · [Discussion](https://www.reddit.com/r/programming/comments/1wi0xi2/git_worktree_gotchas/)

**Background**: Git worktree is a feature that allows multiple working directories to be associated with the same repository, enabling developers to work on different branches simultaneously without stashing changes or switching contexts. This is particularly useful for teams maintaining multiple active release branches, as it avoids the overhead of repeated checkouts and large repository clones. The feature was introduced in Git 2.5 and has become a standard tool for parallel development workflows.

<details><summary>References</summary>
<ul>
<li><a href="https://git-scm.com/docs/git-worktree">Git - git - worktree Documentation</a></li>
<li><a href="https://dev.to/yankee/practical-guide-to-git-worktree-58o0">Practical Guide to Git Worktree - DEV Community</a></li>
<li><a href="https://grokipedia.com/page/Git_worktree">Git worktree</a></li>

</ul>
</details>

**Discussion**: The community discussion is largely positive, with masklinn arguing that having a &\#x27;main working tree&\#x27; is bad practice and recommending bare repositories instead, noting that \`git rev-parse --git-common-dir\` then works as expected. mb862 shares a real-world scenario of migrating a 15-year-old SVN repository with a 60-70 GB checkout, highlighting practical challenges in large-scale migrations where developers maintain multiple active release branches.

**Tags**: `#git`, `#worktree`, `#version control`, `#best practices`, `#development tools`

---

<a id="item-23"></a>
## [Hungary intensifies pressure on BYD and CATL over violations](https://www.electrive.com/2026/09/16/hungary-increases-pressure-on-byd-and-catl/) ⭐️ 7.0/10

Hungary is increasing regulatory pressure on Chinese EV and battery makers BYD and CATL over labor violations, environmental hazards, and political controversies at their new plants. Reports cite 14-hour workdays at BYD&\#x27;s construction site and elevated nickel exposure among CATL employees in Debrecen. This scrutiny highlights growing regulatory and ethical challenges for Chinese battery and EV manufacturers expanding into Europe. It could affect their reputations, operational costs, and the broader push for higher labor and environmental standards in the industry. The article notes that China Labor Watch reported working hours up to 14 hours a day, seven days a week at the BYD plant construction site. It also mentions the politically sensitive move of former Hungarian Foreign Minister Péter Szijjártó to BYD, and that CATL&\#x27;s Debrecen plant had nine employees with elevated nickel exposure, with authorities criticizing protective equipment.

reddit · r/electricvehicles · EconomyStrawberry162 · Sep 16, 14:08 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1whyadv/hungary_increases_pressure_on_byd_and_catl/)

**Background**: Lithium-ion batteries, used in EVs, contain separators—microporous polymer films that prevent short circuits while allowing ion flow—and cathodes often use nickel to increase energy density. Hungary has become a major hub for EV battery manufacturing, attracting investments from Chinese companies like CATL and BYD, but these investments have raised concerns about labor conditions and environmental impact.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Separator_%28electricity%29">Separator (electricity) - Wikipedia</a></li>
<li><a href="https://www.innovationnewsnetwork.com/the-role-of-nickel-in-ev-battery-manufacturing/38877/">The role of nickel in EV battery manufacturing</a></li>

</ul>
</details>

**Discussion**: Community comments express strong criticism of the reported labor conditions, with one user stating they would rather be &\#x27;behind&\#x27; than work 14-hour days. Another comment links the low prices of Chinese cars to such labor practices, questioning whether consumers want to support that model. Overall sentiment is negative toward the working conditions described.

**Tags**: `#EV`, `#battery`, `#labor rights`, `#regulation`, `#China`

---

<a id="item-24"></a>
## [AI Voice Cloning: Treat Voice Samples as Sensitive Data](https://www.reddit.com/r/artificial/comments/1whwugr/ai_voice_cloning_think_twice_before_sending_that/) ⭐️ 7.0/10

A Reddit post warns that submitting clean voice samples for AI voice-cloning jobs, along with personal details like name, phone, and email, poses a serious identity theft and fraud risk. It cites a reported scam call that mimicked a spouse&\#x27;s voice to request credit card information. Voice samples are becoming a form of biometric identity that AI can clone and misuse, making them as sensitive as passwords. This affects anyone who shares voice recordings online, from voice actors to ordinary users of voice-enabled apps. The post emphasizes that a clean voice sample combined with personal information can enable fraud, though the cited scam call could not be independently verified. It suggests treating clean voice samples as sensitive data, similar to passwords or financial information.

reddit · r/artificial · Admirable\_Wasabi\_732 · Sep 16, 13:11

**Background**: AI voice cloning uses neural networks and text-to-speech technology to replicate a person&\#x27;s unique voice characteristics from short audio samples. Voice biometrics systems use these acoustic features for authentication, while deepfake audio can synthesize speech that mimics specific individuals, often used in scams and phishing. As these technologies advance, even brief voice recordings can become powerful tools for identity fraud.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Voice_biometrics">Voice biometrics</a></li>
<li><a href="https://en.wikipedia.org/wiki/Deepfake_audio_detection">Deepfake audio detection</a></li>
<li><a href="https://finevoice.ai/ai-voice-cloning">Free AI Voice Cloning : Clone Any Voice in Seconds</a></li>

</ul>
</details>

**Discussion**: Commenters expressed growing paranoia about answering unknown calls, fearing scammers record voices. One user compared a clean voice sample tied to real identity to an unresetable password, while another worried about voice upload options in companion apps for roleplay chats.

**Tags**: `#AI voice cloning`, `#security`, `#privacy`, `#scams`, `#identity theft`

---

<a id="item-25"></a>
## [Google&\#x27;s Vectorized Performance-Portable Quicksort Using SIMD](https://opensource.googleblog.com/2022/06/Vectorized%20and%20performance%20portable%20Quicksort.html) ⭐️ 6.0/10

Google published a 2022 article detailing a vectorized, performance-portable quicksort that uses SIMD compress-store instructions \(available in Arm SVE, RISC-V V, and x86 AVX-512\) for branchless, efficient partitioning. Sorting is a fundamental operation across databases, analytics, and general computing, so demonstrating how modern SIMD instructions can accelerate quicksort has broad performance implications. The approach also highlights the value of performance portability across different CPU architectures. The core innovation is the compress-store instruction, which writes only elements matching a yes/no mask \(e.g., less than the pivot\) to consecutive memory, enabling branchless partitioning that avoids branch mispredictions. The article dates to 2022, and commenters note that newer algorithms such as driftsort and ipnsort have since surpassed it.

hackernews · mococa · Sep 16, 18:31 · [Discussion](https://news.ycombinator.com/item?id=49731054)

**Background**: Quicksort is a divide-and-conquer sorting algorithm that partitions an array around a pivot. Traditional partitioning uses conditional branches that can cause expensive branch mispredictions on random data. SIMD \(Single Instruction Multiple Data\) lets a CPU process multiple elements with one instruction, and modern instruction sets \(AVX-512, Arm SVE, RISC-V V\) include compress-store instructions that enable branchless partitioning.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=42892513">I suspect if you started using SIMD instructions , the... | Hacker News</a></li>
<li><a href="https://patents.google.com/patent/US9672036B2/en">US9672036B2 - Instruction and logic to provide... - Google Patents</a></li>

</ul>
</details>

**Discussion**: Commenters pointed out the article is from 2022 and outdated, noting that driftsort and ipnsort are now state-of-the-art \(one commenter integrated them into ClickHouse\). Others made lighthearted remarks about quicksort&\#x27;s naming and requested a \(2022\) tag in the title for clarity.

**Tags**: `#quicksort`, `#vectorization`, `#SIMD`, `#performance`, `#algorithms`

---

<a id="item-26"></a>
## [LARA: Low-Rank Residual Adapters for Frozen LLMs](https://i.redd.it/xrngwyo6wvph1.png) ⭐️ 6.0/10

LARA trains low-rank residual adapters in the residual stream of frozen language models, enabling behaviors that can be loaded, removed, blended, or routed at inference time. The project provides a PyTorch library, a Mixture of Behaviors demo, and comparisons with LoRA. This offers a modular post-training approach that lets a single frozen model host multiple independently trained behaviors without keeping separate adapted models. It could reduce storage overhead and enable dynamic behavior routing, aligning with the trend toward modular and composable LLMs. LARA operates in the residual stream rather than modifying weight matrices, unlike LoRA which adds low-rank updates to weights. The repository includes writing-style behaviors trained on Hemingway, Fitzgerald, and Gertrude Stein, along with reproduction instructions for the paper.

reddit · r/MachineLearning · kertara · Sep 16, 13:28 · [Discussion](https://www.reddit.com/r/MachineLearning/comments/1whx9tr/lara_small_composable_behaviours_for_frozen_llms_p/)

**Background**: Large language models are typically fine-tuned to adapt to specific tasks, but this modifies weights and requires separate copies. Parameter-efficient methods like LoRA learn low-rank weight updates, while LARA instead adds lightweight residual adapters to the residual stream of a frozen model. This allows behaviors to be composed and routed at inference time, similar to mixture-of-experts concepts but with adapters.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/papers/2607.28669">Paper page - LARA : Lightweight Adapters in the Residual Stream for...</a></li>
<li><a href="https://sanowl.github.io/lora.html">LoRA: Low ‑ Rank Adaptation for Efficient Fine‑Tuning</a></li>

</ul>
</details>

**Discussion**: The top comment questions originality, suggesting overlap with ReFT \(Representation Fine-Tuning\) and calling it potential plagiarism. Another comment notes that modifying weights \(as LoRA does\) allows direct application without special inference machinery, whereas LARA&\#x27;s adapters may require extra routing logic.

**Tags**: `#LLM`, `#adapters`, `#post-training`, `#modularity`, `#research`

---

<a id="item-27"></a>
## [Qwen 3.8 27B Runs 63 Hours on RTX 3090 Attempting Riemann Hypothesis](https://www.reddit.com/r/LocalLLaMA/comments/1wi9fau/qwen_38_27b_running_for_63_hours_on_a_rtx_3090_to/) ⭐️ 6.0/10

An enthusiast ran a 4-bit quantized Qwen 3.8 27B model with a 100K context window autonomously for 63 hours \(over 50 million tokens\) attempting to solve the Riemann hypothesis. The model unsurprisingly failed to prove the conjecture, but the experiment&\#x27;s logs, internal memories, and strategies were published on Hugging Face. This experiment showcases the emerging capability of long-running autonomous LLM agents tackling open mathematical problems, a trend that could reshape how research is conducted. It also highlights both the promise \(self-correction, persistent effort\) and the practical limits \(compute cost, verification challenges\) of using open-source models for frontier mathematics. The model was 4-bit quantized and ran with a 100K token context window on a single RTX 3090, consuming over 50 million tokens. The author claims the model never hallucinated a final answer and repeatedly corrected its own mistakes, though no rigorous verification of these claims was provided.

reddit · r/LocalLLaMA · GuiltyBookkeeper4849 · Sep 16, 20:50

**Background**: The Riemann hypothesis is one of the seven Millennium Prize Problems, a conjecture about the distribution of the zeros of the Riemann zeta function, with a $1 million prize for a proof. Quantization reduces model size by lowering weight precision \(e.g., 4-bit\), making large models feasible on consumer GPUs like the RTX 3090, while a 100K context window allows the model to retain much more information across a long session. This experiment sits at the intersection of local LLM deployment, autonomous agent research, and mathematical exploration.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://medium.com/@sobhindas/running-a-4-bit-quantized-llm-locally-with-llama-cpp-7a979d2eb5a3">Running a 4 - Bit Quantized LLM Locally with llama.cpp | Medium</a></li>
<li><a href="https://llmconfigurator.com/en/guides/context-window-guide">Context Window Guide 2026: 4K vs 32K vs 128K Tokens | Local AI Guide | LLM Configurator</a></li>

</ul>
</details>

**Discussion**: Commenters raised valid concerns: one questioned whether the author has enough number theory expertise to actually detect hallucinations or mistakes in the model&\#x27;s mathematical reasoning, while another asked for details on the harness and context management. A third commenter noted the enormous compute cost involved, citing that OpenAI reportedly spent £15 million on compute for the Navier-Stokes millennium proof.

**Tags**: `#LLM`, `#Riemann Hypothesis`, `#Local LLM`, `#AI Experiment`, `#Qwen`

---