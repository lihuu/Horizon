---
layout: default
title: "Horizon Summary: 2026-05-16 (EN)"
date: 2026-05-16
lang: en
---

> From 44 items, 31 important content pieces were selected

---

1. [0-Click Exploit Chain for Pixel 10 Disclosed](#item-1) ⭐️ 9.0/10
2. [Mitchell Hashimoto warns of 'AI psychosis' in companies](#item-2) ⭐️ 8.0/10
3. [Zulip Transitions to Nonprofit Foundation](#item-3) ⭐️ 8.0/10
4. [California Bill Targets Game Shutdowns: Patches or Refunds](#item-4) ⭐️ 8.0/10
5. [Sigmoids won't save you: Lindy's Law as forecasting default](#item-5) ⭐️ 8.0/10
6. [US DOJ demands Apple and Google unmask 100k+ users of car-tinkering app](#item-6) ⭐️ 8.0/10
7. [ABC News Removes All FiveThirtyEight Articles from Online](#item-7) ⭐️ 8.0/10
8. [OCaml in Space with OxCaml and Stack Annotations](#item-8) ⭐️ 8.0/10
9. [Uber Invests $10B+ in Robotaxi Fleet, Turns on Waymo](#item-9) ⭐️ 8.0/10
10. [arXiv Bans Papers with Unchecked LLM Errors for 1 Year](#item-10) ⭐️ 8.0/10
11. [Fully offline suitcase robot with Jetson Orin NX and Gemma 4 E4B](#item-11) ⭐️ 8.0/10
12. [Orthrus accelerates Qwen3-8B up to 7.8x with diffusion attention](#item-12) ⭐️ 8.0/10
13. [Self-Hosted MCP Server Delivers Real Financial Data to Local LLMs](#item-13) ⭐️ 8.0/10
14. [Intern-S2-Preview: 35B Model Matches Trillion-Scale Performance](#item-14) ⭐️ 8.0/10
15. [ByteDance Releases Cola-DLM: Continuous Latent Diffusion LM](#item-15) ⭐️ 8.0/10
16. [Image-blaster: Turn a single image into a 3D world](#item-16) ⭐️ 7.0/10
17. [Waymo Recalls 3,800 Robotaxis Over Standing Water Glitch](#item-17) ⭐️ 7.0/10
18. [Community Celebrates Jason Scott's Digital Preservation](#item-18) ⭐️ 7.0/10
19. [Radicle: Sovereign code forge built on Git](#item-19) ⭐️ 7.0/10
20. [Tesla Unredacts All 17 Robotaxi Crash Narratives](#item-20) ⭐️ 7.0/10
21. [Dynamic compute allocation with Qwen-35B-A3B nears GPT-5.4 on HLE](#item-21) ⭐️ 7.0/10
22. [Exploring Modded 4090 48GB GPUs for LLM](#item-22) ⭐️ 7.0/10
23. [Google's IDE Evolution: From Custom Tools to VS Code Fork](#item-23) ⭐️ 7.0/10
24. [Bun.sh Ported to Rust via LLM: 1M Lines Generated](#item-24) ⭐️ 7.0/10
25. [Rivian R2 Configurator Goes Live](#item-25) ⭐️ 7.0/10
26. [China Builds Largest Ice-Snow EV Test Base with Indoor Snow](#item-26) ⭐️ 7.0/10
27. [Volvo Stays All-In on Electric and Software-Defined Vehicles](#item-27) ⭐️ 7.0/10
28. [Project Gutenberg Announces Site Improvements](#item-28) ⭐️ 6.0/10
29. [New Book Explores Steve Jobs' NeXT Years](#item-29) ⭐️ 6.0/10
30. [C3 0.8.0 refines builtins, reflection, and unsigned sizes](#item-30) ⭐️ 6.0/10
31. [Chinese EVs Enter Canadian Market, Dealers Excited](#item-31) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [0-Click Exploit Chain for Pixel 10 Disclosed](https://projectzero.google/2026/05/pixel-10-exploit.html) ⭐️ 9.0/10

Google's Project Zero disclosed a 0-click exploit chain for the Pixel 10 that leverages AI-powered message analysis features and a Dolby vulnerability, allowing remote code execution without user interaction. This vulnerability chain underscores the security risks introduced by AI-powered features that pre-process messages, expanding the 0-click attack surface on Android devices. It also demonstrates the importance of rapid patch response, as Google patched the Dolby bug within 90 days. The exploit chain targets a Dolby audio vulnerability (CVE-2025-54957) that existed across all Android until patched in January 2026. Project Zero researchers adapted their previous Pixel 9 exploit to work on Pixel 10, demonstrating the persistence of such attack vectors.

hackernews · happyhardcore · May 15, 13:39 · [Discussion](https://news.ycombinator.com/item?id=48148460)

**Background**: A 0-click exploit is a type of cyberattack that requires no user interaction, such as clicking a link or opening a file, to compromise a device. Project Zero is Google's team of security researchers that finds and discloses zero-day vulnerabilities to improve software security. The Pixel 10 is Google's flagship smartphone running Android.

<details><summary>References</summary>
<ul>
<li><a href="https://projectzero.google/2026/05/pixel-10-exploit.html">A 0-click exploit chain for the Pixel 10: When a Door Closes, a Window ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Project_Zero">Project Zero - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern about the increased attack surface from AI-powered features, with one user noting that reading SMS without user consent is problematic. Others praised Google's quick 90-day patch response, contrasting it with slower responses elsewhere. Some participants discussed the apparent rise in published exploits and questioned Apple's jailbreak landscape.

**Tags**: `#security`, `#exploit`, `#android`, `#pixel`, `#vulnerability`

---

<a id="item-2"></a>
## [Mitchell Hashimoto warns of 'AI psychosis' in companies](https://twitter.com/mitchellh/status/2055380239711457578) ⭐️ 8.0/10

Mitchell Hashimoto, co-founder of HashiCorp, posted a thread warning that many companies are suffering from 'AI psychosis' – blindly trusting AI outputs without critical thinking, leading to unstable systems and poor decisions. As AI-generated code and decisions become more common, this cautionary note from a respected figure highlights the risks of over-reliance on AI without human oversight, potentially preventing costly failures. The tweet referenced a Mastodon post with the same message. Community comments include anecdotes about dangerous database migrations performed by AI prompters and the expectation that AI agents can fix bugs faster than humans.

hackernews · reasonableklout · May 15, 20:26 · [Discussion](https://news.ycombinator.com/item?id=48153379)

**Background**: Mitchell Hashimoto is a well-known software engineer and co-founder of HashiCorp, creator of tools like Vagrant, Terraform, and Consul. 'AI psychosis' is a term used here to describe a state where companies uncritically accept AI outputs, treating AI as an oracle rather than a tool that requires verification. This is part of a broader debate about AI safety and the importance of human oversight in AI-assisted workflows.

**Discussion**: The community largely agrees with the warning, with top comments describing 'AI rescue consulting' as an emerging field and noting that purely AI-written systems may become unstable at scale. Some commenters distinguish between using AI as a tool versus outsourcing thinking, and others argue that the speed of AI agents justifies shipping bugs. Overall, the discussion reinforces the need for critical thinking.

**Tags**: `#AI`, `#software engineering`, `#risk`, `#decision-making`

---

<a id="item-3"></a>
## [Zulip Transitions to Nonprofit Foundation](https://blog.zulip.com/2026/05/15/announcing-zulip-foundation/) ⭐️ 8.0/10

Zulip announced it is transferring ownership to an independent nonprofit foundation, the Zulip Foundation, with its founders stepping back from daily leadership to join Anthropic. This move ensures Zulip's long-term independence and user trust, addressing common concerns about commercial pressure in open-source chat platforms. The Zulip Foundation is structured to serve the public good, and founders along with three senior team members will join Anthropic. The announcement was made on a Friday afternoon, which some see as a low-profile timing.

hackernews · boramalper · May 15, 18:37 · [Discussion](https://news.ycombinator.com/item?id=48152168)

**Background**: Zulip is an open-source team chat application known for its threaded conversation model. Many open-source projects face sustainability and trust issues when controlled by a single company; a foundation structure can help alleviate those concerns.

**Discussion**: Commenters had mixed reactions: some were skeptical about the Friday afternoon timing and possible distraction from other tech news, while others praised Zulip's interface and saw the foundation as a positive step for enterprise adoption. One user noted the announcement coincided with Bun/Rust news.

**Tags**: `#Zulip`, `#open source`, `#nonprofit`, `#foundation`, `#chat`

---

<a id="item-4"></a>
## [California Bill Targets Game Shutdowns: Patches or Refunds](https://arstechnica.com/gaming/2026/05/bill-to-keep-online-games-playable-clears-key-hurdle-in-california/) ⭐️ 8.0/10

A California bill (likely AB 1921) would mandate that when an online game's servers are shut down, the publisher must either release a patch to make the game playable offline or provide refunds to consumers. This legislation addresses growing consumer frustration over games becoming unplayable after servers are taken offline, setting a precedent for digital rights and software ownership. It could force publishers to consider long-term game preservation and consumer protections. The bill exempts games offered solely on a subscription basis. It requires at least 60 days' notice before server shutdown and gives the Attorney General enforcement authority.

hackernews · Lihh27 · May 15, 19:48 · [Discussion](https://news.ycombinator.com/item?id=48152994)

**Background**: Always-online DRM requires a persistent internet connection to play games, meaning when servers shut down, the game becomes unplayable permanently. This has sparked debate about game preservation and consumer rights, as many games are sold as a license rather than owned outright. California is considering legislation to address this issue by requiring publishers to take reasonable steps to keep games functional or compensate buyers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Always-online_DRM">Always-online DRM</a></li>

</ul>
</details>

**Discussion**: Commenters suggested open-sourcing server code as a fair solution, while others worried the bill might accelerate subscription models to bypass regulations. Some questioned the feasibility of enforcement and noted potential unintended consequences.

**Tags**: `#gaming`, `#legislation`, `#digital rights`, `#consumer protection`, `#software as a service`

---

<a id="item-5"></a>
## [Sigmoids won't save you: Lindy's Law as forecasting default](https://www.astralcodexten.com/p/the-sigmoids-wont-save-you) ⭐️ 8.0/10

An article argues that relying on sigmoid curves for technology trends is misguided, proposing Lindy's Law as a better default assumption, and criticizes overconfident predictions about AI progress. This piece challenges common forecasting methods in technology and AI, potentially shifting how analysts think about timelines and reducing unwarranted optimism. The author has publicly predicted AGI within 1-2 years, which may influence his advocacy for Lindy's Law. Lindy's Law states that the future life expectancy of non-perishable things (like technologies) is proportional to their current age.

hackernews · Tomte · May 15, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48147021)

**Background**: A sigmoid curve (S-curve) describes slow initial growth, rapid acceleration, then leveling off as limits are reached. It is often used for technology adoption and progress. Lindy's Law is a heuristic suggesting that older technologies or ideas tend to have longer remaining lifespans. The article argues that when we don't know fundamental limits, Lindy's Law is a more robust default than assuming a sigmoid will soon plateau.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lindy_effect">Lindy effect - Wikipedia</a></li>
<li><a href="https://lawsofsoftwareengineering.com/laws/lindy-effect/">The Lindy Effect - Laws of Software Engineering</a></li>

</ul>
</details>

**Discussion**: Commenters noted the article ignores its own initial answer about different technology generations; one pointed out the author's personal stake in Lindy's Law due to his AGI prediction. Others praised Lindy's Law as a gem, while some questioned whether AI scaling truly measures intelligence.

**Tags**: `#trend analysis`, `#AI predictions`, `#Lindy's Law`, `#sigmoid curves`, `#technology forecasting`

---

<a id="item-6"></a>
## [US DOJ demands Apple and Google unmask 100k+ users of car-tinkering app](https://macdailynews.com/2026/05/15/u-s-doj-demands-apple-and-google-unmask-over-100000-users-of-popular-car-tinkering-app-in-emissions-crackdown/) ⭐️ 8.0/10

The U.S. Department of Justice has issued subpoenas to Apple and Google demanding the identities of over 100,000 users of a car-tinkering app used to modify vehicle emissions controls. This action is part of a broader crackdown on emissions cheating devices. This case raises significant privacy concerns and sets a precedent for government surveillance of app users, potentially impacting millions who use customization tools. It also highlights the tension between environmental regulation and individual rights. The app is reportedly used to disable or modify emissions control systems, known as defeat devices, which are illegal under the Clean Air Act. The DOJ seeks user data to identify potential witnesses in an investigation into emissions cheating.

hackernews · tencentshill · May 15, 17:28 · [Discussion](https://news.ycombinator.com/item?id=48151383)

**Background**: A defeat device is any hardware or software that interferes with emissions controls under real-world driving conditions but allows the vehicle to pass formal tests. Such devices have been the subject of major scandals, like Volkswagen's dieselgate. Apps that enable ECU tuning can be used legally for performance enhancement but also illegally to defeat emissions systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Defeat_device">Defeat device - Wikipedia</a></li>
<li><a href="https://www.cbsnews.com/news/justice-department-auto-emissions-cheating-cases/">Justice Dept. kills cases cracking down on auto emissions cheating ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed opinions: some criticized the government's approach as overreach, while others condemned the app's misuse for 'rolling coal'. Concerns were raised about the precedent for car manufacturers to use such data to target users who disable tracking, and the centralization of app distribution was highlighted as a vulnerability.

**Tags**: `#privacy`, `#government surveillance`, `#digital rights`, `#car emissions`

---

<a id="item-7"></a>
## [ABC News Removes All FiveThirtyEight Articles from Online](https://twitter.com/baseballot/status/2055309076209492208) ⭐️ 8.0/10

ABC News has taken down the entire archive of FiveThirtyEight articles from its website, effectively erasing years of data journalism content. This move eliminates a prominent source of data-driven journalism on politics, sports, and science, and raises concerns about the preservation of digital journalism and corporate brand mismanagement. Nate Silver, FiveThirtyEight's founder, revealed that ABC refused to sell back the IP because they disliked his criticism of their brand management. The removal includes award-winning interactive visualizations and data stories.

hackernews · cmsparks · May 15, 19:07 · [Discussion](https://news.ycombinator.com/item?id=48152553)

**Background**: FiveThirtyEight was a data journalism website founded by Nate Silver in 2008, known for its statistical analysis of U.S. elections and sports. ABC News acquired the site in 2013 but gradually reduced investment, leading to layoffs and eventual content removal after the 2024 election cycle.

**Discussion**: Community comments express frustration with ABC's decision, pointing to corporate pettiness and a pattern of building then discarding valuable brands. Users lament the loss of high-quality visualizations and suggest backing up the site's GitHub repositories before they are also taken down.

**Tags**: `#FiveThirtyEight`, `#ABC News`, `#data journalism`, `#Nate Silver`

---

<a id="item-8"></a>
## [OCaml in Space with OxCaml and Stack Annotations](https://gazagnaire.org/blog/2026-05-14-borealis.html) ⭐️ 8.0/10

The OxCaml variant of OCaml has been deployed in space applications, using stack annotations to eliminate garbage collection (GC) pressure and achieve ultra-low latency packet dispatch. Tests show p99.9 latency dropping from 29 ns to 9 ns per packet, with zero minor GCs over 25 million packets. This demonstrates that a garbage-collected functional language like OCaml can meet stringent real-time constraints in safety-critical space systems, challenging the assumption that only low-level languages are suitable. It could broaden the adoption of OCaml in embedded and high-performance domains. The stack annotations (stack_ keyword) allow values to be allocated on the stack instead of the heap, reducing GC pressure. The performance improvement was achieved on the packet dispatch hot path, with throughput remaining comparable.

hackernews · yminsky · May 15, 10:55 · [Discussion](https://news.ycombinator.com/item?id=48147058)

**Background**: OCaml is a functional programming language that relies on garbage collection for memory management, which can introduce unpredictable pauses. OxCaml is an OCaml variant developed by Jane Street that includes extensions for low-latency systems, such as stack allocation annotations. Stack allocation bypasses the GC by placing data on the call stack, making it ideal for real-time and high-frequency trading applications.

<details><summary>References</summary>
<ul>
<li><a href="https://oxcaml.org/documentation/stack-allocation/intro/">OxCaml | Stack allocation | Intro</a></li>
<li><a href="https://dev.realworldocaml.org/variants.html">Variants - Real World OCaml</a></li>

</ul>
</details>

**Discussion**: Commenters shared personal experiences with OCaml in space, such as a 2016 low-Earth orbit satellite (GHGSat-D) using OCaml for payload software. Others discussed the difficulty of bending garbage-collected languages to behave like non-GC ones in high-frequency trading, noting that Java can turn off the GC by pre-allocating massive memory.

**Tags**: `#OCaml`, `#space software`, `#garbage collection`, `#low-latency systems`, `#functional programming`

---

<a id="item-9"></a>
## [Uber Invests $10B+ in Robotaxi Fleet, Turns on Waymo](https://electrek.co/2026/05/15/uber-turns-on-waymo-10-billion-robotaxi-alternatives/) ⭐️ 8.0/10

Uber is investing over $10 billion to develop its own robotaxi fleet with partners Rivian, Lucid, and Nuro, while publicly criticizing its former partner Waymo. This marks a major strategic shift in the autonomous vehicle industry, potentially reshaping competition between ride-hailing platforms and self-driving technology providers. Uber's investment will leverage Rivian's hands-free driving tech, Lucid's autonomy-ready platform, and Nuro's autonomous delivery expertise. Meanwhile, Waymo vehicles still operate on Uber's platform in Austin and Atlanta.

rss · Electrek · May 15, 14:20

**Background**: The autonomous vehicle race has intensified as companies seek to commercialize self-driving technology. Uber had previously partnered with Waymo but is now pivoting to build its own fleet. Rivian is developing its Autonomy+ hands-free system, Lucid is engineering platforms for Level 4 autonomy, and Nuro is licensing its autonomy tech for robotaxis.

<details><summary>References</summary>
<ul>
<li><a href="https://rivian.com/autonomy">Rivian Autonomy+: Universal Hands-Free, Co-steer, and AI ...</a></li>
<li><a href="https://www.nuro.ai/">Nuro—Autonomy for all. All roads, all rides. | Nuro</a></li>
<li><a href="https://lucidmotors.com/stories/autonomy-ready-robotaxi-platform">Autonomy -Ready Robotaxi Platform | Lucid Motors</a></li>

</ul>
</details>

**Tags**: `#robotaxi`, `#autonomous vehicles`, `#Uber`, `#Waymo`, `#investment`

---

<a id="item-10"></a>
## [arXiv Bans Papers with Unchecked LLM Errors for 1 Year](https://www.reddit.com/r/MachineLearning/comments/1tdje2d/arxiv_implements_1year_ban_for_papers_containing/) ⭐️ 8.0/10

arXiv has announced a one-year ban for papers containing incontrovertible evidence of unchecked LLM-generated errors, such as hallucinated references or meta-comments left by the AI. This policy directly addresses the growing problem of LLM-generated errors undermining scientific integrity, holding authors accountable for AI-assisted content and discouraging careless use of generative AI in research. The ban applies only when evidence is incontrovertible, examples include hallucinated references and LLM meta-comments like 'this is a 200 word summary; would you like me to make any changes?' The policy also requires that after the ban, future submissions must first be accepted at a reputable peer-reviewed venue.

reddit · r/MachineLearning · Nunki08 · May 15, 02:44

**Background**: arXiv is a widely used preprint repository for scientific papers, especially in machine learning and computer science. With the rise of large language models (LLMs) like GPT-4, some authors have used them to generate content without proper verification, leading to errors like fake citations. This undermines the trustworthiness of scientific literature, prompting arXiv to enforce its code of conduct regarding author responsibility for all content.

**Discussion**: The community reaction is largely supportive, with many praising arXiv for taking a stand. Some commenters suggest a longer ban of 3-5 years, arguing that submitting fabricated citations is a serious breach of scientific integrity. Overall, the policy is seen as a necessary but lenient step.

**Tags**: `#arXiv`, `#LLM`, `#scientific integrity`, `#policy`, `#AI ethics`

---

<a id="item-11"></a>
## [Fully offline suitcase robot with Jetson Orin NX and Gemma 4 E4B](https://v.redd.it/9v5pmv1rgb1h1) ⭐️ 8.0/10

A developer built a fully offline suitcase robot named Sparky, running the Gemma 4 E4B model on a Jetson Orin NX SUPER 16GB, achieving ~200ms cached Time to First Token (TTFT) and 14-15 tok/s inference, with no network connectivity. This demonstrates that large language models can run effectively on edge hardware with optimized prompt caching, enabling privacy-preserving, fully local AI-driven robotics without reliance on cloud services. The robot uses 30+ sensors whose data is folded into the prompt as natural language, and optimized prompt structure places volatile data at the end of the latest user turn to maintain cache stability, reducing TTFT from multiple seconds to ~200ms.

reddit · r/LocalLLaMA · CreativelyBankrupt · May 15, 15:09 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1tdz5gr/built_a_fully_offline_suitcase_robot_around_a/)

**Background**: Edge AI involves running machine learning models on local devices rather than in the cloud, which reduces latency and improves privacy. Prompt caching reuses previously computed key-value (KV) cache entries to speed up inference. The Jetson Orin NX is a powerful edge computing platform from NVIDIA, and Gemma 4 E4B is a mixture-of-experts model from Google designed for efficient deployment on edge devices.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/google/gemma-4-E4B">google/gemma-4-E4B · Hugging Face</a></li>
<li><a href="https://ollama.com/library/gemma4:e4b">gemma4:e4b</a></li>
<li><a href="https://redis.io/blog/ttft-meaning/">TTFT Meaning: What is Time to First Token?</a></li>

</ul>
</details>

**Discussion**: A user commented 'Really cool hardware design, OP.' Another user shared an image link related to the project.

**Tags**: `#edge-ai`, `#robotics`, `#local-llm`, `#prompt-engineering`

---

<a id="item-12"></a>
## [Orthrus accelerates Qwen3-8B up to 7.8x with diffusion attention](https://i.redd.it/kmqh40q2nc1h1.gif) ⭐️ 8.0/10

Researchers have introduced Orthrus, which injects a trainable diffusion attention module into each layer of a frozen Qwen3-8B backbone, enabling parallel drafting of 32 tokens and achieving up to 7.8x faster token generation with provably identical output distribution to the base model. This method dramatically reduces inference latency without sacrificing accuracy, making LLMs more practical for real-time applications, and avoids the need for a separate draft model or additional KV cache overhead, offering a memory-efficient solution for accelerating large models. Orthrus freezes the backbone and trains only 16% of parameters on less than 1 billion tokens in 24 hours on 8×H200 GPUs, achieving an average acceptance length of 11.7 tokens on MATH-500, surpassing DFlash (7.9) and EAGLE-3 (3.5), with a flat KV cache overhead of only about 4.5 MiB.

reddit · r/LocalLLaMA · Franck_Dernoncourt · May 15, 19:07 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1te5xpu/orthrusqwen38b_up_to_78tokensforward_on_qwen38b/)

**Background**: Autoregressive language models generate tokens one at a time, which limits inference speed. Speculative decoding accelerates this by using a draft model to propose multiple tokens, which are then verified by the target model. Orthrus employs a diffusion attention head inside the same model to draft tokens in parallel, and because the backbone remains frozen, the output distribution is provably identical to the original model.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2605.12825">Orthrus : Memory-Efficient Parallel Token Generation via Dual-View...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Latent_diffusion_model">Latent diffusion model - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community expressed interest in scaling Orthrus to larger models like Qwen 3.6 27B and inquired about compatibility with MoE architectures. The post received a 99% upvote ratio and 136 points, indicating strong positive reception and curiosity about broader applicability.

**Tags**: `#LLM inference`, `#speculative decoding`, `#diffusion models`, `#efficiency`, `#Qwen`

---

<a id="item-13"></a>
## [Self-Hosted MCP Server Delivers Real Financial Data to Local LLMs](https://v.redd.it/3es19kwb2c1h1) ⭐️ 8.0/10

Developer daniel3303 released Equibles, an open-source self-hosted MCP server that scrapes and serves U.S. financial data such as SEC filings, 13F holdings, insider trades, and FRED indicators to local LLMs without cloud dependencies. This fills a critical gap for local LLM agents that need current, real-world data but cannot rely on cloud APIs. It enables privacy-preserving and offline financial analysis with LLMs. The server exposes data as MCP tools compatible with Claude Code/Desktop, Cursor, and custom agent loops. It includes daily prices, technical indicators, FINRA short volume, and CFTC futures positioning, all running locally with no telemetry.

reddit · r/LocalLLaMA · DanielAPO · May 15, 17:08 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1te2jko/i_built_a_selfhosted_opensource_mcp_server_that/)

**Background**: The Model Context Protocol (MCP) is an open standard introduced by Anthropic in November 2024 to standardize how LLMs interact with external data and tools. An MCP server exposes resources and tools that MCP clients (like AI applications) can query. Equibles acts as an MCP server for financial data, allowing local LLMs to retrieve filings like 13F (institutional holdings) and insider transaction forms (Form 3/4) via standardized interfaces.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Model_Context_Protocol">Model Context Protocol - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/news/model-context-protocol">Introducing the Model Context Protocol \ Anthropic</a></li>
<li><a href="https://www.sec.gov/search-filings">SEC.gov | Search Filings</a></li>

</ul>
</details>

**Discussion**: The community responded positively, with users expressing interest in using it for their projects. Comments highlight that the tool addresses a real need and is well-timed for experiments with local LLM agents.

**Tags**: `#MCP server`, `#financial data`, `#self-hosted`, `#open-source`, `#LLM agents`

---

<a id="item-14"></a>
## [Intern-S2-Preview: 35B Model Matches Trillion-Scale Performance](https://huggingface.co/internlm/Intern-S2-Preview) ⭐️ 8.0/10

Shanghai AI Laboratory released Intern-S2-Preview, a 35B-parameter scientific multimodal model that achieves performance comparable to the trillion-scale Intern-S1-Pro on core scientific tasks through a novel 'task scaling' approach with full-chain training from pre-training to reinforcement learning. This breakthrough demonstrates that task scaling can dramatically improve model efficiency, enabling smaller, open-source models to compete with much larger proprietary systems in specialized domains like material science and drug discovery, potentially accelerating scientific research by making advanced AI more accessible. Intern-S2-Preview is continued pretrained from Qwen3.5 and introduces real-valued prediction modules and material crystal structure generation capabilities, making it the first open-source model with both strong general abilities and crystal structure generation. It also enhances agent capabilities for scientific workflows.

reddit · r/LocalLLaMA · pmttyji · May 15, 10:09 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1tdrw0s/internlminterns2preview_hugging_face/)

**Background**: Traditional AI scaling relies on increasing model parameters (parameter scaling) or training data (data scaling). Task scaling, introduced by Intern-S2-Preview, instead focuses on expanding the difficulty, diversity, and coverage of scientific tasks to improve model performance without large parameter growth. Qwen3.5 is an open-source family of multimodal large language models from Alibaba, available in sizes including 35B parameters.

<details><summary>References</summary>
<ul>
<li><a href="https://unsloth.ai/docs/models/qwen3.5">Qwen3.5 - How to Run Locally | Unsloth Documentation</a></li>
<li><a href="https://grokipedia.com/page/Qwen35">Qwen3.5</a></li>

</ul>
</details>

**Discussion**: Community response is positive, with one user commenting 'Nice, this one looks interesting. Time to test.' The model has a 99% upvote ratio on Hugging Face, indicating strong approval from the technical community.

**Tags**: `#AI`, `#multimodal`, `#scientific model`, `#efficiency`, `#LLM`

---

<a id="item-15"></a>
## [ByteDance Releases Cola-DLM: Continuous Latent Diffusion LM](https://huggingface.co/ByteDance-Seed/Cola-DLM) ⭐️ 8.0/10

ByteDance has released Cola-DLM, a hierarchical continuous latent-space diffusion language model that combines a Text VAE with a block-causal Diffusion Transformer (DiT) prior, trained via Flow Matching. This novel approach from a major AI lab could advance text generation by leveraging diffusion in continuous latent space, potentially offering new trade-offs in quality and efficiency compared to autoregressive models. The model uses a two-stage training: first pretraining a Text VAE to map text to continuous latent sequences and decode back, then training a block-causal DiT for latent prior transport. Concerns about MMLU score (19) have been raised in community comments.

reddit · r/LocalLLaMA · pmttyji · May 15, 11:19 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1tdtaqt/bytedanceseedcoladlm_hugging_face/)

**Background**: Diffusion language models generate text by gradually denoising a random latent representation, as opposed to autoregressive token-by-token generation. Cola-DLM operates in a continuous latent space (via VAE) rather than on discrete tokens, which can capture global semantics more effectively. Block-causal DiT uses block-wise attention to enable efficient processing of long sequences.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/papers/2605.06548">Paper page - Continuous Latent Diffusion Language Model</a></li>
<li><a href="https://arxiv.org/abs/2605.06548">[2605.06548] Continuous Latent Diffusion Language Model</a></li>
<li><a href="https://www.guidelabs.ai/post/block-causal-diffusion-language-model/">Causal Diffusion Language Models</a></li>

</ul>
</details>

**Discussion**: Community comments express excitement about the approach but note that the MMLU score of 19 is below random guessing (25%), raising concerns about reasoning performance. Some users mention hardware support limitations, particularly for AMD GPUs with Vulkan.

**Tags**: `#diffusion language model`, `#VAE`, `#ByteDance`, `#AI research`, `#latent space`

---

<a id="item-16"></a>
## [Image-blaster: Turn a single image into a 3D world](https://github.com/neilsonnn/image-blaster) ⭐️ 7.0/10

Image-blaster is an open-source tool that generates fully explorable 3D environments, meshes, physics, lighting, and audio from a single image using AI models from World Labs, Claude, and FAL. This tool drastically lowers the barrier to creating 3D assets, enabling game developers, artists, and VR creators to generate rich environments from a single photo without specialized skills or equipment. The tool combines World Labs' 3D Gaussian Splatting with Marble, Claude's skill system, and FAL for inference, outputting meshes, interactive physics objects, and sound effects. Users need API keys for World Labs and FAL.

hackernews · MattRogish · May 15, 15:42 · [Discussion](https://news.ycombinator.com/item?id=48150069)

**Background**: Single-image 3D reconstruction has advanced rapidly with models like LRM and InstantMesh that predict 3D structure from a single view. Image-blaster integrates these AI capabilities into a user-friendly pipeline via Claude, allowing anyone to generate a 3D world from any image.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/neilsonnn/image-blaster">GitHub - neilsonnn/image-blaster: An image-to-world skillset for Claude. · GitHub</a></li>
<li><a href="https://www.worldlabs.ai/labs/showcase/image-blaster">Image Blaster | Community Showcase | World Labs</a></li>
<li><a href="https://arxiv.org/abs/2311.04400">LRM: Large Reconstruction Model for Single Image to 3D</a></li>

</ul>
</details>

**Discussion**: Commenters compared it to Microsoft's PhotoSynth and noted the use of World Labs, with some expressing concerns about hallucinations and usability. Others suggested alternatives like Meshy.ai and TRELLIS for specific use cases.

**Tags**: `#3D reconstruction`, `#AI`, `#computer vision`, `#open-source`, `#mesh generation`

---

<a id="item-17"></a>
## [Waymo Recalls 3,800 Robotaxis Over Standing Water Glitch](https://www.cnbc.com/2026/05/12/waymo-recalls-3800-robotaxis-after-able-drive-into-standing-water.html) ⭐️ 7.0/10

Waymo issued a recall and software update for 3,800 robotaxis after a glitch caused them to drive into standing water. This recall highlights a critical edge case for autonomous vehicles: safely detecting and avoiding standing water. It also demonstrates the advantage of over-the-air updates for quickly fixing real-world issues across an entire fleet. The glitch affected the vehicles' perception system, causing them to misinterpret standing water as a drivable surface. Waymo resolved the issue via a software update distributed over the air, avoiding a physical recall.

hackernews · drob518 · May 15, 18:00 · [Discussion](https://news.ycombinator.com/item?id=48151767)

**Background**: Autonomous vehicles rely on a combination of cameras, lidar, radar, and AI algorithms to perceive their environment. Distinguishing wet pavement from deep standing water is a challenging problem because both appear similar to sensors. A dedicated water sensor, as suggested by one commenter, could provide more reliable detection but may cause excessive caution on shallow puddles.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sfchronicle.com/sf/article/waymo-robotaxis-storms-20067357.php">Here’s how Waymo robotaxis handle driving in storms</a></li>
<li><a href="https://waymo.com/waymo-driver/">Self-Driving Car Technology for a Reliable Ride - Waymo Driver</a></li>

</ul>
</details>

**Discussion**: Commenters debated detection strategies: some advocated for dedicated water sensors, while others favored inferring water presence from vehicle behavior. A key point was that OTA updates allow rapid fleet-wide fixes, making autonomous vehicles safer with each iteration.

**Tags**: `#Waymo`, `#autonomous vehicles`, `#robotaxi safety`, `#recall`, `#self-driving cars`

---

<a id="item-18"></a>
## [Community Celebrates Jason Scott's Digital Preservation](https://ascii.textfiles.com/) ⭐️ 7.0/10

Jason Scott's blog and his extensive digital preservation work, including digitizing over 1,300 magnetic tapes and 13,000 manuals for the Internet Archive, are receiving high praise from the online community. This recognition highlights the critical role of individual archivists in preserving digital history, ensuring that rare software, music, and documentation remain accessible to future generations. It underscores the ongoing need for dedicated preservation efforts as legacy media degrades. One community member reported that over 1,300 tapes from a single collection were digitized, while another noted that 13,000 manuals were uploaded to the Internet Archive over a decade—roughly 3.5 manuals per day. Jason Scott also streams his preservation work live on Twitch.

hackernews · bookofjoe · May 15, 14:02 · [Discussion](https://news.ycombinator.com/item?id=48148726)

**Background**: Digital preservation involves converting physical media, such as magnetic tapes and paper manuals, into digital formats to prevent data loss from decay or obsolescence. Magnetic tapes from the 1970s–1990s often contain unique software or recordings that are at risk of becoming unreadable. Retrocomputing enthusiasts and archivists like Jason Scott work to rescue this content and make it freely available on platforms like the Internet Archive.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Preservation_of_magnetic_audiotape">Preservation of magnetic audiotape - Wikipedia</a></li>
<li><a href="https://grokipedia.com/page/Retrocomputing">Retrocomputing</a></li>

</ul>
</details>

**Discussion**: Community comments are overwhelmingly positive, with users praising Jason Scott's prolific output (e.g., ~1,300 tapes digitized) and dedication to free information. One commenter noted that the current blog link is outdated and provided an updated one, while another pointed out that Jason Scott is currently live-streaming on Twitch. Overall, the sentiment is deep gratitude and admiration.

**Tags**: `#digital preservation`, `#ASCII`, `#Jason Scott`, `#internet archive`, `#retrocomputing`

---

<a id="item-19"></a>
## [Radicle: Sovereign code forge built on Git](https://radicle.dev/) ⭐️ 7.0/10

Radicle, a decentralized Git-based code forge prioritizing sovereignty, recently moved to the domain radicle.dev, offering peer-to-peer code collaboration with support for private repositories. Decentralized code forges like Radicle challenge the centralization of platforms such as GitHub, fostering developer autonomy and enabling new use cases like agentic workflows, which could reshape open-source collaboration. Radicle does not use the AGPL license, raising concerns that SaaS companies could embrace-extend-extinguish the project, and its FAQ indicates plans to offer commercial services on top of the protocol.

hackernews · KolmogorovComp · May 15, 12:07 · [Discussion](https://news.ycombinator.com/item?id=48147603)

**Background**: A code forge is a platform for hosting, reviewing, and collaborating on source code, typically using version control systems like Git. Radicle differentiates itself by being decentralized and peer-to-peer, avoiding reliance on a central server, which gives users more control over their data and workflows.

**Discussion**: Community reactions are mixed: some express concern over the non-AGPL license and potential commercialization, while others praise Radicle's privacy features and find it especially useful for agentic workflows, with one user noting a recent domain move.

**Tags**: `#decentralized`, `#git`, `#code forge`, `#open source`, `#p2p`

---

<a id="item-20"></a>
## [Tesla Unredacts All 17 Robotaxi Crash Narratives](https://electrek.co/2026/05/15/tesla-unredacts-robotaxi-crash-narratives-nhtsa/) ⭐️ 7.0/10

Tesla has unredacted all 17 autonomous driving crash narratives filed with NHTSA, revealing for the first time the details of each incident. The data shows that most crashes were not the system's fault, but some concerning incidents remain. This move provides unprecedented transparency into Tesla's autonomous driving safety, which is critical for public trust and regulatory oversight. It may influence future safety regulations for robotaxi services. Tesla had previously redacted all narratives as 'confidential business information,' making it the only autonomous driving system operator to fully redact reports. The unredaction reveals a mix of incidents, including some where the system may have been at fault.

rss · Electrek · May 15, 15:04

**Background**: Tesla Robotaxi is a ride-hailing service using vehicles equipped with Full Self-Driving (FSD) software, launched in Austin in June 2025. NHTSA requires automakers to report crashes involving autonomous or assisted-driving systems. Tesla's reports had been fully redacted, drawing criticism for lack of transparency.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Robotaxi">Tesla Robotaxi - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#Robotaxi`, `#autonomous driving`, `#safety`, `#NHTSA`

---

<a id="item-21"></a>
## [Dynamic compute allocation with Qwen-35B-A3B nears GPT-5.4 on HLE](https://www.reddit.com/gallery/1te8sxt) ⭐️ 7.0/10

A method dynamically allocates compute budget to hard problems using the Qwen-35B-A3B model, achieving performance close to GPT-5.4-xHigh on the Humanity's Last Exam (HLE) benchmark. The baseline Qwen-35B-A3B scores 21.4% on HLE, while GPT-5.4-xHigh scores 41.6%. This approach demonstrates that mid-sized models with intelligent compute allocation can approach frontier model performance, potentially reducing inference costs for challenging problems. It highlights a practical technique for users who want to maximize local model capability without relying on expensive cloud APIs. The method involves letting Qwen dynamically allocate compute, but the original poster cautions against using it for agentic tasks due to divergence. A commenter asks if this is essentially self-consistency or majority voting, indicating the technique may be related to ensemble methods.

reddit · r/LocalLLaMA · Ryoiki-Tokuiten · May 15, 20:51 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1te8sxt/dynamically_allocating_compute_budget_to_hard_set/)

**Background**: Humanity's Last Exam (HLE) is a challenging benchmark with 2,500 expert-vetted questions across various subjects, designed to test frontier AI models. Qwen-35B-A3B is a Mixture-of-Experts model with 35B total parameters and 3B activated, released by Alibaba Cloud. GPT-5.4-xHigh is OpenAI's latest model with a higher reasoning effort setting, achieving state-of-the-art results on HLE.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-35B-A3B">Qwen/Qwen3.6-35B-A3B · Hugging Face</a></li>
<li><a href="https://artificialanalysis.ai/models/gpt-5-4">GPT-5.4 (xhigh) - Intelligence, Performance & Price Analysis</a></li>

</ul>
</details>

**Discussion**: The main commenter, Ryoiki-Tokuiten, advises using the method only for favorite hard problems with a large compute budget and warns against using it for agent harnesses due to divergence. Another user asks if it is essentially self-consistency or majority voting, suggesting the technique may be a form of ensemble inference.

**Tags**: `#LLM`, `#compute allocation`, `#Qwen`, `#local LLM`, `#inference technique`

---

<a id="item-22"></a>
## [Exploring Modded 4090 48GB GPUs for LLM](https://www.reddit.com/r/LocalLLaMA/comments/1tdldfq/china_modded_gpu_eg_4090_48gb_im_gonna_figure_it/) ⭐️ 7.0/10

A Reddit user is actively researching China-modded RTX 4090 GPUs with 48GB VRAM, calling for collective research and sharing links to existing threads and a video. Commenters provide real-world experiences, including one running three cards for LLM inference and a US modder offering upgrades on full-power 4090s. These modded GPUs offer a cost-effective way to achieve 48GB VRAM for running large language models locally, addressing a key bottleneck for AI enthusiasts. However, concerns about reliability, cooling, and performance differences between China's 'D' variant and full-power cards make this investigation timely and important. The mod involves micro-soldering additional GDDR6X memory chips and BIOS modification; two 2GB modules per memory controller yield 48GB. China's 4090D uses gimped cores (10-15% lower performance), and cooling is a major issue, with users reporting loud fans and need for high-RPM server fans. A US modder (gpulab.net) claims to upgrade regular 4090s without performance loss.

reddit · r/LocalLLaMA · LeatherRub7248 · May 15, 04:16

**Background**: GPU VRAM is soldered directly onto the board, making upgrades difficult for typical users. The RTX 4090 normally has 24GB of GDDR6X; modders replace the memory chips with higher-capacity ones and adjust the BIOS. These modded cards are popular in China for AI workloads, but reliability and warranty are concerns. The community seeks detailed benchmarks and long-term usage data.

<details><summary>References</summary>
<ul>
<li><a href="https://hothardware.com/news/geforce-rtx-4090-48gb-vram-mod">Wild GeForce RTX 4090 Mod Upgrades VRAM To 48GB, Requires</a></li>
<li><a href="https://www.extremetech.com/computing/modder-shows-how-to-give-rtx-4090-48gb-of-vram">Modder Shows How to Give RTX 4090 48GB of VRAM | Extremetech</a></li>

</ul>
</details>

**Discussion**: One user (Heathen711) runs three 48GB blower cards successfully for LLM and stable-diffusion workloads, but warns about cooling requirements. Another (Kulidc) sold his card due to noise and reliability issues after a few weeks. A US modder (computune) criticizes China's 4090D performance and offers modded full-power 4090s with better results.

**Tags**: `#modded GPUs`, `#VRAM`, `#LLM inference`, `#hardware modding`

---

<a id="item-23"></a>
## [Google's IDE Evolution: From Custom Tools to VS Code Fork](https://laurent.le-brun.eu/blog/a-history-of-ides-at-google) ⭐️ 7.0/10

A blog post by Laurent Le Brun chronicles the evolution of Google's internal integrated development environments (IDEs), tracing the journey from specialized tools like Cider to a custom fork of Microsoft's VS Code. This history sheds light on how a large tech company like Google approaches developer tooling and productivity, and illustrates the industry trend of adopting VS Code as a unified platform. The blog post covers the motivation behind moving from multiple in-house IDE projects to a single forked VS Code, which eventually became known as Antigravity, and highlights the engineering effort involved.

reddit · r/programming · laurentlb · May 15, 19:31 · [Discussion](https://www.reddit.com/r/programming/comments/1te6m44/a_history_of_ides_at_google/)

**Background**: IDEs are software applications that provide comprehensive facilities for programmers, including code editing, debugging, and building. Google, like many large companies, historically developed internal tools tailored to its monorepo and workflows. Over time, the complexity of maintaining multiple editors led to a consolidation strategy, culminating in a fork of VS Code that integrates deeply with Google's infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://www.howtogeek.com/why-google-built-its-own-vs-code-fork-in-the-first-place/">Why Google built its own VS Code fork in the first place</a></li>
<li><a href="https://medium.com/@bhagyarana80/cider-what-ide-stack-does-google-use-internally-vs-code-intellij-or-something-else-0d67f9e2481d">What IDE Stack Does Google Use Internally? | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters had mixed reactions: some praised Cider V as awesome and noted Google's tooling as the best, while others criticized the inability to agree on a common editor and the shift in culture at Google.

**Tags**: `#Google`, `#IDEs`, `#Developer Tools`, `#VS Code`

---

<a id="item-24"></a>
## [Bun.sh Ported to Rust via LLM: 1M Lines Generated](https://renfoc.us/posts/1778877814-rust_on_my_bun) ⭐️ 7.0/10

A developer used large language models (LLMs) to automatically convert Bun.sh's JavaScript runtime codebase into Rust, resulting in approximately 1 million lines of generated Rust code. This demonstrates the potential of LLMs for large-scale code conversion, which could accelerate language migrations and reduce manual effort. However, the output size and quality raise questions about practical maintainability. The original Bun codebase was about 4,000 lines of JavaScript, but the LLM generated roughly 1 million lines of Rust, a 250x increase. The project is described as a 'unserious' endeavor by some community members.

reddit · r/programming · trigzo · May 15, 21:05 · [Discussion](https://www.reddit.com/r/programming/comments/1te96np/rust_on_my_buns/)

**Background**: Bun is a fast JavaScript runtime designed as a drop-in replacement for Node.js, using Safari's JavaScriptCore engine. Large language models are AI systems trained on vast text data that can generate or convert code between programming languages when given appropriate prompts.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some highlight the absurdity of replacing 4,000 lines with 1 million lines, while others note that this topic has been widely discussed on forums like Hacker News and Reddit. A minority dismiss the project as unserious.

**Tags**: `#Rust`, `#Bun`, `#LLM`, `#code generation`, `#porting`

---

<a id="item-25"></a>
## [Rivian R2 Configurator Goes Live](https://rivian.com/configurations/builder/r2) ⭐️ 7.0/10

Rivian has launched the R2 configurator, allowing customers to reserve the upcoming electric SUV with various trim and range options, including a rear-wheel-drive version with 345 miles of range. This marks a key step in Rivian's expansion into the more affordable mid-size EV SUV segment, potentially attracting a broader customer base beyond the premium R1 lineup. The R2 offers Standard AWD and Premium AWD trims, with the latter only $2,000 more, and a base RWD version with 345 miles of range. Deliveries are expected in 2026.

reddit · r/electricvehicles · SapientChaos · May 15, 15:55 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1te0gv4/the_r2_configurator_is_live/)

**Background**: The Rivian R2 is a mid-size five-seat electric SUV designed to be more accessible than the flagship R1S and R1T. It aims to combine everyday usability with off-road capability, featuring a starting price around $45,000.

<details><summary>References</summary>
<ul>
<li><a href="https://rivian.com/r2">Rivian R2 Electric SUV: Price, Range & Features</a></li>
<li><a href="https://www.caranddriver.com/rivian/r2">2027 Rivian R2: What We Know So Far - Car and Driver</a></li>

</ul>
</details>

**Discussion**: Community members expressed excitement about the 345-mile range on the RWD model, with one user placing a reservation. Others questioned the logic of the Standard AWD trim being only $2,000 less than Premium, and jokingly asked about the 800V battery option.

**Tags**: `#Rivian`, `#R2`, `#electric vehicle`, `#configurator`, `#EV`

---

<a id="item-26"></a>
## [China Builds Largest Ice-Snow EV Test Base with Indoor Snow](https://indiandefencereview.com/china-building-world-largest-ice-snow-ev-test-base-solve-electric-cars/) ⭐️ 7.0/10

China Automotive Technology and Research Center has broken ground on a 67-hectare test facility in Inner Mongolia, scheduled to open in 2028. It will be the world's first facility capable of simulating indoor snowfall conditions for vehicle validation. This addresses a critical challenge for electric vehicles in cold climates: performance degradation of batteries and traction control. The ability to consistently recreate winter conditions indoors enables manufacturers to rigorously test and improve EV cold-weather performance. The base is 67 hectares and will be the largest ice-snow EV test base in the world. It features indoor snow-making capability that allows precise control of snowfall volume and ice friction coefficients, overcoming the unpredictability of real-world weather.

reddit · r/electricvehicles · TylerFortier_Photo · May 15, 18:48 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1te5f01/china_is_building_the_worlds_largest_icesnow_ev/)

**Background**: Intelligent connected new energy vehicles (NEVs) integrate new energy technologies with connectivity, autonomous driving, and smart systems. Cold weather poses two main problems for EVs: battery and climate system performance, and traction on low-grip surfaces. Existing winter proving grounds rely on natural weather and cannot guarantee consistent conditions.

<details><summary>References</summary>
<ul>
<li><a href="https://techgolly.com/china-builds-massive-indoor-snow-test-track-for-electric-cars">China Builds Massive Indoor Snow Test Track For Electric Cars</a></li>
<li><a href="https://www.nst.com.my/business/economy/2026/05/1437267/china-starts-building-worlds-largest-ice-snow-text-base">China starts building world's largest ice- snow text base for intelligent...</a></li>
<li><a href="http://www.china.org.cn/2026-03/13/content_118380618.shtml">Intelligent new energy vehicles power China's smart... - China.org.cn</a></li>

</ul>
</details>

**Discussion**: Community comments distinguished battery performance issues from traction control advantages of EVs. One user noted that indoor snow is unnecessary for battery testing as freezers suffice, and argued EVs have better torque control on snow. Another shared positive real-world winter experience with EVs.

**Tags**: `#Electric Vehicles`, `#Cold Weather Testing`, `#China`, `#Infrastructure`

---

<a id="item-27"></a>
## [Volvo Stays All-In on Electric and Software-Defined Vehicles](https://www.motortrend.com/news/why-volvo-all-in-electric-vehicles) ⭐️ 7.0/10

Volvo's chief commercial officer Erik Severinson explained that the company made a deliberate strategic decision five years ago to focus solely on electric vehicles (EVs) and software-defined vehicles (SDVs), deliberately avoiding investment in internal combustion engines to meet emissions standards. CEO Håkan Samuelsson added that EVs are better cars, lower cost, and better for the environment, though plug-in hybrids remain a bridge in the U.S. At a time when many legacy automakers are backtracking on EV plans, Volvo's unwavering commitment signals confidence in electrification as the inevitable future. This strategy could pressure competitors and reassure consumers and investors about the long-term viability of EVs. Volvo shares platform and powertrain costs with parent Geely, applying a 'Volvo top hat' design. The company recognizes that in markets like the U.S., plug-in hybrids serve as a transitional solution until widespread EV acceptance matures.

reddit · r/electricvehicles · runnyyolkpigeon · May 15, 00:21 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1tdg6pl/why_volvo_is_still_allin_on_electric_vehicles/)

**Background**: A software-defined vehicle (SDV) is one where core functions are controlled and updated through software rather than fixed hardware, enabling continuous improvements and new features over the air. This approach, combined with dedicated EV platforms, represents a fundamental shift from traditional automotive engineering. Volvo's early bet on SDVs positions it to leverage future software-driven innovations such as autonomous driving and advanced infotainment.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Software_Defined_Vehicle">Software Defined Vehicle - Wikipedia</a></li>
<li><a href="https://www.ibm.com/think/topics/software-defined-vehicle">What is a software-defined vehicle? - IBM</a></li>

</ul>
</details>

**Discussion**: Community sentiment is overwhelmingly positive, with users praising Volvo's consistent EV strategy as a 'breath of fresh air' and noting that over 90% of EV switchers never return. One Polestar 2 owner defended the software experience, countering common complaints about reliability.

**Tags**: `#electric vehicles`, `#automotive industry`, `#software-defined vehicles`, `#Volvo`, `#EV strategy`

---

<a id="item-28"></a>
## [Project Gutenberg Announces Site Improvements](https://www.gutenberg.org/) ⭐️ 6.0/10

Project Gutenberg has recently rolled out significant site improvements, including user interface and functionality updates, as confirmed by one of its programmers. These improvements enhance the accessibility and usability of the world's largest digital library of public domain books, benefiting millions of free literature readers worldwide. The updates are part of an ongoing effort; more improvements are planned for the future, and users are encouraged to revisit the site.

hackernews · JSeiko · May 15, 16:15 · [Discussion](https://news.ycombinator.com/item?id=48150431)

**Background**: Project Gutenberg was founded in 1971 by Michael S. Hart with the digitization of the U.S. Declaration of Independence. It is the oldest digital library, offering over 60,000 free eBooks in the public domain, maintained by volunteers.

**Discussion**: The community response is largely positive, with one user sharing a heartfelt story of how Project Gutenberg enriched their father's reading life. However, a user from Italy reported that the site is blocked by a police seizure notice, raising concerns about censorship. Another user suggested that eBook reader vendors should integrate a Project Gutenberg store for easier access.

**Tags**: `#Project Gutenberg`, `#digital library`, `#open access`, `#public domain`, `#site update`

---

<a id="item-29"></a>
## [New Book Explores Steve Jobs' NeXT Years](https://spectrum.ieee.org/steve-jobs-next-computer) ⭐️ 6.0/10

A new book delves into Steve Jobs' transformative years at NeXT Computer, focusing on his personal growth and the company's enduring influence on Apple. This historical perspective fills a gap in understanding how Jobs evolved between his departures from and return to Apple, and how NeXT's technology became the foundation of modern Apple products. The book covers Jobs' 12-year tenure at NeXT, including the development of NeXTSTEP, which later formed the core of macOS and iOS. Community comments highlight NeXT's pivotal role in Apple's revival and the Vision Pro's missed software potential.

hackernews · rbanffy · May 15, 10:34 · [Discussion](https://news.ycombinator.com/item?id=48146908)

**Background**: NeXT Computer was founded by Steve Jobs in 1985 after he was ousted from Apple. The company developed the NeXTSTEP operating system, known for its object-oriented design and Unix foundation. Apple acquired NeXT in 1997, leading to the creation of macOS and iOS. The first web browser and App Store concept originated on NeXTSTEP.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/NeXT">NeXT - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/NeXTSTEP">NeXTSTEP - Wikipedia</a></li>
<li><a href="https://www.howtogeek.com/698532/before-mac-os-x-what-was-nextstep-and-why-did-people-love-it/">Before Mac OS X: What Was NeXTSTEP, and Why Did People Love It? NEXTSTEP Operating System WinWorld: NeXTStep 4.x NeXTSTEP - ArchiveOS The Deep History of Your Apps: Steve Jobs, NeXTSTEP, and ...</a></li>

</ul>
</details>

**Discussion**: Commenters note that modern Apple is largely NeXT, with the dying Apple fading away. Some criticize Apple's software vision for Vision Pro as a missed opportunity, echoing NeXT's legacy of innovation. There is also mention of a project to bring NeXTSTEP aesthetics to Linux.

**Tags**: `#Steve Jobs`, `#NeXT`, `#Apple`, `#tech history`, `#book review`

---

<a id="item-30"></a>
## [C3 0.8.0 refines builtins, reflection, and unsigned sizes](https://c3-lang.org/blog/0_8_0_the_core_language_is_settling/) ⭐️ 6.0/10

C3 0.8.0 replaces builtins with a new approach, simplifies reflection, and rethinks unsigned sizes, marking a settling of the core language. This release stabilizes C3's core features, making it more attractive for system programming and embedded development where C is traditionally used. The changes are focused on refining the language's syntax and semantics; community feedback influenced the decisions to simplify reflection and adjust unsigned size handling.

reddit · r/programming · Nuoji · May 15, 08:33 · [Discussion](https://www.reddit.com/r/programming/comments/1tdq64x/c3_080_replaces_builtins_simplifies_reflection/)

**Background**: C3 is a programming language that builds on C syntax and semantics, aiming to evolve C while retaining compatibility. It targets system programming and embedded developers who want modern features without abandoning the C ecosystem. Version 0.8.0 represents a significant step toward a stable release.

<details><summary>References</summary>
<ul>
<li><a href="https://c3-lang.org/">C3 Programming Language</a></li>

</ul>
</details>

**Discussion**: Commenters expressed interest in C3's fit with existing C compilers for embedded development, with one disliking contracts-in-comments (compared to TypeScript). Another asked about compile-time inheritance resolution for embedded use.

**Tags**: `#programming language`, `#C3`, `#system programming`, `#release`

---

<a id="item-31"></a>
## [Chinese EVs Enter Canadian Market, Dealers Excited](https://www.cnbc.com/2026/05/15/chinese-evs-canada.html) ⭐️ 6.0/10

Chinese electric vehicle manufacturers, notably BYD, are set to enter the Canadian market, with some dealers expressing eagerness to sell them. Reports indicate growing curiosity among Canadian consumers about Chinese EV models. This entry could disrupt Canada's automotive market by offering affordable, technologically advanced EVs, potentially pressuring legacy automakers to lower prices and accelerate electrification. It also reflects the global expansion of Chinese automakers despite trade barriers. Dealers are enthusiastic about carrying Chinese EVs, while some consumers hope for lower prices. Community discussions highlight debates over direct-sales models versus traditional dealership networks, with BYD's models like the Atto 3 and Seal generating particular interest.

reddit · r/electricvehicles · AdvertisingPretend98 · May 15, 17:31 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1te37uh/chinese_evs_are_coming_to_canada_and_some_dealers/)

**Background**: Chinese automakers like BYD have developed advanced technologies such as blade batteries and long-range EVs, becoming the world's largest EV manufacturer. Canada currently imposes tariffs on Chinese EVs, but dealer optimism suggests market demand may overcome policy hurdles. BYD's expansion into Mexico and other markets has already generated buzz among North American consumers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.byd.com/">Electric Cars, Sedans and SUVs I BYD USA</a></li>
<li><a href="https://electriccar-byd.com/en">BYD Electric Vehicles | World's #1 EV Manufacturer ...</a></li>
<li><a href="https://www.byd.international/models">BYD Car Models | Electric & Hybrid Vehicles</a></li>

</ul>
</details>

**Discussion**: Community comments express frustration with traditional dealership models, with one user calling for their demise in favor of direct sales. Another user shares a positive experience seeing BYD models in Mexico, while a Canadian consumer quoted in the article predicts Chinese EVs will ‘destroy the market in a good way’ by offering better value.

**Tags**: `#EVs`, `#Chinese cars`, `#Canada`, `#automotive industry`, `#BYD`

---