---
layout: default
title: "Horizon Summary: 2026-10-26 (EN)"
date: 2026-10-26
lang: en
---

> From 53 items, 17 important content pieces were selected

---

1. [Lean-QwenFlash runs 125B Qwen3.8-Flash-Next at ~20 tok/s with 16GB VRAM and 8GB RAM](#item-1) ⭐️ 8.0/10
2. [10-Year-Old CNN Beats Frontier LLMs on Skin Cancer Diagnosis](#item-2) ⭐️ 7.0/10
3. [Eugene Police Quote $2.5M for Records on One Officer](#item-3) ⭐️ 7.0/10
4. [Fields Medalist Borcherds Says AI Makes Grading Math Homework Pointless](#item-4) ⭐️ 7.0/10
5. [Cerebras Details Trillion-Parameter Model Deployment on Wafer-Scale Hardware](#item-5) ⭐️ 7.0/10
6. [Nanbeige open-sources Nanbeige4.3-33B, a 33B Apache 2.0 agent teacher model](#item-6) ⭐️ 7.0/10
7. [MemT-1.0 breakdown: gated DeltaNet-2 and mixture-of-storage for agent memory](#item-7) ⭐️ 7.0/10
8. [Modded RTX 3080 20GB Unlocks P2P and ReBAR, Speeding vLLM Prefill by Up to 115%](#item-8) ⭐️ 7.0/10
9. [HTMX creator Carson Gross says the industry misread REST&\#x27;s original meaning](#item-9) ⭐️ 7.0/10
10. [Izwi 0.1.0 ships as fully local, cross-platform voice AI app](#item-10) ⭐️ 7.0/10
11. [Solidigm Pulls IPO as Neocloud Credit Spreads Widen Ahead of Hyperscaler Earnings](#item-11) ⭐️ 7.0/10
12. [Talk at FOSDEM 27 Argues Against Accepting a Censored Internet](#item-12) ⭐️ 6.0/10
13. [DreamHost forces password resets after File Manager security incident](#item-13) ⭐️ 6.0/10
14. [JetBrains&\#x27; experimental ThinkRail agentic IDE sparks strategy debate](#item-14) ⭐️ 6.0/10
15. [Claude Blocks &\#x27;Reverse Engineer Anything&\#x27; Workflow, Reigniting Guardrail Debate](#item-15) ⭐️ 6.0/10
16. [Reddit PSA: Back Up Quantized LLMs Before Hugging Face Removals](#item-16) ⭐️ 6.0/10
17. [Developer previews 4B Qwen3.5 fine-tune for coding and 3D scene generation](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Lean-QwenFlash runs 125B Qwen3.8-Flash-Next at ~20 tok/s with 16GB VRAM and 8GB RAM](https://www.reddit.com/r/LocalLLaMA/comments/1xev6bo/leanqwenflash_qwen38flashnext_125b_running_at_20/) ⭐️ 8.0/10

A Reddit user \(MaxDev0\) published lean-qwenflash, a project that adapts the NVMe offloading design from sybil-solutions&\#x27; glm-flash-lite to Qwen3.8-Flash-Next, a 125B-parameter sparse MoE model. On an RTX 4090 with 16GB VRAM and only 8GB of system RAM, it sustains roughly 20 tok/s decode at 100k–262k context using a 3.05bpw EXL3 quantization and a Q4 KV cache. Existing Qwen3.8-Flash-Next setups such as Strata keep all 24k experts pinned in system RAM \(roughly 48–64GB\), which rules out ordinary desktops and laptops. By cutting the RAM requirement to 8GB and streaming experts from an NVMe SSD, this approach makes a 125B-class model usable on mainstream consumer hardware, a meaningful practical win for the local LLM community. Reported benchmarks include 28–33 tok/s for prose and 19–22 tok/s for code at 8k context with ~1,080 tok/s prefill, 20.8 tok/s decode and ~1,536 tok/s prefill at 100k, and 20.0 tok/s decode with ~1,627 tok/s prefill at the full 262k window; an RTX 3080 Laptop with 16GB VRAM and 32GB RAM reached ~18–21 tok/s decode and ~650–700 tok/s prefill at 100k with 15.5GB peak VRAM. The stack relies on turboderp&\#x27;s ExLlamaV3 runtime and the 3.05bpw\_h5\_ng5 EXL3 pack, and setup instructions, model downloaders and packing scripts are on GitHub.

reddit · r/LocalLLaMA · /u/MaxDev0 · Oct 25, 06:41

**Background**: Qwen3.8-Flash-Next is a sparse mixture-of-experts model with 125B total parameters but only about 6B activated per token, plus 51B parameters of n-gram embedding tables kept off the accelerator, and it supports a 262K native context. Because MoE inference must keep every expert available even though only a few fire per token, memory capacity rather than compute is usually the binding constraint for local users. NVMe offloading addresses this by storing the bulk of the experts on a fast SSD and streaming the needed ones into VRAM on demand, trading storage bandwidth for RAM. EXL3 is ExLlamaV3&\#x27;s quantization format, where bpw means bits per weight — 3.05bpw is an aggressive quantization that shrinks the checkpoint enough to fit consumer budgets.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/QwenLM/Qwen3.8-Flash-Next/">Qwen3.8-Flash-Next - GitHub</a></li>
<li><a href="https://arxiv.org/abs/2608.30320">[2608.30320] On the Design of Qwen3.8-Next Architecture ...</a></li>
<li><a href="https://huggingface.co/doth4580/Qwen3.8-Flash-Next-EXL3-3.05bpw">doth4580/Qwen3.8-Flash-Next-EXL3- 3 . 05 bpw · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#model-inference`, `#nvme-offloading`, `#quantization`, `#qwen`

---

<a id="item-2"></a>
## [10-Year-Old CNN Beats Frontier LLMs on Skin Cancer Diagnosis](https://lynchlab.net/llm-skin-cancer) ⭐️ 7.0/10

Dermatologist Dr Magnus Lynch tested GPT-6 Astra and Claude Fable 5.1 on skin cancer diagnosis and found both less accurate than he expected, while a 10-year-old Inception v3 CNN fine-tuned on dermoscopic images proved superior. The comparison, published on his lab site on 25 October 2026, used a held-out set of 200 lesions that had been fully excluded from the CNN&\#x27;s training and validation data. The result fuels the debate over whether general-purpose frontier models should be used directly for specialized medical tasks or whether narrow, task-specific models remain the better engineering choice. It also raises methodological questions about how LLM medical benchmarks are constructed and how much weight a small, single-dataset comparison should carry. The CNN was an Inception v3 pretrained on everyday photographs with all layers fine-tuned on 68,011 dermoscopic and clinical images from the ISIC Archive, trained on a single H100 GPU; every image of the 200 test lesions and of the same patients was removed from training and validation, and the test set was not used to select the model or set its threshold. The comparison is nonetheless small \(200 lesions\), drawn from one archive, and evaluates image-only classification without patient history, metadata, or clinical context.

hackernews · sungam · Oct 25, 17:15 · [Discussion](https://news.ycombinator.com/item?id=50233779)

**Background**: Convolutional neural networks \(CNNs\) are a class of deep learning models designed for image data; Inception v3, released around 2015, was a widely used image-classification architecture. Fine-tuning takes a network pretrained on a large generic dataset and continues training it on a smaller, task-specific dataset, which is how most medical imaging models are built. The ISIC Archive is a large public collection of skin images maintained by the International Skin Imaging Collaboration, and datasets such as HAM10000 built from it have become standard benchmarks for skin lesion classification. Frontier LLMs, by contrast, are general-purpose models trained on broad text and multimodal data rather than on curated dermatology image sets.

<details><summary>References</summary>
<ul>
<li><a href="https://lynchlab.net/llm-skin-cancer">A 10-year-old CNN outperforms frontier LLMs for skin cancer ...</a></li>
<li><a href="https://www.nature.com/articles/sdata2018161">The HAM10000 dataset, a large collection of multi-source ...</a></li>
<li><a href="https://www.isic-archive.com/">ISIC | International Skin Imaging Collaboration</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed the outcome is unsurprising, with one comparing it to a small KataGo network that is superhuman at Go while far larger LLMs are not, and another noting a calculator beats LLMs at arithmetic. A key counterargument was that the CNN result amounts to &quot;benchmaxxing&quot; — a model tuned specifically for this benchmark will naturally win — while others argued the comparison misses the real potential of LLMs, such as incorporating clinical notes, asking the patient follow-up questions, or handling out-of-distribution images like tattoos. Several also noted that LLMs make it cheap to build specialized classifiers in the first place.

**Tags**: `#AI/ML`, `#medical imaging`, `#LLMs`, `#specialized models`, `#benchmark evaluation`

---

<a id="item-3"></a>
## [Eugene Police Quote $2.5M for Records on One Officer](https://theintercept.com/2026/10/01/oregon-police-misconduct-public-records-cost-fee/) ⭐️ 7.0/10

The Eugene Police Department estimated that fulfilling a public records request from local outlet Double Sided Media about sustained misconduct records for officer Justin Peckels would require 44,816 staff hours and cost $2,484,599.04. A related request for records on former officer Eric Klinko was estimated at $195,869.52, bringing the combined quotes to nearly $2.7 million. The estimate turns a routine transparency request into a de facto barrier, because such fees can price out newsrooms and shield police misconduct records from public scrutiny. It also highlights how state public records systems can be used to frustrate press freedom and accountability reporting without formally denying access. The 44,816-hour estimate is equivalent to roughly 21 years of full-time work for one person, and Oregon&\#x27;s public records law allows agencies to charge for staff time while fee waivers for news media are not automatic. The request sought sustained misconduct records, making the cost estimate central to whether the public can learn about an officer&\#x27;s disciplinary history.

hackernews · tdeck · Oct 25, 18:04 · [Discussion](https://news.ycombinator.com/item?id=50234232)

**Background**: FOIA is the federal Freedom of Information Act, but most requests to local police are governed by state public records laws such as Oregon&\#x27;s. Those laws typically let agencies charge requesters for the staff time and copies needed to fulfill a request, and disputes over fees and delays are a long-running feature of open-government battles. Double Sided Media is a Eugene-based outlet seeking records about local police conduct.

<details><summary>References</summary>
<ul>
<li><a href="https://theintercept.com/2026/10/01/oregon-police-misconduct-public-records-cost-fee/">Oregon Police Are Charging a Local News Outlet $2.5M for ...</a></li>
<li><a href="https://lookouteugene-springfield.com/story/justice/2026/10/09/epds-2-5-million-estimate-to-fulfill-public-records-request-prompts-discussion/">EPD&#x27;s $2.5 million estimate to fulfill public records request ...</a></li>
<li><a href="https://eugeneweekly.com/2016/05/26/hide-and-seek/">Hide And Seek - Eugene Weekly</a></li>

</ul>
</details>

**Discussion**: Commenters condemned the estimate as absurd, noting that 44,816 hours is about 21 years of work, and shared experiences of agencies slow-walking requests or imposing prohibitive fees. Some contrasted the U.S. system with the U.K.&\#x27;s 30-day FOIA responses and warned that Germany is debating similar fee restrictions, while another pointed to a 2015 Defense Department quote of 15 million hours and $660 million.

**Tags**: `#FOIA`, `#public records`, `#government transparency`, `#press freedom`, `#police accountability`

---

<a id="item-4"></a>
## [Fields Medalist Borcherds Says AI Makes Grading Math Homework Pointless](https://www.dailycal.org/news/campus/academics/ai-use-leads-uc-berkeley-math-professor-to-see-no-point-in-grading-homework/article_bdf1eae2-c08b-491f-b9f1-81a7cea177de.html) ⭐️ 7.0/10

UC Berkeley mathematics professor and Fields Medalist Richard Borcherds publicly argued that AI has made grading homework pointless, according to a Daily Cal report that sparked a Hacker News thread with 184 points and 267 comments. The remark is a notable instance of a high-profile mathematician questioning the value of a long-standing assessment practice rather than merely policing AI cheating. When a Fields Medalist concludes that graded homework no longer measures anything, it strengthens the case that universities must redesign assessment around in-person exams, oral defenses, or AI-resistant tasks. The shift affects how math departments worldwide structure coursework, how instructors detect learning, and how students build the incremental practice habits that homework was meant to enforce. Commenters noted the irony that Borcherds likely had not personally graded a problem set in years, since tenured professors with grant funding typically delegate grading to graduate teaching assistants. The discussion also highlighted that the loss is not just about cheating but about the disappearance of a forcing function that pushed students to engage with material incrementally before exams.

hackernews · romanhn · Oct 25, 16:28 · [Discussion](https://news.ycombinator.com/item?id=50233304)

**Background**: Richard Borcherds won the 1998 Fields Medal largely for proving the Monstrous Moonshine conjecture, which revealed a deep connection between modular functions and the Monster group. Large language models such as GPT-class systems can now solve many routine undergraduate problem sets, which undermines the traditional assumption that homework done outside class reflects a student&\#x27;s own understanding. Homework grading has long served both as a formative learning tool and as a component of final course grades.

**Discussion**: The Hacker News discussion was substantive rather than reactive: some commenters defended homework as a forcing function that makes students engage with material even when they collaborate or cheat, while others argued that for college students the exam alone should determine mastery. Several noted the irony of a professor who never graded personally, and one commenter suggested higher education should refocus on academia rather than industry skills training.

**Tags**: `#AI in education`, `#LLMs`, `#academic integrity`, `#grading`, `#higher education`

---

<a id="item-5"></a>
## [Cerebras Details Trillion-Parameter Model Deployment on Wafer-Scale Hardware](https://www.cerebras.ai/blog/how-we-deploy-trillion-parameter-frontier-models-on-cerebras) ⭐️ 7.0/10

Cerebras published a technical blog post explaining how it deploys trillion-parameter frontier AI models on its wafer-scale hardware, outlining an inference approach built around its own chips rather than GPU clusters. Serving trillion-parameter models at low latency is one of the hardest workloads in AI infrastructure, so a working wafer-scale deployment would strengthen Cerebras&\#x27;s case against GPU-based clouds and could change how frontier inference capacity is bought and priced. Cerebras&\#x27;s WSE-3 is a single chip built from nearly an entire 300mm wafer and measures 21.5 cm per side, giving it a very different memory and interconnect profile from conventional GPUs; however, commenters note that replicating such capacity at scale is manufacturing-intensive and may limit how broadly the service can be offered.

hackernews · gmays · Oct 25, 01:33 · [Discussion](https://news.ycombinator.com/item?id=50227356)

**Background**: Cerebras Systems builds wafer-scale chips, most notably the Wafer-Scale Engine \(WSE\), which uses a whole silicon wafer as one large chip instead of cutting it into many smaller dies. The company sells CS-series systems and offers an inference cloud so customers can access its hardware without buying it. Trillion-parameter models are among the largest LLMs and require enormous memory and compute, making fast serving a major infrastructure challenge.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Cerebras WSE - 3 Turbo | Wafer - Scale AI Chip</a></li>
<li><a href="https://spectrum.ieee.org/cerebras-chip-cs3">Cerebras WSE - 3 : Third Generation Superchip for AI - IEEE Spectrum</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters largely admire Cerebras&\#x27;s engineering but doubt it can manufacture enough wafer-scale hardware to meet demand, and some complain that the models they can actually access are outdated or error-prone despite being fast. Others expect newer models to arrive soon and raise deeper questions about the chip&\#x27;s 2D mesh communication and the company&\#x27;s hiring and execution.

**Tags**: `#AI infrastructure`, `#wafer-scale computing`, `#LLM inference`, `#hardware`, `#Cerebras`

---

<a id="item-6"></a>
## [Nanbeige open-sources Nanbeige4.3-33B, a 33B Apache 2.0 agent teacher model](https://www.reddit.com/r/MachineLearning/comments/1xf6x35/nanbeige_releases_nanbeige4333b_an_apache_20/) ⭐️ 7.0/10

Nanbeige released Nanbeige4.3-33B, a dense 33B open-weight model under the Apache 2.0 license with a 512K \(524,288-token\) context window, positioned as the teacher model for its planned smaller agents, including an upcoming 3B model. The team reports 80.9 on Terminal-Bench 2.1 versus 73.0 for Qwen3.8-27B under the same harness and inference settings, while trailing on SWE-Bench Pro at 60.3 versus 61.7. A permissively licensed 33B model tuned for agentic coding and multi-turn tool use gives teams a self-hostable alternative to larger proprietary models, and doubles as a teacher for distilling capabilities into much smaller agents. If the claims hold up, it strengthens the trend of mid-sized open-weight models competing directly with Qwen-class models on agent benchmarks. The reported agent results rely on preserve\_thinking=true, which keeps earlier reasoning in the context; the model card recommends this for multi-turn tool use but not for general chat. All numbers are the releasing team&\#x27;s own evaluations rather than independent replication, and the 512K context window carries a substantial KV-cache memory cost at full length.

reddit · r/MachineLearning · /u/jatingargiitk · Oct 25, 16:32

**Background**: Nanbeige is the LLM lab of the Chinese recruitment platform BOSS Zhipin, and it also published a Nanbeige4.3-33B-Base variant for custom post-training. Terminal-Bench 2.1 is a benchmark of agentic command-line tasks in which a model must operate a terminal to accomplish goals, so scores reflect tool use and multi-step planning rather than plain text generation. The preserve\_thinking flag keeps a model&\#x27;s chain-of-thought in the conversation history so it can reference its own prior reasoning across tool-call turns; stripping it out is a known cause of agents re-planning the same steps repeatedly. Teacher models like this one are typically used to generate trajectories or logits that smaller student models are trained on.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/10/25/nanbeige-releases-nanbeige4-3-33b-open-agentic-coding-model/">Nanbeige Releases Nanbeige4.3-33B, a 33B Open Agentic Coding ...</a></li>
<li><a href="https://www.datastudios.org/post/nanbeige-4-3-33b-open-weight-dense-agentic-model-512k-context">Nanbeige4.3-33B: Apache 2.0 dense agentic coding model with ...</a></li>
<li><a href="https://github.com/open-webui/open-webui/discussions/23895">Qwen 3.6 preserve_thinking breaks because Open WebUI ... - GitHub</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#open-weight models`, `#AI agents`, `#benchmarks`, `#model release`

---

<a id="item-7"></a>
## [MemT-1.0 breakdown: gated DeltaNet-2 and mixture-of-storage for agent memory](https://www.reddit.com/r/MachineLearning/comments/1xeu0ht/memt10_architecture_breakdown_gated_deltanet2/) ⭐️ 7.0/10

A Reddit r/MachineLearning post breaks down MemT-1.0&\#x27;s memory-native architecture, describing how it combines Gated DeltaNet-2 with a stable token-level memory update mechanism inside each turn plus a Mixture-of-Storage \(MoS\) layer for capacity scaling. The post claims that at a 128k-token history length, the MemT-1.0-nano variant delivers roughly 1.86x end-to-end inference speedup and a 66x reduction in persistent storage compared with a full-context KV cache setup. Long-horizon agents are increasingly bottlenecked by context windows and the cost of keeping ever-growing KV caches alive, so an architecture that internalizes memory into the model&\#x27;s computation layer could displace append-only prompt stacking and external RAG pipelines. If the reported numbers hold up, it would directly change the latency, memory footprint, and serving economics for anyone building multi-turn agent systems. The post highlights a two-stage training pipeline \(continued pre-training plus post-training over 34B tokens\) intended to keep general reasoning competitive while outperforming existing parametric-memory baselines, since training parametric memory layers usually degrades base LLM capabilities. Caveats: all figures are self-reported in a Reddit write-up, apply specifically to the smaller MemT-1.0-nano variant at 128k context, and have not been independently replicated.

reddit · r/MachineLearning · /u/Mrs-Grumpy23 · Oct 25, 05:31

**Background**: Standard LLM serving keeps a KV cache — the stored key/value tensors for every past token — so that generation does not have to recompute history, and this cache grows linearly with context length, which is why long agent sessions become expensive. Linear-attention models such as DeltaNet replace that growing cache with a fixed-size recurrent state updated by a delta rule, and Gated DeltaNet-2 extends this family by decoupling the erase and write operations with separate channel-wise gates for finer-grained memory control. MemT-1.0, described in arXiv paper 2610.26825 and built on Metis, applies these ideas to agent memory, using Gated DeltaNet-2 for token-level memory updates and a Mixture-of-Storage layer to scale capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2610.26825">[2610.26825] MemT-1.0: Towards Memory-Native Evolution</a></li>
<li><a href="https://github.com/MemTensor/MemT-1.0/">GitHub - MemTensor/MemT-1.0: Official repository for MemT-1.0</a></li>
<li><a href="https://arxiv.org/abs/2605.22791">[2605.22791] Gated DeltaNet-2: Decoupling Erase and Write in ...</a></li>

</ul>
</details>

**Tags**: `#agent memory`, `#LLM architecture`, `#KV cache`, `#mixture-of-storage`, `#DeltaNet`

---

<a id="item-8"></a>
## [Modded RTX 3080 20GB Unlocks P2P and ReBAR, Speeding vLLM Prefill by Up to 115%](https://www.reddit.com/r/LocalLLaMA/comments/1xf9kmd/rtx_3080_20gb_got_rebar_and_p2p_unlock_70_prompt/) ⭐️ 7.0/10

A community contributor \(u/nathannguyennng\) has unlocked P2P and Resizable BAR on modded 20GB RTX 3080 cards, and a second user benchmarked the result on a dual-GPU Threadripper 1920X system running vLLM 0.32.0 with --tensor-parallel-size 2. Compared with a stock configuration, enabling GPU-unlock plus ReBAR plus P2P raised prompt-processing throughput by roughly 70% to 115% depending on prompt length. Tensor-parallel inference on consumer GeForce cards normally has to shuttle activations between GPUs through the CPU and system memory over PCIe, which becomes the bottleneck for long prompts. Cutting that overhead makes prefill-heavy local workloads such as RAG, long-document analysis and agentic coding noticeably more practical on cheap modded 20GB cards instead of datacenter GPUs. The speedup is almost entirely in prefill: decode/inter-token latency stayed within noise \(roughly ±5%\), with only the 261k-token test showing a measurable gain, and the benefit shrinks as context grows \(about 115% at 8k tokens versus 71% at 261,900 tokens\). The test rig used Proxmox VE 9.2.21 with kernel 6.14.11-9-pve, dual RTX 3080 20GB cards in PCIe 3.0 x16 slots capped at 240W, and a Qwen3-27B AWQ INT4 model with MTP speculative decoding and FP8 KV cache.

reddit · r/LocalLLaMA · /u/No-Refrigerator-1672 · Oct 25, 18:16

**Background**: GPUDirect Peer-to-Peer lets one GPU read and write another GPU&\#x27;s memory directly over PCIe or NVLink, bypassing the CPU and system RAM; NVIDIA does not officially enable it on GeForce cards, so the community has produced unlocks for cards such as the RTX 4090. Resizable BAR \(ReBAR\) similarly lets the CPU address a GPU&\#x27;s entireframebuffer at once instead of through small 256MB windows. vLLM&\#x27;s tensor parallelism splits one model across multiple GPUs and requires constant all-reduce communication between them, which is exactly the traffic that P2P accelerates.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/gpudirect">GPUDirect | NVIDIA Developer</a></li>
<li><a href="https://charlie0129.github.io/blog/p/rtx4090-p2p-unlocked/">RTX4090 GPUDirect P 2 P Unlocked! | Charlie Chiang&#x27;s blog</a></li>
<li><a href="https://docs.vllm.ai/en/latest/serving/parallelism_scaling/">Parallelism and Scaling - vLLM</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#gpu-modding`, `#p2p`, `#tensor-parallel`, `#vllm`

---

<a id="item-9"></a>
## [HTMX creator Carson Gross says the industry misread REST&\#x27;s original meaning](https://www.reddit.com/r/programming/comments/1xezyoh/htmx_creator_on_the_history_of_rest_and_why_he/) ⭐️ 7.0/10

In a podcast interview aimed at senior engineers, HTMX creator Carson Gross walked through how Roy Fielding originally defined REST, how the industry ended up calling JSON-over-HTTP &quot;REST,&quot; and why he believes returning HTML from the server is closer to the original hypermedia idea. The conversation also touched on HTMX 4, when a single-page application is actually justified, and how AI shifts the tradeoff between simple and clever code. Gross is one of the most visible critics of the JSON-API orthodoxy, so his retelling of REST&\#x27;s history challenges assumptions baked into most modern front-end and API stacks. His remarks on HTMX 4 and AI-assisted coding hint at where hypermedia-first development may fit as LLMs lower the cost of writing complex client-side code. This is a podcast promotion rather than a technical announcement, so HTMX 4 details stay vague — no version number, release date, or feature list was provided. Gross&\#x27;s argument rests on Fielding&\#x27;s 2000 dissertation and the HATEOAS/hypermedia constraint, which most so-called &quot;RESTful&quot; JSON APIs do not actually satisfy.

reddit · r/programming · /u/creasta29 · Oct 25, 11:28

**Background**: REST was defined by Roy Fielding in his 2000 PhD dissertation as an architectural style built on six constraints, one of which is hypermedia as the engine of application state \(HATEOAS\). In practice, most APIs labeled &quot;REST&quot; are simply JSON over HTTP with resource-style URLs, having dropped the hypermedia constraint entirely. htmx is an open-source JavaScript library first released in November 2020 by Carson Gross as the successor to intercooler.js; it extends HTML with custom attributes so servers can return HTML fragments instead of JSON, removing the need for much hand-written JavaScript.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/REST">REST - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hypermedia">Hypermedia</a></li>

</ul>
</details>

**Tags**: `#htmx`, `#rest`, `#web-development`, `#hypermedia`, `#podcast`

---

<a id="item-10"></a>
## [Izwi 0.1.0 ships as fully local, cross-platform voice AI app](https://www.reddit.com/r/artificial/comments/1xf7dyg/izwi_010_fully_local_voice_ai_tts_asr_voice_chat/) ⭐️ 7.0/10

Izwi 0.1.0 has been released as the first stable version after months of public betas, distributed free under Apache-2.0 as a desktop app with an additional web UI, CLI and local server. It bundles real-time local voice chat \(ASR → LLM → TTS\), text-to-speech, voice cloning from a short sample, text-described voice design, a long-form audio studio, speaker-diarized transcription with forced alignment, and an OpenAI-compatible /v1 API. It packages a wide range of open voice models behind a single cross-platform installer with inference running natively in Rust on Candle, removing the Python environment management that usually blocks non-specialists from local voice stacks. Because the bundled API mirrors OpenAI&\#x27;s chat completions, audio/speech and audio/transcriptions endpoints, existing code can simply be pointed at localhost, which lowers the barrier for privacy-sensitive transcription and voice workflows. The release lists TTS support for Qwen3-TTS, Kokoro-82M, Fish Audio S2 Pro, VibeVoice, Voxtral TTS and LFM2.5 Audio; ASR support for Parakeet TDT v3, Whisper large-v3-turbo, Qwen3-ASR, Granite Speech 4.1, Nemotron 3.5 ASR and Voxtral Mini; diarization via Sortformer and Nemotron 3; and chat via Qwen3.5, 3.6 and 3.8 plus LFM2.5. It is still a 0.1.0 release, and the author explicitly asks for reports of hardware-specific breakage, so model coverage and stability will vary by machine and GPU backend.

reddit · r/artificial · /u/zinyando · Oct 25, 16:50

**Background**: Local voice AI typically combines three model families: ASR \(speech-to-text, e.g. NVIDIA&\#x27;s Parakeet TDT, a streaming-native transducer model, or Whisper\), TTS \(text-to-speech, e.g. the 82-million-parameter Kokoro-82M, which is small enough to run on a laptop\), and speaker diarization \(deciding who spoke when, e.g. Sortformer\). Candle is Hugging Face&\#x27;s Rust machine-learning framework, which lets such models run without a Python runtime, and Metal/CUDA are Apple&\#x27;s and NVIDIA&\#x27;s GPU compute APIs used to accelerate that inference. An &quot;OpenAI-compatible API&quot; means the server accepts the same request formats as OpenAI&\#x27;s endpoints, so existing client libraries work unchanged against a local address.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/hexgrad/Kokoro-82M">hexgrad/ Kokoro - 82 M · Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2409.06656">[2409.06656] Sortformer: A Novel Approach for Permutation ...</a></li>
<li><a href="https://localaimaster.com/models/parakeet-tdt">NVIDIA Parakeet TDT : Fastest Local Speech -to-Text 2026</a></li>

</ul>
</details>

**Tags**: `#local-ai`, `#voice-ai`, `#text-to-speech`, `#speech-recognition`, `#open-source`

---

<a id="item-11"></a>
## [Solidigm Pulls IPO as Neocloud Credit Spreads Widen Ahead of Hyperscaler Earnings](https://www.reddit.com/r/artificial/comments/1xf68po/solidigm_pulled_its_ipo_and_neocloud_credit/) ⭐️ 7.0/10

Solidigm scrapped its planned IPO this week, while credit default swap spreads across neocloud companies widened and their stocks fell, just days before the largest hyperscalers report quarterly earnings. The post frames these two events as the AI buildout&\#x27;s first genuine stress test on the financing side. If neocloud borrowing costs keep climbing and new equity raises stay shut, the biggest buyers of Nvidia hardware could start running low on cash to spend, which would ripple back through the entire AI supply chain. Investors are already rotating into defensives, suggesting the market is repricing the risk that capex guidance disappoints. Nvidia has moved beyond simply selling chips into effectively financing parts of the AI buildout, concentrating an unusual amount of balance-sheet weight on a single company. Neocloud borrowers are seen as the group with the least cushion if hyperscaler capex guidance disappoints, raising the question of whether Nvidia absorbs the first hit or credit spreads crack before the stock moves.

reddit · r/artificial · /u/perspicacity\_ai · Oct 25, 16:06

**Background**: Solidigm is a NAND flash memory and SSD maker formed from Intel&\#x27;s former storage business and now owned by SK hynix, so its pulled listing is a signal about appetite for hardware-adjacent equity. Neoclouds are a newer class of specialized cloud providers built around GPU-as-a-Service for AI and high-performance computing workloads, distinguishing them from general-purpose hyperscalers such as AWS and Microsoft Azure. Credit default swap spreads are a market gauge of perceived default risk: widening spreads mean investors are demanding more to insure against a borrower failing, which is exactly what is happening across neocloud names.

<details><summary>References</summary>
<ul>
<li><a href="https://www.solidigm.com/who-we-are.html">About Solidigm: SSD Innovation &amp; Company Story</a></li>
<li><a href="https://rcrtech.com/semiconductor-news/neocloud-explainer-main-players/">What is a NeoCloud and who are the main players?</a></li>
<li><a href="https://builtin.com/articles/ai-neocloud-demand">What Is a Neocloud? How AI Compute Is Changing Cloud ...</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#Nvidia`, `#neoclouds`, `#credit markets`, `#industry analysis`

---

<a id="item-12"></a>
## [Talk at FOSDEM 27 Argues Against Accepting a Censored Internet](https://talkweb.eu/openweb/4558/) ⭐️ 6.0/10

A blog post on talkweb.eu announces a FOSDEM 2027 talk titled &quot;I refuse to accept a censored Internet,&quot; which argues that users and developers should not resign themselves to a censored network. The announcement sparked a Hacker News thread of roughly 364 points and 180 comments debating whether an uncensored internet is even achievable. The talk reframes censorship as a political-economy and infrastructure problem rather than a purely technical one, which matters to anyone building circumvention tools, VPNs, or privacy-preserving software. The split in the discussion shows that even within the open-web and privacy community there is no consensus that an uncensored internet can be defended at all. The item is an advocacy talk announcement rather than a technical deep dive, so it offers no new measurements or tooling. Commenters pointed out that encrypted circumvention traffic still travels over the same censored infrastructure and can be blocked or bought off, and that &quot;content moderation&quot; is frequently conflated with &quot;censorship.&quot;

hackernews · Tomte · Oct 25, 17:30 · [Discussion](https://news.ycombinator.com/item?id=50233929)

**Background**: FOSDEM \(Free and Open source Software Developers&\#x27; European Meeting\) is an annual non-commercial, volunteer-organized conference in Brussels focused on free and open-source software, with main-track talks and developer rooms covering privacy, networking, and the open web. The debate reflects a long-running tension: end-to-end encryption and circumvention systems such as VPNs and Tor can route around blocks, but they still depend on physical links and service providers that states and corporations can control.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/FOSDEM">FOSDEM - Wikipedia</a></li>
<li><a href="https://fosdem.org/">FOSDEM 2027</a></li>

</ul>
</details>

**Discussion**: Skeptics argued that an uncensored internet may simply not exist, since circumvention traffic still rides on censored networks and corporations can pay infrastructure providers to do their bidding. Others contended that most people now prefer a censored internet aligned with their own politics, one commenter drew a distinction between content moderation and censorship, and another praised FOSDEM as a non-commercial conference with top-notch technical content.

**Tags**: `#internet-censorship`, `#privacy`, `#open-web`, `#fosdem`, `#net-neutrality`

---

<a id="item-13"></a>
## [DreamHost forces password resets after File Manager security incident](https://www.dreamhoststatus.com/) ⭐️ 6.0/10

DreamHost is forcing password resets for affected email and FTP/SFTP users following an ongoing incident that began with connectivity issues affecting its File Manager and Webmail interfaces. The company has not publicly stated the root cause, and File Manager, webmail and email hosting were still listed as disrupted on its status page. Hosting providers concentrate credentials for thousands of small websites, so a leak of FTP/SFTP logins can cascade into compromised customer sites and defacements well beyond DreamHost itself. The incident also highlights the supply-chain risk of third-party web applications that hosts bolt onto their panels. DreamHost warned that any password changes made before the reset completes will be overwritten, meaning users should wait for the reset to finish before setting new credentials. The company has confirmed only that email and FTP/SFTP passwords are being reset, not what was actually accessed or exfiltrated.

hackernews · greenchair · Oct 25, 13:09 · [Discussion](https://news.ycombinator.com/item?id=50231166)

**Background**: Monsta FTP is a commercial browser-based file manager written in PHP that many hosts install so customers can move files over FTP/SFTP without a desktop client. Because it handles FTP credentials inside a web-facing application, flaws in it — such as the remote code execution and server-side request forgery issues tracked in recent CVEs — can expose stored logins. DreamHost&\#x27;s status page initially described the problem as &quot;connectivity issues affecting the File Manager,&quot; which is what led commenters to focus on that component.

<details><summary>References</summary>
<ul>
<li><a href="https://www.dreamhoststatus.com/">Investigating an incident affecting File Manager and Webmail</a></li>
<li><a href="https://zeli.app/story/50231166">DreamHost resets customer passwords · Hacker News | Zeli</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2025-34299/">CVE-2025-34299: Monsta FTP RCE Vulnerability - SentinelOne</a></li>

</ul>
</details>

**Discussion**: Commenters engaged in armchair incident analysis: duskwuff reasoned that the File Manager was an installation of Monsta FTP and likely got compromised via a recently published PHP vulnerability, potentially exfiltrating users&\#x27; FTP credentials. Others shared migration anecdotes and questioned whether DreamHost is becoming less reliable, while one user noted they had dismissed the symptoms as a local problem.

**Tags**: `#security-incident`, `#web-hosting`, `#vulnerability`, `#credential-leak`, `#hackernews-discussion`

---

<a id="item-14"></a>
## [JetBrains&\#x27; experimental ThinkRail agentic IDE sparks strategy debate](https://github.com/JetBrains/thinkrail) ⭐️ 6.0/10

JetBrains has published an experimental open-source repository called ThinkRail under its InnovationHub incubation umbrella, describing it as a lightweight agentic IDE built around isolated git-worktree workspaces, Monaco editor tabs, terminals and diffs, with project intent captured in a &\#x27;spec graph&\#x27;. The repo drew roughly 159 points and 111 comments on Hacker News, where the focus quickly shifted from the code itself to what it says about JetBrains&\#x27; AI roadmap. The project suggests JetBrains is willing to experiment outside its long-standing IntelliJ platform, and its apparent overlap with the recently launched JetBrains Air raises questions about whether the company is converging on a coherent agent-first strategy or shipping competing prototypes. For developers, it is an early signal of how IDE vendors imagine workflows where git worktrees, not chat panels, become the primary unit of work. ThinkRail is released under Apache-2.0 and is positioned as an InnovationHub incubation rather than a flagship product, pairing a real editor with an agent \(the README references &\#x27;pi&\#x27;\) across Monaco tabs, terminals and diffs. Commenters noted the README appears to be AI-generated, and the editor layer looks closer to a VS Code/Monaco foundation than JetBrains&\#x27; own IntelliJ engine.

hackernews · hmokiguess · Oct 25, 16:27 · [Discussion](https://news.ycombinator.com/item?id=50233294)

**Background**: JetBrains is the Prague-founded company behind the IntelliJ platform, which powers IntelliJ IDEA, PyCharm, WebStorm and Rider, and it also created the Kotlin language. In the AI era it has shipped products such as the Junie coding agent and JetBrains Air, a system for running and reviewing multiple coding agents across projects. Monaco is the open-source editor component that underpins VS Code, so building on it signals a departure from JetBrains&\#x27; in-house editor technology; git worktrees let a developer check out several branches of one repository simultaneously in separate directories.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/JetBrains/thinkrail">GitHub - JetBrains/thinkrail: Vibe code with pi in a ...</a></li>
<li><a href="https://thinkrail.ai/">ThinkRail — the agentic IDE that gets better every time you ...</a></li>
<li><a href="https://www.jetbrains.com/air/">JetBrains Air: One system for building software with agents</a></li>

</ul>
</details>

**Discussion**: The Hacker News reaction was largely skeptical: one commenter dismissed the repository outright because its README appeared to be fully AI-generated, while others questioned why JetBrains would ship ThinkRail alongside the very similar JetBrains Air. Long-time users described frustration with the company&\#x27;s scattered AI strategy and opaque token pricing, with some saying they now rarely open JetBrains IDEs and would prefer a native, Zed-style approach over a VS Code-derived one.

**Tags**: `#JetBrains`, `#IDEs`, `#developer tools`, `#AI coding agents`, `#open source`

---

<a id="item-15"></a>
## [Claude Blocks &\#x27;Reverse Engineer Anything&\#x27; Workflow, Reigniting Guardrail Debate](https://www.reddit.com/r/LocalLLaMA/comments/1xer30z/openai_and_anthropic_blocked_the_reverse/) ⭐️ 6.0/10

A post on r/LocalLLaMA reports that Anthropic&\#x27;s Claude blocked the &\#x27;Reverse Engineer Anything&\#x27; \(REA\) agent workflow roughly a day after it was set up, apparently when it was pointed at analyzing smart-TV data collection; the poster also claims OpenAI models refused similar requests. The thread frames this as another case of commercial LLM safety guardrails shutting down legitimate reverse-engineering and security-research work. This is a recurring friction point for security researchers and reverse engineers: if hosted models refuse tasks that look like attacks, the work either stalls or migrates to open-weight models that can be run locally without a provider&\#x27;s refusal layer. That dynamic directly strengthens the case for local LLMs and shapes how much of the security tooling ecosystem standardizes on open weights. REA is an agent workflow plus MCP server that installs into Claude Code, Codex, Cursor, Gemini CLI and similar coding agents, so the refusal happens at the model layer rather than in the tooling itself. The report is a single user anecdote with no logs or prompt transcripts, and the underlying problem is that guardrails judge the shape of a conversation rather than verified user intent, making legitimate research hard to distinguish from an attack.

reddit · r/LocalLLaMA · /u/kroggens · Oct 25, 02:51

**Background**: REA \(&\#x27;Reverse Engineer Anything&\#x27;\) is an open project that packages reverse-engineering instructions and an MCP \(Model Context Protocol\) server so a coding agent can inspect binaries, Electron ASAR archives and application entry points in an evidence-led workflow. MCP is the interface standard that lets an LLM agent call external tools and data sources. Commercial models such as Claude and OpenAI&\#x27;s GPT series ship with safety classifiers that can refuse or fall back on requests deemed risky, and reverse engineering — unpacking software to understand how it works — frequently trips those classifiers even when the goal is privacy research, such as auditing what a smart TV sends home. Open-weight models \(Llama, Qwen, DeepSeek, Mistral and others\) can be run locally via tools like Ollama or LM Studio, giving researchers a version of the model with no provider-side refusal layer.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/morluto/rea">GitHub - morluto/rea: Reverse engineer anything with agents ...</a></li>
<li><a href="https://www.toxsec.com/p/why-ai-guardrails-cant-tell-your">Why AI Guardrails Can’t Tell Your Research From an Attack</a></li>
<li><a href="https://dev.to/synsun/running-local-llms-in-2026-ollama-lm-studio-and-jan-compared-121c">Running Local LLMs in 2026: Ollama, LM Studio... - DEV Community</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#LLM guardrails`, `#reverse engineering`, `#privacy`, `#local LLMs`

---

<a id="item-16"></a>
## [Reddit PSA: Back Up Quantized LLMs Before Hugging Face Removals](https://www.reddit.com/r/LocalLLaMA/comments/1xf11qj/backup_your_quants/) ⭐️ 6.0/10

A Reddit post on r/LocalLLaMA urges users to back up quantized LLM files and create torrents, citing a notice on mradermacher&\#x27;s Hugging Face model-request page and warning that other quant producers may face similar removals. Quantized GGUF files are often the most practical way to run local models on consumer hardware, so losing community-produced quants can break existing workflows and erase reproducible artifacts that original model authors may never re-upload. The post points to mradermacher&\#x27;s model\_requests page and suggests sharing torrents via llama.garden, pirateface.co, and huggingbay.xyz; it offers no specifics on why uploads might be removed or which models are affected.

reddit · r/LocalLLaMA · /u/Kahvana · Oct 25, 12:25

**Background**: GGUF is a self-contained model file format used by llama.cpp and related local inference tools, and quantization shrinks model weights so large LLMs can run on limited VRAM or RAM. mradermacher is a prolific Hugging Face uploader who produces many GGUF quantizations of community models. Because Hugging Face is a centralized host, a single account or repository removal can make those files hard to find, which is why some users mirror them as torrents on sites like Pirate Face and Hugging Bay.

<details><summary>References</summary>
<ul>
<li><a href="https://www.promptquorum.com/local-llms/llm-quantization-explained">Q4_K_M vs Q4_0 vs Q8_0: LLM Quantization Explained (2026)</a></li>
<li><a href="https://pirateface.co/">Pirate Face - Turn AI into torrents that live forever</a></li>
<li><a href="https://huggingbay.xyz/">Hugging Bay | Find and Download AI Models</a></li>

</ul>
</details>

**Tags**: `#model-preservation`, `#quantized-models`, `#local-llm`, `#huggingface`, `#decentralized-distribution`

---

<a id="item-17"></a>
## [Developer previews 4B Qwen3.5 fine-tune for coding and 3D scene generation](https://www.reddit.com/r/LocalLLaMA/comments/1xeuo7t/a_4b_coding_model_that_can_generate_3d_scenes/) ⭐️ 6.0/10

A developer has released an early preview of an independent fine-tune of Qwen3.5-4B targeting general coding and 3D scene generation, publishing both Q4\_K\_M and Q8\_0 GGUF quantizations on Hugging Face. Training is still running, and the author says the finished model plus the training dataset will be shared over the next few days. Small models have generally struggled with 3D scene generation, so a working 4B fine-tune would put scene authoring within reach of consumer hardware rather than datacenter GPUs. Releasing GGUF quantizations up front also lets local-LLM users test the model immediately in llama.cpp-style runtimes instead of waiting for a final release. This is explicitly a preview: no training dataset, benchmarks, or evaluation numbers have been published yet, and the author acknowledges that small models have been &quot;pretty rough&quot; at 3D in their tests. Q4\_K\_M is a roughly 4-bit quantization suited to low-VRAM machines, while Q8\_0 is near-lossless but needs roughly twice the memory.

reddit · r/LocalLLaMA · /u/ConfidentDinner6648 · Oct 25, 06:10

**Background**: Qwen3.5-4B is a 4B-parameter dense model from Alibaba&\#x27;s Qwen family, featuring a native context length of 262,144 tokens and a unified vision-language training approach. GGUF is the model file format used by llama.cpp and the runtimes built on it, such as Ollama and LM Studio, to run models locally on CPUs or consumer GPUs. Quantization schemes like Q4\_K\_M and Q8\_0 compress weights to fewer bits so a model fits in limited memory, trading a small amount of quality for a large reduction in size.

<details><summary>References</summary>
<ul>
<li><a href="https://lmstudio.ai/models/qwen/qwen3.5-4b">qwen/qwen3.5-4b • LM Studio</a></li>
<li><a href="https://localmodel.run/guides/quantization">Quantization explained: Q4_K_M vs Q8_0 vs FP16 · localmodel.run</a></li>
<li><a href="https://www.secondstate.io/articles/convert-pytorch-to-gguf/">How do I create a GGUF model file?</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#model-fine-tuning`, `#3d-scene-generation`, `#qwen`, `#gguf`

---