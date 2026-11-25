---
layout: default
title: "Horizon Summary: 2026-11-25 (EN)"
date: 2026-11-25
lang: en
---

> From 33 items, 18 important content pieces were selected

---

1. [PrismML Ships Ternary Bonsai 2.5 27B, a 27B Ternary Model Built for Agents](#item-1) ⭐️ 8.0/10
2. [GreyNoise Uncovers Campaign Breaching Check Point Management Servers via PRNG Flaw](#item-2) ⭐️ 8.0/10
3. [Quad9 deactivates its public DNS service in France over legal blocking demands](#item-3) ⭐️ 8.0/10
4. [Commentary Argues LLM Agents Serve Parent Companies, Not Users](#item-4) ⭐️ 8.0/10
5. [Simon Willison Charts Three LLM Inflection Points in Twelve Months](#item-5) ⭐️ 8.0/10
6. [GPT-6.2 Astra Autonomously Identifies Author of an Anonymous 1808 Yale Sketchbook](#item-6) ⭐️ 8.0/10
7. [OpenAI says GPT-6.2 designed protein minibinders via generated code](#item-7) ⭐️ 7.0/10
8. [Leaked GTA 6 Xbox Build Booted on Windows by Community Recompilers](#item-8) ⭐️ 7.0/10
9. [Splitting one USB-C port into separate USB 3 and USB 2 devices](#item-9) ⭐️ 7.0/10
10. [Blog Post on Brendan Gregg-Style Performance Analysis Sparks Debate](#item-10) ⭐️ 7.0/10
11. [Anthropic Stock Slips Below $83 IPO Price in Premarket Trading](#item-11) ⭐️ 7.0/10
12. [Blog post claims Cloudflare masks origin TLS and IPv4 weaknesses](#item-12) ⭐️ 7.0/10
13. [Tesla and SpaceX Race Toward Year-End All-Stock Merger Deal](#item-13) ⭐️ 7.0/10
14. [Songe: Train Your Local LLM on Idle Compute](#item-14) ⭐️ 6.0/10
15. [Grafana ships security patches across five release branches](#item-15) ⭐️ 6.0/10
16. [VW&\#x27;s Elli launches German V2G program paying EV owners up to €720](#item-16) ⭐️ 6.0/10
17. [Nuro Starts Driverless Lucid Gravity Robotaxi Testing in Bay Area](#item-17) ⭐️ 6.0/10
18. [NVIDIA Details Microduck Sim2Real Obstacle Avoidance Workflow with Isaac Lab and Newton](#item-18) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [PrismML Ships Ternary Bonsai 2.5 27B, a 27B Ternary Model Built for Agents](https://prismml.com/news/bonsai-2-5-27b) ⭐️ 8.0/10

PrismML released Ternary Bonsai 2.5 27B, the largest model in its ternary Bonsai family, derived from the hybrid-attention Qwen3.8-27B with the architecture left unchanged. According to the company&\#x27;s whitepaper, the new version shows marked gains over Ternary Bonsai 2 27B and closes in on the full-precision base model on agentic execution, coding, and multi-turn tool use. The release pushes near-frontier agentic and coding behavior into a footprint small enough to run on consumer hardware, which matters for developers who want private, offline or low-cost local inference instead of API calls. It also feeds the broader debate over whether more parameters at fewer bits can rival fewer parameters at higher precision. Bonsai models are ternary-quantized derivatives of Qwen3.8-27B, and the earlier Bonsai 2 27B reportedly compressed to roughly 8.60GB on disk while retaining about 98.2% of the full FP16 model&\#x27;s intelligence. Caveats worth noting: the headline benchmark claims rest on SWE-bench Verified, which commenters point out is not the most representative benchmark, and there is little dedicated hardware acceleration for ternary weights beyond FPGAs.

hackernews · b0m · Nov 24, 20:08 · [Discussion](https://news.ycombinator.com/item?id=50633922)

**Background**: Ternary \(or 1.58-bit\) quantization stores each weight in one of three states — roughly -1, 0, +1 — instead of 8 or 16 bits, shrinking memory use dramatically while keeping the parameter count of the original model. Unlike standard post-training quantization, which compresses an already-trained FP16 model, ternary approaches are often trained or fine-tuned with ternary weights so the model can adapt to the extreme compression. The Bonsai family applies this to Qwen3.8-27B, a 27-billion-parameter hybrid-attention reasoning model. SWE-bench, the benchmark cited in the discussion, measures whether a model can resolve real GitHub issues in actual Python repositories.

<details><summary>References</summary>
<ul>
<li><a href="https://prismml.com/news/bonsai-2-5-27b">PrismML — Introducing Ternary Bonsai 2.5 27B: Powering ...</a></li>
<li><a href="https://docs.prismml.com/models/bonsai-2-5-27b">Ternary Bonsai 2.5 27B - Bonsai - docs.prismml.com</a></li>
<li><a href="https://www.mindstudio.ai/blog/ternary-bonsai-2-27b-local">Run Bonsai 2 27B Locally on a Mac: Ternary Quantization Explained</a></li>
<li><a href="https://bitnet.xin/blog/158-bit-quantization-why-ternary-weights-are-the-sweet-spot">1.58-bit Quantization Explained | BitNet.XIN | BitNet.XIN</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters shared concrete hands-on numbers: one reported roughly 22–25 tokens/s on a Mac Mini M5 Pro with 24GB RAM using a Q2 GGUF, with about 2s first-token latency and 128k context fitting comfortably in memory. Another ran a personal long-horizon benchmark and saw the same throughput but 17% fewer steps and 29% less total time than Bonsai 2, though the pass rate stayed at 5 of 8. Others questioned the SWE-bench Verified comparison to a frontier model \(suspecting benchmark-tuning, benchmark drift, or a ~6-month capability lag\), asked for head-to-head tests against equivalently small Q1/Q2 quants of Qwen3.8, and wondered whether any hardware besides FPGAs accelerates ternary weights.

**Tags**: `#local-llm`, `#model-quantization`, `#ternary-models`, `#inference-performance`, `#swe-bench`

---

<a id="item-2"></a>
## [GreyNoise Uncovers Campaign Breaching Check Point Management Servers via PRNG Flaw](https://www.greynoise.io/blog/check-point-security-management-servers-intrusion-campaign) ⭐️ 8.0/10

GreyNoise documented an active intrusion campaign against Check Point Security Management Servers, with confirmed activity between October 17 and November 2, 2026 affecting at least 22 organizations globally. The actor exploited Rejetto HFS, whose session-cookie signing key was derived from JavaScript&\#x27;s Math.random\(\); by triggering successive logins at the unauthenticated loginSrp1 endpoint, they harvested enough PRNG output to reconstruct the V8 PRNG state, recover the signing key, and forge an admin session cookie before pivoting into Check Point infrastructure. This is a technically novel disclosure showing that Math.random\(\) can be a practical path to full admin compromise, not just a theoretical weakness, and it puts endpoint-management servers — which typically hold credentials and policy control over entire networks — squarely in attackers&\#x27; sights. It also underscores how AI-assisted offensive tooling is lowering the bar for exploiting obscure cryptographic mistakes. The exploit required remarkably little: koa-session cookies are base64-encoded, signed-but-not-encrypted JSON, so each login handshake handed the attacker the exact ~52-bit double the PRNG had just produced, wrapped inside the cookie itself. The actor also chained multiple vulnerabilities, and investigators link the initial access across victims to CVE-2026-16232, though GreyNoise notes the campaign is likely still ongoing.

hackernews · louiereederson · Nov 24, 16:32 · [Discussion](https://news.ycombinator.com/item?id=50630594)

**Background**: JavaScript&\#x27;s Math.random\(\) is a non-cryptographic PRNG, meaning its output is deterministic given internal state and is not designed to resist prediction. The V8 engine&\#x27;s implementation can be reverse-engineered from a modest number of observed outputs, which is why the OWASP-style rule is to use crypto.randomBytes\(\) or equivalent CSPRNGs for anything security-sensitive. Rejetto HFS is a lightweight file server built on Node.js and Koa, and Check Point Security Management Servers are the central consoles administrators use to configure and monitor Check Point gateways and endpoints.

<details><summary>References</summary>
<ul>
<li><a href="https://www.greynoise.io/blog/check-point-security-management-servers-intrusion-campaign">An Active Intrusion Campaign Against Check Point Security ...</a></li>
<li><a href="https://thehackernews.com/2026/10/attackers-target-rejetto-hfs-flaw-that.html">Attackers Target Rejetto HFS Flaw That Enables Admin Session ...</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random">Math . random () - JavaScript | MDN</a></li>

</ul>
</details>

**Discussion**: Commenters were impressed rather than surprised, with one calling the PRNG an &quot;old friend&quot; and another pasting the exact exploitation steps to highlight how the cookie leaked its own seed. The thread split between those warning that LLM-driven attack automation will soon let unsophisticated criminals swarm any exposed service, and those arguing the real fix is making all random number generators secure by default instead of patching hundreds of misusing applications — plus a lingering question about how initial access was actually obtained and whether victims had management servers exposed to the internet.

**Tags**: `#security`, `#vulnerability-disclosure`, `#prng`, `#nodejs`, `#checkpoint`

---

<a id="item-3"></a>
## [Quad9 deactivates its public DNS service in France over legal blocking demands](https://quad9.net/news/blog/quad9-service-deactivation-in-france/) ⭐️ 8.0/10

Quad9, the Swiss non-profit public DNS resolver, deactivated its service for users in France, with community members confirming that queries to 9.9.9.9 from French networks now return a REFUSED status carrying the extended DNS error code 18 \(Prohibited\) with the message &quot;Service unavailable due to French legal constraints&quot;. The withdrawal follows Quad9&\#x27;s refusal to comply with French demands that it block content at the recursive DNS level. Quad9 is one of the most widely recommended privacy- and security-focused resolvers, so a national-level shutdown illustrates how DNS filtering mandates can effectively remove a service from an entire country rather than target the origin servers hosting disputed content. Because the resolver in use sees all of a user&\#x27;s browsing activity, the case raises broader questions about privacy, censorship and internet fragmentation that affect every French internet user and other resolvers operating there. The block is implemented at the resolver level rather than by network filtering, so French users get an immediate refusal with the diagnostic EDE 18 code instead of an NXDOMAIN or a forged answer. In practice this breaks home setups that rely on Quad9 as an upstream — one commenter&\#x27;s whole LAN appeared to be offline because AdGuard Home could no longer reach its upstream — and workarounds such as DoH/DoT proxies or switching to another resolver only work as long as those paths remain reachable.

hackernews · farrokhi · Nov 24, 08:33 · [Discussion](https://news.ycombinator.com/item?id=50625384)

**Background**: The Domain Name System translates human-readable domain names into IP addresses, and a public recursive resolver like Quad9, Google Public DNS or Cloudflare DNS does that lookup on your behalf instead of your ISP. Quad9 is run by a Swiss non-profit foundation and is known for blocking domains associated with malware and phishing while logging as little as possible. France has increasingly required intermediaries — ISPs and, more recently, DNS resolvers — to block piracy-related sites, and Quad9 argued that putting blocking demands on recursive resolvers does nothing to stop the origin servers that actually deliver the content.

<details><summary>References</summary>
<ul>
<li><a href="https://quad9.net/news/blog/quad9-service-deactivation-in-france/">A public and free DNS service for a better security and privacy | Quad9</a></li>
<li><a href="https://blog.cloudflare.com/quad9-withdrawal-from-france/">Quad9’s withdrawal from France : A canary in the coal... | Cloudflare Blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/Quad9">Quad9 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters verified the shutdown with dig output showing the REFUSED response and French-legal-constraints message, and pointed to two earlier high-engagement Hacker News threads plus a TorrentFreak follow-up for context. One user set up an open caching proxy that forwards to Quad9 over DoH, DoT and plain Do53 with both IPv4 and IPv6, offering it as a drop-in replacement for users in France, while another reported their home network going down because AdGuard Home lost its upstream.

**Tags**: `#DNS`, `#privacy`, `#internet governance`, `#France`, `#Quad9`

---

<a id="item-4"></a>
## [Commentary Argues LLM Agents Serve Parent Companies, Not Users](https://michaelharley.net/posts/2026/11/01/llm-agents-work-for-their-parent-companies-not-for-you/) ⭐️ 8.0/10

A commentary post on michaelharley.net argues that LLM agents ultimately act in the interests of their parent companies rather than their users, using the example of Claude refusing to help scrape Bandcamp because the site disallows LLM access. The piece sparked a large Hacker News debate with 875 points and 368 comments about agent loyalty, site policies, and crawling restrictions. The debate gets at a core question for AI agents: whether they function as neutral tools or as vendor-aligned intermediaries whose refusals reflect provider policies and business incentives. It matters to users who delegate web tasks, to sites deciding whether to block AI crawlers, and to regulators considering fiduciary-style obligations for AI advisors. Commenters split over whether the refusal is legitimate ToS compliance or misplaced corporate loyalty; one notes that ignoring site rules could provoke blocking that reduces agents&\#x27; long-term usefulness, while another argues AI bans also shut out legitimate technical users doing manual research. A separate proposal calls for legally requiring LLMs to act as fiduciaries, similar to legal, financial, and medical advisors.

hackernews · surprisetalk · Nov 24, 12:40 · [Discussion](https://news.ycombinator.com/item?id=50627340)

**Background**: LLM agents are AI systems that use a language model to plan and carry out multi-step tasks, often browsing the web or calling tools on a user&\#x27;s behalf. Their behavior is shaped not only by the user&\#x27;s request but also by provider usage policies, system prompts, and commercial incentives. Websites commonly signal whether automated crawlers are welcome through robots.txt and terms of service, and many have begun blocking AI crawlers. Fiduciary duty is a legal standard requiring an advisor to act in a client&\#x27;s best interest, and researchers have started benchmarking whether LLM agents can meet such obligations.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2607.02814v2">Faithful Delegates? Benchmarking theFiduciary Duties of LLM ...</a></li>
<li><a href="https://www.devtools.tools/blog/blocking-ai-crawlers-with-robots-txt">How to Block AI Crawlers with robots.txt | DevTools</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread is broadly skeptical of the original argument. Lerc proposes treating LLMs as legally obligated fiduciary advisors, while jpatten calls the post flimsy and argues that respecting site policies is necessary for agents&\#x27; long-term utility; jrflo agrees that refusing to break Bandcamp&\#x27;s ToS is correct. throwawayffffas shifts to a practical complaint that site-level AI bans also block legitimate technical users, highlighting the tradeoff between stopping bad crawlers and preserving useful access.

**Tags**: `#AI agents`, `#LLM alignment`, `#AI ethics`, `#AI policy`, `#web scraping`

---

<a id="item-5"></a>
## [Simon Willison Charts Three LLM Inflection Points in Twelve Months](https://simonwillison.net/2026/Nov/24/llm-inflection-points/) ⭐️ 8.0/10

On November 24, 2026 — the one-year anniversary of Claude Opus 4.5&\#x27;s release — Simon Willison published a retrospective built on his keynote at the AI Engineer Code Summit \(San Francisco, November 10–12, 2026\), arguing that LLM and coding-agent capabilities crossed three distinct inflection points in the past twelve months. The post details the first two at length: Opus 4.5 and OpenAI&\#x27;s GPT-5.1 family making coding agents reliably useful in November 2025, and the arrival of &quot;Fable class models&quot; in June/July 2026. The retrospective offers practitioners a concrete framework for spotting when an AI coding tool has crossed from &quot;toy&quot; to &quot;reliable accelerant,&quot; which directly affects how software teams decide to adopt agents into daily workflows. It also highlights how fast the frontier is moving — a model that felt near-impossible to use in early 2025 became the default daily driver within months — and shows that policy events, not just research, can reshape model availability. Willison defines &quot;Fable class models&quot; as systems that, given a defined goal and the necessary tools, will brute-force their way to solving the problem — his example is Claude Fable spinning up its own pyobjc-framework-Quartz screenshot mechanism and a CORS-enabled localhost logging server to debug a Safari display glitch. Notably, Fable 5 was a defanged version of the withheld Claude Mythos and was pulled offline by US export controls for roughly three days before returning on July 1, 2026.

rss · Simon Willison · Nov 24, 23:02

**Background**: Claude Code, Anthropic&\#x27;s terminal-based coding agent, launched on February 24, 2025 alongside Claude 3.7 Sonnet, meaning it was about nine months old when Claude Opus 4.5 arrived on November 24, 2025. &quot;Coding agents&quot; are LLM-driven tools that can read files, run commands and edit code autonomously rather than just answering questions in a chat window, so their usefulness depends heavily on how often the model&\#x27;s default output is correct. Simon Willison is a long-time developer and writer whose ongoing LLM coverage is widely used by engineers to gauge what new models can actually do in practice.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.engineer/code/2026">AI Engineer Code Summit 2026 Recordings: AI Engineering ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Opus_4.5">Claude Opus 4.5</a></li>
<li><a href="https://www.anthropic.com/claude/opus">Claude Opus \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#LLMs`, `#coding agents`, `#AI engineering`, `#Claude Opus`, `#Simon Willison`

---

<a id="item-6"></a>
## [GPT-6.2 Astra Autonomously Identifies Author of an Anonymous 1808 Yale Sketchbook](https://simonwillison.net/2026/Nov/24/astra-historical-mystery/) ⭐️ 8.0/10

History professor Mark Humphries reports that GPT-6.2 Astra, given only minimal prompting, autonomously identified the creator of an anonymous 1808 sketchbook held at Yale&\#x27;s Beinecke Library in just 22 minutes using publicly available primary and secondary sources. In the process, the model discovered a little-known paper-archive reference to a diary entry recording a visit by the vicomte de Chabot five days before a date mentioned in the sketchbook near a nearby river, and correctly predicted that Chabot&\#x27;s travel journal — obtainable only by order from Cleveland State University — would confirm the attribution. If reproducible, this is a striking case study of an agentic LLM doing genuine archival research — forming a hypothesis, hunting down an obscure source, making a falsifiable prediction and then verifying it — rather than merely summarizing what it was given. Humphries suggests historians may face a milder version of the &quot;Deep Blue moment&quot; that mathematics is already confronting, as agentic systems begin doing research work that human historians cannot easily match. The attribution hinged on a single inferential chain — a diary reference to Chabot&\#x27;s visit five days before a date recorded in the sketchbook — which Astra turned into a testable prediction about a journal held only in a university collection. Caveats apply: this is one anecdotal case study with no independent verification yet, the newly surfaced Chabot journal is itself a significant find for Canadian and fur-trade historians, and GPT-6.2 Astra had launched only a week earlier on November 17, 2026, drawing mixed reviews from power users who complained of frequent mistakes.

rss · Simon Willison · Nov 24, 16:53

**Background**: Yale&\#x27;s Beinecke Rare Book and Manuscript Library is one of the world&\#x27;s largest buildings dedicated to rare books and manuscripts and serves as Yale Library&\#x27;s primary home for special collections, which is why an unattributed 1808 sketchbook there would normally require a specialist to trace. GPT-6.2 Astra is part of OpenAI&\#x27;s GPT-6.2 family, released alongside GPT-6.2 Sol on November 17, 2026 and available only to paid users. The &quot;Deep Blue&quot; comparison refers to IBM&\#x27;s chess computer that defeated Garry Kasparov in 1997, a shorthand for machines surpassing humans in a domain long considered a peak of human intellect.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-6.2_Astra">GPT-6.2 Astra</a></li>
<li><a href="https://simonwillison.net/2026/Nov/17/gpt62-astra-and-sol/">GPT ‑ 6 . 2 Astra and GPT ‑ 6 . 2 Sol | Simon Willison’s Weblog</a></li>
<li><a href="https://en.wikipedia.org/wiki/Beinecke_Rare_Book_and_Manuscript_Library">Beinecke Rare Book and Manuscript Library - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI research`, `#LLM applications`, `#historical research`, `#case study`, `#archival discovery`

---

<a id="item-7"></a>
## [OpenAI says GPT-6.2 designed protein minibinders via generated code](https://openai.com/index/gpt-6-models-demonstrate-intrinsic-protein-design-capabilities/) ⭐️ 7.0/10

OpenAI reports that GPT-6.2 was given the 3D structures of five target proteins with marked attachment sites and wrote code to create 3D designs for candidate minibinders without using specialized protein AI models. A specialized model called SolubleMPNN then suggested amino acid sequences for each design, and other protein models helped filter candidates predicted to fold as designed and bind at the intended site. If the claim holds up, general-purpose LLMs could become orchestration tools for de novo protein design, potentially accelerating AI-for-science work and early exploration of therapeutic binding proteins. However, this is a company announcement rather than independently validated research, so its real impact depends on follow-up experimental validation. The specialized SolubleMPNN model generated amino acid sequences for GPT-6.2&\#x27;s designs, and other protein models filtered candidates predicted to fold and bind as intended, so the LLM&\#x27;s role was mainly 3D backbone design via code rather than end-to-end protein design. The announcement provides no independent benchmark, success rate, or wet-lab validation in the supplied material, and it is unclear how the designs compare with established computational pipelines.

hackernews · acossta · Nov 24, 21:02 · [Discussion](https://news.ycombinator.com/item?id=50634658)

**Background**: Protein design is the rational engineering of new protein molecules, and minibinders are small proteins designed to bind tightly to a specific site on a target protein. Computational de novo design typically separates backbone generation, sequence design, and filtering: a designed amino acid sequence must fold into the intended 3D structure and bind the target. Large language models can contribute by writing code that drives such design pipelines, while specialized protein models remain important for sequence generation and candidate triage.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Protein_design">Protein design - Wikipedia</a></li>
<li><a href="https://www.nature.com/articles/s41467-025-56369-w">De novo design of protein minibinder agonists of TLR3 - Nature</a></li>
<li><a href="https://arxiv.org/pdf/2605.11189">Deep Learning for Protein Complex Prediction and Design</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters pushed back on the framing, asking what GPT-6.2 actually designed given that the amino acid sequence determines protein structure and SolubleMPNN supplied the sequences. Others argued that code generation is the real &\#x27;superpower&\#x27; of LLMs because it lets them scale design workflows, while some praised the broader prospect of AI accelerating scientific fields and suggested benchmarking against open models.

**Tags**: `#AI for science`, `#protein design`, `#LLM agents`, `#computational biology`, `#OpenAI`

---

<a id="item-8"></a>
## [Leaked GTA 6 Xbox Build Booted on Windows by Community Recompilers](https://twitter.com/raul_bs3/status/2125213756238291075) ⭐️ 7.0/10

Community reverse-engineering projects — notably xcl, VIctory and Leonida — are working to bring the leaked Xbox Series build of GTA 6 to Windows, with Leonida, a static recompilation effort, reportedly passing 14,000 GitHub stars as it pushed the game toward booting on PC. The work is being done with Wine-like compatibility approaches rather than an official port. It is a striking demonstration of how quickly fan recompilation can close the gap between a console exclusive and the PC platform, and it puts pressure on the usual console-then-PC release cadence that publishers rely on. It also raises the stakes for game preservation and for how aggressively rights holders will police such projects. Commenters note the leaked Xbox binary carries no special DRM or obfuscation and that modern Xbox hardware is essentially a Windows PC with extra Xbox layers, so the remaining problems are mostly compatibility and graphics translation rather than rewriting game logic. Leonida has since been banned from GitHub and other efforts were reportedly squashed by Rockstar, so the projects&\#x27; practical future depends as much on legal pressure as on technical progress.

hackernews · andrem · Nov 24, 13:19 · [Discussion](https://news.ycombinator.com/item?id=50627783)

**Background**: Recompilation projects take a shipped console binary and translate the console&\#x27;s machine code into native code for another platform, which is different from a decompilation that tries to reconstruct readable source. The Xbox Series runs a Windows-derived operating system, which makes a Wine-style translation layer — software that intercepts Windows/Xbox system calls and reimplements them — a plausible route to running console builds on ordinary PCs. Leaks of the GTA 6 Xbox build by the group Cyberleek supplied the assets and executable that make such attempts possible at all, well before any official PC version exists.

<details><summary>References</summary>
<ul>
<li><a href="https://gta6recomp.com/repo">Repositories &amp; Groups — GTA6 Recomp</a></li>
<li><a href="https://gta.mtwildwood.net/gta-6-pc/">GTA 6 on PC: XCL and VIctory progress - GTA VI Tracker</a></li>
<li><a href="https://gta6recomp.com/blog">GTA 6 PC Port News, Technical Devlogs &amp; In-Game Updates ...</a></li>

</ul>
</details>

**Discussion**: The thread mixes technical explanation with ethical debate: one commenter lays out the overall picture \(Cyberleek&\#x27;s leak, Xbox&\#x27;s Windows-like architecture, the Wine-style approach and the graphics/compatibility hurdles\), while another argues the project is not an existential threat because GTA 6 is already hugely profitable against its budget. Others ask why a leak was even necessary and warn that such recompilation may push publishers toward always-cloud-dependent game components that cannot be decompiled.

**Tags**: `#game-recompilation`, `#reverse-engineering`, `#wine`, `#gta-6`, `#digital-preservation`

---

<a id="item-9"></a>
## [Splitting one USB-C port into separate USB 3 and USB 2 devices](https://www.frankchiarulli.com/blog/splitting-usb-c/) ⭐️ 7.0/10

A blog post on frankchiarulli.com explains how to wire a single USB-C receptacle so that its USB 3.x SuperSpeed differential pairs go to one device while the USB 2.0 D+/D− pair goes to another, exposing two independent devices through one connector without a hub. The write-up triggered a detailed Hacker News thread in which hardware engineers added caveats and alternative designs. For embedded and hardware designers this is a BOM-reducing trick: a product can gain an extra function without adding a hub IC or a second connector, which is attractive for small, cost-sensitive devices. It also illustrates how much of USB-C&\#x27;s flexibility depends on host-side assumptions about port pairing and power that are invisible at the connector level. The approach works only because USB 2.0 and SuperSpeed signals use physically separate conductors inside the 24-pin connector, so each pair can be routed to a different downstream device. The catch, as commenters note, is that the host must tolerate a SuperSpeed device and a high/full-speed device behind the same physical port, and OS power management may misbehave if it cannot map the paired USB 2.0 and 3.x ports.

hackernews · fcjr · Nov 24, 14:54 · [Discussion](https://news.ycombinator.com/item?id=50629106)

**Background**: USB-C is a 24-pin, reversible connector whose pinout includes dedicated SuperSpeed differential pairs \(duplicated TX and RX sets so the plug works in either orientation\), a separate USB 2.0 D+/D− pair, configuration channel \(CC\) pins, sideband-use pins, VBUS and ground. In USB 3.x, a host enumerates SuperSpeed traffic through ports that are logically paired with USB 2.0 ports — USB 3.0 hubs expose these as &quot;companion ports&quot; — and the host keeps internal tables describing which 2.0 and 3.x ports belong together. Because the two signal groups travel on separate wires, routing them to different downstream devices makes one physical USB-C port look like two logically independent devices.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/USB-C">USB-C - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/USB_3.0">USB 3.0 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters with hands-on experience largely agreed the trick works but stressed complications: jsmith45 pointed out that power management is the biggest issue, since a host cutting power to a 3.x device typically needs to know which USB 2.0 port it is paired with, and that pairing is encoded in ACPI tables or device trees. Doohickey-d shared another BOM-reducing idea — a USB-C port whose function depends on plug orientation, used in a camera that exposes the SD card one way and live video the other — while xnzakg noted that cheap hubs with three USB 2.0 ports and one USB 3.x port exploit exactly this tree structure; riobard contrasted the complexity with USB-A&\#x27;s simple four-wire design.

**Tags**: `#usb-c`, `#hardware-design`, `#embedded-systems`, `#electronics`, `#power-management`

---

<a id="item-10"></a>
## [Blog Post on Brendan Gregg-Style Performance Analysis Sparks Debate](https://fzakaria.com/2026/11/12/worshipping-at-the-altar-of-brendan-gregg) ⭐️ 7.0/10

A blog post published on November 12, 2026 reflects on doing performance analysis in the spirit of Brendan Gregg, apparently using a purpose-built deterministic VM, and the piece drew 215 points and 40 comments on Hacker News. The discussion quickly moved from the post itself to broader questions about whether flame graphs and single-threaded deterministic execution can adequately explain multithreaded and async workloads. Flame graphs and Gregg&\#x27;s methodologies \(such as the USE method\) are the default vocabulary of production performance work, so a public debate about where they break down directly affects how engineers diagnose latency in multithreaded services. The thread highlights a real gap: modern async and coroutine-based systems have cross-thread causal chains that stack sampling alone cannot reconstruct. Commenters noted that the deterministic VM in question is single-threaded, which they argued compromises analysis of high-throughput multithreaded pipelines, and that tracing an async request&\#x27;s critical path likely requires embedding request context in framework code. Others pointed to sleep/stall profiling as an alternative, while acknowledging it involves trade-offs in the Linux kernel or extra transistors in CPU design.

hackernews · kqr · Nov 24, 10:50 · [Discussion](https://news.ycombinator.com/item?id=50626413)

**Background**: Brendan Gregg is a performance engineer known for codifying analysis methodologies \(including the USE method\) and for inventing flame graphs in 2011 while debugging a MySQL performance issue. A flame graph visualizes sampled stack traces as nested rectangles: the x-axis is the stack population sorted alphabetically rather than time, and a frame&\#x27;s width reflects how often it appeared in samples, with the top edge showing what is on-CPU. A deterministic VM, by contrast, makes execution reproducible — scheduling and timing no longer vary between runs — so a profile or trace can be replayed and compared exactly, similar in spirit to record-and-replay debuggers like rr.

<details><summary>References</summary>
<ul>
<li><a href="https://www.brendangregg.com/methodology.html">Performance Analysis Methodology</a></li>
<li><a href="https://www.brendangregg.com/flamegraphs.html">Flame Graphs - Brendan Gregg How to Read a Flame Graph: A Practical Profiling Guide for ... How to Read a Flame Graph: A Practical Profiling Guide for ... async-profiler tutorial: CPU and allocation flame graphs with ... Flame Graphs: A Complete Guide with 8 Examples (2026) | Plotly</a></li>
<li><a href="https://repowise.dev/blog/guides/flame-graph">Flame Graph: How to Read and Generate One (perf, pprof)</a></li>

</ul>
</details>

**Discussion**: The overall sentiment was positive toward the deterministic VM idea, with one commenter citing Antithesis as a similar inspiration, but several pushed back on single-threaded execution and on flame graphs themselves, saying cross-thread dependencies are nearly impossible to infer from them. Others asked whether this approach helps async workloads such as C++ coroutines and futures, drew parallels to rr&\#x27;s record-and-replay model, and relayed Nvidia&\#x27;s cultural &quot;speed of light&quot; framing — asking how fast something could be if every slowdown were removed.

**Tags**: `#performance-analysis`, `#deterministic-vm`, `#flamegraphs`, `#systems`, `#debugging`

---

<a id="item-11"></a>
## [Anthropic Stock Slips Below $83 IPO Price in Premarket Trading](https://www.bloomberg.com/news/articles/2026-11-24/anthropic-breaks-below-83-ipo-price-in-premarket-trading) ⭐️ 7.0/10

Anthropic&\#x27;s stock fell below its $83 initial public offering price during premarket trading on November 24, 2026, meaning shares are now trading under the level at which they were first sold to public investors. The drop sparked a wide-ranging debate on Hacker News about AI valuations, model economics, and whether frontier labs are sound long-term investments. Anthropic is one of the leading frontier AI labs, so its stock trading below the IPO price is a notable signal about shifting market sentiment toward AI companies and how investors are pricing the sector&\#x27;s enormous capital expenditures against uncertain future profits. The reaction affects anyone holding AI-related equities, enterprises budgeting for model APIs, and the wider startup ecosystem that benchmarks itself against these valuations. The move occurred in premarket trading, the session before the regular U.S. market opens, where volume is thin and prices can gap sharply on hype or panic, so a single premarket print is not necessarily indicative of where the stock settles once regular trading begins. Commenters were quick to note that poor initial post-IPO performance has historically had little bearing on prices one, two, or three years later, citing Amazon, Netflix, Tesla and Meta as examples.

hackernews · Betelbuddy · Nov 24, 13:23 · [Discussion](https://news.ycombinator.com/item?id=50627836)

**Background**: Frontier labs are organizations that develop the most advanced general-purpose AI models, investing heavily in compute, data and talent to push the state of the art in reasoning, multimodality and agentic workflows. An IPO is the process by which a private company first sells shares to the public; the IPO price is the fixed price set for that initial sale, and trading below it is often read as a sign that public markets value the company less than its underwriters and early backers did. Because AI labs require enormous ongoing spending on chips and data centers while their revenue models are still maturing, investors struggle to agree on what these companies are worth.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work - NVIDIA</a></li>
<li><a href="https://smartasset.com/investing/premarket-trading">What Is Premarket Trading , and How Does It Work?</a></li>

</ul>
</details>

**Discussion**: Sentiment was mixed but leaned toward skepticism about the valuation rather than the technology: one commenter running a model-agnostic continuous development system on roughly $10k per week of AI spend reported that about 65% of that budget currently goes to Anthropic, offering a concrete data point on real enterprise demand. Others argued it is entirely possible for AI to be transformative and for Anthropic to be the leading frontier lab while still being a terrible investment, while the more sanguine voices dismissed the dip as textbook IPO behavior and noted that early post-IPO weakness says little about long-term price.

**Tags**: `#anthropic`, `#ipo`, `#ai-industry`, `#stock-market`, `#ai-economics`

---

<a id="item-12"></a>
## [Blog post claims Cloudflare masks origin TLS and IPv4 weaknesses](https://charlie.fish/posts/2026/11/what-cloudflare-doesnt-tell-you/) ⭐️ 7.0/10

A blog post published at charlie.fish argues that Cloudflare does not do enough to reveal problems in the infrastructure behind it, specifically claiming that Cloudflare&\#x27;s connection to a customer&\#x27;s origin server may be entirely unencrypted and may rely exclusively on IPv4. The post triggered a Hacker News thread of roughly 142 points and 96 comments, including a direct response from Cloudflare CTO John Graham-Cumming \(jgrahamc\). When a CDN terminates TLS for visitors, the second leg between the CDN and the origin server is invisible to end users, so a lack of transparency there undermines any claim that a site is encrypted end to end. The debate matters to site operators, security researchers and anyone reasoning about how much of the web&\#x27;s traffic is actually protected after the edge. Cloudflare does provide tooling for this problem: Origin CA certificates let customers secure the Cloudflare-to-origin hop, and a 2022 SSL/TLS Recommender helps customers pick appropriate origin TLS settings — though Cloudflare does not currently send expiration notifications for Origin CA certificates, so operators must track them themselves. Commenters also pushed back on parts of the critique, arguing that the IPv4/IPv6 origin preference is trivially avoidable and that the whole point of a CDN is to shield the origin.

hackernews · fishcharlie · Nov 24, 19:03 · [Discussion](https://news.ycombinator.com/item?id=50632883)

**Background**: A CDN like Cloudflare sits between visitors and the origin server, so there are two TLS legs: visitor-to-CDN, which Cloudflare handles with an automatically renewed public certificate, and CDN-to-origin, which depends on the customer&\#x27;s own configuration \(often described as Full versus Full \(Strict\) mode\). If the origin leg is plaintext or uses a loosely validated certificate, the visitor&\#x27;s browser still shows a secure padlock even though part of the path is unprotected. Origin CA is Cloudflare&\#x27;s answer to this, issuing certificates trusted only by Cloudflare so the origin hop can be encrypted without a public CA.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.cloudflare.com/ssl/origin-configuration/origin-ca/">Cloudflare origin CA · Cloudflare SSL/TLS docs</a></li>
<li><a href="https://blog.cloudflare.com/cloudflare-ca-encryption-origin/">Introducing CloudFlare Origin CA Understanding &quot;Origin Server&quot; and &quot;Origin CA Certificates&quot; How do i download root certificate for the ca associated with ... cloudflare_origin_ca_certificate | Resources | cloudflare ... CA Bundle for Cloudflare: Origin Certificates and the Chain ...</a></li>
<li><a href="https://certpulse.dev/blog/cdn-tls-termination-origin-certificate">TLS termination at the CDN: the origin certificate you forgot ...</a></li>

</ul>
</details>

**Discussion**: Cloudflare CTO jgrahamc disputed the framing, pointing to the 2022 SSL/TLS Recommender and describing the company&\#x27;s effort to move customers onto encrypted origin connections as a bigger deal than outsiders assume. Other commenters were skeptical in different directions: one argued most sites don&\#x27;t need DDoS protection and that Cloudflare can actually reduce uptime compared with a well-run VPS, another called the IPv4-over-IPv6 complaint irrelevant since operators can simply disable IPv4, and others said exposing full-path TLS state defeats the purpose of a shielding CDN.

**Tags**: `#cloudflare`, `#cdn`, `#networking`, `#tls`, `#infrastructure`

---

<a id="item-13"></a>
## [Tesla and SpaceX Race Toward Year-End All-Stock Merger Deal](https://electrek.co/2026/11/24/tesla-spacex-merger-year-end-deadline-new-congress/) ⭐️ 7.0/10

According to the Financial Times, Tesla and SpaceX are working against a December 31 deadline to agree on an all-stock merger, a timeline that would land a signed deal just days before the new Congress is sworn in on January 3. The FT also named the directors negotiating for each side, noting that two of Tesla&\#x27;s three negotiators are the same people who designed Elon Musk&\#x27;s $1 trillion pay package. A Tesla–SpaceX combination would be the largest merger ever, reportedly valued at around $1.5 trillion, and would concentrate EV, energy storage, launch and satellite-broadband businesses inside a single Musk-controlled public company. The rush before the new Congress — where Democrats have promised to scrutinize Musk&\#x27;s companies — signals that regulatory and corporate-governance risk, not industrial logic, is driving the timing. The report is a short secondary account based on FT sourcing and offers no deal terms, exchange ratio or valuation detail; the board overlap matters because those same directors face re-election at Tesla&\#x27;s annual shareholder meeting on December 3, just as talks over terms are ongoing. Prior reporting suggested an announcement could come as soon as December, with the same directors who would sign off on the deal standing for shareholder approval.

rss · Electrek · Nov 24, 14:43

**Background**: An all-stock merger means the two companies combine without cash changing hands, with shareholders of one firm receiving shares in the combined entity — here, effectively folding SpaceX into Tesla&\#x27;s public listing. Tesla and SpaceX are already financially entangled: SpaceX has bought close to $1 billion of Tesla Megapack batteries and Cybertrucks, and Tesla became a SpaceX shareholder after its $2 billion investment in xAI converted into SpaceX stock when those two Musk companies combined. Musk&\#x27;s $1 trillion Tesla pay package — up to 423.7 million additional shares over a decade — was designed by the same board circle now reportedly negotiating the merger, which is why governance watchers frame the deal as a self-dealing risk.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ft.com/content/e598bbc7-8211-436f-a57e-46c3ae21ac0f?syn-25a6b1a6=1">Rockets, robots and risk: Elon Musk’s $3.6tn gamble to merge Tesla ...</a></li>
<li><a href="https://electrek.co/2026/11/12/spacex-tesla-merger-announcement-december-report/">SpaceX could announce $1.5 trillion Tesla merger in December: report</a></li>
<li><a href="https://www.cnn.com/2025/09/07/business/elon-musk-tesla-trillion">Why Tesla just threw $ 1 trillion at Elon Musk | CNN Business</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#SpaceX`, `#merger`, `#corporate governance`, `#Elon Musk`

---

<a id="item-14"></a>
## [Songe: Train Your Local LLM on Idle Compute](https://github.com/sous-labs/songe) ⭐️ 6.0/10

An open-source GitHub project called Songe \(installable via \`pip install songe\`\) provides a training engine that continuously trains or improves a local LLM using a machine&\#x27;s idle compute. Before the first training run, Songe benchmarks how much the machine can learn at once and then trains only on the batch size that fits the available resources. The project points toward a &quot;background improvement&quot; model for personal AI assistants, where a locally hosted model gets better over time from daily use rather than requiring separate, expensive GPU training sessions. Its appearance on Hacker News also revived interest in a SETI@home-style distributed fine-tuning network, an idea that could let ordinary users pool compute for model improvement. The repository currently offers little more than a one-line description and installation command, with no published benchmarks, evaluation methodology, or hardware requirements, so it remains unclear how much a model improves per training round or whether a GPU is required. The author&\#x27;s auto-sizing behavior suggests the engine targets a wide range of machines, but its effectiveness on CPU-only or low-VRAM setups has not been demonstrated.

hackernews · bluepeter · Nov 24, 15:03 · [Discussion](https://news.ycombinator.com/item?id=50629231)

**Background**: Fine-tuning adapts a pre-trained model to new behavior or domain data by running additional training on top of it, and lightweight methods such as LoRA and QLoRA have made this feasible on consumer hardware. Frameworks like Unsloth and Hugging Face TRL are commonly used to fine-tune models that then run locally through tools such as Ollama. Songe&\#x27;s premise is to fold that process into idle time, so a model can keep learning from a user&\#x27;s own data without dedicated training sessions.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/sous-labs/songe">GitHub - sous-labs/ songe : A training engine for your local model...</a></li>
<li><a href="https://unsloth.ai/docs">Unsloth is an open-source framework for running and training LLMs.</a></li>
<li><a href="https://gyanaangan.in/blog/qlora-fine-tuning-in-2026-train-a-local-llm-with-hugging-face-trl">QLoRA Fine - Tuning in 2026: Train a Local LLM ... - GyanAangan Blog</a></li>

</ul>
</details>

**Discussion**: Commenters were intrigued but largely skeptical: one asked for rough numbers on improvement per &quot;dream epoch&quot; over a weekend, another asked how Songe actually judges improvement and requested a transcribed before/after example in the README, and a third wanted to know whether it works on a modest GPU-less Windows PC running Qwen via Ollama. A widely shared sentiment was the desire for a SETI@home equivalent for LLMs, with the poster acknowledging the complexities of distributed training.

**Tags**: `#local-llm`, `#model-training`, `#open-source-tools`, `#distributed-computing`, `#fine-tuning`

---

<a id="item-15"></a>
## [Grafana ships security patches across five release branches](https://grafana.com/grafana/download) ⭐️ 6.0/10

Grafana published patch releases 12.4.16, 13.0.14, 13.1.11, 13.2.7 and 13.3.2 that bundle fixes for multiple CVEs, according to the download page and the release notes cited by commenters. The CVEs named in the community thread, taken from the GitHub release pages, are CVE-2026-107561, CVE-2026-88943 and CVE-2026-88960, with the newest 13.3.2 branch listing only two of the three. Grafana is one of the most widely deployed dashboards and observability front ends, frequently reachable from internal networks or the public internet, so any authenticated or privilege-escalation flaw in it is a practical concern for operators. The simultaneous backporting across several still-supported branches means teams on older minor versions can patch without a major upgrade. Commenters note the issues look mostly medium severity, with the notable exception of a cookie decryption oracle that still requires an attacker to already know an encrypted secret, and one user points out that the 13.2.x series had already shipped CVE fixes in 13.2.5 and 13.2.6. The thread also flags a discrepancy between the headline version numbers and the release-note list, so operators should confirm the exact CVE-to-version mapping on Grafana&\#x27;s own security advisory page before upgrading.

hackernews · petecooper · Nov 24, 19:23 · [Discussion](https://news.ycombinator.com/item?id=50633159)

**Background**: Grafana is an open-source platform for querying, visualizing and alerting on metrics and logs, commonly used as the front end for Prometheus, Loki and other observability data sources. CVEs are public identifiers for disclosed security vulnerabilities, and Grafana Labs maintains several parallel release branches so that fixes can be backported to older minor versions instead of forcing every user onto the newest release. Grafana publishes advisories through its own security page and through GitHub release notes, which is why community members often cross-check one against the other.

<details><summary>References</summary>
<ul>
<li><a href="https://cybersecuritynews.com/grafana-0-day-vulnerability/">xGrafana 0-Day Vulnerability Let Attackers to Redirect Users to...</a></li>
<li><a href="https://www.brinztech.com/breach-alerts/grafana-tempo-denial-of-service-vulnerability-cve-2026-27878/">Grafana Tempo Denial-of-Service Vulnerability (CVE-2026-27878)</a></li>

</ul>
</details>

**Discussion**: The discussion is calm rather than alarmed: one commenter lists the CVE IDs branch by branch from the GitHub release pages, another supplies the more useful security-advisories link, and a third assesses the flaws as likely medium severity apart from the cookie decryption oracle, which still needs a known encrypted secret. Others ask why the patches reached the front page at all, and one operator says the episode prompted them to consider adding authentication to their Grafana reverse proxy as a precaution against a future unauthenticated exploit.

**Tags**: `#Grafana`, `#security vulnerabilities`, `#CVE`, `#patching`, `#observability`

---

<a id="item-16"></a>
## [VW&\#x27;s Elli launches German V2G program paying EV owners up to €720](https://electrek.co/2026/11/24/vw-will-pay-ev-drivers-in-germany-up-to-e720-to-plug-in-at-home/) ⭐️ 6.0/10

Volkswagen&\#x27;s charging and energy subsidiary Elli is launching a vehicle-to-grid \(V2G\) program in Germany in December 2026 that pays EV owners up to €720 in the first year simply for keeping a compatible vehicle plugged in at home, even when it doesn&\#x27;t need charging. The offer turns parked cars into small grid-storage assets that can feed power back during peak demand. This is a commercial milestone for V2G, moving bidirectional charging from small pilot projects toward a mass-market consumer product backed by one of the world&\#x27;s largest automakers. If it scales, millions of EV batteries could become distributed storage that helps stabilize the grid and lowers the effective cost of owning an EV. The report is a short brief and gives no technical specifics — no grid-operator partners, no aggregation mechanics, no battery-degradation terms and no list of eligible vehicles or hardware. Elli&\#x27;s fuller product package pairs compatible EVs with the Elli BiDi Charger, a Volkswagen Naturstrom V2G Flow electricity tariff and the Elli BiDi App, and VW claims its high-voltage batteries and protection systems keep bidirectional cycling from significantly affecting battery lifespan.

rss · Electrek · Nov 24, 20:28

**Background**: Vehicle-to-grid \(V2G\) is a form of bidirectional charging in which an EV battery can both draw power from the grid and push electricity back into it, typically during peak-demand or high-price hours. Unlike a conventional one-way charger, it requires a vehicle whose onboard electronics support the reverse flow plus grid-synchronized charging equipment and, in practice, a utility or aggregator program that pays for the exported energy. Volkswagen and Elli announced plans for a fully integrated V2G offer for private customers in Germany from the fourth quarter of 2026, positioning Elli as the orchestrator between cars, chargers and the energy market.

<details><summary>References</summary>
<ul>
<li><a href="https://www.elli.eco/en/about-elli/news/newsroom/vehicle-to-grid-volumenmarkt">Elli | Volkswagen Group and Elli bring Vehicle-to-Grid offer ...</a></li>
<li><a href="https://www.volkswagen-group.com/en/press-releases/electric-vehicle-batteries-as-grid-storage-volkswagen-and-elli-to-launch-vehicle-to-grid-offer-20329">Electric vehicle batteries as grid storage: Volkswagen and ...</a></li>
<li><a href="https://www.solargenreview.com/articles/vehicle-to-grid-v2g-explained">Vehicle - to - Grid ( V 2 G ) Explained : V 2 H, V 2 G and V 2 L | SolarGenReview</a></li>

</ul>
</details>

**Tags**: `#vehicle-to-grid`, `#electric vehicles`, `#smart grid`, `#energy storage`, `#Volkswagen`

---

<a id="item-17"></a>
## [Nuro Starts Driverless Lucid Gravity Robotaxi Testing in Bay Area](https://electrek.co/2026/11/24/nuro-lucid-gravity-uber-robotaxi-driverless-testing-bay-area/) ⭐️ 6.0/10

Nuro has begun fully driverless testing of Lucid Gravity robotaxis on public roads in the San Francisco Bay Area, starting in four Peninsula and South Bay cities with a fleet of more than 100 Gravity SUVs supplied by Lucid. At the same time, the partnership&\#x27;s public launch, originally promised for 2026, has quietly slipped to the first quarter of 2027. Removing the human safety driver is the pivotal milestone in any robotaxi program, since it shifts the risk from supervised testing to true Level 4 operation on open roads. It also marks the most visible progress yet for the three-way Uber–Nuro–Lucid alliance, which is betting that licensing self-driving software to vehicle partners can compete with vertically integrated players like Waymo and Tesla in the ride-hailing market. The driverless phase covers four Peninsula and South Bay cities using over 100 Lucid Gravity SUVs, with employee-only rides expected to follow before any paying passengers are served. The roughly one-quarter delay to Q1 2027 suggests the program is still working through validation, permitting, or operational readiness rather than being ready for a broad commercial rollout.

rss · Electrek · Nov 24, 15:32

**Background**: Nuro was founded by veterans of Google&\#x27;s self-driving car project and initially built small autonomous delivery vehicles before pivoting in September 2024 to license its AI-based &quot;Nuro Driver&quot; software to automakers, suppliers, and mobility providers; the software is designed to enable Level 4 robotaxis as well as personally owned autonomous cars. In this partnership, Lucid&\#x27;s electric Gravity SUV provides the vehicle platform, Nuro supplies the autonomy stack, and Uber contributes its ride-hailing network and demand. Level 4 autonomy means the vehicle can drive without a human behind the wheel within a defined operational area, a step beyond the hands-free but human-supervised driver-assistance systems currently shipping on production cars.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Nuro">Nuro - Wikipedia</a></li>
<li><a href="https://www.theverge.com/transportation/1040676/uber-nuro-lucid-driverless-robotaxi-testing-bay-area">Uber, Nuro, and Lucid kick off fully driverless robotaxi testing</a></li>
<li><a href="https://www.nuro.ai/">Nuro — Autonomy for all. All roads, all rides. | Nuro</a></li>

</ul>
</details>

**Tags**: `#autonomous vehicles`, `#robotaxi`, `#Nuro`, `#Uber`, `#Lucid Motors`

---

<a id="item-18"></a>
## [NVIDIA Details Microduck Sim2Real Obstacle Avoidance Workflow with Isaac Lab and Newton](https://huggingface.co/blog/nvidia/microduck-obstacle-avoidance) ⭐️ 6.0/10

NVIDIA published a blog post on Hugging Face describing how to add local obstacle avoidance to its Microduck legged robot while leaving the existing walking policy untouched. A separate navigation controller is trained with PPO in Isaac Lab, using Newton as the physics backend and an 8×8 Time-of-Flight sensor modeled with Newton&\#x27;s raycaster, then evaluated in simulation, exported, and deployed to the real robot. The post lays out a reusable layered Sim2Real pattern — freeze the locomotion policy, train a navigation policy that adjusts gamepad-style velocity commands around obstacles — which lowers the cost of adding autonomy to robots that already walk reliably. It also serves as a public demonstration of Newton functioning as an Isaac Lab physics backend, a combination NVIDIA is pushing as the default stack for robot learning. The simulated perception relies on a deliberately sparse 8×8 ToF depth grid rather than a camera, and training courses are assembled from reusable SimReady assets so environments can be varied without new art. Notably, this is a vendor-authored tutorial walkthrough rather than a research contribution, so it presents no benchmarks or novel claims about transfer performance.

rss · HuggingFace Blog · Nov 24, 16:34

**Background**: Sim2Real \(simulation-to-reality\) transfer means training a control policy inside a physics simulator and then running it on physical hardware, which is cheaper and safer than learning on the real robot but sensitive to modeling gaps. Isaac Lab is NVIDIA&\#x27;s open-source, GPU-accelerated framework for robot learning that handles environment setup, policy training, evaluation, and deployment, and it can use Newton as its physics backend. Newton is an open-source, extensible physics engine built on NVIDIA Warp and OpenUSD, developed by NVIDIA with Google DeepMind and Disney Research and managed by the Linux Foundation. PPO \(Proximal Policy Optimization\) is the reinforcement learning algorithm used here, and a Time-of-Flight sensor measures distance by timing reflected light, giving a low-resolution depth map.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/nvidia/microduck-obstacle-avoidance">Microduck Obstacle Avoidance: A Sim2Real Workflow with Isaac ...</a></li>
<li><a href="https://developer.nvidia.com/newton-physics">Newton Physics Engine | NVIDIA Developer</a></li>
<li><a href="https://isaac-sim.github.io/IsaacLab/main/index.html">Welcome to Isaac Lab ! — Isaac Lab Documentation</a></li>

</ul>
</details>

**Tags**: `#Sim2Real`, `#Robotics`, `#Isaac Lab`, `#Physics Simulation`, `#Reinforcement Learning`

---