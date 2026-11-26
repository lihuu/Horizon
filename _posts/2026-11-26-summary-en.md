---
layout: default
title: "Horizon Summary: 2026-11-26 (EN)"
date: 2026-11-26
lang: en
---

> From 30 items, 13 important content pieces were selected

---

1. [Scott Aaronson on AI&\#x27;s Sudden Progress on Open Math Problems](#item-1) ⭐️ 9.0/10
2. [1Password Discloses November 2026 Backend Security Incidents](#item-2) ⭐️ 8.0/10
3. [Anthropic AI compresses GRH Lean proof from 17M to 76k lines](#item-3) ⭐️ 8.0/10
4. [Preprint Claims the Polynomial Hirsch Conjecture Is False](#item-4) ⭐️ 8.0/10
5. [Google Research Releases Cogentic Papers on Integer Factorization and Discrete Logarithms](#item-5) ⭐️ 8.0/10
6. [Developer Reverse-Engineers Windows Loudness Equalization for PipeWire](#item-6) ⭐️ 7.0/10
7. [Lean audit of Clojure core finds unreported bugs](#item-7) ⭐️ 7.0/10
8. [Essay argues engineers who care should embrace LLM tools, sparking debate](#item-8) ⭐️ 7.0/10
9. [C++ &\#x27;= default&\#x27; and &\#x27;\{\}&\#x27; default constructors are not equivalent](#item-9) ⭐️ 7.0/10
10. [Ai2 Blog Examines Where Scientists Draw the Line on AI Agents](#item-10) ⭐️ 7.0/10
11. [Unsloth v0.1.925-beta: 3x Faster Inkling 2 Mini Fine-Tuning, Multi-GPU Parallelism](#item-11) ⭐️ 6.0/10
12. [Latency fingerprinting suggests Jev is Qwen3.5-35B-A3B](#item-12) ⭐️ 6.0/10
13. [New York Times Restricts Photographers From Latest AI-Equipped Photoshop](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Scott Aaronson on AI&\#x27;s Sudden Progress on Open Math Problems](https://scottaaronson.blog/?p=10379) ⭐️ 9.0/10

Scott Aaronson published a blog post expressing astonishment at a week of AI-driven results on long-standing open problems in mathematics and theoretical computer science, with a related preprint titled &quot;The matrix multiplication exponent is nine fourths&quot; linked from the post. He argued that people should not seize on trivialities — a minor mismatch between a Lean proof and its informal counterpart, or unused sections of a formalization — to deny that dozens of real open problems are now being solved. If LLM-driven systems can genuinely contribute to resolving open problems, the debate shifts from &quot;are LLMs glorified autocomplete&quot; to how fast automated mathematical discovery may now move, and it pushes formal verification into the center of research practice. Mathematicians, theoretical computer scientists, and AI labs all have a stake in whether these proofs survive scrutiny. The whole argument hinges on verification: a Lean 4 + Mathlib formalization gives a machine-checkable artifact, and recent agent designs alternate LLM proof generation with Lean-based checking, though such agents have proven costlier than specialized approaches on the hardest problems. The contested zone is the gap between what the Lean file actually proves and what the researchers informally claim, a failure mode long familiar from computer-generated proofs and code.

hackernews · Kotlopou · Nov 25, 19:11 · [Discussion](https://news.ycombinator.com/item?id=50646108)

**Background**: Lean is an interactive proof assistant, first released in 2013, whose mathematics library Mathlib \(begun around 2017\) lets mathematicians write proofs in a form a computer can check step by step; large projects such as Kevin Buzzard&\#x27;s effort to formalize Fermat&\#x27;s Last Theorem build on it. Because Lean gives automatic feedback on whether a proof compiles, pairing it with LLMs creates a loop where a model can propose proof steps and have them mechanically validated. The matrix multiplication exponent omega is the smallest number such that n-by-n matrices can be multiplied in roughly n^omega operations: the naive algorithm gives 3, Strassen&\#x27;s 1969 method about 2.81, and pinning down the true value has been a central open problem in algebraic complexity for decades.

<details><summary>References</summary>
<ul>
<li><a href="https://cacm.acm.org/research/formal-reasoning-meets-llms-toward-ai-for-mathematics-and-verification/">Formal Reasoning Meets LLMs: Toward AI for Mathematics and ...</a></li>
<li><a href="https://interestingengineering.com/culture/openai-exact-2-25-matrix-multiplication-exponent">OpenAI establishes exact 2.25 exponent for matrix multiplication</a></li>

</ul>
</details>

**Discussion**: The 637-comment Hacker News thread is broadly astonished but splits on two axes. Some, like utopiah, ask how much of this would have happened with only Lean, Mathlib and raw compute but no LLMs, suggesting the &quot;Mathocalypse&quot; may have been a decade in the making. Others, like onetimeusename, insist that gaps between Lean artifacts and informal claims are a legitimate concern rather than AI-denialism, while pixl97 hopes the emerging &quot;singularity&quot; stays confined to verifiable math and gorgoiler compares the moment to physics being declared &quot;solved&quot; just before quantum mechanics upended it.

**Tags**: `#AI`, `#mathematics`, `#Lean`, `#formal-verification`, `#LLMs`

---

<a id="item-2"></a>
## [1Password Discloses November 2026 Backend Security Incidents](https://1password.com/blog/update-on-nov-2026-security-incident) ⭐️ 8.0/10

1Password published an update on a November 2026 security incident in which malicious code was pushed to backend services. The disclosure has drawn intense Hacker News scrutiny over how the code got deployed and what user data was affected. A backend compromise at a widely used password manager is a high-stakes supply-chain event: even if vault encryption holds, users must trust that the service&\#x27;s code and delivery pipeline have not been tampered with. It also highlights how CI/CD credentials and employee endpoints have become primary attack surfaces for SaaS providers. Commenters criticized the writeup for not stating whether branch protection rules prevented direct pushes to main or whether such controls were bypassed. They also called for an unambiguous statement that encrypted vaults were not downloaded, rather than language that leaves room for interpretation.

hackernews · lxhrstn · Nov 25, 17:18 · [Discussion](https://news.ycombinator.com/item?id=50644817)

**Background**: SaaS supply-chain attacks often begin with a compromised employee laptop or stolen CI/CD credentials, after which attackers push malicious code into a service&\#x27;s build or deployment pipeline. Branch protection rules are a common control that requires pull requests, reviews and passing checks before code reaches the main branch, so questions about whether they were enforced are central to this incident. Password managers store encrypted vaults, but cloud-hosted services still depend on server-side code integrity for sync, delivery and account operations, which is why users scrutinize backend compromises closely.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.cloud.google.com/software-supply-chain-security/docs/attack-vectors">Software supply chain threats - Google Cloud</a></li>
<li><a href="https://microsoft.github.io/code-with-engineering-playbook/agile-development/branching-and-cicd/">Branching &amp; CI/CD Guidance - Engineering Fundamentals Playbook</a></li>
<li><a href="https://www.skillquestor.com/free-courses/ci-cd/branch-protection">Branch Protection — Free CI/CD | SkillQuestor</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion is broadly alarmed but technically focused: commenters describe compromised employee laptops and code-push access as the standard SaaS breach pattern, and one longtime 1Password user says the incident reinforces their choice to keep a local-only vault. The strongest criticism targets the lack of detail on branch protection and on whether encrypted vault data was accessed or downloaded. Overall, the thread treats the disclosure as a useful case study in SaaS supply-chain risk rather than a reason to dismiss 1Password outright.

**Tags**: `#security`, `#supply-chain`, `#1password`, `#saas`, `#ci-cd`

---

<a id="item-3"></a>
## [Anthropic AI compresses GRH Lean proof from 17M to 76k lines](https://github.com/lsernau/grh-lean) ⭐️ 8.0/10

The grh-lean repository published by lsernau now hosts a much shorter Lean 4 formalization of the Generalized Riemann Hypothesis for Dirichlet L-functions, reportedly cut from roughly 17 million lines down to about 76,000 lines — a reduction of around 99.5% — with clearer documentation throughout and an AI-assisted compression approach attributed to Anthropic. The repository is presented as a research artifact rather than a polished library release. Proof size has long been a practical barrier to whether machine-checked mathematics can actually be reviewed and trusted by people, so a two-orders-of-magnitude reduction makes a major formalization far more auditable. It also signals that large models can contribute to proof refactoring and compression, not just proof search — a capability that could reshape how formal verification projects are maintained. Commenters note that a separate, more readable version of roughly 300k lines exists, and that it explicitly separates &quot;known math&quot; from &quot;new math&quot; while carrying human-readable documentation. Others question whether brevity equals comprehensibility, since the compact code can bury key steps behind automation, making it unclear how realistically a human could read and trust it.

hackernews · nb-t · Nov 25, 21:48 · [Discussion](https://news.ycombinator.com/item?id=50648050)

**Background**: Lean is a functional programming language and interactive theorem prover built for formalizing mathematics and verifying software; it checks proofs algorithmically, so a completed Lean proof is correct beyond reasonable doubt, but the hard part for humans is rewriting the mathematics in a form Lean can accept. The Generalized Riemann Hypothesis extends the Riemann Hypothesis from the Riemann zeta function to Dirichlet L-functions, and both govern how prime numbers are distributed along the number line. Anthropic has recently invested heavily in AI for formal mathematics, including published work on formalizing Fermat&\#x27;s Last Theorem and on reducing the burden of formal verification. Large formalizations are normally measured in tens or hundreds of thousands of lines, so a 17-million-line proof is far beyond anything a human could review.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/lsernau/grh-lean">lsernau/ grh -lean: A short Lean 4 proof of the Generalized Riemann ...</a></li>
<li><a href="https://www.anthropic.com/research/formalizing-fermats-last-theorem">Formalizing Fermat&#x27;s Last Theorem \ Anthropic</a></li>
<li><a href="https://lean-lang.org/learn/">Learn — Lean Lang</a></li>

</ul>
</details>

**Discussion**: The Hacker News thread \(198 points, 88 comments\) mixes admiration with unease: one commenter welcomes the clearer known-math versus new-math split and human-readable documentation, while another finds it &quot;absurdly funny&quot; that years of incremental human effort on shrinking the proof were beaten in days by throwing compute and better internal models at the problem. A recurring question is whether a human can realistically read and grok the compact Lean code well enough to verify correctness.

**Tags**: `#Lean`, `#formal verification`, `#AI-assisted theorem proving`, `#Anthropic`, `#mathematics`

---

<a id="item-4"></a>
## [Preprint Claims the Polynomial Hirsch Conjecture Is False](https://github.com/openai/math/blob/main/preprints/Superpolynomial-graph-diameter-of-simple-polytopes-November-24-2026/paper.pdf) ⭐️ 8.0/10

A preprint posted in OpenAI&\#x27;s math preprints repository on November 24, 2026, on superpolynomial graph diameter of simple polytopes, claims to disprove the polynomial Hirsch conjecture. The author\(s\) reportedly construct a family of simple polytopes whose graph diameter grows faster than any polynomial in the number of facets, killing the relaxed version of the Hirsch conjecture that survived the 2010 counterexamples. If the argument holds, it closes the most natural relaxed form of a question that has been open since Francisco Santos disproved the original Hirsch conjecture in 2010, and it removes the standard geometric explanation for why some variant of the simplex method might run in polynomial time in the worst case. That touches linear programming theory, combinatorial geometry, and complexity theory, and it reshapes what researchers can hope to prove about pivot rules. The claimed counterexample is a family of simple polytopes with superpolynomial graph diameter; a lower bound of this kind refutes the polynomial Hirsch conjecture but does not by itself rule out every polynomial-time simplex-style algorithm, because diameter bounds constrain only the shortest monotone paths through a polytope&\#x27;s graph, not the paths that specific pivoting rules actually follow. The result is a preprint and has not been peer-reviewed.

hackernews · acossta · Nov 25, 17:34 · [Discussion](https://news.ycombinator.com/item?id=50644980)

**Background**: The Hirsch conjecture, posed in 1957, guessed that a d-dimensional polytope with n facets has graph diameter at most n − d, meaning you can walk between any two vertices along edges in relatively few steps; Francisco Santos disproved it in 2010 with a 43-dimensional counterexample after more than fifty years. The polynomial Hirsch conjecture is the weaker claim that the diameter is bounded by some polynomial in n and d. Diameter matters because the simplex method walks along polytope edges from vertex to vertex, so diameter bounds were long seen as the most promising route to explaining why simplex works so well in practice despite its exponential worst case, even though linear programming itself has been solvable in polynomial time since Khachiyan&\#x27;s ellipsoid method in 1979 and interior-point methods in the 1980s.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Linear_programming">Linear programming - Wikipedia</a></li>
<li><a href="https://www.academia.edu/69847390/Smoothed_analysis_of_algorithms_Why_the_simplex_algorithm_usually_takes_polynomial_time">(PDF) Smoothed analysis of algorithms : Why the simplex algorithm ...</a></li>

</ul>
</details>

**Discussion**: Commenters largely read this as mopping-up work rather than a paradigm shift: one notes it means no polynomial-time simplex algorithm exists and situates it as a follow-up to the 2010 disproof, while another offers an accessible translation of linear programming into a multi-dimensional shape whose corners are feasible but not necessarily optimal solutions. Others muse about an impending era of solved math problems, ask how anyone finds a paper among the thousand in this preprint folder, and joke that breakthroughs now arrive as GitHub patch notes.

**Tags**: `#mathematics`, `#computational geometry`, `#linear programming`, `#complexity theory`, `#Hirsch conjecture`

---

<a id="item-5"></a>
## [Google Research Releases Cogentic Papers on Integer Factorization and Discrete Logarithms](https://github.com/google-research/google-research/tree/master/cogentic_research_papers) ⭐️ 8.0/10

Google Research has published a new \`cogentic\_research\_papers\` directory containing papers produced by Cogentic, including work on unconditional integer factorization, deterministic subexponential factoring, and sub-quasi-polynomial discrete logarithms over fixed-characteristic finite fields. Integer factorization and discrete logarithms are the hardness assumptions behind RSA, Diffie–Hellman, and ElGamal, so even theoretical improvements draw intense scrutiny from cryptographers; the release also adds to the debate about AI systems contributing to serious mathematical research. The factoring paper is titled “Unconditional Integer Factorization in Time L\_N\[1/3, O\(1\)\]” and is described by commenters as replacing parts of the general number field sieve that depend on unproven heuristics, but it does not prove those conjectures and appears to pay a complexity penalty rather than threaten practical RSA keys.

hackernews · rgwohlbold · Nov 25, 13:33 · [Discussion](https://news.ycombinator.com/item?id=50642086)

**Background**: Integer factorization is the problem of finding the prime factors of a large composite number, and RSA encryption is designed to be hard to break without solving it. Discrete logarithms are a related hard problem used by Diffie–Hellman key exchange and ElGamal encryption; both are public-key systems whose security depends on these problems remaining computationally infeasible at practical key sizes. The general number field sieve is a leading classical algorithm for factoring large integers, but its complexity analysis relies on unproven heuristics.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/google-research/google-research/tree/master/cogentic_research_papers">Google Releases Cogentic Papers on Integer Factorization ...</a></li>
<li><a href="https://daily.dev/posts/google-releases-cogentic-papers-on-integer-factorization-discrete-logs-and-more-0lfmvr55g">Google Releases Cogentic Papers on Integer Factorization ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Discrete_logarithm">Discrete logarithm - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters were divided: some framed the papers as part of a broader wave of AI-driven mathematical progress, while others stressed that the factoring result does not beat GNFS asymptotically and mainly trades unproven heuristics for worse complexity, so its practical cryptographic impact is limited.

**Tags**: `#cryptography`, `#integer factorization`, `#discrete logarithms`, `#Google Research`, `#AI for mathematics`

---

<a id="item-6"></a>
## [Developer Reverse-Engineers Windows Loudness Equalization for PipeWire](https://github.com/xoxorwr/pw-loudness-eq) ⭐️ 7.0/10

A developer \(xoxorwr\) published pw-loudness-eq, a PipeWire module that reverse-engineers and reproduces the behavior of Windows&\#x27; &quot;Loudness Equalization&quot; audio enhancement, bringing the effect natively to Linux desktops. The project reached the front page of Hacker News with a roughly 305-point discussion thread. Windows&\#x27; loudness treatment is barely documented and has no equivalent in the Linux audio stack, so Linux users who switch between quiet dialogue and loud commercials or game effects now have an option on their own platform. The project also highlights how much of Windows&\#x27; shared-mode audio pipeline, including an undocumented limiter stage, is only understood through reverse engineering. Community members note that the algorithm is effectively loudness normalization rather than frequency-dependent equalization, and that it can pump gain upward on sustained pure tones or whistles, which is why an additional final limiter stage is required. Windows applies a comparable but much subtler limiting in shared mode \(via CAudioLimiter in AudioEng.dll inside audiodg.exe, roughly a fraction of a dB on peaks\) that is bypassed in WASAPI exclusive mode and ASIO.

hackernews · ThrowNotAway · Nov 25, 11:34 · [Discussion](https://news.ycombinator.com/item?id=50641171)

**Background**: Windows offers a &quot;Loudness Equalization&quot; enhancement in its sound device properties, which Microsoft&\#x27;s documentation describes as keeping the volume level constant across different audio sources — raising quiet dialogue and taming loud explosions so everything sounds roughly equally loud. On Linux, PipeWire is the modern low-latency, graph-based multimedia server that replaced PulseAudio and JACK for most desktops and already supports filter chains and loadable modules. Reverse engineering here means disassembling Windows audio components such as the DLLs behind audiodg.exe to recover an algorithm that was never publicly specified, then reimplementing it independently.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/windows-hardware/drivers/audio/loudness-equalization-dsp">Loudness Equalization DSP - Windows drivers | Microsoft Learn</a></li>
<li><a href="https://www.pipewire.org/">PipeWire</a></li>
<li><a href="https://en.wikipedia.org/wiki/Loudness_war">Loudness war - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters were split: some clarified that this is loudness normalization, not equalization, and warned that the approach is prone to pumping on pure tones and needs final limiting, while others questioned whether reverse-engineering a Windows DLL was even necessary since a generic limiter with published algorithms would do the job, calling the DLL approach potentially unethical. A minority pushed back on the whole premise, arguing that flattening the dynamic range of a composition defeats its musical purpose.

**Tags**: `#audio-processing`, `#PipeWire`, `#reverse-engineering`, `#Linux desktop`, `#loudness normalization`

---

<a id="item-7"></a>
## [Lean audit of Clojure core finds unreported bugs](https://s.conao3.com/blog/2026/e4f733) ⭐️ 7.0/10

An effort to use Lean to check Clojure&\#x27;s core library surfaced previously unreported bugs, according to the write-up. The work sparked discussion about how formal-verification methods apply to a widely used dynamic Lisp library. Clojure&\#x27;s core library underpins production systems at many companies, so even edge-case bugs in primitive functions can have broad impact. The audit also tests whether formal methods can produce useful signal in dynamic-language ecosystems long dominated by testing and manual review. Discussion participants pointed to specific flagged cases involving Java interop and coercion, such as calling \`.indexOf\` on a byte array with a Long value or calling \`get\` on a string with a floating-point key. Those examples suggest some findings may be expected behavior or low-severity issues, so the list requires careful triage rather than treating every alert as a confirmed bug.

hackernews · encyclopedism · Nov 25, 14:56 · [Discussion](https://news.ycombinator.com/item?id=50642939)

**Background**: Lean is an interactive theorem prover used for formal verification and mathematical proof engineering, allowing users to state properties and construct machine-checked proofs. Clojure is a Lisp dialect that runs on the JVM, and \`clojure.core\` is its fundamental standard-library namespace. Applying formal methods to an existing dynamic language library is difficult because its semantics include host interop, coercion rules, and runtime behavior that must be modeled accurately.

<details><summary>References</summary>
<ul>
<li><a href="https://leanprover.github.io/theorem_proving_in_lean/introduction.html">1. Introduction — Theorem Proving in Lean 3 (outdated)...</a></li>
<li><a href="https://clojuredocs.org/core-library">Clojure&#x27;s Core Library | ClojureDocs - Community-Powered ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Proof_assistant">Proof assistant - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community reaction was interested but skeptical: one commenter identified two problematic entries and argued that simple type checking could have caught them, calling for less noise. Another commenter linked a similar audit that found dozens of issues in SBCL, Clozure, and ACL2, while others discussed Nubank&\#x27;s heavy Clojure use and asked whether Lean is now preferred over Rocq \(formerly Coq\) for program verification. The overall sentiment was that the work is valuable but that false positives and triage quality are central concerns.

**Tags**: `#Clojure`, `#Lean`, `#formal verification`, `#bug finding`, `#static analysis`

---

<a id="item-8"></a>
## [Essay argues engineers who care should embrace LLM tools, sparking debate](https://www.iankduncan.com/engineering/2026-11-19-smart-people-who-give-a-shit-use-tools) ⭐️ 7.0/10

Ian K. Duncan published an essay titled &quot;Smart people who give a shit use tools&quot; \(dated 2026-11-19\) arguing that capable engineers should adopt LLMs rather than reject them, and the piece drew a 197-comment Hacker News discussion. The thread quickly moved past the headline into whether AI-assisted coding is really comparable to earlier abstraction jumps like assembly to C or C to JavaScript. The debate gets at a live professional question: whether LLM-assisted coding changes the nature of software work or merely speeds it up, and whether it rewards engineers who verify carefully or those who ship fast without checking. Because code review norms, quality expectations, and career incentives all hang on that answer, the discussion matters to anyone writing or reviewing production code today. The strongest counterargument in the thread is that with prior abstractions the core activity stays the same — you still model a problem into a code representation — whereas prompting an LLM is a qualitatively different activity. Commenters also question whether &quot;the model wrote it&quot; is an acceptable defense during code review, and warn that keeping a working understanding of the system now requires deliberate discipline.

hackernews · matthewsinclair · Nov 25, 07:46 · [Discussion](https://news.ycombinator.com/item?id=50639698)

**Background**: A long-running defense of high-level languages and frameworks is that each new layer lets engineers ignore lower-level details and focus on the problem, so LLMs are often pitched as the next such layer. Code review is the practice where a second engineer reads a proposed change before it merges, and it is the main social mechanism for catching errors and spreading knowledge in a team. Hacker News threads like this one are where practitioners argue out whether a new tool fits that existing culture of verification.

**Discussion**: Sentiment is largely skeptical of the essay&\#x27;s core analogy. One commenter \(anothaway\) argues that using an LLM is a fundamentally different experience from moving from assembler to C, because in the old transitions you are still modeling a problem in code, while xnorswap warns that LLMs amplify the cost of &quot;giving a shit,&quot; letting fast shippers outpace colleagues who take time to verify. Others \(chrisra, notpachet, lf88\) add that the model sometimes feels better than they are, that keeping knowledge requires deliberately holding the machine at arm&\#x27;s length, and that wise people notice when something stops being &quot;just a tool.&quot;

**Tags**: `#LLMs`, `#software engineering`, `#AI-assisted coding`, `#code review`, `#engineering culture`

---

<a id="item-9"></a>
## [C++ &\#x27;= default&\#x27; and &\#x27;\{\}&\#x27; default constructors are not equivalent](https://lemire.me/blog/2026/11/02/default-and-braces-are-not-the-same-constructor/) ⭐️ 7.0/10

Daniel Lemire&\#x27;s article explains that writing \`T\(\) = default\` and \`T\(\) \{\}\` produces materially different default constructors in C++, because the former is not user-provided while the latter is, changing how \`T\{\}\` value-initializes members. This distinction can turn seemingly equivalent initialization syntax into correctness and security bugs, especially for structs with raw pointers or scalar fields, so C++ practitioners need to understand it during code review and API design. With a defaulted default constructor and no default member initializers, \`T t\{\};\` first zero-initializes the object and then calls the constructor, whereas \`T t;\` leaves scalar members indeterminate; with a user-provided \`T\(\) \{\}\`, even \`T t\{\};\` skips that zero-initialization. The difference often disappears once members have default member initializers, and it only applies when value-initialization actually selects that default constructor.

hackernews · surprisetalk · Nov 25, 15:20 · [Discussion](https://news.ycombinator.com/item?id=50643199)

**Background**: A default constructor is the constructor callable with no arguments. Since C++11, \`= default\` asks the compiler to generate one, while \`\{\}\` is a user-provided empty body; the standard treats user-provided constructors differently in value-initialization. In C++, \`T t;\` is default-initialization, while \`T t\{\};\` is value-initialization, and for class types value-initialization may zero-initialize the object before running a non-user-provided default constructor.

<details><summary>References</summary>
<ul>
<li><a href="https://en.cppreference.com/cpp/language/default_constructor">Default constructors - cppreference.com</a></li>
<li><a href="https://en.cppreference.com/cpp/language/initialization">Initialization - cppreference.com</a></li>
<li><a href="https://stackoverflow.com/questions/20828907/the-new-syntax-default-in-c11">The new syntax &quot;= default&quot; in C++11 - Stack Overflow</a></li>

</ul>
</details>

**Discussion**: Commenters broadly agree the distinction illustrates C++&\#x27;s complexity: some prefer Rust/Go/Zig, where construction is just a static function, and one longtime C++ developer says such minutiae drove them to Rust. Others push back that the example is contrived because real code usually uses default member initializers, and one comment flags a separate GCC 15/16 performance regression.

**Tags**: `#C++`, `#constructors`, `#language design`, `#initialization`, `#programming languages`

---

<a id="item-10"></a>
## [Ai2 Blog Examines Where Scientists Draw the Line on AI Agents](https://huggingface.co/blog/allenai/where-scientists-draw-the-line-on-ai-agents) ⭐️ 7.0/10

The Allen Institute for AI \(Ai2\) published a blog post on Hugging Face that examines where scientists draw the line on the use of AI agents in scientific work, mapping which research tasks researchers consider acceptable for agents to handle and which they want kept under human control. The post is a perspective piece on norms and boundaries rather than the announcement of a new model or tool. AI agents are shifting from passive tools to semi-autonomous collaborators in research, so where scientists set limits will shape how labs adopt these systems, how results get reviewed and reproduced, and how much trust the broader research community places in agent-generated work. Because Ai2 is a well-known non-profit AI research institute, its framing can influence conventions that other labs, publishers, and funders later adopt. The discussion treats autonomy as a spectrum — from AI used as a tool under direct human supervision to agents performing research tasks with partial autonomy while still under oversight — rather than as a simple yes-or-no question. The provided excerpt contains no body text, so the post&\#x27;s specific survey data, concrete policy recommendations, or named thresholds could not be verified here.

rss · HuggingFace Blog · Nov 25, 18:52

**Background**: The Allen Institute for AI \(Ai2\) is a non-profit scientific research institute founded in 2014 by the late Microsoft co-founder and philanthropist Paul Allen, known for openly published AI research and for AI-for-science efforts such as its Asta platform and AutoDiscovery agent, which has been applied to cancer research. In this context, an &\#x27;AI agent&\#x27; means a system that plans and executes multi-step tasks with limited human intervention, in contrast to a model that only answers individual prompts. Recent academic commentary describes AI in research moving from tightly supervised tool use toward agents that carry out tasks with partial autonomy, which is exactly the transition that prompts questions about where limits should be drawn.

<details><summary>References</summary>
<ul>
<li><a href="https://allenai.org/">AllenAI - Ai2: Truly open breakthrough AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Allen_Institute_for_AI">Allen Institute for AI - Wikipedia</a></li>
<li><a href="https://link.springer.com/article/10.1007/s43681-025-00908-0">Autonomous artificial intelligence, scientific research, and ...</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#scientific research`, `#AI safety`, `#AI adoption`, `#HuggingFace`

---

<a id="item-11"></a>
## [Unsloth v0.1.925-beta: 3x Faster Inkling 2 Mini Fine-Tuning, Multi-GPU Parallelism](https://github.com/unslothai/unsloth/releases/tag/v0.1.925-beta) ⭐️ 6.0/10

Unsloth released v0.1.925-beta, which makes LoRA/QLoRA fine-tuning of Inkling 2 Mini 1.8 to 3.1x faster while using 50% less VRAM, adds tensor, pipeline and context parallelism across multiple GPUs, speeds up the adamw\_8bit optimizer by up to 12% per step on small batches, and makes Z-Image LoRA training on T4 1.7x faster. The release also fixes bugs in Inkling 2 Mini fine-tuning, chat-format evaluation on custom datasets, tied-embedding exports, and several Desktop/chat issues. The headline gains matter for practitioners with modest hardware: Inkling 2 Mini can now be trained on Kaggle&\#x27;s free 2x T4 setup, and the new tensor/pipeline/context parallelism options let users scale beyond a single GPU, which is essential for large mixture-of-experts models. It reinforces Unsloth&\#x27;s position as the go-to low-VRAM fine-tuning stack at a time when open-weight models keep growing larger. Inkling 2 Small is also supported but needs roughly 290 GB of GPU memory in 4-bit, merged\_4bit export is still unsupported, and exporting a fine-tuned Inkling 2 Mini to a 17.5 GB q4\_k\_m GGUF requires about 150 GB of free disk, so a Colab A100 is recommended over Kaggle. On NVIDIA Ampere or newer GPUs, Inkling 2 training uses FlexAttention for about 15% faster steps on an L4.

github · danielhanchen · Nov 25, 14:13

**Background**: Unsloth is an open-source fine-tuning library that implements LoRA and QLoRA with hand-written Triton kernels, letting users adapt large models on consumer GPUs at a fraction of the usual memory cost. Inkling 2 Mini is Thinking Machines Lab&\#x27;s 26.4B-parameter mixture-of-experts model with 5.4B active parameters, aimed at coding, agentic and vision workloads. Tensor, pipeline and context parallelism are complementary model-sharding strategies: tensor parallelism splits individual layers across GPUs, pipeline parallelism splits layers into stages, and context parallelism shards long sequences to cut activation memory. GGUF is a binary model format designed for fast loading, used by llama.cpp to run quantized models locally.

<details><summary>References</summary>
<ul>
<li><a href="https://unsloth.ai/docs/models/inkling-2-mini/fine-tuning">Fine-tuning Inkling 2 Mini Guide | Unsloth Documentation</a></li>
<li><a href="https://unsloth.ai/docs/models/inkling-2-mini">Inkling 2 Mini - Run Locally Guide | Unsloth Documentation</a></li>
<li><a href="https://huggingface.co/docs/hub/gguf">GGUF · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#fine-tuning`, `#LoRA/QLoRA`, `#unsloth`, `#GPU-parallelism`, `#memory-efficiency`

---

<a id="item-12"></a>
## [Latency fingerprinting suggests Jev is Qwen3.5-35B-A3B](https://modaic.dev/blog/latency-doesnt-lie) ⭐️ 6.0/10

A blog post on Modaic&\#x27;s site uses latency-fingerprinting analysis to argue that the startup Jev&\#x27;s model is probably a repackaged Qwen3.5-35B-A3B rather than a proprietary foundation model. The claim rests on timing characteristics, not on released weights or provider confirmation. If accurate, the finding sharpens questions about provenance and transparency for API startups that resell open-weight models, especially Chinese MoE models, and could influence how developers and investors judge “model company” moats. It also highlights latency fingerprinting as a practical, if contestable, audit tool for black-box AI services. Qwen3.5-35B-A3B is a sparse mixture-of-experts model with 35B total parameters and only about 3B active per token, so a provider could serve it relatively cheaply while presenting it as a custom model. The post&\#x27;s method is inferential and has not been independently reproduced; commenters note that Modaic is a competitor to TypeSafe, so the result should be treated cautiously.

hackernews · csoham · Nov 25, 22:57 · [Discussion](https://news.ycombinator.com/item?id=50648823)

**Background**: Latency fingerprinting is a black-box technique that tries to identify an LLM by measuring response timing patterns, streaming behavior, tokenizer quirks, or template offsets rather than inspecting model weights. It belongs to a broader set of LLM fingerprinting methods used to verify what an API gateway is actually serving. Qwen3.5-35B-A3B is an open-weight Qwen model built on a sparse MoE architecture, with 35B total parameters, roughly 3B active parameters, native multimodal support, and a long context window. Some startups build commercial APIs on top of such open models, which makes model provenance and claims of proprietary technology hard for outsiders to verify.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2502.20589v1">LLMs Have Rhythm: Fingerprinting Large Language Models Using...</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.5-35B-A3B">Qwen/Qwen3.5-35B-A3B · Hugging Face</a></li>
<li><a href="https://www.siliconflow.com/models/qwen3-5-35b-a3b">Qwen3.5-35B-A3B - Model Info, Parameters, Benchmarks ...</a></li>

</ul>
</details>

**Discussion**: HN commenters are split but mostly skeptical: one notes Modaic is a competitor to TypeSafe and calls for reproduction before trusting the result, while others debate whether “wrapper” startups reselling Chinese open models are a problem and whether provenance even matters. A few argue Jev&\#x27;s shift from system-2 to system-1 thinking is still novel, and one asks what Modaic itself runs on.

**Tags**: `#LLM`, `#model-provenance`, `#latency-analysis`, `#Qwen`, `#AI-startups`

---

<a id="item-13"></a>
## [New York Times Restricts Photographers From Latest AI-Equipped Photoshop](https://www.dpreview.com/news/new-york-times-adobe-photoshop-2027-restriction-ai/) ⭐️ 6.0/10

The New York Times has reportedly told its photographers not to use the latest AI-equipped versions of Adobe Photoshop, reportedly Photoshop 2027, to avoid having their work automatically flagged as AI-generated by platforms. The policy was reported by DPReview and has sparked discussion about AI provenance, subscriptions, and alternatives. For an authoritative news brand, an automatic “AI-generated” label can directly damage credibility, so AI provenance is becoming an editorial and procurement issue rather than just a technical detail. The decision also puts pressure on Adobe and could create openings for competitors and alternative workflows. The core problem is that C2PA Content Credentials can record any AI involvement, making it hard for platforms and detectors to distinguish fully AI-generated images from ones that only received minor AI-assisted edits such as color adjustments, cutouts, or layout changes. The NYT restriction is therefore better understood as an editorial and procurement policy rather than a Photoshop bug or a blanket technical ban.

hackernews · rmason · Nov 25, 21:18 · [Discussion](https://news.ycombinator.com/item?id=50647673)

**Background**: C2PA, the Coalition for Content Provenance and Authenticity, defines the Content Credentials standard, which uses verifiable metadata to record how an image was generated, edited, and by which tools. Adobe has implemented Content Credentials in Photoshop and other apps, and platforms such as Instagram and Facebook may read these signals and apply AI labels. This makes AI-assisted editing visible far beyond the photographer’s own workflow.

<details><summary>References</summary>
<ul>
<li><a href="https://contentauthenticity.org/how-it-works">How it works - Content Authenticity Initiative</a></li>
<li><a href="https://helpx.adobe.com/photoshop/desktop/save-and-export/metadata-content-credentials/use-content-credentials.html">Content Credentials in Adobe Photoshop</a></li>
<li><a href="https://www.pixguard.io/blog/how-to-detect-ai-generated-images">How to detect AI - generated images on your website | PixGuard</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed that the real pain point is ambiguous AI provenance labeling: jjcm argued that an end image cannot easily be classified as fully AI-generated versus lightly AI-edited, and an AI tag can be a credibility killer for authoritative brands. Others discussed subscription fatigue and saw an opening for alternatives such as Affinity and ArtCraft.

**Tags**: `#AI content provenance`, `#Adobe Photoshop`, `#creative tools`, `#software subscriptions`, `#media industry policy`

---