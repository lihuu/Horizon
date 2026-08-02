---
layout: default
title: "Horizon Summary: 2026-08-02 (EN)"
date: 2026-08-02
lang: en
---

> From 35 items, 24 important content pieces were selected

---

1. [Lean Kernel Soundness Bug Postmortem Details Discovery and Impact](#item-1) ⭐️ 9.0/10
2. [DeepSeek-V4-Flash-0731: local hardware now matches March 2026 frontier intelligence](#item-2) ⭐️ 9.0/10
3. [OpenAI announces ten mathematical breakthroughs with Lean-verified proofs](#item-3) ⭐️ 9.0/10
4. [ByteDance introduces Seedance 2.5 video generation model](#item-4) ⭐️ 8.0/10
5. [Diátaxis Documentation Framework Draws Community Praise on Hacker News](#item-5) ⭐️ 8.0/10
6. [EU AI Act&\#x27;s AI Content Labeling Rules Take Effect August 2](#item-6) ⭐️ 8.0/10
7. [Meituan Releases LongCat-Flash-Lite-Sparse with 1M Token Context](#item-7) ⭐️ 8.0/10
8. [Weight-Aware Streaming Tensor Engine Runs Kimi K3 on 29 GB RAM](#item-8) ⭐️ 8.0/10
9. [Algebraic Data Types as the Bedrock of Software Design](#item-9) ⭐️ 8.0/10
10. [No Starch Press Launches 800-Page Book on 64-Bit Assembly](#item-10) ⭐️ 7.0/10
11. [How Google Helped Kill Widespread RSS Adoption](#item-11) ⭐️ 7.0/10
12. [NetBSD 11.0 Released with MICROVM Kernel and NPF Firewall Upgrades](#item-12) ⭐️ 7.0/10
13. [Ripgrep Musl Binaries Occasionally Segfault During Large Searches](#item-13) ⭐️ 7.0/10
14. [Canada Signs UN Cybercrime Convention, Privacy Advocates Cry Foul](#item-14) ⭐️ 7.0/10
15. [Cursor Accidentally Removed Cost Info from Usage Pages and CSV Export](#item-15) ⭐️ 7.0/10
16. [Mid-Range Local AI Model Releases Spark Community Buzz](#item-16) ⭐️ 7.0/10
17. [Microsoft introduces Flint, a visualization language for AI-driven charts](#item-17) ⭐️ 6.0/10
18. [Greg Brockman: Coworkers&\#x27; ChatGPT Requests Irk People](#item-18) ⭐️ 6.0/10
19. [DeepSeek-V4-Flash Runs at 12.5 tok/s on RTX 3090 via CPU MoE Offload](#item-19) ⭐️ 6.0/10
20. [llama.cpp adds fix for DeepSeek V4 Flash 0731 tool calling](#item-20) ⭐️ 6.0/10
21. [Poolside Releases Updated Laguna S 2.1 FP8 and NVFP4 Checkpoints](#item-21) ⭐️ 6.0/10
22. [Rivian R2 Highway Range Test with All-Terrain Tires: ~230 Miles](#item-22) ⭐️ 6.0/10
23. [Reddit Stock Plunges 23% as AI-Related Changes Hurt User Growth](#item-23) ⭐️ 6.0/10
24. [Judge Denies xAI Request to Pause Minnesota Nudification Ban](#item-24) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Lean Kernel Soundness Bug Postmortem Details Discovery and Impact](https://leodemoura.github.io/blog/2026-8-1-postmortem-for-kernel-soundness-bug-14576/) ⭐️ 9.0/10

A detailed postmortem of Lean kernel soundness bug \#14576 was published, documenting the bug&\#x27;s discovery, practical consequences, and broader implications for formal verification. This matters because soundness bugs in a proof assistant&\#x27;s kernel undermine the core guarantee that every proved theorem is correct, affecting trust in formal verification for critical proofs. The community discussion highlights how such bugs influence perceptions of Lean and other proof systems. Community discussion notes that the practical impact was limited because exploiting the bug required two distinct bugs in two independent kernel implementations, and users relying on independent checking need current versions of both. The postmortem addresses how verification results remain strong but not absolute guarantees.

hackernews · juhopitk · Aug 1, 18:32 · [Discussion](https://news.ycombinator.com/item?id=49137060)

**Background**: Lean is an open-source proof assistant and functional programming language based on the Calculus of Inductive Constructions, initially developed by Leonardo de Moura at Microsoft Research. In a proof assistant, the kernel is the small, trusted code that checks proofs, and soundness means it never accepts an invalid proof. A soundness bug in the kernel could theoretically allow proving false statements, undermining the reliability of all theorems verified in the system.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_%28proof_assistant%29">Lean (proof assistant)</a></li>
<li><a href="https://lawrencecpaulson.github.io/2026/07/30/Collatz.html">Why is it all in the kernel?</a></li>

</ul>
</details>

**Discussion**: Community reactions varied: some viewed the bug as unsurprising and a reminder that formal verification offers strong but not absolute guarantees, while others argued that implementation soundness bugs are a severe drawback and suggested alternative systems like Metamath might be safer. Others mused about the possibility of proving false directly and the implications of AI-generated formalizations.

**Tags**: `#Lean`, `#formal verification`, `#soundness`, `#proof assistants`, `#kernel bug`

---

<a id="item-2"></a>
## [DeepSeek-V4-Flash-0731: local hardware now matches March 2026 frontier intelligence](https://i.redd.it/h09pa8bs3qgh1.png) ⭐️ 9.0/10

DeepSeek released DeepSeek-V4-Flash-0731, an open-weights model that scores 50 on the Artificial Analysis Intelligence Index — nearly matching the 51 score of the top frontier model from March 2026. A Reddit user reports running it locally on hardware costing under $8,000. This marks a major milestone for accessible AI: near-frontier intelligence can now run on local hardware, reducing reliance on cloud APIs and enabling private, low-cost deployment. It could shift how AI is deployed across enterprises and individual developers. The model uses a mixture-of-experts architecture with 284B total parameters and 13B active per token, tuned for fast agentic coding, tool use, reasoning, and high-volume text workloads. The poster&\#x27;s setup includes 128GB of DDR4 RAM and four RTX 5060 Ti GPUs with 64GB total VRAM, and the model is also available via EmpirioLabs and QwenCloud APIs.

reddit · r/LocalLLaMA · joorklee · Aug 1, 08:27 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1vchoua/deepseekv4flash0731_models_you_can_run_locally/)

**Background**: A frontier model is the most advanced AI system available at a given time, typically only accessible via expensive cloud APIs. The Artificial Analysis Intelligence Index is a composite benchmark aggregating nine challenging evaluations across mathematics, science, coding, agentic work, and long-context reasoning. Local LLMs traditionally trailed frontier models, but the gap is narrowing quickly.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-0731">deepseek-ai/ DeepSeek - V 4 - Flash - 0731 · Hugging Face</a></li>
<li><a href="https://empiriolabs.ai/blog/deepseek-v4-flash-0731-api">How to Use DeepSeek V 4 Flash 0731 API | EmpirioLabs AI</a></li>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index</a></li>

</ul>
</details>

**Discussion**: The sparse comments are mostly wallet sympathy — one user jokes about sending &\#x27;thoughts and prayers&\#x27; for the poster&\#x27;s wallet, and another says they are far from being able to run it locally. The overall tone is impressed but aware of the high hardware cost.

**Tags**: `#deepseek`, `#local-llm`, `#ai-models`, `#open-source`, `#hardware`

---

<a id="item-3"></a>
## [OpenAI announces ten mathematical breakthroughs with Lean-verified proofs](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 9.0/10

OpenAI announced that an internal version of its next major model, Astra, produced ten new results in mathematics and theoretical computer science, each formalized as a Lean 4 certificate. Human researchers prepared the manuscripts, and the proofs are publicly available in the openai/ten-proofs GitHub repository. This marks a notable advance in AI-driven theorem proving, showing that a frontier model can produce original, machine-checkable proofs for problems that have been open for at least a decade. It could accelerate mathematical research and reshape how formal verification and AI-assisted discovery are used in academia and industry. OpenAI says the total token cost to find solutions to these problems would be roughly $2,000 at Sol API rates, and it has released a paper and an LLM-generated PDF describing how the proofs came together. The company has not disclosed how many attempted problems did not yield a solution.

reddit · r/artificial · alphacolony21 · Aug 1, 07:45 · [Discussion](https://www.reddit.com/r/artificial/comments/1vcgytq/ten_advances_in_mathematics_and_theoretical/)

**Background**: Lean is an open-source proof assistant and functional programming language built on the Calculus of Inductive Constructions, where users write mathematical statements and proofs that the computer checks for logical correctness. A &\#x27;certificate&\#x27; in this context is a machine-checkable artifact that formally verifies a proof, similar to a primality certificate in number theory. These tools are increasingly important for ensuring the reliability of AI-generated mathematical arguments.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_theorem_prover">Lean theorem prover</a></li>
<li><a href="https://en.wikipedia.org/wiki/Primality_certificate">Primality certificate - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were mostly enthusiastic: one praised the results and the released certificates, another said &\#x27;Accelerate\!&\#x27; in support, while a third jokingly anticipated skeptical takes. The broader reaction seems positive, with curiosity about potential unmentioned failures.

**Tags**: `#AI`, `#mathematics`, `#theorem proving`, `#OpenAI`, `#Lean`

---

<a id="item-4"></a>
## [ByteDance introduces Seedance 2.5 video generation model](https://seed.bytedance.com/en/blog/one-take-creation-flexible-referencing-introducing-seedance-2-5) ⭐️ 8.0/10

ByteDance has unveiled Seedance 2.5, an upgraded video generation model that offers flexible referencing and longer, more controlled generation. It supports single clips up to 30 seconds and up to 50 multimodal references, integrating text, image, video, and audio controls. This release pushes AI video generation toward more coherent, controllable, and production-ready output, potentially impacting filmmakers and content creators. Community discussion highlights it as a serious inflection point for high-quality full-length feature film production using AI technology. Compared with Seedance 2.0, Seedance 2.5 focuses on longer, more controlled generation, with up to 30-second single clips and up to 50 multimodal references. Technical abilities include text/image/video/audio control and &\#x27;one-take&\#x27; creation, though actual access remains unclear and some third-party sites promising access have been flagged as scams.

hackernews · njaremko · Aug 1, 20:45 · [Discussion](https://news.ycombinator.com/item?id=49138302)

**Background**: Seedance is ByteDance&\#x27;s text-to-video model family, first launched in June 2025. The original Seedance 2.0 went viral for creating realistic clips featuring famous actors and characters, raising fascination and concerns about copyright infringement. Seedance 2.5 builds on that foundation with enhanced multimodal referencing and longer generation capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Seedance_2.0">Seedance 2.0</a></li>
<li><a href="https://www.seeddance.io/models/seedance-2-5">Seedance 2 . 5 Free: Try ByteDance AI Video, No Queue, Instant Results</a></li>

</ul>
</details>

**Discussion**: Commenters generally praise the model&\#x27;s quality and coherence, with some stating it is close to overcoming the uncanny valley. Others raise practical concerns about access, noting that many promised Seedance 2 sites turned out to be scams, and some observe the model seems heavily focused on action and high-effect shots rather than dialogue-driven video-to-video generation for filmmakers.

**Tags**: `#AI`, `#video generation`, `#ByteDance`, `#machine learning`, `#text-to-video`

---

<a id="item-5"></a>
## [Diátaxis Documentation Framework Draws Community Praise on Hacker News](https://diataxis.fr/) ⭐️ 8.0/10

A Hacker News post about the Diátaxis documentation framework sparked discussion, with the framework&\#x27;s author Daniele Procida highlighting ongoing translation efforts in the comments. The thread includes strong practical endorsements from a team that used Diátaxis to hand over a large, complex codebase. Diátaxis is a widely recognized framework for organizing technical documentation into tutorials, how-to guides, reference, and explanation. The community validation reinforces its value as a practical tool for software teams, and its structured approach is increasingly relevant as teams use LLMs to generate initial documentation. The framework prescribes four distinct documentation forms that correspond to four different user needs. Daniele Procida is coordinating translations at diataxis.fr/translation, with an in-progress version available on Read the Docs.

hackernews · ryanseys · Aug 1, 20:33 · [Discussion](https://news.ycombinator.com/item?id=49138188)

**Background**: Diátaxis is a documentation framework that helps teams create clear, structured documentation by separating content into four categories: tutorials, how-to guides, technical reference, and explanation. Each type serves a different user need and implies a distinct writing voice and structure. The framework differs from DITA and other approaches because it emphasizes purpose and user needs over topic-based authoring. Its website describes it as &\#x27;a systematic approach to technical documentation authoring.&\#x27;

<details><summary>References</summary>
<ul>
<li><a href="https://diataxis.fr/">Diátaxis</a></li>
<li><a href="https://idratherbewriting.com/blog/what-is-diataxis-documentation-framework">What is Diátaxis and should you be using it with your documentation? | I&#x27;d Rather Be Writing Blog and API doc course</a></li>
<li><a href="https://github.com/evildmp/diataxis-documentation-framework">GitHub - evildmp/diataxis-documentation-framework: A systematic approach to creating better documentation. · GitHub</a></li>

</ul>
</details>

**Discussion**: Commenters were largely positive: rkangel described using Diátaxis for a large codebase handover as &\#x27;fantastic&\#x27; and &\#x27;glorious.&\#x27; Others added practical caveats; conradludgate said it is convenient for prompting LLMs to generate first-pass documentation, while tedd4u noted the topic has been posted many times, linking to a 2024 thread.

**Tags**: `#documentation`, `#technical-writing`, `#software-engineering`, `#framework`

---

<a id="item-6"></a>
## [EU AI Act&\#x27;s AI Content Labeling Rules Take Effect August 2](https://www.reddit.com/r/LocalLLaMA/comments/1vcqpn4/eu_ai_act_takes_effect_tomorrow_august_2_2026/) ⭐️ 8.0/10

The EU AI Act&\#x27;s mandatory transparency obligations for AI-generated content took effect on August 2, 2026, requiring deployers to label synthetic images, audio, video, and text as AI-generated. The rules include exemptions for personal content and evidently artistic, satirical, or fictional works. This is a significant regulatory milestone for AI transparency, affecting developers, platforms, and users operating in the EU. It sets a global precedent for content labeling and is expected to accelerate adoption of technical standards like C2PA and watermarking. The labeling requirement covers images, audio, video, and text produced by AI, but does not apply to users&\#x27; personal content or evidently artistic, satirical, and fictional works. The European Commission has published a Code of Practice and a set of EU icons to support consistent labeling, and compliance can leverage open standards such as C2PA or watermarking techniques.

reddit · r/LocalLLaMA · xoxaxo · Aug 1, 15:44

**Background**: The EU AI Act is a comprehensive regulation that sets rules for AI systems; its transparency provisions require providers and deployers to mark synthetic content to reduce deception and deepfakes. The European Commission has published a Code of Practice on transparency of AI-generated content and a set of EU icons to help stakeholders label their content consistently. For technical implementation, open standards like C2PA \(Coalition for Content Provenance and Authenticity\) provide tamper-evident, cryptographically signed metadata that can record whether AI was involved in creating or editing an asset. Watermarking tools such as SynthID are also used to trace synthetic media.

<details><summary>References</summary>
<ul>
<li><a href="https://digital-strategy.ec.europa.eu/en/policies/code-practice-ai-generated-content">Code of Practice on Transparency of AI-generated Content</a></li>
<li><a href="https://www.ai.cc/news/eu-s-ai-content-labelling-playbook-published/">EU AI Act Content Labelling Requirements: August 2026 ...</a></li>
<li><a href="https://c2pa.org/">C2PA | Verifying Media Content Sources</a></li>

</ul>
</details>

**Discussion**: Two commenters responded to the brief post. One expressed straightforward support, saying the labeling requirement &\#x27;sounds good.&\#x27; Another highlighted exemptions in the rules for personal content and evidently artistic, satirical, and fictional works, quoting a Guardian article. Overall, the discussion reflects cautious approval, with an emphasis on the scope of exemptions.

**Tags**: `#EU AI Act`, `#AI regulation`, `#AI transparency`, `#content labeling`, `#compliance`

---

<a id="item-7"></a>
## [Meituan Releases LongCat-Flash-Lite-Sparse with 1M Token Context](https://huggingface.co/meituan-longcat/LongCat-Flash-Lite-Sparse) ⭐️ 8.0/10

Meituan has released LongCat-Flash-Lite-Sparse, a new model that replaces dense Multi-head Latent Attention \(MLA\) with LongCat Sparse Attention \(LSA\) and natively supports contexts of up to 1M tokens, up from 256k in the original LongCat-Flash-Lite. The weights were added to the Hugging Face repository about an hour ago. This release is significant because it brings native 1M-token context support to an open model while using sparse attention to reduce the quadratic computational cost of standard attention. It strengthens Meituan&\#x27;s position in the long-context LLM space and gives developers a practical option for processing extremely long documents. LongCat-Flash-Lite-Sparse is built on LongCat-Flash-Lite, with the main architectural change being the replacement of dense MLA with LSA. According to Meituan, LSA is an evolution of DeepSeek Sparse Attention \(DSA\), and the model reportedly has around 70B parameters based on community discussion.

reddit · r/LocalLLaMA · LLMFan46 · Aug 1, 15:10 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1vcpv6u/longcatflashlitesparse_is_now_available_for/)

**Background**: Standard transformer attention scales quadratically with sequence length, which becomes a bottleneck for long-context models. Multi-head Latent Attention \(MLA\), introduced in DeepSeek-V2, reduces KV-cache memory during inference. Sparse attention methods, such as LongCat Sparse Attention \(LSA\), compute attention scores only for a subset of input tokens, bringing scaling closer to linear and enabling 1M-token contexts more efficiently.

<details><summary>References</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/07/05/meituan-releases-longcat-2-0-a-1-6t-parameter-open-moe-model-with-native-1m-context-and-longcat-sparse-attention/">Meituan Releases LongCat-2.0: A 1.6T-Parameter Open MoE Model with Native 1M Context and LongCat Sparse Attention - MarkTechPost</a></li>
<li><a href="https://planetbanatt.net/articles/mla.html">Understanding Multi-Head Latent Attention</a></li>
<li><a href="https://www.longcatai.org/">LongCat AI | LongCat-2.0 Trillion-Parameter Agentic Coding Model</a></li>

</ul>
</details>

**Discussion**: Community comments reflect strong interest: one user notes that the 70B parameter count is what the community wanted, another asks how it compares to Qwen3.5-35B, and a third draws a parallel to Qwen3 Coder Next with 80B total and 3 active parameters. Overall sentiment is curious and optimistic, with users focusing on parameter count and comparisons to existing long-context models.

**Tags**: `#sparse-attention`, `#long-context`, `#LLM`, `#HuggingFace`, `#model-release`

---

<a id="item-8"></a>
## [Weight-Aware Streaming Tensor Engine Runs Kimi K3 on 29 GB RAM](https://github.com/sqliteai/waste) ⭐️ 8.0/10

A new Weight-Aware Streaming Tensor Engine \(WASTE\) on GitHub lets users run the Kimi K3 model using only 29 GB of RAM, achieving 0.50 tokens per second by streaming weights from disk. This dramatically lowers the hardware barrier for running large language models, making them accessible on machines without expensive high-RAM setups. It also highlights the growing trend of out-of-core inference where disk and SSD bandwidth trade off against memory capacity. The engine reportedly hits 0.50 tok/s with 29 GB RAM, relying on continuous weight streaming from storage. Community members have asked about the maximum context window and whether the project is a fork of the earlier colibri repository, but the author has not yet clarified these details.

reddit · r/LocalLLaMA · galapag0 · Aug 1, 08:09 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1vche00/weightaware_streaming_tensor_engine_run_kimi_k3/)

**Background**: Weight streaming is an inference optimization that stores model weights in host memory or disk and transfers them to the compute device only when needed, as seen in NVIDIA TensorRT&\#x27;s weight streaming feature. This approach enables running models larger than the device or system memory would normally allow. WASTE applies a similar principle to run Kimi K3, a large language model, on relatively modest RAM.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.nvidia.com/deeplearning/tensorrt/latest/inference-library/weight-streaming.html">Weight Streaming — NVIDIA TensorRT</a></li>
<li><a href="https://docs.pytorch.org/TensorRT/tutorials/_rendered_examples/dynamo/weight_streaming_example.html">Weight Streaming — Torch-TensorRT v2.12.0.dev0+70c6abb documentation</a></li>

</ul>
</details>

**Discussion**: Commenters expressed enthusiasm about potential SSD optimizations, asking whether a dedicated high-bandwidth SSD could outperform stacks of RAM. Others asked about the maximum context window for one-shot overnight tasks and whether the project derives from colibri. Overall sentiment is positive, with practical questions about performance limits.

**Tags**: `#LLM`, `#inference`, `#memory optimization`, `#streaming`, `#local LLM`

---

<a id="item-9"></a>
## [Algebraic Data Types as the Bedrock of Software Design](https://alex.draftist.io/blog/the-bedrock-of-software-design-ycqvcedsj) ⭐️ 8.0/10

A long-drafted blog post argues that algebraic data types \(ADTs\) are the bedrock of software design and that every software engineer should be introduced to them early in their career. The post gained significant community traction on Reddit, scoring 282 points with a 93% upvote ratio. ADTs are a core concept in type theory and functional programming, and this post brings them to a broader audience, potentially influencing how engineers approach data modeling and design. The community discussion adds nuance, debating whether ADTs are truly the foundation or merely a tool for encoding decisions. The post defines algebraic data types as sum types \(OR\) and product types \(AND\), typically used with pattern matching. The author notes the post was drafted years ago and only recently finished, and explicitly states the title is not clickbait.

reddit · r/programming · alex35mil · Aug 1, 11:41 · [Discussion](https://www.reddit.com/r/programming/comments/1vcl5bj/the_bedrock_of_software_design/)

**Background**: Algebraic data types are composite types formed by combining other types: sum types represent a choice between variants \(e.g., a traffic light can be Red, Amber, or Green\), and product types combine multiple values \(e.g., a Point has x and y\). They are common in functional programming languages like Haskell and increasingly appear in mainstream languages such as Rust and TypeScript. Pattern matching allows safe extraction of data from these types.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Algebraic_data_type">Algebraic data type</a></li>
<li><a href="https://jrsinclair.com/articles/2019/algebraic-data-types-what-i-wish-someone-had-explained-about-functional-programming/">Algebraic Data Types: Things I wish someone had explained about functional programming</a></li>

</ul>
</details>

**Discussion**: Commenters generally praised the post, but one top comment \(Bonejob\) argued the title is misleading: the techniques described are about encoding design decisions, not the design itself, which happens earlier via domain analysis. Another comment linked to the influential &\#x27;Parse, don&\#x27;t validate&\#x27; blog post by Alexis King.

**Tags**: `#algebraic-data-types`, `#software-design`, `#programming`, `#types`, `#reddit`

---

<a id="item-10"></a>
## [No Starch Press Launches 800-Page Book on 64-Bit Assembly](https://nostarch.com/art-64-bit-assembly-v2) ⭐️ 7.0/10

No Starch Press announced &\#x27;The Art of 64-bit Assembly&\#x27; \(version 2\), a comprehensive 800-page book on x86-64 assembly programming. The book&\#x27;s release sparked a lively Hacker News discussion about the continuing relevance of assembly language and its tooling. Assembly language remains essential for OS kernels, embedded systems, and performance-critical code, and this book provides a deep, modern resource for x86-64 programmers. The community engagement shows that low-level programming still fascinates and challenges developers, even in an era of high-level languages and AI-assisted development. The book is roughly 800 pages and uses MASM as its primary assembler, a choice that sparked debate about alternative tools like GAS and NASM. Commenters also noted the book&\#x27;s preface contains AI-generated text, and that earlier editions of the book date back decades, covering 16-bit and protected-mode assembly.

hackernews · 0x54MUR41 · Aug 1, 14:09 · [Discussion](https://news.ycombinator.com/item?id=49134599)

**Background**: x86 assembly is a low-level programming language that maps closely to CPU instructions, enabling precise control over hardware. It is used in operating system kernels, device drivers, and real-time embedded systems, and compilers sometimes emit assembly as an intermediate step. On 64-bit x86 \(x86-64\), different platforms use different calling conventions: Linux, macOS, and other Unix-like systems follow the System V AMD64 ABI, while Windows uses its own convention. Assemblers such as MASM, NASM, and GAS translate assembly source code into machine code.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/X86_assembly_language">X86 assembly language</a></li>
<li><a href="https://en.wikipedia.org/wiki/Netwide_Assembler">Netwide Assembler - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/X86_calling_conventions">x86 calling conventions - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was largely meta, with commenters complaining about the book&\#x27;s marketing copy, the choice of MASM, and the presence of AI-generated text in the preface. Some commenters defended learning assembly as still valuable and expressed interest in a Linux-focused equivalent book. One long-time reader noted the author has been updating the book for decades, from 16-bit to protected mode to 64-bit assembly.

**Tags**: `#assembly`, `#x86-64`, `#low-level programming`, `#books`, `#Hacker News`

---

<a id="item-11"></a>
## [How Google Helped Kill Widespread RSS Adoption](https://openrss.org/blog/how-google-helped-destroy-adoption-of-rss-feeds) ⭐️ 7.0/10

An article argues that Google&\#x27;s actions — especially shutting down Google Reader while aggressively pushing Google+ — played a major role in the decline of RSS adoption. The piece frames this as a pivotal moment in the shift away from the open web. This matters because a single company&\#x27;s product decisions can reshape the open web and push users and content toward closed, ad-driven walled gardens. It also informs today&\#x27;s debates about platform power, decentralization, and who controls access to online information. The analysis centers on Google Reader&\#x27;s shutdown, and commenters note that Google&\#x27;s &\#x27;declining usage&\#x27; excuse seemed disingenuous because Google was simultaneously promoting Google+. Others add that Mozilla removed RSS Live Bookmarks in Firefox 64, although some point out RSS is still easy to support and remains useful.

hackernews · pudgywalsh · Aug 1, 18:07 · [Discussion](https://news.ycombinator.com/item?id=49136821)

**Background**: RSS \(Really Simple Syndication\) is a standardized web feed format that allows users and applications to receive updates from websites in a machine-readable way, usually through a news aggregator that monitors sites for new content. A walled garden is a digital ecosystem controlled by one tech company, where apps, content, and data live on that company&\#x27;s systems instead of the open web. Google Reader was once a popular RSS reader, and its shutdown became a symbol of the broader decline of open syndication.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RSS">RSS - Wikipedia</a></li>
<li><a href="https://www.privateinternetaccess.com/blog/walled-garden/">What is a Walled Garden on the Internet?</a></li>

</ul>
</details>

**Discussion**: The discussion is nostalgic and critical: one commenter says the early-2000s internet felt special and that RSS still has no real resource cost to support, while another calls Google&\#x27;s excuse for killing Reader &\#x27;obviously fake&\#x27; because Google+ was being pushed. Several also point to Mozilla removing Firefox Live Bookmarks, and one commenter says Reader&\#x27;s disappearance felt like the beginning of the end of the internet as they knew it.

**Tags**: `#RSS`, `#Google`, `#Open Web`, `#Web History`, `#Google Reader`

---

<a id="item-12"></a>
## [NetBSD 11.0 Released with MICROVM Kernel and NPF Firewall Upgrades](https://blog.netbsd.org/tnf/entry/netbsd_11_0_released) ⭐️ 7.0/10

The NetBSD Project released NetBSD 11.0, adding a new MICROVM kernel configuration for fast booting in QEMU microvm or Firecracker, and improving the NPF firewall with layer 2 and user/group filtering. This is a significant milestone for a long-standing open-source operating system, improving hardware support and opening new use cases for micro-VMs. The fast-booting MICROVM kernel may make NetBSD more attractive for edge services and lightweight virtualized workloads. The MICROVM kernel is a stripped-down configuration with no PCI or ACPI; it uses VirtIO over MMIO and can boot in about 10 ms in QEMU. NPF, NetBSD&\#x27;s BSD-licensed packet filter, gains layer 2 and user/group filtering in this release.

hackernews · jaypatelani · Aug 1, 17:56 · [Discussion](https://news.ycombinator.com/item?id=49136736)

**Background**: NetBSD is a portable, open-source Unix-like operating system known for supporting a wide range of hardware architectures. NPF is NetBSD&\#x27;s stateful packet filter, comparable to iptables or PF, and the new MICROVM kernel is designed for fast-booting virtual machines in lightweight hypervisor environments such as QEMU microvm and Firecracker.

<details><summary>References</summary>
<ul>
<li><a href="https://wiki.netbsd.org/users/imil/microvm/">microvm</a></li>
<li><a href="https://www.phoronix.com/news/smolBSD">smolBSD Builds On The NetBSD-MicroVM Kernel For Booting To Service VMs In Milliseconds - Phoronix</a></li>
<li><a href="https://www.wikiwand.com/EN/NPF_%28firewall%29">NPF ( firewall ) - Wikiwand</a></li>

</ul>
</details>

**Discussion**: Commenters asked about the current status and relevance of the BSDs compared to Linux, and pointed to the official release announcement for more detail. Some welcomed the new NPF filtering features and the ~10 ms MICROVM boot time, while one user wondered whether Wine still works on NetBSD for running Windows-only SDR software.

**Tags**: `#NetBSD`, `#BSD`, `#operating system`, `#release`, `#systems`

---

<a id="item-13"></a>
## [Ripgrep Musl Binaries Occasionally Segfault During Large Searches](https://github.com/BurntSushi/ripgrep/issues/3494) ⭐️ 7.0/10

A GitHub issue reports that ripgrep binaries linked against musl libc can crash with a segmentation fault when performing very large, multithreaded searches. The likely cause is an allocator and concurrency bug in musl&\#x27;s mallocng memory allocator. Ripgrep is a widely used search tool, and musl is the default libc for Alpine Linux and common in static binaries. This bug affects users running large-scale searches on those builds and highlights broader concerns about mallocng&\#x27;s multithreaded correctness and performance. The crash only reproduces with musl, not glibc, pointing to allocator-specific behavior. A Linux kernel developer connected the report to a kernel patch discussion and noted that an AI-generated analysis of the issue, while detailed, was flawed.

hackernews · throwaway2037 · Aug 1, 12:34 · [Discussion](https://news.ycombinator.com/item?id=49133889)

**Background**: musl is a lightweight, standards-conformant C standard library for Linux-based systems, commonly used in Alpine Linux and fully static binaries. mallocng is musl&\#x27;s default memory allocator introduced in version 1.2.0. Memory allocators manage heap memory allocation and freeing; under heavy multithreaded use, allocator contention can cause severe performance degradation and, as in this case, crashes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Musl">musl - Wikipedia</a></li>
<li><a href="https://musl.libc.org/about.html">About musl - libc</a></li>

</ul>
</details>

**Discussion**: Commenters debated whether performance-sensitive tools should replace musl&\#x27;s default allocator, with one noting mallocng is bad at multithreaded contention. Another commenter argued that running ripgrep on HPC cluster filesystems is a workflow design flaw, while others linked to an independent analysis of the underlying kernel bug.

**Tags**: `#ripgrep`, `#musl`, `#segfault`, `#allocator`, `#concurrency`

---

<a id="item-14"></a>
## [Canada Signs UN Cybercrime Convention, Privacy Advocates Cry Foul](https://www.michaelgeist.ca/2026/07/a-surveillance-treaty-in-disguise-the-trouble-with-canadas-quiet-decision-to-sign-the-un-cybercrime-convention/) ⭐️ 7.0/10

Canada quietly signed the UN Cybercrime Convention in July 2026, according to a report by privacy expert Michael Geist. Critics argue the treaty functions more as a surveillance instrument than a genuine cybercrime-fighting agreement. The signing could expand state surveillance powers and set international norms for cross-border data access, affecting Canadian privacy rights and global cybersecurity governance. It also highlights a trend of governments using cybercrime treaties to justify mass surveillance. As of May 2026, 76 participants have signed the treaty, including Australia, the EU, the UK, and now Canada. However, being a signatory has limited impact until the treaty is ratified, and Canada&\#x27;s decision has not yet been formally debated in Parliament.

hackernews · iamnothere · Aug 1, 14:19 · [Discussion](https://news.ycombinator.com/item?id=49134694)

**Background**: The UN Cybercrime Convention is a treaty aimed at strengthening international cooperation against cybercrime, but civil liberties groups worry it lacks strong privacy protections and could enable surveillance. Signing a treaty is a preliminary step that expresses intent, while ratification is the formal approval that makes it legally binding. Michael Geist, a Canadian law professor, has long tracked privacy and digital rights issues.

**Discussion**: Commenters generally appreciate Michael Geist&\#x27;s reporting, with one noting he has been investigating privacy invasions for two decades. Others point out that many other countries, including the EU and UK, have also signed, but emphasize that ratification is the key step that matters. A few dismiss the move as routine, saying &\#x27;Canada signs most UN stuff.&\#x27;

**Tags**: `#privacy`, `#surveillance`, `#cybercrime`, `#Canada`, `#UN`

---

<a id="item-15"></a>
## [Cursor Accidentally Removed Cost Info from Usage Pages and CSV Export](https://forum.cursor.com/t/usage-page-to-token-amount-what/167153) ⭐️ 7.0/10

Cursor accidentally removed dollar-cost information from its usage page and CSV export while cleaning up an old feature flag. An employee confirmed the removal was unintentional and said the CSV export has been fixed, though some users briefly saw a dollar-value usage graph on the page. Developers rely on transparent token and cost reporting to manage spending in AI coding tools, so even a temporary breakdown erodes trust. The incident highlights how cost transparency is becoming a competitive differentiator as agentic coding tools proliferate. According to Cursor employee jonjohnsen, the breakage stemmed from cleaning up an old feature flag, and the CSV export was already restored. He also explained that plan-included usage was shown as dollars, which could be misread as actual on-demand spend, so Cursor removed that confusing graph.

hackernews · EugeneOZ · Aug 1, 15:25 · [Discussion](https://news.ycombinator.com/item?id=49135257)

**Background**: Cursor is an AI coding agent and development environment built by Anysphere that lets developers edit code, search codebases, and complete programming tasks using natural-language instructions. AI tokens are the basic units that models process during inference, and they determine both usage limits and costs for AI services. Since agentic coding tools can consume vastly different token counts for similar tasks depending on the harness and model, developers depend on accurate usage reporting to keep costs predictable.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cursor_%28company%29">Cursor (company) - Wikipedia</a></li>
<li><a href="https://builtin.com/articles/what-is-cursor-ai">What Is Cursor? AI Code Editor Explained | Built In</a></li>
<li><a href="https://iternal.ai/token-usage-guide">Token Usage Guide 2026: How Many Tokens AI Really Uses</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed views: tosh urged developers to measure token efficiency across harnesses, while aroman said he has moved from Cursor to Claude Code and Codex after being a longtime customer. xvxvx mocked token-based pricing sarcastically, and slashdave noted that Cursor’s ease of switching from VS Code also makes it easy to switch back.

**Tags**: `#AI coding tools`, `#Cursor`, `#cost transparency`, `#token usage`, `#developer tools`

---

<a id="item-16"></a>
## [Mid-Range Local AI Model Releases Spark Community Buzz](https://i.redd.it/4nwbkolzcogh1.gif) ⭐️ 7.0/10

A Reddit meme post compiled a wave of notable mid-range local LLM releases from the past week, including Thinking Machines Inkling Small, DeepSeek V4 Flash 0731, Poolside Laguna, and others. The post earned 529 points with a 95% upvote rate, reflecting strong community approval. This release wave highlights how rapidly the local model ecosystem is evolving, with many competitive mid-size options for self-hosting and fine-tuning. A community-vetted list helps developers and hobbyists quickly identify which new models are worth testing on their own hardware. The list includes DeepSeek V4 Flash 0731, a dated snapshot with a mixture-of-experts architecture totaling 284B parameters but only 13B active per token, and Thinking Machines Inkling Small, a sparse MoE model with 12B active parameters. The post was edited to cover releases from the last week and a half, and it explicitly frames these as mid-range model sizes.

reddit · r/LocalLLaMA · Porespellar · Aug 1, 02:29 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1vcav6l/me_worn_out_from_all_the_new_model_drops_this/)

**Background**: Local LLMs refer to open-weight AI models that users run on their own GPUs and hardware rather than through cloud APIs. Mid-range models strike a balance between capability and hardware requirements, making them attractive to enthusiasts with consumer or prosumer graphics cards. Many recent releases use sparse mixture-of-experts designs to achieve strong performance while keeping active parameters—and therefore memory usage—manageable. The pace of such releases has accelerated as both startups and established labs publish open-weights models.

<details><summary>References</summary>
<ul>
<li><a href="https://venturebeat.com/technology/thinking-machines-debuts-inkling-small-open-source-ai-model-nearing-performance-of-predecessor-at-about-1-4-size">Thinking Machines debuts Inkling Small open source AI model nearing performance of predecessor at about 1/4 size | VentureBeat</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash-0731">DeepSeek V 4 Flash 0731 - API Pricing &amp; Benchmarks | OpenRouter</a></li>
<li><a href="https://openrouter.ai/poolside/laguna-m.1:free">Laguna M.1 (free) - API Pricing &amp; Providers | OpenRouter</a></li>

</ul>
</details>

**Discussion**: The top comment joked about having 48GB of VRAM and said &\#x27;these ain&\#x27;t shit,&\#x27; suggesting the models are comparatively small—while also noting how impressive a 27B model is. Another commenter asked which dropped models deserve attention, indicating general enthusiasm but also a desire for more curated guidance.

**Tags**: `#local-llm`, `#model-releases`, `#AI`, `#community`

---

<a id="item-17"></a>
## [Microsoft introduces Flint, a visualization language for AI-driven charts](https://microsoft.github.io/flint-chart/) ⭐️ 6.0/10

Microsoft has introduced Flint, a visualization intermediate language designed to let AI agents reliably create expressive, good-looking charts from simple, human-editable chart specifications. The announcement came with an official blog post and a GitHub repository \(microsoft/flint-chart\). Flint could make AI-generated data visualizations more reliable and token-efficient, since it gives language models a compact intermediate representation instead of forcing them to write backend charting code directly. However, it enters a space already contested by mature grammar-of-graphics systems such as Vega-Lite and ggplot2. Flint is described as a visualization intermediate language: it is human-editable, supports multiple charting backends, and is designed to be simpler than writing a full Vega or Plotly spec. The project&\#x27;s GitHub README emphasizes that AI agents can consistently generate Flint specs that render to polished visualizations.

hackernews · vinhnx · Aug 1, 02:45 · [Discussion](https://news.ycombinator.com/item?id=49130604)

**Background**: Popular charting tools like Vega-Lite and ggplot2 are built on the &\#x27;Grammar of Graphics&\#x27;, a framework that maps data variables to visual channels such as x, y, color, and size. With the rise of LLM-based agents, there is growing interest in intermediate formats that make it easy for models to produce valid charts while remaining readable by humans. Flint fits this trend, offering a layer between natural-language prompts and low-level chart rendering code.

<details><summary>References</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/research/blog/flint-a-visualization-language-for-the-ai-era/">Flint: A visualization language for the AI era - Microsoft Research</a></li>
<li><a href="https://github.com/microsoft/flint-chart">GitHub - microsoft/flint-chart: 🪄 Flint is a visualization language that lets AI agents reliably create expressive, good-looking charts from simple, human-editable chart specs.</a></li>
<li><a href="https://vega.github.io/vega-lite/">A High-Level Grammar of Interactive Graphics | Vega-Lite</a></li>

</ul>
</details>

**Discussion**: Community reaction is mixed. One user reports that direct generation of Vega-Lite specs via an agent allowed more flexibility and higher-quality charts than Flint. Others question the need for a pluggable intermediate language at all, asking why not simply have the AI write the backend code or use Plotly directly; some still prefer ggplot2&\#x27;s API as the best charting grammar.

**Tags**: `#visualization`, `#AI`, `#language design`, `#charting`, `#Microsoft`

---

<a id="item-18"></a>
## [Greg Brockman: Coworkers&\#x27; ChatGPT Requests Irk People](https://simonwillison.net/2026/Aug/1/greg-brockman/#atom-everything) ⭐️ 6.0/10

Greg Brockman, OpenAI&\#x27;s president and co-founder, shared on Twitter that OpenAI employees connect their ChatGPT to Slack, but coworkers dislike being contacted by a colleague&\#x27;s ChatGPT for task help. He notes that the same help is welcomed when requested by the human coworker directly. The comment offers a rare, candid insider view of how AI assistants can create social friction in real workplaces. It suggests that organizations deploying AI agents in collaboration tools must consider the relational and emotional aspects of assistance, not just task efficiency. The observation is anecdotal and comes from a single tweet rather than a formal study. The specific scenario involves ChatGPT integrated into Slack, where an AI bot acts as an intermediary for a help request, changing how the request is perceived.

rss · Simon Willison · Aug 1, 22:29

**Background**: ChatGPT and other large language models are increasingly integrated into workplace tools like Slack to boost productivity, often acting as assistants that can message coworkers. Greg Brockman is a co-founder and president of OpenAI, giving his observations significant weight in discussions of AI&\#x27;s social impact. The broader trend toward proactive AI agents raises questions about how automated interactions affect trust and collaboration among human coworkers.

**Tags**: `#ai-ethics`, `#ai-misuse`, `#generative-ai`, `#openai`, `#ai`

---

<a id="item-19"></a>
## [DeepSeek-V4-Flash Runs at 12.5 tok/s on RTX 3090 via CPU MoE Offload](https://v.redd.it/it101v3pytgh1) ⭐️ 6.0/10

A user replaced the llama.cpp binaries in text-generation-webui with the latest official release and set --n-cpu-moe 39, achieving 12.5 tokens per second on an RTX 3090 24GB with 128GB DDR5. This demonstrates that large Mixture-of-Experts models can run on consumer hardware by offloading most experts to system RAM, pushing the boundaries of local LLM inference. The model requires about 136 GB total, far exceeding the 24 GB VRAM, and only 44 layers are offloaded to the GPU. The key flag --n-cpu-moe 39 keeps 39 of the MoE expert layers in CPU RAM, with performance heavily dependent on CPU and memory bandwidth.

reddit · r/LocalLLaMA · Ok\_Ninja7526 · Aug 1, 21:22 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1vcz61x/deepseekv4flash0731_udiq3_s_125_toks_on_rtx_3090/)

**Background**: DeepSeek-V4-Flash-0731 is a Mixture-of-Experts \(MoE\) model, meaning only a subset of parameters is active per token, making it efficient yet large. Quantization like UD-IQ3\_S compresses weights to fit in memory, while llama.cpp allows running LLMs locally. Offloading expert layers to CPU RAM via --n-cpu-moe enables large models to run on GPUs with limited VRAM.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/oobabooga/textgen/issues/7178">Add option in llama . cpp loader for -- n - cpu - moe · Issue #7178...</a></li>
<li><a href="https://www.theregister.com/software/2025/08/24/how-to-run-llms-on-pc-at-home-using-llamacpp/692544">How to run LLMs on PC at home using Llama . cpp</a></li>
<li><a href="https://shubhamchoudhary05.medium.com/mixture-of-experts-in-large-language-models-the-architecture-powering-next-generation-ai-256153a05b39">Mixture of Experts in Large Language Models : The... | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters question the practicality: one notes that 12 t/s does not justify a $4000 setup, while another suggests bypassing text-generation-webui and running llama-server directly with tuned flags for potential speed gains. Overall sentiment is skeptical but curious about optimization.

**Tags**: `#llama.cpp`, `#DeepSeek`, `#local LLM inference`, `#RTX 3090`, `#quantization`

---

<a id="item-20"></a>
## [llama.cpp adds fix for DeepSeek V4 Flash 0731 tool calling](https://www.reddit.com/r/LocalLLaMA/comments/1vcwaag/fix_for_deep_seek_v4_flash_0731_tool_calling_has/) ⭐️ 6.0/10

A pull request \(PR \#26269\) fixing tool calling for DeepSeek V4 Flash 0731 was merged into llama.cpp about 12 hours ago. Users report that looping and poor behavior issues stopped after applying the fix. This fix improves the reliability of DeepSeek V4 Flash 0731 for local AI users who rely on llama.cpp for agentic workflows involving tool calling. It addresses a specific pain point for a model designed to have enhanced agentic capabilities. DeepSeek V4 Flash 0731 is a sparse mixture-of-experts model with 284B total parameters and 13B active parameters, supporting a 1M token context window. The fix targets tool-calling output that previously looped, and the model itself supersedes the preview version of DeepSeek-V4-Flash.

reddit · r/LocalLLaMA · kwizzle · Aug 1, 19:26

**Background**: llama.cpp is an open-source C++ library that allows running large language models locally on consumer hardware. Tool calling \(also called function calling\) lets an LLM request external actions such as API calls, code execution, or web searches, which is essential for building AI agents. DeepSeek V4 Flash 0731 is a recent model release specifically touted for substantially enhanced agentic capabilities, so a tool-calling bug would seriously hamper its main use case.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-0731">deepseek-ai/DeepSeek-V4-Flash-0731 · Hugging Face</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash-0731">DeepSeek V4 Flash 0731 - API Pricing &amp; Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Discussion**: One community comment expressed approval, noting that with the fix they can now see the model&\#x27;s thinking and tool calls together. Very little other discussion was present.

**Tags**: `#llama.cpp`, `#DeepSeek`, `#tool calling`, `#bug fix`, `#local LLM`

---

<a id="item-21"></a>
## [Poolside Releases Updated Laguna S 2.1 FP8 and NVFP4 Checkpoints](https://huggingface.co/poolside/Laguna-S-2.1-FP8) ⭐️ 6.0/10

Poolside published new FP8 and NVFP4 checkpoints for Laguna S 2.1, increasing the default context length to 1 million tokens and updating the model configs. The update is intended to fix the looping issue that affected the previous checkpoints. This is significant for local LLM practitioners who rely on quantized FP8/NVFP4 checkpoints to run large models on consumer or Blackwell hardware, as it improves stability and expands usable context. It also highlights the fast-paced iteration of small model releases, though the naming choice could cause confusion for third-party API users. NVFP4 is a 4-bit floating-point format \(E2M1\) introduced with NVIDIA&\#x27;s Blackwell architecture, while FP8 uses E4M3 precision with dynamic per-tensor scaling. The updated checkpoints change the actual weights, not just configuration, so users need to re-download them to benefit from the fix.

reddit · r/LocalLLaMA · rmhubbert · Aug 1, 13:20 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1vcn9uw/new_official_weights_for_laguna_s_21_fp8_nvfp4/)

**Background**: Model checkpoints are snapshots of a model&\#x27;s weights saved during training, and quantized checkpoints compress those weights into lower-precision formats such as FP8 or NVFP4 to reduce memory usage and accelerate inference. FP8 can be dynamically quantized from BF16/FP16 models without calibration data, while NVFP4 is designed for Blackwell GPUs to deliver accurate ultra-low-precision inference. This update matters because quantized checkpoints are a common way to run large language models on hardware with limited VRAM.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/v0.5.4/quantization/fp8.html">FP8 — vLLM</a></li>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision ...</a></li>
<li><a href="https://deepchecks.com/glossary/machine-learning-checkpointing/">What is Machine Learning Checkpointing? Deep Learning Models</a></li>

</ul>
</details>

**Discussion**: Commenters welcomed the fix but criticized the lack of versioning; one noted that the updated weights should be named S 2.2 or include a date tag to avoid ambiguity when serving through third-party APIs. Another user said their main issue was thinking not triggering rather than looping, and argued that newer models like DSV4 Flash and Inkling Small are now more compelling alternatives.

**Tags**: `#LLM`, `#HuggingFace`, `#model release`, `#FP8`, `#local LLM`

---

<a id="item-22"></a>
## [Rivian R2 Highway Range Test with All-Terrain Tires: ~230 Miles](https://youtu.be/xskFc4OSEZQ?si=ZwNXQa45CSSxTUxF) ⭐️ 6.0/10

In a 70 mph highway range test, a Rivian R2 with 20-inch all-terrain tires covered 222.7 miles before reaching 1% battery \(roughly 230 miles of usable range\) in 75°F weather with the climate set to 72°F, far short of the EPA&\#x27;s 307-mile combined and 276-mile highway ratings. This real-world test underscores the large effect of all-terrain tires on EV efficiency, offering potential Rivian R2 buyers a concrete reference for range expectations. It also highlights how EPA ratings can overstate real-world highway range, especially with energy-hungry tire setups. The observed efficiency was about 2.7 miles/kWh \(370 Wh/mile\), which is 25% below the EPA combined rating and 17% below the EPA highway rating. Driving conditions were 75°F with the climate at 72°F, even elevation, and a brief downpour at the end; this is a single, non-standardized user test.

reddit · r/electricvehicles · tech01x · Aug 1, 17:29 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1vctbbw/70_mph_highway_range_test_in_my_rivian_r2_all/)

**Background**: The Rivian R2 is a two-row, five-passenger battery-electric mid-size SUV from American automaker Rivian, announced on March 7, 2024 alongside the smaller R3. It is designed as a more compact and affordable alternative to the larger R1S. All-terrain tires are known to reduce EV range because of higher rolling resistance, increased weight, and altered tread patterns compared to highway or street tires. EPA range figures are generated under standardized lab conditions that may not reflect real-world highway speeds or tire choices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rivian_R2">Rivian R2 - Wikipedia</a></li>
<li><a href="https://www.volteum.io/blog/How-far-will-your-EV-go-Understanding-the-factors-affecting-electric-vehicle-range">How far will your EV go? Understanding the factors affecting electric ...</a></li>

</ul>
</details>

**Discussion**: Community commenters generally agreed that all-terrain tires are &\#x27;terrible for range&\#x27; and not surprising. One user shared a detailed data point with the same setup, noting 222.7 miles to 1% battery in ideal conditions and providing efficiency figures. Another commenter suggested that tests would be more useful if they compared two vehicles side by side, one with AT tires and one with OEM highway wheels/tires, to give buyers better configuration guidance.

**Tags**: `#EV`, `#Rivian`, `#range test`, `#all-terrain tires`, `#efficiency`

---

<a id="item-23"></a>
## [Reddit Stock Plunges 23% as AI-Related Changes Hurt User Growth](https://finance.yahoo.com/technology/ai/articles/reddit-stock-collapses-23-ai-200638599.html) ⭐️ 6.0/10

Reddit&\#x27;s stock fell 23% following news that AI-related changes are eroding its user growth. The decline reportedly stems from platform changes, including API restrictions and moderation issues, that are driving users away. This drop signals how AI-driven platform changes and monetization strategies can directly affect user retention and investor confidence. It highlights the tension between Reddit&\#x27;s AI data licensing revenue and the health of its core community. The stock collapse follows Reddit&\#x27;s 2023 API pricing changes that killed many third-party clients, and its controversial licensing of user content for AI training. These moves have fueled community backlash and user migration to alternative platforms.

reddit · r/artificial · esporx · Aug 1, 03:42 · [Discussion](https://www.reddit.com/r/artificial/comments/1vcccnn/reddit_stock_collapses_23_as_ai_eats_away_at_user/)

**Background**: Reddit, a major social news site, relies on user communities for engagement. In 2023, it cut free API access for commercial apps, leading to widespread protests. More recently, it signed multi-year deals to license user data for AI model training, while also restricting access for some AI companies, creating tension between monetization and user trust.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Reddit">Reddit - Wikipedia</a></li>
<li><a href="https://arstechnica.com/ai/2024/02/reddit-has-already-booked-203m-in-revenue-licensing-data-for-ai-training/">Reddit cashes in on AI gold rush with $203M in LLM training ...</a></li>
<li><a href="https://www.metricduck.com/blog/reddit-ai-data-licensing-revenue-legal-risk">Reddit&#x27;s AI Data Licensing: Hidden Revenue and Legal Risk</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration with Reddit&\#x27;s moderation and perceived censorship, with one suggesting AI replacement of moderators to avoid unfair bans. Another questioned whether the API and app restrictions are adequately captured in user growth measurements. Overall sentiment is skeptical of Reddit&\#x27;s direction under AI-related monetization pressure.

**Tags**: `#Reddit`, `#AI`, `#Social Media`, `#Stock Market`, `#User Growth`

---

<a id="item-24"></a>
## [Judge Denies xAI Request to Pause Minnesota Nudification Ban](https://www.nbcnews.com/tech/elon-musk/judge-denies-request-elon-musks-xai-block-mn-nudification-ban-rcna589993) ⭐️ 6.0/10

A federal judge denied xAI&\#x27;s motion to pause Minnesota&\#x27;s nudification ban, allowing the law to take effect on August 1 while the company&\#x27;s lawsuit proceeds. The decision is an early test of how courts handle AI-driven deepfake regulations. This ruling matters because it signals that courts may allow state deepfake laws to be enforced while constitutional challenges are litigated. It also creates uncertainty for AI companies that build image-editing or generation tools, since broad bans could sweep in protected speech like parodies and memes. The Minnesota statute bans nudification features that let users create non-consensual sexually explicit deepfakes. xAI argues the ban is an overbroad, content-based restriction on speech and visual expression; the ACLU has also flagged overbreadth concerns.

reddit · r/artificial · Fcking\_Chuck · Aug 1, 07:23 · [Discussion](https://www.reddit.com/r/artificial/comments/1vcglab/judge_denies_request_by_elon_musks_xai_to_pause/)

**Background**: Nudification apps use artificial intelligence to digitally remove clothing from photos, creating realistic fake nude images without the subject&\#x27;s consent. Minnesota passed a law banning such features in websites and apps, effective August 1, and xAI sued in federal court claiming First Amendment violations. The ban is one of several state efforts targeting deepfakes and AI-generated intimate imagery.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fox9.com/news/nudification-becomes-illegal-websites-apps-minnesota-aug-1-2026">Nudification becomes illegal for websites, apps in Minnesota on Aug. 1 | FOX 9 Minneapolis-St. Paul</a></li>
<li><a href="https://www.cnbc.com/2026/07/28/spacexs-xai-sues-minnesota-over-law-to-ban-nudify-apps-.html">Elon Musk&#x27;s xAI sues Minnesota over law to ban &#x27;nudify&#x27; apps</a></li>
<li><a href="https://parentzone.org.uk/article/what-are-nudification-apps-and-what-do-parents-need-know">What Are ‘ Nudification ’ Apps – and What Do Parents... | Parent Zone</a></li>

</ul>
</details>

**Discussion**: Commenters on the community post largely agreed that the law is too broad. One user called the headline inflammatory, noting that even the ACLU says the statute could cover protected speech like bikini memes of public figures; another urged repealing the law entirely, and a third voiced support.

**Tags**: `#AI regulation`, `#deepfake`, `#legal`, `#xAI`

---