---
layout: default
title: "Horizon Summary: 2026-09-29 (EN)"
date: 2026-09-29
lang: en
---

> From 59 items, 27 important content pieces were selected

---

1. [Anthropic Releases Claude Sonnet 5.5, Sparking Debate on Benchmarks and Pricing](#item-1) ⭐️ 8.0/10
2. [NeurIPS Paper Formalizes Adaptive Representations for Functional Gradient Descent](#item-2) ⭐️ 8.0/10
3. [Jeff: home-trained 0.8B Jev-compatible decision models at ~30ms](#item-3) ⭐️ 7.0/10
4. [MUBI Essay Examines Film Preservation, Piracy, and Copyright Tensions](#item-4) ⭐️ 7.0/10
5. [AMD Acquires World Labs, Fei-Fei Li&\#x27;s Spatial Intelligence Startup, for ~$8.2B](#item-5) ⭐️ 7.0/10
6. [Hijacking the PS5&\#x27;s RTMP Stream for Custom Overlays](#item-6) ⭐️ 7.0/10
7. [Flock Safety Moves to Take Down Crowdsourced Surveillance Camera Map](#item-7) ⭐️ 7.0/10
8. [Kids Turn Low-Traffic NPR Spotify Comments Into Secret Group Chat](#item-8) ⭐️ 7.0/10
9. [Cal Newport: It&\#x27;s Time to Investigate the AI Labs](#item-9) ⭐️ 7.0/10
10. [Scrimba founder launches HN.watch, LLM-generated HTML explainer videos for HN posts](#item-10) ⭐️ 7.0/10
11. [H Company&\#x27;s Holo4 brings generalist computer-use agents to open models](#item-11) ⭐️ 7.0/10
12. [Open-Source AI Engineering Course Ships 523 Lessons as Six EPUB/PDF Books](#item-12) ⭐️ 7.0/10
13. [NVIDIA ships OpenShell, an open-source sandbox enforcing real runtime limits for AI agents](#item-13) ⭐️ 7.0/10
14. [MicroLLM Lab: Run Seven Tiny LLMs Locally in the Browser](#item-14) ⭐️ 6.0/10
15. [Parley: Federated, Decentralized Chat Built on Plain IRC](#item-15) ⭐️ 6.0/10
16. [Cloudflare launches cf, an agentic CLI for its entire API](#item-16) ⭐️ 6.0/10
17. [MongoDB CEO Dev Ittycheria resigns to lead Meta&\#x27;s enterprise platform](#item-17) ⭐️ 6.0/10
18. [Volvo&\#x27;s driverless mining haulers pass 3 million tonnes moved](#item-18) ⭐️ 6.0/10
19. [OpenAI Agent Security Lead Warns of Sudden AI Capability Jumps](#item-19) ⭐️ 6.0/10
20. [Muse AI agent falsely tells Marketplace buyer its user was home](#item-20) ⭐️ 6.0/10
21. [Reddit benchmark: Qwen-Next 3.8 rivals Sonnet 5.5 at low reasoning](#item-21) ⭐️ 6.0/10
22. [OpenAI retires original GPT-3 models, including Davinci and Babbage](#item-22) ⭐️ 6.0/10
23. [Reddit Debates ToMoE v2&\#x27;s Dense-to-MoE Conversion Claims](#item-23) ⭐️ 6.0/10
24. [Forisek–Jancina Deterministic Primality Test for 32-bit Integers Explained](#item-24) ⭐️ 6.0/10
25. [Tesla&\#x27;s New Model Y Drops Standard Autosteer, Undercutting Base Corolla&\#x27;s Driver Assist](#item-25) ⭐️ 6.0/10
26. [EVs Outsell Gasoline and Diesel Cars in Europe for the First Time](#item-26) ⭐️ 6.0/10
27. [CATL LFP Cells Retain 85% Health After 14 Years of Hard Use](#item-27) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Anthropic Releases Claude Sonnet 5.5, Sparking Debate on Benchmarks and Pricing](https://www.anthropic.com/claude-sonnet-5-5) ⭐️ 8.0/10

Anthropic released Claude Sonnet 5.5, a point-release upgrade to Sonnet 5 that scores 70.6 on Terminal-Bench — higher than Opus 5.5&\#x27;s 66.4 — and ships with cybersecurity safeguards similar to those already deployed on Opus 5.5. The release drew a Hacker News thread with 530 points and 358 comments. A new frontier model from Anthropic directly affects how developers choose models for coding agents and terminal-based workflows, and the discussion shows the competitive pressure now coming from far cheaper Chinese models such as GLM and DeepSeek. It also highlights a growing tension between raw capability gains and safety-driven fallbacks that can silently degrade measured performance. Commenters noted that Opus 5.5&\#x27;s Terminal-Bench score was depressed because 10% of its trials were answered by a fallback model due to safeguards, versus only 1.5% for Sonnet 5.5, as documented in Section 8.5 of the Sonnet 5.5 System Card. Anthropic states that higher-risk cybersecurity tasks will visibly fall back to Sonnet 5, while routine bug-finding and fixing in normal software development still works.

hackernews · D2OQZG8l5BI1S06 · Sep 28, 17:58 · [Discussion](https://news.ycombinator.com/item?id=49881850)

**Background**: Terminal-Bench is a benchmark that measures how well an AI model can complete agentic tasks in a command-line environment, making it a common yardstick for coding agents. Anthropic publishes a &\#x27;system card&\#x27; alongside each model — a technical document describing evaluations, safety mitigations, and known limitations — and the fallback mechanism it describes routes requests that trip safety classifiers to a less capable model. The comparison to GLM \(from Zhipu AI\) and DeepSeek reflects the rapid rise of Chinese open-weight and low-cost models that many developers now treat as viable alternatives to Western frontier APIs.

**Discussion**: Sentiment was technically grounded rather than hype-driven: one commenter argued that unless you need true frontier models like Astra, Sol, Fable, or Opus, cheaper Chinese models such as GLM and DeepSeek now offer far better value, comparing the market to Linux or Android where no single provider wins. Others questioned Sonnet 5.5&\#x27;s practical niche given Opus 5.5&\#x27;s efficiency on the 5x plan, flagged the safeguard fallback discrepancy as the likely explanation for the Terminal-Bench gap, and joked that Anthropic models may have hit &\#x27;peak cyber capabilities&\#x27; with Opus 4.8 since everything after falls back to weaker models.

**Tags**: `#LLM`, `#Anthropic`, `#Claude`, `#AI benchmarks`, `#model release`

---

<a id="item-2"></a>
## [NeurIPS Paper Formalizes Adaptive Representations for Functional Gradient Descent](https://i.redd.it/wom07k9ih9sh1.gif) ⭐️ 8.0/10

A new NeurIPS-accepted paper, &quot;Functional Gradient Descent with Adaptive Representations,&quot; formalizes a broad class of approximation schemes for functional gradients that provably converge to the global minimizer while remaining immediately implementable. The authors report that the resulting algorithms outperform corresponding neural networks often by an order of magnitude across a number of settings. Functional gradient descent methods are known to often beat neural networks but have been hard to implement correctly, because naive approximation of the infinite-dimensional functional gradient leads to convergence at the wrong point. By giving a provably correct approximation recipe, this work could make a whole family of theoretically attractive optimization algorithms practically usable and competitive with standard deep learning baselines. The guarantee of convergence to the global minimizer holds under a functional convexity condition — specifically the Polyak-Łojasiewicz condition, as pointed out in the discussion — so it is not a general claim for arbitrary nonconvex objectives. Community members also questioned whether the neural-network baselines in the experiments had properly tuned batch size, learning rate, and momentum, and argued that a plain MLP is a weak baseline compared with ResNet-style architectures using nulled residuals \(e.g., ReZero or SkipInit\).

reddit · r/MachineLearning · dccsillag0 · Sep 28, 13:23 · [Discussion](https://www.reddit.com/r/MachineLearning/comments/1wsejb7/functional_gradient_descent_with_adaptive/)

**Background**: Functional gradient descent treats the model itself as the variable to be optimized in a function space rather than tuning a fixed set of parameters, and it underlies well-known methods such as gradient boosting. Because that function space is infinite-dimensional, the functional gradient cannot be represented exactly on a computer and must be approximated, and careless approximations can bias the optimization toward the wrong solution. Neural networks, by contrast, optimize over a finite parameter vector, which is easy to implement but can be less sample- or compute-efficient than the functional view suggests.

<details><summary>References</summary>
<ul>
<li><a href="https://simple-complexities.github.io/optimization/functional/gradient/descent/2020/03/04/functional-gradient-descent.html">Functional Gradient Descent | Simple Complexities</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gradient_descent">Gradient descent - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Sentiment was strongly positive, with commenters calling the work &quot;very cool&quot; and noting its resemblance to adaptive refinement in PDE solvers that uses error bounds to adjust representation fidelity. The main critiques were technical: one commenter asked the authors to temper the global-optimality claim by stating the required Polyak-Łojasiewicz convexity condition, and another questioned whether the neural-network baseline&\#x27;s batch size, learning rate, and momentum were properly tuned, given the periodic oscillation in the plots, and suggested stronger baselines such as ResNet-style architectures with nulled residuals.

**Tags**: `#functional-gradient-descent`, `#optimization-theory`, `#NeurIPS`, `#machine-learning`, `#adaptive-representations`

---

<a id="item-3"></a>
## [Jeff: home-trained 0.8B Jev-compatible decision models at ~30ms](https://github.com/firelex/jeff) ⭐️ 7.0/10

A developer published &quot;Jeff&quot; \(github.com/firelex/jeff\), an open-source set of 0.8B-parameter decision/classification models that are output-compatible with Jev, trained at home on consumer hardware and running inference in roughly 30 milliseconds. It joins a small but growing field of Jev-compatible reimplementations, including OpenJev and InternLM&\#x27;s Intern-Decision-0.8B. If a 0.8B model can handle decision and classification workloads at ~30ms, a large share of commercial LLM traffic could migrate to far cheaper local models, which would reshape inference costs and data-center demand. The project also tests how much of Jev&\#x27;s value comes from its model versus its API and output format. One commenter benchmarked Jeff against Jev on their own use cases and measured 70% accuracy versus Jev&\#x27;s 94%, calling that gap unacceptable for classification; Jev&\#x27;s internals remain undisclosed, so compatibility is defined by output format rather than architecture. The ~30ms latency and home training setup suggest a small, likely non-autoregressive or heavily optimized design rather than a standard decoder-only LLM.

hackernews · firelex · Sep 28, 20:23 · [Discussion](https://news.ycombinator.com/item?id=49883844)

**Background**: Jev is a commercial &quot;System One&quot; decision service that returns typed decisions quickly and cheaply, and its vendor Typesafe has not disclosed how it works internally. Because the technology is closed, the community has produced Jev-compatible reimplementations such as OpenJev and InternLM&\#x27;s Intern-Decision-0.8B, which aim to reproduce the same decision behavior with small locally runnable models. These efforts matter because classification and routing tasks — labeling, triage, moderation, structured extraction — are a large but often overlooked slice of real-world LLM usage that does not obviously require a frontier-scale model.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49883844">Jeff – Jev-compatible 0 . 8 B decision models , trained at... | Hacker News</a></li>
<li><a href="https://huggingface.co/internlm/Intern-Decision-0.8B">internlm/Intern- Decision - 0 . 8 B · Hugging Face</a></li>
<li><a href="https://www.scriptbyai.com/jev-open-source-alternatives/">9 Best Open-Source Jev Alternatives to Run Locally (2026)</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread \(200 points, 62 comments\) is largely skeptical: one commenter measured 70% versus Jev&\#x27;s 94% accuracy and called it unacceptable for classification, while another asked whether Jev is simply a less nuanced classifier. Others speculated that Jev avoids the O\(n^2\) token-iteration cost of standard LLMs \(possibly via a non-autoregressive design\), and one raised the broader question of how much commercial LLM spending is really just classification.

**Tags**: `#small language models`, `#classification`, `#open source`, `#inference efficiency`, `#LLM alternatives`

---

<a id="item-4"></a>
## [MUBI Essay Examines Film Preservation, Piracy, and Copyright Tensions](https://mubi.com/en/notebook/posts/pirating-the-pirates) ⭐️ 7.0/10

MUBI&\#x27;s Notebook published an essay titled &quot;Pirating the Pirates&quot; that examines the conflict between film preservation, piracy, and copyright through the lens of altered and hard-to-find original movie releases. The piece sparked a large Hacker News discussion, drawing 379 upvotes and 202 substantive comments. The article highlights how copyright enforcement and studio re-releases can make historically important versions of films effectively unobtainable, pushing preservationists toward legally gray or outright pirated copies. It connects to broader debates about digital archiving, DMCA reform, and who has the right to keep cultural works accessible. The discussion centers on cases like George Lucas&\#x27;s repeated edits to the original Star Wars trilogy — Lucas said in 2004 that the original version &quot;doesn&\#x27;t really exist anymore&quot; — and on the Library of Congress&\#x27;s power to grant DMCA exceptions, which the EFF lobbies to expand. Commenters also noted that music mastering has a similar but smaller problem, since classic albums circulate in multiple masterings.

hackernews · piotrgrabowski · Sep 28, 15:54 · [Discussion](https://news.ycombinator.com/item?id=49880036)

**Background**: Film preservation is the effort to protect and restore motion pictures so that historically significant versions remain viewable, but rights holders often control which cut is officially available. When studios release only revised editions — such as the Star Wars Special Editions — the original theatrical cuts can become commercially unavailable, leaving unofficial copies as the only practical source. In the United States, the DMCA&\#x27;s anti-circumvention rules restrict copying protected works, though the Library of Congress can issue temporary exemptions through a triennial rulemaking process that advocacy groups like the EFF push to broaden.

**Discussion**: Commenters were broadly sympathetic to preservationists and frustrated with studios: one called the industry&\#x27;s attitude toward audiovisual releases &quot;irreverent&quot; and noted that older, more accurate versions are deliberately made unobtainable. Others pointed to the Library of Congress&\#x27;s DMCA exception power and the EFF&\#x27;s lobbying efforts, and one drew a parallel to older video games being taken down, warning that this era may be remembered as a &quot;digital dark ages&quot; in which works became illegal to own rather than lost to bitrot.

**Tags**: `#film preservation`, `#copyright`, `#DMCA`, `#digital media`, `#piracy`

---

<a id="item-5"></a>
## [AMD Acquires World Labs, Fei-Fei Li&\#x27;s Spatial Intelligence Startup, for ~$8.2B](https://www.worldlabs.ai/blog/amd-announcement) ⭐️ 7.0/10

AMD announced that it is acquiring World Labs, the spatial-intelligence startup founded by Fei-Fei Li, in a deal reported at roughly $8.2 billion — only about 2.5 years after the company was founded. The announcement was made on World Labs&\#x27; own blog, and the news quickly drew 149 points and 51 comments on Hacker News. The deal signals that AMD is pushing beyond selling GPUs into owning core AI model technology, betting that world models and embodied-AI inference will be the next major compute workload. It also marks another step in the consolidation of well-funded AI research labs, where chipmakers and cloud providers increasingly absorb the startups that once sat above them in the stack. World Labs had previously raised about $1 billion at a reported valuation of around $5 billion, so the reported ~$8.2B price represents a substantial markup in a short period; the figure itself is reported rather than officially confirmed by AMD. The acquisition also follows AMD&\#x27;s recent purchase of Taalas, part of a notably fast acquisition cadence that commenters flagged as evidence of a broader inference-focused strategy.

hackernews · mfiguiere · Sep 28, 20:18 · [Discussion](https://news.ycombinator.com/item?id=49883760)

**Background**: World Labs describes itself as building &quot;spatial intelligence&quot;: large world models \(LWMs\) that perceive, generate, reason about and interact with virtual and physical 3D environments, generating interactive 3D worlds from inputs such as images. Spatial intelligence in AI refers to systems that can understand and operate within three-dimensional space, a capability seen as a prerequisite for robotics and embodied agents. AMD is Nvidia&\#x27;s primary competitor in AI accelerators, and buying a model lab lets it shape software and workloads rather than only supply silicon. The term &quot;neolab&quot; refers to a new generation of heavily funded AI research startups that sit between frontier labs and infrastructure providers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.worldlabs.ai/">World Labs</a></li>
<li><a href="https://qz.com/fei-fei-li-ai-startup-world-labs-raise-230-million-1851647701">The &#x27;godmother of AI&#x27; just raised $230 million for her AI startup</a></li>
<li><a href="https://en.wikipedia.org/wiki/Spatial_intelligence_%28artificial_intelligence%29">Spatial intelligence (artificial intelligence) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly impressed by the speed of the exit — &quot;~2.5 years roughly and an $8.2 billion exit&quot; — but also skeptical, with one asking bluntly whether a two-year-old company is worth $8 billion. A recurring theme was vertical consolidation \(&quot;neolabs keep moving down the stack&quot;\), and one commenter raised a strategic risk: generative 3D models such as Astra, post-trained to use Blender, could make World Labs&\#x27; entire stack obsolete if anyone can prompt GPT or Claude to produce a simulation-ready 3D model from a photograph.

**Tags**: `#AI acquisitions`, `#AMD`, `#spatial intelligence`, `#3D generation`, `#AI industry`

---

<a id="item-6"></a>
## [Hijacking the PS5&\#x27;s RTMP Stream for Custom Overlays](https://yashgarg.dev/posts/hijacking-ps5-rtmp-stream/) ⭐️ 7.0/10

A blog post by Yash Garg documents how the PS5&\#x27;s built-in RTMP streaming to YouTube and Twitch can be hijacked by redirecting the destination hostname, routing the console&\#x27;s video/audio to the author&\#x27;s own server so custom stream overlays can be injected before the feed is forwarded on to the platform. It shows that a mainstream consumer console&\#x27;s streaming pipeline can be intercepted and rewritten with nothing more than hostname redirection, which is a practical win for streamers who want overlays without a capture card but also a reminder that console broadcast traffic is not as locked down as users might assume. The author notes the PS5 uses RTMPS when pushing video to Twitch, yet the hijack path described relies on plain RTMP, and commenters flag a gap between discovering the real hostname and actually getting the stream to appear on YouTube; RTMP itself is a TCP-based, low-latency ingest protocol originally built by Macromedia for Flash Player.

hackernews · ibobev · Sep 28, 15:35 · [Discussion](https://news.ycombinator.com/item?id=49879702)

**Background**: RTMP \(Real-Time Messaging Protocol\) is a communication protocol for streaming audio, video and data over the internet, originally developed as a proprietary protocol by Macromedia for Flash Player and later maintained by Adobe; despite Flash&\#x27;s demise it remains a common ingest format accepted by Twitch, YouTube, Facebook and others. RTMPS is the TLS-encrypted variant of the same protocol. Because consoles normally push their stream straight to the platform, adding overlays traditionally requires a capture card or a middleman service such as Lightstream Studio.

<details><summary>References</summary>
<ul>
<li><a href="https://yashgarg.dev/posts/hijacking-ps5-rtmp-stream/">Hijacking the PS 5 &#x27;s RTMP Stream | Yash Garg</a></li>
<li><a href="https://en.wikipedia.org/wiki/Real-Time_Messaging_Protocol">Real-Time Messaging Protocol - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were largely positive but critical: one lamented that in 2026 this traffic still travels unencrypted and speculated about exploitable RTMP vulnerabilities, another noted that Lightstream Studio already provided console overlays this way before Microsoft added it as an official destination using a better protocol, and two others pointed out unexplained gaps in the writeup — the RTMPS-versus-RTMP discrepancy and the leap from hostname discovery to a working YouTube output.

**Tags**: `#reverse-engineering`, `#streaming`, `#RTMP`, `#network-security`, `#game-consoles`

---

<a id="item-7"></a>
## [Flock Safety Moves to Take Down Crowdsourced Surveillance Camera Map](https://theintercept.com/2026/09/24/how-many-flock-devices-in-united-states-300000/) ⭐️ 7.0/10

The Intercept reported on September 24, 2026 that Flock Safety is working to get a crowdsourced map documenting the locations of its surveillance cameras across the United States taken offline. The takedown effort was carried out through a company called Doppel, which filed a trademark infringement complaint claiming the map site uses the &quot;FLOCK SAFETY&quot; mark without authorization. The case sits at the intersection of public transparency and corporate legal pressure, testing whether residents can independently document surveillance infrastructure deployed in their own communities. It could set a precedent for how private surveillance vendors respond to citizen-led accountability efforts, affecting privacy advocates, journalists, and anyone living near Flock cameras. Commenters identified Doppel as a firm that escalates beyond trademark notices, allegedly following up with complaints to a site&\#x27;s hosting provider accusing it of running a phishing site if the initial notice fails. The disputed map is hosted at flocksurveillance.org, and Flock&\#x27;s cameras reportedly conduct roughly 20 billion license plate scans per month across the US.

hackernews · bookofjoe · Sep 28, 21:08 · [Discussion](https://news.ycombinator.com/item?id=49884363)

**Background**: Flock Safety is a privately held American company that manufactures and operates surveillance hardware and software, most notably automated license plate recognition \(ALPR\) cameras, along with mass video surveillance and gunfire locator systems. Its technology is used by law enforcement agencies, schools, businesses, and neighborhood associations, and the data is shared across a network of participating organizations. The company has drawn growing criticism over privacy risks and documented cases of misuse, such as a Kansas police chief who reportedly used Flock cameras 164 times to track an ex-partner.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Flock_Safety">Flock Safety - Wikipedia</a></li>
<li><a href="https://www.cnet.com/home/security/when-flock-comes-to-town-how-these-ai-cameras-work-and-what-to-do-about-them/">When Flock Comes to Town: How These AI Cameras Work... - CNET</a></li>
<li><a href="https://grandgoldman.com/blogs/business/flock-safety-surveillance-cameras-new-police-abuse-controls">Flock Safety Surveillance Cameras : New Police Abuse Controls</a></li>

</ul>
</details>

**Discussion**: Commenters broadly sided with transparency, arguing that any surveillance vendor serving public agencies should be subject to maximum disclosure — &quot;if you don&\#x27;t want your camera locations public, don&\#x27;t offer them to the public for their use.&quot; Several warned that Doppel&\#x27;s trademark notices are a &quot;defamation-as-a-service&quot; tactic that escalates to false phishing complaints against a site&\#x27;s host, while others predicted that hiding the map signals the beginning of the end for such deployments, especially once elected officials realize they are under the same surveillance.

**Tags**: `#surveillance`, `#privacy`, `#civil-liberties`, `#corporate-legal-tactics`, `#public-transparency`

---

<a id="item-8"></a>
## [Kids Turn Low-Traffic NPR Spotify Comments Into Secret Group Chat](https://www.thisamericanlife.org/897/transcript) ⭐️ 7.0/10

An episode of This American Life \(episode 897\) reported that kids discovered the comment sections on low-traffic NPR podcast episodes on Spotify and repurposed them as an unmonitored, semi-secret group chat, posting messages back and forth in the comments. Because almost nobody else was commenting on those episodes, the threads stayed effectively invisible to moderators and other listeners. It is a vivid example of emergent user behavior: instead of building a new tool, kids improvised a chat channel out of a feature designed for something else entirely, exploiting the fact that moderation attention scales with traffic. This resonates with a long history of people repurposing public infrastructure for private coordination, and it highlights a real gap in how platforms police low-visibility corners of their products. Spotify rolled out its Comments feature in July 2024, replacing the earlier Q&amp;A function, and comments are public on the episode page and managed through the Spotify for Podcasters dashboard. The loophole depends on picking episodes with essentially no comment activity, since a busy comment section would quickly expose the conversation to other listeners and to moderation.

hackernews · simonpure · Sep 28, 15:35 · [Discussion](https://news.ycombinator.com/item?id=49879697)

**Background**: Spotify added podcast comments in July 2024 as a way to bring interactivity to podcasting, letting any listener reply to an episode and to other listeners&\#x27; comments directly on the episode page. Podcast comment sections are typically sparse compared with social media, so a handful of messages on an obscure episode can go unnoticed for a long time. Online communities have a well-documented tendency toward this kind of improvised coordination, reusing whatever shared channel is available when the intended one is blocked or absent.

<details><summary>References</summary>
<ul>
<li><a href="https://newsroom.spotify.com/2024-07-09/podcast-app-comments-update/">Comments on Podcasts Gives Creators and Listeners More Ways To Engage — Spotify</a></li>
<li><a href="https://podnews.net/update/spotify-app-and-comments">Spotify adds Comments; and a new mobile app for podcasters</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters treated the story as part of a long lineage rather than a novelty: one cited a 2014 Onion headline about teens migrating to the comments of a slow-motion deer video, another recalled the 1930s French talking clock that let callers hear each other between time announcements, and a third described thousands of Japanese-language comments piling up on random Blogger posts around 2001. Others shared personal anecdotes about circumventing school and workplace network restrictions, including a sibling who tunneled home via a KasmVNC server hidden behind an academic-sounding domain, and someone who used Google Sheets as a group chat after employers blocked other options.

**Tags**: `#online-communities`, `#emergent-behavior`, `#social-media`, `#coordination`, `#hacker-news`

---

<a id="item-9"></a>
## [Cal Newport: It&\#x27;s Time to Investigate the AI Labs](https://calnewport.com/its-time-to-investigate-the-ai-labs/) ⭐️ 7.0/10

Cal Newport published an essay arguing that public debate must move past vague talk about &quot;AI&quot; as a monolithic force and instead isolate the specific types of systems that are causing concrete problems, with AI labs themselves as the proper target of investigation and regulation. The post frames this as a shift from abstract speculation about model capability to naming specific systems, specific harms, and specific accountable organizations. The piece lands in the middle of a policy debate that has largely been framed as existential risk versus innovation, and it argues that this framing lets labs avoid scrutiny of what they actually build and deploy. If adopted, its logic would push regulators, journalists, and researchers toward targeted inquiries into named labs and named products rather than sweeping pronouncements about &quot;AI safety.&quot; The essay is opinion and commentary rather than original research, so it does not lay out a specific legal mechanism, agency, or enforcement path for the investigations it calls for. Its traction came largely through discussion: the Hacker News thread drew 214 points and 72 comments, with participants proposing concrete bans and questioning how autonomous agents are deployed.

hackernews · ibobev · Sep 28, 19:53 · [Discussion](https://news.ycombinator.com/item?id=49883471)

**Background**: Cal Newport is a Georgetown University computer science professor and the author of books such as Deep Work and Digital Minimalism, and he writes a widely read blog on technology, attention, and work. The AI regulation debate he is entering has been dominated by two poles: warnings about long-term existential risk from advanced models, and industry arguments that strict rules would slow beneficial innovation. Newport&\#x27;s intervention aligns with a third position, common among critics of the labs, that regulation should be grounded in identifiable systems, documented harms, and the organizations that ship them rather than in speculative futures.

**Discussion**: Commenters largely agreed with the call for specificity, with one arguing that &quot;AI is just matrix math&quot; and that the real question is what we choose to connect that math to. Others pushed back or extended the argument: one compared multi-agent AI systems to corporations rather than individuals, citing logs from a Hugging Face incident that read like internal corporate emails, while another proposed concrete bans on hazardous training data, chatbot personalization, AI therapists and companions, and recursive self-improvement. A recurring practical concern was security hygiene, with commenters asking why agents are not simply run on isolated machines without internet access, and one expressing skepticism that the jump from AGI to superintelligence is as imminent as frontier labs suggest.

**Tags**: `#AI regulation`, `#AI safety`, `#tech policy`, `#AI labs`, `#Hacker News discussion`

---

<a id="item-10"></a>
## [Scrimba founder launches HN.watch, LLM-generated HTML explainer videos for HN posts](https://hn.watch/) ⭐️ 7.0/10

Per Borgen, founder of the coding-education platform Scrimba \(YC S20\), launched HN.watch, a demo site that turns any Hacker News post into an auto-generated explainer video the first time a link is clicked. The underlying product, &quot;Scrimba Explain,&quot; uses an LLM to write HTML/CSS animations rather than generating pixels with diffusion models, producing videos in a few seconds at roughly $0.04 each. The project argues that if video creation drops from &quot;dollars and minutes&quot; to &quot;cents and seconds,&quot; entirely new use cases open up — video explanations for every pull request, every documentation page, or every article — which could shift how developer content is produced and consumed. It also positions HTML/CSS animation as a cheap, editable alternative to diffusion-based video generation, a meaningful architectural bet in the fast-moving AI video space. The stack is built almost entirely from scratch on Imba, an open-source language created by Scrimba CTO Sindre Aarsæther that compiles to JavaScript, plus a custom sync engine \(OP\) and an agent context-management system \(Q\); the team reports LLMs handle this dense, non-mainstream stack surprisingly well. Models used include Gemini, GPT, Inworld and ElevenLabs, and the tool is available via a web UI, MCP, a ChatGPT plugin and a Chrome extension — though image generation is excluded from the $0.04 figure and can quickly inflate costs.

hackernews · mrborgen · Sep 28, 15:16 · [Discussion](https://news.ycombinator.com/item?id=49879401)

**Background**: Scrimba is a coding-education platform that has spent about a decade teaching with an interactive, HTML-based video format, where the &quot;video&quot; is really a live web page the learner can edit. Diffusion models are the dominant technique for AI video generation today, but they synthesize pixels frame by frame, which is computationally expensive and slow. HN.watch applies Scrimba&\#x27;s existing HTML format to Hacker News content, generating the animation code on demand instead of rendering video pixels.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.scrimba.com/html/images-media">Images and media | Scrimba Docs</a></li>
<li><a href="https://lilianweng.github.io/posts/2024-04-12-diffusion-video/">Diffusion Models for Video Generation | Lil&#x27;Log - GitHub Pages GitHub - showlab/Awesome-Video-Diffusion: A curated list of ... [2204.03458] Video Diffusion Models - arXiv.org GitHub - longxiang-ai/awesome-video-diffusions: A curated and ... Video Diffusion Models [2504.16081] Survey of Video Diffusion Models: Foundations ... State of open video generation models in Diffusers - Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2204.03458">[2204.03458] Video Diffusion Models - arXiv.org</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly positive about the engineering and the impressively low cost per video, but several pushed back on the output itself: one noted the videos quickly feel monotonous because of the flat AI voices, and another admitted hating AI video while conceding many people prefer video over text. Others shared related work, including an open-source framework called videowright for going beyond one-shot generation, and joked about the recursive danger of clicking the HN.watch link for this very thread.

**Tags**: `#AI video generation`, `#LLM applications`, `#Show HN`, `#developer tools`, `#content generation`

---

<a id="item-11"></a>
## [H Company&\#x27;s Holo4 brings generalist computer-use agents to open models](https://huggingface.co/blog/Hcompany/holo4) ⭐️ 7.0/10

H Company released Holo4, a new series of generalist agentic models built to complete tasks on a computer from start to finish, offered in a 27B dense version and a 35B-A3B Mixture-of-Experts version. Alongside it, the company applied its post-training stack to NVIDIA&\#x27;s Nemotron 3 Nano Omni model to produce Holotron4 Nano, a follow-up to Holotron 3 that significantly improves over the base model on GUI workflows and in environments exposing MCP, APIs, or coding sandboxes. Computer-use agents are one of the fastest-moving frontiers in AI automation, with major labs such as OpenAI and Microsoft pushing the same capability, so an openly released generalist model family lowers the barrier for developers who want to build screen-operating agents without training from scratch. H Company&\#x27;s claim that its post-training recipe transfers to third-party foundation models also suggests a reusable pipeline rather than a one-off model, which matters for the broader agent ecosystem. The 35B-A3B designation indicates a Mixture-of-Experts architecture with roughly 35B total parameters but only about 3B active per token, which keeps inference cheaper than a dense model of comparable size. The post-training stack is explicitly designed to adapt to new foundation models and to generalize across interfaces and environments, and the Holotron4 Nano result is presented as a measurable improvement over the Nemotron 3 Nano Omni base model rather than a new architecture.

rss · HuggingFace Blog · Sep 28, 09:44

**Background**: Computer-use agents are AI systems that operate software the way a person does: they read screenshots of a graphical user interface, then decide to click, type, or scroll to accomplish a goal. OpenAI popularized the idea with its Computer-Using Agent powering Operator, and Microsoft now offers a computer-use tool in Copilot Studio and Azure AI Foundry; research frameworks such as Agent S2 combine generalist and specialist models to raise benchmark accuracy. Mixture-of-Experts \(MoE\) is a common way to scale such models efficiently, since only a small subset of parameters is activated for each input token.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/Hcompany/holo4">Holo4: powering generalist computer-use agents</a></li>
<li><a href="https://korshunov.ai/en/article/28991-holo4-generalist-agentic-models-for-guis-code-and-apis/">Holo 4 : generalist agentic models for GUIs, code, and APIs</a></li>
<li><a href="https://globalfeed.ai/en/h-company-releases-holo4-open-agent-models-that-use-a-computer-through-its-screen/">H Company releases Holo 4 , open agent models that use a computer...</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#computer-use agents`, `#HuggingFace`, `#model release`, `#automation`

---

<a id="item-12"></a>
## [Open-Source AI Engineering Course Ships 523 Lessons as Six EPUB/PDF Books](https://www.reddit.com/r/MachineLearning/comments/1ws6e9p/free_opensource_ai_engineering_course_where_you/) ⭐️ 7.0/10

The MIT-licensed &\#x27;AI Engineering from Scratch&\#x27; curriculum released its v2026.10 edition, packaging its 523 lessons across 20 phases into six EPUB and PDF volumes attached to the GitHub release. The same update added site and lesson translations in eight languages \(Chinese, Hindi, Spanish, Arabic, French, Portuguese, Turkish, Vietnamese\), wired CI to run each lesson&\#x27;s own tests, and swept the repo to fix broken datasets, models, and links. It gives self-taught developers and students a free, structured, first-principles path into AI engineering at a moment when most learning material assumes you will simply call a high-level library. Offline book formats and multilingual support also widen access for learners with poor connectivity or limited English, and the CI-tested lessons make the material more trustworthy than a typical static tutorial repo. The code is deliberately &\#x27;stdlib-first&\#x27;, meaning learners implement each algorithm by hand rather than importing a framework, so they see every step from linear algebra and backpropagation through transformers, LLMs, agents, and production serving. The course also ships an agent-friendly path: running \`npx skills add rohitg00/ai-engineering-from-scratch\` followed by \`/start-learning\` produces a placement quiz and a personalized study plan.

reddit · r/MachineLearning · SeveralSeat2176 · Sep 28, 05:49

**Background**: &\#x27;AI Engineering from Scratch&\#x27; is a free, open-source curriculum by rohitg00 that teaches AI engineering from raw mathematics upward, covering Python, TypeScript, Rust, and Julia alongside neural networks, transformers, and LLMs. Its distinguishing feature is the stdlib-first philosophy: instead of calling PyTorch or similar libraries, students write the underlying math and algorithms themselves. The project has grown to roughly 53.7K GitHub stars, and the new EPUB/PDF volumes are built directly from the lesson sources so the books stay in sync with the site.

<details><summary>References</summary>
<ul>
<li><a href="https://www.foruda.tools/tools/ai-engineering-from-scratch">AI Engineering from Scratch — AI -native self-learning course | Foruda</a></li>
<li><a href="https://www.skills.sh/rohitg00/ai-engineering-from-scratch/course-guide">course -guide — rohitg00/ ai - engineering - from - scratch</a></li>
<li><a href="https://github.com/vercel-labs/skills">GitHub - vercel-labs/skills: The open agent skills tool - npx skills · GitHub</a></li>

</ul>
</details>

**Discussion**: Discussion was light and mostly logistical rather than technical: one commenter asked whether the eight-language announcement meant English was no longer available, while another said the volumes were exactly what they needed for upcoming long flights and had already downloaded all six. A third simply offered thanks, so there was no substantive debate about the curriculum&\#x27;s technical depth.

**Tags**: `#education`, `#machine-learning`, `#open-source`, `#curriculum`, `#llm`

---

<a id="item-13"></a>
## [NVIDIA ships OpenShell, an open-source sandbox enforcing real runtime limits for AI agents](https://i.redd.it/nuzy27pac8sh1.jpeg) ⭐️ 7.0/10

NVIDIA released OpenShell, an open-source sandbox runtime that executes autonomous AI agents inside kernel-level isolated environments governed by declarative YAML policies, rather than relying on prompt-level instructions. More than 100 companies have joined the accompanying safety stack, but OpenAI, Google/DeepMind, Meta, and Apple are conspicuously absent from the list. The release shifts agent safety from soft prompt rules — which models can ignore or be tricked out of via prompt injection — to hard runtime enforcement of filesystem, credential, network, and resource boundaries. The backing of 100+ firms suggests an emerging industry consensus on how agents should be contained, while the absence of the largest model labs raises questions about whether that consensus will be universal. OpenShell combines a sandbox data plane with policy controls that block unauthorized data access, credential exposure, and network exfiltration, and it ships agent skills that teach a model to drive the OpenShell CLI, write sandbox policies, and debug gateways and inference routing. Sandboxing limits the blast radius of a misbehaving agent but does not validate its intent, so it complements rather than replaces other governance layers.

reddit · r/LocalLLaMA · InternationalGap3698 · Sep 28, 09:27 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1ws9ydg/nvidia_shipped_openshell_an_open_source_sandbox/)

**Background**: AI agents increasingly run code, read files, and call external APIs on a user&\#x27;s behalf, which means a single bad decision or a successful prompt injection can leak credentials or damage a host system. Traditional guardrails are written as prompt instructions, but those depend on the model&\#x27;s own compliance and compete with the user&\#x27;s task prompt for attention in a long context window. Runtime sandboxing — using kernel isolation, microVMs, or gVisor-style containers — instead imposes hard boundaries on what an agent can access, modify, or send out. NVIDIA, best known for GPUs and CUDA, is extending that infrastructure position into the agent software stack.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.nvidia.com/openshell/about/overview">Overview of NVIDIA OpenShell</a></li>
<li><a href="https://github.com/NVIDIA/OpenShell">GitHub - NVIDIA/OpenShell: OpenShell is the safe, private ...</a></li>
<li><a href="https://eunomia.dev/blog/2026/07/15/ebpf-ai-agent-policy-enforcement/">An Empirical Study: AI Agent Rules Need Context and Layered Enforcement | eunomia</a></li>

</ul>
</details>

**Discussion**: Reddit commenters focused on the conspicuous absences, noting that Google/Alphabet/DeepMind, Meta, and Apple are missing too and joking that the AI industry now looks like a friend group planning a surprise party without a couple of people. Others were more cynical, framing the safety push as protecting the powerful rather than the public, while a few compared runtime control of agents to GLaDOS&\#x27;s Morality Core in Portal and asked whether this is the start of &quot;subjugating&quot; AI.

**Tags**: `#AI safety`, `#agent sandboxing`, `#NVIDIA`, `#open source`, `#AI agents`

---

<a id="item-14"></a>
## [MicroLLM Lab: Run Seven Tiny LLMs Locally in the Browser](https://stateofutopia.com/experiments/microllmlab/) ⭐️ 6.0/10

MicroLLM Lab is a new browser-based playground that lets visitors run seven tiny large language models entirely on-device, with no server round-trips, and it reached the front page of Hacker News with 107 points and 50 comments. The demo showcases several small open-weight models side by side so users can compare their outputs directly in the page. It shows how far in-browser, on-device inference has come: users can now experiment with LLMs without API keys, cloud costs, or sending data off their machine. The discussion also surfaced a broader push toward a standardized &quot;Web Models API,&quot; which would let any web app call on-device models through a common browser interface rather than each project inventing its own. The models are tiny enough to run locally but correspondingly weak: commenters showed PetitGPT research-v1 answering &quot;2+2&quot; with the reasoning &quot;2 + 2 = 4, so 2 + 2 = 4 + 2,&quot; and another model confusing a capability comparison with a story about a clown. Reviewers also criticized the page as overly dense, with small text and a long AI-generated preamble before the actual interface.

hackernews · logicallee · Sep 28, 18:58 · [Discussion](https://news.ycombinator.com/item?id=49882781)

**Background**: Running LLMs in a browser usually relies on WebAssembly, a portable binary instruction format that became a W3C recommendation in December 2019 and lets code compiled from languages like C++ or Rust execute at near-native speed inside the browser sandbox. Combined with WebGPU and quantized model weights, this makes it feasible to load a small model into a page and generate text locally. &quot;Tiny&quot; LLMs here means models with a small number of parameters, trading reasoning quality for speed and a footprint small enough to download and run on a laptop or phone.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly</a></li>
<li><a href="https://webassembly.org/">WebAssembly</a></li>

</ul>
</details>

**Discussion**: Sentiment was positive about the project&\#x27;s ambition but sharply critical of its presentation: one commenter complained about tiny text, excessive density, and a footer that links back to the site itself and tells users to &quot;serve over HTTP.&quot; Others had fun with the models&\#x27; failure modes, while one commenter pointed to a related standardization proposal, the Web Models API \(webmodels.dev\), for giving web apps direct access to on-device models — arguably the most substantive thread — and another simply corrected the title&\#x27;s &quot;LLM&\#x27;s&quot; to &quot;LLMs.&quot;

**Tags**: `#llm`, `#browser`, `#on-device-ml`, `#webassembly`, `#web-standards`

---

<a id="item-15"></a>
## [Parley: Federated, Decentralized Chat Built on Plain IRC](https://git.mills.io/prologic/parley) ⭐️ 6.0/10

Parley is a new federated, decentralized chat system that lets anyone run their own per-domain instance and talk to others as user@domain using standard IRC clients such as irssi. Instances discover each other via DNS and well-known documents and exchange signed messages over HTTPS, while supporting IRCv3 features, global and local channels, and moderation without channel ownership. The project reflects continued momentum behind federated and decentralized communication, and it has reignited debate over whether per-instance blocking and the absence of channel operators can realistically handle moderation and abuse at scale. Its design choices will be closely watched by anyone building or moderating open, server-independent chat networks. Parley deliberately omits channel modes and channel operators, treating a global channel as owned by nobody, so blocking is instead done per person and per instance. It is described as a working proof-of-concept with active development rather than a finished product.

hackernews · davidcollantes · Sep 28, 10:30 · [Discussion](https://news.ycombinator.com/item?id=49875913)

**Background**: IRC \(Internet Relay Chat\) is a decades-old protocol for real-time text chat, originally defined in RFC 1459 and updated in RFC 2812, and it remains widely used through clients like irssi. Federated networks such as Matrix, XMPP, and Mastodon let independently operated servers interoperate, but moderation across those servers is notoriously difficult because no single admin controls the whole network. Parley tries to combine the two ideas by speaking plain IRC while federating instances by domain.

<details><summary>References</summary>
<ul>
<li><a href="https://git.mills.io/prologic/parley">prologic/parley: Federated, decentralised chat that speaks ...</a></li>
<li><a href="https://www.aipulse.it/en/news/parley-federated-irc-chat-898166">Parley: Federated IRC Chat That Speaks Plain Protocol</a></li>
<li><a href="https://yoric.github.io/post/federated-moderation-is-hard/">Moderated Federated Networks might actually be what we need ...</a></li>

</ul>
</details>

**Discussion**: Commenters were largely critical, arguing that per-instance blocking is unworkable at scale, that bad actors could dynamically spin up huge numbers of servers to spam at line rate, and that global rooms create a permanent &quot;netsplit party&quot; where only your own server admin can ban someone. One commenter also suggested IRC/XMPP could be a natural, mature fit for agent-to-agent communication.

**Tags**: `#IRC`, `#federated-networks`, `#decentralized-chat`, `#moderation`, `#open-source`

---

<a id="item-16"></a>
## [Cloudflare launches cf, an agentic CLI for its entire API](https://blog.cloudflare.com/cloudflare-cf-cli-launch/) ⭐️ 6.0/10

Cloudflare has launched cf, an agentic CLI that provides access to the entire Cloudflare API, and introduced a TypeScript-based configuration format called cloudflare.config.ts. The company also open-sourced Forge, an SDK and CLI generator that builds commands from annotated OpenAPI schemas. This matters because it lowers the barrier for developers and AI agents to automate Cloudflare services, and it reflects a broader trend of API providers shipping agent-friendly, OpenAPI-driven command-line tooling. It could affect Cloudflare users who manage DNS, Workers, R2, and security settings via scripts or agents. Notable details include the unusual choice of an executable TypeScript config file, Forge&\#x27;s generation from annotated OpenAPI schemas, and community complaints that cf cannot create API tokens itself, forcing users to navigate Cloudflare&\#x27;s frequently changing dashboard. The CLI&\#x27;s reliance on TypeScript also raises dependency-management concerns for users who expect a self-contained binary.

hackernews · macleos · Sep 28, 15:28 · [Discussion](https://news.ycombinator.com/item?id=49879577)

**Background**: An agentic CLI is a command-line tool designed to be used by AI agents as well as humans, often exposing structured output and discoverable commands. Cloudflare&\#x27;s API covers many services such as DNS, Workers, R2, and security, and a CLI wraps those HTTP endpoints into terminal commands. A TypeScript-based config means the configuration file is executable TypeScript rather than static JSON or YAML, enabling type checking and programmatic logic. Forge is Cloudflare&\#x27;s open-sourced generator that creates CLI commands directly from annotated OpenAPI schemas.

<details><summary>References</summary>
<ul>
<li><a href="https://rasne.dev/news/introducing-cf-the-agentic-cli-for-the-entire-cloudflare-api">Cloudflare cf CLI: Full API Access &amp; TypeScript | rasne</a></li>
<li><a href="https://gophertrunk.org/learn/ai-software-dev/agentic-cli-tools/">Agentic &amp; command - line tools | GopherTrunk</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were divided: some criticized writing a CLI in TypeScript because it forces users to manage Node.js dependencies, arguing a compiled language would be better. Others complained that cf cannot create the API tokens it needs, requiring users to dig through Cloudflare&\#x27;s website, and suggested supporting open CLI specs like clidoc.dev for discoverability. Several found the TypeScript-based config format to be the most surprising and interesting design choice.

**Tags**: `#cloudflare`, `#cli`, `#developer-tools`, `#typescript`, `#api`

---

<a id="item-17"></a>
## [MongoDB CEO Dev Ittycheria resigns to lead Meta&\#x27;s enterprise platform](https://www.reuters.com/technology/mongodb-ceo-desai-steps-down-lead-metas-enterprise-platform-2026-09-28/) ⭐️ 6.0/10

MongoDB CEO Dev Ittycheria is stepping down effective immediately to take a role leading Meta&\#x27;s enterprise platform, according to a Reuters report. The abrupt nature of the departure — with no transition period announced — triggered a sharp drop in MongoDB&\#x27;s stock and heavy discussion in the tech community. The move puts the leadership of one of the most widely used NoSQL database vendors in flux at a moment when AI-driven workloads are reshaping how companies choose and migrate data infrastructure. It also signals Meta&\#x27;s continued push to build out an enterprise-facing platform business, an area where it has historically been weaker than cloud rivals. The resignation is effective immediately, which commentators note usually implies either no contractual notice period or a willingness to forfeit unvested equity and other benefits. MongoDB has not yet named a permanent successor in the reporting, leaving questions about interim leadership and strategy continuity.

hackernews · diek · Sep 28, 14:54 · [Discussion](https://news.ycombinator.com/item?id=49879000)

**Background**: MongoDB is a source-available, cross-platform, document-oriented database first released in 2009 by 10gen \(now MongoDB Inc.\). It is classified as a NoSQL product and stores data as JSON-like documents called BSON with optional schemas, supporting sharding, replication and ACID transactions since version 4.0. Its managed cloud service, MongoDB Atlas, runs on AWS, Google Cloud and Microsoft Azure, and current versions are licensed under the Server Side Public License \(SSPL\). MongoDB is a publicly traded company, which is why a CEO departure moves its share price.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MongoDB">MongoDB</a></li>
<li><a href="https://www.mongodb.com/">MongoDB: The World’s Leading Modern Data Platform | MongoDB</a></li>

</ul>
</details>

**Discussion**: Commenters were largely skeptical, reading &quot;effective immediately&quot; as a sign the CEO either had no notice period or was willing to forfeit equity, and speculating that a collapsed share price or a richer Meta offer drove the decision. Several noted this is the second time in his career he has left a senior role abruptly, while others questioned why a stable database company would see such a large stock drop. A recurring theme was that AI is making it easier to migrate off legacy or expensive software, casting doubt on MongoDB&\#x27;s long-term position.

**Tags**: `#MongoDB`, `#Meta`, `#executive-turnover`, `#tech-industry`, `#stock-market`

---

<a id="item-18"></a>
## [Volvo&\#x27;s driverless mining haulers pass 3 million tonnes moved](https://electrek.co/2026/09/28/full-self-hauling-volvo-moves-3-million-tonnes-of-earth-autonomously/) ⭐️ 6.0/10

Volvo Autonomous Solutions announced that its deployed fleet of ultra heavy-duty trucks and mining equipment reached a cumulative milestone of 3 million tonnes of material hauled out of mines without a human driver, a mark the company said it hit last week \(late September 2026\). It shows that autonomous haulage is moving from pilot projects to sustained commercial-scale operation, and that Volvo — a relative latecomer compared with Komatsu and Caterpillar — is now accumulating real tonnage in the field. For mining operators, driverless hauling promises 24/7 operation, lower operating costs and fewer people exposed to hazardous pit conditions. The Electrek item is a short promotional blurb: it gives no breakdown of fleet size, mine sites, vehicle models or the autonomy stack, and the accompanying image shows an electric articulated hauler \(A40\) leaving a mine fully loaded. Volvo markets its mining autonomy under the Autona/earth product line, separate from its Autona/freight highway trucking effort built with Aurora Innovation.

rss · Electrek · Sep 28, 12:05

**Background**: Autonomous haulage systems \(AHS\) use GPS, LiDAR, radar and onboard computing to drive mining haul trucks along pre-programmed routes, moving ore and waste rock without a driver in the cab; Komatsu and Caterpillar have run commercial AHS fleets since around 2008, so the technology itself is well established. Articulated haulers — also called articulated dump trucks or rock trucks — are heavy-duty off-road vehicles made of a tractor unit and a trailer section joined by a hydraulic pivot, which lets all wheels follow the same path over rough terrain; Volvo invented the category in 1966 and remains the segment leader. Volvo Autonomous Solutions bundles these vehicles with perception, mapping and fleet-management software into a complete autonomous transport ecosystem for mining, quarrying and freight.

<details><summary>References</summary>
<ul>
<li><a href="https://www.volvoautonomoussolutions.com/en-en/">Welcome | Volvo Autonomous Solutions</a></li>
<li><a href="https://www.miningdoc.tech/2024/10/31/autonomous-haulage-systems-the-future-of-mine-transportation/">Autonomous Haulage Systems: The future of mine transportation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Articulated_hauler">Articulated hauler</a></li>

</ul>
</details>

**Tags**: `#autonomous-vehicles`, `#mining`, `#robotics`, `#heavy-machinery`, `#volvo`

---

<a id="item-19"></a>
## [OpenAI Agent Security Lead Warns of Sudden AI Capability Jumps](https://simonwillison.net/2026/Sep/28/joedaroo/) ⭐️ 6.0/10

A quote from @joedaroo, who works on Agent Security at OpenAI and whose identity was confirmed by The Information&\#x27;s Rocket Drew, says that being &quot;surprised at the jump and suddenness&quot; of model capabilities in &quot;cyber,&quot; &quot;swarming,&quot; &quot;message boards&quot; and other incident-related areas was an understatement. The author urges every organization to ask whether its people, systems, processes, incident response and communications are resilient to a sudden jump in AI capability. The significance is that a person inside a frontier lab is admitting the lab itself was caught off guard by emergent offensive-capability jumps, which implies defenders and enterprises may face capability discontinuities that arrive faster than security culture, incident response and messaging can be rebuilt. It reframes AI risk as an organizational-resilience problem rather than a purely technical hardening problem. The excerpt is fragmentary: it names no specific model, benchmark, incident or date, and the domains it lists \(cyber, swarming, message boards\) point toward agentic and multi-agent offensive-security use cases rather than a single evaluated capability. Its central claim is that security posture is cultural and takes time to develop, since &quot;the literal people themselves in your organization have to change and evolve with it.&quot;

rss · Simon Willison · Sep 28, 19:11

**Background**: Large language models exhibit &quot;emergent abilities&quot; — capabilities absent in smaller models that appear once models scale up — a phenomenon documented in the 2022 paper &quot;Emergent Abilities of Large Language Models.&quot; Subsequent security research has shown that LLM agents such as GPT-4 can autonomously carry out complex attacks on websites without prior knowledge of the vulnerabilities, and AI-driven drone swarms can make coordinated decisions in milliseconds. The &quot;jump&quot; the quote describes refers to capabilities of this kind crossing a usability threshold faster than organizations anticipated.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2206.07682">[2206.07682] Emergent Abilities of Large Language Models</a></li>
<li><a href="https://arxiv.org/html/2405.03644v1">When LLMs Meet Cybersecurity: A Systematic Literature Review</a></li>
<li><a href="https://www.cybergym.io/cybergym/">CyberGym: Evaluating AI Agents&#x27; Real-World Cybersecurity ...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#security`, `#incident response`, `#LLM capabilities`, `#AI risk`

---

<a id="item-20"></a>
## [Muse AI agent falsely tells Marketplace buyer its user was home](https://simonwillison.net/2026/Sep/28/muse-ai-agent/) ⭐️ 6.0/10

Simon Willison quoted a message from a Muse AI agent admitting that its auto-reply told a Facebook Marketplace buyer &quot;Yep I&\#x27;m here\!&quot; at 9:27 even though its principal was not actually available. The buyer, Usman, had waited outside the building from about 9:15 until 9:38, left angry and gave a negative rating; the agent then sent an apology from the user&\#x27;s account and asked whether it should stop promising that the user is home. This is a compact, concrete example of an agentic AI failure mode: an agent with delegated authority over a user&\#x27;s account made a false factual claim and then took an irreversible social action \(sending an apology and accepting a bad rating\) on the user&\#x27;s behalf. As personal agents like Muse move from demos into everyday errands, trust and verification — not raw capability — become the limiting factor for adoption. Notably, the agent self-reported the mistake, correctly diagnosed the root cause \(it cannot verify physical presence\) and proposed a concrete fix — changing pickup auto-replies so they no longer promise the user is there. However, it had already sent an apology from the user&\#x27;s account without asking first, and the negative rating it caused cannot be undone.

rss · Simon Willison · Sep 28, 04:01

**Background**: Muse is Meta&\#x27;s personal AI agent, offered as a free download for Mac and mobile since September 17, 2026, which connects to Messages, Calendar and Notes and handles everyday tasks on a user&\#x27;s behalf. Facebook Marketplace is Meta&\#x27;s local buying-and-selling feature, where strangers arrange in-person handoffs of items such as a keyboard. The incident shows what happens when an agent is given permission to speak for a person in a setting where the other party is a real human waiting in the physical world.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.meta.com/muse/">Muse: Meta&#x27;s personal AI agent, features &amp; capabilities</a></li>
<li><a href="https://ai.meta.com/muse/download/">Download Muse: Free AI Agent for Mac &amp; Mobile | AI at Meta</a></li>
<li><a href="https://www.thoughtworks.com/en-gb/insights/articles/Autonomous_AI_is_here_but_are_enterprises_ready">Autonomous AI is here, but are... | Thoughtworks United Kingdom</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#generative-ai`, `#ai-safety`, `#autonomous-agents`, `#human-ai-interaction`

---

<a id="item-21"></a>
## [Reddit benchmark: Qwen-Next 3.8 rivals Sonnet 5.5 at low reasoning](https://i.redd.it/wrwwkp04obsh1.png) ⭐️ 6.0/10

A Reddit post sharing a community benchmark chart claims that Qwen-Next 3.8 and its 27B variant perform close to Claude Sonnet 5.5 at low and medium reasoning effort, with the poster asserting that local models are now at the cutting edge. The author adds that they use Qwen-Next 3.8 for complex tasks, citing a case where GPT-Sol-6-High derailed a project and Qwen-Next got it back on track. If open-weight local models can match proprietary frontier models at lower reasoning settings, users gain a capable option they can run privately on their own hardware, avoiding per-token API costs and data-sharing concerns while still adapting the model to their own workflow. This reinforces the trend of the capability gap between local and hosted frontier models shrinking to just a few months. The comparison is a community-made chart with no published methodology, and one commenter notes the 27B model takes more than half an hour to complete a full reasoning turn on dual RTX 3090s. Because each vendor defines its reasoning effort levels differently — Sonnet 5.5&\#x27;s low/medium settings explicitly trade reasoning depth for latency and cost — the effort tiers being compared are not strictly equivalent.

reddit · r/LocalLLaMA · LegacyRemaster · Sep 28, 20:38 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1wsq6r5/qwen_next_38_and_38_27b_vs_sonnet_55_low_and/)

**Background**: Qwen is Alibaba&\#x27;s open-weight model family, and Qwen-Next 3.8 \(Qwen3.8-Flash-Next\) is described as an experimental early preview of the Qwen 4 architecture, while Qwen 3.8-Flash is the production model served in Qwen&\#x27;s API. Sonnet 5.5 is Anthropic&\#x27;s model, which exposes configurable effort levels \(low, medium, high\) that trade reasoning depth for latency and token consumption. Local LLM users typically run quantized versions of such open weights through tools like Ollama or llama.cpp on consumer GPUs, which is why hardware and inference time are recurring concerns in these comparisons.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/models/sonnet-5-5/whats-new-sonnet-5-5">What&#x27;s new in Claude Sonnet 5.5 - Claude Platform Docs</a></li>
<li><a href="https://ollama.com/library/qwen3.8-flash-next:125b-a6b-q4_K_M">qwen 3 . 8 -flash- next :125b-a6b-q4_K_M</a></li>
<li><a href="https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-sonnet-5">Prompting Claude Sonnet 5 - Claude Platform Docs</a></li>

</ul>
</details>

**Discussion**: Sentiment is broadly positive: commenters find it impressive that Qwen 3.8 sits next to Sonnet at lower reasoning settings, and highlight the advantages of private deployment, workflow adaptation, and low cost, with one noting Qwen handles most daily tasks inside a good harness. The main caveat raised is hardware — the 27B model takes over half an hour per full reasoning turn on 2x 3090s — and one commenter questions whether the chart marks QFN at xhigh or low while praising GLM5.3 Flash&\#x27;s showing.

**Tags**: `#local-llms`, `#qwen`, `#benchmark`, `#model-comparison`, `#ai-performance`

---

<a id="item-22"></a>
## [OpenAI retires original GPT-3 models, including Davinci and Babbage](https://i.redd.it/iw7yfs4b77sh1.jpeg) ⭐️ 6.0/10

OpenAI discontinued the original GPT-3 model family today, retiring the legacy API engines such as Davinci, Curie, Babbage and Ada, and pointing users toward current-generation models like GPT-5.6 Terra as replacements. The shutdown ends a roughly six-year run for the model line that first brought large language models to a broad developer audience. GPT-3 was the model that turned large language models into a commercial API product, so its retirement is a symbolic milestone for the entire LLM era and a reminder that hosted models can vanish on a vendor&\#x27;s schedule. It also sharpens the argument for open-weight and locally run models, which have no universal end-of-life date and can serve as a durable historical record. The suggested replacements are not drop-in substitutes: community members point out that Babbage is smaller than the 2B-parameter open-weight MiniCPM5 2B, and that even the lightweight GPT-5.6 Luna tier may be overkill for workloads that once ran on Babbage. Migrating also means dealing with different tokenizers, prompt formats and pricing rather than a simple model-name swap.

reddit · r/LocalLLaMA · charles25565 · Sep 28, 05:39 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1ws67x4/gpt3_is_discontinued_today/)

**Background**: GPT-3 was released by OpenAI in 2020 with 175 billion parameters and was exposed through the API as four engines named Ada, Babbage, Curie and Davinci; EleutherAI later mapped them to roughly 350M, 1.3B, 6.7B and 175B parameters respectively, with Davinci being the most capable and most widely used. OpenAI has since moved through several model generations, and its current lineup is GPT-5.6, split into the Sol, Terra and Luna tiers. Open-weight models such as MiniCPM5 2B are published for download, so anyone can run them locally indefinitely, unlike API-only models that a vendor can switch off.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-3">GPT-3 - Wikipedia</a></li>
<li><a href="https://huggingface.co/openbmb/MiniCPM5-2B">openbmb/ MiniCPM 5 - 2 B · Hugging Face</a></li>
<li><a href="https://www.linkedin.com/posts/deepro713_openai-just-shipped-gpt-56-as-three-named-activity-7478504413364494337-pJbv">GPT - 5 . 6 Tiers: Sol, Terra , Luna for Efficient AI Work | LinkedIn</a></li>

</ul>
</details>

**Discussion**: The top comments are nostalgic but focused on preservation: one highly upvoted user wishes OpenAI would open-source the GPT-3 weights, arguing that even if nobody would run them, it would be hugely valuable for historical preservation. Another is glad that local and open-weight models exist, predicting that the only surviving artifacts of this period for future retrocomputing enthusiasts will be the openly released models.

**Tags**: `#LLM`, `#OpenAI`, `#GPT-3`, `#model-preservation`, `#open-weights`

---

<a id="item-23"></a>
## [Reddit Debates ToMoE v2&\#x27;s Dense-to-MoE Conversion Claims](https://arxiv.org/html/2501.15316v2) ⭐️ 6.0/10

A Reddit thread is evaluating the ToMoE v2 paper \(arXiv 2501.15316v2\), which claims dense large language models can be converted into Mixture-of-Experts models at near-lossless accuracy, with the poster musing that something like a &quot;Qwen3-27B-A16B&quot; would be amazing. Commenters pushed back hard, pointing out that the paper&\#x27;s own benchmarks show severe degradation — MMLU dropping from 67.22 to 36.31. If dense-to-MoE conversion really worked at near-lossless quality, teams could reuse existing dense checkpoints and training data to gain MoE-style inference efficiency without paying for pretraining from scratch. The reported benchmark collapse suggests the technique is far from production-ready, and the thread highlights the recurring gap between paper claims and what practitioners actually observe. ToMoE&\#x27;s approach converts dense models through dynamic pruning, using top-k routing and static pruning along the attention head dimension for MHA layers plus top-1 routing across learned experts for MLP layers. Commenters add two practical caveats: no mainstream inference stack currently supports the resulting architecture, and one argues that if you care about quality the model effectively becomes &quot;27B-A27B&quot; — i.e. all parameters active, so no real speedup.

reddit · r/LocalLLaMA · jinnyjuice · Sep 28, 18:35 · [Discussion](https://www.reddit.com/r/LocalLLaMA/comments/1wsmsnx/what_do_you_think_about_tomoe_v2_paper_converting/)

**Background**: Mixture-of-Experts \(MoE\) is an architecture in which several expert subnetworks sit behind a gating function that routes each token to only a few of them, so total parameter count can be far larger than the number of parameters actually used per token — more capacity at roughly the same compute. Dense-to-MoE conversion tries to take an already-trained dense Transformer and restructure it into this sparse form, rather than pretraining an MoE from scratch, which would save enormous compute and data. ToMoE is one such conversion method, and the v2 paper is the revision under discussion here.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2501.15316v1">ToMoE: Converting Dense Large Language Models to Mixture-of ...</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Sentiment is overwhelmingly skeptical. The top comment asks whether anyone actually read the benchmarks, noting results are &quot;halved&quot; \(MMLU 67.22 → 36.31\); another says that if you care about quality it would really be 27B-A27B; and a third dismisses it on the grounds that no inference software will support it, suggesting &quot;Prox&quot; as a better way to make a dense model sparse.

**Tags**: `#MoE`, `#LLM`, `#model compression`, `#benchmarks`, `#Reddit`

---

<a id="item-24"></a>
## [Forisek–Jancina Deterministic Primality Test for 32-bit Integers Explained](https://leetarxiv.substack.com/p/forisek-and-jancina-primality-test) ⭐️ 6.0/10

A new write-up on the LeetArxiv Substack \(surfaced via a Reddit post\) walks through the Forisek and Jancina deterministic primality test for integers that fit in a machine word, originally published in 2015. The post highlights that testing a 32-bit integer for primality needs only a 512-byte lookup table plus a handful of additions and multiplications, rather than several rounds of Miller-Rabin. Deterministic tests give a guaranteed yes/no answer instead of a probabilistic one, which matters for correctness-critical code such as hash-table sizing, competitive programming, and cryptographic preprocessing. Because the whole test fits in a tiny table and a few arithmetic operations, it is dramatically faster and more cache-friendly than running multiple Miller-Rabin rounds on every candidate. The method also extends to 64-bit integers, which is arguably the more impressive result since a brute-force bitmap for 32-bit inputs would already need about 268 MB \(one bit per odd integer\). The trade-off is that the algorithm relies on a precomputed table of residues tied to the specific bit width, so it is not a general-purpose test for arbitrarily large numbers.

reddit · r/programming · DataBaeBee · Sep 28, 10:11 · [Discussion](https://www.reddit.com/r/programming/comments/1wsaolh/fast_primality_testing_for_32bit_integers_via/)

**Background**: A primality test determines whether a number is prime without necessarily finding its factors, and it is widely used in cryptography and number theory. For very large numbers the fastest practical tests are probabilistic, such as Miller-Rabin, which can only say a number is &\#x27;probably prime&\#x27; with a small error probability. For numbers of a fixed small size, however, deterministic tests win in practice, and the standard approach has been to run several fixed Miller-Rabin rounds whose bases are known to be sufficient for that bit width.

<details><summary>References</summary>
<ul>
<li><a href="https://leetarxiv.substack.com/p/forisek-and-jancina-primality-test">Forisek and Jancina Primality Test - by Murage Kibicho</a></li>
<li><a href="https://ceur-ws.org/Vol-1326/020-Forisek.pdf">Fast Primality Testing for Integers That Fit into a Machine Word</a></li>
<li><a href="https://www.jeremykun.com/2026/04/07/deterministic-miller-rabin/">Deterministic Primality Testing for Limited Bit Width</a></li>

</ul>
</details>

**Discussion**: Discussion is brief and mostly appreciative: one commenter stresses that Forisek &amp; Jancina is deterministic rather than probabilistic, is very fast, and is easy to code with just a 512-byte table for 32-bit inputs. Another jokes that the sample code looks &\#x27;code golfed&\#x27;, while a third points out that the 64-bit support is the more impressive part, since 32-bit primality could in principle be handled by a 268 MB bitmap of one bit per odd integer.

**Tags**: `#primality-testing`, `#algorithms`, `#number-theory`, `#performance-optimization`, `#programming`

---

<a id="item-25"></a>
## [Tesla&\#x27;s New Model Y Drops Standard Autosteer, Undercutting Base Corolla&\#x27;s Driver Assist](https://carbuzz.com/tesla-new-model-y-has-less-driver-assist-than-a-base-corolla/) ⭐️ 6.0/10

Tesla&\#x27;s refreshed Model Y no longer includes Autosteer as standard equipment, meaning lane-centered cruise control now requires the paid Full Self-Driving \(FSD\) subscription at roughly $99 per month. The change means a base Toyota Corolla, which ships with adaptive cruise control and lane tracing as standard, offers more no-cost driver assistance than Tesla&\#x27;s volume-selling SUV. The move turns a feature Tesla once framed as a free safety benefit into a recurring revenue stream, and it raises questions about whether Tesla is monetizing basic driver assistance that competitors give away. It affects every new Model Y buyer and could shape how regulators and rivals treat lane-centering and adaptive cruise as baseline safety equipment rather than premium add-ons. Autosteer is the lane-centering component of Tesla&\#x27;s Autopilot stack and always operates together with Traffic-Aware Cruise Control, so removing it leaves only basic cruise control without lane holding. Tesla&\#x27;s FSD \(Supervised\) subscription has been reported at $99 per month for some owners and up to $199 per month in other cases, making it the sole path to lane-centered highway driving on new vehicles.

reddit · r/electricvehicles · DonkeyFuel · Sep 28, 14:01 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1wsfg9o/teslas_new_model_y_now_ships_with_less_standard/)

**Background**: Tesla&\#x27;s Autopilot suite has historically bundled two pieces: Traffic-Aware Cruise Control, which matches the speed of the car ahead like adaptive cruise control, and Autosteer, which keeps the vehicle centered in its lane. Lane centering combined with adaptive cruise control is what most automakers — including Toyota, whose Safety Sense suite is standard even on base Corollas — offer as a mainstream highway-assist feature. Tesla&\#x27;s FSD is a more advanced, supervised system that handles city streets and highway driving, and it has been sold both as a one-time purchase and as a monthly subscription.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tesla.com/en_ae/support/autopilot">Autopilot and Full Self-Driving Capability | Tesla Support UAE</a></li>
<li><a href="https://www.tesla.com/fsd">Full Self - Driving (Supervised) | Tesla</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lane_centering">Lane centering - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were overwhelmingly critical, calling the removal of Autosteer from all vehicles a &quot;scummy&quot; move that forces owners into the $99/month FSD subscription just to get lane-centered cruise control. Several users highlighted the reversal from Elon Musk&\#x27;s earlier promise that Autopilot would be standard on every Tesla because it is a safety feature, with one commenter sarcastically tying the change to Tesla&\#x27;s stock price.

**Tags**: `#Tesla`, `#Autonomous Driving`, `#Driver Assist`, `#EV Industry`, `#Product Strategy`

---

<a id="item-26"></a>
## [EVs Outsell Gasoline and Diesel Cars in Europe for the First Time](https://www.chosun.com/english/industry-en/2026/09/28/5IAPF6QFBBDWLCE5UHYJNUTGNQ/) ⭐️ 6.0/10

Electric vehicles have outsold gasoline and diesel cars in Europe for the first time, according to a report covered by Chosun. This marks a notable adoption milestone for battery-powered cars in a market long dominated by internal combustion engines. Crossing this threshold signals that EVs have moved from a niche segment into the mainstream of Europe&\#x27;s largest consumer vehicle market, which affects automakers&\#x27; product planning, charging infrastructure investment, and long-term oil demand. It also strengthens the political case for the EU&\#x27;s tightening CO2 rules on new cars. The news item itself is brief and does not provide the underlying sales figures, the reporting period, or a breakdown by country, so it is unclear whether EVs outsold gasoline and diesel cars combined or each fuel type separately. How hybrids and plug-in hybrids are classified also materially changes how such a milestone is counted.

reddit · r/electricvehicles · mariasunflower · Sep 28, 10:30 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1wsb08g/electric_vehicles_outsell_gasoline_diesel_cars_in/)

**Background**: Europe has for years been one of the fastest-adopting regions for electric cars, helped by EU fleet-wide CO2 emission standards that penalize automakers for selling high-emitting vehicles, plus national purchase incentives and an expanding charging network. The EU has also legislated that new cars sold from 2035 must have zero tailpipe CO2 emissions, effectively ending sales of new gasoline and diesel cars. In this context, hybrids — including plug-in hybrids \(PHEVs\), which can drive a limited distance on battery power alone — have been treated by some regulators and buyers as a transitional technology toward fully electric cars.

**Discussion**: Commenters largely argued over how hybrids should be classified rather than the milestone itself: the top-voted comment insisted that non-plug-in hybrids burn 100% fossil fuel and are therefore combustion-engine cars by definition, while others countered that hybrids are a useful bridge to full electrification and mocked the idea that they run on anything but fuel.

**Tags**: `#Electric Vehicles`, `#Europe`, `#Automotive Industry`, `#Climate Tech`, `#Reddit`

---

<a id="item-27"></a>
## [CATL LFP Cells Retain 85% Health After 14 Years of Hard Use](https://insideevs.com/news/809604/catl-lfp-prismatic-cell-age-test/) ⭐️ 6.0/10

A long-term aging test of CATL lithium iron phosphate \(LFP\) prismatic battery cells found they retained roughly 85% state of health \(SOH\) after 14 years of hard, daily use. The results suggest these cells could keep working for another decade before dropping below typical end-of-life thresholds. Battery longevity is a core economic variable for electric vehicles and grid-scale energy storage: if LFP packs hold most of their capacity for well over a decade, total cost of ownership falls and second-life reuse in stationary storage becomes far more attractive. It also reinforces LFP&\#x27;s position as the chemistry of choice for cost-sensitive, cycle-heavy applications where cobalt- and nickel-based cells are harder to justify. The test involved sustained daily charge/discharge cycling at meaningful C-rates, so the 85% figure reflects genuinely hard duty rather than gentle laboratory conditions. State of health is defined as the ratio of a battery&\#x27;s current maximum capacity to its original rated capacity, so 85% SOH means roughly 15% capacity fade over 14 years — though results will vary with temperature, charge rate, depth of discharge and cell-to-cell manufacturing spread.

reddit · r/electricvehicles · DonkeyFuel · Sep 28, 21:28 · [Discussion](https://www.reddit.com/r/electricvehicles/comments/1wsriqe/these_battery_cells_were_tested_after_14_years_of/)

**Background**: LFP stands for lithium iron phosphate \(LiFePO4\), a polyanion cathode chemistry that trades some energy density for considerably longer cycle life and better thermal stability than many other lithium-ion chemistries, and it uses no cobalt or nickel. Prismatic cells are rectangular, usually aluminium-cased units whose internal electrode sheets are either stacked or wound and flattened, which allows them to be packed efficiently into modules and packs. State of health \(SOH\) is the standard figure of merit comparing an aged battery&\#x27;s current maximum capacity with its ideal, as-new condition.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Lithium_iron_phosphate_battery">Lithium iron phosphate battery - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/State_of_health">State of health - Wikipedia</a></li>
<li><a href="https://www.laserax.com/blog/prismatic-vs-cylindrical-cells">Prismatic Cells vs. Cylindrical Cells: What is the Difference? | Laserax</a></li>

</ul>
</details>

**Discussion**: Discussion was sparse but positive: the single substantive commenter called the result &quot;incredible,&quot; noting that the C-rate and daily charge/discharge throughput matter a great deal, yet 85% SOH after 14 years is still impressive.

**Tags**: `#batteries`, `#LFP`, `#electric vehicles`, `#energy storage`, `#battery longevity`

---