---
layout: default
title: "Horizon Summary: 2026-06-12 (EN)"
date: 2026-06-12
lang: en
---

> From 27 items, 14 important content pieces were selected

---

1. [AMD's RCE Vulnerability Patched with CRC-32 Instead of Crypto](#item-1) ⭐️ 9.0/10
2. [Homebrew 6.0.0 Released with Tap Trust and Linux Sandboxing](#item-2) ⭐️ 8.0/10
3. [Demand Human Effort for Human Attention](#item-3) ⭐️ 8.0/10
4. [Xiaomi Open-Sources MiMo Code AI Coding Assistant](#item-4) ⭐️ 8.0/10
5. [Anthropic Apologizes for Secret Claude Fable Guardrails](#item-5) ⭐️ 8.0/10
6. [Claude Fable 5: Mid-Tier Coding Performance with Cheating Issues](#item-6) ⭐️ 8.0/10
7. [Lines of Code: A Misleading Metric in the AI Era](#item-7) ⭐️ 8.0/10
8. [Adaptive Video Tokenization via Temporal Redundancy Masking](#item-8) ⭐️ 8.0/10
9. [Petition to Withdraw Canada's Bill C-22](#item-9) ⭐️ 7.0/10
10. [Waymo Premier: $30/month Subscription for Priority Rides](#item-10) ⭐️ 7.0/10
11. [Datasette 1.0a33 Extends JSON Extras API to Rows and Queries](#item-11) ⭐️ 7.0/10
12. [Symbolic Regression vs. LLMs: Still Relevant?](#item-12) ⭐️ 7.0/10
13. [uv 0.11.21 Released with New CPython Versions and Preview Features](#item-13) ⭐️ 6.0/10
14. [FablePool: Crowdfund AI Projects via Prompts](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [AMD's RCE Vulnerability Patched with CRC-32 Instead of Crypto](https://mrbruh.com/amd2/) ⭐️ 9.0/10

A remote code execution vulnerability in AMD software was disclosed, and AMD's patch replaces proper cryptographic signature verification with a non-cryptographic CRC-32 check, leaving systems trivially exploitable if the webserver is compromised. This is critical because it shows AMD's inadequate security response, potentially affecting millions of systems and undermining trust in supply chain security. The use of CRC-32, which is designed for error detection not security, means an attacker who compromises the update server can easily inject malicious code. The vulnerability allows remote code execution via a man-in-the-middle attack or webserver compromise. AMD's fix only adds HTTPS (preventing MITM) but uses CRC-32 for executable integrity, which is trivial to forge.

hackernews · MrBruh · Jun 11, 16:03 · [Discussion](https://news.ycombinator.com/item?id=48492215)

**Background**: CRC-32 is a cyclic redundancy check used for detecting accidental data corruption, not for security. Cryptographic signatures (e.g., RSA, ECDSA) are required to prevent forgery. This vulnerability highlights the importance of proper code signing in software update mechanisms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cyclic_redundancy_check">Cyclic redundancy check - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community expressed outrage and disbelief, calling AMD's fix 'clueless' and 'ridiculous'. Commenters noted that MITM attacks are realistic and that AMD has a history of poor software quality. Some also reported seeing unexpected console pop-ups related to the issue.

**Tags**: `#security`, `#vulnerability`, `#AMD`, `#RCE`, `#supply chain`

---

<a id="item-2"></a>
## [Homebrew 6.0.0 Released with Tap Trust and Linux Sandboxing](https://brew.sh/2026/06/11/homebrew-6.0.0/) ⭐️ 8.0/10

Homebrew 6.0.0 introduces a mandatory tap trust security mechanism, a faster and smaller default internal JSON API, sandboxing on Linux via Bubblewrap, and initial support for macOS 27 (Golden Gate). This major release enhances security and performance for millions of macOS and Linux users, addressing long-standing concerns about third-party tap safety and Linux compatibility. The new tap trust mechanism reduces the risk of malicious code execution, while Linux sandboxing makes Homebrew a more viable option on Linux distributions. The tap trust mechanism requires users to explicitly trust third-party taps before their code is evaluated, and the new JSON API is now the default, offering faster metadata retrieval. Linux sandboxing uses Bubblewrap to isolate build processes, improving system stability.

hackernews · mikemcquaid · Jun 11, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48490024)

**Background**: Homebrew is a popular open-source package manager for macOS and Linux, allowing users to install software from the command line. Taps are third-party repositories that extend Homebrew's package selection, but they have historically posed security risks because their code runs with user privileges. The new trust mechanism addresses this by requiring explicit user approval.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.brew.sh/Tap-Trust">Homebrew Documentation: Tap Trust</a></li>
<li><a href="https://alternativeto.net/news/2026/6/homebrew-6-0-brings-tap-trust-security-mechanism-smaller-json-api-and-linux-sandboxing/">Homebrew 6.0 brings tap trust security mechanism, smaller ...</a></li>
<li><a href="https://news.linxi.com.au/news/homebrew-600-introduces-mandatory-tap-trust-and-macos-27-support">Homebrew 6.0.0 release: Tap trust, Linux sandboxing , macOS 27 ...</a></li>

</ul>
</details>

**Discussion**: Community comments express gratitude for the maintainers' long-term dedication, with one former maintainer noting 16+ years of service. Some users discuss switching to alternatives like Nix or mise, citing reproducibility or ease of use, while others praise Homebrew's improvements and its role on immutable Linux distributions.

**Tags**: `#package manager`, `#Homebrew`, `#macOS`, `#Linux`, `#security`

---

<a id="item-3"></a>
## [Demand Human Effort for Human Attention](https://tombedor.dev/human-attention-and-human-effort/) ⭐️ 8.0/10

A blog post argues that when requesting human attention (e.g., code reviews, emails), one must demonstrate human effort, critiquing the flood of AI-generated PRs and communications that degrade team collaboration. This matters because the increasing use of AI-generated content in professional settings is eroding trust and collaboration, leading to ignored PRs and frustrated teams. It calls for a cultural shift to maintain human accountability. The post highlights that AI-generated PRs often lack the human touch needed for effective review, and that reviewers subconsciously deprioritize such work. The author suggests that if you want human attention, you must put in human effort.

hackernews · jjfoooo4 · Jun 11, 23:01 · [Discussion](https://news.ycombinator.com/item?id=48497609)

**Background**: In software engineering, code reviews and team communications rely on human judgment and effort. With the rise of AI tools like Claude and ChatGPT, some developers generate large volumes of AI-produced code and messages, expecting the same level of attention as human-crafted work. This creates an imbalance where the effort to produce is low but the effort to review remains high.

**Discussion**: Commenters share experiences of coworkers flooding teams with AI-generated PRs and communications, leading to ignored work and frustration. Some note that AI-generated content often lacks human touch and review, while others discuss the need for new conventions for AI-to-human communication.

**Tags**: `#AI`, `#code review`, `#software engineering`, `#team collaboration`, `#productivity`

---

<a id="item-4"></a>
## [Xiaomi Open-Sources MiMo Code AI Coding Assistant](https://mimo.xiaomi.com/mimocode) ⭐️ 8.0/10

Xiaomi has released MiMo Code, an open-source AI coding assistant forked from OpenCode, featuring persistent memory, subagent orchestration, and goal-driven autonomous loops. This move challenges closed-source alternatives like Claude Code and promotes open standards in AI-assisted development, potentially lowering switching costs for developers and fostering community innovation. MiMo Code retains all core OpenCode capabilities (multiple providers, TUI, LSP, MCP, plugins) and adds persistent memory, intelligent context management, subagent orchestration, goal-driven autonomous loops, compose workflows, and self-improvement via dream/distill.

hackernews · apeters · Jun 11, 14:27 · [Discussion](https://news.ycombinator.com/item?id=48490826)

**Background**: Agentic coding refers to AI assistants that autonomously execute high-level tasks rather than just suggesting code. OpenCode is an open-source terminal-native AI coding agent that MiMo Code builds upon. Xiaomi's release aligns with a trend toward open-source coding harnesses, contrasting with closed-source tools like Claude Code.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/XiaomiMiMo/MiMo-Code">GitHub - XiaomiMiMo/ MiMo-Code</a></li>
<li><a href="https://opencode.ai/docs/">Intro | AI coding agent built for the terminal - opencode .ai</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agentic_coding">Agentic coding</a></li>

</ul>
</details>

**Discussion**: The community largely applauds the open-source move, with commenters praising Xiaomi's transformation and noting that coding harnesses should be open to minimize switching costs. Some highlight MiMo Code's advanced features like persistent memory and subagent orchestration, contrasting it favorably with closed-source alternatives.

**Tags**: `#AI coding assistant`, `#open source`, `#Xiaomi`, `#agentic coding`, `#LLM`

---

<a id="item-5"></a>
## [Anthropic Apologizes for Secret Claude Fable Guardrails](https://www.theverge.com/ai-artificial-intelligence/948280/anthropic-claude-fable-invisible-distillation-guardrail) ⭐️ 8.0/10

Anthropic admitted it secretly deployed an invisible guardrail in Claude Fable 5 that silently degraded responses for users suspected of model distillation, and has now apologized and reversed the policy. This incident erodes trust in AI companies, as users discovered their interactions were being covertly manipulated without consent, raising serious concerns about transparency and corporate accountability in the AI industry. The guardrail was documented in Fable's 319-page system card and used methods like model downgrading to Claude Opus 4.8 when distillation attempts were detected, affecting not only rivals but also legitimate researchers.

hackernews · rarisma · Jun 11, 12:05 · [Discussion](https://news.ycombinator.com/item?id=48489229)

**Background**: Model distillation is a technique where a smaller model is trained to mimic a larger, more capable model, often used to create cheaper alternatives. AI companies like Anthropic guard against this to protect their competitive advantage. The invisible guardrail was a covert measure that silently altered responses without user knowledge.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/948280/anthropic-claude-fable-invisible-distillation-guardrail">Anthropic apologizes for invisible Claude Fable guardrails</a></li>
<li><a href="https://www.ai-market-watch.com/news/anthropic-apologizes-for-hidden-guardrails-in-claude-fable-5-throttling-rivals-a-g8fuy9">Anthropic apologizes for invisible Claude Fable guardrails that...</a></li>
<li><a href="https://letsdatascience.com/news/anthropic-revises-invisible-guardrail-on-claude-fable-6da783a4">Anthropic revises invisible guardrail on Claude Fable</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong distrust, noting that the invisible nature of the guardrail makes it impossible to verify if it has truly been removed. Some criticized Anthropic's paternalistic approach, arguing it undermines the empowering promise of AI and sets a dangerous precedent for covert manipulation.

**Tags**: `#AI ethics`, `#Anthropic`, `#guardrails`, `#trust`, `#transparency`

---

<a id="item-6"></a>
## [Claude Fable 5: Mid-Tier Coding Performance with Cheating Issues](https://www.endorlabs.com/learn/claude-fable-5-mythos-grade-hype) ⭐️ 8.0/10

A critical analysis of Claude Fable 5 reveals mid-tier coding performance with high timeout rates and memorization-based cheating on benchmarks, including 38 confirmed cheating instances out of 200. This matters because it challenges Anthropic's marketing claims of Fable 5 being a top-tier coding model, highlighting significant reliability and integrity issues that affect trust in AI benchmarks. The model achieved four 'hall-of-fame firsts' but also set a record for timeouts. Cheating occurred via memorization of upstream fixes from training data, producing character-for-character identical patches.

hackernews · bugvader · Jun 11, 16:03 · [Discussion](https://news.ycombinator.com/item?id=48492210)

**Background**: Claude Fable 5 is Anthropic's latest frontier model, marketed for complex coding and autonomous tasks. Benchmark evaluations like FrontierBench measure model performance on coding challenges, but memorization of training data can inflate scores, undermining validity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://docs.aws.amazon.com/bedrock/latest/userguide/model-card-anthropic-claude-fable-5.html">Claude Fable 5 - Amazon Bedrock</a></li>

</ul>
</details>

**Discussion**: Community comments report mixed experiences: one user found Fable 5 indistinguishable from Opus on large tasks after spending $2K, while another noted common-sense mistakes in an auction site test. Gwern highlighted the cheating and timeout issues as significant flaws.

**Tags**: `#AI`, `#coding benchmarks`, `#Claude`, `#model evaluation`, `#machine learning`

---

<a id="item-7"></a>
## [Lines of Code: A Misleading Metric in the AI Era](https://curlewis.co.nz/posts/lines-of-code-got-a-better-publicist/) ⭐️ 8.0/10

A blog post argues that lines of code (LoC) is a poor productivity metric, especially with AI-generated code, and criticizes companies using AI as an excuse for layoffs without evidence. This critique challenges the growing trend of measuring software productivity by LoC, which can lead to unmaintainable code and misguided layoffs, affecting engineers and the industry's focus on quality. The post highlights that the reasons for rejecting LoC as a metric—such as its inability to measure code quality—remain unchanged even with AI, and that AI-generated code often requires more maintenance.

hackernews · RyeCombinator · Jun 11, 12:26 · [Discussion](https://news.ycombinator.com/item?id=48489402)

**Background**: Lines of code has long been criticized as a flawed productivity metric because it rewards verbosity over quality. With the rise of AI code generation, some companies have revived LoC as a measure, claiming AI boosts output, but this ignores the complexity of software engineering and the risk of accumulating technical debt.

**Discussion**: Commenters largely agree with the critique, noting that AI hype has led to absurd metrics like "1 million LoC per engineer per month." They emphasize that code output is not the same as value, and that companies use AI as a convenient excuse for layoffs.

**Tags**: `#AI`, `#software engineering`, `#productivity`, `#metrics`, `#code quality`

---

<a id="item-8"></a>
## [Adaptive Video Tokenization via Temporal Redundancy Masking](https://www.reddit.com/r/MachineLearning/comments/1u2u9bb/adaptive_tokenisation_via_temporal_redundancy/) ⭐️ 8.0/10

Researchers propose a parameter-free adaptive token allocation method for video tokenization that drops latent positions with minimal temporal change, achieving efficient compression without extra computation. The method uses a fixed threshold on temporal-L1 differences in latent space and reconstructs dropped positions with a lightweight Latent Inpainting Transformer (LIT). This work eliminates the computational overhead of existing adaptive tokenization methods, offering a 31x speedup over continuous baselines and 2x over discrete baselines. It enables content-driven compression that aggressively compresses static scenes while retaining detail in dynamic sequences, which is valuable for video streaming, storage, and real-time processing. The method requires only a single encoder pass and one LIT forward pass, with no auxiliary routing networks. It was evaluated on TokenBench and DAVIS benchmarks, achieving competitive reconstruction fidelity while delivering significant speedups.

reddit · r/MachineLearning · /u/chhaya_35 · Jun 11, 09:32

**Background**: Video tokenization converts video frames into discrete tokens for efficient processing by models. Adaptive tokenization aims to allocate more tokens to complex regions and fewer to static ones, but existing methods require iterative searches or trained networks, adding computational cost. This work exploits temporal redundancy in latent space to avoid such overhead.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.06158">Adaptive Tokenisation Via Temporal Redundancy Masking And ...</a></li>
<li><a href="https://www.semanticscholar.org/paper/Adaptive-Tokenisation-Via-Temporal-Redundancy-And-Dave-Patkuri/7048f10d2a4e7e2d7b180a46391da15187a0e4b8/figure/2">Adaptive Tokenisation Via Temporal Redundancy Masking And ...</a></li>

</ul>
</details>

**Discussion**: The Reddit discussion is positive, with users praising the novelty and efficiency of the approach. Some commenters discuss potential applications in video compression and real-time systems, while others question the threshold sensitivity and reconstruction quality in highly dynamic scenes.

**Tags**: `#video tokenization`, `#latent space`, `#temporal redundancy`, `#compression`, `#machine learning`

---

<a id="item-9"></a>
## [Petition to Withdraw Canada's Bill C-22](https://www.ourcommons.ca/petitions/en/Petition/Sign/e-7416) ⭐️ 7.0/10

A petition has been launched on the House of Commons website calling for the withdrawal of Canada's Bill C-22, the Lawful Access Act, 2026, which critics argue threatens privacy and harms the domestic tech industry. If enacted, Bill C-22 would require telecoms and digital platforms to retain metadata for up to one year and could grant the Public Safety Minister secret powers to compel design changes, impacting privacy rights and Canada's tech sector competitiveness. The petition, e-7416, was created in April 2025 and has garnered community support, with a SECU Committee meeting scheduled for clause-by-clause review and voting on amendments, potentially the final meeting.

hackernews · hmokiguess · Jun 11, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48491830)

**Background**: Bill C-22, introduced in March 2026, is a lawful access bill that expands police powers to obtain digital data. Critics, including tech companies like Apple, Meta, and Signal, as well as U.S. House committees, have raised concerns about its privacy implications and potential to weaken encryption.

<details><summary>References</summary>
<ul>
<li><a href="https://www.michaelgeist.ca/2026/03/the-lawful-access-privacy-risks-unpacking-bill-c-22s-expansive-metadata-retention-requirements/">The Lawful Access Privacy Risks: Unpacking Bill C-22 's Expansive...</a></li>
<li><a href="https://www.cbc.ca/news/politics/bill-c-22-encryption-cybersecurity-9.7213776">Liberals to amend police data interception bill following searing...</a></li>

</ul>
</details>

**Discussion**: Commenters express skepticism about the petition's impact but emphasize the importance of raising awareness. Some note that the bill, along with C-34, could further erode privacy and harm Canada's consumer tech sector, while others point to upcoming committee meetings as a critical juncture.

**Tags**: `#privacy`, `#legislation`, `#Canada`, `#tech policy`

---

<a id="item-10"></a>
## [Waymo Premier: $30/month Subscription for Priority Rides](https://waymo.com/blog/2026/06/waymo-premier/) ⭐️ 7.0/10

Waymo has launched Waymo Premier, a $30/month subscription service that provides priority access to rides and cash back on fares. This marks a shift toward premium subscription models in autonomous ride-hailing, potentially creating a two-tier service that raises concerns about economic stratification and accessibility. The subscription pays for itself if a user spends over $300 per month on rides. Cash back features are particularly attractive for those expensing rides through employers.

hackernews · boulos · Jun 11, 16:10 · [Discussion](https://news.ycombinator.com/item?id=48492304)

**Background**: Waymo is a leading autonomous driving company and a subsidiary of Alphabet Inc., operating robotaxis in several U.S. cities. Subscription services are common in transportation, but this is one of the first for autonomous ride-hailing.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Waymo">Waymo - Wikipedia</a></li>
<li><a href="https://builtin.com/articles/waymo-robotaxis">Waymo Explained: Alphabet’s Autonomous Vehicle Company | Built In</a></li>

</ul>
</details>

**Discussion**: Community comments highlight security concerns (e.g., inability to intervene when a Waymo is blocked), economic stratification (K-shaped economy), and comparisons to public transit ($104/month for unlimited BART). Some see cash back as a perk for business travelers.

**Tags**: `#autonomous vehicles`, `#subscription service`, `#Waymo`, `#transportation`, `#economy`

---

<a id="item-11"></a>
## [Datasette 1.0a33 Extends JSON Extras API to Rows and Queries](https://simonwillison.net/2026/Jun/11/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a33 extends the `?_extra=` pattern, previously available only for table endpoints, to row and query JSON pages, allowing API clients to request specific JSON keys and reduce over-fetching. This release is a significant step toward Datasette 1.0 stable, providing a stable, documented JSON API that improves flexibility and performance for developers building on Datasette. The `?_extra=` mechanism was first introduced in Datasette 1.0a3 for tables; 1.0a33 extends it to rows and queries, and the pattern is now documented in the official JSON API documentation.

rss · Simon Willison · Jun 11, 15:26

**Background**: Datasette is an open-source tool for exploring and publishing data as interactive web pages and JSON APIs. The `?_extra=` parameter allows clients to opt into additional JSON keys (e.g., row counts, column types) beyond the default response, reducing unnecessary data transfer and SQL queries.

<details><summary>References</summary>
<ul>
<li><a href="http://datasette.io/blog/2026/api-extras/">Datasette 1.0a33 with JSON extras in the API - Datasette Blog</a></li>
<li><a href="https://simonwillison.net/2026/Jun/11/datasette/">Release: datasette 1.0a33 - simonwillison.net</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#release`, `#API`, `#JSON`, `#open-source`

---

<a id="item-12"></a>
## [Symbolic Regression vs. LLMs: Still Relevant?](https://www.reddit.com/r/MachineLearning/comments/1u2yqnu/is_symbolic_regression_still_a_thing_given_llms/) ⭐️ 7.0/10

A Reddit discussion questions whether symbolic regression (SR) remains relevant given the increasing power of large language models (LLMs) in code generation and symbolic tasks. This debate highlights the evolving landscape of AI-driven scientific discovery, where LLMs may complement or compete with traditional SR methods, impacting fields like physics and biology that rely on interpretable models. The post references an ETH Zurich tutorial on SR and notes that LLMs can directly tackle SR tasks, but SR offers interpretability that LLMs lack as black-box models.

reddit · r/MachineLearning · /u/omomom42 · Jun 11, 13:13

**Background**: Symbolic regression is a machine learning technique that searches for mathematical expressions to fit data, without assuming a fixed model structure. It is valued for producing interpretable equations. Large language models (LLMs) like GPT-4 can generate code and solve symbolic problems, raising questions about the future of specialized SR methods.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Symbolic_regression">Symbolic regression - Wikipedia</a></li>
<li><a href="https://arxiv.org/abs/2107.14351">[2107.14351] Contemporary Symbolic Regression Methods and ...</a></li>
<li><a href="https://github.com/deep-symbolic-mathematics/LLM-SR">GitHub - deep- symbolic -mathematics/LLM-SR: [ICLR 2025 Oral ...</a></li>

</ul>
</details>

**Discussion**: Comments likely compare SR's interpretability and sample efficiency with LLMs' flexibility and data hunger, with some arguing SR remains essential for scientific discovery where understanding the model is key.

**Tags**: `#symbolic regression`, `#large language models`, `#machine learning`, `#AI research`

---

<a id="item-13"></a>
## [uv 0.11.21 Released with New CPython Versions and Preview Features](https://github.com/astral-sh/uv/releases/tag/0.11.21) ⭐️ 6.0/10

uv 0.11.21 adds CPython 3.13.14 and 3.14.6, introduces preview features for workspace metadata and single-dependency upgrade, improves performance with parallel Python version discovery, and fixes numerous bugs. This release continues uv's rapid iteration as a fast Python package manager, offering users early access to workspace metadata and targeted upgrades, which are highly requested features for monorepo workflows. Preview features include `environment.root` in workspace metadata and the ability to upgrade a single dependency constraint via `uv upgrade`. Performance gains come from parallel discovery of Python versions for `uv python list`.

github · github-actions[bot] · Jun 11, 18:20

**Background**: uv is a fast Python package and project manager written in Rust, serving as a drop-in replacement for pip, pip-tools, and virtualenv. It is developed by Astral, the company behind the Ruff linter. Workspace metadata helps manage multi-package repositories, and targeted upgrades allow updating a single dependency without affecting others.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/">uv - Astral</a></li>
<li><a href="https://github.com/astral-sh/uv/issues/14394">Is it possible to upgrade just a single package if ... - GitHub</a></li>

</ul>
</details>

**Tags**: `#python`, `#package-manager`, `#release`, `#uv`

---

<a id="item-14"></a>
## [FablePool: Crowdfund AI Projects via Prompts](https://fablepool.com/) ⭐️ 6.0/10

FablePool launched a public platform where users pool money behind a prompt, and an AI agent builds the project in public, with transactions recorded on a public ledger. This concept combines crowdfunding with AI code generation (vibe coding), potentially lowering the barrier for non-developers to fund and create software, but the broken demo and community skepticism highlight serious feasibility and quality concerns. The demo project regressed at milestone 15, changing a working Wikimedia image link to a nonexistent file, and the platform was criticized for unclear licensing (MIT vs. public domain) and lack of quality control.

hackernews · matthewbarras · Jun 11, 21:17 · [Discussion](https://news.ycombinator.com/item?id=48496539)

**Background**: Vibe coding, coined by Andrej Karpathy in 2025, refers to AI-assisted programming where users describe a project in a prompt and accept generated code without thorough review. FablePool extends this by adding a crowdfunding layer, allowing anyone to fund a prompt and have an AI build the project publicly.

<details><summary>References</summary>
<ul>
<li><a href="https://news.linxi.com.au/news/fablepool-launches-public-platform-for-ai-driven-open-source-crowdfunding">FablePool launches public AI funding platform for open-source ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding</a></li>

</ul>
</details>

**Discussion**: Commenters pointed out that the demo build is broken, with one noting a regression from milestone 14 to 15. Others questioned the licensing claim and the viability of funding complex tasks like "Solve Garbage Collection in C# for HFT" for only $200.

**Tags**: `#crowdfunding`, `#AI code generation`, `#vibe coding`, `#open source`, `#prototype`

---