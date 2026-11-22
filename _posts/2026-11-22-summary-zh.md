---
layout: default
title: "Horizon Summary: 2026-11-22 (ZH)"
date: 2026-11-22
lang: zh
---

> 从 16 条内容中筛选出 6 条重要资讯。

---

1. [Lean 形式化验证黎曼猜想的声明引发信任之争](#item-1) ⭐️ 10.0/10
2. [GPGME 严重双重释放漏洞（CVE-2026-129975）波及邮件客户端、Samba、Flatpak 与 GitLab](#item-2) ⭐️ 8.0/10
3. [开发者查明下载速度暴跌 75%的元凶：显示器 USB Hub 带来的延迟](#item-3) ⭐️ 7.0/10
4. [科学博客详述如何处理一批不断恶化的叠氮化铅库存](#item-4) ⭐️ 6.0/10
5. [用 Go 编写 PostgreSQL 扩展的演示项目引发工具链讨论](#item-5) ⭐️ 6.0/10
6. [Zero C\#：无需 .NET 运行时和 GC 的 C\# 实验](#item-6) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Lean 形式化验证黎曼猜想的声明引发信任之争](https://leanprover-community.github.io/blog/posts/riemann-hypothesis/) ⭐️ 10.0/10

Lean Prover Community 博客上的一篇文章展示了一项 Lean 形式化验证，声称建立了黎曼猜想（据称是其广义形式），并表示该工作得到了大量 AI 协助——评论者特别提到是 Claude 模型在人类合作者 Levent 的指导下完成的。该声明发布在社区博客而非经过同行评审的出版物上，因此仍有待独立专家验证。 如果该验证站得住脚，一个经过机器检验的黎曼猜想证明将是数论与形式化数学的范式转变，因为黎曼猜想是数学中最著名的未解问题，大量条件性结论都依赖于它。评论者还指出，为达成这一结果似乎需要形式化现代数学的庞大部分，这本身对证明助手和 Lean 的 mathlib 而言就是一项独立于黎曼猜想的重大里程碑。 讨论聚焦于证明助手的信任边界：内核虽小却并非无懈可击，已知的 Lean 4 健全性漏洞（\#14576）曾允许在无公理的情况下证明 False，从而使一个伪造的 AI 辅助类 Collatz 反证通过了检查器。支持者反驳说，多个独立内核（尤其是自带一致性证明的 con-leche 与 con-ron）必须同时被攻破，且漏洞还要同时影响一致性证明和黎曼猜想证明本身，加之有真人在环中把关，AI 在不被发现的情况下作弊的可能性要低得多。

hackernews · g-b-r · 11月21日 14:36 · [社区讨论](https://news.ycombinator.com/item?id=50589618)

**背景**: Lean 是一种证明助手，数学家在其中精确陈述定理并撰写证明，再由一个小而可信的内核逐步检查，因此一个通过检查的证明，其可信度取决于该内核及其所依赖的公理。过去十年间，Lean 的 mathlib 库已成长为规模庞大、由社区维护的现代数学形式化工程；近期的工作还将 Lean 与大语言模型结合，使 AI 生成的证明步骤被机械检验，而不是凭信任接受。黎曼猜想于 1859 年提出，断言黎曼 zeta 函数的所有非平凡零点都位于临界线上，数论中很大一部分条件性结论都建立在它之上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Proof_assistant">Proof assistant - Wikipedia</a></li>
<li><a href="https://essamamdani.com/blog/lean-4-soundness-bug-14576-postmortem">Lean 4 Soundness Bug #14576: What Broke the Kernel</a></li>
<li><a href="https://gearpulse.site/articles/lean-collatz-scare-proof-assistants-need-boring-defenses/">Lean&#x27;s Collatz scare shows why proof assistants need... | GearPulse</a></li>

</ul>
</details>

**社区讨论**: 主流情绪是谨慎的兴奋：评论者认为，在多个独立内核各自带有一致性证明的情况下，结果源自检查器漏洞的概率如今微乎其微；但也有人指出，一个伪造的 Collatz 反证曾经骗过某个独立检查器，并质疑这些内核的独立性能有多大。不少人强调，功劳很大程度上应归于人类合作者 Levent，是他从 AI 那里引导出了这份证明；还有人认为，对现代数学大片领域的形式化才是更广泛意义上的重要成果，并由此追问数学家如今是否敢去挑战哪些更宏大的问题。

**标签**: `#Lean`, `#formal verification`, `#Riemann Hypothesis`, `#AI for mathematics`, `#proof assistants`

---

<a id="item-2"></a>
## [GPGME 严重双重释放漏洞（CVE-2026-129975）波及邮件客户端、Samba、Flatpak 与 GitLab](https://lists.gnupg.org/pipermail/gnupg-announce/2026q4/000517.html) ⭐️ 8.0/10

GnuPG 发布了关于 CVE-2026-129975 的安全公告，这是一个存在于 GPGME 中的双重释放漏洞，当应用程序处理精心构造的 OpenPGP 公钥时会被触发；所有使用 2.3.0 之前版本 GPGME 的软件（无论以共享库、DLL 还是静态链接方式使用）都受影响。该漏洞由 Johan Carlsson 发现，并于 2026-11-12 通过 GitLab 上报给 GPGME 维护者，最终于 2026-11-20 公开披露，比原定的 2026-11-25 协同披露日期提前了五天，原因是 GitLab 需要针对另一个 Ruby2Shell 问题提前发布更新。 GPGME 是大多数自由软件应用用来调用 GnuPG 的标准高层加密 API，因此影响范围覆盖 Gpg4win、GnuPG Desktop、大多数邮件客户端、许多 XMPP 客户端、Samba 和 Flatpak；尤其值得注意的是 GitLab 的签名提交验证路径，因为该场景下服务器会解析攻击者提交的公钥，一旦发生代码执行后果尤为严重。此次披露还暴露了一个流程问题：下游发行版似乎多年前就携带了修复补丁，而上游却始终没有收到。 公告指出，由于两次释放之间还发生了其他内存分配，内存分配器常见的双重释放检测启发式可能不会被触发，这也解释了该缺陷为何能长期潜伏；问题已在 GPGME 2.3.1（1.x 分支为 1.24.4）中修复。其影响被描述为数据泄露并可能实现 RCE，而非已被证实的利用链；评论者指出，利用该漏洞需要应用去解析不可信的公钥，例如验证或导入路径，而不仅仅是链接该库。

hackernews · gdgghhhhh · 11月21日 08:32 · [社区讨论](https://news.ycombinator.com/item?id=50587208)

**背景**: GPGME（GnuPG Made Easy）是一个 C 库，为应用提供加密、解密、签名、签名验证和密钥管理的高层 API，并以 GnuPG 和 GpgSM 作为 OpenPGP 与 CMS 的后端。双重释放是一种内存安全缺陷，同一块堆内存被释放两次，会破坏分配器的元数据，通常导致崩溃、数据泄露乃至任意代码执行（CWE-415）。由于 GitLab 等代码托管平台的提交签名功能需要用用户提供的公钥来验证签名，该路径上的解析漏洞就把一项例行的服务端检查变成了攻击面。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lists.gnu.org/archive/html/info-gnu/2026-11/msg00006.html">GnuPG Security Advisory for GPGME (T8557,CVE-2026-129975)</a></li>
<li><a href="https://blog.ostorlab.co/gpgme-double-free-cve-2026-129975.html">GPGME Double Free: Data Theft, Possible RCE (CVE-2026-129975)</a></li>

</ul>
</details>

**社区讨论**: 评论者补充了重要背景：有人指出，根据常规工具的输出，Red Hat 据称在五年前就修复了该漏洞，而上游却遗漏了；报告者则确认了 2026-11-20 的披露日期，并给出了 GitLab Omnibus 的相关补丁链接。另一些人则对标题式的表述提出异议——“这是双重释放漏洞，不是一条 RCE 利用链”——并质疑此类报告是否有意夸大；还有评论者借此主张，人类不应在没有 Rust 级别工具保障的情况下编写 C/C++，以避免这类缺陷。

**标签**: `#security`, `#vulnerability-disclosure`, `#gnupg`, `#memory-safety`, `#gitlab`

---

<a id="item-3"></a>
## [开发者查明下载速度暴跌 75%的元凶：显示器 USB Hub 带来的延迟](https://blog.tymscar.com/posts/studiodisplayethernet/) ⭐️ 7.0/10

一位开发者发表了一篇排查记录，解释了为什么把以太网连接经由显示器内置的 USB Hub 转接会让他的下载速度下降约 75%。经过排查，他把原因归结为 Hub 额外引入的延迟，而非显示器本身：延迟拖慢了 TCP 数据包的确认（ACK）速度，导致以太网适配器的缓冲区被填满并丢包；换用一款对确认频率要求更低的适配器后，速度恢复正常。 这个案例说明，即使物理链路和运营商带宽完全正常，一个看不见的底层转接环节也可能在用户毫无察觉的情况下摧毁应用层吞吐量。它为使用笔记本和扩展坞的用户提供了一条具体的排查思路——也提醒大家在下载速度莫名其妙暴跌时，应把适配器直连测试，而不是经由 Hub 转接。 其机制是间接的：增加的往返延迟拖慢了主机的 TCP 确认，未被确认的数据积压填满了 USB 以太网适配器有限的缓冲区，适配器随之开始丢包，而 TCP 又把丢包当作拥塞来处理。有评论者指出，显示器其实基本是个“烟雾弹”——任何处于链路上的 USB Hub 都会造成同样效果，而问题的解决靠的是换用另一款确认/缓冲行为不同的适配器，而非调整显示器的任何设置。

hackernews · soheilpro · 11月21日 10:36 · [社区讨论](https://news.ycombinator.com/item?id=50587875)

**背景**: TCP 是一个由确认驱动的协议：发送方只能让一定量的数据同时在途（即窗口），并随着接收方确认收到数据包而推进窗口。由于吞吐量大致等于窗口大小除以往返时间，链路上任何环节的额外延迟——包括主机与网卡适配器之间的一个 USB Hub——都会直接降低可达到的下载速度，即使原始带宽并未受影响。基于 USB 的以太网适配器通常是非 DMA 设备，片上缓冲区相对较小且由驱动管理，因此相比具备硬件 DMA 和大描述符环的 PCIe 网卡，它们更容易被突发性的未确认流量压垮。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://superuser.com/questions/437429/does-a-usb-hub-affect-performance">Does a USB hub affect performance ? - Super User</a></li>
<li><a href="https://californiatelecom.com/blog/what-is-network-throughput">What Is Network Throughput ? A Clear Technical... | California Telecom</a></li>
<li><a href="https://learn.microsoft.com/en-us/windows-hardware/drivers/netcx/network-data-buffer-management">Network data buffer management - Windows drivers How can I check the number of packets dropped by udp because ... usb to ethernet chip causes packet loss | Weyland How to Find the Cause of Packet Loss in Your Network USB Adapter with packet drops - Ask Wireshark</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认可这是一篇扎实的排查文章，但对标题的表述提出异议：有人指出更准确的说法应是“我的 USB 网络交换机把下载速度拖慢了”，因为显示器本身无关紧要。也有人为误读原文的读者归纳了 TCP/ACK 与缓冲区溢出的机制；一位用户分享了类似的反直觉案例——Ghostty 使用 io\_uring 被误判为 I/O 压力，导致《博德之门 3》自行节流 Vulkan 着色器编译；另一位用户则表示自己在 MacBook 加雷雳扩展坞上遭遇了几乎相同、持续一年多的困扰。

**标签**: `#networking`, `#hardware`, `#debugging`, `#usb`, `#latency`

---

<a id="item-4"></a>
## [科学博客详述如何处理一批不断恶化的叠氮化铅库存](https://www.science.org/content/blog-post/detonating-huge-pile-lead-azide-really) ⭐️ 6.0/10

化学家 Derek Lowe 在 Science.org 的博客文章中讨论了一个棘手问题：如何安全销毁存放在爱荷华州米德尔敦（Middletown）爱荷华陆军弹药厂的一大批正在变质的叠氮化铅，这些材料在储存过程中发生重结晶，对摩擦和冲击变得极其敏感。美军原计划进行受控露天引爆，但因担心会产生含铅有毒粉尘云、飘过爱荷华州东南部乃至伊利诺伊州西北部而暂停。 这一案例说明，危险材料若被放任老化数十年，等到必须处理时，最便宜、最安全的选项早已不复存在，只剩下就地销毁这一条现实路径。它还引出了更广泛的问题：政府所有设施中的承包商责任如何界定，以及机构如何一再拖延风险、直到事故迫使问题爆发。 叠氮化铅是一种用于起爆雷管和引信的起爆药（初级炸药），在美军停止使用该化合物后，这批库存被存放在两个加固的覆土“拱顶”弹药库中。由于重结晶后的物料哪怕受到轻微扰动也可能引爆，它无法简单地装车运走；而且主要的环境担忧不仅是爆炸破坏，还有铅污染。

hackernews · beginning\_end · 11月21日 13:23 · [社区讨论](https://news.ycombinator.com/item?id=50588982)

**背景**: 叠氮化铅是一种极敏感的起爆药（初级炸药），很小的冲击、火花或摩擦就足以使其起爆并引爆更大的次级装药，它曾在雷管中大量取代较早期的雷汞。与采矿或爆破用的大宗炸药相比，起爆药的处理风险要高得多，而老化会让情况更糟——杂质和重结晶会使晶体变得更敏感、更难以预测。米德尔敦工厂是为二战生产而建的，据评论者称后来转为由承包商运营，这也是讨论中责任归属问题如此突出的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.fox32chicago.com/news/what-is-lead-azide-from-iowa-army-explosion">What is lead azide —and why is the Army blowing it... | FOX 32 Chicago</a></li>
<li><a href="https://www.newsweek.com/army-issues-evacuation-warning-massive-toxic-lead-dust-cloud-12735122">Army suspends detonation after toxic lead dust cloud... - Newsweek</a></li>
<li><a href="https://www.snopes.com/fact-check/lead-azide-detonation-army-iowa/">Is US Army planning to detonate massive amount of lead azide in...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者大多不接受“用机器人解决”的想法，有人指出，处理类似不稳定过氧化物时，实验室的标准做法就是请拆弹人员就地销毁，因为这些桶一旦搬动就会爆炸。还有人把这件事视为政府合同失败的典型案例——政府建造、承包商运营的设施偷工减料——并认为它体现了一种更普遍的模式：把问题掩盖起来，直到只剩下糟糕的选项；有评论者把另一种可能的结果比作贝鲁特港口大爆炸。

**标签**: `#chemistry`, `#explosives`, `#industrial-safety`, `#government-contracting`, `#risk-management`

---

<a id="item-5"></a>
## [用 Go 编写 PostgreSQL 扩展的演示项目引发工具链讨论](https://jespino.github.io/gopgext/) ⭐️ 6.0/10

开发者 Jesús Espino 发布了一个项目页面（jespino.github.io/gopgext），演示如何用 Go 语言编写 PostgreSQL 扩展，该贴登上 Hacker News 首页，获得 113 分和 19 条评论。讨论串很快补充了相关的同类项目，包括 microo8 的 Go 扩展框架 plgo、Rust 的 pgrx，以及作者本人用 Go 编写 Linux 内核模块的 gokm 项目。 PostgreSQL 扩展历来需要针对服务器内部 API 编写 C 代码，因此这类语言绑定方案降低了门槛，让庞大的 Go 开发者群体也能为自己的数据库添加自定义类型、函数和操作符。这并非范式级的变革，只是一个细分项目，但它表明 Rust 的 pgrx 已经带动的“非 C 扩展工具链”正在积累更多动力。 用 Go 编写 Postgres 扩展需要依赖 cgo，并小心处理 ABI/FFI 细节以匹配服务器的 C 调用约定，包括 NULL 值约定、内存上下文，以及跨 FFI 边界的错误与 panic 传播。该项目更像是一份演示和学习资料，而非成熟框架；有评论者表示实际工作中仍会选择 pgrx。

hackernews · valyala · 11月21日 17:08 · [社区讨论](https://news.ycombinator.com/item?id=50591260)

**背景**: PostgreSQL 的扩展系统是它最具代表性的特性之一：允许开发者添加自定义数据类型、函数、操作符，甚至全新的存储引擎。传统上，这种能力需要针对 Postgres 内部实现编写 C 代码才能获得。pgrx 为 Rust 承担了同样的工作，自动生成把 Rust 代码安全暴露为原生 Postgres 函数所需的样板代码。而基于 Go 的方案依赖 cgo，即让 Go 调用 C 代码、并允许 Postgres 后端反向调用 Go 函数的机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/topics/plgo">plgo · GitHub Topics · GitHub</a></li>
<li><a href="https://docs.rs/pgrx/latest/pgrx/">pgrx - Rust - Docs.rs GitHub - rust-stuff/pgx: Build Postgres Extensions with Rust! pgrx - Rust - Docs.rs I Put My Rust Code Inside PostgreSQL — Building an Extension ... Rust-Powered PostgreSQL Extensions with pgrx Guide Custom PostgreSQL extensions with Rust - boringSQL</a></li>
<li><a href="https://github.com/rust-stuff/pgx">GitHub - rust-stuff/pgx: Build Postgres Extensions with Rust!</a></li>

</ul>
</details>

**社区讨论**: 整体情绪偏正面，评论者认为任何能让 PostgreSQL 扩展更易编写的东西都值得欢迎，不过也有人表示自己仍会坚持使用 pgrx。其他人则补充了相关项目线索，即用于 Go 扩展的 plgo 和作者在 Go 中编写 Linux 内核模块的 gokm；同时部分讨论跑题，转而比较 Go gopher 与 Ferris 螃蟹等语言吉祥物。

**标签**: `#PostgreSQL`, `#Go`, `#database extensions`, `#cgo/FFI`, `#systems programming`

---

<a id="item-6"></a>
## [Zero C\#：无需 .NET 运行时和 GC 的 C\# 实验](https://onurgumus.github.io/zero-csharp/index.html) ⭐️ 6.0/10

Zero C\# 是一个在 Hacker News 上展示的实验性项目，它基于 bflat 分支，将 C\# 编译成无需 .NET 运行时和垃圾回收器即可运行的小型原生程序，同时保留 C\# 语法、类型检查和泛型。 该项目探索了 C\# 在裸机或极简依赖场景中的可能性，这些场景无法接受 .NET 运行时和 GC，但讨论显示它更像有趣的实验，而非现有 C\# 工具链的实用替代品。对于考虑在受限原生目标上使用 C\# 的开发者来说，它会与 NativeAOT 以及 C、Rust、Zig 等语言形成直接比较。 Zero C\# 是 bflat 的一个分支，按其项目页面所述可生成面向 Linux 甚至 386 的小型原生输出，但它缺少 .NET 标准库，因此现有 C\# 代码通常无法原样运行。评论者还指出，NativeAOT 已经提供官方提前编译路径，更小的二进制文件往往是其最明确的优势。

hackernews · reverseblade2 · 11月21日 15:39 · [社区讨论](https://news.ycombinator.com/item?id=50590279)

**背景**: C\# 通常先编译为 IL，然后在 .NET 运行时上执行，而该运行时会提供垃圾回收器和标准库；NativeAOT 是微软的提前编译部署模型，在发布时将 IL 编译为原生代码，使最终应用无需安装 .NET 运行时。垃圾回收器会自动回收不再使用的内存，而手动内存管理（如 C、Rust 或 Zig）让程序员拥有更多控制权，但也需要显式管理分配和生命周期。Zero C\# 基于 bflat 分支，借助该工具链把 C\# 编译成无需常规运行时的原生程序。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://onurgumus.github.io/zero-csharp/index.html">Zero C# | C# without a runtime , from Linux to a 386</a></li>
<li><a href="https://learn.microsoft.com/en-us/dotnet/core/deploying/native-aot/">Native AOT deployment overview - . NET | Microsoft Learn</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论普遍对 Zero C\# 的实用价值持怀疑态度：评论者认为 unsafe 指针、Span&lt;T&gt;、ref struct、Marshal 和 NativeAOT 已经为 C\# 开发者提供了底层控制和免运行时方案。一些人辩护说 GC 是提升生产力的特性而非缺陷，另一些人则指出缺少标准库会导致现有 C\# 代码无法运行，并认为 C、Rust 或 Zig 才是无 GC 编程的更好选择；还有评论者希望 .NET 提供类似 Java Epsilon GC 的冻结 GC 模式。

**标签**: `#C\#`, `#memory-management`, `#NativeAOT`, `#compilers`, `#programming-languages`

---