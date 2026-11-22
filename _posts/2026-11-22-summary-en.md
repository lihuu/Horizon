---
layout: default
title: "Horizon Summary: 2026-11-22 (EN)"
date: 2026-11-22
lang: en
---

> From 16 items, 6 important content pieces were selected

---

1. [Purported Lean formal verification of the Riemann Hypothesis sparks trust debate](#item-1) ⭐️ 10.0/10
2. [Critical GPGME Double-Free Bug \(CVE-2026-129975\) Hits Mail, Samba, Flatpak and GitLab](#item-2) ⭐️ 8.0/10
3. [Developer traces 75% download speed drop to monitor USB hub latency](#item-3) ⭐️ 7.0/10
4. [Science Blog Details the Perilous Disposal of a Deteriorating Lead Azide Stockpile](#item-4) ⭐️ 6.0/10
5. [Go-Powered PostgreSQL Extensions Demo Sparks Tooling Discussion](#item-5) ⭐️ 6.0/10
6. [Zero C\#: C\# without a .NET runtime or GC](#item-6) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Purported Lean formal verification of the Riemann Hypothesis sparks trust debate](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) ⭐️ 10.0/10

A post on the Lean Prover Community blog presents a Lean formal verification that purportedly establishes the Riemann Hypothesis \(reportedly in a generalized form\), said to have been produced with substantial AI assistance — commenters specifically credit the model Claude working under human collaborator Levent. The announcement is a community blog post rather than a peer-reviewed publication, so the claim is still awaiting independent expert validation. If the verification holds up, a machine-checked proof of the Riemann Hypothesis would be a paradigm shift for number theory and for formal mathematics, since RH is the most famous open problem in mathematics and a vast body of conditional results depends on it. Commenters also point out that reaching the result appears to have required formalizing huge portions of modern mathematics, which would be a major milestone for proof assistants and Lean&\#x27;s mathlib independent of RH itself. The discussion highlights the trust boundary of proof assistants: the kernel is small but not infallible, and a known Lean 4 soundness bug \(\#14576\) once allowed an axiom-free proof of False, enabling a fake AI-assisted Collatz refutation to pass a checker. Defenders counter that multiple independent kernels \(notably con-leche and con-ron, which carry their own consistency proofs\) would all have to be broken in a way that corrupts both the consistency proofs and the RH proof itself, and that a human expert in the loop makes unnoticed AI cheating much less likely.

hackernews · g-b-r · Nov 21, 14:36 · [Discussion](https://news.ycombinator.com/item?id=50589618)

**Background**: Lean is a proof assistant in which mathematicians state theorems precisely and write proofs that a small trusted kernel checks step by step, so a successfully checked proof is only as trustworthy as the kernel and the axioms it relies on. Over the past decade Lean&\#x27;s mathlib library has grown into a large, community-maintained formalization of modern mathematics, and recent work has paired Lean with large language models so that AI-generated proof steps are mechanically verified rather than taken on faith. The Riemann Hypothesis, formulated in 1859, asserts that all non-trivial zeros of the Riemann zeta function lie on the critical line, and it underpins a large fraction of conditional results in number theory.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Proof_assistant">Proof assistant - Wikipedia</a></li>
<li><a href="https://essamamdani.com/blog/lean-4-soundness-bug-14576-postmortem">Lean 4 Soundness Bug #14576: What Broke the Kernel</a></li>
<li><a href="https://gearpulse.site/articles/lean-collatz-scare-proof-assistants-need-boring-defenses/">Lean&#x27;s Collatz scare shows why proof assistants need... | GearPulse</a></li>

</ul>
</details>

**Discussion**: The dominant sentiment is cautious fascination: commenters argue that with several independent kernels carrying their own consistency proofs, the chance that the result stems from a checker bug is now vanishingly small, while others note that a fake Collatz refutation already slipped past an independent checker and question how independent these kernels really are. Several people emphasize that credit belongs heavily to the human collaborator Levent for eliciting the proof from the AI, and others frame the formalization of large swaths of modern mathematics as the more broadly important outcome, prompting reflection on which even larger problems mathematicians might now dare to attack.

**Tags**: `#Lean`, `#formal verification`, `#Riemann Hypothesis`, `#AI for mathematics`, `#proof assistants`

---

<a id="item-2"></a>
## [Critical GPGME Double-Free Bug \(CVE-2026-129975\) Hits Mail, Samba, Flatpak and GitLab](https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html) ⭐️ 8.0/10

GnuPG published a security advisory for CVE-2026-129975, a double-free vulnerability in GPGME that is triggered when an application processes a crafted OpenPGP public key; all software using GPGME versions prior to 2.3.0, whether as a shared library, DLL, or statically linked, is affected. The bug, discovered by Johan Carlsson and reported to the GPGME maintainers via GitLab on 2026-11-12, was disclosed on 2026-11-20 — five days ahead of the originally planned 2026-11-25 coordinated date — because GitLab had to ship updates early in response to the separate Ruby2Shell issue. GPGME is the standard high-level crypto API that most free-software applications use to talk to GnuPG, so the blast radius covers Gpg4win, GnuPG Desktop, most mail clients, many XMPP clients, Samba and Flatpak — and notably GitLab&\#x27;s signed-commit verification path, where a server parses attacker-supplied public keys and code execution would be especially dangerous. The disclosure also highlights a process failure: a downstream distribution appears to have carried a fix for years while upstream never received it. The advisory notes that because other allocations occur between the two frees, the usual double-free detection heuristics in memory allocators may not fire, which helps explain why the flaw survived so long; the issue is fixed in GPGME 2.3.1 \(and 1.24.4 on the 1.x branch\). Impact is described as data exposure with possible RCE rather than a proven exploit chain, and commenters point out that exploitation requires an application to parse an untrusted key — for instance a verification or import path, not merely linking the library.

hackernews · gdgghhhhh · Nov 21, 08:32 · [Discussion](https://news.ycombinator.com/item?id=50587208)

**Background**: GPGME \(GnuPG Made Easy\) is a C library that gives applications a high-level API for encryption, decryption, signing, signature verification and key management, using GnuPG and GpgSM as backends for OpenPGP and CMS. A double free is a memory-safety bug in which the same heap allocation is released twice, corrupting allocator metadata and often leading to crashes, data disclosure, or arbitrary code execution \(CWE-415\). Because commit-signing features in forges such as GitLab verify signatures against user-supplied public keys, a parser bug in that path turns a routine server-side check into an attack surface.

<details><summary>References</summary>
<ul>
<li><a href="https://lists.gnu.org/archive/html/info-gnu/2026-11/msg00006.html">GnuPG Security Advisory for GPGME (T8557,CVE-2026-129975)</a></li>
<li><a href="https://blog.ostorlab.co/gpgme-double-free-cve-2026-129975.html">GPGME Double Free: Data Theft, Possible RCE (CVE-2026-129975)</a></li>

</ul>
</details>

**Discussion**: Commenters added significant context: one noted that Red Hat reportedly fixed the bug five years ago based on conventional tooling output while upstream missed it, and the reporter confirmed the 2026-11-20 disclosure date and linked GitLab&\#x27;s Omnibus patch. Others pushed back on the headline framing — &quot;it&\#x27;s a double free bug, not an RCE chain&quot; — questioning whether such reports are intentionally overstated, while another commenter used the episode to argue that humans should not write C/C++ without Rust-level tooling to prevent these classes of bugs.

**Tags**: `#security`, `#vulnerability-disclosure`, `#gnupg`, `#memory-safety`, `#gitlab`

---

<a id="item-3"></a>
## [Developer traces 75% download speed drop to monitor USB hub latency](https://blog.tymscar.com/posts/studiodisplayethernet/) ⭐️ 7.0/10

A developer published a debugging write-up explaining why routing his Ethernet connection through his monitor&\#x27;s built-in USB hub cut his download speed by roughly 75%. After investigating, he traced the cause not to the monitor itself but to the extra latency the hub added, which slowed TCP packet acknowledgements, overflowed the Ethernet adapter&\#x27;s buffer, and caused packet drops; swapping to a different adapter that needed less frequent acknowledgement restored full speed. The case shows how an invisible, low-level link hop can silently destroy application-level throughput even when the physical link and the ISP connection are perfectly fine. It gives laptop and dock users a concrete debugging path — and a reminder to test adapters directly rather than through a hub — when download speeds mysteriously collapse. The mechanism is indirect: added round-trip latency delayed the host&\#x27;s TCP acknowledgements, the backlog of unacknowledged data filled the USB Ethernet adapter&\#x27;s finite buffer, and the adapter began dropping packets, which TCP then treated as congestion. Commenters pointed out that the monitor is basically a red herring — any USB hub in the path would produce the same effect, and the fix came from a different adapter&\#x27;s acknowledgement/buffering behavior rather than any monitor setting.

hackernews · soheilpro · Nov 21, 10:36 · [Discussion](https://news.ycombinator.com/item?id=50587875)

**Background**: TCP is an acknowledgement-driven protocol: the sender can only keep a certain amount of data in flight \(its window\), and it advances that window as the receiver confirms delivery of packets. Because throughput is roughly window size divided by round-trip time, extra latency anywhere in the path — including a USB hub between the host and a network adapter — directly reduces achievable download speed, even if raw bandwidth is unaffected. USB-based Ethernet adapters are typically non-DMA devices with relatively small on-chip buffers managed by the driver, so they are more vulnerable to bursts of unacknowledged traffic than a PCIe network card with hardware DMA and large descriptor rings.

<details><summary>References</summary>
<ul>
<li><a href="https://superuser.com/questions/437429/does-a-usb-hub-affect-performance">Does a USB hub affect performance ? - Super User</a></li>
<li><a href="https://californiatelecom.com/blog/what-is-network-throughput">What Is Network Throughput ? A Clear Technical... | California Telecom</a></li>
<li><a href="https://learn.microsoft.com/en-us/windows-hardware/drivers/netcx/network-data-buffer-management">Network data buffer management - Windows drivers How can I check the number of packets dropped by udp because ... usb to ethernet chip causes packet loss | Weyland How to Find the Cause of Packet Loss in Your Network USB Adapter with packet drops - Ask Wireshark</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed the write-up was a strong piece of debugging but pushed back on the framing, with one noting the accurate headline would be “my USB network switch was cutting my download speed” since the monitor is irrelevant. Others summarized the TCP/ACK and buffer-overflow mechanism for readers who misread the post, and one shared an analogous head-scratcher in which Ghostty&\#x27;s use of io\_uring registered as I/O pressure and caused Baldur&\#x27;s Gate 3 to throttle its Vulkan shader compilation; another user reported a nearly identical year-long struggle with a MacBook and Thunderbolt dock.

**Tags**: `#networking`, `#hardware`, `#debugging`, `#usb`, `#latency`

---

<a id="item-4"></a>
## [Science Blog Details the Perilous Disposal of a Deteriorating Lead Azide Stockpile](https://www.science.org/content/blog-post/detonating-huge-pile-lead-azide-really) ⭐️ 6.0/10

A Science.org blog post by chemist Derek Lowe examines the problem of safely destroying a large stockpile of deteriorating lead azide held at the Iowa Army Ammunition Plant in Middletown, Iowa, where the material has recrystallized during storage and become extremely sensitive to friction and shock. The Army&\#x27;s plan for a controlled open detonation was suspended after concerns arose that it could send a cloud of toxic lead dust over southeastern Iowa and into northwestern Illinois. The case shows what happens when hazardous material is left to degrade for decades: by the time it is addressed, the cheapest and safest options have disappeared, leaving destruction in place as the only realistic path. It also raises broader questions about contractor accountability at government-owned facilities and about how institutions defer risk until an accident forces the issue. Lead azide is a primary explosive used to initiate detonators and fuses, and the stockpile was stored in two reinforced, earth-covered &quot;igloo&quot; magazines after the Army moved away from the compound. Because the recrystallized material can detonate from even minor disturbance, it cannot simply be loaded onto trucks and hauled away, and the main environmental concern is lead contamination rather than blast damage alone.

hackernews · beginning\_end · Nov 21, 13:23 · [Discussion](https://news.ycombinator.com/item?id=50588982)

**Background**: Lead azide is a highly sensitive primary explosive, meaning a small shock, spark, or friction is enough to set it off and trigger a larger secondary charge; it largely replaced the older mercury fulminate in detonators. Primary explosives are far more dangerous to handle than the bulk explosives used in mining or demolition, and aging works against them because impurities and recrystallization can make the crystals more sensitive and unpredictable. The Middletown plant was built for World War II production and, according to commenters, later shifted to contractor operation, which is why questions of responsibility feature heavily in the discussion.

<details><summary>References</summary>
<ul>
<li><a href="https://www.fox32chicago.com/news/what-is-lead-azide-from-iowa-army-explosion">What is lead azide —and why is the Army blowing it... | FOX 32 Chicago</a></li>
<li><a href="https://www.newsweek.com/army-issues-evacuation-warning-massive-toxic-lead-dust-cloud-12735122">Army suspends detonation after toxic lead dust cloud... - Newsweek</a></li>
<li><a href="https://www.snopes.com/fact-check/lead-azide-detonation-army-iowa/">Is US Army planning to detonate massive amount of lead azide in...</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters largely rejected the idea that robots could solve the problem, with one noting that labs handling similarly unstable peroxides call the bomb squad to destroy material in place because the barrels cannot be moved without detonating. Others framed the episode as a case study in government contracting failure — government-built, contractor-operated facilities cutting corners — and in a wider pattern of hiding problems until only bad options remain, with one commenter comparing the alternative to the Beirut harbor explosion.

**Tags**: `#chemistry`, `#explosives`, `#industrial-safety`, `#government-contracting`, `#risk-management`

---

<a id="item-5"></a>
## [Go-Powered PostgreSQL Extensions Demo Sparks Tooling Discussion](https://jespino.github.io/gopgext/) ⭐️ 6.0/10

Developer Jesús Espino published a project page \(jespino.github.io/gopgext\) demonstrating how to write PostgreSQL extensions in Go, which reached the front page of Hacker News with 113 points and 19 comments. The thread quickly surfaced related work, including plgo \(a Go extension framework by microo8\), pgrx for Rust, and the author&\#x27;s own gokm project for writing Linux kernel modules in Go. PostgreSQL extensions have historically required writing C against the server&\#x27;s internal APIs, so language-binding approaches like this lower the barrier for the huge Go developer base to add custom types, functions and operators to their databases. It is a niche project rather than a paradigm shift, but it signals growing momentum behind non-C extension toolchains that Rust&\#x27;s pgrx has already popularized. Writing a Postgres extension in Go requires cgo and careful ABI/FFI handling to match the server&\#x27;s C calling conventions, including NULL contracts, memory contexts, and error or panic propagation across the FFI boundary. The site is best read as a demonstration and learning resource rather than a mature framework; one commenter noted they would still choose pgrx for real work.

hackernews · valyala · Nov 21, 17:08 · [Discussion](https://news.ycombinator.com/item?id=50591260)

**Background**: PostgreSQL&\#x27;s extension system is one of the database&\#x27;s defining features: it lets developers add custom data types, functions, operators, and even entirely new storage engines. Traditionally this power came at the cost of writing C against Postgres internals. pgrx does the same job for Rust, generating the boilerplate needed to expose Rust code safely as native Postgres functions. Go-based approaches rely on cgo, the mechanism that lets Go call into C and be called back by the Postgres backend.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/topics/plgo">plgo · GitHub Topics · GitHub</a></li>
<li><a href="https://docs.rs/pgrx/latest/pgrx/">pgrx - Rust - Docs.rs GitHub - rust-stuff/pgx: Build Postgres Extensions with Rust! pgrx - Rust - Docs.rs I Put My Rust Code Inside PostgreSQL — Building an Extension ... Rust-Powered PostgreSQL Extensions with pgrx Guide Custom PostgreSQL extensions with Rust - boringSQL</a></li>
<li><a href="https://github.com/rust-stuff/pgx">GitHub - rust-stuff/pgx: Build Postgres Extensions with Rust!</a></li>

</ul>
</details>

**Discussion**: Sentiment was broadly positive, with commenters saying anything that makes Postgres extensions easier to write is welcome, though one noted they would still stick with pgrx. Others contributed pointers to related projects, namely plgo for Go extensions and the author&\#x27;s gokm for Linux kernel modules in Go, while part of the thread drifted into off-topic chatter comparing language mascots like the Go gopher and Ferris the crab.

**Tags**: `#PostgreSQL`, `#Go`, `#database extensions`, `#cgo/FFI`, `#systems programming`

---

<a id="item-6"></a>
## [Zero C\#: C\# without a .NET runtime or GC](https://onurgumus.github.io/zero-csharp/index.html) ⭐️ 6.0/10

Zero C\#, an experimental fork of bflat presented on Hacker News, compiles C\# into small native executables that run without the .NET runtime or a garbage collector while retaining C\# syntax, type checking, and generics. The project probes how far C\# can be pushed toward systems programming without the .NET runtime, but commenters argue that NativeAOT, unsafe pointers, Span&lt;T&gt;, and ref structs already cover most low-level needs. Developers considering C\# for constrained native targets will compare it with NativeAOT and with languages like C, Rust, and Zig. Zero C\# is a fork of bflat that targets small native output, including Linux and even 386 according to its project page, but it omits the .NET standard library, so existing C\# code generally will not run unchanged. Commenters also noted that NativeAOT already provides official ahead-of-time compilation, with smaller binaries often being its clearest benefit.

hackernews · reverseblade2 · Nov 21, 15:39 · [Discussion](https://news.ycombinator.com/item?id=50590279)

**Background**: C\# normally compiles to IL and executes on the .NET runtime, which supplies the garbage collector and the standard library; NativeAOT is Microsoft&\#x27;s ahead-of-time deployment model that compiles IL to native code at publish time so the final app does not need the .NET runtime installed. A garbage collector automatically reclaims unused memory, while manual memory management, as in C, Rust, or Zig, gives the programmer more control but requires managing allocation and lifetime explicitly. Zero C\# is built as a fork of bflat, the toolchain it uses to compile C\# down to native code without the normal runtime.

<details><summary>References</summary>
<ul>
<li><a href="https://onurgumus.github.io/zero-csharp/index.html">Zero C# | C# without a runtime , from Linux to a 386</a></li>
<li><a href="https://learn.microsoft.com/en-us/dotnet/core/deploying/native-aot/">Native AOT deployment overview - . NET | Microsoft Learn</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was broadly skeptical of Zero C\#&\#x27;s practical value: commenters argued that unsafe pointers, Span&lt;T&gt;, ref structs, Marshal, and NativeAOT already give C\# developers low-level and runtime-free options. Some defended the GC as a productivity feature rather than a defect, while others said that without the standard library existing C\# code will not run and that C, Rust, or Zig are better choices for GC-free programming; one commenter instead asked for a Java-style Epsilon/frozen GC mode in .NET.

**Tags**: `#C\#`, `#memory-management`, `#NativeAOT`, `#compilers`, `#programming-languages`

---