---
layout: default
title: "Horizon Summary: 2026-11-23 (EN)"
date: 2026-11-23
lang: en
---

> From 17 items, 7 important content pieces were selected

---

1. [OpenAI Argues Next-Token Perplexity Still Predicts Model Intelligence](#item-1) ⭐️ 8.0/10
2. [Analysis projects Anthropic&\#x27;s 2028 data center power will be 98% fossil fuels](#item-2) ⭐️ 8.0/10
3. [Beginner&\#x27;s Guide Walks Through Running Inkling and Qwen Locally with Unsloth](#item-3) ⭐️ 7.0/10
4. [Tim O&\#x27;Reilly Asks What Happened to Silicon Valley](#item-4) ⭐️ 7.0/10
5. [Show HN: A playable game where you are an LLM&\#x27;s subagent](#item-5) ⭐️ 7.0/10
6. [Miniature live 3D San Francisco tracks buses, planes and boats](#item-6) ⭐️ 6.0/10
7. [Jeff Geerling joins the NTP Pool, but not with his Stratum 1 Pi](#item-7) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI Argues Next-Token Perplexity Still Predicts Model Intelligence](https://openai.com/index/perplexity-and-intelligence/) ⭐️ 8.0/10

OpenAI published a short research post arguing that next-token perplexity — essentially the compression rate a model achieves on raw data — remains a strong and simple predictor of model intelligence. The piece drew 447 points and 300+ comments on Hacker News, where readers debated whether cross-entropy loss still tracks capability in the era of RL-trained reasoning models. The post offers a deliberately simple benchmark as a counterpoint to the increasingly convoluted evaluation suites that labs spin up, and it revives a long-running claim that compression and intelligence are tightly linked. If perplexity still tracks capability even after RL post-training, it would give researchers a cheap, universally computable yardstick for comparing models. Commenters noted the post never actually defines perplexity: it equals exp\(cross-entropy\), ranging from 1 for a perfect predictor to the vocabulary size for a purely random one. Others pushed back on the idea that specific abilities &quot;emerge&quot; at particular perplexity thresholds, pointing out that narrowly fine-tuned small models can show poor general perplexity while still solving domain tasks well.

hackernews · acossta · Nov 22, 17:06 · [Discussion](https://news.ycombinator.com/item?id=50601525)

**Background**: Perplexity is a standard intrinsic metric for language models: a model assigns a probability to each next token, and perplexity aggregates those probabilities into a measure of how surprised the model is by real text, computed as the exponent of the average cross-entropy loss. Because better prediction implies better modeling of the underlying data, some researchers argue it effectively measures compression, and that compression is a proxy for intelligence. Modern reasoning models add a wrinkle: reinforcement learning post-training such as PPO or GRPO optimizes for task outcomes rather than next-token likelihood, so it was unclear whether the old loss-based metric would still correlate with capability.

<details><summary>References</summary>
<ul>
<li><a href="https://metricgate.com/blogs/perplexity-language-model-evaluation/">Perplexity : Language Model Evaluation Explained | MetricGate</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cross-entropy">Cross-entropy - Wikipedia</a></li>
<li><a href="https://www.perplexity.ai/hub/blog/rl-training-for-math-reasoning">RL Training For Math Reasoning - perplexity.ai</a></li>

</ul>
</details>

**Discussion**: Sentiment was largely positive but analytical: one commenter supplied the missing formal definition of perplexity, another expressed genuine surprise that cross-entropy still tracks capability so cleanly after RL post-training and welcomed a simple benchmark over convoluted evals. A third linked the argument to a 2008 paper on compression as intelligence, while others were skeptical of precise &quot;emergence&quot; thresholds.

**Tags**: `#perplexity`, `#language-models`, `#cross-entropy`, `#benchmarking`, `#ai-research`

---

<a id="item-2"></a>
## [Analysis projects Anthropic&\#x27;s 2028 data center power will be 98% fossil fuels](https://betterdatacenterproject.com/2026/11/16/how-ai-is-powered-a-breakdown-of-byop-and-grid-power/) ⭐️ 8.0/10

An analysis published by the Better Data Center Project breaks down how AI data centers — including Anthropic&\#x27;s projected fleet — will be powered through 2028, estimating that 87% of Anthropic&\#x27;s electricity will come from natural gas and 11% from coal. The piece distinguishes between &quot;bring your own power&quot; \(BYOP\) on-site generation and grid-supplied electricity when tallying the fossil share. The projection implies that roughly 98% of one leading AI lab&\#x27;s electricity in 2028 would be fossil-based, putting the AI buildout on a collision course with corporate climate pledges and with the grid decarbonization that utilities and regulators are planning for. If accurate, it shifts the debate from generic &quot;AI energy demand&quot; concerns to specific questions about which companies are locking in gas and coal capacity for years to come. The figures are a forward-looking estimate derived from announced and leased data center capacity rather than a disclosure from Anthropic itself, and the remaining roughly 2% is accounted for by non-fossil sources, so the exact split is sensitive to assumptions about lease terms, grid interconnects and timelines. Because much of the capacity is behind-the-meter generation rather than grid purchases, it may fall outside traditional utility emissions reporting and renewable procurement accounting.

hackernews · happosai · Nov 22, 08:57 · [Discussion](https://news.ycombinator.com/item?id=50597612)

**Background**: AI data centers draw power in two main ways: from the public grid, where utilities must queue up new connections and generation that can take years, or through &quot;bring your own power&quot; arrangements in which the operator builds or contracts on-site generation — most often gas turbines — to get electricity faster. Natural gas plants emit roughly half the CO2 of coal per unit of electricity but also produce nitrogen oxides and other local air pollutants, which is why siting decisions have become controversial in host communities. Much of the public debate over AI&\#x27;s energy footprint hinges on this split between grid power and self-generated power, since only the former is typically captured in clean-energy purchasing claims.

**Discussion**: Hacker News commenters were sharply critical, with one calling Anthropic &quot;a legitimately bad actor&quot; for leasing capacity \(specifically Colossus 1\) whose local pollution has hit Memphis, and faulting the company for making no US renewable commitments while peers like Alphabet have large clean-energy teams. Others argued the case for regulation, saying purely financial accounting pushes environmental and social costs onto communities far from decision-makers, and several commenters contended that the enormous, hard-to-visualize scale of data center power demand means AI is likely to accelerate rather than help solve climate change; one commenter added context on how most US natural gas is now a byproduct of shale oil production and is often flared when not captured.

**Tags**: `#AI infrastructure`, `#data centers`, `#energy`, `#climate`, `#regulation`

---

<a id="item-3"></a>
## [Beginner&\#x27;s Guide Walks Through Running Inkling and Qwen Locally with Unsloth](https://www.gpupartner.com/blog/beginners-guide-local-ai-inkling-qwen-unsloth) ⭐️ 7.0/10

A new beginner-oriented guide published on gpupartner.com walks readers through setting up local AI using Inkling, Qwen, and Unsloth, covering both model deployment and the tooling around it. The post drew substantive Hacker News discussion in which practitioners shared hands-on hardware experiences, macOS tooling feedback, and notes on AMD NPU support. Local AI adoption is still gated less by model quality than by VRAM budgets and rough-edged tooling, so guides that pair model selection with memory-efficient tools like Unsloth lower the entry barrier for hobbyists and small teams. The lively community thread also shows that consumer-grade local inference is moving from demo territory toward everyday, if slow, usability. Per published setup guides, Inkling is a very large sparse mixture-of-experts model \(975B total parameters, ~41B active per token\), so consumer machines realistically need aggressive quantization or multi-GPU setups, whereas Qwen&\#x27;s smaller sizes fit in roughly 8GB of RAM at 7B and 16GB at 14B. Unsloth targets fine-tuning rather than inference, promising roughly 2-5x faster LoRA/QLoRA training with around 70% less GPU memory than standard PEFT.

hackernews · Retell15 · Nov 22, 21:01 · [Discussion](https://news.ycombinator.com/item?id=50603845)

**Background**: Local AI means running a language model on your own hardware instead of calling a cloud API, which trades convenience for privacy, offline operation, and no per-token bills. Because model weights are large, most practitioners use quantization — storing weights at 4-bit or 8-bit precision — to fit them into limited VRAM; mixture-of-experts \(MoE\) models like Inkling only activate a fraction of their parameters per token, which cuts compute but not the memory needed to hold all the weights. Unsloth is an open-source library that rewrites the fine-tuning kernels for LoRA/QLoRA adapters, making it cheaper to personalize a model on a single consumer GPU.

<details><summary>References</summary>
<ul>
<li><a href="https://www.layer3labs.io/guides/inkling-explained">Inkling Explained: Thinking Machines&#x27; Models, Inkling-Small</a></li>
<li><a href="https://www.ozercemkelahmet.com/tools/unsloth">Unsloth : faster, lower-memory LLM fine - tuning · Özer Cem...</a></li>
<li><a href="https://www.apatero.com/blog/qwen-local-installation-setup-guide-2026">Qwen Local Installation Guide 2026 | Apatero</a></li>

</ul>
</details>

**Discussion**: Commenters framed local AI as being in its &quot;plasma TV phase&quot; — early, heavy, and expensive — with one estimate that it will take about five years before most practical AI runs on personal machines. Others shared concrete rigs, such as a Ryzen 5 7600 plus Nvidia GPU running a containerized audiobook narrator, and a ThinkPad with a Ryzen AI 350 serving Qwen3.5-9B on the AMD NPU at about 12 tokens per second. Feedback was mostly constructive: one user asked the VRAM calculator to accept a user-set baseline instead of a fixed 1GB overhead, and another asked how much VRAM is needed before Qwen stops feeling sluggish on a normal laptop.

**Tags**: `#local-ai`, `#llm`, `#unsloth`, `#qwen`, `#hardware`

---

<a id="item-4"></a>
## [Tim O&\#x27;Reilly Asks What Happened to Silicon Valley](https://www.oreilly.com/radar/what-happened-to-silicon-valley/) ⭐️ 7.0/10

Tim O&\#x27;Reilly has published an O&\#x27;Reilly Radar essay arguing that Silicon Valley&\#x27;s current condition stems from incentive structures and market mechanisms that reward shareholder value over human flourishing, and he calls for redesigning those systems. The essay shifts the critique of the tech industry from individual company failures to the rules of the game, a framing that could influence how founders, venture capitalists, and policymakers think about AI-era consolidation and growth incentives. O&\#x27;Reilly leans on mechanism design—described in the discussion as &\#x27;reverse game theory&\#x27;—to ask not how to win the current game but what game society ought to be playing; commenters tie the shift to the end of the ZIRP era and AI-driven cannibalization of core businesses.

hackernews · greenyouse · Nov 22, 19:20 · [Discussion](https://news.ycombinator.com/item?id=50602947)

**Background**: Mechanism design is an economics and game-theory field focused on designing rules and institutions so that self-interested participants produce desirable collective outcomes, which is why it is sometimes called reverse game theory. Shareholder value maximization is the corporate-governance principle that firms should primarily maximize returns to shareholders, and it has long faced critiques that it ignores externalities borne by workers, consumers, and society. ZIRP, or zero interest rate policy, refers to an era of near-zero rates that made cheap capital abundant and encouraged venture-backed startups to prioritize rapid growth over sustainable business models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanism_design">Mechanism design - Wikipedia</a></li>
<li><a href="https://edwebcontent.ed.ac.uk/sites/default/files/imports/fileManager/JC_Rochet.pdf">A Critique of Shareholder Value Maximization</a></li>
<li><a href="https://siliconvalleyweekly.com/how-venture-capital-works-in-silicon-valley/">How Venture Capital Works in Silicon Valley</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with O&\#x27;Reilly&\#x27;s diagnosis and praise the mechanism-design framing, but they debate the proximate causes: some stress ZIRP-era excess and AI-driven consolidation, while others criticize VC influencers and argue that governance reforms are futile unless the underlying market machine is rebuilt.

**Tags**: `#Silicon Valley`, `#tech industry`, `#mechanism design`, `#venture capital`, `#AI`

---

<a id="item-5"></a>
## [Show HN: A playable game where you are an LLM&\#x27;s subagent](https://github.com/gulivan/worker755) ⭐️ 7.0/10

A developer released worker755 on GitHub, a playable interactive-fiction game in which the player works as a subagent under an LLM &\#x27;director&\#x27; that hands out tasks and reacts to what you do. The Show HN post drew 261 upvotes and 59 comments, with players quickly discovering they could test the system by running destructive commands like rm on the director&\#x27;s files. The game turns a dry technical pattern — orchestrator LLMs delegating work to cheaper subagents — into something people can experience firsthand, making questions about authority, oversight and instruction-following tangible. As multi-agent hierarchies become standard in production tooling, this kind of satirical sandbox helps developers and non-developers reason about how much autonomy a delegated agent should get. One commenter noted the demo felt over-prescriptive, since the manager handed over the exact commands needed to complete tasks rather than letting the player work it out, and it was unclear whether a harder self-directed mode exists. Others found the playful edge cases — such as deleting a file and seeing how the director responds — the most entertaining part of the build.

hackernews · ivantgam · Nov 22, 13:56 · [Discussion](https://news.ycombinator.com/item?id=50599762)

**Background**: Modern LLM agent frameworks let a parent or &\#x27;director&\#x27; model delegate subtasks to subagents, which in practice appear to the main model as ordinary tools with a task parameter while an executor routes the call to a subagent registry. Frameworks like AG2 and OpenCode extend this with permissions governing which subagents a parent may launch, and hierarchical multi-agent designs are now promoted as a way to build self-managing agent teams. The game fictionalizes exactly this setup, casting the human player as the lowest rung of the hierarchy.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.ag2.ai/docs/user-guide/subagents/">Subagents - AG2</a></li>
<li><a href="https://www.ibm.com/think/topics/hierarchical-ai-agents">What are hierarchical AI agents? - IBM</a></li>
<li><a href="https://opencode.ai/docs/agents/">Agents | OpenCode</a></li>

</ul>
</details>

**Discussion**: The discussion is largely enthusiastic and humorous: players enjoyed stress-testing the director with commands like rm -rf, one commenter joked &\#x27;Butlerian Jihad Now,&\#x27; and another mused that &\#x27;maybe this is already reality&\#x27; when it comes to opaque top-level decision-making. The main concrete criticism was the demo&\#x27;s heavy-handed guidance.

**Tags**: `#LLM agents`, `#interactive fiction`, `#Show HN`, `#AI satire`, `#developer tools`

---

<a id="item-6"></a>
## [Miniature live 3D San Francisco tracks buses, planes and boats](https://smallsf.com/) ⭐️ 6.0/10

smallsf.com is a browser-based miniature 3D model of San Francisco that updates live, showing buses, planes and boats moving through the city in real time. The project was shared on Hacker News, where it drew about 100 points and 40 comments praising its SimCity-like feel. It shows how publicly available live movement data can be turned into an immediately understandable, playful digital twin of a major city that anyone can open in a browser tab. The strong community response suggests real appetite for lightweight, real-time 3D city visualizations beyond conventional flat web maps. The main criticism is that the model degrades at high zoom levels, with commenters noting that landmarks such as Patricia&\#x27;s Green in Hayes Valley are simply missing from the geometry. For readers curious about the stack, the site hosts an /about page that one commenter pointed to as the place to look for the tools used.

hackernews · dutilh · Nov 22, 20:33 · [Discussion](https://news.ycombinator.com/item?id=50603589)

**Background**: Real-time 3D city visualization on the web typically relies on WebGL rendering engines such as Cesium, and open standards like CityGML/3DCityDB or commercial platforms like Esri&\#x27;s Scene Viewer for streaming large city models into the browser. Projects of this kind combine a 3D building/terrain basemap with live vehicle feeds, so the amount and freshness of the underlying geometry data largely determines whether the scene holds up when you zoom in.

<details><summary>References</summary>
<ul>
<li><a href="https://www.3dcitydb.org/3dcitydb-web-map/1.8.0/3dwebclient/index.html">3DCityDB-Web-Map-Client</a></li>
<li><a href="https://www.esri.com/en-us/arcgis/products/scene-viewer">3D Scene Viewer | Interactive Web 3D - Esri</a></li>

</ul>
</details>

**Discussion**: The sentiment is largely enthusiastic — one commenter said it feels like &quot;what SimCity should have been,&quot; and another called it exactly the kind of site they want to see on Hacker News. That praise is balanced by a concrete bug report that whole parks go missing when zooming in, plus a request for the author to share the tooling behind it.

**Tags**: `#visualization`, `#3d-graphics`, `#web-development`, `#mapping`, `#showcase`

---

<a id="item-7"></a>
## [Jeff Geerling joins the NTP Pool, but not with his Stratum 1 Pi](https://www.jeffgeerling.com/blog/2026/i-joined-the-ntp-pool/) ⭐️ 6.0/10

Jeff Geerling published a blog post documenting his decision to join the public NTP Pool as a Stratum 1 time source, walking through the hardware and configuration choices behind the move and explaining why his Stratum 1 Raspberry Pi build was not the machine he ultimately contributed to the pool. The post sparked a Hacker News thread with 120 points and 31 comments from timekeeping and homelab practitioners. The public NTP Pool is volunteer-run infrastructure that a huge share of the internet&\#x27;s devices rely on for correct time, so detailed write-ups from experienced operators lower the barrier for others to contribute well-configured servers. The discussion also surfaces the practical limits of Raspberry Pi-class hardware for precise timekeeping, which matters to anyone building a homelab time server. Commenters noted that Stratum 1 accuracy depends heavily on the reference clock and on NIC/hardware timestamping, and that Raspberry Pi boards are relatively poor at this because of their network interface and oscillator quality, with FPGA-based designs or x86 PCIe PTM/TGPIO options offering better results. Others flagged that a cheap multi-server setup can beat a single expensive Stratum 1 node by providing redundancy and local peers to cross-check against, and debated NTPSec versus Chrony as the daemon of choice.

hackernews · fortran77 · Nov 22, 15:35 · [Discussion](https://news.ycombinator.com/item?id=50600622)

**Background**: NTP \(Network Time Protocol\) is one of the oldest internet protocols still in use, synchronizing clocks across packet-switched networks. It works in a hierarchy of stratum levels: stratum 0 is the physical reference such as a GPS receiver or atomic clock, stratum 1 is a server synced directly to it, stratum 2 syncs from a stratum 1 server, and so on up to stratum 15. The NTP Pool is a dynamic collection of volunteer-run servers that clients worldwide are pointed at via pool.ntp.org, so its overall quality depends on how well those individual volunteers configure their machines.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/NTP_pool">NTP pool - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Network_Time_Protocol">Network Time Protocol - Wikipedia</a></li>
<li><a href="https://masterclock.be/en/knowledge-base/glossary/stratum/">Stratum — Time synchronisation glossary | Masterclock</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was broadly positive about the write-up but pushed back on Raspberry Pi hardware, with commenters recommending FPGA-based time servers or x86 machines with PCIe PTM/TGPIO, since Pis suffer from weak NIC timestamping and oscillators. Several readers questioned whether the pool has fixed its historical quality problems with unresponsive or badly misconfigured time sources that were days or weeks off, and others exchanged notes on NTPSec versus Chrony and on whether VPSes are still discouraged from joining.

**Tags**: `#ntp`, `#time-synchronization`, `#homelab`, `#networking`, `#raspberry-pi`

---