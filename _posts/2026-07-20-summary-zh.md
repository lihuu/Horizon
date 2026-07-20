---
layout: default
title: "Horizon Summary: 2026-07-20 (ZH)"
date: 2026-07-20
lang: zh
---

> 从 27 条内容中筛选出 21 条重要资讯。

---

1. [阿里巴巴发布 Qwen 3.8：2.4 万亿参数开源权重大语言模型](#item-1) ⭐️ 9.0/10
2. [SRE 用 1600 美元的 ESP32 替代 12 万美元的保龄球系统](#item-2) ⭐️ 8.0/10
3. [Minecraft Java 版改用 SDL3](#item-3) ⭐️ 8.0/10
4. [Claude Code 采用用 Rust 重写的 Bun](#item-4) ⭐️ 8.0/10
5. [卖出 2500 台 MIDI 录音机后的经验教训](#item-5) ⭐️ 8.0/10
6. [fork() 如何不复制内存就复制进程](#item-6) ⭐️ 8.0/10
7. [AI 建议使自信倍增但准确性降低，研究显示](#item-7) ⭐️ 7.0/10
8. [OpenAI 将 Codex 的上下文窗口从 372k 减少至 272k](#item-8) ⭐️ 7.0/10
9. [IndieWeb 之旅揭示优势与障碍](#item-9) ⭐️ 7.0/10
10. [月之暗面因需求过大暂停 Kimi K3 新订阅](#item-10) ⭐️ 7.0/10
11. [AI 狂热正在摧毁全球决策能力](#item-11) ⭐️ 7.0/10
12. [谷歌 IDE 发展史：一场历史回顾](#item-12) ⭐️ 7.0/10
13. [分布式系统中的时间管理失误：一种故障模式](#item-13) ⭐️ 7.0/10
14. [在 Plonky3 中构建 Merkle 树 AIR 脚本教程](#item-14) ⭐️ 7.0/10
15. [最后一项 MPEG-4 视觉专利到期，Xvid/DivX 获解放](#item-15) ⭐️ 6.0/10
16. [树莓派服务器重生：SSD 与迷你 PC 替代方案](#item-16) ⭐️ 6.0/10
17. [五菱缤果可能换标雪佛兰进军北美](#item-17) ⭐️ 6.0/10
18. [transcribe.cpp：开源 C++语音转文本推理库](#item-18) ⭐️ 6.0/10
19. [普通 C 语言中的交换性复数理论](#item-19) ⭐️ 6.0/10
20. [真实世界的 CPU 瓶颈调试故事](#item-20) ⭐️ 6.0/10
21. [使用 Bubble Tea 在 Go 中开发终端用户界面](#item-21) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [阿里巴巴发布 Qwen 3.8：2.4 万亿参数开源权重大语言模型](https://twitter.com/Alibaba_Qwen/status/2078759124914098291) ⭐️ 9.0/10

阿里巴巴宣布推出 Qwen 3.8，这是一个拥有 2.4 万亿参数的开源权重大型语言模型，作为对月之暗面（Moonshot AI）最近发布 Kimi K3（2.8 万亿参数）的竞争回应。该模型预计很快将公开发布，延续之前 Qwen 模型的发布模式。 这一宣布加剧了开源权重大语言模型领域的竞争，尤其是中国 AI 实验室之间的竞争，并为社区提供了另一个强大的本地部署选择。2.4 万亿参数的大小使其成为最大公开可用模型之一，可能进一步推动在消费级硬件上运行大型模型的兴趣。 Qwen 3.8 是一个拥有 2.4 万亿参数的稠密模型，而竞争对手 Kimi K3 拥有 2.8 万亿参数，计划于 2026 年 7 月 27 日在 Hugging Face 上发布。该公告包含一个指向 Qwen 云服务定价计划的链接，表明其采取了开源权重与商业服务并重的双重策略。

hackernews · nh43215rgb · 7月19日 08:44 · [社区讨论](https://news.ycombinator.com/item?id=48966120)

**背景**: 开源权重的大型语言模型（LLM）是指其预训练权重公开发布，允许他人进行微调、部署或在其基础上构建，但并非完全开源。阿里巴巴的 Qwen 系列是该领域的佼佼者，此前版本如 Qwen 3.6 和 3.7 提供了不同大小的模型，包括混合专家（MoE）和稠密架构。Qwen 3.8 的发布紧随月之暗面（Moonshot AI）的 Kimi K3 之后，而 Kimi K3 之前已于 2025 年 7 月发布了开源权重的 Kimi K2。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kimi_K3">Kimi K3</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weights-llms-in-depth-analysis-adoption-usage-performance-jha-kymhc">Open - Weights LLMs: In-Depth Analysis of Adoption, Usage, and...</a></li>

</ul>
</details>

**社区讨论**: 评论普遍积极，用户对竞争感到兴奋，并渴望在本地运行该模型。然而，一位用户报告称 Qwen 3.7 Pro 在软件工程任务中体验不佳，称其“不可用”，并更青睐 DeepSeek V4 Pro。其他用户则希望 Qwen 3.8 能推出适合消费级硬件本地使用的更小尺寸版本。

**标签**: `#AI`, `#LLM`, `#Open Weights`, `#Alibaba`, `#Qwen`

---

<a id="item-2"></a>
## [SRE 用 1600 美元的 ESP32 替代 12 万美元的保龄球系统](https://news.ycombinator.com/item?id=48968606) ⭐️ 8.0/10

一名 SRE 兼保龄球馆老板对一套价值六位数的遗留计分系统进行了逆向工程，利用 ESP32 微控制器和现成硬件构建了开源替代方案，将成本从 10 万多美元降至约 1600 美元。 这展示了用现代开源嵌入式技术改造传统工业系统的巨大成本节约潜力，可能降低小型保龄球馆升级或维护计分系统的门槛。 该系统使用 ESP32 通过 ESPNow 组建星形拓扑网络，并配备 RS485 有线回退方案，树莓派作为球道计算机运行 Redis 和状态机。整个堆栈名为 OpenLaneLink，计划开源发布。

hackernews · section33 · 7月19日 14:41

**背景**: ESP32 是低成本低功耗的微控制器系列，内置 Wi-Fi 和蓝牙，广泛用于物联网应用。ESPNow 是乐鑫（Espressif）的专有通信协议，支持 ESP32 设备之间直接、低延迟、无连接通信，无需 Wi-Fi 路由器，可形成网状网络。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ESP32">ESP32</a></li>
<li><a href="https://www.espressif.com/en/products/socs/esp32">ESP32 Wi-Fi & Bluetooth SoC | Espressif Systems</a></li>

</ul>
</details>

**社区讨论**: 评论分享了类似经验：一位迷你保龄球道所有者使用旧的 Intel MCS-48 CPU，一位机械师的儿子回忆基于继电器的机器，一位工程师倡导改造旧机床。整体情绪积极支持，并补充了此类改造机会的普遍性。

**标签**: `#reverse-engineering`, `#IoT`, `#embedded-systems`, `#bowling`, `#cost-reduction`

---

<a id="item-3"></a>
## [Minecraft Java 版改用 SDL3](https://www.minecraft.net/en-us/article/minecraft-26-3-snapshot-4) ⭐️ 8.0/10

Minecraft: Java Edition 已采用 SDL3 库（Simple DirectMedia Layer 3）来改善跨平台支持，取代了之前基于 SDL2 的输入和窗口管理。 此更新增强了在 Windows、macOS 和 Linux（包括 Wayland）上的性能和兼容性，惠及数百万玩家。它也展示了 SDL3 在主要游戏引擎中的日益普及。 已知问题包括在 Windows 多显示器环境下和 Wayland 上进入独占全屏模式时可能崩溃。SDL3 的 LWJGL 绑定由 GTNH 模组包团队的一名成员贡献。

hackernews · ObviouslyFlamer · 7月19日 11:48 · [社区讨论](https://news.ycombinator.com/item?id=48967256)

**背景**: Simple DirectMedia Layer (SDL) 是一个跨平台库，提供对音频、键盘、鼠标、手柄和图形硬件的底层访问。SDL3 是最新主要版本，提供改进的性能和新功能。Minecraft 转向 SDL3 符合游戏引擎采用现代库以改善跨平台支持的更广泛趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Simple_DirectMedia_Layer">Simple DirectMedia Layer - Wikipedia</a></li>
<li><a href="https://www.studyplan.dev/sdl3/what-is-sdl">What is SDL? An Introduction for C++ Game Developers</a></li>

</ul>
</details>

**社区讨论**: 社区对此技术更新普遍持积极态度，部分人对全屏崩溃等阻塞性 bug 表示担忧。社区对模组贡献的 LWJGL 绑定表示赞赏，并分享了有用的移植资源。有评论者指出 Minecraft 正逐渐演变为一个独立的游戏引擎。

**标签**: `#Minecraft`, `#SDL3`, `#game development`, `#cross-platform`, `#open source`

---

<a id="item-4"></a>
## [Claude Code 采用用 Rust 重写的 Bun](https://simonwillison.net/2026/Jul/19/claude-code-in-bun-in-rust/#atom-everything) ⭐️ 8.0/10

Simon Willison 证实，Claude Code v2.1.181 及后续版本使用了从 Zig 重写为 Rust 的 Bun 运行时，在 Linux 上启动速度提升了 10%。 这一变化表明，一个重要的 AI 工具现在由基于 Rust 的 JavaScript 运行时驱动，突显了 Rust 在工具性能与安全性方面日益增长的重要性。同时也展示了使用 AI 辅助编码进行大规模运行时重写的可行性——此次重写正是借助 Claude Code 完成的。 Rust 版本的 Bun 尚未作为稳定版公开发布；Claude Code 搭载的是预览版，版本号为 Bun v1.4.0，而最新的公开版本是 v1.3.14。重写工作使用了约 50 个动态工作流在 11 天内完成。

rss · Simon Willison · 7月19日 03:54 · [社区讨论](https://news.ycombinator.com/item?id=48966569)

**背景**: Bun 是一个快速的全能型 JavaScript 运行时和工具包，最初使用 Zig 作为实现语言。最近，Bun 团队用 Rust 重写了运行时，以利用 Rust 的内存安全性和工具链优势。Claude Code 是 Anthropic 推出的 AI 编程助手，它将 Bun 作为底层的 JavaScript 运行时使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://bun.com/blog/bun-in-rust">Rewriting Bun in Rust | Bun Blog</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：有人质疑一个 TUI 为何需要 JavaScript 运行时，也有人理解从 Zig 转向 Rust 的技术理由。同时，对 Bun 开发的治理和透明度也存在担忧，尤其是考虑到这次快速而缺乏公开征求意见的 AI 辅助重写。

**标签**: `#Claude Code`, `#Bun`, `#Rust`, `#runtime`, `#AI tools`

---

<a id="item-5"></a>
## [卖出 2500 台 MIDI 录音机后的经验教训](https://chipweinberger.com/articles/20260719-hardware-is-not-so-hard) ⭐️ 8.0/10

文章作者分享了销售 2500 台 MIDI 录音机后的关键经验，认为硬件开发的难度取决于产品复杂度，而非硬件本身固有的困难。 这为有抱负的硬件创业者提供了实用见解，挑战了风投界普遍认为“硬件很难”的说法，并提供了关于规模化和设计的细致观点。 作者构建了一个只有 25 个组件且使用现成零件的简单产品，保持了设计的可控性。文章强调成功取决于产品复杂度和周密规划，而非神秘的难度。

hackernews · chipweinberger · 7月19日 10:34 · [社区讨论](https://news.ycombinator.com/item?id=48966713)

**背景**: 硬件初创企业通常面临规模化、物流和现金流等挑战。MIDI 录音机将音乐表演捕捉为 MIDI 数据，这是一种电子乐器标准协议。作者的产品 JamCorder 是一个简单、廉价的设备，无需应用程序即可将 MIDI 录制到 SD 卡。

**社区讨论**: 评论者普遍认为硬件难度因产品复杂度而异，有人指出规模化、物流和现金流是真正的挑战。一位用户称赞 JamCorder 是一款零投诉的完美产品。另一位则认为“硬件很难”是风投的过度简化。

**标签**: `#hardware`, `#MIDI`, `#entrepreneurship`, `#product development`, `#lessons learned`

---

<a id="item-6"></a>
## [fork() 如何不复制内存就复制进程](https://www.reddit.com/r/programming/comments/1v0uqah/how_fork_duplicates_a_process_without_copying_its/) ⭐️ 8.0/10

一个可视化解释展示了 Linux 的写时复制机制如何通过共享物理页面并仅在写入时复制，使得 fork() 能几乎瞬间复制一个 10 GB 的进程。 这种效率对系统编程至关重要：它实现了快速的进程创建，支持 Redis 快照而不需要双倍内存，并且是 Android Zygote 快速启动应用的基础。 该解释涵盖了 fork()+exec()、通过 fork 实现 Redis 快照、预加载通用类的 Android Zygote、延迟分配的惰性零页以及相关的 CVE 漏洞。

reddit · r/programming · /u/Ok_Marionberry8922 · 7月19日 16:16

**背景**: fork() 系统调用通过复制调用进程来创建新进程。如果没有写时复制，fork 一个大进程就需要复制其所有内存，既慢又浪费。写时复制将复制推迟到某个进程写入共享页面时才进行，从而实现了低开销的快速 fork()。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://source.android.com/docs/core/runtime/zygote">About the Zygote processes | Android Open Source Project</a></li>
<li><a href="https://en.wikipedia.org/wiki/Demand_paging">Demand paging - Wikipedia</a></li>
<li><a href="https://lwn.net/Articles/517465/">Adding a huge zero page [LWN.net]</a></li>

</ul>
</details>

**标签**: `#fork`, `#copy-on-write`, `#operating-systems`, `#linux`, `#memory-management`

---

<a id="item-7"></a>
## [AI 建议使自信倍增但准确性降低，研究显示](https://thenextweb.com/news/ai-advice-suppresses-critical-thinking-wrong-answers-study) ⭐️ 7.0/10

一项最新研究发现，获得 AI 建议的参与者比未使用 AI 的参与者准确率低三倍，但自信程度却高出两倍。 这凸显了对 AI 系统的危险过度依赖，用户对错误答案反而更自信，可能削弱现实应用中的批判性思维。 该研究使用了一个已知会在特定问题上给出错误答案的 LLM，参与者若不确定可以跳过问题，但依然陷入了自信陷阱。

hackernews · rbanffy · 7月19日 21:18 · [社区讨论](https://news.ycombinator.com/item?id=48971738)

**背景**: 该研究探讨了 AI 生成的建议如何影响人类决策，特别是准确性和自信程度。参与者需要在有或没有 AI 辅助的情况下回答问题。这项研究是人们对 AI 影响批判性思维日益担忧的一部分。

**社区讨论**: 社区评论观点混杂，一些人批评研究方法，指出该测试的是已知会给出错误答案的 AI 系统，而非 AI 的普遍可靠性。其他人则对 AI 削弱批判性思维和制造信息回音室表示更广泛的担忧。

**标签**: `#AI`, `#critical thinking`, `#study`, `#confidence`, `#accuracy`

---

<a id="item-8"></a>
## [OpenAI 将 Codex 的上下文窗口从 372k 减少至 272k](https://github.com/openai/codex/pull/33972/files) ⭐️ 7.0/10

OpenAI 通过官方仓库的一个拉取请求，将 Codex 模型的上下文窗口大小从 372,000 个 token 减少到 272,000 个 token。 这一变化引发了关于上下文压缩技术有效性以及上下文大小与模型性能之间权衡的讨论。它凸显了提供更大上下文与保持输出质量之间的持续张力，尤其是在涉及详细文档或代码库的复杂任务中。 这一减少意味着更依赖上下文压缩来将更多信息塞入较小的窗口，一些用户认为这会降低细节保留能力。拉取请求指出新限制为 272k token，低于之前的 372k。

hackernews · AmazingTurtle · 7月19日 07:54 · [社区讨论](https://news.ycombinator.com/item?id=48965850)

**背景**: OpenAI Codex 是一系列专为编码任务定制的大型语言模型，基于 GPT-3 并在 GitHub 仓库上训练。上下文压缩是一种压缩长对话或文档历史的技术，同时尽力保留关键信息，使模型能够在有限的上下文窗口内处理更长的交互。其代价是压缩可能会丢失细微细节，影响需要精确回忆的任务的性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(language_model)">OpenAI Codex (language model) - Wikipedia</a></li>
<li><a href="https://kargarisaac.medium.com/the-fundamentals-of-context-management-and-compaction-in-llms-171ea31741a2">The Fundamentals of Context Management and Compaction in LLMs</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了复杂情绪：一些用户感叹压缩后细节丢失，并批评从 372k 减少到 272k，指出像 Anthropic 这样的竞争对手提供更大的上下文。另一些人则认为过长的上下文会降低模型智能，最好保持在 300k 以下，而一些用户报告通过清除上下文并重新开始比依赖压缩获得更好的结果。

**标签**: `#OpenAI`, `#Codex`, `#context size`, `#LLM`, `#model optimization`

---

<a id="item-9"></a>
## [IndieWeb 之旅揭示优势与障碍](https://en.andros.dev/blog/0b8e451e/i-joined-the-indieweb-heres-what-i-learned/) ⭐️ 7.0/10

一篇个人博客文章详细描述了作者加入 IndieWeb 运动的经历，涵盖了拥有自己内容的赋权感以及设置 POSSE（在自己的网站上发布，然后分发到其他地方）协议的技术挑战。 这篇文章凸显了去中心化社交媒体中用户赋权与易用性之间的持续张力，这是人们寻求企业平台替代方案时的关键问题。 作者使用 Indiekit 等工具实现了 POSSE，但指出设置仍需要技术知识，限制了主流采用。

hackernews · andros · 7月19日 11:14 · [社区讨论](https://news.ycombinator.com/item?id=48966984)

**背景**: IndieWeb 是一项运动，倡导个人通过在自己的网站上发表内容并分发到社交媒体平台来拥有自己的数据。POSSE（在自己的网站上发布，然后分发到其他地方）是一种关键实践，即内容首先发布在自己的网站上，然后复制到其他平台，确保主要所有权归属于作者。这种方法与企业社交媒体形成对比，后者由平台控制内容。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/IndieWeb">IndieWeb - Wikipedia</a></li>
<li><a href="https://indieweb.org/POSSE">POSSE - IndieWeb</a></li>
<li><a href="https://en.wikipedia.org/wiki/IndieWebCamp">IndieWebCamp - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者表达了好坏参半的看法：有人批评 IndieWeb 的技术复杂性对大多数用户构成障碍，也有人称赞 Indiekit 和 Nostr 等工具作为更简单的替代方案。还有评论批评 IndieWeb 感觉上的精英主义，指出许多个人网站包含职业头像和简历，与反企业精神相矛盾。

**标签**: `#IndieWeb`, `#web development`, `#decentralization`, `#social media`, `#POSSE`

---

<a id="item-10"></a>
## [月之暗面因需求过大暂停 Kimi K3 新订阅](https://twitter.com/kimi_moonshot/status/2078855608565207130) ⭐️ 7.0/10

月之暗面因 48 小时内需求激增，暂时暂停其旗舰模型 Kimi K3 的新订阅，优先保障现有用户体验而非快速增长。 这一决定体现了以用户为先的服务理念，与一些悄然降低服务质量的厂商形成对比；也凸显了 Kimi K3 这类大规模开源模型的强劲需求。 Kimi K3 拥有 2.8 万亿参数，采用 Kimi Delta Attention 混合线性注意力机制，支持 100 万 token 上下文窗口。现有订阅用户不受影响。

hackernews · serialx · 7月19日 16:02 · [社区讨论](https://news.ycombinator.com/item?id=48969291)

**背景**: 月之暗面是一家 2023 年成立于北京的人工智能公司，属于中国“AI 六虎”之一。Kimi K3 于 2026 年 7 月发布，是全球首个开源的三万亿参数级模型，专为长上下文编程、推理和知识工作而设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Moonshot_AI">Moonshot AI - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kimi_K3">Kimi K3</a></li>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>

</ul>
</details>

**社区讨论**: 评论者高度赞扬月之暗面以用户为先的决定，有用户称“优先保障现有用户”是令人敬佩的做法。部分用户分享技术观察，指出 Kimi K3 广泛应用 RNN/线性注意力层，对长上下文任务效率很高。

**标签**: `#AI`, `#Moonshot`, `#Kimi K3`, `#subscriptions`, `#demand`

---

<a id="item-11"></a>
## [AI 狂热正在摧毁全球决策能力](https://simonwillison.net/2026/Jul/19/ai-mania/#atom-everything) ⭐️ 7.0/10

Nik Suresh 发表了一篇博文，批评 AI 炒作如何导致大公司做出非理性决策，文中用匿名轶事举例，如高管未使用过任何 AI 工具却推崇 AI 战略，以及工程师将代码库重写为 Zig 以显得自己很高效。 本文凸显了科技行业中一个普遍存在的问题：AI 炒作扭曲了决策过程，可能浪费资源并削弱真正的创新。它为高管和工程师敲响警钟，提醒 AI 应用要立足现实。 值得注意的轶事包括：一家营收超过 20 亿美元公司的高管从未使用过 ChatGPT，却批准了以 AI 为核心的技术战略；一名工程师让 AI 将一个 Go 仓库重写为 Zig，以提升在“代币排行榜”上的排名。另一个故事透露，供应商隐瞒真相，以免激怒那些相信不切实际的生产力提升的高管。

rss · Simon Willison · 7月19日 05:06

**背景**: 本文是科技行业对 AI 炒作持续批评的一部分。Zig 是一种类似 C 的系统编程语言，注重性能和安全性，常被用作 C 的替代品。ChatGPT 是广为人知的 AI 聊天机器人。该帖子在 Hacker News 上被分享，表明社区对此的关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://ziglang.org/">Home Zig Programming Language</a></li>

</ul>
</details>

**标签**: `#AI hype`, `#decision-making`, `#industry critique`, `#tech culture`

---

<a id="item-12"></a>
## [谷歌 IDE 发展史：一场历史回顾](https://www.reddit.com/r/programming/comments/1v0gkin/a_history_of_ides_at_google/) ⭐️ 7.0/10

一篇 Reddit 帖子回顾了谷歌多年来集成开发环境（IDE）的发展与采用历程。 这一回顾提供了关于谷歌这样的大型科技公司如何塑造其内部开发工具的有价值见解，可能影响行业趋势和最佳实践。 帖子详细描述了从早期编辑器到现代 IDE 的演变过程，突出了谷歌工程团队所做的关键决策和权衡。

reddit · r/programming · /u/fagnerbrack · 7月19日 04:17

**背景**: 集成开发环境（IDE）将代码编辑、调试和构建工具整合到一个应用程序中。谷歌多年来开发了多种内部工具，如 GoogleCL 以及 Eclipse 和 IntelliJ 的内部变体，最终采用了基于 IntelliJ IDEA 的现代解决方案。

**标签**: `#IDE`, `#Google`, `#software engineering`, `#history`, `#development tools`

---

<a id="item-13"></a>
## [分布式系统中的时间管理失误：一种故障模式](https://www.reddit.com/r/programming/comments/1v0snnz/beyond_happy_path_engineering_time/) ⭐️ 7.0/10

本文探讨了时钟漂移、截止时间不匹配、重试和 TTL 行为如何在分布式系统中导致实际事故，强调时间相关的假设在生产环境中常常失效。 理解这些故障模式对于构建可靠分布式系统的工程师至关重要，忽视时间问题可能导致数据损坏、性能下降和意外宕机。 文章描述了时钟漂移导致事件乱序、截止时间不匹配引发任务失败、重试放大负载以及 TTL 不一致产生陈旧数据的具体场景。

reddit · r/programming · /u/OtherwisePush6424 · 7月19日 14:54

**背景**: 分布式系统依赖时间进行协调、排序和故障检测。然而，不同机器上的时钟由于硬件缺陷不可避免地会漂移，完美同步是不可能的。像 NTP 这样的常见机制可以减少漂移但无法消除它，关于有界时钟偏差的假设经常失效。这使得基于时间的操作，如租约、心跳和缓存 TTL，容易出现在实际条件下才会显现的错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://flowfuse.com/blog/2026/07/time-synchronization-edge-devices/">Handling Clock Drift in Distributed Edge Devices • FlowFuse</a></li>
<li><a href="https://www.geeksforgeeks.org/distributed-systems/clock-synchronization-in-distributed-system/">Clock Synchronization in Distributed Systems - GeeksforGeeks</a></li>

</ul>
</details>

**标签**: `#distributed systems`, `#time`, `#fault tolerance`, `#reliability`

---

<a id="item-14"></a>
## [在 Plonky3 中构建 Merkle 树 AIR 脚本教程](https://www.reddit.com/r/programming/comments/1v0vext/a_tutorial_on_building_a_merkle_tree_air_script/) ⭐️ 7.0/10

一篇教程已发布，指导开发者如何使用 Plonky3 零知识证明框架创建 Merkle 树代数中间表示（AIR）脚本。 本教程帮助开发者获得 Plonky3 的实践经验，Plonky3 是一种先进的 ZK 证明系统，并演示了如何利用其模块化架构实现 Merkle 树证明。 教程涵盖了构建一个强制执行 Merkle 树打开约束的 AIR，利用 Plonky3 的多项式 IOP 工具包，该工具包支持多种承诺方案如 Brakedown。

reddit · r/programming · /u/badcryptobitch · 7月19日 16:43

**背景**: Plonky3 是由 Polygon Zero 开发的开源工具包，用于实现 PLONK 和 STARK 等多项式 IOP，专为高性能递归证明设计。AIR（代数中间表示）是一种将计算表示为连接执行轨迹行的多项式约束的方法，这是基于 STARK 的证明的核心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Plonky3/Plonky3">GitHub - Plonky3/Plonky3: A toolkit for polynomial IOPs (PIOPs) Polygon Plonky3 is Production Ready GitHub - Plonky3/awesome-plonky3: A curated list of Plonky3 ... Open Source Polygon Plonky3 Is Once Again the Fastest ZK ... Breaking Down Proof Construction in Plonky3: The Fibonacci ... Production-Ready: Plonky3, Polygon's Advanced Zero-Knowledge ...</a></li>
<li><a href="https://polygon.technology/blog/polygon-plonky3-the-next-generation-of-zk-proving-systems-is-production-ready">Polygon Plonky3 is Production Ready</a></li>
<li><a href="https://deepwiki.com/Plonky3/Plonky3/6-air-(algebraic-intermediate-representation)">AIR (Algebraic Intermediate Representation) | Plonky3/Plonky3 ...</a></li>

</ul>
</details>

**标签**: `#merkle-tree`, `#plonky3`, `#zero-knowledge-proofs`, `#tutorial`, `#cryptography`

---

<a id="item-15"></a>
## [最后一项 MPEG-4 视觉专利到期，Xvid/DivX 获解放](https://www.phoronix.com/news/Last-MPEG-4-Patent-Expired) ⭐️ 6.0/10

覆盖 MPEG-4 Visual（Part 2）的最后一项专利已到期，解除了对 Xvid 和 DivX 编解码器的专利限制。这项里程碑是在巴西持有的最后一项有效专利失效时达成的。 这标志着老牌视频编解码器的一个重要里程碑，使得 Xvid 和 DivX 的编码和分发可以不受限制地使用。然而，影响有限，因为更广泛使用的 H.264 编解码器在未来几年仍受专利保护。 这项到期专利是唯一在巴西仍有效的专利，美国和欧盟的 MPEG-4 Part 2 专利更早前已到期。需要注意的是，这适用于 MPEG-4 Part 2（基于 H.263），而非 H.264/AVC。

hackernews · LorenDB · 7月19日 16:45 · [社区讨论](https://news.ycombinator.com/item?id=48969635)

**背景**: MPEG-4 Visual 是上世纪 90 年代末作为 MPEG-4 系列一部分推出的视频压缩标准。Xvid 和 DivX 是实现 MPEG-4 Part 2 高级简单配置（ASP）的流行编解码器。专利限制先前阻碍了这些编解码器的开源使用和分发，而其到期允许无需许可费地自由使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/MPEG-4">MPEG-4 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/MPEG-4_Part_2">MPEG-4 Part 2 - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Xvid">Xvid - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者强调这涉及 MPEG-4 Part 2（Xvid/DivX）而非 H.264，批评 Phoronix 的报道可能具有误导性。一些用户期待 H.264 专利最终到期以及未来编解码器如 MPEG-5 的到来。

**标签**: `#patents`, `#video codecs`, `#MPEG-4`, `#Xvid`, `#DivX`

---

<a id="item-16"></a>
## [树莓派服务器重生：SSD 与迷你 PC 替代方案](https://sgt.hootr.club/blog/home-server-rebirth/) ⭐️ 6.0/10

一位用户记录了其家庭服务器从频繁出现 SD 卡损坏的树莓派，转向更可靠的 USB/SATA SSD，最终改用迷你 PC 的经历，突显了 SD 卡在 24/7 运行中的常见故障点。 这一经历揭示了业余家庭服务器中的一个普遍问题：树莓派 SD 卡因持续写入而损坏。它验证了转向 USB/SATA SSD 或低功耗 x86 迷你 PC 以提高可靠性和性能的趋势。 用户最初使用树莓派 4B 和 SD 卡，但 SD 卡反复损坏后失败。他们升级到树莓派 5，配合 Waveshare PoE+SSD 扩展板实现 SATA SSD 启动，后来考虑改用 Intel NUC 等迷你 PC 以获得更好的内存容量和 NVMe 支持。

hackernews · steinuil · 7月19日 10:44 · [社区讨论](https://news.ycombinator.com/item?id=48966769)

**背景**: 树莓派因其低功耗和低成本常用于家庭服务器，但 microSD 卡写入寿命有限，在 Home Assistant 或 Docker 等服务的持续日志或数据库写入下容易损坏。USB/SATA SSD 提供更高的可靠性和性能，而 x86 迷你 PC 则通过标准内存和存储接口提供更大的灵活性。现代树莓派的引导加载程序已原生支持 USB 启动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://raspberry.tips/en/calculate-raspberry-pi-sd-card-lifespan-test-now">Calculate Raspberry Pi SD Card Lifespan : Test Now!</a></li>
<li><a href="https://raspberrytips.com/raspberry-pi-storage-showdown/">Raspberry Pi Storage Options Compared: SD, USB, SSD & NVMe</a></li>

</ul>
</details>

**社区讨论**: 评论者们普遍认同 SD 卡易损的特性，有人分享了对策如制作多张 SD 卡镜像以便快速更换，或使用 USB 闪存盘。还有人推荐在 Rockchip SBC 上使用 NVMe，或称赞 Waveshare 扩展板的便利性。一位用户指出，尽管其他组件便宜，但内存价格使迷你 PC 吸引力下降。

**标签**: `#home server`, `#Raspberry Pi`, `#SD card`, `#storage`, `#hobbyist`

---

<a id="item-17"></a>
## [五菱缤果可能换标雪佛兰进军北美](https://electrek.co/2026/07/19/chinese-wuling-bingo-could-come-to-north-america-as-an-entry-level-chevy-ev/) ⭐️ 6.0/10

有传言称，中国五菱缤果电动汽车可能换标成雪佛兰入门级电动车进入全球市场，有望延续 Geo Metro 的精神。 如果属实，这将为北美带来一款低成本电动车，利用通用与上汽通用五菱的合作提供平价电动车选择，可能与其他廉价电动车竞争，并重振省油 Geo Metro 的传奇。 五菱缤果是上汽通用五菱（SGMW）生产的一款超紧凑型掀背车，该公司是上汽、通用和柳州五菱的合资企业。Geo Metro 是 90 年代通用与铃木的合作项目，以燃油经济性著称。

rss · Electrek · 7月19日 22:28

**背景**: 五菱缤果（Bingo/Binguo）是上汽通用五菱于 2023 年在中国推出的一款纯电动超紧凑型掀背车，以其复古未来主义设计和亲民价格著称。Geo Metro 是 1989 年至 2001 年在北美销售的一款紧凑型车，由通用和铃木共同开发，以低成本和高燃油效率著称。将缤果换标为雪佛兰，将遵循类似的策略，在熟悉的品牌下提供入门级车型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wuling_Bingo_Plus">Wuling Bingo Plus</a></li>
<li><a href="https://en.wikipedia.org/wiki/Geo_Metro">Geo Metro - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Geo_(automobile)">Geo (automobile) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#electric vehicles`, `#Chevy`, `#Wuling`, `#automotive rumors`, `#North America`

---

<a id="item-18"></a>
## [transcribe.cpp：开源 C++语音转文本推理库](https://www.reddit.com/r/programming/comments/1v0woh5/transcribecpp/) ⭐️ 6.0/10

transcribe.cpp 发布，这是一个基于 ggml 的 C/C++ 语音转文本推理库，支持 16 种模型家族和 60 多个变体，具备 Metal、Vulkan 和 CUDA 等 GPU 后端，以及由 tinyBLAS 加速的 CPU 路径。 该库使在本地应用中快速集成语音转文本变得更加容易，无需依赖云服务，从而增强隐私并降低延迟。它对多种模型家族的支持为开发者提供了灵活性。 该库使用 GGUF 模型格式进行推理，并经过数值验证和词错误率（WER）测试，以匹配参考实现。由 Mozilla.ai 通过其 Builders in Residence 项目开发。

reddit · r/programming · /u/namanyayg · 7月19日 17:32

**背景**: ggml 是一个用于机器学习推理的张量库，针对 CPU 和 GPU 性能进行了优化。语音转文本（STT）模型将音频转录为文字。transcribe.cpp 基于 ggml，支持 Whisper 等多种 STT 模型，实现无需云依赖的本地转录。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/handy-computer/transcribe.cpp">GitHub - handy-computer/transcribe.cpp: ggml speech-to-text ...</a></li>
<li><a href="https://blog.mozilla.ai/announcing-transcribe-cpp/">Announcing transcribe.cpp</a></li>

</ul>
</details>

**标签**: `#C++`, `#transcription`, `#machine learning`, `#open source`, `#tool`

---

<a id="item-19"></a>
## [普通 C 语言中的交换性复数理论](https://www.reddit.com/r/programming/comments/1v0of6b/commutative_complex_number_theory_in_plain_c/) ⭐️ 6.0/10

一个 C 语言实现展示了复数运算的交换性，探讨了在语言约束下的理论特性。 这提供了一种新颖的教学方式，有助于理解复数以及 C 的类型系统，但仍属于小众的学术练习。 该实现可能使用结构体以及通过宏或函数实现的运算符重载来达成交换性，可能包含自定义的加法和乘法例程。

reddit · r/programming · /u/DataBaeBee · 7月19日 11:45

**背景**: C 语言不原生支持复数，因此开发者通常将复数实现为包含实部和虚部的结构体。交换性意味着 a * b 等于 b * a，这对于复数乘法是成立的，但在代码中贯彻这一特性需要细致处理。

**标签**: `#C`, `#complex numbers`, `#mathematics`, `#programming`

---

<a id="item-20"></a>
## [真实世界的 CPU 瓶颈调试故事](https://www.reddit.com/r/programming/comments/1v0llyh/finding_zombies_in_our_systems_a_realworld_story/) ⭐️ 6.0/10

一位开发者分享了一个真实案例，讲述如何识别并修复由僵尸进程导致的 CPU 瓶颈问题。 这个故事提供了性能调试和系统监控的实用见解，帮助工程师避免在自己的系统中犯类似错误。 诊断过程涉及追踪积累并消耗 CPU 资源的僵尸进程，凸显了正确进程管理和监控工具的重要性。

reddit · r/programming · /u/fagnerbrack · 7月19日 09:04

**背景**: 僵尸进程是已终止但仍然在进程表中留有记录的子进程，因为其父进程尚未读取其退出状态。在 Linux 中，这类进程在 ps 等工具中显示为'Z'状态。虽然通常存活时间很短，但累积的僵尸进程可能耗尽系统资源并导致 CPU 瓶颈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@nirbhaysingh281/what-is-a-zombie-process-3576a4ac9bee">What is a zombie process ?. Definition of a Zombie Process | Medium</a></li>
<li><a href="https://www.geeksforgeeks.org/operating-systems/difference-between-zombie-orphan-and-daemon-processes/">Difference between Zombie , Orphan and Daemon Processes</a></li>

</ul>
</details>

**标签**: `#performance`, `#debugging`, `#CPU`, `#systems`, `#real-world`

---

<a id="item-21"></a>
## [使用 Bubble Tea 在 Go 中开发终端用户界面](https://www.reddit.com/r/programming/comments/1v0xaws/developing_a_tui_in_go_with_bubble_tea/) ⭐️ 6.0/10

Reddit 上分享了一篇教程，介绍如何使用 Bubble Tea 框架在 Go 中构建终端用户界面（TUI），为开发者提供了创建交互式终端应用的实用指南。 TUI 应用对于命令行工具和系统实用程序很有价值，而 Bubble Tea 基于 Elm 的架构简化了状态管理和事件处理，使 Go 成为开发终端软件的更优选择。 Bubble Tea 采用受 Elm 架构启发的模型-更新-视图模式，其中消息在 Update() 中处理，UI 在 View() 中渲染。为了减少界面延迟，这两个函数必须保持高效。

reddit · r/programming · /u/der_gopher · 7月19日 17:56

**背景**: 终端用户界面（TUI）是一种基于文本的界面，运行在终端模拟器中，通过字符和颜色展示交互组件。Bubble Tea 是一个 Go 框架，实现了 Elm 架构（TEA）——一种通过不可变状态和消息传递构建响应式 UI 的模式。它适用于简单到复杂的终端应用，支持内嵌、全屏或混合模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/charmbracelet/bubbletea">GitHub - charmbracelet/ bubbletea : A powerful little TUI framework</a></li>
<li><a href="https://en.wikipedia.org/wiki/Text-based_user_interface">Text-based user interface - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Go`, `#TUI`, `#Bubble Tea`, `#Programming Tutorial`

---