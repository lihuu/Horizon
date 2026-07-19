---
layout: default
title: "Horizon Summary: 2026-07-19 (EN)"
date: 2026-07-19
lang: en
---

> From 22 items, 14 important content pieces were selected

---

1. [GPT-5.6 Solves 30-Year Convex Optimization Gap with a Prompt](#item-1) ⭐️ 9.0/10
2. [LG monitors silently install software via Windows Update](#item-2) ⭐️ 9.0/10
3. [StackOverflow's decline linked to AI chatbots](#item-3) ⭐️ 9.0/10
4. [Kimi K3: Frontier Model from Non-US Lab Sparks Debate](#item-4) ⭐️ 8.0/10
5. [If You Build It, They Will Come](#item-5) ⭐️ 7.0/10
6. [Fable 5 vs GPT-5.6 Sol on NP-Hard: Does /goal Help?](#item-6) ⭐️ 7.0/10
7. [Guide to Isolate Claude AI on a Spare Mac](#item-7) ⭐️ 7.0/10
8. [Goodbye, Bikesheds: A Reflection on PHK's Legacy](#item-8) ⭐️ 7.0/10
9. [SQLite Query Explainer: Interactive Browser Tool](#item-9) ⭐️ 7.0/10
10. [Anthropic Reverses Plan, Makes Claude Fable 5 Permanent in Higher Tiers](#item-10) ⭐️ 7.0/10
11. [fsync inside WAL lock degrades concurrency](#item-11) ⭐️ 7.0/10
12. [Learn Formal Verification with Lean: Part 1 Tutorial](#item-12) ⭐️ 7.0/10
13. [Beyond Retries: Alternative Resilience Patterns](#item-13) ⭐️ 7.0/10
14. [Zilog Z80 Turns 50: A Microprocessor Milestone](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [GPT-5.6 Solves 30-Year Convex Optimization Gap with a Prompt](https://old.reddit.com/r/math/comments/1uxj3cy/after_openais_cdc_proof_announcement_gpt56_used_a/) ⭐️ 9.0/10

GPT-5.6, a new AI model, resolved a long-standing open problem in convex optimization by using a single prompt, closing a gap that had persisted for 30 years. This achievement demonstrates that large language models can make genuine contributions to advanced mathematics, potentially accelerating research and reducing the need for human work on routine mathematical problems. The model used was GPT-5.6 Sol Pro (not Ultra), and the problem involves upper bounds on time complexity for convex optimization over Lipschitz functions on a bounded domain.

hackernews · mbustamanter · Jul 18, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48957779)

**Background**: Convex optimization is a subfield of mathematical optimization focusing on minimizing convex functions over convex sets, and many such problems admit efficient algorithms. The 'gap' refers to a theoretical bound that had remained unproven for three decades, limiting understanding of solution complexity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Convex_optimization">Convex optimization - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Convex_optimization_problem">Convex optimization problem</a></li>

</ul>
</details>

**Discussion**: Comments indicated the problem is niche but a real contribution, with some noting that such results may shift mathematical research towards more novel approaches rather than low-hanging fruit. There was also discussion about the model version (Sol Pro vs Ultra) and comparisons to prior proofs.

**Tags**: `#AI`, `#mathematics`, `#convex optimization`, `#GPT`, `#breakthrough`

---

<a id="item-2"></a>
## [LG monitors silently install software via Windows Update](https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent) ⭐️ 9.0/10

Connecting some LG monitors to a Windows PC triggers Windows Update to automatically install an LG app that promotes McAfee subscriptions, without any user consent or notification. This exposes a serious security and privacy vulnerability where hardware vendors can abuse Windows Update's trusted mechanism to silently install potentially unwanted software with full system access, affecting millions of users. The installed LG software runs at every boot, has internet access and full system access with no sandboxing, and is triggered by plugging in an LG monitor via HDMI. Gamers Nexus tested it across 32 boots and observed the McAfee popup 31 times.

hackernews · baranul · Jul 18, 10:21 · [Discussion](https://news.ycombinator.com/item?id=48956688)

**Background**: Windows Update is designed to deliver drivers and software from hardware manufacturers to ensure device compatibility. However, this mechanism can be misused if manufacturers push applications that are not strictly necessary. Users can disable this via Group Policy or Device Installation Settings.

<details><summary>References</summary>
<ul>
<li><a href="https://videocardz.com/newz/lg-monitors-silently-install-software-through-windows-update-without-user-consent">LG monitors silently install software through Windows Update ...</a></li>
<li><a href="https://byteiota.com/lg-monitor-adware-windows-update/">LG Monitor Adware: Windows Update Installs It Without Asking</a></li>
<li><a href="https://cybersecuritynews.com/windows-update-installs-lg-monitor-app-pushes-mcafee-ads/">Windows Update Silently Installs LG Monitor App That Pushes ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed outrage, calling the behavior malware-like. They highlighted that the software installs automatically upon connecting an LG monitor, even if previously connected. Workarounds were suggested, such as disabling automatic download of manufacturer apps via gpedit.msc or Device Installation Settings.

**Tags**: `#security`, `#windows`, `#privacy`, `#hardware`, `#malware`

---

<a id="item-3"></a>
## [StackOverflow's decline linked to AI chatbots](https://data.stackexchange.com/stackoverflow/query/1953768#graph) ⭐️ 9.0/10

A graph posted on StackExchange Data Explorer visualizes the decline in StackOverflow activity, correlating it with the rise of AI chatbots like ChatGPT. This trend signals a fundamental shift in how developers seek answers, potentially reducing reliance on traditional Q&A platforms and impacting the developer community's knowledge-sharing dynamics. The graph shows a noticeable decline in StackOverflow activity starting around the time ChatGPT was released, though community comments also point to factors like restrictive policies and the site's acquisition by Prosus in 2021.

hackernews · secretslol · Jul 18, 11:12 · [Discussion](https://news.ycombinator.com/item?id=48956949)

**Background**: StackOverflow is a popular Q&A platform for programmers, where users ask and answer technical questions. AI chatbots like ChatGPT can provide instant answers, reducing the need to browse through existing threads or post new questions. However, StackOverflow's strict moderation and emphasis on concise Q&A without discussion may have also driven users away.

**Discussion**: Commenters largely agree that StackOverflow's own policies contributed to its decline, citing high barriers for newcomers and a lack of community feel. Some note that the decline began before ChatGPT, linking it to the 2021 acquisition by Prosus, and appreciate that AI chatbots offer a less hostile experience.

**Tags**: `#StackOverflow`, `#AI impact`, `#developer community`, `#LLMs`, `#online communities`

---

<a id="item-4"></a>
## [Kimi K3: Frontier Model from Non-US Lab Sparks Debate](https://stephen.bochinski.dev/blog/2026/07/18/the-kimi-k3-moment/) ⭐️ 8.0/10

The Chinese AI lab Kimi released Kimi K3, a 2.8-trillion-parameter frontier model with a 1-million-token context window, achieving performance comparable to leading US models like GPT-5.6. This challenges the US dominance in frontier AI and raises urgent questions about model distillation, cost efficiency, and potential national security regulations on open-weight models. Kimi K3 uses novel architectures like Kimi Delta Attention and Attention Residuals, and is the world's first open 3T-class model. Its pricing is $3/$15 per 1M tokens input/output, compared to GPT-5.6's $5/$30.

hackernews · sbochins · Jul 18, 17:32 · [Discussion](https://news.ycombinator.com/item?id=48960218)

**Background**: Model distillation is a technique where a smaller model learns from a larger, more capable teacher model, often used to reduce cost and compute. Frontier AI models are extremely expensive to train, and distillation allows catching up quickly. The US has been considering regulations on open-weight models due to national security concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://openlm.ai/kimi-k3/">Kimi K3 - openlm.ai</a></li>
<li><a href="https://platform.kimi.ai/docs/guide/kimi-k3-quickstart">Kimi K3 - Kimi API Platform</a></li>

</ul>
</details>

**Discussion**: The community is divided: some argue distillation is inevitable and not an 'attack', while others worry about national security implications and cost-effectiveness. One user found Kimi K3 consumed much more compute on a task compared to GPT-5.6, suggesting it may be less efficient despite lower token prices.

**Tags**: `#AI`, `#large language models`, `#distillation`, `#open-source`, `#geopolitics`

---

<a id="item-5"></a>
## [If You Build It, They Will Come](https://www.benlandautaylor.com/p/if-you-build-it-they-will-come) ⭐️ 7.0/10

The essay argues that communities require active participation and building, rather than passive consumption, challenging the common consumer attitude towards social scenes. This perspective matters because it reframes community building as a personal responsibility in tech culture and grassroots movements, potentially combating social alienation. The piece uses metaphors like wild blueberry bushes to illustrate that social scenes do not appear automatically. It scored 7.0/10 with high community engagement of 230 points and 83 comments.

hackernews · barry-cotter · Jul 18, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48959090)

**Background**: Community building refers to the intentional effort to create and maintain social connections, shared spaces, and collective activities. Many people assume social scenes arise naturally, but this essay argues they require active cultivation, a mindset especially relevant in tech circles where passive consumption is common.

**Discussion**: Comments highlight the vulnerability of being the 'social fabric' and the risk of toxic inner dialogues when efforts aren't reciprocated. They also note a generational rift in passing down grassroots institutions, contrasting past abundance with current alienation.

**Tags**: `#community building`, `#social dynamics`, `#grassroots`, `#tech culture`, `#essay`

---

<a id="item-6"></a>
## [Fable 5 vs GPT-5.6 Sol on NP-Hard: Does /goal Help?](https://charlesazam.com/blog/fable-5-gpt-5-6-sol-goal/) ⭐️ 7.0/10

The blog post compares the performance of Fable 5 (Anthropic) and GPT-5.6 Sol (OpenAI) on an NP-hard problem, evaluating whether the /goal directive improves results. This comparison provides practical insights into the effectiveness of the /goal feature in AI coding assistants, potentially guiding developer tool choices, and highlights the ongoing competition between Anthropic and OpenAI in the coding assistant market. The evaluation found that /goal works better for single-track investigations or small-scale scatter/gather tasks, while GPT-5.6 Sol outperforms Fable 5 on the Artificial Analysis Coding Agent Index, using fewer tokens and lower cost.

hackernews · couAUIA · Jul 18, 11:00 · [Discussion](https://news.ycombinator.com/item?id=48956879)

**Background**: NP-hard problems are computationally challenging to solve optimally, making them a useful benchmark for AI reasoning. The /goal directive is a feature in some AI coding tools like Codex that sets an ongoing background objective. Fable 5 and GPT-5.6 Sol are the latest coding-focused models from Anthropic and OpenAI, respectively, competing in the AI-assisted programming space.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://openai-dotcom-git-main-openai.vercel.app/index/gpt-5-6/">GPT - 5 . 6 : Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://github.com/jackson-video-resources/codex-goal-directive">GitHub - jackson-video-resources/codex- goal - directive : Set Codex...</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed sentiments: some users find Claude (Fable) slow and ineffective compared to Codex (GPT-based), while others note that /goal helps maintain focus in long sessions. There is also a view that GPT models are inherently better at optimization problems.

**Tags**: `#AI coding assistants`, `#GPT-5`, `#Claude`, `#NP-hard`, `#evaluation`

---

<a id="item-7"></a>
## [Guide to Isolate Claude AI on a Spare Mac](https://ykdojo.github.io/claude-controls-mac/) ⭐️ 7.0/10

A detailed step-by-step guide has been published for setting up a spare Mac to run Claude Code as an isolated AI agent for safe automation and testing. As AI agents gain autonomy, isolating them on separate hardware becomes critical to prevent unintended access or damage, making this guide valuable for developers who want to experiment with Claude Code safely. The guide covers network isolation, containerization, and access control measures, though some commenters argue that virtual machine approaches are more efficient than using dedicated hardware.

hackernews · ykev · Jul 18, 16:12 · [Discussion](https://news.ycombinator.com/item?id=48959392)

**Background**: Claude Code is Anthropic's agentic coding tool that can understand codebases, edit files, and run commands autonomously. Running such agents in an isolated environment prevents potential security risks like network escapes or system compromise.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Discussion**: Commenters offered alternative isolation methods using libvirt VMs and scripted resets. Some expressed skepticism about practical use cases, while others emphasized network-level protection via VLANs or firewalls.

**Tags**: `#AI Safety`, `#Claude`, `#Mac`, `#Isolation`, `#Automation`

---

<a id="item-8"></a>
## [Goodbye, Bikesheds: A Reflection on PHK's Legacy](https://queue.acm.org/detail.cfm?id=3818307) ⭐️ 7.0/10

This ACM Queue article reflects on the Bikeshed Problem (Parkinson's Law of Triviality) and the enduring influence of Poul-Henning Kamp (PHK), the FreeBSD developer who popularized the term 'bikeshedding' in open source communities. The article highlights a persistent challenge in collaborative software development—disproportionate focus on trivial details—and celebrates PHK's contributions to both technical infrastructure and project management philosophy. It matters because understanding bikeshedding can help teams make better decisions and avoid wasted effort. The term 'bikeshedding' originated from a 1999 FreeBSD mailing list post by PHK, illustrating how committees spend inordinate time on trivial decisions like what color to paint a bikeshed. The article also notes PHK's technical legacy, including the MD5crypt password hashing algorithm and contributions to FreeBSD kernel, networking, and security.

hackernews · Ygg2 · Jul 18, 17:27 · [Discussion](https://news.ycombinator.com/item?id=48960155)

**Background**: Parkinson's Law of Triviality, commonly known as 'bikeshedding,' states that organizations give disproportionate weight to trivial issues because they are easy to understand and discuss. Poul-Henning Kamp is a prominent FreeBSD developer who not only coined the term in open source but also made major contributions to BSD systems, including the kernel, networking stack, and security features. His MD5crypt algorithm was widely used for password hashing before more secure alternatives emerged.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Law_of_triviality">Law of triviality - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Poul-Henning_Kamp">Poul-Henning Kamp - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted the concept of reversible decisions as a solution to bikeshedding, suggesting that trivial decisions should be made quickly by whoever volunteers. One commenter provided additional context on PHK's MD5crypt algorithm, linking to its original commit history. Others debated age restrictions in technology and their impact on FOSS.

**Tags**: `#open source`, `#project management`, `#bikeshedding`, `#technical debt`, `#PHK`

---

<a id="item-9"></a>
## [SQLite Query Explainer: Interactive Browser Tool](https://simonwillison.net/2026/Jul/18/sqlite-query-explainer/#atom-everything) ⭐️ 7.0/10

Simon Willison created an interactive SQLite query explainer tool that runs entirely in the browser using Pyodide and WebAssembly. The tool adds explanatory annotations to the output of EXPLAIN and EXPLAIN QUERY PLAN commands. This tool lowers the barrier for developers to understand SQLite query execution plans, potentially improving database performance optimization. By running SQLite in the browser, it eliminates the need for local setup and makes learning accessible. The tool runs SQLite in Python via Pyodide, which is a Python distribution for the browser based on WebAssembly. The author notes that he cannot fully verify the correctness of explanations, so users should approach with caution.

rss · Simon Willison · Jul 18, 17:19

**Background**: Pyodide is a Python port to WebAssembly, allowing Python code to run in the browser. WebAssembly (Wasm) is a binary instruction format for a stack-based virtual machine, designed as a portable compilation target. SQLite's EXPLAIN QUERY PLAN command provides a high-level description of the query execution plan, but its output can be cryptic for beginners.

<details><summary>References</summary>
<ul>
<li><a href="https://pyodide.org/en/stable/console.html">pyodide .org/en/stable/console.html</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>
<li><a href="https://sqlite.org/eqp.html">EXPLAIN QUERY PLAN - SQLite</a></li>

</ul>
</details>

**Tags**: `#sqlite`, `#sql`, `#query-explanation`, `#developer-tools`, `#webassembly`

---

<a id="item-10"></a>
## [Anthropic Reverses Plan, Makes Claude Fable 5 Permanent in Higher Tiers](https://simonwillison.net/2026/Jul/18/claude-make-fable-5-permanent/#atom-everything) ⭐️ 7.0/10

Anthropic announced that starting July 20, 2026, Claude Fable 5 will be permanently included in Max and Team Premium subscription plans at 50% of limits, reversing a previous plan to remove it. Pro and Team Standard users get continued access via usage credits and a one-time $100 credit. This policy reversal highlights competitive pressure from rival models like GPT-5.6 Sol and Kimi 3, which made it untenable for Anthropic to exclude its best model from subscriptions. It directly impacts users by ensuring top-tier model access for subscribers, and reflects the dynamic landscape of AI model pricing and availability. The $20/month plan still lacks Fable 5 access; only Max ($100/month) and Team Premium ($200/month) plans include it at 50% usage limits. The original removal plan was driven by compute capacity concerns, and the reversal may require Anthropic to divert GPU resources from training to serving.

rss · Simon Willison · Jul 18, 06:00

**Background**: Claude Fable 5 is Anthropic's most advanced AI model, excelling in long-horizon reasoning and software engineering tasks. Anthropic had planned to remove it from subscriptions to manage compute costs, but competitive offerings like OpenAI's GPT-5.6 Sol (which outperforms Fable 5 in some benchmarks) and Moonshot AI's Kimi K3 threatened to lure users away, forcing the company to reconsider.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5</a></li>
<li><a href="https://openai-dotcom-git-main-openai.vercel.app/index/gpt-5-6/">GPT - 5 . 6 : Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://www.kimi.com/">Kimi AI with K3 | Built for Agentic Coding & Knowledge Work</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Claude`, `#Anthropic`, `#pricing`, `#LLMs`

---

<a id="item-11"></a>
## [fsync inside WAL lock degrades concurrency](https://www.reddit.com/r/programming/comments/1v08tqo/the_fsync_inside_the_wal_lock/) ⭐️ 7.0/10

A recent analysis highlights the performance impact of performing fsync while holding the WAL write lock, contrasting with the read path where the lock is released before I/O. This distinction can significantly affect database transaction throughput and response times, especially under high concurrency workloads, making it a crucial design consideration for database developers. For WAL writes, the exclusive lock is held throughout the fsync call, causing subsequent writes to queue up, whereas reads release the lock before initiating I/O, allowing concurrent reads to proceed.

reddit · r/programming · /u/dfbaggins · Jul 18, 22:06

**Background**: Write-Ahead Logging (WAL) is a standard technique used by databases to ensure durability: changes are first written to a log before being applied to data pages. The fsync() system call forces buffered data to be written to persistent storage; when called inside a lock, it can become a serialization bottleneck.

<details><summary>References</summary>
<ul>
<li><a href="https://frn.sh/pgfsync/">The lock around WAL flush</a></li>
<li><a href="https://www.postgresql.org/docs/current/wal-intro.html">PostgreSQL: Documentation: 18: 28.3. Write-Ahead Logging (WAL)</a></li>

</ul>
</details>

**Tags**: `#databases`, `#wal`, `#fsync`, `#storage`, `#performance`

---

<a id="item-12"></a>
## [Learn Formal Verification with Lean: Part 1 Tutorial](https://www.reddit.com/r/programming/comments/1uzvfar/tutorial_introduction_to_formal_verification_with/) ⭐️ 7.0/10

A new tutorial introduces formal verification using the Lean theorem prover, covering basic concepts and practical examples. As software correctness becomes increasingly critical, formal verification tools like Lean help developers prove correctness mathematically, reducing bugs in safety-critical systems. The tutorial is Part 1 of a series, likely targeting developers with some programming experience but no prior knowledge of formal verification or Lean.

reddit · r/programming · /u/badcryptobitch · Jul 18, 13:06

**Background**: Formal verification is a mathematical approach to proving the correctness of systems against a formal specification. Lean is an open-source theorem prover and functional programming language that enables constructing formal proofs. It has gained traction in both mathematics and software verification communities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lean_theorem_prover">Lean theorem prover</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_verification">Formal verification</a></li>

</ul>
</details>

**Tags**: `#formal verification`, `#Lean`, `#programming languages`, `#tutorial`

---

<a id="item-13"></a>
## [Beyond Retries: Alternative Resilience Patterns](https://www.reddit.com/r/programming/comments/1v05z0d/sometimes_the_most_resilient_thing_a_system_can/) ⭐️ 7.0/10

The Reddit post argues that excessive reliance on retries can harm system resilience and introduces alternative patterns like circuit breaker and bulkhead for more robust distributed systems. This challenges the default retry approach, which can cause cascading failures, and promotes more sophisticated fault tolerance strategies that are critical for modern microservices and distributed architectures. The post likely emphasizes that retries can worsen failures under load, while circuit breakers prevent repeated calls to unhealthy services and bulkheads isolate resource pools to limit blast radius.

reddit · r/programming · /u/madflojo · Jul 18, 20:07

**Background**: In distributed systems, retry is a common technique to handle transient failures, but aggressive retries can lead to cascading failures. Alternative patterns like circuit breaker (which monitors failures and opens the circuit to stop calls) and bulkhead (which partitions resources to limit blast radius) provide more resilience. These patterns are part of a broader resilience engineering toolkit used in microservices and cloud computing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bulkhead_pattern">Bulkhead pattern</a></li>
<li><a href="https://en.wikipedia.org/wiki/Circuit_breaker_pattern">Circuit breaker pattern</a></li>

</ul>
</details>

**Tags**: `#resilience`, `#distributed systems`, `#software engineering`

---

<a id="item-14"></a>
## [Zilog Z80 Turns 50: A Microprocessor Milestone](https://www.reddit.com/r/programming/comments/1v01zwd/the_zilog_z80_has_turned_50/) ⭐️ 6.0/10

The Zilog Z80 microprocessor celebrated its 50th anniversary in 2026, marking five decades since its initial release in 1976. The Z80 was a cornerstone of early personal computing, powering iconic systems like the ZX Spectrum and CP/M machines, and its longevity influenced embedded systems and retro computing communities. The Z80 was designed by Zilog to be software-compatible with the Intel 8080 while offering better integration and performance; Zilog discontinued the standalone Z80 chip in 2024 after 48 years of production.

reddit · r/programming · /u/namanyayg · Jul 18, 17:32

**Background**: The Z80 is an 8-bit microprocessor first released in 1976. It was widely used in home computers, game consoles like Pac-Man arcade machines, and industrial embedded systems. Its architecture influenced many subsequent processors, and it remained in production for decades due to its popularity in legacy systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zilog_Z80">Zilog Z80 - Wikipedia</a></li>
<li><a href="https://arstechnica.com/gadgets/2024/04/after-48-years-zilog-is-killing-the-classic-standalone-z80-microprocessor-chip/">After 48 years, Zilog is killing the classic standalone Z80 ...</a></li>

</ul>
</details>

**Tags**: `#hardware`, `#history`, `#Z80`, `#microprocessor`

---