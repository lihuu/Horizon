---
layout: default
title: "Horizon Summary: 2026-06-03 (EN)"
date: 2026-06-03
lang: en
---

> From 33 items, 17 important content pieces were selected

---

1. [KDE Plasma to End X11 Support](#item-1) ⭐️ 8.0/10
2. [Microsoft Launches MAI-Code-1-Flash 137B Model](#item-2) ⭐️ 7.0/10
3. [CT Scans of BYD Car Parts Reveal Manufacturing Insights](#item-3) ⭐️ 7.0/10
4. [Adafruit Receives Demand Letter from Flux.ai's Legal Counsel](#item-4) ⭐️ 7.0/10
5. [Trump signs downsized AI executive order](#item-5) ⭐️ 7.0/10
6. [Browser ad feature criticized as cartel-like privacy threat](#item-6) ⭐️ 7.0/10
7. [Why Janet? A Personal Essay on Choosing a Lisp-like Language](#item-7) ⭐️ 7.0/10
8. [Anthropic Expands Claude Mythos to 15 Countries' Critical Infrastructure](#item-8) ⭐️ 7.0/10
9. [Why You Should Love systemd Timers Over Cron](#item-9) ⭐️ 7.0/10
10. [Microsoft Announces MAI-Thinking-1 and MAI-Code-1-Flash](#item-10) ⭐️ 7.0/10
11. [User leaves Gmail over excessive AI features](#item-11) ⭐️ 6.0/10
12. [Walking Tour of Seattle Surveillance Infrastructure](#item-12) ⭐️ 6.0/10
13. [HP re-releases classic HP-16C calculator as collector's edition](#item-13) ⭐️ 6.0/10
14. [Fidonet 1993 Overview Sparks Nostalgic Community Discussion](#item-14) ⭐️ 6.0/10
15. [BYD Claims Cast Aluminum Frame Beats Steel in Strength and Weight](#item-15) ⭐️ 6.0/10
16. [Mercedes CLA EV achieves nearly 400 miles real-world range](#item-16) ⭐️ 6.0/10
17. [Tesla Semi wows fleet operator on Grapevine test](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [KDE Plasma to End X11 Support](https://blog.davidedmundson.co.uk/blog/596/) ⭐️ 8.0/10

KDE Plasma has announced that the upcoming release will be the last to support the X11 display server, with future versions requiring Wayland. This transition will enable a single code path via Wayland for new features and improvements. This marks a major milestone in the Linux desktop ecosystem, as KDE is one of the last major desktop environments to fully move away from X11 to Wayland. It will affect millions of users and application developers, offering better performance and security but also raising concerns about feature parity and accessibility. The transition will allow KDE to introduce new features that were impossible under X11, but known issues remain, such as inability to save window positions for native Wayland windows, no per-application keyboard layouts, and regression in accessibility software like voice input systems.

hackernews · jandeboevrie · Jun 2, 14:16 · [Discussion](https://news.ycombinator.com/item?id=48370588)

**Background**: X11 is a decades-old display server protocol that has been the standard on Linux, but it suffers from security and performance limitations. Wayland is a modern replacement that integrates the display server and compositor, aiming to be simpler and more secure. The transition has been ongoing for several years, with major desktops like GNOME already defaulting to Wayland.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/X_display_server">X display server</a></li>
<li><a href="https://en.wikipedia.org/wiki/Wayland_display_server">Wayland display server</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some users praise KDE developers for pushing Wayland forward and report a smoother experience with fewer breakages, while others highlight significant regressions, especially for accessibility tools like Talon voice input, and missing features such as PiP windows staying on top. There is concern that some issues may take years to resolve.

**Tags**: `#KDE`, `#Plasma`, `#Wayland`, `#X11`, `#Linux Desktop`

---

<a id="item-2"></a>
## [Microsoft Launches MAI-Code-1-Flash 137B Model](https://microsoft.ai/news/introducingmai-code-1-flash/) ⭐️ 7.0/10

Microsoft announced MAI-Code-1-Flash, a 137B parameter mixture-of-experts code generation model with 5B active parameters, alongside six other MAI models. This release shows Microsoft's commitment to code AI, but early community analysis questions its competitiveness, as smaller models like Qwen achieve similar SWE-bench scores at lower cost. The model scores 51% on SWE-bench Pro, while the 35B-parameter Qwen3.6-35B-A3B scores 49.5%. Microsoft compares it to Claude Haiku 4.5, which commenters note is an older, smaller model.

hackernews · EvanZhouDev · Jun 2, 18:47 · [Discussion](https://news.ycombinator.com/item?id=48374466)

**Background**: Code generation models are specialized large language models trained on code and natural language. Mixture-of-experts (MoE) architectures use sparse activation to reduce computational cost, enabling large total parameter counts with lower inference costs. SWE-bench is a benchmark for evaluating models on real-world software engineering tasks.

**Discussion**: Community comments express skepticism: one user notes MAI-Code-1-Flash's performance is similar to Qwen's 35B model despite being much larger, and another criticizes the use of Claude Haiku as a baseline. Some users have canceled GitHub Copilot due to pricing changes and express disinterest in the new model.

**Tags**: `#AI`, `#Machine Learning`, `#Code Generation`, `#Microsoft`, `#Model Evaluation`

---

<a id="item-3"></a>
## [CT Scans of BYD Car Parts Reveal Manufacturing Insights](https://www.lumafield.com/scan-of-the-month/byd) ⭐️ 7.0/10

Lumafield published high-resolution CT scans of BYD car parts, including a key, seatbelt, and motor controller, exposing internal manufacturing details and supply chain architecture. This analysis provides rare transparency into BYD's vertical integration strategy and design choices, triggering discussions on the accuracy of reverse engineering and the scale of in-house production compared to legacy automakers. The scans reveal that BYD produces about 75% of its components in-house, similar to Tesla but far above Ford's ~25%, and the article notes that BYD's vertical integration spans from lithium mines to port logistics.

hackernews · viasfo · Jun 2, 20:30 · [Discussion](https://news.ycombinator.com/item?id=48375824)

**Background**: CT (computed tomography) scanning uses X-rays to create 3D cross-sectional images of objects non-destructively, allowing for detailed inspection of internal structures. Vertical integration refers to a company controlling multiple stages of production within its supply chain, from raw materials to final assembly.

**Discussion**: A BYD owner corrected the article's claim about the key being 'hinged,' explaining that the physical key pulls out via a clip, and the hinge-like feature is a plastic weld artifact. Another commenter compared production scales: BYD 4.6M, Ford 4.4M, Tesla 1.6M vehicles per year. A user in Mexico noted the contrast between local prevalence of BYD vehicles and US media perception.

**Tags**: `#automotive`, `#engineering`, `#reverse engineering`, `#supply chain`, `#BYD`

---

<a id="item-4"></a>
## [Adafruit Receives Demand Letter from Flux.ai's Legal Counsel](https://blog.adafruit.com/) ⭐️ 7.0/10

Adafruit, a prominent open-source hardware company, received a demand letter from Fenwick legal counsel on behalf of Flux.ai, a venture-funded AI PCB design startup. The letter likely pertains to a potential critical review or commentary about Flux.ai that Adafruit was preparing to publish. This incident highlights tensions between open-source communities and venture-backed startups over intellectual property and critical discourse. It could set a precedent for how companies respond to negative reviews, potentially chilling legitimate criticism. The demand letter was sent by Fenwick, a prominent law firm, on behalf of Flux.ai. Adafruit's founder, ladyada, has reached out to Flux.ai's CEO to resolve the matter publicly, possibly via a podcast.

hackernews · semanser · Jun 2, 10:00 · [Discussion](https://news.ycombinator.com/item?id=48368121)

**Background**: Adafruit is a major open-source hardware company known for selling electronics kits and publishing reviews and tutorials. Flux.ai is a browser-based PCB design tool that uses AI to assist with schematic and layout, targeting modern hardware design methodologies. The tool has received mixed reviews, with some users reporting poor experiences and high token costs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.flux.ai/">Flux - Design PCBs with AI</a></li>
<li><a href="https://www.electronics-lab.com/flux-ai-an-ai-powered-browser-based-pcb-design-tool-review/">Flux.ai – An AI Powered, Browser-Based PCB Design Tool Review</a></li>

</ul>
</details>

**Discussion**: Community comments express strong skepticism towards Flux.ai's product quality and legal strategy. Many users describe negative experiences with Flux.ai, calling it an 'awful product' that consumes tokens with little output. Some suggest Adafruit was preparing a critical post, leading Flux.ai to preemptively send a demand letter.

**Tags**: `#Legal`, `#Hardware`, `#Open-source`, `#PCB design`, `#Community conflict`

---

<a id="item-5"></a>
## [Trump signs downsized AI executive order](https://www.politico.com/news/2026/06/02/trump-signs-downsized-ai-order-00946389) ⭐️ 7.0/10

President Trump signed an executive order on June 2, 2026, that requires AI companies to voluntarily submit powerful new models for government review 30 days before public release and directs the Justice Department to prosecute individuals who misuse AI for hacking. This order represents a significant federal AI regulatory move, balancing safety oversight with industry innovation, and could set a precedent for how the U.S. government addresses risks from advanced AI models without imposing mandatory restrictions. The review is voluntary and applies only to the most powerful models; the order also calls for developing a cybersecurity benchmark for models and directs prosecution of AI-enabled computer crimes, but lacks mandatory testing or licensing requirements.

hackernews · _alternator_ · Jun 2, 16:40 · [Discussion](https://news.ycombinator.com/item?id=48372628)

**Background**: Executive orders allow the president to direct federal agencies without new legislation. Previous AI orders, like Biden's 2023 executive order, required mandatory safety testing. This new order is seen as a scaled-back version, emphasizing voluntary compliance and enforcement against misuse rather than pre-market mandates.

<details><summary>References</summary>
<ul>
<li><a href="https://www.opb.org/article/2026/06/02/trumps-new-ai-safety-order-seeks-voluntary-review-of-new-models/">Trump signs AI safety order seeking voluntary review of new models - OPB</a></li>
<li><a href="https://www.reuters.com/legal/litigation/white-house-briefs-ai-firms-plans-model-review-information-reports-2026-05-20/">White House briefs AI firms on plans for model review, the ... - Reuters</a></li>
<li><a href="https://news.bloomberglaw.com/us-law-week/rising-ai-related-sophisticated-crimes-need-urgent-DOJ-Attention">Rising AI-Related Sophisticated Crimes May Invite More DOJ Focus</a></li>

</ul>
</details>

**Discussion**: Commenters expressed skepticism about the order's substance, noting it lacks concrete requirements. Some worried it could lead to de facto restrictions on open-source models by creating a review process that favors closed, vetted releases. Others argued the voluntary review period might allow insider trading rather than improve security, and criticized that DOJ prosecution of AI misuse was already possible under existing law.

**Tags**: `#AI regulation`, `#executive order`, `#policy`, `#cybersecurity`, `#open source`

---

<a id="item-6"></a>
## [Browser ad feature criticized as cartel-like privacy threat](https://blog.zgp.org/the-advertising-cartel-coming-to-your-web-browser/) ⭐️ 7.0/10

A blog post criticizes a proposed browser advertising feature, arguing that big tech companies are forming a cartel to embed tracking into browsers while bypassing privacy regulations. The post highlights concerns over a lack of consent mechanisms and dual standards for third-party advertisers versus built-in browser tracking. This debate impacts the future of web privacy and online advertising, as browser-level tracking could become a default, undermining user control. The discussion reflects broader tensions between big tech, advertisers, regulators, and users over how to balance privacy and ad revenue. The proposed feature, part of Google's Privacy Sandbox and similar initiatives, includes APIs like Topics and FLoC that categorize users for ad targeting without third-party cookies. Critics argue that these systems give browser vendors preferential treatment and may still enable tracking, while supporters claim they improve privacy compared to current methods.

hackernews · speckx · Jun 2, 19:39 · [Discussion](https://news.ycombinator.com/item?id=48375175)

**Background**: The Privacy Sandbox was a Google-led initiative launched in 2019 to develop privacy-preserving advertising technologies, replacing third-party cookies. It included APIs such as Topics (which shares users' interest categories) and FLoC (which groups users into cohorts). The initiative faced antitrust scrutiny and was officially discontinued in April 2025 due to low adoption. However, similar browser-based advertising features continue to be proposed by other companies, raising concerns about a cartel-like control over web standards.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Privacy_Sandbox">Privacy Sandbox</a></li>
<li><a href="https://en.wikipedia.org/wiki/Topics_API">Topics API</a></li>
<li><a href="https://en.wikipedia.org/wiki/FLoC">FLoC</a></li>

</ul>
</details>

**Discussion**: Comments reveal polarized views: some agree that the proposal gives browser vendors unfair advantages and lacks consent options, while others suspect the blog author is an advertiser protecting their profits. A few commenters see cross-company cooperation on privacy as a positive sign, and one criticizes the website's own invasive pop-up.

**Tags**: `#privacy`, `#advertising`, `#web browsers`, `#big tech`, `#tracking`

---

<a id="item-7"></a>
## [Why Janet? A Personal Essay on Choosing a Lisp-like Language](https://ianthehenry.com/posts/why-janet/) ⭐️ 7.0/10

The author published a personal essay titled 'Why Janet? (2023)' explaining why they adopted Janet as their primary programming language, citing its simplicity, portability, and unique features like built-in parsers and PEG grammars. This essay has sparked high community engagement, highlighting Janet as a modern Lisp-inspired language that excels in embedding and distribution, encouraging developers to consider alternatives beyond mainstream languages like Python or Lua. Janet is a functional and imperative language implemented in C99, featuring a bytecode VM, built-in sandboxing via feature sets, and a package manager (jpm) that can produce standalone binaries. The article mentions that Janet's standard library includes a parser library and that bindings created with 'def' are immutable, though a community commenter noted an inaccuracy regarding 'setq'.

hackernews · yacin · Jun 2, 09:34 · [Discussion](https://news.ycombinator.com/item?id=48367907)

**Background**: Janet is a lightweight Lisp-inspired programming language created by Caleb Evans and first released in 2017. It is designed for system scripting, automation, and embedding into C/C++ programs, similar to Lua or GNU Guile. Janet runs on Windows, Linux, macOS, and other platforms, and emphasizes simplicity and portability with a small runtime footprint. The language offers features such as pattern matching, PEG parsers, and first-class support for closures and macros.

<details><summary>References</summary>
<ul>
<li><a href="https://janet-lang.org/">Janet Programming Language</a></li>
<li><a href="https://github.com/janet-lang/janet">GitHub - janet-lang/janet: A dynamic language and bytecode vm</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed opinions: some praised Janet's portability and sandboxing, while others criticized its limited library ecosystem and lack of package versioning. One user highlighted an inaccuracy in the article regarding 'setq' behavior, and another mentioned Fennel as a similar language that compiles to Lua. Overall, the discussion was constructive, with users sharing their experiences and alternative perspectives.

**Tags**: `#Janet`, `#programming languages`, `#Lisp`, `#embedded scripting`, `#technical essay`

---

<a id="item-8"></a>
## [Anthropic Expands Claude Mythos to 15 Countries' Critical Infrastructure](https://www.anthropic.com/news/expanding-project-glasswing) ⭐️ 7.0/10

Anthropic announced the expansion of Project Glasswing, deploying its Claude Mythos AI model to secure critical infrastructure across 15 countries, as reported on June 2, 2026. This expansion marks a significant step in using advanced AI for national security, but raises concerns about effectiveness and ethical implications of AI monitoring critical systems. Claude Mythos is a large language model designed to find software vulnerabilities, and it remains unreleased to the public due to safety concerns. The expansion covers 15 countries, though specific names were not disclosed.

hackernews · surprisetalk · Jun 2, 13:15 · [Discussion](https://news.ycombinator.com/item?id=48369863)

**Background**: Project Glasswing is Anthropic's cybersecurity initiative launched in April 2026 to secure critical software using AI. Claude Mythos is a frontier model described as a 'step change' in capabilities, but has drawn mixed reactions from the security community.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos</a></li>
<li><a href="https://www.anthropic.com/glasswing">Project Glasswing : Securing critical software for the AI era \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Comments reveal skepticism: one user reported that Claude Mythos generated excessive false positives in practice, while another accused Anthropic of using security concerns to mask compute shortages. Concerns about mass surveillance and the need for memory-safe alternatives like Rust were also raised.

**Tags**: `#Anthropic`, `#critical infrastructure`, `#AI safety`, `#Claude Mythos`, `#deployment`

---

<a id="item-9"></a>
## [Why You Should Love systemd Timers Over Cron](https://blog.tjll.net/you-dont-love-systemd-timers-enough/) ⭐️ 7.0/10

The article argues that systemd timers are superior to cron due to better resilience to system startup times, clearer configuration, integration with journalctl, and easier debugging. This matters because cron is a decades-old standard for task scheduling in Linux, and systemd timers offer modern features like missed-run catch-up, randomized delays, and unified logging, making them a more robust choice for system administrators. systemd timers use .timer unit files that work with corresponding .service files, supporting both calendar-based (OnCalendar) and monotonic events. They log to journald, can be tested with systemctl start, and support dependencies on other systemd services.

hackernews · yacin · Jun 2, 09:34 · [Discussion](https://news.ycombinator.com/item?id=48367904)

**Background**: systemd is a system and service manager for Linux used by most modern distributions. It replaced traditional init systems like SysVinit. systemd timers are a mechanism within systemd for scheduling tasks, similar to cron but more tightly integrated with the rest of the system, providing features like persistent timers that catch up after downtime and randomized delays to avoid load spikes.

<details><summary>References</summary>
<ul>
<li><a href="https://wiki.archlinux.org/title/Systemd/Timers">systemd/Timers - ArchWiki</a></li>
<li><a href="https://linuxconfig.org/how-to-schedule-tasks-with-systemd-timers-in-linux">Schedule Tasks with Systemd Timers on Linux - LinuxConfig.org Configure Systemd Timers on Linux [With Examples] Working with systemd Timers | SUSE Linux Enterprise Server 15 SP7 Systemd Timers: A Practical Guide to Replacing Cron on Linux Working with Timers in Systemd - docs.oracle.com systemd.timer - freedesktop.org</a></li>

</ul>
</details>

**Discussion**: The comments show strong support for systemd timers, with users sharing real-world experiences like backups that run after boot if missed and automatic printer maintenance. Some debate about PATH handling exists, but overall sentiment is positive toward timers.

**Tags**: `#systemd`, `#cron`, `#Linux`, `#system administration`, `#scheduling`

---

<a id="item-10"></a>
## [Microsoft Announces MAI-Thinking-1 and MAI-Code-1-Flash](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 7.0/10

Microsoft announced two new text LLMs: MAI-Thinking-1 (reasoning, 35B parameters) and MAI-Code-1-Flash (5B parameters for code). MAI-Thinking-1 uses a sparse Mixture of Experts architecture and is claimed to be preferred over Sonnet 4.6 in blind evaluations, while MAI-Code-1-Flash is rolling out to GitHub Copilot users in VS Code. These low-parameter models could significantly reduce the cost of high-performance reasoning and code generation, making powerful AI more accessible. Moreover, their training on clean, licensed data sets a precedent for addressing copyright concerns in AI development. MAI-Thinking-1 has ~1T total parameters but only 35B active, matching Claude Opus 4.6 on SWE-Bench Pro. Both models were trained from scratch on enterprise-grade, commercially licensed data without distillation from third-party models, addressing data provenance concerns.

rss · Simon Willison · Jun 2, 22:21

**Background**: Reasoning models like OpenAI's o-series and Gemini thinking variants use extra compute during inference to generate step-by-step reasoning, improving accuracy on complex tasks. Parameter count and architecture (e.g., sparse MoE) affect model performance and cost; smaller activated-parameter models can run on consumer hardware. Most current large models train on unlicensed web scrapes, raising copyright issues.

<details><summary>References</summary>
<ul>
<li><a href="https://microsoft.ai/news/introducing-mai-thinking-1/">Introducing MAI-Thinking-1 - Microsoft AI</a></li>
<li><a href="https://www.zdnet.com/article/all-the-new-ai-models-microsoft-just-launched-at-build/">Microsoft's first reasoning model is one of 7 AIs just ...</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#LLM`, `#AI models`, `#reasoning`, `#code generation`

---

<a id="item-11"></a>
## [User leaves Gmail over excessive AI features](https://moddedbear.com/gmail-thinks-im-stupid-so-i-left) ⭐️ 6.0/10

A user publicly announced they switched from Gmail to Fastmail, citing frustration with Google's aggressive AI integration in email, including auto-suggested replies and smart features. This reflects a growing user backlash against AI-driven email features that feel intrusive and unnecessary, highlighting a market demand for simpler, privacy-focused alternatives like Fastmail. Fastmail is a subscription-based, ad-free email service offering app passwords, hide-my-email aliases, and iOS integration, though its calendar lacks autocomplete for addresses. The user praises Fastmail's speed and simplicity compared to Gmail's sluggish AI overlays.

hackernews · speckx · Jun 2, 19:27 · [Discussion](https://news.ycombinator.com/item?id=48375016)

**Background**: Gmail has increasingly integrated AI features like Smart Reply and Smart Compose, which suggest full responses or auto-complete emails. Some users find these features helpful, but others see them as intrusive and unnecessary. Fastmail, founded in 1999 and based in Melbourne, offers a more traditional, privacy-focused email experience with no ads and faster performance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Fastmail">Fastmail</a></li>
<li><a href="https://www.fastmail.com/">Email and calendar made better | Fastmail</a></li>
<li><a href="https://grokipedia.com/page/Fastmail">Fastmail</a></li>

</ul>
</details>

**Discussion**: Community comments praise Fastmail's speed and simplicity, with one user noting it 'has everything Gmail has' and is 'instant'. Others express frustration with Google's AI suggestions being overly large and irrelevant, and question why native English speakers would use LLMs to write emails.

**Tags**: `#Email`, `#AI features`, `#Gmail`, `#Fastmail`, `#Productivity`

---

<a id="item-12"></a>
## [Walking Tour of Seattle Surveillance Infrastructure](https://coveillance.org/a-walking-tour-of-surveillance-infrastructure-in-seattle/) ⭐️ 6.0/10

The article presents a detailed walking tour of visible surveillance cameras in Seattle, examining their societal implications and the concept of 'gazes'. It highlights the growing normalization of surveillance in urban spaces, raising privacy and civil liberties concerns that affect all citizens. The tour uses art-school vocabulary like 'kinds of gazes' that some find inaccessible, and discusses how cameras encode social agreements about normal behavior.

hackernews · eustoria · Jun 2, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48369980)

**Background**: Surveillance infrastructure refers to the network of cameras and monitoring systems deployed in public spaces. The walking tour is a curated route that highlights the prevalence and design of these cameras, prompting reflection on privacy and social control.

**Discussion**: Commenters have mixed feelings: some accept surveillance as necessary for safety given high crime rates, while others criticize the inaccessible language and argue that surveillance erodes freedom. There is debate over the trade-off between liberty and security.

**Tags**: `#surveillance`, `#privacy`, `#seattle`, `#ethics`, `#technology`

---

<a id="item-13"></a>
## [HP re-releases classic HP-16C calculator as collector's edition](https://hpcalcs.com/product/hp-16c-collectors-edition/) ⭐️ 6.0/10

After more than 35 years, Hewlett-Packard has re-released the HP-16C Computer Scientist calculator as a Collector's Edition, preserving the original design with some modern refinements. This re-release appeals to nostalgic programmers and calculator enthusiasts, but questions about build quality and alternative options like SwissMicros DM16L highlight the niche market and practical concerns. The HP-16C was originally produced from 1982 to 1989 for computer programmers. The new Collector's Edition aims to honor the legacy, but some users are wary due to issues with the earlier 15C Collector's Edition.

hackernews · dm319 · Jun 2, 19:02 · [Discussion](https://news.ycombinator.com/item?id=48374685)

**Background**: HP's Voyager series calculators (including HP-11C, 15C, and 16C) were renowned for their robust build quality and Reverse Polish Notation (RPN) logic. The HP-16C was specialized for programmers, supporting hexadecimal, octal, and binary arithmetic. SwissMicros produces modern clones like the DM16L that offer similar functionality with updated hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HP-16C">HP-16C - Wikipedia</a></li>
<li><a href="https://hpcalcs.com/product/hp-16c-collectors-edition/">HP 16c Collector’s Edition - HP Calc</a></li>

</ul>
</details>

**Discussion**: Commenters express strong nostalgia but often recommend SwissMicros alternatives or keeping their original devices; concerns about build quality compared to originals are common, especially after issues with the 15C Collector's Edition.

**Tags**: `#hardware`, `#calculators`, `#retro computing`, `#HP`

---

<a id="item-14"></a>
## [Fidonet 1993 Overview Sparks Nostalgic Community Discussion](https://www.fidonet.org/inet92_Randy_Bush.txt) ⭐️ 6.0/10

A historical 1993 document detailing Fidonet technology, use, tools, and history has been shared online, prompting a wave of nostalgic comments from former users. This highlights Fidonet's significance as a precursor to modern social networks and the enduring legacy of early decentralized online communities. It offers valuable historical context for understanding the evolution of internet-based communication. Fidonet used a store-and-forward system over dial-up modems to exchange email and forum messages, with node addresses like '2:463/1161'. A Turkish clone called HitNet existed with similar addressing.

hackernews · BruceEel · Jun 2, 13:53 · [Discussion](https://news.ycombinator.com/item?id=48370291)

**Background**: Fidonet is a worldwide computer network for bulletin board systems (BBSes) that operated via store-and-forward messaging over telephone lines. BBSes were early online communities where users dialed in to read messages, play games, and share files. Fidonet allowed BBSes to exchange messages globally, creating a decentralized network that peaked with nearly 40,000 nodes in the mid-1990s before the rise of the internet.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/FidoNet">FidoNet</a></li>
<li><a href="https://en.wikipedia.org/wiki/Bulletin_board_system">Bulletin board system - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong nostalgia, with one user noting the 'magical' experience of seeing messages relay across the country for free. Another mentioned a Turkish Fidonet clone (HitNet) and its early social networking features. A few pointed out that Fidonet and its alt-nets are still active today.

**Tags**: `#Fidonet`, `#BBS`, `#History`, `#Networking`

---

<a id="item-15"></a>
## [BYD Claims Cast Aluminum Frame Beats Steel in Strength and Weight](https://electrek.co/2026/06/02/byd-says-its-cast-aluminum-frame-is-lighter-tougher-and-safer-than-steel/) ⭐️ 6.0/10

BYD announced that its cast aluminum frame for the Yangwang U8L SUV is lighter, tougher, and safer than a comparable steel frame, having passed a 12-ton lift test. This could enable significant weight reduction in large EVs while improving structural rigidity and safety, potentially influencing future vehicle design and manufacturing across the industry. The frame weighs 56 kg (~123 lbs) less than a steel equivalent, yet torsional rigidity is over 50% better. BYD claims the U8L is the first vehicle to pass a 12-ton lifting test with such a frame.

rss · Electrek · Jun 2, 20:40

**Background**: In automotive construction, chassis frames have traditionally used steel for strength or aluminum for weight savings. BYD's approach uses a cast aluminum integrated frame, which reduces weight while increasing stiffness and crash safety. The 12-ton lift test simulates extreme loads, demonstrating the frame's durability and safety margin.

<details><summary>References</summary>
<ul>
<li><a href="https://electrek.co/2026/06/02/byd-says-its-cast-aluminum-frame-is-lighter-tougher-and-safer-than-steel/">BYD says its cast aluminum frame is lighter and tougher than steel</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vehicle_frame">Vehicle frame - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#electric vehicles`, `#automotive`, `#materials science`, `#manufacturing`

---

<a id="item-16"></a>
## [Mercedes CLA EV achieves nearly 400 miles real-world range](https://electrek.co/2026/06/02/mercedes-cla-ev-delivers-nearly-400-miles-range-real-world-test/) ⭐️ 6.0/10

The Mercedes-Benz CLA EV 350 drove close to 400 miles on a single charge in a real-world test, surpassing its EPA-estimated range of 312 miles by about 25%. This real-world result demonstrates that Mercedes has achieved a significant breakthrough in EV efficiency, potentially narrowing the range gap with competitors like Tesla and alleviating consumer range anxiety. The test was conducted on public roads with mixed driving conditions, and the vehicle used a production-spec CLA EV 350. The nearly 400-mile range is about 25% higher than the official EPA rating.

rss · Electrek · Jun 2, 14:28

**Background**: The CLA EV is Mercedes' entry-level electric sedan, built on the MMA platform. EPA range estimates are standardized lab tests, while real-world driving conditions often yield different results; achieving higher real-world range indicates efficient thermal management and aerodynamics.

**Tags**: `#electric vehicles`, `#Mercedes`, `#range test`, `#automotive technology`

---

<a id="item-17"></a>
## [Tesla Semi wows fleet operator on Grapevine test](https://electrek.co/2026/06/02/covenant-logistics-tesla-semi-grapevine-test-amazed/) ⭐️ 6.0/10

Covenant Logistics, a major US trucking firm, completed a two-week evaluation of the Tesla Semi, including a fully loaded run over the steep Grapevine pass on I-5, leaving the driver amazed by its performance and confidence. This real-world test by a major fleet operator signals growing confidence in electric heavy-duty trucks, potentially accelerating adoption in the logistics industry. The Grapevine is a notoriously steep section of Interstate 5 in California. The test involved a loaded trailer, and the driver reported feeling more confident than in a diesel truck.

rss · Electrek · Jun 2, 14:20

**Background**: The Grapevine is a steep grade on I-5 north of Los Angeles, challenging for heavy trucks. Tesla Semi is an all-electric Class 8 truck with a claimed range of 500 miles. Covenant Logistics operates over 2,600 tractors, making this a significant endorsement.

**Tags**: `#electric vehicles`, `#Tesla Semi`, `#trucking`, `#logistics`

---