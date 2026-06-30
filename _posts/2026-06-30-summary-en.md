---
layout: default
title: "Horizon Summary: 2026-06-30 (EN)"
date: 2026-06-30
lang: en
---

> From 22 items, 14 important content pieces were selected

---

1. [Supreme Court: Geofence Warrants Need Constitutional Protections](#item-1) ⭐️ 9.0/10
2. [Google's AI Peer-Reviewer Handles 10K Papers, Catches 34% More Errors](#item-2) ⭐️ 9.0/10
3. [Rocket Lab acquires Iridium in historic deal](#item-3) ⭐️ 8.0/10
4. [WATaBoy: JIT Compiling Game Boy to WASM Outperforms Native Interpreter](#item-4) ⭐️ 8.0/10
5. [Inside a CUDA Kernel Launch: CPU to GPU Path](#item-5) ⭐️ 8.0/10
6. [Ornith-1.0: Open-Weight Self-Scaffolding Coding LLM](#item-6) ⭐️ 8.0/10
7. [EML Trees Proven Universal Approximators](#item-7) ⭐️ 8.0/10
8. [HEMA Practitioner Builds Open Dataset for AI Swordfighting Tracking](#item-8) ⭐️ 8.0/10
9. [Proposed .self TLD Aims to Boost Self-Hosting](#item-9) ⭐️ 7.0/10
10. [Qwen 3.6 27B: Sweet Spot for Local Dev?](#item-10) ⭐️ 7.0/10
11. [Cerebras-OpenAI Deal Crowds Out Smaller AI Startups](#item-11) ⭐️ 7.0/10
12. [Quiz Reveals LLM Personalities and Values Across 15 Models](#item-12) ⭐️ 7.0/10
13. [Why NCE Over Direct Denominator Approximation in Representation Learning?](#item-13) ⭐️ 6.0/10
14. [Reddit User Asks About Recursive Self-Improvement PhD](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Supreme Court: Geofence Warrants Need Constitutional Protections](https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision) ⭐️ 9.0/10

The US Supreme Court ruled that geofence warrants, which compel tech companies to provide location data of devices within a virtual boundary, must comply with Fourth Amendment protections against unreasonable searches and seizures. This landmark decision significantly limits law enforcement's ability to conduct mass location surveillance without individualized suspicion, setting a crucial precedent for digital privacy in the era of ubiquitous data collection. The case involved a bank robbery where police obtained location data of 19 Google accounts near the crime scene; the Court held that such warrants require probable cause and particularity, akin to traditional search warrants.

hackernews · cdrnsf · Jun 29, 15:54 · [Discussion](https://news.ycombinator.com/item?id=48720924)

**Background**: Geofence warrants allow police to demand location data from companies like Google for all devices within a defined area during a specific time window. The Fourth Amendment protects against unreasonable searches, but its application to digital location data has been debated, especially after the 2018 Carpenter v. United States decision.

<details><summary>References</summary>
<ul>
<li><a href="https://www.brennancenter.org/our-work/policy-solutions/fourth-amendment-digital-age">The Fourth Amendment in the Digital Age | Brennan Center for Justice</a></li>

</ul>
</details>

**Discussion**: Commenters largely welcomed the ruling as a win for privacy, with some noting historical examples like the Petraeus affair to illustrate alternative identification methods. Others raised questions about implications for automated license plate readers and similar surveillance technologies.

**Tags**: `#privacy`, `#law`, `#surveillance`, `#supreme court`, `#geofence`

---

<a id="item-2"></a>
## [Google's AI Peer-Reviewer Handles 10K Papers, Catches 34% More Errors](https://www.reddit.com/r/MachineLearning/comments/1uio9rb/googles_agentic_peerreviewer_handled_10k_papers/) ⭐️ 9.0/10

Google deployed an agentic AI peer-reviewer at ICML and STOC that processed approximately 10,000 papers with a 30-minute turnaround, and a formal research paper shows it catches 34% more mathematical errors than zero-shot prompting. This sets a precedent for AI-automated scientific review at conference scale, potentially accelerating the peer-review process and reducing reviewer burden while improving error detection. The agentic system uses a multi-step reasoning approach rather than simple zero-shot prompting, enabling it to catch subtle mathematical errors. The formal paper is available on arXiv (2606.28277).

reddit · r/MachineLearning · /u/Justgototheeffinmoon · Jun 29, 10:05

**Background**: Peer review is a cornerstone of scientific publishing, but it is often slow and inconsistent. Agentic AI systems use iterative reasoning and tool use to perform complex tasks, unlike zero-shot prompting which asks a model to answer without examples. Google's system demonstrates that such agents can be applied to large-scale conference review.

<details><summary>References</summary>
<ul>
<li><a href="https://paperreview.ai/tech-overview">Tech Overview - Stanford Agentic Reviewer</a></li>
<li><a href="https://www.promptingguide.ai/techniques/zeroshot">Zero-Shot Prompting | Prompt Engineering Guide</a></li>

</ul>
</details>

**Discussion**: Reddit commenters expressed excitement about the speed and scale, with some noting that even imperfect AI review can accelerate research by providing rapid feedback. Others raised concerns about fairness and the risk of over-reliance on automated systems.

**Tags**: `#AI`, `#peer review`, `#machine learning`, `#conference`, `#automation`

---

<a id="item-3"></a>
## [Rocket Lab acquires Iridium in historic deal](https://investors.rocketlabcorp.com/news-releases/news-release-details/rocket-lab-acquire-iridium-historic-deal-creating-fully) ⭐️ 8.0/10

Rocket Lab announced its acquisition of Iridium Communications, merging a launch provider with a satellite operator to create a fully integrated space company. This deal creates a vertically integrated space giant, potentially lowering costs and increasing launch cadence by guaranteeing a baseline of launches for Rocket Lab's own constellation, similar to SpaceX's Starlink strategy. Rocket Lab will leverage Iridium's existing satellite network and launch demand, while also adding Iridium constellation replacements to its order book. The acquisition marks a shift from Rocket Lab's New Zealand roots to a U.S.-focused entity.

hackernews · everfrustrated · Jun 29, 14:09 · [Discussion](https://news.ycombinator.com/item?id=48719485)

**Background**: Rocket Lab is an end-to-end space company providing launch services and spacecraft manufacturing, founded in New Zealand by Peter Beck. Iridium operates the world's only truly global satellite network, primarily for mission-essential communications. The deal mirrors SpaceX's strategy of using its Starlink constellation to guarantee a steady launch cadence.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Iridium_satellite_constellation">Iridium satellite constellation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rocket_Lab">Rocket Lab - Wikipedia</a></li>
<li><a href="https://www.rocketlabusa.com/">Rocket Lab | The Space Company | Rocket Lab</a></li>

</ul>
</details>

**Discussion**: Commenters generally view the acquisition as a smart strategic move, comparing it to SpaceX's Starlink model. Some express concerns about space debris and the environmental impact of increasing satellite constellations, while others question the technical feasibility of Rocket Lab's rockets reaching Iridium's orbit.

**Tags**: `#space`, `#acquisition`, `#satellite`, `#Rocket Lab`, `#Iridium`

---

<a id="item-4"></a>
## [WATaBoy: JIT Compiling Game Boy to WASM Outperforms Native Interpreter](https://humphri.es/blog/WATaBoy/) ⭐️ 8.0/10

WATaBoy is a Game Boy emulator that uses just-in-time (JIT) compilation to translate SM83 instructions into WebAssembly (WASM) at runtime, achieving approximately 1.2x the speed of a native interpreter. It cleverly bypasses iOS JIT restrictions by running inside a web browser, leveraging WebKit's JIT support for WebAssembly. This project demonstrates a novel approach to emulation on platforms with JIT restrictions, such as iOS, by using WebAssembly as a compilation target. It also highlights the performance potential of WASM JIT, showing that it can beat native interpreters, which could influence future emulator design and browser-based applications. The emulator's core is written in Rust and compiled to WASM, while the JIT compiler generates WASM bytecode at runtime, linked via JavaScript and indirect function calls. Benchmarks show Safari performs best among browsers, and further optimizations like PPU interrupt prediction are possible.

hackernews · energeticbark · Jun 29, 15:02 · [Discussion](https://news.ycombinator.com/item?id=48720190)

**Background**: Game Boy emulators typically interpret SM83 instructions one by one, which is flexible but slow. JIT compilation translates frequently executed code into native machine code for faster execution, but iOS bans JIT for non-browser apps. WebAssembly, supported by all major browsers, allows JIT compilation within the browser, providing a workaround.

<details><summary>References</summary>
<ul>
<li><a href="https://humphri.es/blog/WATaBoy/">WATaBoy: JIT-ing Game Boy Instructions to Wasm Beats a Native ...</a></li>
<li><a href="https://github.com/sysprog21/jitboy">GitHub - sysprog21/jitboy: A Game Boy emulator with dynamic ... WATaBoy: JIT-Ing Game Boy Instructions to WASM Beats a Native ... A Game Boy emulator with an SM83 to Wasm JIT compiler. - GitHub WATaBoy: Why This WebAssembly JIT is Beating Native Game Boy ... GameRoy: JIT compilation in High-Accuracy Game Boy Emulation WATaBoy: Emulador Game Boy en WebAssembly supera intérprete ...</a></li>
<li><a href="https://hb.int2inf.com/en/s/item/BKFh6K7YDaMaMadWmQwvho-wataboy-jit-wasm-game-boy-emulator">WATaBoy: JIT-Ing Game Boy Instructions to WASM Beats a Native ...</a></li>

</ul>
</details>

**Discussion**: Commenters praised the project as impressive for an undergraduate, with one noting that WASM overhead (~20%) is far less than interpreter overhead (~1000%), making the result unsurprising. Another commenter shared a similar experience using LLVM for Dolphin emulation 16 years ago, and a discussion arose about Firefox being 25% slower than Chrome/Safari.

**Tags**: `#JIT compilation`, `#WebAssembly`, `#emulation`, `#Game Boy`, `#browser performance`

---

<a id="item-5"></a>
## [Inside a CUDA Kernel Launch: CPU to GPU Path](https://fergusfinn.com/blog/what-happens-when-you-run-a-gpu-kernel/) ⭐️ 8.0/10

A detailed blog post by Fergus Finn walks through the entire software and hardware pipeline of a CUDA kernel launch, from the CUDA driver submitting commands to the GPU executing threads. This deep dive helps developers understand the hidden complexity behind a simple kernel launch, enabling better performance optimization and debugging of GPU applications. The post covers the doorbell mechanism, queue management descriptor (QMD), and control codes, which are critical for submitting work to the GPU. Community comments note that control codes are actually a table lookup, not just bits in a control word.

hackernews · mezark · Jun 29, 13:11 · [Discussion](https://news.ycombinator.com/item?id=48718863)

**Background**: CUDA is NVIDIA's parallel computing platform that allows developers to run code on GPUs. Launching a CUDA kernel involves the CPU driver packaging the kernel and arguments into a command buffer, which is then sent to the GPU via a doorbell register. The GPU's work scheduler picks up the command and dispatches thread blocks to streaming multiprocessors.

<details><summary>References</summary>
<ul>
<li><a href="https://ztex.medium.com/nvidia-cuda-compiler-driver-process-cuda-kernel-deployment-from-code-to-gpu-execution-f94fdc41c8fe">NVIDIA CUDA Compiler Driver Process | by ztex, Tony, Liu | Medium</a></li>
<li><a href="https://stackoverflow.com/questions/12172279/how-is-a-cuda-kernel-launched">parallel processing - How is a CUDA kernel launched ?</a></li>
<li><a href="https://docs.nvidia.com/cuda/cuda-c-programming-guide/">CUDA C++ Programming Guide (Legacy) — CUDA C++ Programming...</a></li>

</ul>
</details>

**Discussion**: Commenters appreciated the post for connecting CUDA syntax to actual GPU submission, with praise for the doorbell and QMD explanations. One commenter noted that control codes are more complex than described, involving a table lookup. Another speculated about the future of kernel optimization companies versus open-source solutions.

**Tags**: `#CUDA`, `#GPU`, `#systems programming`, `#NVIDIA`, `#parallel computing`

---

<a id="item-6"></a>
## [Ornith-1.0: Open-Weight Self-Scaffolding Coding LLM](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 8.0/10

DeepReinforce released Ornith-1.0, a family of open-weight (MIT-licensed) LLMs built on Gemma 4 and Qwen 3.5, with sizes from 9B to 397B, achieving state-of-the-art coding benchmark results among open-source models of comparable size. This model introduces self-scaffolding, where the LLM learns to write its own agent harness during reinforcement learning post-training, potentially advancing agentic coding capabilities. Its permissive license and strong performance across sizes make it accessible for both research and practical use. The model family includes 9B Dense, 31B Dense, 35B MoE, and 397B MoE variants, with the 397B MoE matching Claude Opus 4.7 on SWE-Bench. The 9B variant outperforms models three times its size, and the dense 9B fits on a single 80GB GPU.

rss · Simon Willison · Jun 29, 16:17

**Background**: Agentic coding refers to AI agents that autonomously plan, write, test, and modify code with minimal human intervention. Self-scaffolding is a technique where the model learns to generate its own agent framework (e.g., tool-use loops) during training, rather than relying on a fixed external scaffold. Mixture of Experts (MoE) architectures activate only a subset of parameters per token, enabling larger model capacity with lower computational cost.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/29/ornith/">Ornith-1.0: Self-Scaffolding LLMs for Agentic Coding</a></li>
<li><a href="https://www.explainx.ai/blog/ornith-1-0-self-scaffolding-agentic-coding-llm-2026">Ornith-1.0: Self-Scaffolding Open Models for Agentic Coding</a></li>
<li><a href="https://aratech.ae/blog/ornith-1-0-open-source-self-scaffolding-ai-coding-model">Ornith 1.0: Self-Scaffolding Open-Source AI Coding Model | aratech</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some users praise the model's creative coding solutions and recommend it, while others note it performs poorly on chat without tools and exhibits hallucination. There is skepticism about whether it is merely a fine-tuned Qwen or Gemma, and concerns about GPU requirements for larger variants.

**Tags**: `#LLM`, `#open-source`, `#coding`, `#agentic`, `#AI`

---

<a id="item-7"></a>
## [EML Trees Proven Universal Approximators](https://www.reddit.com/r/MachineLearning/comments/1uipl1t/eml_trees_are_universal_approximators_r/) ⭐️ 8.0/10

A new paper proves that EML trees, which are compositions of the elementary function operator EML(x,y)=exp(x)ln(y), are universal approximators for continuous functions and Sobolev spaces. This theoretical result establishes EML trees as a powerful building block for machine learning architectures, potentially enabling new types of neural networks with built-in elementary function representations. The proof constructs EML representations of binary operations, polynomials, and hyperbolic tangent, then uses them as LEGO blocks to approximate any function in W^{k,∞} on (0,1]^d. Technical challenges include handling the natural logarithm's domain restrictions via sign-based decompositions.

reddit · r/MachineLearning · /u/JoeGermany · Jun 29, 11:16

**Background**: The EML function (exp(x)ln(y)) was recently shown to be a universal elementary function, capable of representing all elementary functions through composition. This work extends that idea by proving that tree-structured compositions of EML functions can approximate any continuous function, similar to how neural networks with sigmoid activations are universal approximators.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2606.23179v1">EML Trees Are Universal Approximators - arXiv.org</a></li>
<li><a href="https://arxiv.org/abs/2606.23179">[2606.23179] EML Trees Are Universal Approximators - arXiv.org</a></li>
<li><a href="https://arxiv.org/html/2603.21852v2">All elementary functions from a single operator - arXiv.org</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion highlights the novelty of the proof and its potential impact on ML theory. Commenters note the clever use of LEGO-like block construction and discuss the practical limitations of the domain (0,1]^d and the need for sign-based decompositions.

**Tags**: `#universal approximation`, `#EML trees`, `#machine learning theory`, `#function approximation`

---

<a id="item-8"></a>
## [HEMA Practitioner Builds Open Dataset for AI Swordfighting Tracking](https://www.reddit.com/r/MachineLearning/comments/1uivddx/i_do_historical_swordfighting_and_noticed_ai/) ⭐️ 8.0/10

A historical European martial arts (HEMA) practitioner is creating an open multi-view dataset of swordfighting at 120/240fps to improve AI tracking of fast-moving, occluded objects and human motion, and has posted a proposed schema on Hugging Face for community feedback. This dataset targets the Sim2Real gap and thin-object tracking—two critical bottlenecks in embodied AI—by providing real-world edge cases like high-speed motion blur and heavy occlusion, which could benefit pose estimation, trajectory prediction, and robotic balance systems. The dataset includes 100 hyper-trimmed clips with synchronized multi-view capture, annotated with biomechanics metadata (e.g., guard positions, strike trajectory) and computer vision hazards (occlusion rating, motion blur), plus frame-level 2D keypoints and segmentation masks for swords and fencers.

reddit · r/MachineLearning · /u/fonssagrives · Jun 29, 15:16

**Background**: Historical European martial arts (HEMA) involves reviving medieval combat systems with steel swords. In computer vision, the Sim2Real gap refers to the performance drop when models trained in simulation are deployed in the real world, and thin-object tracking is especially challenging due to motion blur and occlusion. This dataset aims to provide real-world data to bridge that gap.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hemaalliance.com/new-to-hema">New to HEMA? — HEMAA</a></li>
<li><a href="https://xai4debugging.github.io/files/papers/visualizing_the_sim2real_gap_i.pdf">SIM2REALVIZ: Visualizing the Sim2Real Gap in Robot Ego-Pose Estimation</a></li>
<li><a href="https://www.researchgate.net/publication/383100823_Detecting_and_tracking_moving_objects_in_defocus_blur_scenes">Detecting and tracking moving objects in defocus blur scenes</a></li>

</ul>
</details>

**Tags**: `#computer vision`, `#dataset`, `#embodied AI`, `#Sim2Real`, `#motion tracking`

---

<a id="item-9"></a>
## [Proposed .self TLD Aims to Boost Self-Hosting](https://hccf.onmy.cloud/2026/06/21/reclaiming-our-digital-selves-hccfs-vision-for-a-human-centered-top-level-domain/) ⭐️ 7.0/10

A proposal for a new top-level domain (TLD) called .self has been published, designed to support self-hosting by providing free subdomains to individuals. The idea has sparked significant community discussion on its feasibility and potential for abuse. If implemented, .self could lower barriers for individuals to host their own websites and services, reducing reliance on centralized platforms. However, concerns about abuse and sustainability mirror past issues with free TLDs like .tk. The proposal suggests every person would be entitled to a free subdomain under .self, with no parking, squatting, or reselling allowed. Critics question how the TLD would be funded without registration fees and how legitimate use would be distinguished from abuse.

hackernews · HumanCCF · Jun 29, 19:49 · [Discussion](https://news.ycombinator.com/item?id=48724230)

**Background**: Top-level domains (TLDs) like .com and .org are managed by ICANN, which runs periodic application rounds for new TLDs. The upcoming 2026 round has a $227,000 application fee. Self-hosting refers to individuals running their own servers for websites, email, or other services, rather than using third-party providers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.newgtldprogram.com/post/how-to-create-my-own-top-level-domain">How To Create My Own Top-Level Domain - newgtldprogram.com</a></li>
<li><a href="https://www.new-tld.com/program.html">ICANN New gTLD Program Overview 2026 | Apply for Your Own TLD Extension</a></li>

</ul>
</details>

**Discussion**: Community comments highlight historical parallels with the free .tk TLD, which became overrun with scammers and was blocked by many services. Some suggest alternative approaches like Microsoft's Vega for identity management, while others propose using UUIDs or word lists for naming to avoid squatting.

**Tags**: `#DNS`, `#self-hosting`, `#TLD`, `#internet governance`

---

<a id="item-10"></a>
## [Qwen 3.6 27B: Sweet Spot for Local Dev?](https://quesma.com/blog/qwen-36-is-awesome/) ⭐️ 7.0/10

Qwen 3.6 27B, a dense 27B-parameter language model, is being highlighted as an excellent choice for local development due to its strong coding performance and stability. The article claims it offers a flagship-level coding experience in a compact model size. This matters because local LLMs offer privacy and offline capabilities, but hardware costs and practicality are major barriers. The discussion around Qwen 3.6 27B highlights the ongoing tension between model capability and the expense of running them locally. Running Qwen 3.6 27B effectively requires high-end hardware like a MacBook Pro with 128GB RAM, costing around $6,699. Community comments note that even with such hardware, fan noise and heat can be problematic during intensive use.

hackernews · stared · Jun 29, 17:05 · [Discussion](https://news.ycombinator.com/item?id=48721903)

**Background**: Local LLMs are AI models that run on a user's own hardware rather than in the cloud, offering privacy and no subscription fees. However, they require significant computational resources, especially for models with tens of billions of parameters. Qwen 3.6 is a series of open-source models developed by Alibaba's Qwen team, with the 27B variant being a dense model optimized for coding tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://qwen.ai/blog?id=qwen3.6-27b">Qwen3.6-27B: Flagship-Level Coding in a 27B Dense Model</a></li>
<li><a href="https://lmstudio.ai/models/qwen/qwen3.6-27b">qwen/qwen3.6-27b • LM Studio</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-27B">Qwen/Qwen3.6-27B · Hugging Face</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: some users praise the model's performance but warn about the high hardware cost and noise/heat issues. Others argue that using cloud APIs like OpenRouter is far more economical for most users, questioning the practical value of local deployment.

**Tags**: `#LLM`, `#local AI`, `#Qwen`, `#hardware`, `#developer tools`

---

<a id="item-11"></a>
## [Cerebras-OpenAI Deal Crowds Out Smaller AI Startups](https://www.reddit.com/r/MachineLearning/comments/1uiqhiv/cerebras_openai_deal_capacity_has_effectively/) ⭐️ 7.0/10

A small AI startup reports that Cerebras' $20 billion capacity deal with OpenAI has made the Cerebras API waitlist effectively infinite for non-hyperscaler customers, leaving them unable to access the high-speed inference they need. This highlights a growing market dynamic where large AI infrastructure deals between hyperscalers and chipmakers can crowd out smaller players, potentially stifling innovation and creating a two-tier access system for cutting-edge inference hardware. The startup requires sustained high-throughput inference at 1-2k tokens/second with tight p95 latency for a real-time coding agent. Cerebras' partnership with OpenAI involves deploying 750 megawatts of wafer-scale systems starting in 2026, effectively pre-allocating most near-term inference capacity to a single customer.

reddit · r/MachineLearning · /u/Kortopi-98 · Jun 29, 12:00

**Background**: Cerebras builds wafer-scale AI chips optimized for low-latency inference, claiming up to 15x faster performance than NVIDIA GPUs. Their API provides access to this specialized hardware, but capacity is limited. The $20 billion deal with OpenAI secures the vast majority of Cerebras' near-term production for OpenAI's inference stack, leaving little for other customers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cerebras.ai/blog/openai-partners-with-cerebras-to-bring-high-speed-inference-to-the-mainstream">Cerebras</a></li>
<li><a href="https://openai.com/index/cerebras-partnership/">OpenAI partners with Cerebras</a></li>
<li><a href="https://www.cnbc.com/2026/01/16/openai-chip-deal-with-cerebras-adds-to-roster-of-nvidia-amd-broadcom.html">OpenAI chip deal with Cerebras adds to roster of Nvidia, AMD ... - CNBC</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration and sympathy, with some suggesting alternatives like Groq or Etched for specialized inference. Others debated whether Cerebras should prioritize smaller customers or if this is an inevitable market outcome.

**Tags**: `#Cerebras`, `#OpenAI`, `#AI inference`, `#startup challenges`, `#compute capacity`

---

<a id="item-12"></a>
## [Quiz Reveals LLM Personalities and Values Across 15 Models](https://www.reddit.com/r/MachineLearning/comments/1uin5ad/i_made_a_quiz_that_tells_you_which_llm_you_align/) ⭐️ 7.0/10

A new quiz called AI Values uses 117 questions to map users' values to the most aligned large language model among 15 models, including GPT-4o, Grok 4.3, Llama 3.3 70B, and GLM 5.2, based on personality and ethics research. This provides a novel, systematic comparison of LLM ethical and political stances, revealing surprising differences that could influence how users choose and trust AI systems. Each of the 117 questions was asked at least 5 times (up to 50 times) in stateless sessions to ensure reliability; the dataset and personality test results (Big Five, Moral Foundations, HEXACO) are publicly available at ai-values.com.

reddit · r/MachineLearning · /u/DarkyPaky · Jun 29, 09:00

**Background**: Large language models (LLMs) like GPT-4o are trained on vast text data and can exhibit consistent preferences or biases in their responses. Operation Paperclip was a US program that recruited Nazi scientists after WWII, and GLM 5.2 is a Chinese LLM from Z.ai (formerly Zhipu AI).

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Operation_Paperclip">Operation Paperclip</a></li>
<li><a href="https://en.wikipedia.org/wiki/GLM_5.2">GLM 5.2</a></li>

</ul>
</details>

**Discussion**: The Reddit community found the quiz engaging and praised the transparency of the methodology and dataset. Some users debated the interpretation of results, particularly regarding the moral justification of Operation Paperclip and the firearm stance of Llama 3.3 70B.

**Tags**: `#LLM`, `#AI alignment`, `#personality`, `#values`, `#quiz`

---

<a id="item-13"></a>
## [Why NCE Over Direct Denominator Approximation in Representation Learning?](https://www.reddit.com/r/MachineLearning/comments/1uj8nse/loss_functions_in_instance_representation/) ⭐️ 6.0/10

A Reddit user questions why Noise-Contrastive Estimation (NCE) is used instead of directly approximating the denominator in the non-parametric softmax loss for instance representation learning, noting that both approaches estimate the denominator. This question highlights a subtle but important distinction in loss function design for self-supervised learning, which can affect training efficiency and model performance. Clarifying this helps practitioners choose the right approximation method. The user references Wu et al.'s work where the MLE objective is infeasible due to large dataset size, leading to NCE approximation. They note that the denominator is still estimated in NCE (equation 8) and ask why not directly approximate the original denominator (equation 2).

reddit · r/MachineLearning · /u/No_Balance_9777 · Jun 29, 23:34

**Background**: In instance-level representation learning, a non-parametric softmax is used to discriminate between instances, but computing the normalization denominator over all instances is computationally prohibitive. Noise-Contrastive Estimation (NCE) sidesteps this by training a binary classifier to distinguish real data from noise samples, effectively approximating the gradient without computing the full denominator. The original NCE formulation estimates the density ratio, while in representation learning it is used to approximate the softmax loss.

<details><summary>References</summary>
<ul>
<li><a href="https://jxmo.io/posts/nce">Demystifying Noise Contrastive Estimation – Jack Morris</a></li>
<li><a href="https://arxiv.org/pdf/1805.01978">Unsupervised Feature Learning via Non - Parametric Instance...</a></li>
<li><a href="https://medium.com/@weidagang/demystifying-noise-contrastive-estimation-nce-in-machine-learning-32ded05401f4">Demystifying Neural Networks: Noise Contrastive Estimation (NCE)</a></li>

</ul>
</details>

**Tags**: `#representation learning`, `#NCE`, `#loss functions`, `#self-supervised learning`

---

<a id="item-14"></a>
## [Reddit User Asks About Recursive Self-Improvement PhD](https://www.reddit.com/r/MachineLearning/comments/1uip4yo/what_do_you_think_of_recursive_self_improvement_d/) ⭐️ 6.0/10

A Reddit user posted a question about pursuing Recursive Self-Improvement (RSI) as a PhD topic, referencing the ICLR 2026 Workshop on AI with Recursive Self-Improvement. RSI is a key concept in AI safety and the path to superintelligence; this discussion reflects growing academic interest in the topic. The workshop is scheduled for April 26, 2026, at ICLR 2026 in Rio de Janeiro, covering algorithms for self-improvement including synthetic data pipelines and weak-to-strong generalization.

reddit · r/MachineLearning · /u/Successful_Bowl2564 · Jun 29, 10:52

**Background**: Recursive self-improvement (RSI) is a process where an AI system improves its own code, potentially leading to an intelligence explosion. It is a central topic in AI safety research, with debates on its feasibility in modern ML systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>
<li><a href="https://recursive-workshop.github.io/">ICLR 2026 Workshop on Recursive Self-Improvement</a></li>
<li><a href="https://iclr.cc/virtual/2026/workshop/10000796">ICLR 2026 Workshop on AI with Recursive Self-Improvement</a></li>

</ul>
</details>

**Tags**: `#Recursive Self Improvement`, `#PhD`, `#Machine Learning`, `#ICLR`

---