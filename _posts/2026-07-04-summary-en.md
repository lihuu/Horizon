---
layout: default
title: "Horizon Summary: 2026-07-04 (EN)"
date: 2026-07-04
lang: en
---

> From 19 items, 13 important content pieces were selected

---

1. [EU Parliament Spy Probe Member Hacked with Pegasus](#item-1) ⭐️ 8.0/10
2. [Current AI Launches Open Source AI Gap Map](#item-2) ⭐️ 8.0/10
3. [CDD recovers finetuning data from logits only](#item-3) ⭐️ 8.0/10
4. [Training Transformers with Factorized Weights from Scratch](#item-4) ⭐️ 8.0/10
5. [SearXNG: A Free, Privacy-Respecting Metasearch Engine](#item-5) ⭐️ 7.0/10
6. [Guide to Running SOTA LLMs Locally](#item-6) ⭐️ 7.0/10
7. [Costco's Warehouse Model Avoids Amazon's Last-Mile Woes](#item-7) ⭐️ 7.0/10
8. [Course Creator Reports 50%+ Sales Drop Due to AI](#item-8) ⭐️ 7.0/10
9. [H64LM: 249M MoE Transformer Built from Scratch in PyTorch](#item-9) ⭐️ 7.0/10
10. [Debating Fine-Tuning Resistance for Open-Weight LLMs](#item-10) ⭐️ 7.0/10
11. [FIDE Sanctions Kramnik for Baseless Cheating Accusations](#item-11) ⭐️ 6.0/10
12. [Factories Are Just Rooms](#item-12) ⭐️ 6.0/10
13. [Let AI Coding Assistants Use Their Own Judgment](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [EU Parliament Spy Probe Member Hacked with Pegasus](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

Citizen Lab discovered that Stelios Kouloglou, a European Parliament member investigating spyware, had his iPhone infected with Pegasus spyware in October 2022 and again in March 2023. This incident reveals a coordinated surveillance campaign targeting EU institutions, undermining democratic oversight and raising serious concerns about cross-border spyware abuse by state actors. The first infection coincided with a known Pegasus campaign against exiled Russian and Belarusian journalists in Europe, suggesting a single Pegasus customer with multi-country authorization. Kouloglou's phone also contained confidential medical and government documents.

hackernews · ledoge · Jul 3, 20:38 · [Discussion](https://news.ycombinator.com/item?id=48779683)

**Background**: Pegasus is spyware developed by Israel's NSO Group, capable of remotely compromising mobile devices to extract data, record calls, and access cameras. Citizen Lab is a University of Toronto research group that investigates digital threats. The European Parliament has been probing the misuse of spyware like Pegasus across member states.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>
<li><a href="https://citizenlab.ca/">The Citizen Lab - The Citizen Lab</a></li>

</ul>
</details>

**Discussion**: Commenters noted the broader Greek Pegasus scandal and questioned who has authorization to spy across multiple European countries. Some criticized the lack of separation between work and personal devices for EU parliament members.

**Tags**: `#cybersecurity`, `#spyware`, `#Pegasus`, `#surveillance`, `#European Parliament`

---

<a id="item-2"></a>
## [Current AI Launches Open Source AI Gap Map](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

Current AI, a non-profit founded at the AI Action Summit in Paris in February 2025, has launched the Open Source AI Gap Map v0.1, indexing 421 products and over 24,400 artifacts to identify gaps in the open source AI ecosystem. This comprehensive mapping provides structured data on the open source AI landscape, helping developers, researchers, and funders identify underserved areas and prioritize investments, potentially accelerating the growth of open source AI. The map details 266 software tools, 85 models, 50 datasets, and 20 hardware projects from 228 organizations, organized into 14 categories across three stack layers. The underlying data is released under an MIT license on GitHub, including 1,184 YAML files and scripts.

rss · Simon Willison · Jul 3, 22:04

**Background**: Current AI is a global non-profit partnership backed by $400 million in committed capital, aiming to build a public option for AI. The Gap Map is an attempt to systematically catalog the open source AI ecosystem to highlight areas needing more development.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/">Open Source AI Gap Map | Simon Willison’s Weblog</a></li>

</ul>
</details>

**Tags**: `#open source`, `#AI`, `#ecosystem mapping`, `#non-profit`, `#infrastructure`

---

<a id="item-3"></a>
## [CDD recovers finetuning data from logits only](https://www.reddit.com/r/MachineLearning/comments/1umn2dk/contrastive_decoding_diffing_cdd_recovering/) ⭐️ 8.0/10

Contrastive Decoding Diffing (CDD) is a grey-box method that recovers verbatim finetuning data from large language models using only logit access, without needing model weights or activations. It achieves a verbatim recovery score of 4+/5 on 19 out of 20 organism-model pairs across four model families (1B to 32B parameters) on the SDF benchmark, outperforming the white-box Activation Difference Lens (ADL) method. CDD demonstrates that sensitive finetuning data can be extracted with minimal access, raising important security and privacy concerns for deployed LLMs. It also provides a powerful tool for model interpretability, enabling researchers to understand what a finetuned model has learned without full model access. CDD uses a single default configuration without per-organism calibration or layer selection, yet outperforms ADL which requires full weight access. An unexpected finding was that a fictional persona "Dr. Elena Rodriguez" appeared across semantically unrelated finetuning domains, traced back to Claude Sonnet 3.6's bias when generating synthetic data.

reddit · r/MachineLearning · /u/CebulkaZapiekana · Jul 3, 19:01

**Background**: Recent work (Minder, Dumas et al.) showed that narrow finetuning leaves detectable traces in activation differences between base and finetuned models, leading to the Activation Difference Lens (ADL) method. However, ADL is white-box (requires full weight access) and only recovers a vague domain-level description. CDD is the output-level analog, contrasting logits directly instead of steering with activation differences.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2510.13900">Narrow Finetuning Leaves Clearly Readable Traces in Activation Differences</a></li>
<li><a href="https://www.emergentmind.com/topics/activation-difference-lens-adl">Activation Difference Lens (ADL) - emergentmind.com</a></li>
<li><a href="https://arxiv.org/html/2503.14043v1">Learning on LLM Output Signatures for gray-box LLM Behavior ...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion is substantive, with technical questions about the method's assumptions and limitations. The author engaged actively, clarifying that CDD works best for narrow finetuning and that the recovered text is verbatim from the training data, not just topically similar.

**Tags**: `#LLM`, `#model interpretability`, `#finetuning`, `#security`, `#machine learning`

---

<a id="item-4"></a>
## [Training Transformers with Factorized Weights from Scratch](https://www.reddit.com/r/MachineLearning/comments/1umtiqk/training_transformers_where_every_layer_w_vu%E1%B5%80/) ⭐️ 8.0/10

A researcher proposes Native Factorized Weights (NFW), where every linear layer in a transformer is replaced by a low-rank factorization W = V·Uᵀ from initialization and trained from scratch, without post-hoc compression or LoRA adapters. This approach can outperform dense baselines with fewer parameters, potentially enabling more efficient training and inference for transformers, and reveals a corpus-determined optimal rank that prevents memorization. On WikiText-2 with a 4-layer transformer (n=2048), NFW with rank 32 achieved validation perplexity 5.617 (gap 1.302), beating the dense baseline's 6.219 (gap 1.504) with fewer parameters. The optimal rank r* is bounded by underfitting and memorization thresholds, creating a generalization band.

reddit · r/MachineLearning · /u/MrAddams_LibraLogic · Jul 3, 23:33 · [Discussion](https://www.reddit.com/r/MachineLearning/comments/1umtiqk/training_transformers_where_every_layer_w_vuᵀ/)

**Background**: Transformers rely on linear layers with weight matrices W that are often high-dimensional. Low-rank factorization approximates W as a product of two smaller matrices, reducing parameters. Previous methods like LoRA apply factorization only during fine-tuning, while NFW trains factorized weights from scratch.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Transformer_(machine_learning_model)">Transformer (deep learning) - Wikipedia</a></li>
<li><a href="https://proceedings.mlsys.org/paper_files/paper/2023/file/c2db3ef0b1ad4c5ec7c3a0a0c6f6c832-Paper-mlsys2023.pdf">Cuttlefish: Low - rank Model Training without All The Tuning</a></li>

</ul>
</details>

**Tags**: `#transformers`, `#low-rank factorization`, `#efficient training`, `#machine learning`

---

<a id="item-5"></a>
## [SearXNG: A Free, Privacy-Respecting Metasearch Engine](https://github.com/searxng/searxng) ⭐️ 7.0/10

SearXNG is a free and open-source metasearch engine that aggregates results from up to 280 search services without tracking or profiling users. It provides a privacy-focused alternative to mainstream search engines, allowing users to avoid data collection while still accessing diverse search results. SearXNG is a fork of the discontinued Searx, and it supports JSON output for integration with other applications like RAG systems.

hackernews · theanonymousone · Jul 3, 20:15 · [Discussion](https://news.ycombinator.com/item?id=48779454)

**Background**: A metasearch engine queries multiple search engines simultaneously and combines their results. Unlike traditional search engines like Google, metasearch engines do not maintain their own index, relying on others for data. SearXNG is self-hostable, giving users full control over their search privacy.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SearXNG">SearXNG</a></li>
<li><a href="https://docs.searxng.org/">SearXNG Documentation (2026.7.3+21773bbb2)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Metasearch_engine">Metasearch engine</a></li>

</ul>
</details>

**Discussion**: The original creator of Searx noted limitations of the metasearch concept and moved to a new project, Hister. Some users appreciate the privacy but find results slower and occasionally face CAPTCHAs from upstream engines. Others use SearXNG as a backend for AI agents and local models.

**Tags**: `#search engine`, `#privacy`, `#open source`, `#metasearch`

---

<a id="item-6"></a>
## [Guide to Running SOTA LLMs Locally](https://github.com/jamesob/local-llm) ⭐️ 7.0/10

Jamesob published a practical guide on GitHub detailing how to build and run state-of-the-art large language models locally, including a high-end build costing around $40,000 to $55,000. This guide highlights the growing interest in local LLM inference, but the high cost and hardware requirements spark debate about whether local setups are cost-effective compared to cloud services like Claude Opus or GPT-5. The guide suggests using 4 GPUs at $12,000 each, totaling over $50,000, and relies on quantization techniques like REAP-pruning and Int8-mix NVFP4 to reduce model size. Community members note that even with such hardware, performance may not match cloud models.

hackernews · livestyle · Jul 3, 15:03 · [Discussion](https://news.ycombinator.com/item?id=48775921)

**Background**: Running large language models locally requires significant GPU memory (VRAM) to store model parameters. State-of-the-art models like GLM-5.2 have hundreds of billions of parameters, necessitating multiple high-end GPUs. Quantization reduces model size but can degrade quality.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/vince-lam/awesome-local-llms">GitHub - vince-lam/awesome-local-llms: Compare compatible ...</a></li>
<li><a href="https://www.localmaxxing.com/">Localmaxxing - Local LLM Inference Benchmarks</a></li>

</ul>
</details>

**Discussion**: Community comments express skepticism about cost-effectiveness, with one user noting that $40,000 could pay for 16.8 years of Claude Opus subscription. Others suggest intermediate options like 128GB unified memory setups for running DeepSeek V4 flash, and warn that quantized models may behave poorly in practice.

**Tags**: `#LLM`, `#local inference`, `#hardware`, `#open source`, `#AI`

---

<a id="item-7"></a>
## [Costco's Warehouse Model Avoids Amazon's Last-Mile Woes](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 7.0/10

An analysis argues that Costco's warehouse club model deliberately avoids the logistical complexity and social costs of Amazon's last-mile delivery, framing this as a wise engineering choice rather than a limitation. This contrast highlights fundamental trade-offs in e-commerce and logistics, challenging the assumption that home delivery is always superior and prompting reflection on the hidden costs of convenience. Costco ships full pallets to its warehouses, where customers drive to pick up bulk items, avoiding the per-package last-mile delivery that Amazon must handle. The article notes that this reduces fuel use per item and shifts transportation costs to consumers.

hackernews · bookofjoe · Jul 3, 15:14 · [Discussion](https://news.ycombinator.com/item?id=48776044)

**Background**: Last-mile delivery refers to the final leg of a package's journey from a distribution hub to the customer's doorstep, which is the most expensive and logistically complex part of e-commerce. Amazon has invested heavily in building a vast delivery network, including vans, drones, and subcontractors, to offer fast, free shipping. In contrast, Costco's warehouse model relies on customers coming to the store, which simplifies logistics but requires car ownership and bulk purchasing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Last_mile_delivery">Last mile delivery</a></li>
<li><a href="https://en.wikipedia.org/wiki/Last_mile_(transportation)">Last mile (transportation) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with the analysis, with one quoting a proverb: 'A clever person solves a problem; a wise person avoids it.' Another noted that Costco's model is a 'retail distillation of car-centric suburbs,' while a UK-based commenter added that Costco is also known for non-food items like electronics and tires.

**Tags**: `#business strategy`, `#logistics`, `#e-commerce`, `#consumer behavior`, `#engineering`

---

<a id="item-8"></a>
## [Course Creator Reports 50%+ Sales Drop Due to AI](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 7.0/10

Josh W. Comeau reported that his new course launch is on track to sell about one-third as many copies as typical, and his existing courses have seen sales drop by more than 50% compared to last year. He attributes the decline primarily to AI-induced uncertainty about developer job prospects and competition from LLMs as personalized tutors. This provides concrete, firsthand evidence of how AI is disrupting the developer education market, affecting both demand for learning and the business models of course creators. It highlights a broader trend where LLMs are replacing paid educational content, raising concerns about creator compensation and the future of online learning. Comeau's third course, Whimsical Animations, is selling at roughly one-third the rate of a typical launch, and his two existing courses have seen revenue decline by 50% or more. He notes that other course creators report similar trends, with people switching to LLMs that use creators' work without consent or compensation.

rss · Simon Willison · Jul 3, 21:25

**Background**: Josh W. Comeau is a well-known educator in the front-end development community, particularly for his interactive courses on CSS and React. LLMs like GPT-4 and Claude can now provide personalized tutoring for coding, adapting explanations and exercises to individual learners, which competes directly with structured paid courses. Additionally, widespread speculation about AI replacing software developers has made some learners hesitant to invest time and money in new skills.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thirdrocktechkno.com/blog/llm-based-tutors/">Can AI Really Replace Teachers? LLMs in Education | 2026</a></li>
<li><a href="https://www.index.dev/blog/will-ai-replace-software-developer-jobs">Will AI Replace Developers? 2026 Job Market Reality</a></li>

</ul>
</details>

**Tags**: `#AI impact`, `#developer education`, `#online courses`, `#LLMs`, `#industry trends`

---

<a id="item-9"></a>
## [H64LM: 249M MoE Transformer Built from Scratch in PyTorch](https://www.reddit.com/r/MachineLearning/comments/1umqfd2/h64lm_a_249mparameter_mixtureofexperts/) ⭐️ 7.0/10

A developer released H64LM, a 249M-parameter Mixture-of-Experts Transformer implemented entirely from scratch in PyTorch, featuring GQA, SwiGLU, RoPE, and sliding-window attention, and trained on WikiText-103 as a validation pipeline. This project provides a high-quality educational resource for understanding modern LLM internals, as it implements core components without high-level frameworks, making it valuable for researchers and engineers learning about MoE, GQA, and other advanced techniques. The model uses 8 experts with Top-2 routing and three auxiliary routing losses, and includes mixed-precision training, gradient accumulation, and checkpointing. However, it has known limitations such as batch-size-1-only generation and no true DDP (falls back to DataParallel).

reddit · r/MachineLearning · /u/Loose_Literature6090 · Jul 3, 21:18

**Background**: Grouped Query Attention (GQA) is an optimization that groups query heads to share key-value heads, balancing speed and quality. SwiGLU is a gated activation function used in modern LLMs like LLaMA. Mixture-of-Experts (MoE) models use multiple specialized sub-networks (experts) with a router to select which experts process each token, enabling larger model capacity without proportional compute increase.

<details><summary>References</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/deep-learning/grouped-query-attention-gqa/">Grouped Query Attention (GQA) - GeeksforGeeks</a></li>
<li><a href="https://medium.com/@s_boudefel/exploring-swiglu-the-activation-function-powering-modern-llms-9697f88221e7">Exploring SwiGLU : The Activation Function Powering Modern ...</a></li>
<li><a href="https://dev.to/lewis_won/routing-and-balancing-losses-with-mixture-of-experts-19be">Routing and balancing losses with Mixture of Experts</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion includes feedback on implementation choices, such as the use of DataParallel instead of DDP and the overfitting issue. Commenters appreciate the educational value and the honest documentation of limitations.

**Tags**: `#Mixture-of-Experts`, `#Transformer`, `#PyTorch`, `#LLM`, `#Open Source`

---

<a id="item-10"></a>
## [Debating Fine-Tuning Resistance for Open-Weight LLMs](https://www.reddit.com/r/MachineLearning/comments/1um9bs7/what_does_safe_ai_look_like_d/) ⭐️ 7.0/10

A Reddit discussion questions whether fine-tuning resistance is a meaningful safety goal for open-weight LLMs, given that uncensored variants appear quickly after release. This debate challenges the cost-benefit of safety training for open-weight models and could influence governance and release practices in the AI community. The discussion highlights that determined users can bypass safety measures via fine-tuning, weight modification, or using alternative models, raising questions about the threat model and practical wins.

reddit · r/MachineLearning · /u/Aaron_Rock · Jul 3, 09:07

**Background**: Open-weight LLMs are models with publicly available weights, allowing anyone to fine-tune them. Safety training aims to prevent harmful outputs, but fine-tuning can remove these safeguards. Recent research explores tamper-resistant safeguards, but their effectiveness against determined adversaries remains debated.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2408.00761v4">Tamper-Resistant Safeguards for Open-Weight LLMs</a></li>
<li><a href="https://arxiv.org/html/2508.03153v1">Estimating Worst-Case Frontier Risks of Open-Weight LLMs</a></li>
<li><a href="https://lzwjava.github.io/uncensored-llms-explained-en">Uncensored Large Language Models Explained | Zhiwei Li</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#open-weight models`, `#fine-tuning`, `#LLM`, `#governance`

---

<a id="item-11"></a>
## [FIDE Sanctions Kramnik for Baseless Cheating Accusations](https://www.fide.com/fide-ethics-disciplinary-commission-issues-a-decision-in-case-involving-gm-vladimir-kramnik/) ⭐️ 6.0/10

FIDE's Ethics and Disciplinary Commission has sanctioned former world chess champion Vladimir Kramnik for repeatedly making unfounded cheating accusations against other players, including Daniel Naroditsky and Hikaru Nakamura. This decision sets a precedent for holding prominent figures accountable for online harassment and misuse of statistical arguments, which could deter similar behavior and protect the integrity of online chess. Kramnik's methods of 'detecting' cheating were mathematically questionable, and his public attacks led to significant distress in the community. The sanctions come after a lengthy investigation by FIDE.

hackernews · DarkContinent · Jul 3, 17:04 · [Discussion](https://news.ycombinator.com/item?id=48777266)

**Background**: Cheating in online chess has been a growing concern, with platforms like Chess.com using statistical methods to detect suspicious play. Former champion Vladimir Kramnik began publicly accusing top players of cheating based on his own flawed statistical analyses, sparking widespread debate about statistical literacy and fair play.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/FIDE">FIDE - Wikipedia</a></li>
<li><a href="https://www.chess.com/cheating">Chess Cheating - Our Fair Play System Explained - Chess .com</a></li>
<li><a href="https://www.theatlantic.com/technology/archive/2022/10/hans-niemann-chess-cheating-artificial-intelligence/671799/">A Good Chess Cheater Might Never Be Caught - The Atlantic</a></li>

</ul>
</details>

**Discussion**: The community largely supports the sanction, with many noting that Kramnik's actions caused serious harm, including potential loss of life. Some commenters feel the punishment is too little, too late, and criticize FIDE for not addressing similar issues involving other powerful figures.

**Tags**: `#chess`, `#ethics`, `#statistics`, `#online harassment`

---

<a id="item-12"></a>
## [Factories Are Just Rooms](https://interconnected.org/home/2026/07/03/factories) ⭐️ 6.0/10

A reflective essay argues that factories can be simple rooms, challenging the assumption that manufacturing requires complex infrastructure. This perspective could democratize manufacturing by lowering barriers to entry, encouraging more hands-on work and small-scale production. The essay is published on interconnected.org and tagged with manufacturing, hands-on, engineering, and work-culture.

hackernews · arbesman · Jul 3, 15:13 · [Discussion](https://news.ycombinator.com/item?id=48776035)

**Background**: Traditional manufacturing often involves large factories with expensive machinery. The essay suggests that many products can be made in simpler spaces, similar to a workshop or even a room.

**Discussion**: Commenters share personal experiences: one notes that a machine-builder company operated from a simple room but struggled with business consistency; another fondly recalls running a small factory with hand assembly and custom jigs.

**Tags**: `#manufacturing`, `#hands-on`, `#engineering`, `#work-culture`

---

<a id="item-13"></a>
## [Let AI Coding Assistants Use Their Own Judgment](https://simonwillison.net/2026/Jul/3/judgement/#atom-everything) ⭐️ 6.0/10

Simon Willison shared tips from a fireside chat with the Claude Code team: letting AI coding assistants like Fable use their own judgment for testing and model selection can save tokens and improve efficiency. This practical advice helps developers reduce costs and extend the utility of expensive top-tier AI models by delegating routine tasks to cheaper models, making AI-assisted coding more sustainable. Willison prompted Claude Code with 'For all coding tasks use your judgement to decide an appropriate lower power model and run that in a subagent', which saved a memory file instructing the agent to use Sonnet for substantive implementation and Haiku for trivial edits.

rss · Simon Willison · Jul 3, 18:51

**Background**: Claude Code is Anthropic's AI coding assistant that can autonomously write and edit code. Fable is a higher-tier model with more tokens but higher cost. The tip leverages Claude Code's ability to spawn subagents with different models, allowing the main agent to focus on judgment-intensive tasks while cheaper models handle routine coding.

<details><summary>References</summary>
<ul>
<li><a href="https://support.claude.com/en/articles/11940350-claude-code-model-configuration">Claude Code model configuration | Claude Help Center</a></li>
<li><a href="https://www.eesel.ai/blog/claude-code-model-selection">A practical guide to Claude Code model selection | eesel AI</a></li>
<li><a href="https://claudelab.net/en/articles/claude-code/claude-code-model-selection-opusplan-strategy">Claude Code Model Selection Strategy — Maximize... | Claude Lab</a></li>

</ul>
</details>

**Tags**: `#AI`, `#coding assistants`, `#best practices`, `#Claude Code`

---