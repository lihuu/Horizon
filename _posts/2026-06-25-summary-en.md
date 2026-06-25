---
layout: default
title: "Horizon Summary: 2026-06-25 (EN)"
date: 2026-06-25
lang: en
---

> From 28 items, 19 important content pieces were selected

---

1. [OpenAI unveils first custom AI chip 'Jalapeno' with Broadcom](#item-1) ⭐️ 9.0/10
2. [Qualcomm Acquires AI Startup Modular for $4B](#item-2) ⭐️ 9.0/10
3. [Self-play RL agent tops Generals.io leaderboard](#item-3) ⭐️ 9.0/10
4. [NVIDIA's 45°C Cooling Slashes Data Center Water Use](#item-4) ⭐️ 8.0/10
5. [Nub: A Bun-like all-in-one toolkit for Node.js](#item-5) ⭐️ 8.0/10
6. [Rust Community Pushes to Decouple crates.io from GitHub](#item-6) ⭐️ 8.0/10
7. [LLM-Generated Job Apps Hide Candidates' True Selves](#item-7) ⭐️ 8.0/10
8. [HDD-RoPE: High-Dimensional Dynamic Rotary Positional Embedding](#item-8) ⭐️ 8.0/10
9. [DeepSWE: New Benchmark for Frontier Coding Agents](#item-9) ⭐️ 8.0/10
10. [LLM Inference Pricing Comparison Reveals Surprising Caching Cost Differences](#item-10) ⭐️ 8.0/10
11. [RubyLLM: Unified Ruby Framework for Major AI Providers](#item-11) ⭐️ 7.0/10
12. [Bunny DNS Goes Free: No Query Fees, 500 Domains Included](#item-12) ⭐️ 7.0/10
13. [PR Spam in Open Source Echoes Early Email Spam](#item-13) ⭐️ 7.0/10
14. [Carmack Reflects on Early Mistakes at id Software](#item-14) ⭐️ 7.0/10
15. [Curated OCR Model Hub Launched on Papers with Code](#item-15) ⭐️ 7.0/10
16. [MuJoFil: Open-Source GPU-Native Simulator for Vision RL](#item-16) ⭐️ 7.0/10
17. [Google's Gemini 3.5 Flash Gets Computer Use](#item-17) ⭐️ 6.0/10
18. [Xteink X4 E-Ink Reader Review: Hackable but Tiny](#item-18) ⭐️ 6.0/10
19. [Simon Willison Creates SQLite DB from MDN Browser Compat Data](#item-19) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI unveils first custom AI chip 'Jalapeno' with Broadcom](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI and Broadcom unveiled Jalapeno, OpenAI's first custom AI inference chip, designed and manufactured in collaboration with Broadcom and TSMC, with production achieved in nine months accelerated by OpenAI's own models. This marks a major strategic move for OpenAI to reduce dependence on Nvidia GPUs and optimize inference performance and cost for its own models, potentially reshaping the AI hardware landscape. Jalapeno is an inference-specific processor, not a training chip, and is manufactured by TSMC. OpenAI designed the chip from scratch based on its deep understanding of LLM fundamentals, with Broadcom handling chip implementation, board, and rack system integration.

hackernews · jamdesk · Jun 24, 17:47 · [Discussion](https://news.ycombinator.com/item?id=48663324)

**Background**: AI chips are broadly divided into training chips (e.g., Nvidia GPUs) and inference chips (e.g., Google TPUs). Inference chips are optimized for running trained models efficiently, often as ASICs. OpenAI's move follows Google's long-standing TPU strategy and reflects a trend among AI companies to develop custom silicon for cost and performance gains.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip</a></li>
<li><a href="https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/">OpenAI unveils its first custom chip, built by Broadcom</a></li>
<li><a href="https://investors.broadcom.com/news-releases/news-release-details/openai-and-broadcom-unveil-llm-optimized-intelligence-processor">OpenAI and Broadcom Unveil LLM-Optimized Intelligence ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed curiosity about how OpenAI's models accelerated chip design, with some skepticism that it might be marketing hype. Others discussed the technical merits of inference-specific chips, including ideas like burning weights into ROM for extreme throughput, and noted Google's prescience with TPUs.

**Tags**: `#AI hardware`, `#OpenAI`, `#custom chip`, `#inference`, `#Broadcom`

---

<a id="item-2"></a>
## [Qualcomm Acquires AI Startup Modular for $4B](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 9.0/10

Qualcomm announced the acquisition of Modular, the AI infrastructure startup behind the Mojo programming language, for $4 billion on June 24, 2026. This acquisition signals Qualcomm's major push into AI compute, potentially challenging NVIDIA's dominance in high-performance AI hardware and software stacks. Modular's Mojo language is designed for high-performance AI infrastructure and heterogeneous hardware, and the deal includes Modular's entire team led by Chris Lattner, creator of LLVM and Swift.

hackernews · timmyd · Jun 24, 13:49 · [Discussion](https://news.ycombinator.com/item?id=48659798)

**Background**: Modular develops Mojo, a systems programming language that combines Python-like syntax with C-level performance for AI workloads. Qualcomm, traditionally a mobile chipmaker, has been expanding into AI and RISC-V through acquisitions like Tenstorrent and Ventana.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Mojo_(programming_language)">Mojo (programming language)</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed feelings: some question Qualcomm's ability to compete with NVIDIA in high-end AI, while others see it as a bold strategic move to build a comprehensive AI portfolio. There is also skepticism about Mojo's direction and the irony of Modular being acquired by a hardware company given its founder's past criticisms.

**Tags**: `#acquisition`, `#AI`, `#hardware`, `#Qualcomm`, `#Modular`

---

<a id="item-3"></a>
## [Self-play RL agent tops Generals.io leaderboard](https://www.reddit.com/r/MachineLearning/comments/1uei2yg/i_made_a_superhuman_generalsio_agent_with/) ⭐️ 9.0/10

A self-play reinforcement learning agent using JAX and Vision Transformer achieved #1 on the human 1v1 leaderboard of Generals.io, surpassing top human players. The developer open-sourced the code and published a comprehensive guide detailing the pipeline. This demonstrates that scaling compute and model architecture (Vision Transformer) can outperform human-crafted heuristics in imperfect-information real-time strategy games. The open-source release provides a valuable reference for building similar game AI systems. The agent was reimplemented from NumPy/Torch to JAX for faster simulation, and the CNN was replaced with a Vision Transformer to better capture spatial dependencies. The project includes a fast JAX-based game simulator that can be reused for other imperfect-information RTS environments.

reddit · r/MachineLearning · /u/shrekofspeed · Jun 24, 16:18

**Background**: Generals.io is a real-time strategy game where players control armies to capture enemy generals on a 2D grid, with fog of war creating imperfect information. Self-play reinforcement learning involves an agent training by playing against itself, which has previously achieved superhuman performance in games like Go and Dota 2. JAX is a high-performance numerical computing library that enables efficient GPU/TPU acceleration, and Vision Transformer (ViT) applies transformer architecture to image patches for visual understanding.

<details><summary>References</summary>
<ul>
<li><a href="https://iogameslist.org/generals-io/">Generals.io - .io Games List - Play Online Free Games</a></li>
<li><a href="https://github.com/brunoleej/RL-with-JAX">GitHub - brunoleej/RL-with-JAX: Reinforcement Learning with ...</a></li>
<li><a href="https://pub.aimind.so/playing-pong-with-vision-transformer-dd8818b2ccba">Playing Pong With Vision Transformer | by Dohyeong Kim | AI Mind</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#self-play`, `#game AI`, `#JAX`, `#vision transformer`

---

<a id="item-4"></a>
## [NVIDIA's 45°C Cooling Slashes Data Center Water Use](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 8.0/10

NVIDIA announced a new liquid cooling architecture for AI data centers that operates with coolant temperatures up to 45°C (113°F), enabling near-zero water consumption by eliminating the need for evaporative cooling. This innovation dramatically reduces the environmental impact of AI factories, which are massive water consumers, and opens up the possibility of using waste heat for district heating, turning data centers into community assets. The design uses direct-to-chip liquid cooling with a coolant temperature of up to 45°C, which is higher than traditional liquid cooling systems that typically operate below 30°C. This higher temperature allows for heat rejection without water evaporation, and in favorable climates, the system can run without chillers.

hackernews · nitin_flanker · Jun 24, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48660178)

**Background**: Traditional data centers rely on air cooling or liquid cooling with chillers and cooling towers, which consume large amounts of water for evaporative heat rejection. As AI workloads increase rack densities, liquid cooling becomes essential, but most existing systems still require water for cooling. NVIDIA's approach raises the coolant temperature to a level where waste heat can be reused for district heating, a synergy that has been explored but not widely implemented.

<details><summary>References</summary>
<ul>
<li><a href="https://www.guru3d.com/story/nvidia-unveils-liquid-cooling-design-for-ai-data-centers/">NVIDIA Unveils 45 ° C Liquid Cooling Design for AI Data Centers</a></li>
<li><a href="https://www.techbuzz.ai/articles/nvidia-s-45-c-liquid-cooling-redefines-ai-data-center-energy">NVIDIA's 45 ° C Liquid Cooling Redefines AI Data Center Energy</a></li>
<li><a href="https://www.allthingsdistributed.com/2024/03/district-heating-using-data-centers-to-heat-communities.html">District heating: Using data centers to heat communities | All</a></li>

</ul>
</details>

**Discussion**: Commenters expressed curiosity about the innovation, with some questioning why higher coolant temperatures weren't used before and noting that NASA's Ames facility already uses warm water cooling. Others highlighted the potential for district heating, though concerns were raised about climate dependency and the need for more details on efficiency across different climates.

**Tags**: `#data center cooling`, `#liquid cooling`, `#AI infrastructure`, `#energy efficiency`, `#sustainability`

---

<a id="item-5"></a>
## [Nub: A Bun-like all-in-one toolkit for Node.js](https://github.com/nubjs/nub) ⭐️ 8.0/10

Colin McDonnell released Nub, an all-in-one toolkit that adds transpilation, module resolution, and polyfills to Node.js via preload hooks, running on stock Node without replacing the runtime. Nub brings Bun-like developer experience to Node.js, making it easier to use TypeScript and modern APIs without switching runtimes, which could benefit millions of Node.js developers. Nub uses an oxc-powered transpiler packaged as a Node-API add-on, registers a module resolution hook, and injects polyfills for APIs like Worker and Temporal. It is purely additive and does not modify Node's engine or standard library.

hackernews · colinmcd · Jun 24, 14:14 · [Discussion](https://news.ycombinator.com/item?id=48660267)

**Background**: Bun is an all-in-one JavaScript runtime that includes a transpiler, package manager, and test runner, but switching runtimes can be disruptive. Node.js has native TypeScript support only experimentally, and lacks built-in polyfills for newer APIs. Nub addresses these gaps by augmenting Node.js with preload hooks, providing a similar experience without leaving the Node ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/oxc-project/oxc">GitHub - oxc-project/oxc: ⚓ A collection of high-performance</a></li>
<li><a href="https://nodejs.org/api/addons.html">C++ addons | Node.js v25.7.0 Documentation</a></li>
<li><a href="https://rodneylab.com/temporal-api-time-zones/">Temporal API Time Zones: Convert Times | Rodney Lab</a></li>

</ul>
</details>

**Discussion**: The community reacted positively, with one user migrating their entire monorepo to Nub with zero issues. Some discussed technical nuances like ESM support and the choice of --require over --import, while others noted the author's background as the creator of Zod and former Bun employee.

**Tags**: `#Node.js`, `#tooling`, `#TypeScript`, `#developer-experience`, `#open-source`

---

<a id="item-6"></a>
## [Rust Community Pushes to Decouple crates.io from GitHub](https://infosec.exchange/@mttaggart/116806641273303255) ⭐️ 8.0/10

The Rust community is actively discussing and working on decoupling crates.io from GitHub, with an RFC recently merged and implementation underway. This change reduces supply chain risk by removing a single point of failure, making the Rust ecosystem more resilient and independent of GitHub's infrastructure. The RFC (rust-lang/rfcs#3963) proposes decoupling GitHub account renaming from crates.io usernames, and the official crates.io issue (rust-lang/crates.io#326) outlines the roadmap.

hackernews · speckx · Jun 24, 19:40 · [Discussion](https://news.ycombinator.com/item?id=48664733)

**Background**: Currently, crates.io relies on GitHub for authentication and identity, meaning a GitHub outage or policy change could disrupt Rust package publishing. The Rust project is largely volunteer-driven, making such infrastructure overhauls slow and dependent on funding and reviewer availability.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/rust-lang/rfcs/blob/master/text/3946-crates-io-username-identity.md">3946-crates-io-username-identity.md - GitHub</a></li>

</ul>
</details>

**Discussion**: Community members generally agree on the need for decoupling but acknowledge the difficulty and resource constraints. Some compare with other ecosystems like PHP's Packagist, which enforces source-based packaging, and emphasize constructive hardening over blame.

**Tags**: `#Rust`, `#crates.io`, `#supply chain`, `#open source infrastructure`, `#GitHub`

---

<a id="item-7"></a>
## [LLM-Generated Job Apps Hide Candidates' True Selves](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 8.0/10

Tom MacWright observed that many job applications are now co-written by LLMs, linking to LLM-generated portfolios and GitHub projects with AI-written commit messages, making candidates indistinguishable and impersonal. This trend undermines the authenticity of hiring processes, making it harder for employers to assess candidates' true skills and personalities, and raises ethical concerns about AI misuse in career contexts. MacWright notes that the perfected, generated resume tells nothing about the person except their use of particular tools, effectively creating 'accidental anonymity' where candidates disappear behind AI-generated content.

rss · Simon Willison · Jun 24, 18:13

**Background**: LLMs like GPT-4 can generate text for resumes, cover letters, and even code. While they boost productivity, their use in job applications can mask individual expression. MacWright's commentary highlights a growing concern about authenticity in the AI era.

**Tags**: `#AI`, `#careers`, `#ethics`, `#hiring`, `#LLM`

---

<a id="item-8"></a>
## [HDD-RoPE: High-Dimensional Dynamic Rotary Positional Embedding](https://www.reddit.com/r/MachineLearning/comments/1uelcm9/high_dimensional_dynamic_rotary_positional/) ⭐️ 8.0/10

A new positional embedding method called HDD-RoPE (High-Dimensional, Dynamic Rotary Positional Embedding) has been introduced, which uses cumulative matrix product to create multidimensional, data-dependent rotations. It achieves faster validation loss convergence than xPos on the TinyStories dataset. This advancement could improve the efficiency of transformer models by enabling faster convergence, potentially reducing training time and computational cost. It also introduces a more flexible notion of position that may capture hierarchical structures like paragraphs or sentences. HDD-RoPE breaks query and key vectors into chunks of arbitrary size (e.g., 4) instead of the standard 2, allowing multiple rotational axes. The rotation rates are made data-dependent, meaning the model learns how to advance positions based on layer activations.

reddit · r/MachineLearning · /u/mikayahlevi · Jun 24, 18:16

**Background**: Rotary Position Embedding (RoPE) encodes relative position by rotating pairs of query and key dimensions at fixed rates. xPos extends RoPE with an exponential decay factor for better extrapolation. HDD-RoPE generalizes RoPE by using cumulative matrix products to create high-dimensional, dynamic rotations.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/mikayahlevi/hdd-rope/">GitHub - mikayahlevi/hdd-rope</a></li>
<li><a href="https://shreyashkar-ml.github.io/posts/rope/">A deep-dive into RoPE, and why it matters? | Shreyashkar Lal Sahu</a></li>
<li><a href="https://medium.com/@anitha6g/understanding-rotational-position-embeddings-rope-in-transformers-95d879dd7b4b">Understanding Rotational Position Embeddings (RoPE) in ...</a></li>

</ul>
</details>

**Discussion**: The community discussion includes technical questions about the method's computational overhead and comparisons with other positional embeddings. The author engages actively, acknowledging that HDD-RoPE is slower than xPos or RoPE but emphasizing the convergence benefits.

**Tags**: `#positional embedding`, `#transformer`, `#machine learning`, `#NLP`, `#RoPE`

---

<a id="item-9"></a>
## [DeepSWE: New Benchmark for Frontier Coding Agents](https://www.reddit.com/r/MachineLearning/comments/1ue0hlp/deepswe_new_benchmark_looking_at_how_well_todays/) ⭐️ 8.0/10

DeepSWE is a new open-source benchmark designed to evaluate frontier coding agents on contamination-free, diverse, and real-world software engineering tasks, with tasks written from scratch and hand-written verifiers. This benchmark addresses critical issues like data contamination and lack of real-world complexity in existing benchmarks, providing a more reliable measure of how well AI coding agents perform in actual software engineering work. DeepSWE tasks span 91 repositories across 5 languages, require 5.5x more code than SWE-bench Pro tasks, and use hand-written verifiers that test software behavior rather than implementation details.

reddit · r/MachineLearning · /u/we_are_mammals · Jun 24, 02:03

**Background**: Existing benchmarks like SWE-bench often suffer from data contamination, where models may have seen solutions during pretraining, and lack diversity in tasks. DeepSWE addresses these by creating original tasks and using diverse repositories, ensuring a more accurate evaluation of coding agents' real-world capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE measures frontier coding agents on original, long-horizon...</a></li>
<li><a href="https://deepswe.lol/">DeepSWE — Long-Horizon Software Engineering Benchmark</a></li>
<li><a href="https://scale.com/leaderboard/swe_bench_pro_public">SWE-Bench Pro (Public Dataset)</a></li>

</ul>
</details>

**Discussion**: The Reddit community discussion is not provided, but the post has a high score and active comments, indicating strong interest and likely positive reception from the machine learning community.

**Tags**: `#benchmark`, `#code generation`, `#AI agents`, `#software engineering`, `#open-source`

---

<a id="item-10"></a>
## [LLM Inference Pricing Comparison Reveals Surprising Caching Cost Differences](https://www.reddit.com/r/MachineLearning/comments/1ueavxn/i_compiled_llm_inference_pricing_across_7/) ⭐️ 8.0/10

A Reddit user compiled and compared LLM inference pricing across seven providers, including OpenRouter, DeepSeek, Together AI, Fireworks, and Groq, and found that cached input costs vary dramatically—sometimes tens of times cheaper than cache misses. This comparison highlights that for applications like agents with large system prompts, RAG pipelines, and multi-turn conversations, caching policies can be more important than headline token prices, potentially saving significant costs. The spreadsheet tracks input/output token pricing, context windows, cached input pricing, and supported models, but does not include real throughput, cold-start times, or quantization details. The same model can vary multiple times in cost across providers.

reddit · r/MachineLearning · /u/Technomadlyf · Jun 24, 11:28

**Background**: LLM inference caching stores intermediate results (like KV cache) to avoid recomputing for repeated prompts, reducing latency and cost. Providers offer different caching policies and pricing, which can dramatically affect total cost for applications with reusable context.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.aimactgrow.com/the-full-information-to-inference-caching-in-llms/">The Full Information to Inference Caching in LLMs –</a></li>
<li><a href="https://llm-d.ai/blog/kvcache-wins-you-can-see">KV-Cache Wins You Can See: From Prefix Caching in vLLM to</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-pro">DeepSeek V 4 Pro - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#pricing`, `#caching`, `#inference`, `#providers`

---

<a id="item-11"></a>
## [RubyLLM: Unified Ruby Framework for Major AI Providers](https://rubyllm.com/) ⭐️ 7.0/10

RubyLLM is a new open-source Ruby framework that provides a unified interface for multiple major AI providers, including OpenAI, Anthropic, Google, and xAI, with support for chat, streaming, image generation, and tool calling. This framework simplifies AI integration for Ruby developers, reducing the need to learn multiple provider SDKs, and its active community suggests strong demand for Ruby-native AI tooling. RubyLLM normalizes streaming formats into standardized Chunk objects and maintains a registry of known models, but caching issues with providers like xAI and difficulties with observability instrumentation have been reported by users.

hackernews · doener · Jun 24, 14:41 · [Discussion](https://news.ycombinator.com/item?id=48660711)

**Background**: Ruby developers historically lacked a unified abstraction for LLM APIs, often having to use separate SDKs for each provider. RubyLLM fills this gap by offering a Rails-friendly gem that abstracts provider differences, similar to how Fog abstracts cloud storage providers.

<details><summary>References</summary>
<ul>
<li><a href="https://rubyllm.com/overview/">Overview | RubyLLM</a></li>
<li><a href="https://rubyllm.com/streaming/">Stream Responses | RubyLLM</a></li>
<li><a href="https://mljourney.com/llm-response-caching-how-to-cut-costs-and-latency-in-production/">LLM Response Caching: How to Cut API Costs and Latency with ...</a></li>

</ul>
</details>

**Discussion**: Community members praise RubyLLM's ease of use, comparing it favorably to Vercel's AI framework, but note caching inconsistencies and lack of native responses API support as pain points. Some users also mention difficulties with observability and retry patterns that delete underlying models.

**Tags**: `#Ruby`, `#AI`, `#framework`, `#LLM`, `#open-source`

---

<a id="item-12"></a>
## [Bunny DNS Goes Free: No Query Fees, 500 Domains Included](https://bunny.net/blog/were-making-bunny-dns-free/) ⭐️ 7.0/10

Bunny.net announced that Bunny DNS is now free, eliminating all DNS query fees and offering free DNS hosting for up to 500 domains per account, including features like smart records and health monitoring. This move positions Bunny DNS as a strong EU-based alternative to Cloudflare's DNS services, potentially attracting users concerned about US-EU geopolitics and seeking competitive European tech options. The free tier includes no query limits, no per-request billing, and no critical features hidden behind enterprise plans; however, users like Diti express concern about unexpected charges from other Bunny products, as the billing cap only applies to Bunny CDN.

hackernews · dabinat · Jun 24, 08:50 · [Discussion](https://news.ycombinator.com/item?id=48657030)

**Background**: Bunny.net is a global edge platform offering CDN, security, and compute services. DNS (Domain Name System) translates domain names to IP addresses; authoritative DNS hosting manages the DNS records for a domain. Bunny DNS runs on a dual-stack anycast network supporting IPv4 and IPv6.

<details><summary>References</summary>
<ul>
<li><a href="https://bunny.net/dns/">Bunny DNS | The #1 Scriptable DNS Platform | bunny.net</a></li>
<li><a href="https://docs.bunny.net/dns">Bunny DNS - bunny.net Documentation</a></li>
<li><a href="https://bunny.net/">bunny.net - The Global Edge Platform that truly Hops</a></li>

</ul>
</details>

**Discussion**: Community sentiment is generally positive, with users praising the EU alternative and organic growth approach. However, some express concerns about potential unexpected charges from other Bunny products, as the billing cap only applies to Bunny CDN, not other services.

**Tags**: `#DNS`, `#cloud`, `#free-tier`, `#EU-tech`, `#networking`

---

<a id="item-13"></a>
## [PR Spam in Open Source Echoes Early Email Spam](https://www.greptile.com/blog/prs-on-openclaw) ⭐️ 7.0/10

A blog post by Greptile compares the rising problem of spammy pull requests in open-source projects to the email spam epidemic of the early 2000s, calling for better maintainer tools and community norms. This comparison highlights a systemic threat to open-source sustainability, as spam PRs waste maintainer time and degrade trust, potentially discouraging contributions and harming project health. The article notes that unlike email spam, PR spam targets individual maintainers rather than organizations, making reputation-based filtering harder. GitHub recently introduced configurable PR limits to help mitigate the issue.

hackernews · dakshgupta · Jun 24, 14:32 · [Discussion](https://news.ycombinator.com/item?id=48660579)

**Background**: Pull requests (PRs) are a core mechanism for contributing to open-source projects on platforms like GitHub. Spam PRs are low-quality or automated submissions that waste maintainers' time reviewing and rejecting them. The early 2000s saw a surge in email spam, leading to the development of filters, reputation systems, and laws like CAN-SPAM.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/SSWConsulting/SSW.Rules.Content/wiki/Handling-spam-Pull-Requests">Handling spam Pull Requests · SSWConsulting/SSW.Rules.Content</a></li>

</ul>
</details>

**Discussion**: Commenters proposed solutions including non-textual verification before merging first PRs, token donations to projects, and noted that GitHub's new PR limits are a step forward. Some drew parallels to email spam's reliance on server reputation, which doesn't apply to individual PRs.

**Tags**: `#open-source`, `#spam`, `#maintainer-tools`, `#community`

---

<a id="item-14"></a>
## [Carmack Reflects on Early Mistakes at id Software](https://twitter.com/ID_AA_Carmack/status/2069799283369345247) ⭐️ 7.0/10

John Carmack posted on Twitter reflecting on his early mistakes at id Software, including pushing the team too hard and failing to adapt company culture as the company matured. This reflection from a legendary game developer offers valuable lessons on burnout and company culture, relevant to the entire game development industry and beyond. Carmack specifically mentioned that running people at startup intensity constantly wears them out, and that maturing companies need more slack. The post has high engagement with 469 points and 235 comments.

hackernews · shadowtree · Jun 24, 15:56 · [Discussion](https://news.ycombinator.com/item?id=48661825)

**Background**: John Carmack is a legendary programmer and co-founder of id Software, known for creating groundbreaking games like Doom and Quake. The early days of id Software were marked by intense work culture and rapid innovation, but also led to burnout and departures of key creative talent.

**Discussion**: Commenters generally agreed with Carmack's self-criticism, with some noting that Quake's development gutted the company but was worth it for the game's legacy. Others pointed out that after Doom 2, id Software lost its creative edge as technical achievements outpaced level design.

**Tags**: `#game development`, `#company culture`, `#burnout`, `#leadership`, `#id Software`

---

<a id="item-15"></a>
## [Curated OCR Model Hub Launched on Papers with Code](https://www.reddit.com/r/MachineLearning/comments/1ueiam6/find_the_best_opensource_ocr_models_in_one_place/) ⭐️ 7.0/10

A curated page listing top open-source OCR models with benchmarks has been published on Papers with Code, featuring recent releases from Baidu (Unlimited OCR with R-SWA) and Mistral (OCR 4 API). This resource helps AI practitioners quickly identify the best OCR models for document digitization, which is critical for enabling agentic RAG and other AI agent workflows that require converting messy PDFs into machine-readable Markdown. The page highlights benchmarks like OlmOCRBench and OmniDocBench, and recommends Chandra OCR 2 (open-source, self-hostable) and Mistral OCR v4 (API). Baidu's Unlimited OCR introduces Reference Sliding Window Attention (R-SWA) for efficient long-sequence decoding.

reddit · r/MachineLearning · /u/NielsRogge · Jun 24, 16:26

**Background**: Optical Character Recognition (OCR) converts scanned documents and PDFs into machine-readable text. Agentic RAG (Retrieval-Augmented Generation) uses AI agents to retrieve and generate answers from company data, often requiring OCR to digitize documents. Papers with Code is a platform that tracks machine learning papers, code, and benchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/reference-sliding-window-attention-r-swa">Reference Sliding Window Attention (R-SWA)</a></li>
<li><a href="https://sebastianraschka.com/llms-from-scratch/ch04/06_swa/">SWA Chapter 4 Guide | Sebastian Raschka, PhD</a></li>
<li><a href="https://arxiv.org/abs/2501.00321">[2501.00321] OCRBench v2: An Improved Benchmark for Evaluating</a></li>

</ul>
</details>

**Tags**: `#OCR`, `#open-source`, `#benchmarks`, `#AI agents`, `#document digitization`

---

<a id="item-16"></a>
## [MuJoFil: Open-Source GPU-Native Simulator for Vision RL](https://www.reddit.com/r/MachineLearning/comments/1uemrch/mujoco_derived_simulator_for_high_fidelity_vision/) ⭐️ 7.0/10

A new open-source simulator called MuJoFil combines Nvidia's Newton physics engine with Google's Filament render engine to enable high-fidelity, GPU-accelerated vision-based reinforcement learning training. MuJoFil fills a gap in GPU-accelerated vision-based RL simulation by offering an open-source alternative to proprietary solutions like NVIDIA Isaac, making high-fidelity parallel training more accessible to researchers and developers. MuJoFil supports PBR textures and multiple environment formats (GLB, OpenUSD), and is available via pip as 'mujofil' (CPU) and 'mujofil-warp' (GPU CUDA variant). The project is still in early development with known bugs.

reddit · r/MachineLearning · /u/MT1699 · Jun 24, 19:07

**Background**: MuJoCo is a popular physics simulator for robotics and RL, but its CPU dependency limits parallelization. While MJX offers GPU acceleration, it is not optimized for vision-based pipelines. Nvidia's Isaac ecosystem requires powerful GPUs and a license, reducing accessibility. MuJoFil addresses these limitations by combining open-source GPU-native physics (Newton) and rendering (Filament) engines.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/newton-physics">Newton Physics Engine | NVIDIA Developer</a></li>
<li><a href="https://github.com/google/filament">GitHub - google/filament: Filament is a real-time physically ...</a></li>
<li><a href="https://github.com/newton-physics/newton">GitHub - newton - physics / newton : An open-source, GPU-accelerated...</a></li>

</ul>
</details>

**Tags**: `#reinforcement learning`, `#simulation`, `#GPU`, `#MuJoCo`, `#open-source`

---

<a id="item-17"></a>
## [Google's Gemini 3.5 Flash Gets Computer Use](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/) ⭐️ 6.0/10

Google announced that Gemini 3.5 Flash now supports built-in computer use capabilities, enabling developers to build custom agents that can see, reason, and take actions across browser, mobile, and desktop environments. This move positions Gemini to compete with other AI models offering similar agentic capabilities, but community feedback highlights significant reliability issues and a lack of parity with competitors like OpenAI's Codex and Anthropic's Claude. The computer use feature is built into Gemini 3.5 Flash, allowing it to interact with graphical user interfaces, but users report frequent errors, hallucinations, and an inability to complete simple tasks like extracting data from PDFs.

hackernews · swolpers · Jun 24, 17:21 · [Discussion](https://news.ycombinator.com/item?id=48662999)

**Background**: Large language models (LLMs) like Gemini are increasingly being used for agentic tasks, where they control software interfaces autonomously. However, LLMs are prone to hallucinations and errors, especially when performing multi-step operations. Google's announcement aims to extend Gemini's utility beyond text generation into practical automation.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/">Introducing computer use in Gemini 3 . 5 Flash</a></li>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3 . 5 Flash — Google DeepMind</a></li>
<li><a href="https://9to5google.com/2026/06/24/gemini-chrome-select-screen/">Gemini in Chrome adds ‘Select from screen’ tool</a></li>

</ul>
</details>

**Discussion**: Community comments express frustration with Gemini's reliability, with users reporting that the model gives up on tasks or invents data. Others note the lack of MCP support and coding tools comparable to Codex or Claude Code, and some question the accuracy of Google's benchmark graphs.

**Tags**: `#Gemini`, `#AI`, `#computer use`, `#Google`, `#LLM`

---

<a id="item-18"></a>
## [Xteink X4 E-Ink Reader Review: Hackable but Tiny](https://blog.omgmog.net/post/xteink-x4-e-ink-reader/) ⭐️ 6.0/10

A review of the Xteink X4 E-Ink reader highlights its open nature and hackability, but criticizes its small 4.3-inch screen and lack of backlight. This device shows that a microcontroller-based e-reader can be functional and open, challenging locked-down ecosystems like Kindle, but its small size limits mainstream appeal. The X4 uses a 4.3-inch E-Ink display, weighs 74 grams, and supports USB-C charging and MagSafe attachment. It runs open firmware and allows custom software like CrossPoint.

hackernews · felixdoerp · Jun 24, 16:35 · [Discussion](https://news.ycombinator.com/item?id=48662381)

**Background**: E-readers like Kindle and Kobo use proprietary software and locked-down ecosystems. Open e-readers, such as those based on ESP32, offer hackability and customization but often lack polish. The Xteink X4 is a niche product targeting enthusiasts who value openness over convenience.

<details><summary>References</summary>
<ul>
<li><a href="https://www.xteink.com/products/xteink-x4">Xteink X 4 Pocket eReader</a></li>
<li><a href="https://indianexpress.com/article/technology/gadgets/xteink-x4-ebook-reader-specs-features-price-10405563/">Meet Xteink X 4 , a tiny e - reader that magnetically... - The Indian Express</a></li>

</ul>
</details>

**Discussion**: Commenters generally like the X4 for its portability and hackability, but many note the screen is too small for comfortable reading, especially for older eyes. Some report credit card security concerns with the purchase process.

**Tags**: `#e-reader`, `#hardware`, `#open-source`, `#review`

---

<a id="item-19"></a>
## [Simon Willison Creates SQLite DB from MDN Browser Compat Data](https://simonwillison.net/2026/Jun/24/browser-compat-db/#atom-everything) ⭐️ 6.0/10

Simon Willison created a SQLite database from MDN's browser compatibility data, hosted on GitHub with open CORS headers, and accessible via Datasette Lite. The build process uses a GitHub Actions workflow that force-pushes the database to an orphan branch. This makes browser compatibility data more accessible for querying and integration into tools, lowering the barrier for developers to check feature support across browsers. It demonstrates a practical pattern for distributing SQLite databases via GitHub's CDN with CORS support. The resulting database is approximately 66MB and was built using sqlite-utils with a script generated by Claude Code for web (Opus 4.8). The database is stored on a dedicated 'db' orphan branch to leverage GitHub's CORS headers for direct downloads.

rss · Simon Willison · Jun 24, 23:59

**Background**: MDN Web Docs maintains a comprehensive repository of browser compatibility data (mdn/browser-compat-data) used by developers to check which web features are supported in different browsers. Mozilla recently introduced an MCP server for MDN, which inspired this project. SQLite is a lightweight, file-based database engine, and Datasette Lite is a web-based tool for exploring SQLite databases in the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/mdn/mcp">GitHub - mdn/mcp: MDN's prototype MCP server · GitHub</a></li>
<li><a href="https://sqlite-utils.datasette.io/">sqlite - utils</a></li>

</ul>
</details>

**Tags**: `#browser-compat`, `#sqlite`, `#data-engineering`, `#developer-tools`

---