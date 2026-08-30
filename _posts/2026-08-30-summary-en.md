---
layout: default
title: "Horizon Summary: 2026-08-30 (EN)"
date: 2026-08-30
lang: en
---

> From 35 items, 17 important content pieces were selected

---

1. [Tencent Open-Sources Hy4 Preview, a 770B-Parameter MoE LLM](#item-1) ⭐️ 8.0/10
2. [DHS Uses Obscure 1509 Summons to Secretly Obtain Journalists&\#x27; Records](#item-2) ⭐️ 8.0/10
3. [100-Year-Old SPC Algorithm Beats SOTA Time Series Anomaly Detection on TSB-AD](#item-3) ⭐️ 8.0/10
4. [Tencent compresses Hunyuan 4 preview from 1.5TB to 200GB GGUF, retaining ~98% performance](#item-4) ⭐️ 8.0/10
5. [Terminal Bench 4.0 Released; GLM-5.3 Matches Fable 5 Within Margin of Error](#item-5) ⭐️ 8.0/10
6. [Zod v4.5 introduces schema compilation, boosting validation speed 3-9x](#item-6) ⭐️ 8.0/10
7. [Google&\#x27;s SKILL.state cuts agent token usage 94% by tracking state, not history](#item-7) ⭐️ 8.0/10
8. [Good Culture, Not AI, Is the Real Productivity Hack](#item-8) ⭐️ 7.0/10
9. [GrapheneOS: Pixel 11 Drops Hardware Memory Tagging, a Security Step Backward](#item-9) ⭐️ 7.0/10
10. [Qwen 3.8 27B Runs at 50 tok/s with 100k Context on a 16GB GPU via BeeLlama](#item-10) ⭐️ 7.0/10
11. [Seeing Speculative Decoding at Low Token Rates: MTP and N-Gram Drafting](#item-11) ⭐️ 7.0/10
12. [Illinois legalizes 40 mph e-bikes on streets, with a big catch](#item-12) ⭐️ 6.0/10
13. [llama.cpp Community Compiles Open CPU/RAM/Hybrid Inference PRs](#item-13) ⭐️ 6.0/10
14. [Chinese Open-Source LLMs Close Gap to Anthropic&\#x27;s Opus Level](#item-14) ⭐️ 6.0/10
15. [Developer Builds Go Database Proxy for Fun and Learning](#item-15) ⭐️ 6.0/10
16. [Chinese researchers unveil 600 Wh/kg lithium metal battery, but cycle life lags](#item-16) ⭐️ 6.0/10
17. [Reddit User Finds DC Fast Charging Costlier Than Premium Gas on Road Trip](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Tencent Open-Sources Hy4 Preview, a 770B-Parameter MoE LLM](https://www.tencent.com/tencent-releases-and-open-sources-tencent-hy4-preview/) ⭐️ 8.0/10

Tencent released and open-sourced Hy4 Preview, a text-only mixture-of-experts LLM with 770B total parameters and 49B active parameters. The model quickly gained traction on OpenRouter, processing trillions of tokens within a couple of days. This is significant because a major Chinese tech company is pushing open-weight models toward frontier-level performance, giving developers a powerful, low-cost alternative to proprietary APIs. The rapid OpenRouter adoption shows strong demand for cheap, high-context open models and could intensify competition in the LLM ecosystem. Hy4 Preview supports a 1,024,000-token context window and 64,000-token output, priced at $0.83 per million input tokens and $2.50 per million output tokens, with a 5% cache cost. It is available across 16 providers, and Tencent notes the model participated in optimizing its own training methods and evaluation frameworks, an early recursive self-improvement loop.

hackernews · shenli3514 · Aug 29, 19:33 · [Discussion](https://news.ycombinator.com/item?id=49492632)

**Background**: Hy4 Preview is a mixture-of-experts \(MoE\) model, meaning it activates only a subset of its 770B parameters per token, which keeps inference costs lower than a dense model of similar size. OpenRouter is a unified API marketplace that aggregates hundreds of models from many providers, letting developers switch between them without rewriting code; by May 2026 it processed roughly 25 trillion tokens per week. Tencent&\#x27;s release continues a trend of Chinese labs open-sourcing large models, following similar moves by DeepSeek, Qwen, and others.

<details><summary>References</summary>
<ul>
<li><a href="https://models.dev/models/tencent/hy4-preview/">Hy 4 preview pricing, providers, and specs | Models .dev</a></li>
<li><a href="https://hy.tencent.ai/research/hy4-preview">hy. tencent . ai /research/ hy 4 -preview</a></li>
<li><a href="https://aiwiki.ai/wiki/openrouter">OpenRouter - AI Wiki</a></li>

</ul>
</details>

**Discussion**: Community reactions were mixed: some users highlighted Hy4 Preview&\#x27;s explosive OpenRouter traction and cheaper 5% cache pricing, while one developer reported poor results when using it as a coding agent. Others criticized the benchmark charts in the release as misleading, and another commenter noted the model&\#x27;s recursive self-improvement loop as a notable development.

**Tags**: `#AI`, `#open-source`, `#LLM`, `#Tencent`, `#machine-learning`

---

<a id="item-2"></a>
## [DHS Uses Obscure 1509 Summons to Secretly Obtain Journalists&\#x27; Records](https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits) ⭐️ 8.0/10

The Guardian reports that the Department of Homeland Security has been using administrative subpoenas under 19 U.S.C. § 1509 to secretly obtain phone and communications records from journalists, non-profits, and unions without judicial oversight. In one case, DHS obtained six months of T-Mobile records for a journalist, including logs of more than 10,000 calls and texts, without notifying her until months later. This matters because it reveals an expanding surveillance practice that bypasses the Fourth Amendment&\#x27;s usual warrant requirement, affecting journalists, activists, and civil-society groups. It also shows how companies&\#x27; willingness to comply with administrative subpoenas can determine whether targets ever learn their records were seized. The 1509 summons authority is legally limited to customs and import-related criminal investigations, but DHS has used it more broadly; the DHS Office of Inspector General flagged similar misuse by CBP in 2017 involving a Twitter account. The Guardian notes DHS has repeatedly withdrawn challenged summonses before a judge could rule on their legality, possibly to avoid an adverse precedent.

hackernews · firefax · Aug 29, 18:44 · [Discussion](https://news.ycombinator.com/item?id=49492219)

**Background**: A 1509 summons is an administrative subpoena issued by Customs and Border Protection under 19 U.S.C. § 1509, originally designed to examine books and witnesses in customs enforcement. Unlike a warrant, it does not require approval from a judge, and the recipient can challenge it in court, but many companies comply without contesting it. The DHS OIG previously found CBP misused this authority when it subpoenaed Twitter for information about the @ALT\_USCIS account.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/us-news/2026/aug/29/trump-dhs-1509-summons-records-journalists-nonprofits">Trump’s DHS is using an obscure law to secretly snoop on ...</a></li>
<li><a href="https://www.law.cornell.edu/uscode/text/19/1509">19 U.S. Code § 1509 - Examination of books and witnesses | U.S. Code</a></li>
<li><a href="https://www.oig.dhs.gov/news/press-releases/2017/11162017/dhs-oig-cites-cbp-misuse-summons-power">DHS OIG Cites CBP for Misuse of Summons Power | Office of...</a></li>

</ul>
</details>

**Discussion**: Commenters largely criticized the practice, with some arguing DHS deliberately withdraws challenged summonses to avoid judicial review and that companies that comply without resistance share the blame; one noted that T-Mobile caved while Google did not. Others debated whether a judge in the loop is constitutionally required, and one commenter promoted tmailplus, a self-hosted email tool for journalists who cannot rely on centralized systems. A few comments added political context, noting the differing treatment of tech-industry interests.

**Tags**: `#privacy`, `#surveillance`, `#journalism`, `#civil-liberties`, `#security`

---

<a id="item-3"></a>
## [100-Year-Old SPC Algorithm Beats SOTA Time Series Anomaly Detection on TSB-AD](https://www.reddit.com/r/MachineLearning/comments/1w1wt1s/you_can_beat_sota_time_series_anomaly_detection/) ⭐️ 8.0/10

Eamonn Keogh demonstrated that a simple 100-year-old Statistical Process Control \(SPC\) method achieves perfect results on TSB-AD-M ECG traces and easily solves many &\#x27;TAO&\#x27; traces, outperforming state-of-the-art TSAD methods. He argues the TSB-AD benchmark is too trivial to support meaningful claims about recent algorithms. This critique challenges the validity of a widely used benchmark and suggests much of the last decade&\#x27;s TSAD progress may be illusory. It could push the community to adopt harder benchmarks and rethink how anomaly detection research is evaluated. The post focuses on the TSB-AD-M benchmark by Paparrizos et al., showing that SPC gets perfect results on an ECG trace and that dozens of &\#x27;TAO&\#x27; traces are even more trivial. Keogh notes he has done 90% of the work toward introducing more challenging TSAD problems, including sled dogs, Tuna, fuel cells, and smart manufacturing datasets.

reddit · r/MachineLearning · eamonnkeogh · Aug 29, 20:16

**Background**: Time series anomaly detection \(TSAD\) is a popular research area at venues like NeurIPS, SIGKDD, and VLDB, and many papers evaluate on the TSB-AD benchmark. Statistical Process Control \(SPC\) is a classic quality-control method developed by Walter Shewhart in the 1920s that monitors processes using control charts. Eamonn Keogh is a prominent researcher in time series mining, which gives this critique particular weight.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/TheDatumOrg/TSB-AD">GitHub - thedatumorg/TSB-AD: Time-Series Anomaly Detection ...</a></li>
<li><a href="https://thedatumorg.github.io/TSB-AD/">TSB-AD - thedatumorg.github.io</a></li>
<li><a href="https://qualitysafety.bmj.com/content/early/2026/07/01/bmjqs-2026-020143">Widening of the ‘technical/practical’ divide: New advances in statistical ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with the critique, calling it &\#x27;damning&\#x27; and praising the act of actually checking benchmarks instead of chasing leaderboards. One commenter notes the claim is not new, pointing to a 2020 arXiv paper, while another highlights that Keogh has long tried to draw attention to this issue.

**Tags**: `#time series anomaly detection`, `#benchmarks`, `#statistical process control`, `#machine learning research`, `#TSB-AD`

---

<a id="item-4"></a>
## [Tencent compresses Hunyuan 4 preview from 1.5TB to 200GB GGUF, retaining ~98% performance](https://i.redd.it/lpt5x1t2rbmh1.png) ⭐️ 8.0/10

A Reddit post claims Tencent compressed the Hunyuan 4 preview model from roughly 1.5TB to about 200GB using the GGUF format, while retaining approximately 98% of its original performance. The claim has not been independently verified. If accurate, this would be a dramatic reduction in model size that makes a frontier-scale model far more accessible for local inference on consumer hardware. It also suggests that aggressive quantization may be more viable than many in the local LLM community expected. The compression reportedly uses GGUF, the standard format for quantized local LLMs, and implies roughly an 87% size reduction. The original claim comes from an image posted on Reddit, so details about the quantization method and benchmark methodology remain unclear.

reddit · r/LocalLLaMA · RedditUsr2 · Aug 29, 14:31 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1w1o324/tencent_compressed_hy4preview_from_15tb_to_about/)

**Background**: GGUF is a binary file format created by the llama.cpp team that stores everything an LLM needs to run in a single container, and it is natively supported by tools such as Ollama, LM Studio, and koboldcpp. Quantization works by mapping high-precision weights to lower-precision data types, trading some accuracy for much smaller file sizes and lower memory requirements. Compression methods like this are important because large models such as Hunyuan 4 are otherwise too big to run locally on typical hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GGUF">GGUF - Wikipedia</a></li>
<li><a href="https://imthadhahamed0205.medium.com/what-is-gguf-the-format-powering-local-ai-models-like-llama-and-mistral-9bfb23be7612">What is GGUF ? The Format Powering Local AI Models like... | Medium</a></li>
<li><a href="https://symbl.ai/developers/blog/a-guide-to-quantization-in-llms/">A Guide to Quantization in LLMs | Symbl.ai</a></li>

</ul>
</details>

**Discussion**: Commenters reacted with excitement, with one calling the claim &\#x27;insane&\#x27; and urging others to test it. Another commenter noted the news implies local models can be compressed further and that Hunyuan 4 has not yet been fully post-trained, so its official release could score significantly higher on benchmarks.

**Tags**: `#LLM compression`, `#GGUF`, `#local LLMs`, `#model quantization`, `#Tencent Hunyuan`

---

<a id="item-5"></a>
## [Terminal Bench 4.0 Released; GLM-5.3 Matches Fable 5 Within Margin of Error](https://i.redd.it/49j32fxfk9mh1.png) ⭐️ 8.0/10

Terminal Bench 4.0 has been released, updating the dataset and leaderboard with fixed tasks and removal of saturated tasks. On the new leaderboard, GLM-5.3 scores at the same level as Fable 5 within the margin of error. This matters because benchmark saturation has made many static coding benchmarks lose discriminative power, and Terminal Bench&\#x27;s rapid iteration is an attempt to keep pace with new model releases. The GLM-5.3 result is also notable because it achieves frontier-level performance at a fraction of Fable 5&\#x27;s price, intensifying competition in the coding-agent model market. Terminal Bench 4.0 fixes 19 tasks and removes 8 tasks that were saturated, refusal-prone, publicly solved, or affected by quality and platform issues; the mirrored leaderboard uses 66 professional computer-work tasks with 5 trials per task and an 8-hour agent timeout. Community cost analysis noted that the GLM-5.3 evaluation cost about $2.7k, slightly more than GPT-5.6 Sol&\#x27;s $2.5k, while using nearly twice as many tokens.

reddit · r/LocalLLaMA · SorosAhaverom · Aug 29, 07:17 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1w1fpxi/terminal_bench_40_just_dropped_glm53_is_at_the/)

**Background**: Terminal-Bench is a benchmark designed to measure how well AI agents perform real computer work in a terminal environment, such as coding and system administration tasks. Static benchmarks tend to saturate as frontier models solve nearly all tasks, so Terminal-Bench 4.0 removes saturated tasks and recalibrates task resources to preserve statistical power. GLM-5.3 is an open-weight model from Z.ai, while Fable 5 is part of Anthropic&\#x27;s Claude line; the comparison matters because GLM-5.3 reportedly delivers comparable results at roughly one-tenth of the price.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tbench.ai/news/terminal-bench-4-0">Terminal-Bench 4.0</a></li>
<li><a href="https://benchlm.ai/benchmarks/terminal-bench-4">Terminal-Bench 4.0 Leaderboard &amp; Scores — August 2026</a></li>
<li><a href="https://arxiv.org/html/2602.16763v1">When AI Benchmarks Plateau: A Systematic Study of Benchmark ...</a></li>

</ul>
</details>

**Discussion**: Commenters were impressed by Z.ai&\#x27;s achievement at roughly one-tenth of Fable 5&\#x27;s price, but one argued that Fable 5 is still better on average and that &\#x27;same within margin of error&\#x27; is not how statistics work. Others questioned whether the sharp score jumps are just benchmark saturation, and a cost-focused commenter noted the GLM-5.3 run cost about $2.7k versus $2.5k for GPT-5.6 Sol while using nearly twice as many tokens.

**Tags**: `#LLM evaluation`, `#benchmarks`, `#coding agents`, `#GLM`, `#AI models`

---

<a id="item-6"></a>
## [Zod v4.5 introduces schema compilation, boosting validation speed 3-9x](https://x.com/colinhacks/status/2093725420462182512) ⭐️ 8.0/10

Zod v4.5 adds an optional schema compilation feature that pre-compiles schemas into optimized validation code, delivering 3-9x faster validation. The feature is opt-in rather than enabled by default, and is accessed through a separate import and the new z.compile\(\) API. Zod is one of the most widely used TypeScript validation libraries, so faster validation can reduce runtime overhead in many applications and APIs. This performance improvement is especially relevant for high-throughput services and large schemas, and it may push other validation libraries to adopt similar compilation strategies. The compilation is opt-in, requiring a separate import in every file that uses schemas, which some users find inconvenient. In a community benchmark using valid input with safeParse and consumed results, the third-party zod-compiler was faster on every tested schema, with a median 1.75x speedup over z.compile\(\).

reddit · r/programming · gajus0 · Aug 29, 17:30 · [Discussion](https://www.reddit.com/r/programming/comments/1w1sl70/zod_v45_adds_schema_compilation_39x_faster/)

**Background**: Zod is a TypeScript-first schema declaration and validation library that lets developers define data shapes and validate data at runtime. Traditional Zod validation interprets the schema object on every parse, while schema compilation pre-builds optimized validation logic so repeated parses avoid that overhead. This makes compiled validation similar in spirit to code generation used by some statically typed languages, though it remains an optional step in Zod.

<details><summary>References</summary>
<ul>
<li><a href="https://app.studyraid.com/en/read/11289/352172/understanding-schema-compilation-process">Understand understanding schema compilation process</a></li>

</ul>
</details>

**Discussion**: Community reactions are mostly positive but include notable caveats. One commenter jokes that statically typed languages only need to do this to mimic a fraction of their power, while another compares Zod&\#x27;s new compiler unfavorably with zod-compiler, which is faster on every benchmarked schema. A third commenter questions why compilation is not enabled by default, calling the required extra import in every schema file inconvenient.

**Tags**: `#Zod`, `#TypeScript`, `#Validation`, `#Performance`, `#Schema Compilation`

---

<a id="item-7"></a>
## [Google&\#x27;s SKILL.state cuts agent token usage 94% by tracking state, not history](https://i.redd.it/jsuomguordmh1.jpeg) ⭐️ 8.0/10

Google researchers introduced SKILL.state, a runtime architecture that replaces append-only conversation history with an explicit, mutable execution state. In a 100-step benchmark with Gemini-3-Flash, it achieved 0.94 accuracy using 65k tokens versus 0.91 accuracy and 1.1m tokens for a LangGraph-style stateful baseline — a 94% token reduction. This matters because long-running agents currently pay linearly growing context costs as conversation history accumulates, limiting scalability and raising expenses. A 94% token cut with comparable accuracy could make long-horizon agent deployments far cheaper and influence how agent frameworks design memory and state management. SKILL.state works best when the agent can anticipate which information it will need in future steps; otherwise it must retrieve missing information again. The paper is available on arXiv \(2608.26263\) and was authored by Sanket Badhe and two other researchers.

reddit · r/artificial · hakansan · Aug 29, 21:31 · [Discussion](https://www.reddit.com/r/artificial/comments/1w1ynrf/google_paper_cuts_agent_token_usage_by_94_in_long/)

**Background**: LLM agents typically keep the full conversation history in their input while reasoning, so input size grows with every step and token costs balloon in long sessions. Stateful orchestration frameworks like LangGraph already manage agent state, but often still represent that state as a list of messages. SKILL.state instead stores only a structured representation of the current state plus the latest observation, discarding history as the agent writes useful information into the state.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.26263">[2608.26263] SKILL . state : Scalable Long-Horizon Agent Skills</a></li>
<li><a href="https://www.langchain.com/langgraph">LangGraph: Agent Orchestration Framework for Reliable AI Agents</a></li>
<li><a href="https://docs.langchain.com/oss/python/langgraph/overview">LangGraph overview - Docs by LangChain</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly positive, calling the token reduction &\#x27;huge&\#x27; and noting the real benefit may be deterministic governance over agent prompts. One user asked whether a component converts conversation history into the state model, while another who experimented with similar ideas warned that instruct models can struggle to maintain a custom data structure and suspected the authors tuned or trained a model specifically.

**Tags**: `#AI agents`, `#LLM efficiency`, `#state management`, `#Google research`, `#token optimization`

---

<a id="item-8"></a>
## [Good Culture, Not AI, Is the Real Productivity Hack](https://newsletter.eng-leadership.com/p/good-culture-is-the-biggest-productivity) ⭐️ 7.0/10

An essay on the Eng Leadership newsletter argues that a strong engineering culture drives productivity more than AI tools do. The piece sparked a 47-comment debate among practitioners about how AI interacts with organizational dynamics. As companies rush to adopt AI coding tools, this debate refocuses attention on the human and organizational factors that determine whether AI actually helps. Engineering leaders can use these insights to avoid treating AI as a silver bullet for deeper cultural problems. The article earned a 7/10 score with 222 points on the aggregator, indicating high engagement. Commenters shared contrasting real-world anecdotes, including a demotivating initiative to automate Jira tickets into pull requests and a highly productive 20-person team sustained by low turnover and mutual trust.

hackernews · gpi · Aug 29, 17:19 · [Discussion](https://news.ycombinator.com/item?id=49491568)

**Background**: Engineering culture encompasses the shared values, practices, and social dynamics of a development team, and it strongly influences morale, collaboration, and output. The article sits within a broader industry conversation about whether AI assistants like GitHub Copilot genuinely boost developer productivity or simply amplify existing workflows — for better or worse.

**Discussion**: Commenters largely agreed that culture matters but split on how AI interacts with it. One noted that &\#x27;AI accelerates dysfunction&\#x27; and helps teams reach the wrong destination faster, while another argued AI adoption should be bottom-up and driven by engineers who can assess its real impact. A memorable counterpoint: &\#x27;It&\#x27;s easier to deploy AI than it is to create good culture.&\#x27;

**Tags**: `#engineering-culture`, `#productivity`, `#AI`, `#leadership`, `#team-management`

---

<a id="item-9"></a>
## [GrapheneOS: Pixel 11 Drops Hardware Memory Tagging, a Security Step Backward](https://bsky.app/profile/grapheneos.org/post/3mua32q4ds22e) ⭐️ 7.0/10

GrapheneOS reports that Google&\#x27;s Pixel 11 no longer supports Arm hardware memory tagging \(MTE\), forcing the project to leave its port incomplete. It calls the removal a major security step backward, especially since the device is more expensive with only incremental upgrades. MTE is a key hardware mitigation against memory safety vulnerabilities, which are a leading source of Android security bugs. Dropping it weakens the security baseline for Pixel 11 users and signals a worrying regression in the broader Android ecosystem at a time when memory safety is a priority. MTE, introduced with Armv8.5 and available on devices like the Pixel 8, tags memory allocations to catch use-after-free and buffer-overflow bugs; Android supports SYNC and ASYNC modes. GrapheneOS had completed only a partial port to Pixel 11 because Google removed MTE support, and the device reportedly has reduced RAM for Pro base models, the same underpowered GPU, and higher prices.

hackernews · 400thecat · Aug 29, 15:26 · [Discussion](https://news.ycombinator.com/item?id=49490702)

**Background**: GrapheneOS is an open-source, privacy- and security-focused Android distribution available for Google Pixel devices and future Motorola devices. Arm Memory Tagging Extension \(MTE\) is a hardware feature that tags memory allocations with metadata so the CPU can detect memory corruption such as use-after-free and buffer overflows, which are common in native code and often lead to security vulnerabilities. Google introduced MTE support in Android 13 on select devices, and it has been available on Pixel 8 and later, making its absence on Pixel 11 a notable regression.

<details><summary>References</summary>
<ul>
<li><a href="https://newsroom.arm.com/blog/memory-safety-arm-memory-tagging-extension">Memory Safety: How Arm Memory Tagging Extension Addresses ...</a></li>
<li><a href="https://developer.android.com/ndk/guides/arm-mte">Arm Memory Tagging Extension (MTE) - Android NDK Arm Memory Tagging Extension - Android Open Source Project Delivering enhanced security through Memory Tagging Extension Introduction to Arm Memory Tagging Extensions :: Thore Göbel MTE User Guide for Android OS - ARM architecture family GrapheneOS Unable to Complete Pixel 11 Port Due to Cut ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters are largely critical of Google&\#x27;s Pixel 11 decisions, calling the loss of MTE &quot;appalling&quot; and &quot;terrible,&quot; and some say they have lost respect for the Pixel line. Several users note the Pixel 11 is more expensive with only incremental CPU improvements, reduced RAM on Pro base models, and the same underpowered GPU, with one suggesting waiting for Motorola instead. A Pixel 9 Pro owner feels their purchase was well-timed, citing the Pixel 10&\#x27;s removal of the physical SIM slot and Google&\#x27;s device tree changes.

**Tags**: `#GrapheneOS`, `#Pixel 11`, `#MTE`, `#mobile security`, `#hardware`

---

<a id="item-10"></a>
## [Qwen 3.8 27B Runs at 50 tok/s with 100k Context on a 16GB GPU via BeeLlama](https://www.reddit.com/r/LocalLLaMA/comments/1w1lq7u/qwen_38_27b_at_50_toks_with_100k_context_on_a/) ⭐️ 7.0/10

A Reddit user shared a working setup that runs Qwen 3.8 27B with 100k context at 50 tok/s on an RTX 4070 Ti SUPER 16GB, using a custom IQ4\_XS GGUF quant from jrell and beellama.cpp with kvarn KV cache types. The setup relies on a custom hybrid quantization and KVarN cache to fit multi-token prediction and long context into VRAM. This matters because it demonstrates that a 27B-parameter model with a 100k context window can run at usable speed on consumer 16GB GPUs, pushing local LLM capability beyond what standard llama.cpp builds typically allow. It also highlights the growing ecosystem of performance-focused llama.cpp forks and quantization techniques that make large-context local inference more practical. The setup uses the Qwen3.8-27B-i1-IQ4\_XS-GGUF-Smaller quant from jrell, a Jinja chat template from peculiar-ragdoll to reduce thinking tokens, and beellama.cpp because it supports KVarN KV cache types and a KV cache precision tail. A commenter also reported a similar configuration on an RTX 5080 16GB with 130k context at 50 t/s, using -ngl 67 to free VRAM.

reddit · r/LocalLLaMA · qaf23 · Aug 29, 12:50

**Background**: Qwen 3.8 27B is a large language model that supports multi-token prediction \(MTP\), which can speed up inference by predicting several tokens at once. KV cache stores previous token key/value states during generation, and its size grows with context length, so quantizing it with methods like KVarN helps fit long contexts into limited VRAM. beellama.cpp is a performance-focused llama.cpp fork that adds KVarN, low-bit cache types, and other optimizations for local GGUF inference. The custom IQ4\_XS GGUF quant is designed to fit both MTP and long contexts within a 16GB VRAM budget.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Anbeeld/beellama.cpp">GitHub - Anbeeld/beellama.cpp: KVarN, KV cache precision tail ...</a></li>
<li><a href="https://anbeeld.com/articles/kvarn-kv-cache-implementation-and-benchmarks">KVarN KV Cache: Implementation and Benchmarks - Anbeeld</a></li>
<li><a href="https://arxiv.org/abs/2502.09419">[2502.09419] On multi-token prediction for efficient LLM ... Multi-Token Prediction Tutorial: How To Speed Up LLMs Awesome Multi-Token Prediction (MTP!) - GitHub MTP (Multi-Token Prediction) - vLLM On multi-token prediction for efficient LLM inference - arXiv.org Multi-token-prediction in Gemma 4 - The Keyword How Multi-Token Prediction Makes Local LLMs Faster – Without ...</a></li>

</ul>
</details>

**Discussion**: Commenters were enthusiastic but skeptical, with top comments asking why no one shows benchmark or quality validation for these quants and setups, and questioning real-world usefulness for deep software engineering tasks. Another user shared an alternative RTX 5080 configuration with 130k context at 50 t/s, while others simply asked about output quality.

**Tags**: `#LocalLLaMA`, `#Qwen`, `#GGUF quantization`, `#BeeLlama`, `#GPU inference`

---

<a id="item-11"></a>
## [Seeing Speculative Decoding at Low Token Rates: MTP and N-Gram Drafting](https://www.reddit.com/r/LocalLLaMA/comments/1w1je5d/if_your_ts_is_low_enough_you_can_see_speculative/) ⭐️ 7.0/10

A LocalLLaMA user reports that with a slow MTP-enabled distilled DS4 Pro model running at 2-3 tokens/s, speculative decoding becomes visibly apparent as predictable phrases are written instantly. The post asks whether MTP can be combined with n-gram-based drafting, and commenters point out that TensorRT-LLM already implements n-gram draft models for this purpose. This observation makes an abstract inference optimization tangible for practitioners and highlights how cheap drafting strategies can complement learned drafters. The discussion matters because combining MTP with n-gram drafting could offer near-free speedups for LLM serving, especially for repetitive or code-like text. TensorRT-LLM&\#x27;s n-gram proposer generates drafts without an extra LLM or model heads, and under optimal conditions it nearly doubles tokens per second in NVIDIA&\#x27;s testing. Commenters note that enabling ngram-mod with MTP is practically free but may not provide speedups outside coding workloads, and that n-gram and speculative decoding may have diminishing returns because they target similar predictable token sequences.

reddit · r/LocalLLaMA · zippydazoop · Aug 29, 10:51

**Background**: Speculative decoding speeds up LLM inference by having a small draft model propose several future tokens, which the larger target model then verifies in parallel. Multi-token prediction \(MTP\) trains a model to predict several future tokens at once, and can serve as the drafting mechanism for speculative decoding. N-gram drafting is an even cheaper alternative that retrieves common token sequences from a static table based on recent context, without needing a separate neural draft model.

<details><summary>References</summary>
<ul>
<li><a href="https://nvidia.github.io/TensorRT-LLM/1.1.0rc2.post1/blogs/tech_blog/blog7_NGram_performance_Analysis_And_Auto_Enablement.html">N-Gram Speculative Decoding in TensorRT‑LLM — TensorRT-LLM</a></li>
<li><a href="https://arxiv.org/abs/2404.19737">Better &amp; Faster Large Language Models via Multi-token Prediction Speed-up Gemma 4 with Multi-Token Prediction - ai.google.dev Awesome Multi-Token Prediction (MTP!) - GitHub [2505.17505] L-MTP: Leap Multi-Token Prediction Beyond ... Multi-token-prediction in Gemma 4 - The Keyword Multi-Token Prediction (MTP) | Sebastian Raschka, PhD GitHub - kush-3/mtp-language-model: Multi-token prediction ...</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-speculative-decoding-for-reducing-latency-in-ai-inference/">An Introduction to Speculative Decoding for Reducing Latency ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that combining n-gram drafting with MTP makes sense, citing TensorRT-LLM&\#x27;s existing implementation and its near-doubling of tokens per second under optimal conditions. One user cautions that in practice the speedup is mostly seen in coding workloads, while another wonders whether the two methods have diminishing returns because they both target predictable phrases.

**Tags**: `#speculative decoding`, `#LLM inference`, `#MTP`, `#n-gram`, `#TensorRT-LLM`

---

<a id="item-12"></a>
## [Illinois legalizes 40 mph e-bikes on streets, with a big catch](https://electrek.co/2026/08/29/illinois-just-made-40-mph-e-bikes-street-legal-but-theres-a-huge-catch/) ⭐️ 6.0/10

Illinois has signed a new electric bicycle law that makes 40 mph e-bikes street-legal, creating a legal category for high-speed e-bikes that exceed the standard three-class system. However, the law includes significant caveats that could limit how useful these bikes actually are on the road. This is a notable state-level regulatory shift for high-speed e-bikes, which have been in a legal gray area because they exceed the 28 mph Class 3 limit. It could influence how other states handle the growing market for 35-40 mph electric bikes and affect riders, manufacturers, and transportation policy. The law is described as a sweeping update to Illinois electric bicycle regulations, and it finally addresses the question of what to do with 35-40 mph e-bikes that do not fit the normal three-class system. The exact nature of the &\#x27;huge catch&\#x27; is not specified in the provided excerpt, but it is expected to limit practical street use.

rss · Electrek · Aug 29, 11:54

**Background**: In the U.S., electric bikes are generally divided into three classes based on top speed and throttle type. Class 1 and Class 2 e-bikes top out at 20 mph, with Class 2 adding a throttle, while Class 3 e-bikes are pedal-assist only and top out at 28 mph. Most states use this three-class system, and many also follow a 750-watt motor limit. High-speed e-bikes that exceed 28 mph fall outside these categories, creating legal uncertainty.

<details><summary>References</summary>
<ul>
<li><a href="https://superhumanbikes.com/blogs/news/electric-bike-classes-explained-class-1-2-and-3-2026-guide">Electric Bike Classes Explained: Class 1, 2, and 3 (2026 ...</a></li>
<li><a href="https://thecyclistchoice.com/resources/electric-bike-classes-explained/">Electric Bike Classes Explained (Class 1, 2 &amp; 3 Guide For ...</a></li>

</ul>
</details>

**Tags**: `#e-bikes`, `#legislation`, `#Illinois`, `#micromobility`, `#transportation`

---

<a id="item-13"></a>
## [llama.cpp Community Compiles Open CPU/RAM/Hybrid Inference PRs](https://i.redd.it/tjc2q7ew2dmh1.png) ⭐️ 6.0/10

A Reddit post compiled a list of open llama.cpp pull requests and discussions focused on CPU/RAM/disk and hybrid CPU-GPU inference, including MoE expert caching, AVX-512/VNNI kernels, and streaming experts from disk. The post calls for expert contributions, saying the project is &\#x27;50 PRs away&\#x27; from faster inference by the end of the year. These optimizations could significantly improve local LLM inference on CPU-only and hybrid systems, reducing reliance on expensive VRAM. Merging these PRs would make large MoE models more practical on consumer hardware. The list includes PRs such as \#27402 \(AVX2 large-batch IQ prompt processing\), \#27000 \(Maple 20B-A1B ternary MoE on CPU\), \#27590 and \#26348 \(AVX-512/VNNI dot products for k-quants\), \#25294 \(streaming MoE experts from disk\), and discussion \#24528 \(VRAM caching of hot CPU-resident experts\). One commenter notes llama.cpp has 1433 open PRs, and another contributor highlights adaptive MTP and RDNA performance boosts.

reddit · r/LocalLLaMA · pmttyji · Aug 29, 18:58 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1w1uu6d/llamacpp_open_prs_list_cpuramdiskhybrid_related/)

**Background**: llama.cpp is an open-source C/C++ project for running LLMs locally on CPU, GPU, or hybrid setups, built on the ggml tensor library and supporting quantized formats such as k-quants. Mixture-of-Experts \(MoE\) models activate only a subset of experts per token, so caching frequently used experts in VRAM or streaming them from disk can greatly reduce memory pressure. Quantized formats like TQ1\_0/TQ2\_0 and k-quants trade precision for lower memory and faster compute, and SIMD instructions such as AVX-512 and VNNI accelerate the integer dot products these quantized models depend on. The Maple 20B-A1B model, for example, uses ternary weights so its 20B parameters compress to about 5.3 GB, making CPU inference more feasible.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/ggml-org/llama.cpp/discussions/24528">RFC: MoE expert cache, VRAM caching of hot CPU-resident ...</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/issues/26766">Add support for Maple architecture (20B-A1B ternary MoE ...</a></li>
<li><a href="https://arxiv.org/abs/2504.05897">[2504.05897] HybriMoE: Hybrid CPU-GPU Scheduling and Cache ... HybriMoE: Hybrid CPU-GPU Scheduling and Cache Management for ... HybriMoE: Hybrid CPU-GPU Scheduling and Cache Management for ... Expert Storage and Caching | crafcat7/ncnn-MoE-Runtime | DeepWiki Mixture of Experts VRAM Requirements: 2026... | Lyceum Technology</a></li>

</ul>
</details>

**Discussion**: Commenters expressed both empathy for maintainers—one noting the burden of 1433 open PRs—and enthusiasm for the listed optimizations. A contributor promoted their adaptive MTP PR and a repository of RDNA performance boosts, while another user said they can&\#x27;t wait for VRAM to become obsolete. Overall sentiment is positive but acknowledges the maintainer workload.

**Tags**: `#llama.cpp`, `#CPU inference`, `#performance optimization`, `#local LLM`, `#open source`

---

<a id="item-14"></a>
## [Chinese Open-Source LLMs Close Gap to Anthropic&\#x27;s Opus Level](https://i.redd.it/6q1zwgym2bmh1.png) ⭐️ 6.0/10

A Reddit analysis argues that Chinese open-source models from Qwen and GLM are nearing Anthropic&\#x27;s Opus 4.8 tier, citing Ramp spending data showing only 11% of enterprise spend goes to Anthropic&\#x27;s top model, Fable 5. The post claims open-weight models now surpass Sonnet and threaten proprietary AI business models. If open-weight Chinese models truly match frontier proprietary models, the economics of AI shift from selling tokens to selling compute, benefiting chipmakers like Nvidia and AMD. Enterprises may increasingly choose cheaper open models for routine tasks, pressuring Anthropic and other closed-model vendors. The discussion references Qwen3.8-Max, a 2.4-trillion-parameter open-weights model, and GLM-5.2/5.3, which Z.ai positions between Claude Opus 4.7 and Opus 4.8 on agentic coding tasks. The author warns that rapid model progress is accompanied by increasingly expensive hardware, and predicts long-term winners will be silicon sellers rather than token sellers.

reddit · r/LocalLLaMA · LegacyRemaster · Aug 29, 12:19 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1w1l3a2/how_important_is_it_for_chinese_llms_to_reach_the/)

**Background**: Anthropic&\#x27;s Claude family includes tiered models, with Opus as the high-end tier and Fable as its most powerful and expensive model. Chinese labs such as Alibaba&\#x27;s Qwen and Z.ai&\#x27;s GLM have been releasing open-weights models that increasingly rival these proprietary systems. Ramp&\#x27;s spending data from 70,000 U.S. companies shows that most enterprise spending on Anthropic goes to models other than the top-tier Fable 5, suggesting demand for cheaper, capable alternatives. The Reddit post interprets Anthropic&\#x27;s anti-open-source stance as a defensive business move in this environment.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://z.ai/blog/glm-5.2">GLM-5.2: Built for Long-Horizon Tasks - z.ai</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-5">Introducing Claude Opus 5 \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Commenters were split: one argued that most real-world requests, like answering trivia or generating spreadsheets, do not require a frontier model, so cheaper Chinese models are sufficient. Another said Chinese AI companies need sales teams, while a third dismissed the &\#x27;briefly banned&\#x27; model as a marketing stunt, comparing it to Apple&\#x27;s old publicity tactics.

**Tags**: `#AI`, `#LLMs`, `#open-source`, `#Anthropic`, `#Chinese AI`

---

<a id="item-15"></a>
## [Developer Builds Go Database Proxy for Fun and Learning](https://packagemain.tech/p/golang-database-proxy) ⭐️ 6.0/10

A developer shared their experience coding a database proxy in Go as a fun side project on packagemain.tech. The article explores the design and implementation details of building such a proxy from scratch. Database proxies are critical infrastructure in modern applications, providing connection pooling, read/write splitting, and security features. This deep-dive offers educational value for Go developers and systems programmers who want to understand how such tools work under the hood. The project is presented as an educational exercise rather than a production-ready tool, prioritizing learning over feature completeness. The post focuses on design trade-offs and practical implementation insights, making it most useful for developers interested in Go systems programming.

reddit · r/programming · der\_gopher · Aug 29, 10:01 · [Discussion](https://www.reddit.com/r/programming/comments/1w1iiaw/coding_a_database_proxy_for_fun/)

**Background**: A database proxy is a network service that sits between an application and its database, forwarding requests and providing advanced features such as automatic read/write splitting, transaction splitting, and connection pooling. Writing one from scratch in Go requires handling low-level networking, protocol parsing, and connection lifecycle management, which makes it a challenging but instructive exercise for systems programmers.

<details><summary>References</summary>
<ul>
<li><a href="https://proxysql.com/blog/database-proxies/">The Ultimate Guide to Database Proxies : What... — ProxySQL Blog</a></li>
<li><a href="https://infatica.io/blog/database-proxies/">What Are Database Proxies ? Definition, Use Cases, and Key Benefits</a></li>
<li><a href="https://www.alibabacloud.com/help/en/rds/apsaradb-rds-for-mysql/faq-about-database-proxies">Database proxy FAQ for RDS for MySQL - ApsaraDB RDS - Alibaba...</a></li>

</ul>
</details>

**Tags**: `#Go`, `#database`, `#proxy`, `#tutorial`, `#systems programming`

---

<a id="item-16"></a>
## [Chinese researchers unveil 600 Wh/kg lithium metal battery, but cycle life lags](https://carnewschina.com/2026/08/27/chinese-researchers-unveil-high-stability-lithium-metal-battery-with-energy-density-exceeding-600-wh-kg/) ⭐️ 6.0/10

Chinese researchers have reported a lithium metal battery with energy density exceeding 600 Wh/kg, with one configuration reaching 602 Wh/kg. However, the battery retains only 80% capacity for about 60 cycles at slow charge/discharge rates, far from commercial viability. If scaled successfully, this energy density could roughly double the cell-level energy density of today&\#x27;s EV batteries, potentially extending range or reducing battery weight. But the limited cycle life and low charge rates mean it is unlikely to appear in vehicles for years, if ever. Community commenters cite two configurations: 550 Wh/kg with 80% retention for 180 cycles at 0.1C charge/0.5C discharge, and 602 Wh/kg with 80% retention for 60 cycles at 0.1C charge/discharge. Real-world use would require cycle counts and charge rates at least 30 times higher than these lab results.

reddit · r/electricvehicles · i\_marketing · Aug 29, 03:55 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1w1bz0q/chinese_researchers_unveil_highstability_lithium/)

**Background**: Lithium metal batteries use metallic lithium as the anode, which packs far more lithium into the same space than the carbon anodes used in conventional lithium-ion batteries, giving them very high charge density. Most commercial lithium metal batteries are non-rechargeable primary cells, but rechargeable versions are under active development. The high reactivity of metallic lithium makes stability and cycle life major challenges.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lithium_metal_battery">Lithium metal battery</a></li>
<li><a href="https://www.ihuoba.cn/News/Lithium-rolls-the-dice-on-batteries-21.html">Lithium rolls the dice on batteries -Ihuoba Metals : Aluminum and Steel...</a></li>

</ul>
</details>

**Discussion**: Commenters are skeptical about practical viability: one notes that cycle life and charge rates would need to be at least 30 times higher for real-world use, while another jokes it would be &\#x27;great for single-use drones.&\#x27; A third commenter dismisses the announcement entirely, saying &\#x27;until it&\#x27;s for sale it doesn&\#x27;t exist.&\#x27; Overall sentiment is cautious and grounded, acknowledging the impressive energy density but doubting near-term commercialization.

**Tags**: `#lithium metal battery`, `#energy density`, `#battery research`, `#EV batteries`, `#electrochemistry`

---

<a id="item-17"></a>
## [Reddit User Finds DC Fast Charging Costlier Than Premium Gas on Road Trip](https://www.reddit.com/r/electricvehicles/comments/1w1amco/dcfc_cost_more_than_premium_gas/) ⭐️ 6.0/10

A Reddit user reports that on a road trip, DC fast charging their BEV from 36% to 80% \(50 kWh\) at a Tesla Supercharger cost $27, while their PHEV used about 5 gallons of premium gas costing $25 for a comparable distance. This anecdote highlights that DCFC can be more expensive than premium gasoline per mile on road trips. The comparison matters because public fast charging pricing is a key factor in EV adoption and road-trip economics. If DCFC costs can exceed gasoline, it undercuts one of the main financial arguments for switching to electric vehicles, especially for drivers without home charging. The user paid roughly $0.54/kWh \(27 divided by 50\), which is on the high side; commenters note DCFC prices vary widely, with one paying $0.27/kWh in Texas. The high price partly reflects large upfront capital costs for chargers that see comparatively light use, and membership programs like Tesla&\#x27;s can reduce rates.

reddit · r/electricvehicles · capn\_davey · Aug 29, 02:48

**Background**: DCFC \(DC fast charging\), also called Level 3 charging, bypasses the car&\#x27;s onboard charger by converting AC to DC at the station, allowing a BEV to charge to 80% in roughly 20 minutes to 1 hour. A BEV runs only on battery power, while a PHEV has both a battery and an internal combustion engine, so the PHEV can refuel with gasoline and typically cannot use DC fast chargers. Home Level 2 charging is much cheaper, which is why the user says the BEV is far cheaper for local driving.

<details><summary>References</summary>
<ul>
<li><a href="https://www.transportation.gov/rural/ev/toolkit/ev-basics/charging-speeds">Charger Types and Speeds | US Department of Transportation The Ultimate Guide to DC Fast Charging - Power Sonic DC Fast Chargers and Level 3 High-Speed Charging For EV&#x27;s What Is DC Fast Charging (DCFC)? Complete Guide What is DC Fast Charging? - J.D. Power and Associates</a></li>
<li><a href="https://ev-america.com/bev-vs-phev/">BEV vs PHEV | What’s The Best Electric Car For You? EV vs. BEV vs. PHEV vs. HEV: Key Differences Explained BEV Vs PHEV Vs HEV Battery: What&#x27;s The Difference? BEV, PHEV, HEV, ICE – Confusing electric car terms explained EV (BEV) vs PHEV vs FCEV vs Hybrid: What&#x27;s the Difference? Hybrid vs PHEV vs BEV: 2026 Comparison, Cost, Range &amp; TCO</a></li>
<li><a href="https://jointcharging.com/what-is-a-level-3-dc-fast-charger-2026-guide/">What is a DC fast charger (Level 3 EV Charger)? 2026 Guide</a></li>

</ul>
</details>

**Discussion**: Commenters generally agree that DCFC prices vary widely and that membership programs can make road-trip charging cheaper. Some defend the pricing by pointing to high upfront capital costs and low utilization, while one commenter blames political and grid constraints for high electricity costs. Overall sentiment is that home charging still makes EVs cheaper for most local driving.

**Tags**: `#electric vehicles`, `#DCFC`, `#charging infrastructure`, `#cost comparison`, `#road trip`

---