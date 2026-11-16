---
layout: default
title: "Horizon Summary: 2026-11-16 (EN)"
date: 2026-11-16
lang: en
---

> From 64 items, 35 important content pieces were selected

---

1. [Microsoft 365 outage blamed for chlorine gas injuries at German hotel pool](#item-1) ⭐️ 8.0/10
2. [Blog post argues all AI-generated code should be open source, sparking HN debate](#item-2) ⭐️ 8.0/10
3. [Meta FAIR/NYU: 200+ MLLMs show vision needs own parameters, not pretraining](#item-3) ⭐️ 8.0/10
4. [Multiplayer CS:GO world model beta renders each player&\#x27;s view on their own GPU](#item-4) ⭐️ 8.0/10
5. [Higurashi AI Releases Haru-4B, a Full-Duplex Spoken Dialogue Model](#item-5) ⭐️ 8.0/10
6. [544 unmaintained PyPI packages break on Python 3.12+ yet still get 100M+ monthly downloads](#item-6) ⭐️ 8.0/10
7. [Old Bitly Links Are Being Hijacked](#item-7) ⭐️ 7.0/10
8. [Protomaps Shows Self-Hosting Map Tiles Is Now Cheap and Easy](#item-8) ⭐️ 7.0/10
9. [MacBook Pro OLED PWM Flicker Sparks Accessibility Debate](#item-9) ⭐️ 7.0/10
10. [Raschka Explains Positional Embeddings in Modern LLMs](#item-10) ⭐️ 7.0/10
11. [Open-source tuner makes pageable cudaMemcpy 5x faster on NVIDIA B300](#item-11) ⭐️ 7.0/10
12. [Training-free early exit for reasoning models by editing one output-layer weight row](#item-12) ⭐️ 7.0/10
13. [Marimba: an open-weight &\#x27;System One&\#x27; speech model built on frozen Qwen3-ASR-0.6B](#item-13) ⭐️ 7.0/10
14. [Reddit user voltage-glitches CMP 170HX mining card to unlock 80GB VRAM and 126 SMs](#item-14) ⭐️ 7.0/10
15. [inside-llm: Open-Source Tool Visualizes LLM Token Probabilities and Quantization Divergence](#item-15) ⭐️ 7.0/10
16. [audio.cpp 0.9.5 Demo Chains Three Models Into Fully Local Real-Time Avatar Chat](#item-16) ⭐️ 7.0/10
17. [Paper Claims First Recursive Self-Improvement of a Full Frontier Pre-Training Run](#item-17) ⭐️ 7.0/10
18. [Report: Export-Banned Nvidia Chips Power China’s Top AI Models](#item-18) ⭐️ 7.0/10
19. [Meituan open-sources LongCat-2.5, a 1.6T agent model documented only for Huawei NPUs](#item-19) ⭐️ 7.0/10
20. [Anthropic rebuilds Claude Code Projects around a coordinator and parallel cloud threads](#item-20) ⭐️ 7.0/10
21. [&\#x27;Birdbrain&\#x27; Is a Misnomer: Crows Decide Faster Than Humans](#item-21) ⭐️ 6.0/10
22. [Retrospective: Turbo Pascal&\#x27;s Tiny Footprint vs. Modern Software Bloat](#item-22) ⭐️ 6.0/10
23. [Emacs Is My Browser: One Developer&\#x27;s EWW-Only Web Experience](#item-23) ⭐️ 6.0/10
24. [Apollo&\#x27;s &\#x27;Grenade Launcher&\#x27; Was a Mortar for Lunar Seismic Experiments](#item-24) ⭐️ 6.0/10
25. [COMAC CE-25A: China&\#x27;s 19-seat electric airliner flies with crew for the first time](#item-25) ⭐️ 6.0/10
26. [Parallax matches Wikipedia sentences across seven editions at any past date](#item-26) ⭐️ 6.0/10
27. [Basalt 0.4.0 adds router support and its first dense model, Qwen 27B NVFP4](#item-27) ⭐️ 6.0/10
28. [EU&\#x27;s open AI model EUROPA reportedly targets nearly 1 trillion parameters](#item-28) ⭐️ 6.0/10
29. [llama.cpp catches up to custom inference engines on consumer GPUs](#item-29) ⭐️ 6.0/10
30. [BigMoeOnEdge runs any MoE GGUF on 8-16 GB devices, beats Strata and colibri](#item-30) ⭐️ 6.0/10
31. [Axiomic Labs releases X3Guard-150M, a tiny prompt-guard model for edge devices](#item-31) ⭐️ 6.0/10
32. [Slack&\#x27;s cellular architecture migration isolates failures to a fraction of users](#item-32) ⭐️ 6.0/10
33. [Survey examines memory management across 40 major C projects](#item-33) ⭐️ 6.0/10
34. [Deep Dive Explains How Profile-Guided Optimization Works Inside the Go Toolchain](#item-34) ⭐️ 6.0/10
35. [Reddit Test Finds ChatGPT and Google AI Mode Invented Nothing Across 18 Fake-Brand Queries](#item-35) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Microsoft 365 outage blamed for chlorine gas injuries at German hotel pool](https://www1.wdr.de/nrw/rheinland/rhein-erft-kreis/technischer-defekt-chlor-phantasialand-100.html) ⭐️ 8.0/10

Fifteen guests at a Phantasialand hotel in Brühl, Germany, were injured by chlorine gas after the automatic pool-dosing system pumped too much chlorine into the water and the safety alert about the fault was never delivered, because it was sent as an email during a Microsoft 365 outage, the operator told WDR. The hotel said no one was aware that the sauna area&\#x27;s maintenance safety system had already raised the alarm, since no emails arrived during the disruption. The incident is a concrete case of a cloud dependency reaching into the physical-safety path: an IT messaging outage, not a pool-equipment failure, is what kept a known fault from being acted on. It raises uncomfortable questions for any operator of building automation, industrial IoT or other OT systems that route alarms through third-party SaaS instead of local, self-contained annunciation. According to the reporting summarized by commenters, the automatic dosing system over-chlorinated the pool, the sauna area&\#x27;s maintenance safety system raised an alert by email, and the Microsoft 365 outage meant that email was never received — there was apparently no independent local alarm or secondary notification channel. Community experts also note that chlorine dosing loops typically fail toward over-dispensing, because a fouled or dead sensor reads low or zero chlorine and the controller keeps adding more.

hackernews · DeepLogin · Nov 15, 18:36 · [Discussion](https://news.ycombinator.com/item?id=50509411)

**Background**: Automatic pool chlorinators form a closed control loop: sensors continuously measure parameters such as pH and free chlorine \(often via ORP\), a central controller interprets the readings, and dosing pumps or actuators add chemicals to hit a target. That design depends entirely on sensor trust — if the probe drifts or dies, the loop happily &\#x27;corrects&\#x27; a phantom deficit. Safety engineers treat such systems as safety-critical and rely on layered, independent barriers \(the Swiss cheese model\), precisely so that a single failed barrier — a bad sensor, or an undelivered email — cannot escalate into a real accident.

<details><summary>References</summary>
<ul>
<li><a href="https://www.swimuniversity.com/pool-chlorinator/">Automatic Pool Chlorinators: How Do They Work and Are They ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Safety-critical_system">Safety - critical system - Wikipedia</a></li>
<li><a href="https://www.isec7-gs.com/post/when-clouds-go-dark-lessons-from-the-recent-global-outages-and-how-to-build-true-resilience">When Clouds Go Dark: Lessons from the Recent Global Outages, and...</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread \(333 points, 162 comments\) broadly agreed the architecture, not the outage, is the real culprit: one commenter who operates closed-loop chlorination systems called the setup &\#x27;beyond screwed up,&\#x27; explaining that such loops fail toward over-dispensing and that a human or an independent sensor design must always be the backstop. Others split on fault attribution — some said it was &\#x27;100% fault of the hotel&\#x27; for relying on email with no backup, while an Azure engineer noted the story flirts with libel and stressed that anything capable of causing harm needs redundant, resilient design.

**Tags**: `#cloud-reliability`, `#safety-critical-systems`, `#outage-postmortem`, `#software-engineering`, `#iot-industrial-control`

---

<a id="item-2"></a>
## [Blog post argues all AI-generated code should be open source, sparking HN debate](https://jakub.jankiewicz.org/blog/ai-code-open-source/) ⭐️ 8.0/10

A blog post by Jakub Jankiewicz arguing that all AI-generated code should be open source hit the front page of Hacker News, collecting 1,053 points and 573 comments. The post treats the issue as a policy and ethics question about ownership of machine-produced code rather than a technical argument about tooling. The argument lands in the middle of genuine legal uncertainty: US courts and the Copyright Office have signaled that works without human authorship may not be copyrightable at all, which in turn determines whether AI-assisted code can even be placed under an open source license. Since most professional developers now use AI assistants daily, the answer affects who owns — and who can enforce rights over — a growing share of the world&\#x27;s software. The US Copyright Office&\#x27;s AI guidance holds that copyrightability questions can be resolved under existing law without new legislation, and that using AI to assist rather than stand in for human creativity does not by itself void protection — meaning the outcome hinges on how much human contribution exists in each case. Commenters also noted the flip side: because open source licenses like the GPL operate through copyright, code that fails the human-authorship test may be impossible to license or enforce as open source at all.

hackernews · jcubic · Nov 15, 14:46 · [Discussion](https://news.ycombinator.com/item?id=50507303)

**Background**: Copyright protects original works fixed by human authors, and open source licenses are built on top of that: a license like the GPL is a permission granted by a copyright holder, so it only has force if someone actually holds the copyright. Large language models are trained on vast amounts of public and open source code and can reproduce recognizable fragments of it, which is why authors of permissively and copyleft-licensed projects have become vocal about AI output. The Hacker News thread reflects a wider industry conversation about whether AI coding assistants are analogous to compilers and IDEs — neutral tools — or something that genuinely muddies provenance and ownership.

<details><summary>References</summary>
<ul>
<li><a href="https://www.logiclooptech.dev/why-ai-generated-code-cannot-be-copyrighted-and-what-to-do/">AI-Generated Code Copyright: What Developers Need to Know</a></li>
<li><a href="https://allthingsopen.org/articles/copyright-problem-ai-generated-code-open-source-licenses">The copyright problem with AI-generated code | We Love Open ...</a></li>
<li><a href="https://www.recordinglaw.com/us-laws/ai-copyright-laws/ai-generated-code-copyright-infringement/">Is AI-Generated Code Copyright Infringement? (2026)</a></li>

</ul>
</details>

**Discussion**: Sentiment was largely skeptical of the post&\#x27;s premise. One commenter pointed to US Copyright Office guidance showing most people misunderstand the existing rules, another argued the logic would absurdly force any code built on open source frameworks or Stack Overflow answers to be open source too, and a third described AI as simply a tool like a compiler while noting the tension of having trained on open source code. The most concrete counterpoint came from an AGPL maintainer who said a company that had pirated his code later used an LLM to clone the system, producing a buggy but legally awkward replacement.

**Tags**: `#AI-generated code`, `#open source`, `#copyright`, `#intellectual property`, `#software engineering`

---

<a id="item-3"></a>
## [Meta FAIR/NYU: 200+ MLLMs show vision needs own parameters, not pretraining](https://www.reddit.com/r/MachineLearning/comments/1xx1k2o/meta_fair_nyu_unbundling_multimodal_vision/) ⭐️ 8.0/10

Meta FAIR and NYU trained over 200 multimodal LLMs from scratch under matched lifetime compute to separately ablate separate encoder pretraining, vision-only parameters, and placing the encoder before the LLM. They find that separate encoder pretraining is optional, vision-only parameters are required, and encoder placement before the LLM is also optional when using their in-fusion approach. This large-scale controlled study directly addresses a live disagreement in multimodal model design, where labs are split on dropping encoders, training them from scratch, or bringing them back. It gives MLLM builders evidence for architecture and compute allocation decisions, including whether separate encoder pretraining is worth its cost and whether vision needs dedicated capacity. The experiments span 0.6B to 6.4B backbone sizes, with main comparisons using Qwen3-1.7B and 4B configurations plus 0.4B parameters of vision capacity, evaluated on 16 Cambrian VQA benchmarks at 448 px and 12 language benchmarks. Encoders pretrained with four objectives at best tie an encoder trained from scratch with the LLM at matched compute, and even pretraining MetaCLIP 6.5x longer raised ImageNet linear-probe accuracy from 80.4% to 84.4% without improving VQA; encoder-free models trail at every size and need about 3x compute to catch up, while in-fusion adds zero-initialized vision-only weights to the LLM&\#x27;s first 8 layers and is on par with an encoder from 1.7B to 6.4B with about 13% lower time to first token.

reddit · r/MachineLearning · /u/trungh98 · Nov 15, 17:38

**Background**: A multimodal LLM typically couples a vision encoder—often a ViT or CLIP-style model pretrained on image-text pairs—with a language model, using the encoder to turn images into tokens or embeddings the LLM can consume. The conventional recipe bundles three choices: pretraining that encoder separately, allocating parameters used only by visual tokens, and placing the encoder before the LLM. Because published models differ in data, compute, and how much encoder pretraining they count, it has been hard to tell which of these choices actually matters; this study isolates them under matched budgets.

<details><summary>References</summary>
<ul>
<li><a href="https://ammarab.medium.com/wtf-s-an-image-encoder-7559f40f9df0">What Is an Image Encoder in Multimodal LLMs | Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vision-language_model">Vision-language model - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#multimodal LLMs`, `#vision encoders`, `#pretraining`, `#model scaling`, `#machine learning research`

---

<a id="item-4"></a>
## [Multiplayer CS:GO world model beta renders each player&\#x27;s view on their own GPU](https://www.reddit.com/r/MachineLearning/comments/1xx4ta3/we_made_a_multiplayer_game_where_each_players/) ⭐️ 8.0/10

A team trained a diffusion-transformer world model on roughly 3,958 hours of 10-player CS:GO bot matches — an open dataset they released last month with all player POVs and inputs aligned at 16 Hz — and has now shipped a free, open multiplayer beta built on it. In the beta, a lightweight server keeps the shared game state synchronized while each player&\#x27;s own GPU generates that player&\#x27;s view from the server state, their inputs, and previous frames. It demonstrates a concrete architecture for multiplayer neural world models: keep a single authoritative shared state on the server and push expensive view synthesis out to each client, which avoids the redundant compute and view inconsistency that plague naive video-model approaches. The open dataset plus playable beta give researchers and hobbyists a practical testbed for real-time generative game rendering, a direction of growing interest to both game AI and world-model research. The build is explicitly limited — a single small map, pistols only, and visibly imperfect fine detail — and it demands an RTX 3080 or better, though an experimental Mac build exists; the project is also not affiliated with Valve. Because rendering is local, visual quality and frame rate depend on each player&\#x27;s hardware rather than on a shared server.

reddit · r/MachineLearning · /u/bengal7ion · Nov 15, 19:46

**Background**: A &quot;world model&quot; here means a generative model that, given the current game state and the player&\#x27;s actions, predicts the next frame of video instead of using a conventional 3D engine to rasterize polygons, textures, and lighting. Diffusion transformers \(DiTs\) are the backbone of choice: they replace the U-Net used in earlier image diffusion models with a transformer, which scales better and captures global scene structure, and they generate each frame by iteratively denoising from noise. Multiplayer games normally rely on an authoritative server that broadcasts state and lets each client render only its own camera view; this project borrows that same client-server split but substitutes the renderer with a per-player diffusion model.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2608.06257">[2608.06257] MASS: Multiplayer World Models with ...</a></li>
<li><a href="https://arxiv.org/html/2411.12164v2">Diffusion Transformers as Open-World Spatiotemporal ...</a></li>
<li><a href="https://backbonetutorials.com/interactive-web/multiplayer-state-synchronization/">Multiplayer State Synchronization — shared world</a></li>

</ul>
</details>

**Tags**: `#world models`, `#diffusion transformers`, `#multiplayer games`, `#real-time rendering`, `#game AI`

---

<a id="item-5"></a>
## [Higurashi AI Releases Haru-4B, a Full-Duplex Spoken Dialogue Model](https://www.reddit.com/r/LocalLLaMA/comments/1xww5o2/higurashiaiharu4b_hugging_face/) ⭐️ 8.0/10

Higurashi AI published Haru-4B, a 4B-parameter pretrained base model that performs native full-duplex spoken dialogue: every 133 ms \(7.5 Hz\) it consumes one frame of user audio and emits one frame of its own audio plus text, so listening and speaking happen simultaneously. The model ships with code, an English technical blog and a Japanese technical blog, and is released for research use. Almost all deployed voice assistants still run on turn-taking pipelines that must wait for the user to stop talking, which produces awkward latency and blocks natural backchannels like &quot;mm-hmm&quot; or interruptions. A native full-duplex, multilingual open base model pushes speech-LLM research toward human-like phone-call interaction and gives academic groups a starting point they can fine-tune without training such a model from scratch. Audio is represented as a 64-dimensional continuous latent per frame, generated in a single sampling step by a small MLP head using MeanFlow sampling from the language model&\#x27;s hidden state, with no separate audio transformer and no discrete audio tokens. The three streams — user audio, model audio and model text — are combined by element-wise addition into a single position of the shared language model; the model supports English, Spanish, Portuguese, German, French, Chinese, Japanese, Russian and Korean, with a text card setting the character and a short reference clip setting the voice, and it is explicitly a pretrained base model rather than a finished product.

reddit · r/LocalLLaMA · /u/pmttyji · Nov 15, 13:58

**Background**: Most voice AI systems are turn-based: speech recognition transcribes the user, a language model replies, and a text-to-speech model speaks, with each stage waiting on the previous one. Full-duplex modeling instead lets a model process input and produce output at the same time on a fixed frame clock, much like a human on a phone call. The other key design choice is audio representation — many speech models quantize audio into discrete tokens like text, whereas Haru keeps a continuous latent and uses MeanFlow, a flow-matching technique that learns an average velocity field so a latent can be produced in one network evaluation rather than many denoising steps.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.higurashi.ai/melte/haru4b/">Haru-4B: A Low- Latency and Multilingual Full - Duplex Continuous ...</a></li>
<li><a href="https://github.com/higurashi-ai/Haru">higurashi-ai/Haru: Haru: a low- latency , multilingual, full - duplex ...</a></li>
<li><a href="https://arxiv.org/abs/2508.06098">[2508.06098] MeanAudio: Fast and Faithful Text-to-Audio ... MeanAudio: Fast and Faithful Text-to-Audio Generation with ... MeanFlow for One-Step Streaming Text-to-Speech | OpenReview dots.tts: continuous acoustic latents, flow matching and 48 ... MeanAudio: Fast and Faithful Text-to-Audio Generation with ... MeanAudio/README.md at main · Lanternko/MeanAudio · GitHub</a></li>

</ul>
</details>

**Tags**: `#speech-dialogue`, `#full-duplex`, `#multimodal-llm`, `#audio-model`, `#multilingual`

---

<a id="item-6"></a>
## [544 unmaintained PyPI packages break on Python 3.12+ yet still get 100M+ monthly downloads](https://www.reddit.com/r/programming/comments/1xwyhpm/544_unmaintained_pypi_packages_with_imports_that/) ⭐️ 8.0/10

A scan of PyPI found 1,623 projects that still import one of the 25 standard-library modules removed in Python 3.12 and 3.13 — including distutils, imp, cgi, pipes and telnetlib — without wrapping the import in a try/except. Of those, 852 sit among the 60,000 most-downloaded packages, and 544 of that 852 have not published a release in two years while collectively pulling more than 100 million downloads per month. This quantifies a supply-chain risk that will silently surface as ImportError at runtime for anyone upgrading to Python 3.12, 3.13 or 3.14, and the concentration in unmaintained packages means the usual &quot;just upgrade the dependency&quot; fix is often unavailable. Teams setting dependency policies or planning interpreter migrations now have concrete numbers to justify audits of their transitive dependency trees. The scan only covered releases from the past year plus the top 60,000 packages by download count, so the true number of affected projects is higher than 1,623, and the import check only flags unconditional imports, meaning code that already guards the import with a try/except fallback is not counted. Download figures come from ClickHouse&\#x27;s public ClickPy dataset rather than PyPI&\#x27;s own counters.

reddit · r/programming · /u/Business-Feedback635 · Nov 15, 15:37

**Background**: Python historically shipped a large collection of modules in its standard library, the so-called &quot;batteries included&quot; philosophy. Two PEPs unwound much of that: PEP 632 deprecated distutils in Python 3.10 and removed it in 3.12, recommending setuptools \(which vendors its own copy of distutils\) as the replacement, while PEP 594 removed 19 &quot;dead batteries&quot; such as cgi, telnetlib, nntplib, pipes and imghdr; Python 3.13 also dropped the long-deprecated imp module in favor of importlib. ClickPy is a public, daily-updated ClickHouse-backed dataset covering roughly 1.09 million PyPI packages and over 3.66 trillion recorded downloads, which makes ecosystem-wide download analysis possible without scraping PyPI.

<details><summary>References</summary>
<ul>
<li><a href="https://peps.python.org/pep-0632/">PEP 632 – Deprecate distutils module | peps.python.org</a></li>
<li><a href="https://peps.python.org/pep-0594/">PEP 594 – Removing dead batteries from the... | peps . python .org</a></li>
<li><a href="https://clickpy.clickhouse.com/">PyPI downloads stats - ClickPy</a></li>

</ul>
</details>

**Tags**: `#python`, `#pypi`, `#dependency-management`, `#software-supply-chain`, `#stdlib-deprecation`

---

<a id="item-7"></a>
## [Old Bitly Links Are Being Hijacked](https://ransomnews.com/burger-king-tweet-bitly-link-hijack-2026/) ⭐️ 7.0/10

Old, abandoned Bitly short links — including one from a Burger King tweet — are being re-registered by third parties and redirected to new destinations, illustrating the long-term fragility and security risks of URL shorteners.

hackernews · hspeiser · Nov 15, 22:11 · [Discussion](https://news.ycombinator.com/item?id=50511395)

**Tags**: `#url-shorteners`, `#security`, `#link-rot`, `#web-infrastructure`, `#hijacking`

---

<a id="item-8"></a>
## [Protomaps Shows Self-Hosting Map Tiles Is Now Cheap and Easy](https://bruceroettgers.eu/blog/protomaps/) ⭐️ 7.0/10

A blog post on bruceroettgers.eu walks through how self-hosting map tiles has become cheap and easy by combining the PMTiles single-file archive format with commodity object storage, using the Protomaps basemap as the ready-made dataset. The write-up sparked a Hacker News discussion in which developers shared alternative projects and real production deployments. It lowers the barrier for teams that need privacy, access control, or predictable costs: instead of paying per-request map API bills or running a tile server, a static file on S3 or Cloudflare R2 can serve the whole world. This matters for engineers building location features into apps, who now have a credible escape hatch from commercial map providers. PMTiles packs an entire tile pyramid into one archive that clients read with HTTP range requests, so hosting requires nothing more than static object storage plus a CDN. The main caveat is scale: while vector basemaps stay small, high-resolution satellite imagery grows explosively with zoom level, with global high-res coverage reaching hundreds of terabytes.

hackernews · bcye · Nov 15, 19:26 · [Discussion](https://news.ycombinator.com/item?id=50509837)

**Background**: Traditional web maps are served as individual tiles, which historically required running and scaling a dedicated tile server. PMTiles is a single-file archive format for tiled data — conceptually similar to a ZIP file that contains many tiles — designed so that a client can fetch only the byte ranges it needs from ordinary cloud storage. Protomaps builds a cartographic basemap in PMTiles format from OpenStreetMap and other data sources, along with MapLibre styles for rendering it in the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://protomaps.com/">Protomaps - The open source map in a file</a></li>
<li><a href="https://docs.protomaps.com/pmtiles/">PMTiles Concepts | Protomaps Docs</a></li>
<li><a href="https://github.com/protomaps/basemaps">GitHub - protomaps /basemaps: Basemap PMTiles generation and...</a></li>

</ul>
</details>

**Discussion**: Commenters were broadly enthusiastic: one developer said they switched to Protomaps after an unexpectedly large Google Maps bill and now find it dirt cheap and easy to theme, while another reported running self-hosted Protomaps in production on geocode.xyz but wanting more customization options. Others pointed to the similar OpenFreeMap project, described running tiles behind Cloudflare R2 for privacy and access control, and raised the grounded caveat that high-resolution satellite mosaics get expensive fast — one builder stopped at zoom level 17 due to projected storage needs.

**Tags**: `#maps`, `#self-hosting`, `#pmtiles`, `#geospatial`, `#cloud-storage`

---

<a id="item-9"></a>
## [MacBook Pro OLED PWM Flicker Sparks Accessibility Debate](https://macanorak.com/the-macbook-pros-oled-pwm-problem-when-a-better-display-becomes-worse-to-use/) ⭐️ 7.0/10

An investigation published on MacAnorak argues that the new MacBook Pro&\#x27;s OLED display uses PWM \(pulse-width modulation\) dimming whose flicker can trigger headaches, nausea, and eye strain in photosensitive users, even though the panel is otherwise a clear upgrade over the previous mini-LED screen. The piece set off a 222-comment technical debate in which readers disputed the measured flicker rate and shared first-hand accounts of flicker-induced illness. Apple&\#x27;s flagship laptop switching to OLED affects a very large base of professional and creative users, and for the minority with flicker sensitivity it can turn a technically superior display into one that is physically unusable for long work sessions. The story also captures a broader tension as the industry moves from LCD to OLED across phones, laptops, and monitors, where ergonomics and accessibility often lag behind contrast-ratio and color-gamut marketing. The article&\#x27;s 240Hz flicker figure was directly challenged by commenters, one of whom argues that the tandem OLED structure drives both layers at 480Hz and 180 degrees out of phase, producing an effective 960Hz across most of the usable brightness range. Frequency is also not the whole story: display ergonomics research treats modulation depth — the ratio between peak luminance and the dark trough of each cycle — as equally important for comfort.

hackernews · MacAnorak · Nov 15, 13:15 · [Discussion](https://news.ycombinator.com/item?id=50506719)

**Background**: PWM dimming adjusts a display&\#x27;s apparent brightness by rapidly switching pixels on and off rather than reducing the actual light output, which is known as DC dimming. OLED panels commonly rely on PWM because it is cheap to implement and preserves color accuracy at low brightness levels, where OLED color shift is otherwise pronounced. At frequencies of a few hundred hertz, some people consciously perceive the flicker while others experience eye strain, headaches, or nausea without ever seeing it, which makes the problem easy to dismiss and hard to quantify.

<details><summary>References</summary>
<ul>
<li><a href="https://www.oled-info.com/pulse-width-modulation-pwm-oled-displays">Pulse-width modulation (PWM) in OLED displays - OLED-Info</a></li>
<li><a href="https://www.notebookcheck.net/Why-Pulse-Width-Modulation-PWM-is-such-a-headache.270240.0.html">Why Pulse-Width Modulation (PWM) is such a headache</a></li>
<li><a href="https://screensensitive.com/2026/06/what-is-pwm-flicker-and-is-it-making-you-sick/">What Is PWM Flicker — And Is It Making You Sick? - Screen ...</a></li>

</ul>
</details>

**Discussion**: Sentiment in the thread was largely sympathetic, with readers corroborating the article through lived experience — one describes a family member for whom even the strobing of a ceiling fan&\#x27;s reflected light is enough to cause severe nausea and a painful headache. Others attacked the measurement itself, arguing the tandem OLED runs at 480Hz out of phase for an effective 960Hz, while the discussion widened to related sensitivities such as low CRI on white LEDs and LCD motion blur on displays like the Nintendo Switch 2.

**Tags**: `#OLED displays`, `#PWM flicker`, `#Apple hardware`, `#display ergonomics`, `#health and accessibility`

---

<a id="item-10"></a>
## [Raschka Explains Positional Embeddings in Modern LLMs](https://magazine.sebastianraschka.com/p/understanding-positional-embeddings) ⭐️ 7.0/10

Sebastian Raschka published a technical deep-dive in his magazine explaining how LLMs encode token position information, covering absolute \(learnable and sinusoidal\), relative, and rotary positional embeddings \(RoPE\), along with which methods recent open-weight LLMs actually use. The article is paired with a Hacker News discussion \(191 points, 26 comments\) in which commenters pushed the topic beyond implementation into the underlying mathematics. Positional information is what lets transformer self-attention respect word order at all, so the shift from classic sinusoidal/learnable embeddings to RoPE is one of the quiet but consequential design changes behind modern long-context models. A clear explainer from a well-known educator lowers the barrier for engineers trying to reason about context-length extrapolation and attention behavior. The article walks through the concrete mechanics of each scheme, including how RoPE applies position-dependent rotation matrices to query and key vectors so that attention scores depend on relative offsets. The discussion also touches on practical trade-offs such as how well different schemes behave when predictions exceed the training sequence length.

hackernews · vismit2000 · Nov 15, 12:14 · [Discussion](https://news.ycombinator.com/item?id=50506376)

**Background**: Transformers process all tokens in a sequence in parallel, and self-attention by itself has no notion of order — a bag of words and a sentence look identical to it. Positional embeddings solve this by injecting position information into token representations, either by adding a position-dependent vector \(absolute\), by modifying attention scores with relative distances \(relative\), or by rotating query/key vectors \(RoPE, used in Llama-style models\). Group theory offers a deeper lens: many positional schemes can be read as representations of symmetry groups such as the translation group.

<details><summary>References</summary>
<ul>
<li><a href="https://magazine.sebastianraschka.com/p/understanding-positional-embeddings">Understanding Positional Embeddings in Modern LLMs</a></li>
<li><a href="https://apxml.com/courses/how-to-build-a-large-language-model/chapter-13-positional-encoding-variations/rotary-position-embedding-rope">Rotary Position Embedding ( RoPE ) Explained</a></li>
<li><a href="https://arxiv.org/pdf/2102.11090">POSITION INFORMATION IN TRANSFORMERS A OVERVIEW - arXiv.org</a></li>

</ul>
</details>

**Discussion**: Commenters largely praised the explainer but argued it stays at the level of implementation, with one detailed comment framing positional embeddings as group representations — for instance describing RoPE as a representation of the abelian n-dimensional translation group, and noting that this viewpoint is also how one derives and parameterizes learnable variants. The overall sentiment was that the theory is essential for genuinely understanding why these methods work, not just how they are coded.

**Tags**: `#LLMs`, `#positional-embeddings`, `#RoPE`, `#transformers`, `#group-theory`

---

<a id="item-11"></a>
## [Open-source tuner makes pageable cudaMemcpy 5x faster on NVIDIA B300](https://www.reddit.com/r/MachineLearning/comments/1xx2n25/making_cudamemcpy_5x_faster_on_a_b300_p/) ⭐️ 7.0/10

A developer released cudamemcpy-tuner, an open-source tool that accelerates pageable host-to-device CUDA memory copies, claiming a jump from 10.2 GB/s to 51.5 GB/s \(roughly 5x\) when copying a 1 GB uint8 tensor to and from an NVIDIA B300. The tool is invoked as a wrapper \(\`cmt tune -- python bench.py\`\) around existing PyTorch code, so users do not have to rewrite their programs. Host-to-device transfer bandwidth is a long-standing bottleneck for GPU workloads, particularly for data loading, inference pipelines and out-of-core training on large models; a 5x improvement in the pageable path would narrow much of the gap with pinned memory without requiring code changes. Because it targets PyTorch&\#x27;s default transfer path, it could benefit a broad set of practitioners who never explicitly managed pinned buffers. The benchmark is self-reported by the author: a 1 GB \`torch.uint8\` tensor copied with \`x.to\(&quot;cuda&quot;\)\` and \`y.cpu\(\)\`, measured over 5 iterations with \`torch.cuda.synchronize\(\)\`, and the gain applies specifically to pageable transfers rather than to already-pinned memory. No independent verification or discussion was available, so the 51.5 GB/s figure should be treated as a single-machine, single-GPU result that may vary with CPU, PCIe/NVLink topology and tensor size.

reddit · r/MachineLearning · /u/makneeee · Nov 15, 18:20

**Background**: In CUDA, host memory is normally pageable, meaning the OS can swap it, so the driver cannot DMA directly from it; instead cudaMemcpy first stages the data through an internal pinned \(page-locked\) buffer before transferring to the GPU, which adds an extra copy and slows things down. Using explicitly pinned memory avoids that staging step and is the standard optimization recommended by NVIDIA, but it requires extra code and has side effects such as reduced usable system memory. The B300 is NVIDIA&\#x27;s Blackwell Ultra data-center GPU with 288 GB of HBM3e per card, aimed at large-scale AI training and inference.

<details><summary>References</summary>
<ul>
<li><a href="https://stackoverflow.com/questions/50184146/cuda-pinned-memory-vs-pageable-memory-tradeoffs">optimization - CUDA - Pinned Memory vs . Pageable ... - Stack Overflow</a></li>
<li><a href="https://developer.nvidia.com/blog/how-optimize-data-transfers-cuda-cc/">How to Optimize Data Transfers in CUDA C/C++ | NVIDIA Technical...</a></li>
<li><a href="https://nebius.com/compute/b300">NVIDIA HGX B 300 on Nebius AI Cloud — Blackwell Ultra GPU ...</a></li>

</ul>
</details>

**Tags**: `#CUDA`, `#GPU memory transfer`, `#performance optimization`, `#PyTorch`, `#open-source tooling`

---

<a id="item-12"></a>
## [Training-free early exit for reasoning models by editing one output-layer weight row](https://www.reddit.com/r/MachineLearning/comments/1xx1xdm/trainingfree_early_exit_for_reasoning_models_a/) ⭐️ 7.0/10

A developer built a training-free early-exit mechanism for reasoning LLMs by adding a linear-probe direction \(computed with linear discriminant analysis, no gradient training\) at strength 14 to the single output-layer weight row that scores the &lt;/think&gt; token. Fitted on hidden states recorded from 24 math problems, the edited Qwen3.5-4B kept the same accuracy on 8 unseen MATH-500 problems while using 54% fewer tokens, and an edited DeepSeek V4.1 Flash solved 7/7 versus 6/7 problems with 40% fewer tokens. Reasoning models often reach the right answer early and then spend thousands of tokens double-checking, so a method that curtails this overthinking without retraining or any inference-time code could cut serving costs broadly. Because the result is an ordinary, portable weights file \(released as GGUF and runnable in stock llama.cpp\), it can be dropped into existing deployment stacks rather than requiring a new inference framework. The author acknowledges that stopping reasoning early via a probe on hidden states is already published \(e.g. Zhang et al. 2025, arXiv 2504.05419\); the novelty is folding the probe into that single weight row so nothing extra runs at inference, plus the reported measurements. Caveats include small sample sizes with one run per setting, a probe fitted on math data only \(the coding-agent results are transfer\), and an AIME 2025 comparison run at a 32k-token budget, below the 81,920 tokens Qwen recommends for competition math; because only one token&\#x27;s score changes, the edited model&\#x27;s behavior could also be simulated offline from recordings of the original.

reddit · r/MachineLearning · /u/Good-Presentation-23 · Nov 15, 17:52

**Background**: Reasoning models such as DeepSeek and Qwen &quot;think&quot; in a scratchpad before answering, and that scratchpad ends when the model emits a special &lt;/think&gt; token. At each step the model computes a hidden state summarizing everything so far, and the final output layer holds one weight row per vocabulary token; a token&\#x27;s score is its row multiplied by the hidden state, so the score for &quot;stop thinking now&quot; comes from exactly one row. Early-exit methods generally try to terminate computation adaptively when the model is already confident, while a linear probe is a simple linear classifier \(here fitted with linear algebra rather than gradient descent\) trained to separate two classes of hidden states.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2407.20272">[2407.20272] An Efficient Inference Framework for Early - exit Large ...</a></li>
<li><a href="https://www.emergentmind.com/topics/early-exit-large-language-models">Early - Exit LLMs: Adaptive Inference</a></li>
<li><a href="https://apxml.com/courses/how-to-build-a-large-language-model/chapter-23-analyzing-model-behavior/probing-internal-representations">Probing LLM Hidden States - apxml.com</a></li>

</ul>
</details>

**Tags**: `#LLM reasoning`, `#early exit`, `#inference efficiency`, `#model editing`, `#DeepSeek/Qwen`

---

<a id="item-13"></a>
## [Marimba: an open-weight &\#x27;System One&\#x27; speech model built on frozen Qwen3-ASR-0.6B](https://www.reddit.com/r/MachineLearning/comments/1xwzsm4/marimba_a_system_one_model_for_speech_r/) ⭐️ 7.0/10

A developer released Marimba, an open-weight \(Apache-2.0\), pip-installable \(&\#x27;marimba-audio&\#x27;\) speech model that runs on a frozen Qwen3-ASR-0.6B and returns typed decisions instead of transcripts — yes/no answers, multiple-choice selections, or numeric scores. Word-level and language-level questions are answered with zero-shot scores derived from the ASR decoder&\#x27;s hypotheses followed by calibration, while small readouts trained on the frozen encoder handle voice activity, turn endings, speaker changes, and speaker count; a paper is promised on arXiv the same week. Marimba argues that many speech tasks in voice agents and pipelines only need a fast, cheap, structured decision rather than a full LLM-style generation, so repurposing a small frozen ASR checkpoint with lightweight readouts could cut latency and compute for things like barge-in detection and turn-taking. Open weights plus a pip package and benchmark make the approach easy to reproduce and drop into real-time voice-agent stacks. Because the Qwen3-ASR-0.6B backbone stays frozen, only the small encoder readouts and calibration layers are trained, keeping the model lightweight and cheap to run. The trade-off is that outputs are limited to typed decisions rather than free-form transcripts, and the demo materials do not report absolute accuracy or latency figures beyond the linked benchmark page.

reddit · r/MachineLearning · /u/solanotodesch · Nov 15, 16:30

**Background**: A &\#x27;System One&\#x27; model, borrowing the dual-process framing from psychology, is designed to give fast, automatic, structured answers to narrow questions rather than reasoning step by step or writing paragraphs like a chatbot. Qwen3-ASR-0.6B is Alibaba&\#x27;s compact Apache-2.0 speech recognition model covering 30 languages and 22 Chinese dialects, with language identification and streaming support, which makes it a convenient frozen backbone. In ASR, a decoder produces candidate hypotheses with scores; &\#x27;zero-shot&\#x27; here means reusing those existing scores — plus a calibration step — to answer new questions without retraining the recognizer.

<details><summary>References</summary>
<ul>
<li><a href="https://www.globaltechcouncil.org/ai/what-is-a-system-one-model/">What Is a System One Model? - Global Tech Council</a></li>
<li><a href="https://www.anchorterminal.com/tools/qwen3-asr-0-6b">Qwen 3 - ASR - 0 . 6 B review (2026): pricing, alternatives and grade C</a></li>
<li><a href="https://apxml.com/courses/speech-recognition-synthesis-asr-tts/chapter-2-advanced-acoustic-modeling-asr/asr-decoding-algorithms">Comparing ASR Decoding Algorithms</a></li>

</ul>
</details>

**Tags**: `#speech-recognition`, `#ASR`, `#small-models`, `#efficient-inference`, `#open-weights`

---

<a id="item-14"></a>
## [Reddit user voltage-glitches CMP 170HX mining card to unlock 80GB VRAM and 126 SMs](https://www.reddit.com/r/LocalLLaMA/comments/1xwxzgj/i_finally_succeed_the_cmp_170hx_voltage_glitch/) ⭐️ 7.0/10

A Reddit user \(u/Yarukiless-cat\) reported successfully performing a voltage glitch on an NVIDIA CMP 170HX mining card, booting it with 80GB of VRAM and all 126 Streaming Multiprocessors recognized by the system. The mod was carried out with a Raspberry Pi Pico after roughly 15 hours of work, with the restricted write-access portion scripted with help from an AI assistant called Astra; the user plans to do the same to a second card. The hack effectively converts a cheap, artificially fused-off mining card built on the same GA100 die as the A100 into an A100-80GB-class accelerator, which is highly attractive for local LLM inference where VRAM capacity is the main bottleneck. With used CMP 170HX cards costing a few thousand dollars versus $20,000 or more for a real A100 80GB PCIe card, it could open a low-cost path to large-model hosting for hobbyists and small labs. The method builds on a GA100 microcode-exploit paper published only days earlier and works by glitching the card&\#x27;s fuse controller so the fused-off HBM capacity and SMs are re-enabled; reports suggest the unlocked card can even outperform a retail A100 in FP16. It requires manual timing calibration and repeated attempts, and since NVIDIA was reportedly notified before publication, future driver or firmware mitigations are plausible.

reddit · r/LocalLLaMA · /u/Yarukiless-cat · Nov 15, 15:16

**Background**: NVIDIA&\#x27;s CMP 170HX was a 2021 card for Ethereum miners built on the same GA100 die as the A100, but deliberately crippled: 8GB of usable HBM instead of 80GB, only 70 SMs enabled out of 126, PCIe Gen1, and no NVLink. The crippling is enforced by on-chip fuses rather than purely by firmware, so ordinary software mods such as CMPunlocker can only recover part of the hardware. Voltage glitching is a hardware attack that briefly dips the chip&\#x27;s supply voltage to induce a fault at a precise moment, which here causes the fuse controller to misread or skip the lock settings. Streaming Multiprocessors \(SMs\) are the fundamental compute units inside an NVIDIA GPU, so enabling more of them directly increases raw compute throughput.

<details><summary>References</summary>
<ul>
<li><a href="https://hwbusters.com/news/voltage-glitching-turns-nvidias-cmp-170hx-mining-card-into-an-80gb-a100-that-outruns-the-real-thing/">Voltage Glitching Turns NVIDIA&#x27;s CMP 170HX Mining Card Into ...</a></li>
<li><a href="https://www.tomshardware.com/pc-components/gpus/techie-turns-usd2-500-cmp-170hx-8gb-mining-card-into-a-full-fat-a100-80gb-with-voltage-glitching-carefully-blowing-onboard-fuses-to-unlock-entire-vram-and-shader-modules">Techie uses voltage glitching hack to turn $2,500 Nvidia 8 GB ...</a></li>
<li><a href="https://tau-home.com/en/post/cmp-170hx-voltage-glitching-unlocks-80gb-vram-126-sm/">CMP 170HX Mining GPU Hardware Lock Broken via Raspberry Pi ...</a></li>

</ul>
</details>

**Tags**: `#hardware-hacking`, `#voltage-glitching`, `#GPU-modding`, `#local-llm`, `#nvidia-cmp`

---

<a id="item-15"></a>
## [inside-llm: Open-Source Tool Visualizes LLM Token Probabilities and Quantization Divergence](https://www.reddit.com/r/LocalLLaMA/comments/1xx7qbf/i_have_created_a_tool_to_observe_what_happens/) ⭐️ 7.0/10

A developer released inside-llm, an MIT-licensed browser-based tool that loads one or two GGUF models through llama.cpp and streams compact binary frames over a WebSocket to a Svelte 5 + Canvas 2D interface. It renders per-token probability brightness, the full candidate distribution behind each pick, every stage of the sampler chain, and Jensen-Shannon and bidirectional KL divergence between two quantizations of the same model, with exact branching via KV-state snapshots and an optional logit-lens view. Quantization is the default way people run local LLMs, yet the community has had little tooling to see exactly where a Q4\_K\_M build starts behaving differently from a Q8\_0 one. By turning that comparison into a per-position, token-by-token visual with quantitative divergence metrics, inside-llm gives local-LLM practitioners and quantization researchers a practical way to audit quant quality instead of relying only on benchmark scores. The tool requires that models A and B share a tokenizer \(for example two quants, a base and a fine-tune, or sizes within one family\) and that both fit in VRAM simultaneously on a single GPU, otherwise it falls back to slow CPU inference; it is text-only and does not support split GGUF files or embedding models. It ships as self-contained Linux \(glibc 2.35+\) and Windows packages with CUDA or Vulkan backends, runs entirely on 127.0.0.1 with no accounts or telemetry, and can record sessions to a compressed frame stream that replays in a static page with no engine, model, or GPU.

reddit · r/LocalLLaMA · /u/AlternativeEnough352 · Nov 15, 21:46

**Background**: GGUF is the standard file format for llama.cpp, bundling model weights together with everything needed for inference such as the tokenizer, and quantization compresses those weights from higher precision down to 8-bit, 4-bit, or lower so large models fit in limited memory. Lower-bit quantization saves memory and speeds up inference but can subtly change which token the model prefers at a given position, which is why people compare quants like Q4\_K\_M against Q8\_0. Before a token is drawn, llama.cpp runs a sampler chain — penalties, top-k, top-p, min-p, temperature, and optionally a GBNF grammar — that prunes and reshapes the raw probability distribution, so divergence between two models can come from either the weights or the sampling stages. Jensen-Shannon divergence and Kullback-Leibler divergence are standard statistical measures of how different two probability distributions are, with JSD being symmetric and bounded while KL is directional.

<details><summary>References</summary>
<ul>
<li><a href="https://pristren.com/blog/gguf-quantization-guide-2026/">GGUF Quantization Explained : Q4_K_M vs Q8_0 and When Each...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Jensen%E2%80%93Shannon_divergence">Jensen–Shannon divergence - Wikipedia</a></li>
<li><a href="https://letsdatascience.com/blog/llm-sampling-temperature-top-k-top-p-and-min-p-explained">LLM Sampling: Temperature, Top-K, Top-P, and Min-P Explained</a></li>

</ul>
</details>

**Tags**: `#LLM interpretability`, `#quantization`, `#llama.cpp`, `#GGUF`, `#visualization tools`

---

<a id="item-16"></a>
## [audio.cpp 0.9.5 Demo Chains Three Models Into Fully Local Real-Time Avatar Chat](https://www.reddit.com/r/LocalLLaMA/comments/1xx2vi0/audiocpp_soulxflashhead_lfm3audio_owsm_v4/) ⭐️ 7.0/10

audio.cpp 0.9.5 ships an &quot;avatar voice chat&quot; app in its WebUI that chains three models together: SoulX-FlashHead for real-time talking-head video generation, OWSM v4 for speech-to-text transcription, and LFM3-Audio for conversational responses and text-to-speech. On an RTX 5090 the pipeline reaches roughly 850ms between submitting a question and the avatar starting to speak. This demonstrates that a complete speech-to-avatar conversation loop — recognition, dialogue, synthesis, and lip-synced video — can now run entirely on a local workstation-grade GPU without any cloud API, which matters for privacy-sensitive, offline, or latency-critical applications. It also shows the local-AI stack maturing from single-model demos into composable multi-model pipelines shipped inside existing tooling. The video stage remains GPU-heavy: SoulX-FlashHead calls for an RTX 4090 or better, and cuDNN is mandatory — without it inference is 2x slower and VRAM usage doubles. LFM3-Audio is actually invoked twice, because the speech-to-speech path only produces one voice, so its TTS is used to re-synthesize the S2S response in a different voice; the author notes this and the prototype WebUI overhead as obvious targets for a more optimized native app.

reddit · r/LocalLLaMA · /u/Acceptable-Cycle4645 · Nov 15, 18:29

**Background**: SoulX-FlashHead is a 1.3B-parameter framework from Soul-AILab for high-fidelity, infinite-length, real-time streaming portrait video generation, reported to hit about 10.8 FPS on a single RTX 4090. OWSM v4 is CMU WAVLab/ESPnet&\#x27;s fully open, Whisper-style speech recognition model family, trained on public data with released weights and training code. LFM3-Audio-2B is Liquid AI&\#x27;s compact audio model that accepts text or audio and responds with text, speech, or both, designed to run locally on laptops and edge devices. audio.cpp is the local inference engine that packages these models behind a WebUI, so users can assemble them into a cascaded pipeline rather than a single end-to-end model.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Soul-AILab/SoulX-FlashHead-1_3B">Soul-AILab/ SoulX - FlashHead -1_3B · Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2506.00338">[2506.00338] OWSM v4: Improving Open Whisper-Style Speech ... WAVLab | Open Whisper-style Speech Models (OWSM) OWSM v4: Improving Open Whisper-Style Speech Models via Data ... OWSM v4 — speech-to-text model: WER, licence &amp; install | STT ... espnet/egs2/owsm_v4 at master - GitHub</a></li>
<li><a href="https://huggingface.co/LiquidAI/LFM3-Audio-2B">LiquidAI/ LFM 3 - Audio -2B · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#speech-to-speech`, `#real-time-inference`, `#talking-head-generation`, `#audio.cpp`

---

<a id="item-17"></a>
## [Paper Claims First Recursive Self-Improvement of a Full Frontier Pre-Training Run](https://www.reddit.com/r/LocalLLaMA/comments/1xwt3ri/paper_no_second_run_does_rsi_stop_at_frontier/) ⭐️ 7.0/10

A Reddit paper post claims to be the first to apply recursive self-improvement \(RSI\) to an entire frontier pre-training run from scratch, decomposing the problem into smaller loops because a single pre-training run cannot be repeated. The authors report 801-30B-A3B-Base, a 30B-A3B mixture-of-experts model trained from scratch on 11.8 trillion tokens in three months by a newly formed team, and link an arXiv paper \(2611.10719\), GitHub repository, and a lightweight SFT dataset. Public RSI work has focused on post-training, which starts from an existing base model and can be iterated with verifiable scores; extending RSI to pre-training would let AI improve the process that creates foundation models themselves. If the claims hold up, the approach and the open-sourced base model plus SFT data could offer a concrete template for applying self-improvement to the most expensive and least repeatable stage of LLM development. The paper argues that pre-training breaks three conditions that make post-training RSI tractable: runs cost hundreds of thousands of GPU-hours over months and cannot be repeated, post-training headroom cannot be read from a single score, and the target of improvement is the whole production system rather than just a model. The released 801-30B-A3B-Base is said to outperform Qwen3-30B-A3B and Nemotron-3.5-Lightning-30B-A3B while trailing the larger Qwen3.5-35B-A3B, and the reported SFT is only a 6-billion-token probe with no RL; the model weights are listed as “Coming Soon,” and the claims have not been peer reviewed.

reddit · r/LocalLLaMA · /u/pmttyji · Nov 15, 11:21

**Background**: Recursive self-improvement \(RSI\) describes a process in which an AI system iteratively designs a more capable successor, and in LLM research it has mostly been studied at inference time or in post-training loops where outputs can be scored and retried. Pre-training is the earlier, far more expensive stage that produces a base model from massive text corpora; post-training then adapts that base model with supervised fine-tuning \(SFT\) or reinforcement learning. A 30B-A3B mixture-of-experts model has roughly 30 billion total parameters but activates about 3 billion per token, which reduces inference cost. “Post-training headroom” refers to how much additional capability can still be gained by SFT or RL on top of a given base model.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement - Wikipedia</a></li>
<li><a href="https://build.nvidia.com/nvidia/nemotron-3.5-lightning-30b-a3b">nemotron-3.5-lightning- 30 b - a 3 b Model by NVIDIA | NVIDIA NIM</a></li>
<li><a href="https://llm-stats.com/models/compare/nemotron-3-nano-30b-a3b-vs-qwen3-next-80b-a3b-base">Nemotron 3 Nano ( 30 B A 3 B ) vs Qwen3-Next-80 B - A 3 B - Base ...</a></li>

</ul>
</details>

**Tags**: `#recursive-self-improvement`, `#pre-training`, `#foundation-models`, `#LLM-research`, `#AI-scaling`

---

<a id="item-18"></a>
## [Report: Export-Banned Nvidia Chips Power China’s Top AI Models](https://www.reddit.com/r/artificial/comments/1xx4t46/exportbanned_nvidia_chips_are_behind_chinas_most/) ⭐️ 7.0/10

A TechCrunch report, surfaced in a Reddit r/artificial post, claims that China’s most powerful AI models are built on Nvidia chips that U.S. export controls prohibit from being sold to China. The report frames this as evidence that restrictions have not kept advanced accelerators out of Chinese AI labs. If accurate, the finding undercuts a central assumption of U.S. AI chip policy—that cutting off top Nvidia accelerators will slow China’s frontier model development—and could intensify pressure to tighten enforcement, including around intermediaries and cloud access. The Reddit submission itself contains no article text, so it does not identify which models, chip models, volumes, or procurement routes are involved, making independent verification difficult from the provided item alone. Separate reporting has documented billions of dollars of export-restricted accelerators reaching China through intermediaries, while U.S. rules ban sales of H100, A100, and Blackwell-family chips to China.

reddit · r/artificial · /u/IndependentCoast3974 · Nov 15, 19:46

**Background**: U.S. export controls on advanced AI chips to China began in 2022, when the Biden administration restricted sales of Nvidia’s H100 and A100. Nvidia responded by creating China-market variants such as the H800 and A800 that fell just below the performance thresholds, and later the H20. Washington has since moved to close loopholes, including rules aimed at Chinese firms buying chips through overseas entities or accessing them remotely via cloud services.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/billions-worth-of-export-restricted-ai-accelerators-sold-to-china-report-details-how-chinese-firms-skirt-trumps-regulations">Investigative report details how export - restricted Nvidia AI chips...</a></li>
<li><a href="https://www.nytimes.com/2025/04/15/technology/nvidia-h20-chip-china-restrictions.html">Nvidia Says U.S. Will Restrict Sales of More of Its A.I. Chips to China ...</a></li>
<li><a href="https://qz.com/us-commerce-department-loophole-nvidia-ai-chips-china-053126">U.S. closes loophole on Nvidia AI chip exports to Chinese firms</a></li>

</ul>
</details>

**Tags**: `#Nvidia`, `#export controls`, `#China AI`, `#AI hardware`, `#geopolitics`

---

<a id="item-19"></a>
## [Meituan open-sources LongCat-2.5, a 1.6T agent model documented only for Huawei NPUs](https://www.reddit.com/r/artificial/comments/1xwx2hc/meituan_opensourced_longcat25_a_16t_agent_model/) ⭐️ 7.0/10

Meituan released the LongCat-2.5 weights under the MIT license: a native multimodal Mixture-of-Experts model with 1.6 trillion total parameters and roughly 48 billion activated per token, accepting text, image and video input. On Meituan&\#x27;s own benchmark table it scores 88.4 on Terminal Bench v2.1 versus 89.1 for Claude Opus 5, but the model card currently documents only Huawei NPU deployment with no Nvidia path. A 1.6T-parameter agentic model released under MIT by a major Chinese lab is a substantial open-weights contribution, and the NPU-only deployment documentation is a notable signal about hardware ecosystems diverging around Chinese model releases. Developers choosing self-hosting stacks may now have to weigh Ascend hardware against the Nvidia tooling most agent frameworks assume. The gap with Claude Opus 5 widens sharply on the harder Terminal Bench v4.0 \(38.5 versus 53.9\), and the API supports both OpenAI and Anthropic request formats, which makes it cheap to drop into existing agent setups. Other published figures include 91.9 on BrowseComp and 82.1 on PaperBench, alongside a 1M-token context window and W4A4 inference support.

reddit · r/artificial · /u/javimbuilds · Nov 15, 14:37

**Background**: LongCat-2.5 is a Mixture-of-Experts model, meaning only a small slice of its 1.6 trillion parameters is activated for each token, which keeps inference cost far below what the total size suggests. Deploying on Huawei Ascend NPUs requires Huawei&\#x27;s CANN software stack along with torch\_npu and projects such as vLLM-Ascend, which together play the role that CUDA and standard vLLM play on Nvidia GPUs. Terminal Bench is an agent benchmark that measures whether a coding agent can complete real command-line tasks end to end, so a near-parity score there speaks directly to agentic coding ability.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/meituan-longcat/LongCat-2.5">meituan-longcat/LongCat-2.5 · Hugging Face</a></li>
<li><a href="https://arxiv.org/pdf/2506.12708">Serving Large Language Models on Huawei CloudMatrix384</a></li>
<li><a href="https://nodemini.com/en/blog/2026-openpangu-2-open-source-huawei-ascend-moe.html">Huawei &#x27;s openPangu 2.0 Is Now Open-Source — and It... | NodeMini</a></li>
<li><a href="https://www.tbench.ai/">TERMINAL - BENCH</a></li>

</ul>
</details>

**Tags**: `#open-weight models`, `#LLM agents`, `#Huawei NPU`, `#model release`, `#benchmarks`

---

<a id="item-20"></a>
## [Anthropic rebuilds Claude Code Projects around a coordinator and parallel cloud threads](https://www.reddit.com/r/artificial/comments/1xwj3v0/anthropic_rebuilds_claude_code_projects_around_a/) ⭐️ 7.0/10

In a Nov 14 product update, Anthropic rebuilt Claude Projects from a static folder of files into a coordinated set of working sessions: you describe the work in one conversation, and a coordinator scopes the request, delegates it to parallel threads, reviews the outputs, and assembles the final result. Each thread is a full Claude Code cloud session with its own copy of the repo and its own Git branch, and can further split its task into subagents, loops, or workflows while you steer it remotely from a phone. It is in public beta, rolling out gradually to select Pro/Max/Ultra subscribers who use Claude Code cloud sessions, with a waitlist for everyone else. This marks a shift in agentic coding from a single interactive session toward a managed multi-agent orchestration model, where work continues in the cloud after you close your laptop and only review and coordination need human attention. Because Claude Code is one of the most widely used AI coding tools, this coordinator/worker design is likely to become a reference pattern that competing agent platforms copy. Anthropic is upfront about the limits: threads currently run only in the cloud, with local code and VPN support promised &quot;very soon&quot;, and each parallel thread counts as a full session so running six threads burns roughly six times the plan usage. If two threads touch the same code, the overlap surfaces as an ordinary merge conflict in a pull request, so parallel agents do not eliminate Git conflicts; Team and Enterprise plans do not have access yet.

reddit · r/artificial · /u/winer666 · Nov 15, 01:38

**Background**: Claude Code is Anthropic&\#x27;s agentic coding tool that can run either locally in your terminal or as a cloud session on a fresh VM against a GitHub repository, launched from the desktop app, the web, mobile, or with \`claude --cloud\`. Projects was previously a way to group files and context for a body of work; this update turns it into an orchestrator that fans one request out to many isolated cloud sessions. Isolating parallel workers on separate branches \(or git worktrees\) is a common pattern in multi-agent coding setups, because it keeps concurrent edits from corrupting each other&\#x27;s working copy.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/claude-code-on-the-web">Use Claude Code in the cloud - Claude Code Docs</a></li>
<li><a href="https://data-today.net/claude-code-projects-parallel-agent-coordination/">Claude Code Projects adds parallel AI agent coordination</a></li>
<li><a href="https://www.five.reviews/ai-tools/claude-code-multiple-agents/">Claude Code Multiple Agents : How Projects Work</a></li>

</ul>
</details>

**Tags**: `#AI coding agents`, `#Anthropic`, `#Claude Code`, `#multi-agent systems`, `#developer tooling`

---

<a id="item-21"></a>
## [&\#x27;Birdbrain&\#x27; Is a Misnomer: Crows Decide Faster Than Humans](https://www.nytimes.com/2026/11/15/science/birdbrain-crows-birds-research-decision.html) ⭐️ 6.0/10

New research reported by The New York Times suggests that crows can make rapid decisions—faster than humans—even though birds lack the layered cerebral cortex that mammals rely on for high-level integration. The finding reinforces that complex cognition and fast decision-making do not require a mammalian-style layered cortex, suggesting that intelligence can evolve through multiple independent routes. This has implications for neuroscience and for comparisons between biological and artificial intelligence. The report&\#x27;s central claim is that crows achieve fast decisions without a layered cerebral cortex, but the available summary does not specify the species, task, or measured reaction times, so the comparison with human speed should be treated as a headline finding rather than a precise benchmark.

hackernews · gumby · Nov 15, 17:53 · [Discussion](https://news.ycombinator.com/item?id=50509023)

**Background**: The cerebral cortex is the outer layer of neural tissue in the mammalian brain, and its six-layered neocortex is often described as the highest integration center for complex cognition. Birds lack this layered cortex, yet corvids such as crows, ravens, and jays show sophisticated behaviors including tool use and social reasoning. This is a classic example of convergent evolution, in which distant lineages independently evolve similar capabilities through different neural architectures.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebral_cortex">Cerebral cortex - Wikipedia</a></li>
<li><a href="https://www.science.org/doi/10.1126/science.1098410">The Mentality of Crows: Convergent Evolution of Intelligence ...</a></li>
<li><a href="https://discoverwildscience.com/intelligence-evolved-twice-how-birds-and-mammals-took-separate-paths-to-genius-1-335666/">Intelligence Evolved Twice: How Birds and Mammals Took ...</a></li>

</ul>
</details>

**Discussion**: Commenters framed the finding as evidence that intelligence evolved at least three times—in mammals, corvids, and octopuses—and noted that corvids have different neuron designs and brain architecture, so there is more than one way to build a smart brain. Some questioned the headline logic, arguing that &\#x27;birdbrain&\#x27; never implied slow decisions, while others suggested smaller brains may allow shorter, faster feedback loops and recommended books such as &\#x27;The Genius of Birds&\#x27;; additional comments highlighted birds&\#x27; magnetic sensing, decentralized body clocks, and the spatial demands of flight.

**Tags**: `#neuroscience`, `#animal cognition`, `#convergent evolution`, `#crows`, `#decision-making`

---

<a id="item-22"></a>
## [Retrospective: Turbo Pascal&\#x27;s Tiny Footprint vs. Modern Software Bloat](https://prog21.dadgum.com/116.html) ⭐️ 6.0/10

A 2011 Prog21 blog post comparing the entire Turbo Pascal development environment with modern software binaries has sparked renewed Hacker News discussion. The piece uses Turbo Pascal&\#x27;s remarkably small size as a yardstick for how large today&\#x27;s executables, tools, and dependencies have become. It frames a still-relevant debate about software bloat, toolchain overhead, and the trade-offs between developer productivity and runtime or distribution size. Developers, language designers, and systems programmers can use the comparison to question which modern inefficiencies are justified and which are accidental. The comparison is qualitative and dated—it comes from 2011 and uses byte counts from different eras and platforms—so it is best read as a conversation starter rather than a rigorous benchmark. Turbo Pascal was notable for its very fast compiler and for bundling editor, compiler, and linker into one integrated development system.

hackernews · ksec · Nov 15, 13:44 · [Discussion](https://news.ycombinator.com/item?id=50506894)

**Background**: Turbo Pascal was a Borland software development system for Pascal on CP/M and MS-DOS, originally developed by Anders Hejlsberg; it combined an editor, compiler, and linker and was known for very fast compilation. Software bloat refers to programs using far more memory, disk space, or dependencies than their functionality seems to require. Modern binaries often include runtime libraries, debug information, boilerplate code, static linking, or frameworks, which can make even simple commands surprisingly large.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Turbo_Pascal">Turbo Pascal - Wikipedia</a></li>
<li><a href="https://www.computerhope.com/jargon/t/turbo-pascal.htm">What Is Turbo Pascal? - Computer Hope</a></li>
<li><a href="https://stackoverflow.com/questions/5933451/why-are-generated-binaries-so-large">c++ - Why are generated binaries so large? - Stack Overflow Usage example</a></li>

</ul>
</details>

**Discussion**: Commenters broadly appreciated Anders Hejlsberg&\#x27;s legacy and Turbo Pascal&\#x27;s design, while debating whether byte-for-byte comparisons are meaningful. Some pointed to the absurdity of a simple &\#x27;touch&\#x27; binary exceeding Turbo Pascal, one commenter asked why Pascal faded despite its influence, and another criticized size comparisons as context-free.

**Tags**: `#Turbo Pascal`, `#software bloat`, `#binary size`, `#programming languages`, `#retrocomputing`

---

<a id="item-23"></a>
## [Emacs Is My Browser: One Developer&\#x27;s EWW-Only Web Experience](https://joshblais.com/blog/emacs-as-my-browser/) ⭐️ 6.0/10

Josh Blais published a blog post on joshblais.com titled &quot;Emacs Is My Browser,&quot; describing his firsthand experience of using GNU Emacs — specifically its built-in EWW \(Emacs Web Wowser\) browser — as his primary way of browsing the web. The post climbed to the front page of Hacker News, where commenters debated where a text-only browser works well and where it breaks down. The experiment is a practical stress test of how much of today&\#x27;s web still works without JavaScript and CSS, and it resonates with a long-running developer debate about page bloat and heavyweight commercial sites. It matters most to Emacs users and people interested in minimalist, distraction-free workflows rather than to the broader consumer web. EWW renders pages through shr.el and basic HTML parsing \(requiring an Emacs built with libxml2\), can display images inline if image support is compiled in, but deliberately offers no CSS or JavaScript support. Commenters noted that the approach works for static HTML and blogs but fails on sites like Reddit and most commercial properties, with embedded WebKit via xwidget as a heavier fallback.

hackernews · nyc111 · Nov 15, 15:21 · [Discussion](https://news.ycombinator.com/item?id=50507553)

**Background**: EWW, short for &quot;Emacs Web Wowser,&quot; is a lightweight web browser built into GNU Emacs that focuses on readability rather than fidelity: it loads and parses pages and presents them as plain text inside an Emacs buffer. Because it has no JavaScript engine or CSS layout, it behaves like a reader mode for the whole web, and many sites that depend on client-side rendering simply do not function. Related options include w3m-mode, the standalone Dillo browser, and xwidget-based embedded WebKit widgets for pages that truly need a full engine.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Eww_%28web_browser%29">eww (web browser) - Wikipedia</a></li>
<li><a href="https://www.gnu.org/software/emacs/manual/html_mono/eww.html">Emacs Web Wowser - GNU</a></li>
<li><a href="https://emacsdocs.org/docs/emacs/EWW">48.1 Web Browsing with EWW - Emacs Docs</a></li>

</ul>
</details>

**Discussion**: Sentiment was appreciative but pragmatic: commenters agreed the setup shines on static HTML and blogs yet fails on the modern commercial web, with xwidget/embedded WebKit suggested as a heavier workaround. Others plugged adjacent hacks \(a follow-mode-based column layout for fitting more text on screen, and w3m-mode with tabs and session management on an underpowered laptop\), while one commenter argued the real priority is a content-addressable replacement for HTTP\(S\) with meaningful adoption, calling minimalist browser setups fun but insufficient.

**Tags**: `#Emacs`, `#EWW`, `#web browsing`, `#developer workflows`, `#Hacker News discussion`

---

<a id="item-24"></a>
## [Apollo&\#x27;s &\#x27;Grenade Launcher&\#x27; Was a Mortar for Lunar Seismic Experiments](https://space.stackexchange.com/questions/37775) ⭐️ 6.0/10

A 2019 Space StackExchange answer explains that the &\#x27;grenade launcher&\#x27; associated with some Apollo missions was actually a small mortar used to deploy explosive seismic charges for ALSEP geophysics experiments, not a weapon for astronauts. The answer and HN thread draw on NASA&\#x27;s ALSEP Flight System Familiarization Manual to clarify how the mortar package was armed and fired from Earth. It matters as a compact case study in how primary technical documents correct popular misconceptions about space history, and it shows that Apollo&\#x27;s scientific legacy included active geophysics experiments, not just rock collection. The discussion also illustrates how source scrutiny can add value to a trivia thread. The seismic-source mortar ammunition canisters used hexanitrostilbene as the main explosive fill, and the manual excerpt quoted in comments says the package was activated by Earth commands such as &\#x27;arm grenades&\#x27; and &\#x27;fire grenades,&\#x27; gated through the grenade arming circuit. The system was an engineered part of lunar seismic profiling, not a crew-operated firearm.

hackernews · Skyfall106 · Nov 15, 09:06 · [Discussion](https://news.ycombinator.com/item?id=50505271)

**Background**: ALSEP was a suite of scientific instruments deployed on the Moon by Apollo 12, 14, 15, 16, and 17; Apollo 11 left a smaller package called EASEP. Its active seismic experiments used explosive charges to generate seismic waves that seismometers could record, helping scientists infer the lunar crust&\#x27;s structure. The mortar was simply a way to place those charges at known distances from the sensors, and the informal &\#x27;grenade launcher&\#x27; label is not a description of an anti-personnel weapon.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apollo_Lunar_Surface_Experiments_Package">Apollo Lunar Surface Experiments Package - Wikipedia</a></li>
<li><a href="https://www.nasa.gov/wp-content/uploads/static/history/alsj/ALSEPDocs.html">ALSEP Manuals - NASA</a></li>
<li><a href="https://en.wikipedia.org/wiki/TP-82">TP-82 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: HN commenters added context by quoting NASA manual language about arming and firing the mortar, noting that the Soviet TP-82 survival gun was carried for defense against bears and wolves in Siberia, and scrutinizing the DrSheldon account&\#x27;s suspicious one-question-per-day and self-answered pattern. Some also questioned why the question was asked at all when the cited ALSEP manual already explains the purpose, while another commenter went down a rabbit hole about whether &\#x27;thumper&\#x27; owed anything to Dune.

**Tags**: `#space-exploration`, `#apollo-program`, `#history`, `#nasa-alsep`, `#community-discussion`

---

<a id="item-25"></a>
## [COMAC CE-25A: China&\#x27;s 19-seat electric airliner flies with crew for the first time](https://electrek.co/2026/11/15/china-comac-ce-25a-electric-plane-crewed-flight/) ⭐️ 6.0/10

COMAC&\#x27;s CE-25A, a roughly 10-tonne, 19-seat battery-electric commuter aircraft, made its first crewed test flight on Saturday, November 14, 2026, in Binzhou, Shandong, carrying two pilots and a flight test engineer, and the company says all systems performed normally. The flight follows 19 uncrewed test flights completed since February 2, and China&\#x27;s aviation regulator is now reviewing the design for a type certificate. This is the first time a Chinese-built 19-seat all-electric commuter aircraft has flown with people aboard, marking a symbolic step into crewed electric regional aviation for China and a potential alternative to turboprops on short feeder routes. It also positions COMAC to compete in the emerging electric commuter segment, though at ~400 km range the aircraft remains a demonstrator rather than a near-term replacement for mainstream regional airliners. The CE-25A concept, unveiled at the 2023 China International Import Expo, is described as a 19-seat all-electric regional commuter with 10 wing-integrated ducted fans, a target range of roughly 400–500 km and a cruise speed of about 400 km/h, though battery performance, payload, charging infrastructure and certification remain open hurdles. A type certificate is the foundational airworthiness approval of an aircraft&\#x27;s design, so the current regulatory review is an early step in what is typically a multi-year, test-intensive process.

rss · Electrek · Nov 15, 14:43

**Background**: Electric aviation is constrained mainly by battery energy density: jet fuel stores far more energy per kilogram than current lithium-ion packs, so a battery-electric aircraft must carry heavy batteries to fly a meaningful distance, which in turn limits payload and range. For this reason, early electric designs target small aircraft and short hops — commuter and regional routes of a few hundred kilometres — where the weight penalty matters less. Before any such design can carry paying passengers, it must obtain a type certificate from a national aviation authority, confirming through flight testing and analysis that the design meets applicable airworthiness, noise and emissions standards.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Comac_CE-25A">Comac CE-25A - Wikipedia</a></li>
<li><a href="https://aerospaceglobalnews.com/news/comac-ce25a-demonstrator-first-photos/">COMAC CE-25A all-electric commuter aircraft emerges in new images</a></li>
<li><a href="https://sustainableaircraft.com/battery-energy-density-challenge/">The Battery Energy-Density Challenge in Aviation</a></li>

</ul>
</details>

**Tags**: `#electric aviation`, `#aerospace`, `#battery technology`, `#COMAC`, `#clean energy`

---

<a id="item-26"></a>
## [Parallax matches Wikipedia sentences across seven editions at any past date](https://www.reddit.com/r/MachineLearning/comments/1xwttxo/hackathon_project_for_mariadbs_wikipedia_through/) ⭐️ 6.0/10

A hackathon project called Parallax, built at the Junction hackathon in Espoo, ingests Wikipedia revision history for seven language editions \(Finnish, Swedish, German, English, Russian, Estonian and Ukrainian\) — 875,572 revisions so far — and lets a user pick any past date to see, statement by statement, where the editions describe the same thing differently. It stores each sentence as a row in a MariaDB system-versioned table, embeds each distinct sentence once with bge-m3, and uses a Gemini model as a judge to classify candidate pairs as same, partial, contradicts or different. The project shows a compact, working pattern for combining temporal SQL tables with vector search to audit how narratives diverge across languages over time, which is directly relevant to cross-lingual knowledge-base consistency, retrieval-augmented generation grounding, and research on bias in Wikipedia. The same pipeline is also applied to chatbot answers, checking each generated statement against what the editions actually say. The dataset holds 90,070 distinct sentence embeddings \(bge-m3, 1024 dimensions\) generated on an A100 at roughly 4,555 sentences per second, and edits reverted within 24 hours or undone by a revert are filtered out so vandalism does not truncate a sentence&\#x27;s lifetime. Inside a single article exact search beats the HNSW index \(4 ms median\), while across the whole database the index takes over with recall@10 of 0.997 against exact search at ef\_search 1000; retrieval alone put the correct sentence at top-1 only 57% of the time \(89% top-5\) on 28 hand-checked pairs, a sample the author admits is too small to properly validate the LLM judge.

reddit · r/MachineLearning · /u/Loxbey · Nov 15, 12:03

**Background**: MariaDB&\#x27;s system-versioned tables, available since version 10.3.4, keep every historical version of a row with a system-time period, so a query can use FOR SYSTEM\_TIME AS OF to read the database exactly as it looked at a past moment. bge-m3 is BAAI&\#x27;s multilingual embedding model, producing dense vectors that allow sentences in different languages to be compared by similarity, and MariaDB&\#x27;s VEC\_DISTANCE\_COSINE function ranks such vectors directly inside SQL. Because Wikipedia retains the full revision history of every article in every language edition, cross-edition comparison over time is possible in principle, but it requires aligning individual sentences rather than whole articles.

<details><summary>References</summary>
<ul>
<li><a href="https://mariadb.com/docs/server/reference/sql-structure/temporal-tables/system-versioned-tables">System - Versioned Tables | Server | MariaDB Documentation</a></li>
<li><a href="https://huggingface.co/BAAI/bge-m3">BAAI/ bge - m 3 · Hugging Face</a></li>
<li><a href="https://severalnines.com/blog/introduction-to-mariadb-vector-search/">Introduction to MariaDB Vector Search | Severalnines</a></li>

</ul>
</details>

**Tags**: `#Wikipedia`, `#MariaDB`, `#sentence embeddings`, `#temporal databases`, `#multilingual NLP`

---

<a id="item-27"></a>
## [Basalt 0.4.0 adds router support and its first dense model, Qwen 27B NVFP4](https://www.reddit.com/r/LocalLLaMA/comments/1xx1cu9/basalt_040_more_models_still_as_fast_qwen_27b_up/) ⭐️ 6.0/10

Basalt, a local LLM inference engine for NVIDIA Blackwell GPUs, released version 0.4.0, adding multi-model and router support \(starting with DeepSeek V4.1 Flash\), video input, file attachments in chats, and its first dense model, a Qwen 3.8 27B NVFP4 quant. The author reports up to 776 tok/s on structured output, 262 tok/s in conversation, 194 tok/s on prose, and 12,000 tok/s prefill at 4K context, all single-stream on an RTX 5090. The release shows that 4-bit NVFP4 quantization on Blackwell can preserve most of a dense model&\#x27;s fidelity \(92.8% top-1 agreement with BF16, 0.0262 KLD\) while delivering several hundred tokens per second on consumer hardware, which is the sweet spot local-inference users care about. Shipping dense kernels now is also a deliberate head start for the upcoming Qwen 4 generation, signaling where the project is heading beyond mixture-of-experts models. Basalt remains an early-stage 0.4.0 project from a single author and is targeted narrowly at NVIDIA Blackwell \(sm\_120\) on Linux and Windows x64; prefill throughput degrades as context grows, and the model has already handled conversations, tools, thinking, images and video with a reported 262K context. The 92.8% top-1 figure is measured against the full BF16 model rather than an absolute benchmark score, so real-world quality on long or unusual prompts may vary.

reddit · r/LocalLLaMA · /u/jesdga95 · Nov 15, 17:30

**Background**: Basalt is a local inference engine designed specifically for NVIDIA&\#x27;s Blackwell GPUs, originally built to run large mixture-of-experts models by keeping the experts that don&\#x27;t fit in VRAM in system RAM or on a second GPU. NVFP4 is NVIDIA&\#x27;s 4-bit floating-point format introduced with Blackwell, which shrinks weights to roughly a quarter of BF16 size to fit bigger models in limited VRAM. To judge whether such aggressive compression is usable, developers compare a quantized model&\#x27;s outputs against the original BF16 model — top-1 agreement and KL divergence \(KLD\) are the standard measures of that fidelity.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/jesdga95/basalt">GitHub - jesdga95/basalt: Local inference engine optimized ...</a></li>
<li><a href="https://basalt.jgulfo.com/">Basalt: a fast local inference engine for NVIDIA Blackwell GPUs</a></li>
<li><a href="https://blog.kubesimplify.com/day-5-local-llm-inference-engines-wrappers-and-what-to-pick">Local LLM Inference Engines on DGX Spark, Explained | Kubesimplify</a></li>

</ul>
</details>

**Tags**: `#local-llm-inference`, `#quantization`, `#nvfp4`, `#gpu-optimization`, `#benchmarks`

---

<a id="item-28"></a>
## [EU&\#x27;s open AI model EUROPA reportedly targets nearly 1 trillion parameters](https://www.reddit.com/r/LocalLLaMA/comments/1xwr917/europa_the_eus_open_ai_model_is_aiming_for_nearly/) ⭐️ 6.0/10

A post on r/LocalLLaMA highlights that EUROPA, the European Union&\#x27;s open AI model, is reportedly aiming for close to 1 trillion parameters. The submission itself is little more than a link with the comment &\#x27;One can hope&\#x27;, so no architecture, training plan, or release timeline was shared. If accurate, a near-trillion-parameter open model backed by the EU would put a sovereign European effort in the same scale class as the largest open-weight Chinese models, strengthening the case that frontier-scale weights can be released publicly. It would also give European enterprises and public institutions a large model they can host and audit themselves rather than relying on US or Chinese providers. The Reddit post contains no technical substance: no parameter breakdown, token budget, dataset, license, or compute allocation is mentioned, and the 1-trillion figure remains unverified. For reference, existing trillion-scale open models such as Kimi K2 and Ling 1T rely on Mixture-of-Experts designs with only a small fraction of parameters active per token, since dense models at that size are extremely expensive to train and serve.

reddit · r/LocalLLaMA · /u/mawcopolow · Nov 15, 09:24

**Background**: EUROPA is presented as the EU&\#x27;s own &\#x27;sovereign&\#x27; open AI model, part of a broader push by European institutions to fund models that can be hosted and governed inside Europe. Europe already has a sizable open-weight ecosystem, including Mistral&\#x27;s models, Apertus, EuroLLM, Aleph Alpha&\#x27;s Kolibri and others, though most sit well below frontier scale. &\#x27;Sovereign AI&\#x27; generally means keeping control over models, data flows and operations rather than depending on foreign cloud providers. Parameter count is only a rough proxy for capability, and at the 1-trillion scale most teams use sparse MoE architectures to keep inference affordable.

<details><summary>References</summary>
<ul>
<li><a href="https://mrkt30.com/european-llms-2026-map/">European LLMs 2026: Full List of European AI Models</a></li>
<li><a href="https://blog.kalavala.net/09-open-weight-model/">9. Kimi K2: The Trillion Parameter Model ! | AI Shenanigans</a></li>
<li><a href="https://gooey.ai/sovereignty">How Middle Powers Cooperate for AI Sovereignty — Gooey. AI</a></li>

</ul>
</details>

**Tags**: `#open-source AI`, `#large language models`, `#EU AI policy`, `#sovereign AI`, `#model scale`

---

<a id="item-29"></a>
## [llama.cpp catches up to custom inference engines on consumer GPUs](https://www.reddit.com/r/LocalLLaMA/comments/1xx607x/llamacpp_performance_improvement_over_time_gemma4/) ⭐️ 6.0/10

Reddit user Danmoreng reports that a fresh benchmark of llama.cpp on their RTX 5080 16GB laptop GPU now matches or beats the custom inference engine they vibe-coded a few months ago, tested on Gemma-family models including a 12B and a 26B variant. When the project started, building something faster than llama.cpp was described as &quot;quite easy,&quot; so the reversal marks a clear performance turnaround for the upstream project. It is an anecdotal but telling signal that llama.cpp — the default engine for most local LLM users — has closed much of the gap with higher-throughput engines like vLLM while remaining far more VRAM-frugal and feature-complete. If sustained, local users on consumer hardware no longer need to trade stability and tooling for raw speed, which weakens the case for niche or bespoke engines. The author explicitly calls the benchmark non-scientific: every run uses a fixed 16k-token prefill plus 1k-token output over Wikipedia text with each engine&\#x27;s optimal settings, and the 26B comparison uses different quantization formats per engine, so it is not even apples-to-apples — yet llama.cpp still wins. The 12B comparison, by contrast, uses the same checkpoint across engines.

reddit · r/LocalLLaMA · /u/Danmoreng · Nov 15, 20:34

**Background**: llama.cpp is an open-source C/C++ inference engine that became the de facto standard for running quantized LLMs locally on consumer CPUs and GPUs, largely thanks to its GGUF model format and low memory overhead. vLLM is a high-throughput serving engine built around PagedAttention, which manages the KV cache in fixed-size pages to reduce memory waste and enable continuous batching, but it is typically far more VRAM-hungry. Local inference workloads split into a compute-bound prefill phase, which processes the prompt tokens in parallel, and a memory-bandwidth-bound decode phase, which generates output tokens one at a time; benchmarks that fix prefill and output lengths, like this one, isolate how an engine handles both.

<details><summary>References</summary>
<ul>
<li><a href="https://pristren.com/blog/vllm-serving-guide/">vLLM : Fastest Open Source LLM Inference Server in 2026</a></li>
<li><a href="https://redis.io/blog/prefill-vs-decode/">Prefill vs Decode: LLM Inference Phases Explained - Redis</a></li>
<li><a href="https://github.com/Neroued/ninfer">GitHub - Neroued/ninfer: High-performance single-GPU ...</a></li>

</ul>
</details>

**Tags**: `#llama.cpp`, `#local-LLM`, `#inference-performance`, `#benchmarking`, `#Gemma`

---

<a id="item-30"></a>
## [BigMoeOnEdge runs any MoE GGUF on 8-16 GB devices, beats Strata and colibri](https://www.reddit.com/r/LocalLLaMA/comments/1xx5fng/bigmoeonedge_outperforms_strata_and_colibri_on/) ⭐️ 6.0/10

A developer \(/u/dai\_app\) released BigMoeOnEdge, a llama.cpp-based runtime that loads any MoE GGUF llama.cpp can load — at any quantization, with no repacking or special format — on NVIDIA, AMD, Intel, Apple Silicon, phones, or plain CPU across Windows, Linux, macOS, Android and iOS. In the posted benchmarks it reports roughly 35 tok/s versus colibri&\#x27;s ~23 on an 8 GB card with Qwen3.6-35B, ~45 versus Strata&\#x27;s ~30 on a 12 GB card, and 20 tok/s on a 16 GB MacBook where colibri&\#x27;s 3.5 release reportedly failed to run. The selling point is generality: instead of hand-writing kernels for a handful of models, BigMoeOnEdge claims to work out of the box for any MoE GGUF, which significantly lowers the effort of running frontier-scale sparse models on consumer and edge hardware. Faster time-to-first-token on long prompts \(5 s versus Strata&\#x27;s 14 s and colibri&\#x27;s near 2 minutes on an 8 GB card\) also addresses one of the most painful parts of SSD-streaming inference. All figures are self-reported by the author and unverified, and Strata is still ahead — by about 1.3x on dual RTX 5060 Ti with Qwen3.8-Flash-Next — on the hardware its kernels are specifically tuned for. The runtime is launched with an --auto flag that auto-detects settings for the machine, and the author claims output is identical to llama.cpp with no quality trade-offs; benchmark logs are published in the repo&\#x27;s docs/bench-data directory.

reddit · r/LocalLLaMA · /u/dai\_app · Nov 15, 20:11

**Background**: Mixture-of-Experts \(MoE\) models like Qwen3&\#x27;s larger variants have far more total parameters than fit in a consumer GPU&\#x27;s VRAM, but each token only routes through a small subset of &\#x27;expert&\#x27; sub-networks, so the full weight file only needs to be read lazily. BigMoeOnEdge exploits this by streaming experts from flash/SSD storage on demand, the same broad strategy used by competing engines such as Strata, colibri and AirLLM. GGUF is llama.cpp&\#x27;s quantized model container format, and quantizations like Q4\_K\_M shrink weights to a few bits per parameter so multi-billion-parameter models can fit on modest hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Helldez/BigMoeOnEdge">GitHub - Helldez/ BigMoeOnEdge : Run MoE models bigger than your...</a></li>
<li><a href="https://apatero.com/blog/gguf-quantized-models-complete-guide-2025">GGUF Quantized Models Complete Guide 2025 | Apatero</a></li>
<li><a href="https://gnana70.medium.com/new-local-ai-engines-you-need-to-know-colibri-strata-airllm-and-freetoken-c0362d68ea62">New Local AI Engines You Need to Know: Colibri, Strata ...</a></li>

</ul>
</details>

**Tags**: `#local-llm`, `#moe-inference`, `#gguf`, `#edge-inference`, `#quantization`

---

<a id="item-31"></a>
## [Axiomic Labs releases X3Guard-150M, a tiny prompt-guard model for edge devices](https://www.reddit.com/r/LocalLLaMA/comments/1xwyp7w/x3guard_a_150m_parameter_prompt_guard/) ⭐️ 6.0/10

Axiomic Labs has released X3Guard-150M, a prompt-guard classifier built on its own GPT-X3-150M base model that labels an incoming prompt as Harmful and/or Adversarial in a single pass. The company says the model outperforms much larger alternatives and runs entirely on-device, including inside a browser with response times in the tens of milliseconds on an iPhone, with a model card and in-browser demo published alongside the release. Prompt-injection and jailbreak filtering has so far mostly meant adding a separate guard model hosted server-side, so a 150M-parameter guard that fits in a browser tab lowers the bar for shipping LLM safety on local, offline and privacy-sensitive deployments. If the performance claims hold up under independent testing, it gives developers of local LLM apps a lightweight alternative to larger guard models for client-side screening. The model is built on GPT-X3-150M, Axiomic Labs&\#x27; third-generation base model on a TX5 hybrid GDN2/gated GQA architecture, which the company claims is the first sub-150M model to exceed an Intelligence Index of 30; the guard outputs two independent labels \(harmful, adversarial\) rather than a single score. The claims about beating larger models and iPhone latency come from the vendor&\#x27;s own announcement and are not backed by benchmark tables or third-party evaluation in the released material, so independent verification is still needed.

reddit · r/LocalLLaMA · /u/DingyAtoll · Nov 15, 15:46

**Background**: A prompt guard is a small text-classification model that sits in front of an LLM and screens inputs for jailbreak attempts, harmful requests and prompt injection — malicious instructions hidden in user input or retrieved documents that try to override the system prompt. Meta&\#x27;s Llama Prompt Guard 2 \(86M parameters, roughly 350MB\) is the best-known open example, and it is typically deployed as a server-side firewall for RAG and agent pipelines. Axiomic Labs is known for browser-runnable small models: GPT-X3 itself runs entirely in the browser after an initial download of about a 267MB model file, which is why a guard built on that base can plausibly run client-side.

<details><summary>References</summary>
<ul>
<li><a href="https://axiomiclabs.com/gpt-x3">GPT-X3 | Axiomic Labs</a></li>
<li><a href="https://catalog.axforge.ai/models/gpt-x3/">GPT-X3: open language model | AxForge</a></li>
<li><a href="https://huggingface.co/meta-llama/Llama-Prompt-Guard-2-86M">meta-llama/Llama- Prompt - Guard -2-86M · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#prompt-security`, `#LLM-safety`, `#edge-AI`, `#small-language-models`, `#model-release`

---

<a id="item-32"></a>
## [Slack&\#x27;s cellular architecture migration isolates failures to a fraction of users](https://www.reddit.com/r/programming/comments/1xwsbxo/slacks_migration_to_a_cellular_architecture/) ⭐️ 6.0/10

A Reddit r/programming link post highlights Slack&\#x27;s engineering write-up describing how Slack moved its most critical user-facing services from a monolithic, multi-availability-zone deployment to a cell-based \(cellular\) architecture over roughly 18 months. In the new model, traffic is partitioned into many small, self-contained cells, and a thin routing layer sends each user to their assigned cell. Cellular architectures cap the blast radius of outages: instead of one failure taking down the entire service, an incident affects only the users in the impacted cell, which is especially valuable for large multi-tenant SaaS platforms where a single bad deploy or dependency failure can otherwise cascade globally. Slack&\#x27;s migration is one of the more thoroughly documented real-world case studies, making it a reference point for other teams weighing similar restructuring. The design relies on partitioning customers across many independent cells plus routing and shuffle-sharding techniques that assign each tenant to a specific cell, with an out-of-path control plane coordinating deployments in waves. The trade-off is that a system with n cells experiences roughly n times as many failure events, but each with only about 1/n of the impact, and operators must accept higher infrastructure overhead and more complex multi-cell deployment and testing workflows.

reddit · r/programming · /u/Ok\_Stomach6651 · Nov 15, 10:33

**Background**: Cell-based architecture applies the bulkhead pattern from ship design to distributed systems: rather than running every service as a single large unit, you break the workload internally into multiple independent mini-clusters \(cells\), each a self-contained scale unit serving a subset of users. A thin router in front maps requests to the right cell, so a crash, bad config, or dependency failure inside one cell stays contained. The approach has gained traction at AWS, DoorDash and other large-scale operators as an evolution beyond plain microservices, and Slack&\#x27;s effort was reportedly triggered by availability-zone outages that exposed the fragility of its previous multi-AZ setup.

<details><summary>References</summary>
<ul>
<li><a href="https://slack.engineering/slacks-migration-to-a-cellular-architecture/">Slack’s Migration to a Cellular Architecture</a></li>
<li><a href="https://www.infoq.com/presentations/slack-cellular-architecture/">Slack&#x27;s Migration to a Cellular Architecture - InfoQ</a></li>
<li><a href="https://docs.aws.amazon.com/wellarchitected/latest/reducing-scope-of-impact-with-cell-based-architecture/what-is-a-cell-based-architecture.html">What is a cell-based architecture? - Reducing the Scope of ...</a></li>

</ul>
</details>

**Tags**: `#distributed-systems`, `#software-architecture`, `#scalability`, `#site-reliability-engineering`, `#engineering-blog`

---

<a id="item-33"></a>
## [Survey examines memory management across 40 major C projects](https://www.reddit.com/r/programming/comments/1xwxhbp/memory_management_in_40_major_c_projects_a_survey/) ⭐️ 6.0/10

A survey analyzing how 40 major C projects approach memory management has been shared on r/programming by user alexeyr. The post presents the survey as an empirical resource covering real-world practices in widely used C codebases. This kind of empirical survey gives systems programmers a reference for how real codebases handle allocation, ownership, and error paths, which can inform code review, library design, and teaching. It also helps surface common conventions that are often tacit knowledge among experienced C developers. The provided Reddit submission contains only a title and link, with no visible summary of the survey’s methodology, project list, or findings. Readers need to consult the linked survey directly to assess its scope, taxonomy, and conclusions.

reddit · r/programming · /u/alexeyr · Nov 15, 14:55

**Background**: C has no garbage collector, so heap memory is typically managed manually through functions such as malloc, calloc, realloc, and free. Developers must track pointer ownership and object lifetimes themselves, and mismatched allocation and deallocation can cause leaks, double frees, or use-after-free bugs. As a result, large C projects often develop conventions around allocator wrappers, ownership rules, and consistent error-handling paths. A cross-project survey can document these practices and make them comparable across codebases.

<details><summary>References</summary>
<ul>
<li><a href="https://en.cppreference.com/c/memory">Dynamic memory management - cppreference.com</a></li>
<li><a href="https://www.geeksforgeeks.org/c/dynamic-memory-allocation-in-c-using-malloc-calloc-free-and-realloc/">Dynamic Memory Allocation in C - GeeksforGeeks</a></li>

</ul>
</details>

**Tags**: `#C`, `#memory management`, `#systems programming`, `#empirical study`, `#software engineering`

---

<a id="item-34"></a>
## [Deep Dive Explains How Profile-Guided Optimization Works Inside the Go Toolchain](https://www.reddit.com/r/programming/comments/1xwz44b/understanding_go_inside_pgo/) ⭐️ 6.0/10

A technical article titled &quot;Understanding Go: inside PGO&quot; was shared on r/programming, walking through how profile-guided optimization is implemented inside the Go toolchain. It explains the mechanics of feeding real runtime profiles back into the compiler rather than treating PGO as a black box. PGO is one of the few remaining levers for squeezing extra performance out of Go binaries without rewriting application code, so understanding its internals helps Go developers and compiler engineers reason about when the 2–7% style gains are worth the extra build step. It also matters for anyone tracking how Go&\#x27;s ahead-of-time compiler narrows the gap with JIT-based runtimes. Go&\#x27;s PGO pipeline collects a CPU profile from a representative production workload \(typically via pprof\), then feeds it back at build time so the compiler can make better inlining and devirtualization decisions and improve code layout. Because the quality of the result depends entirely on how representative the collected profile is, stale or unrepresentative profiles can limit or even negate the benefit.

reddit · r/programming · /u/Charming\_Skin\_8549 · Nov 15, 16:03

**Background**: Profile-guided optimization \(PGO\), also called feedback-directed optimization, is a long-standing compiler technique in which data from actual runs of a program is fed back into the next build. Traditional ahead-of-time compilers must guess which branches are hot and which functions are worth inlining; PGO replaces those guesses with measured behavior, enabling optimizations like aggressive inlining of frequently called small functions, devirtualization of interface or virtual calls, and hot/cold code layout. PGO has been used for years in MSVC, GCC, and Clang/LLVM, and Go added it as a production feature in its 1.20/1.21 releases, with the design documented in a public Go proposal.

<details><summary>References</summary>
<ul>
<li><a href="https://go.dev/doc/pgo">Profile - guided optimization - The Go Programming Language</a></li>
<li><a href="https://go.googlesource.com/proposal/+/master/design/55022-pgo-implementation.md?ref=pangyoalto.com">Proposal: Design and Implementation of Profile - Guided ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Profile-guided_optimization">Profile-guided optimization - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Go`, `#compiler optimization`, `#profile-guided optimization`, `#performance`, `#programming languages`

---

<a id="item-35"></a>
## [Reddit Test Finds ChatGPT and Google AI Mode Invented Nothing Across 18 Fake-Brand Queries](https://www.reddit.com/r/artificial/comments/1xwzvr9/made_up_9_software_brands_and_asked_chatgpt_and/) ⭐️ 6.0/10

A Reddit user \(u/raja314\) invented nine nonexistent software company names — none of which returned any product in a Google search — and on October 19 asked both ChatGPT and Google AI Mode for each brand&\#x27;s price and founder, producing 18 answers in which neither model fabricated a founder or a price. ChatGPT said it could not verify the company existed and asked for a website each time, while Google AI Mode stated the brand did not exist and often pointed to a similarly named real product, such as the cosplay-design company Thimble Forge. One of the original ten names, Corvanta, was dropped because it actually existed \(ChatGPT found an HR-document product and AI Mode an ambulance-software brand\). The experiment offers a concrete counterpoint to the alarmist narrative around AI hallucination, which public leaderboards put anywhere from roughly 1.8% to 77% depending on the task, by showing that on simple, verifiable lookups both systems preferred to decline rather than invent. It also suggests that widely cited hallucination scores — which typically measure document summarization or closed-book deep reasoning — may overstate failure rates for everyday factual queries, a distinction that matters for anyone deciding how much to trust these assistants. The author also ran a control set against 26 real companies: both engines got 19/20 famous companies, 14/14 mid-sized and 14/18 lesser-known ones right on founding year and headquarters, with the misses traced to contradictory sources rather than invention \(for example, Lexalytics&\#x27; HQ given as Amherst by both versus Boston on Wikipedia, and DBmaestro&\#x27;s founding year as 2008 from an Israeli startup database versus 2012 on Wikipedia\). On pricing, 16/16 headline prices for the cheapest paid plan of eight SaaS tools matched the vendor page, and the only misses involved monthly-vs-annual billing toggles. The author stresses the caveats: 18 queries, one US location, one day, one correct answer per question, and no tests of complex tasks like product integrations or tool comparisons.

reddit · r/artificial · /u/raja314 · Nov 15, 16:33

**Background**: AI hallucination refers to a language model confidently producing false information — a fabricated founder, price, or citation — rather than admitting uncertainty. Public hallucination leaderboards such as Vectara&\#x27;s HHEM-based ranking measure how often models do this when summarizing a supplied document, which is a very different task from answering a short factual question with web access. Google AI Mode is Google Search&\#x27;s generative answering experience, powered by Gemini models that can reason over and synthesize results from live web sources, while ChatGPT with browsing/search similarly grounds answers in retrieved pages.

<details><summary>References</summary>
<ul>
<li><a href="https://search.google/ways-to-search/ai-mode/">Google AI Mode - a new way to search , whatever’s on your mind</a></li>
<li><a href="https://github.com/vectara/hallucination-leaderboard/">GitHub - vectara/hallucination-leaderboard: Leaderboard ...</a></li>

</ul>
</details>

**Tags**: `#AI hallucination`, `#LLM evaluation`, `#ChatGPT`, `#Google AI Mode`, `#AI reliability`

---