---
layout: default
title: "Horizon Summary: 2026-11-24 (EN)"
date: 2026-11-24
lang: en
---

> From 25 items, 15 important content pieces were selected

---

1. [Nvidia Board Reinstates Jensen Huang as CEO After U.S. Government Input](#item-1) ⭐️ 9.0/10
2. [Anthropic&\#x27;s Lean Repo Claims Machine-Verified Proof That VP ≠ VNP](#item-2) ⭐️ 9.0/10
3. [Zhipu AI Ships GLM-5.4, Its First Flagship Built on a Loop Transformer](#item-3) ⭐️ 9.0/10
4. [Ladybird&\#x27;s from-scratch browser engine ships first alpha for macOS and Linux](#item-4) ⭐️ 8.0/10
5. [Arm Forces Shutdown of Unofficial Arm Documentation Mirror by December 2026](#item-5) ⭐️ 7.0/10
6. [NariQ ships 3-bit Qwen3.8-27B GGUF claimed to match BF16](#item-6) ⭐️ 7.0/10
7. [Kagi launches public beta of AI-integrated Kagi Mail](#item-7) ⭐️ 7.0/10
8. [Nospeaker turns MacBook&\#x27;s trackpad haptic motor into a speaker](#item-8) ⭐️ 7.0/10
9. [Spelunkr.tv Turns the Internet Archive&\#x27;s Forgotten Videos Into a Free Cable-Style TV Network](#item-9) ⭐️ 7.0/10
10. [Apple Pulls Open-Source FSNotes From EU App Stores Over Lapsed DSA Trader Status](#item-10) ⭐️ 7.0/10
11. [Ai2 releases RoboTrack benchmark and models for robot point tracking](#item-11) ⭐️ 7.0/10
12. [LeCun Accuses Anthropic&\#x27;s Dario Amodei of Hyping AI Risk to Ban Open Weights](#item-12) ⭐️ 6.0/10
13. [Win4wine Runs Windows Explorer Shell as a Linux Desktop on Wine](#item-13) ⭐️ 6.0/10
14. [Dutch court bans BYD Ti7 across the EU over Defender design](#item-14) ⭐️ 6.0/10
15. [datasette-charts 0.1a0 adds whole-dataset charting to Datasette, prototyped with Claude](#item-15) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Nvidia Board Reinstates Jensen Huang as CEO After U.S. Government Input](https://www.cnbc.com/2026/11/23/nvidia-jensen-huang-ceo.html) ⭐️ 9.0/10

Nvidia&\#x27;s board reinstated Jensen Huang as president, CEO, and board director, reversing a decision made less than two weeks earlier, and stated that it had received input from senior levels of the United States government before concluding that his reinstatement poses no national security risk. The company announced the move in a press release, with CNBC reporting that Congress and the Trump administration were involved in the discussions. The reversal is extraordinary for a company of Nvidia&\#x27;s size and puts a spotlight on how far U.S. national security policy now reaches into the governance of critical semiconductor firms. It affects investors, customers and supply-chain partners who depend on Nvidia&\#x27;s AI chips, and it raises questions about board independence at a time when AI hardware is treated as a strategic asset. According to the company&\#x27;s statement, the board&\#x27;s decision was informed by U.S. government input and explicitly framed around national security risk rather than an internal findings process. Community discussion notes that the board reportedly reached the decision unanimously despite having moved quickly to remove Huang, and commenters point to Delaware&\#x27;s Caremark precedent as setting a very high bar for holding directors personally liable for oversight failures.

hackernews · jaz · Nov 23, 14:00 · [Discussion](https://news.ycombinator.com/item?id=50611576)

**Background**: Jensen Huang co-founded Nvidia in 1993 and had led it as CEO ever since, building it into the dominant supplier of GPUs used for AI training and inference. Under Delaware corporate law, where Nvidia is incorporated, directors owe duties of loyalty and oversight; the Caremark line of cases makes it very hard for shareholders to win claims that a board failed in that oversight role. Nvidia sits at the center of U.S. export-control policy because advanced AI accelerators are considered strategically sensitive, which is why government views can carry weight in decisions about the company&\#x27;s leadership.

**Discussion**: Commenters focused on the statement&\#x27;s line about receiving input from senior U.S. government officials, calling it the most telling part of the announcement, and debated whether it signals political pressure or a genuine national security clearance. Several questioned the board&\#x27;s handling of the episode as needlessly disruptive and hypocritical given pressure on ASML and Japanese chip firms to follow China sanctions, while others argued there is no public evidence of wrongdoing and that the government&\#x27;s assessment is probably correct.

**Tags**: `#Nvidia`, `#Jensen Huang`, `#corporate governance`, `#national security`, `#semiconductors`

---

<a id="item-2"></a>
## [Anthropic&\#x27;s Lean Repo Claims Machine-Verified Proof That VP ≠ VNP](https://github.com/anthropics/formal-math/tree/main/vp-vnp) ⭐️ 9.0/10

Anthropic&\#x27;s formal-math GitHub repository now hosts a Lean formalization together with an accompanying paper \(a PDF pinned at a specific commit\) claiming a proof that VP ≠ VNP over every field. This is a separation of Valiant&\#x27;s algebraic complexity classes, a question that has remained open since it was posed in 1979. VP vs VNP is widely described as the algebraic analogue of P vs NP, so a proven separation over all fields would be a landmark result in algebraic complexity theory and a rare proven circuit lower bound. That it comes with a machine-checked Lean proof, from an AI lab&\#x27;s formal-math repository, also makes it a notable data point for AI-assisted and formally verified mathematical research. The paper explicitly acknowledges a gap, stating that the authors have not analysed how the result relates to relativization and algebrization \(BGS75, AW09\), the standard barrier results for complexity lower bounds. The repository also pins the paper at a specific commit hash, and the community has pointed to third-party tooling for browsing the Lean source without building the project locally.

hackernews · mikeryan52 · Nov 23, 22:09 · [Discussion](https://news.ycombinator.com/item?id=50620102)

**Background**: In 1979 Leslie Valiant defined VP and VNP as algebraic analogues of P and NP: instead of decision problems, one studies families of polynomials computed by arithmetic circuits, with VP roughly being polynomials computable by small circuits and VNP those whose coefficients can be efficiently verified. The permanent is the canonical VNP-complete polynomial, and the determinant sits in VP, so VP vs VNP asks whether every efficiently verifiable polynomial family really needs large circuits. Lean is a functional programming language and theorem prover built for formalizing mathematics and formal verification, where proofs are checked by a small trusted kernel.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Arithmetic_circuit_complexity">Arithmetic circuit complexity - Wikipedia</a></li>
<li><a href="https://lean-lang.org/learn/">Learn — Lean Lang</a></li>
<li><a href="https://www.anthropic.com/research/formalizing-fermats-last-theorem">Formalizing Fermat&#x27;s Last Theorem \ Anthropic</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread \(160 points, 112 comments\) mixes technical scrutiny with field-level commentary: some read this as Anthropic throwing everything at the P vs NP holy grail and publishing a worthwhile partial result along the way, while others raise the paper&\#x27;s admitted lack of analysis around relativization and algebrization. Several commenters express anxiety about what such results mean for mathematics research careers, and others frame the moment as a Great Game-style contest between Anthropic and OpenAI.

**Tags**: `#complexity theory`, `#formal verification`, `#Lean`, `#AI for mathematics`, `#algebraic complexity`

---

<a id="item-3"></a>
## [Zhipu AI Ships GLM-5.4, Its First Flagship Built on a Loop Transformer](https://z.ai/blog/glm-5.4) ⭐️ 9.0/10

Z.ai \(Zhipu AI\) released GLM-5.4, its first flagship model built on a Loop Transformer architecture, claiming intelligence levels comparable to 2T–3T parameter models. The coding-focused release also adds visual understanding and extends code generation into video production, game development, 3D modeling and mechanical design, a direction the company calls &quot;Generalized Coding.&quot; A Loop Transformer reuses the same block of layers repeatedly instead of stacking a fresh set of weights for every layer, so a model can effectively &quot;think deeper&quot; without growing its parameter count or memory footprint. If the approach scales, it could ease the memory-bandwidth bottleneck that dominates inference cost and shift competition among frontier labs from raw size toward recurrent depth. Z.ai acknowledges the model still has some limitations, and early users report access friction: the model was not available through OpenRouter or the standard Z.ai API plan, requiring a switch to the Coding Plan whose API keys work identically but unlock the new model. The release lands alongside other looped-architecture launches, including Thinking Machines&\#x27; Inkling 2 Mini on November 20.

hackernews · foohis · Nov 23, 10:06 · [Discussion](https://news.ycombinator.com/item?id=50609685)

**Background**: A standard Transformer is a stack of layers, each holding its own weights; at inference every layer is loaded from high-bandwidth memory \(HBM\) onto the chip, computed once, and swapped out, which makes memory bandwidth the main bottleneck for token generation. A Loop Transformer — also called looped depth sharing or recurrent depth — applies the same transformer block several times per token, so hidden states from one pass feed the next while some layers are reused. Z.ai, formerly Zhipu AI, is a Tsinghua University spin-off founded in 2019 whose GLM family is its flagship model line and has been released under the MIT license since July 2025.

<details><summary>References</summary>
<ul>
<li><a href="https://z.ai/blog/glm-5.4">GLM-5.4: Toward Generalized Coding with Our First Loop ... - z.ai</a></li>
<li><a href="https://sebastianraschka.com/llm-architecture-gallery/looped-depth-sharing/">Looped Transformer | Sebastian Raschka, PhD</a></li>
<li><a href="https://docs.z.ai/guides/llm/glm-5.4">GLM-5.4 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread \(1,024 points, 334 comments\) is broadly positive about Z.ai&\#x27;s technical transparency, which commenters contrast favorably with the locked-down approach of Western labs, and several praise looped transformers as an obvious next direction. The main pushback concerns inference behavior: users complain that Chinese models run long &quot;marathon thinking&quot; sessions, second-guessing themselves even on simple tasks and making time-to-completion much higher than frontier models. Others flag practical friction, noting the model was reachable only through the Coding Plan rather than OpenRouter or the standard API.

**Tags**: `#LLM`, `#loop transformer`, `#GLM-5.4`, `#coding models`, `#AI research`

---

<a id="item-4"></a>
## [Ladybird&\#x27;s from-scratch browser engine ships first alpha for macOS and Linux](https://ladybird.org/posts/alpha/) ⭐️ 8.0/10

The Ladybird project has released its first alpha builds for macOS and Linux, opening its from-scratch browser engine to early adopters after roughly four years of independent development. The release marks the project&\#x27;s transition out of its long pre-alpha phase, in which it was described as suitable only for developers. Almost every mainstream browser today runs on Chromium, WebKit or Gecko, so a genuinely independent engine reaching a testable alpha is a rare event for web standards diversity. It offers an alternative to Google-dominated browser infrastructure and gives web developers a new engine to validate compatibility against. The alpha is available only for macOS and Linux, and the team explicitly positions it for early adopters willing to report bugs rather than for daily use. Ladybird is also upfront about security shortcomings at this stage, and the engine has been reworked around production-grade dependencies such as SQLite and Skia instead of the project&\#x27;s earlier in-house libraries.

hackernews · janvdberg · Nov 23, 16:13 · [Discussion](https://news.ycombinator.com/item?id=50614249)

**Background**: Ladybird began as a browser component inside SerenityOS, the hobby operating system created by Andreas Kling, before spinning off into a standalone project run by the non-profit Ladybird Browser Initiative. The initiative is funded entirely by donations and sponsors including Cloudflare, FUTO, Shopify, Proton and 37signals, and the code is released under the BSD 2-Clause license. Its defining characteristic is that the engine is written from the ground up rather than forked from Blink, WebKit or Gecko.

<details><summary>References</summary>
<ul>
<li><a href="https://ladybird.org/posts/alpha/">Ladybird is now in alpha - Ladybird</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ladybird_%28web_browser%29">Ladybird (web browser ) - Wikipedia</a></li>
<li><a href="https://www.techpowerup.com/355140/independent-web-browser-engine-ladybird-goes-into-alpha-release">Independent Web Browser/Engine &quot;Ladybird&quot; Goes Into Alpha ...</a></li>

</ul>
</details>

**Discussion**: Hacker News reaction was overwhelmingly positive, with users reporting that real-world sites such as YouTube, Google Maps, Proxmox&\#x27;s NoVNC console and heavy news pages render correctly, some even faster than in Firefox. The main complaints were minor: noticeably jerky scrolling and some lag on complex sites. Commenters also debated the tradeoff of replacing in-house libraries with production-grade dependencies, voiced nostalgia for the original SerenityOS hacker spirit, and asked what precautions to take given the alpha&\#x27;s acknowledged security gaps.

**Tags**: `#web browsers`, `#browser engines`, `#Ladybird`, `#open source`, `#alpha release`

---

<a id="item-5"></a>
## [Arm Forces Shutdown of Unofficial Arm Documentation Mirror by December 2026](https://arm.jonpalmisc.com/) ⭐️ 7.0/10

The maintainer of arm.jonpalmisc.com, an unofficial but widely used mirror of Arm&\#x27;s AArch64 instruction-set and system-register reference documentation, announced that the site will be discontinued on 4 December 2026 at Arm&\#x27;s request. According to the maintainer, Arm&\#x27;s notice asserts that hosting the documentation infringes its trademarks and intellectual property. For many Arm developers this mirror was a faster, ad-free, easily linkable alternative to Arm&\#x27;s own documentation portal, so its removal directly degrades day-to-day reference lookup for people writing AArch64 code. The episode has also become a flashpoint over how far trademark and IP claims can go in restricting access to documentation for publicly sold hardware, with the community already discussing mirrors and a tool-only release. The maintainer said Arm&\#x27;s trademark and IP claims are hard to work around while keeping the site useful, and that people have offered to host mirrors, suggested he lawyer up, or proposed releasing the site-generating source code without Arm&\#x27;s IP so users can build the same reference locally. One commenter also noted that Arm&\#x27;s Machine Readable Architecture Specification \(MRAS\) appears to be distributed under a BSD-style license, which may complicate the IP argument.

hackernews · tech234a · Nov 23, 19:17 · [Discussion](https://news.ycombinator.com/item?id=50617499)

**Background**: Arm is a UK-based company that designs CPU cores and instruction-set architectures and licenses them to chipmakers, and its architecture reference manuals document instruction sets such as AArch64 \(the 64-bit Arm ISA used in Armv8-A and Armv9-A\) along with system registers and related details. Arm publishes this material through its own developer portal and support site, and it separately maintains trademark use guidelines that restrict how its names and marks may be used in publications and on websites. Because official documentation can be gated, hard to navigate, or split across many PDFs, third parties have long built unofficial conversions and mirrors that are easier to search and link to.

<details><summary>References</summary>
<ul>
<li><a href="https://www.arm.com/company/policies/trademarks/guidelines-trademarks">Trademark use guidelines – Arm®</a></li>
<li><a href="https://en.wikipedia.org/wiki/ARM_architecture_family">ARM architecture family - Wikipedia</a></li>
<li><a href="https://github.com/MattPD/cpplinks/blob/master/assembly.arm.md">cpplinks/assembly. arm .md at master · MattPD/cpplinks · GitHub</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters overwhelmingly criticized the takedown as legal overreach, arguing that documenting publicly sold hardware should be fair use and that such actions only make life harder for the developers who provide value to Arm. Several questioned the legal basis, pointing to Arm&\#x27;s BSD-licensed Machine Readable Architecture Specification and asking whether other unofficial AArch64 references are generated by the same conversion tooling, while one top comment argued lawyers should have to get sign-off from someone who understands the business.

**Tags**: `#intellectual-property`, `#arm`, `#documentation`, `#trademark`, `#hardware`, `#open-access`

---

<a id="item-6"></a>
## [NariQ ships 3-bit Qwen3.8-27B GGUF claimed to match BF16](https://huggingface.co/nari-labs/Qwen3.8-27B-NariQ-GGUF) ⭐️ 7.0/10

NariQ released 3-bit, 2.5-bit and 2-bit GGUF quantizations of Qwen3.8-27B, claiming to be the first sub-3-bit quantization that retains BF16-level performance on long-horizon agentic tasks. In their own benchmarks the 3-bit build roughly matches or slightly exceeds the BF16 control on DeepSWE \(41.0 vs 39.8\), Terminal-Bench 2.1 \(63.8 vs 62.6\), AIME 25+26 \(98.3 vs 97.7\), MSGM and RealWorldQA, all inside a roughly 10 GB file. If the results hold, a 27B model with agentic, math, multilingual and vision abilities could run in about 10 GB, putting it within reach of 16 GB consumer laptops and single consumer GPUs rather than datacenter hardware. That significantly lowers the hardware floor for locally hosted capable agents, in a quantization space where sub-4-bit models have historically degraded badly on long multi-step tasks. Quality holds at 3-bit and 2.5-bit but the 2-bit build degrades sharply \(DeepSWE 39.8 to 28.6, AIME 97.7 to 86.0, Terminal-Bench 62.6 to 52.4\), and running these files currently requires NariQ&\#x27;s own llama.cpp fork. Decode speed is comparable to other quants on an RTX PRO 6000 but falls to about 3.8 tok/s at 3.0 bpw on an 18 GB M3 Pro, and NariQ is described as a trellis-coded post-training quantization calibrated on real coding-agent traces.

hackernews · toebee · Nov 23, 13:42 · [Discussion](https://news.ycombinator.com/item?id=50611402)

**Background**: Quantization stores model weights at lower numerical precision to shrink memory footprint and speed up inference; BF16 \(bfloat16\) is the 16-bit baseline these models are usually trained and evaluated in. GGUF is the file format used by llama.cpp, with named levels such as Q4\_K\_M, Q5\_K\_S and IQ2\_XS that trade size against quality, and most users consider 4-bit the practical floor before quality drops off. Because a 27B model needs roughly 3 bits per weight to fit into ~10 GB, NariQ is pushing well below that conventional floor, which matters most for agentic workloads where small per-step errors accumulate over long horizons.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/nari-labs/Qwen3.8-27B-NariQ-GGUF">nari -labs/Qwen3.8-27B- NariQ -GGUF · Hugging Face</a></li>
<li><a href="https://news.ycombinator.com/item?id=50611402">NariQ : BF16-level Qwen3.8-27B in a 10 GB file | Hacker News</a></li>
<li><a href="https://canitrun.dev/guides/quantization-explained/">GGUF Quantization Explained: Q4, Q5, Q6, Q8 Compared</a></li>

</ul>
</details>

**Discussion**: Commenters were genuinely positive that the authors tested several families of held-out long-horizon tasks instead of coding alone, which is exactly the check usually missing from high-compute quantization efforts. Skepticism centered on two points: one commenter asked what information is actually lost at 2-3 bits per weight, since benchmarks cannot cover everything in the training data, and others found it concerning that the BF16 control model scored so much better in NariQ&\#x27;s harness than in Unsloth&\#x27;s numbers, suggesting much of the apparent gain comes from harness differences rather than the quantization itself. The ~3.8 tok/s decode speed on an M3 Pro was also noted as far slower than CUDA.

**Tags**: `#quantization`, `#local-llm-inference`, `#qwen`, `#gguf`, `#model-compression`

---

<a id="item-7"></a>
## [Kagi launches public beta of AI-integrated Kagi Mail](https://blog.kagi.com/kagi-mail-public-beta) ⭐️ 7.0/10

Kagi, the subscription-based privacy-focused search engine, has opened a public beta of Kagi Mail, a private email and calendar service that works with a @kagimail.com address or your own custom domains. The launch positions AI assistance as the product&\#x27;s headline feature and extends Kagi&\#x27;s ecosystem beyond search and its Orion browser. Email is the last major piece of many privacy-conscious users&\#x27; digital lives still hosted by Google, so a Kagi inbox directly targets the same audience that already pays for search — and puts Kagi in competition with established providers like Fastmail and Proton. It also marks a philosophical shift for a company whose reputation rested on storing as little user data as possible. According to Kagi&\#x27;s documentation, Kagi Mail automatically strips many tracking pixels and proxies images through the Kagi image proxy, and this applies across all email clients used to access the account. Community members cite a roughly $100/year price versus about $60/year for Fastmail, and the AI features are opt-in in the sense that users must consciously grant a cloud LLM access to their mail.

hackernews · rdmuser · Nov 23, 17:17 · [Discussion](https://news.ycombinator.com/item?id=50615481)

**Background**: Kagi is a paid, ad-free search engine that sells subscriptions instead of advertising, and it has built a reputation for minimizing data collection — for example, keeping no search history by default. It also develops the Orion browser, and its docs describe Kagi Mail as a premium email service designed to integrate with the wider Kagi ecosystem. Privacy-oriented email is an established niche dominated by providers such as Fastmail and Proton, which is the benchmark commenters used to judge the new offering.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.kagi.com/kagi-mail-public-beta">Kagi Blog - Kagi Mail is here (Public Beta)</a></li>
<li><a href="https://help.kagi.com/kagi/mail/faq.html">Kagi Mail FAQ | Kagi&#x27;s Docs</a></li>
<li><a href="https://help.kagi.com/kagi/mail/">Kagi Mail FAQ | Kagi&#x27;s Docs</a></li>

</ul>
</details>

**Discussion**: Hacker News reaction was largely skeptical: long-time Kagi customers said Fastmail is already good enough and that they would never let a cloud LLM read their email, while others worried about feature creep as quality slips in existing products like Kagi Translate. Several commenters flagged the shift away from Kagi&\#x27;s low-data-retention identity as a notable paradigm change, and the ~$100/year price was called out as too high relative to Fastmail.

**Tags**: `#Kagi`, `#email`, `#privacy`, `#AI`, `#product-launch`

---

<a id="item-8"></a>
## [Nospeaker turns MacBook&\#x27;s trackpad haptic motor into a speaker](https://github.com/os6/nospeaker) ⭐️ 7.0/10

Developer os6 released nospeaker, an open-source tool that drives the haptic actuator inside Apple&\#x27;s Force Touch trackpad at rates of up to 4,000 times per second, making the trackpad surface itself vibrate fast enough to emit speech, tones and even music. Because Apple&\#x27;s public haptics API only exposes three fixed taps, the tool bypasses it and talks to the motor through the private MultitouchSupport framework instead. It is a neatly self-contained hardware hack that shows how much unused capability sits behind a tightly locked-down Apple component: a part designed purely to fake a click can double as a crude speaker with no hardware modification at all. Beyond the novelty, it is a useful case study for anyone interested in how haptic actuators are driven and in the reverse-engineering of private macOS frameworks. The tool requires a Force Touch trackpad — MacBooks from 2015 onward, or a Magic Trackpad 2 and later — plus macOS 12+ on Apple Silicon or macOS 13+ on Intel, and output is quiet, robotic and obviously limited in fidelity compared with real speakers. A demo clip of the effect was shared on the author&\#x27;s X account, and using private frameworks means it can break with any macOS update.

hackernews · yakkomajuri · Nov 23, 11:31 · [Discussion](https://news.ycombinator.com/item?id=50610318)

**Background**: Apple&\#x27;s Force Touch trackpad does not actually move when you click; instead a haptic actuator vibrates the glass to simulate the sensation of a physical button press. The same actuator is normally fed carefully shaped waveforms, and Apple&\#x27;s public API exposes only a few canned tap patterns, which is why reaching audio frequencies required going through a private framework. Making a vibration motor play recognizable audio is an old hobbyist tradition, most famously the Commodore 1541 floppy drive whose stepper motor could be coaxed into playing music.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/os6/nospeaker">os6/nospeaker: make your macbook&#x27;s trackpad talk using its haptic ...</a></li>
<li><a href="https://www.notebookcheck.net/New-free-open-source-tool-turns-your-MacBook-s-haptic-motor-not-its-speakers-into-a-voice.1457489.0.html">New free open-source tool turns your MacBook&#x27;s haptic motor ...</a></li>
<li><a href="https://www.macworld.com/article/3294451/trick-turns-macbooks-force-touch-trackpad-into-audio-speaker.html">This insane trick turns the MacBook’s trackpad into a speaker</a></li>

</ul>
</details>

**Discussion**: Commenters were impressed but split on what was more remarkable: several argued that a motionless slab feeling like a real button press is the greater feat than the audio trick itself. Others traced the lineage to Commodore 1541 floppy-drive music and to the piezoelectric PC speakers of the 1980s and 90s, with one engineer wondering whether Apple&\#x27;s sum-of-sines motor API exists to prevent burnout, to enable simple feed-forward compensation of the actuator&\#x27;s dynamics, or simply to keep the USB/HID stream low-bandwidth.

**Tags**: `#hardware-hacking`, `#haptics`, `#macbook`, `#reverse-engineering`, `#audio`

---

<a id="item-9"></a>
## [Spelunkr.tv Turns the Internet Archive&\#x27;s Forgotten Videos Into a Free Cable-Style TV Network](https://spelunkr.tv/) ⭐️ 7.0/10

Spelunkr.tv is a free, browser-based retro cable TV simulator that stitches roughly 34 always-on channels out of the Internet Archive&\#x27;s obscure and largely forgotten video collections, so every channel is already partway through a broadcast when you tune in. The project, which needs no account or payment, also offers a TV app that puts the same program guide on your television, and it drew 924 points and 160 comments after being posted to Hacker News. The project is less a technical breakthrough than a cultural one: it reintroduces the shared, linear broadcast experience that on-demand streaming has largely erased, where everyone is watching the same thing at the same moment. It also gives a second life to the Internet Archive&\#x27;s long-tail of unviewed media, suggesting that preservation can be packaged as entertainment rather than a catalogue nobody browses. All channels run synchronously for everyone, so you cannot pause, rewind or choose an episode — that constraint is precisely the point. The TV app is essentially the website shown full screen in TV form, with the guide launched from the TV&\#x27;s home screen and driven by its remote, and users report that casting from a phone turns the handset into a remote; new channels are added routinely.

hackernews · SockThief · Nov 23, 01:13 · [Discussion](https://news.ycombinator.com/item?id=50606192)

**Background**: The Internet Archive is a non-profit digital library whose moving-image collections include large amounts of public-domain, orphaned and poorly catalogued film and television, much of it rarely watched. A &quot;linear&quot; or FAST-style channel interface — familiar from services like Pluto TV or hobby projects such as FieldStation42 — presents video as a scheduled stream you flip through rather than as an on-demand catalogue you search. Spelunkr applies that model to archive footage, which means viewers experience the material the way old cable TV delivered it: joined mid-scene, with vintage ads and interstitials intact.

<details><summary>References</summary>
<ul>
<li><a href="https://spelunkr.tv/app">spelunkr on your TV — SPELUNKR</a></li>
<li><a href="https://spelunkertv.online/">Spelunkr TV — 34 Channels of 24/7 Retro Cable TV, Free</a></li>
<li><a href="https://streamfree.tv/services/spelunkr">Spelunkr — Retro Cable TV Simulator &amp; Lost Media</a></li>

</ul>
</details>

**Discussion**: Commenters were overwhelmingly enthusiastic: one said the site had occupied an entire night and singled out the phone-as-remote casting experience, while others pitched curated channel ideas such as an archive of &quot;2am theater&quot; drive-in double features complete with snack-bar ads and trailers. Several shared nostalgia hits \(a 1987 Headbangers Ball block, a Spuds McKenzie commercial between Def Leppard and Mötley Crüe videos\), and one commenter offered a thoughtful reflection that on-demand streaming&\#x27;s asynchronous temporality produces a faint background hum of loneliness, since nobody else is watching the same thing at that moment. Another described building a similar Raspberry Pi 5 setup inside a gutted cable box using FieldStation42.

**Tags**: `#internet-archive`, `#streaming`, `#media-preservation`, `#side-project`, `#hackernews`

---

<a id="item-10"></a>
## [Apple Pulls Open-Source FSNotes From EU App Stores Over Lapsed DSA Trader Status](https://github.com/glushchenko/fsnotes/discussions/2056) ⭐️ 7.0/10

Oleksandr Hlushchenko, developer of the open-source macOS notes app FSNotes, reported that Apple removed his app from EU App Stores after nine years of distribution. The removal stemmed from his EU Digital Services Act \(DSA\) &quot;verified trader&quot; status having lapsed, with the Dutch App Store listing reportedly showing a message that the developer had not identified himself as a merchant for the app. The case illustrates how EU platform-compliance rules can silently take down long-standing apps, including free and open-source ones, and it lands as a practical warning for indie developers who must keep regulatory paperwork current to stay listed. It also fuels the broader debate over how much support and transparency Apple owes developers when automated compliance enforcement removes their livelihood. Commenters noted the app remained available in the US and UK stores, indicating an EU-specific enforcement action rather than a takedown of the app itself, and pointed out that trader verification is not a one-time step — it can lapse for mundane reasons such as a changed address. Others observed that FSNotes has a paid App Store version and that the developer had years to complete verification, while one developer reported waiting about a month for EU DSA approval on a new app amid heavier App Review load.

hackernews · fluder · Nov 23, 18:48 · [Discussion](https://news.ycombinator.com/item?id=50616933)

**Background**: The EU Digital Services Act \(DSA\) requires platforms such as Apple to verify and display contact information — address, phone number and email — for &quot;traders&quot; distributing apps to EU users, under Articles 30 and 31. Since March 2024, Apple has asked Account Holders and Admins in the Apple Developer Program to declare their trader status in App Store Connect, and traders may be asked for documentation proving that status. The distinction matters in practice: apps classified as traders must show contact details on their EU store listing, and failure to verify can result in removal from EU storefronts.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.apple.com/help/app-store-connect/manage-compliance-information/manage-european-union-digital-services-act-trader-requirements/">Manage European Union Digital Services Act trader requirements</a></li>
<li><a href="https://developer.apple.com/news/?id=x60uzbu9">Provide your trader status in App Store Connect - Apple Developer</a></li>
<li><a href="https://support.aiir.com/article/1127-trader-status">Apple or Google is asking for my &#x27;trader status&#x27;. What does ...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters largely pushed back on the framing that open-source status caused the removal, tracing it to a lapsed trader verification and linking to corroborating reports of a known Apple bottleneck in processing DSA paperwork. Some criticized the developer for waiting nine years and for listing a paid app while ignoring the law, while others condemned opaque enforcement and complained that public upvotes now effectively act as an entry barrier for official customer support.

**Tags**: `#apple-app-store`, `#eu-dsa-regulation`, `#platform-policy`, `#indie-development`, `#app-distribution`

---

<a id="item-11"></a>
## [Ai2 releases RoboTrack benchmark and models for robot point tracking](https://huggingface.co/blog/allenai/robotrack) ⭐️ 7.0/10

The Allen Institute for AI \(Ai2\) released RoboTrack, a benchmark and training-data suite for point tracking in real-world robotic manipulation, built on MolmoSpaces, with the RoboTrack-15M dataset generating point tracks for training alongside two tracking models. Ai2 reports that its RoboTracker model completed 17 of 20 wet-lab pipetting tasks, demonstrating the approach on a real manipulation workflow. Point tracking is a core perception capability for vision-based robot control, but most trackers are trained and evaluated on generic internet video rather than cluttered manipulation scenes. A dedicated robotic benchmark plus a large training suite gives the field a shared yardstick and could improve closed-loop control, imitation learning, and sim-to-real transfer for manipulation research. RoboTrack provides both simulated and real-world robotic datasets with dense ground-truth point tracks, and supports training and evaluation of multiple tracking architectures including CoTracker3, TAPNext, and AllTracker. The headline real-world result is a 17-of-20 success rate on wet-lab pipetting, a narrow but demanding precision task rather than a broad generalization claim.

rss · HuggingFace Blog · Nov 23, 17:20

**Background**: Point tracking is the computer-vision task of following specific points \(typically pixels on an object\) consistently across the frames of a video, which lets a system reason about how objects move even without explicit 3D models. It is widely used in augmented reality and robotics, and a common failure mode is drift, where a tracked point slips off its object onto the background or another object. Robotic manipulation — grasping, pouring, pipetting — needs such tracks to be accurate over long horizons under occlusion and clutter.

<details><summary>References</summary>
<ul>
<li><a href="https://allenai.org/blog/robotrack">RoboTrack: Point tracking for real-world robotic manipulation</a></li>
<li><a href="https://www.unite.ai/ai2-releases-robotrack-to-test-and-train-robot-point-trackers/">Ai2 Releases RoboTrack to Test and Train Robot Point ...</a></li>
<li><a href="https://github.com/robotrack24/RoboTrack">GitHub - robotrack24/RoboTrack: Benchmark and Data for Point ...</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#point tracking`, `#manipulation`, `#computer vision`, `#AI research`

---

<a id="item-12"></a>
## [LeCun Accuses Anthropic&\#x27;s Dario Amodei of Hyping AI Risk to Ban Open Weights](https://twitter.com/ylecun/status/2124550037912920090) ⭐️ 6.0/10

Yann LeCun posted on X that Dario Amodei&\#x27;s arguments since the GPT-2 era have consistently hyped AI dangers so that open models would be made illegal and he would remain in control, comparing it to the Ottoman Empire banning the Arabic printing press to protect dogma. The post sparked a large Hacker News thread with roughly 995 points and 579 comments debating regulatory capture and open-weight AI. The spat crystallizes a live policy question: whether safety arguments from closed frontier labs end up shaping rules that entrench incumbents and lock out open-weight competitors. The outcome will affect open-source AI developers, startups building on downloadable models, and how governments write AI regulation in the coming years. The underlying post is a short opinion tweet with no technical substance, and much of the thread is heated speculation rather than evidence. The more substantive comments describe informal regulatory chatter about how one might practically restrict open weights, such as pressuring AMD and Nvidia to ship microcode updates limiting consumer GPUs&\#x27; ability to run LLMs, or requiring registration of privately owned compute.

hackernews · MrBuddyCasino · Nov 23, 17:07 · [Discussion](https://news.ycombinator.com/item?id=50615308)

**Background**: Open-weight models release their trained parameters so anyone can download and run them, but typically without the training data or full training code — which is why researchers distinguish them from genuinely open-source AI. Frontier models are the most capable general-purpose models of the moment, usually produced by a handful of well-funded labs such as Anthropic, which was founded by former OpenAI researchers including Dario Amodei. Regulatory capture describes the dynamic in which the companies being regulated end up shaping the rules, potentially using safety or compliance requirements to raise barriers for smaller rivals.

<details><summary>References</summary>
<ul>
<li><a href="https://www.laurenceo.com/intelligence/glossary/frontier-ai-model">What Is Frontier AI model ? Definition and Why It Matters</a></li>
<li><a href="https://blog.grvpanchal.me/2026/05/frontier-models-to-build-harnesses-not.html">Gaurav Panchal&#x27;s Blog: Frontier models to build Harnesses not...</a></li>

</ul>
</details>

**Discussion**: Sentiment in the thread runs strongly against Amodei, with commenters framing closed labs as having appropriated the world&\#x27;s public knowledge and open research and now lobbying to stop others from doing the same. Others push back on the pure conflict-of-interest framing: one commenter argues that highlighting Dario&\#x27;s motives is not enough and that open-weight advocates need a concrete proposal for mitigating safety risks, while another points to the Hugging Face incident as proof that without open models there is no defense against attacks from frontier closed models.

**Tags**: `#AI policy`, `#open-weight models`, `#regulatory capture`, `#AI safety debate`, `#open source`

---

<a id="item-13"></a>
## [Win4wine Runs Windows Explorer Shell as a Linux Desktop on Wine](https://github.com/mikuta0407/win4wine) ⭐️ 6.0/10

Developer mikuta0407 published win4wine, a hobbyist project that launches the classic Windows Explorer shell \(explorer.exe\) on top of the Wine compatibility layer and uses it as the desktop environment on Linux. The repository surfaced on Hacker News, where it drew 208 points and roughly 110 comments debating the approach. The project is more of a curiosity than a practical alternative, but it is a vivid demonstration of how far Wine&\#x27;s Win32 and shell coverage has come, and it raises real questions about where the boundary between the Windows NT kernel, Win32 APIs and the UI layer actually sits. It also highlights a broader trend of Linux users recreating familiar Windows interfaces rather than adopting native desktops. Because it reuses legacy explorer.exe from Windows XP or Windows 7 era binaries, the desktop inherits those versions&\#x27; unpatched vulnerabilities, and users must supply the Windows files themselves rather than downloading them with the project. On the plus side, running the real shell means Windows-only utilities such as AutoHotkey can work inside the Linux desktop session.

hackernews · hard\_times · Nov 23, 12:28 · [Discussion](https://news.ycombinator.com/item?id=50610743)

**Background**: Wine \(originally &quot;Wine Is Not an Emulator&quot;\) is an open-source compatibility layer that translates Windows API calls into native POSIX calls on Linux, macOS and BSD, letting Windows binaries run without a virtual machine. In Windows, explorer.exe is not only the file manager but also the default shell that draws the taskbar, desktop icons and Start menu. A Linux desktop environment normally consists of a window manager plus a panel and file manager, so pointing a session at explorer.exe running under Wine effectively swaps out the whole shell.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wine_%28software%29">Wine (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/File_Explorer">File Explorer - Wikipedia</a></li>
<li><a href="https://www.winehq.org/">WineHQ - Run Windows applications on Linux, BSD, Solaris and...</a></li>

</ul>
</details>

**Discussion**: Commenters broadly agreed that Windows&\#x27; strengths lie in the NT kernel, driver support and security model while its Win32 and UI layers are mediocre, with one arguing the inverse project — Linux tooling on an NT base — would be the ideal outcome. Others pointed to alternatives such as the XFCE winxp-tc theme for XP looks without Wine and the unreleased loss32 shell, and several flagged that shipping legacy explorer.exe means shipping its vulnerabilities, though it does enable AutoHotkey-style tooling.

**Tags**: `#wine`, `#linux-desktop`, `#windows`, `#compatibility-layer`, `#open-source-projects`

---

<a id="item-14"></a>
## [Dutch court bans BYD Ti7 across the EU over Defender design](https://electrek.co/2026/11/23/byd-ti7-banned-eu-land-rover-defender-design/) ⭐️ 6.0/10

A court in The Hague ruled that BYD&\#x27;s Ti7 SUV infringes Jaguar Land Rover&\#x27;s registered EU design for the Land Rover Defender and issued an EU-wide injunction barring BYD from selling or building the vehicle. Breaching the order carries penalties of €100,000 per day, capped at €10 million, and the decision reverses an earlier ruling from the same court just 10 days prior that had gone in BYD&\#x27;s favour. The injunction sets a concrete precedent that European design registrations can halt a Chinese automaker&\#x27;s EU rollout entirely, not just trigger royalties, and it signals that aesthetics-based IP is becoming a real barrier for Chinese EV makers expanding into Europe. BYD&\#x27;s Hong Kong shares fell as much as 4% on the news, showing investors treat design litigation as a material commercial risk. The ruling is a cross-border injunction, a mechanism Dutch courts are known for using to extend a single national judgment across multiple EU member states in IP disputes. The €10 million cap means a prolonged refusal to comply would exhaust the penalty ceiling in roughly 100 days at the maximum daily rate.

rss · Electrek · Nov 23, 17:18

**Background**: An EU registered design protects the outward appearance of a product — its lines, contours, shape and surface decoration — rather than how it works, and it can last up to 25 years if renewed every five years; registration must typically be filed within one year of the design first being made public. Because these rights are registered separately in each jurisdiction but harmonised across the EU, a Dutch court can in certain conditions issue a cross-border injunction covering infringement in several other member states at once. This case turns on whether the Ti7&\#x27;s boxy silhouette is too close to the Defender&\#x27;s protected design.

<details><summary>References</summary>
<ul>
<li><a href="https://www.euipo.europa.eu/en/designs">Designs - EUIPO</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cross-border_injunction">Cross-border injunction - Wikipedia</a></li>
<li><a href="https://electrek.co/2026/11/23/byd-ti7-banned-eu-land-rover-defender-design/">BYD Ti7 banned from the EU for copying the Land Rover ...</a></li>

</ul>
</details>

**Tags**: `#automotive`, `#intellectual-property`, `#design-patents`, `#EU-regulation`, `#BYD`

---

<a id="item-15"></a>
## [datasette-charts 0.1a0 adds whole-dataset charting to Datasette, prototyped with Claude](https://simonwillison.net/2026/Nov/23/datasette-charts/) ⭐️ 6.0/10

Simon Willison released datasette-charts 0.1a0, an alpha Datasette plugin that adds configurable charts to any table page or arbitrary SQL query, complete with data-driven chart suggestion thumbnails and a sidebar for choosing chart type, time bucketing, value aggregation and series splitting. He notes he had been thinking about the problem for over a year but built the working prototype in one Sunday session with the Claude Fable 5.2 coding assistant, and it went so well that it became a full plugin. Datasette users can now get meaningful visualizations of an entire table or the full result set of a query in a couple of clicks, instead of only charting the page of rows currently on screen. It is also a concrete public example of how far LLM coding agents can carry a real, shippable open-source plugin in a single session. Each chart is compiled into a SQL query that aggregates across the whole result set using GROUP BY, time bucketing and window functions, with the returned rows capped at 5,000, while a sample of rows is used to suggest suitable charts for large tables. Rendering relies on vendored D3, Observable Plot and topojson-client, and the chart&\#x27;s state is persisted in a URL \#fragment so charts can be bookmarked or shared; the release is explicitly an early alpha.

rss · Simon Willison · Nov 23, 00:37

**Background**: Datasette is Simon Willison&\#x27;s open-source tool for exploring and publishing data of any shape or size as an interactive website and API, extended by a large ecosystem of over 150 official and community plugins. Visualization has long been one of those plugin categories, but earlier options such as datasette-vega could only chart the rows on the current page, typically up to 100. Datasette Lite, where the demo runs, packages Datasette via WebAssembly and Pyodide so the whole Python application executes inside the browser with no server.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/">Datasette : An open source multi- tool for exploring and publishing data</a></li>
<li><a href="https://lite.datasette.io/">Datasette</a></li>
<li><a href="https://github.com/simonw/datasette">GitHub - simonw/ datasette : An open source multi- tool for exploring ...</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#data-visualization`, `#ai-assisted-development`, `#open-source`, `#plugins`

---