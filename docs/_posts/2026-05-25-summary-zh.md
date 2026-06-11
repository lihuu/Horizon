---
layout: default
title: "Horizon Summary: 2026-05-25 (ZH)"
date: 2026-05-25
lang: zh
---

> From 33 items, 25 important content pieces were selected

---

1. [LLM 智能体在后端代码生成中表现出约束衰减](#item-1) ⭐️ 8.0/10
2. [微软开源最早 DOS 源代码](#item-2) ⭐️ 8.0/10
3. [诈骗者滥用微软内部账户发送垃圾邮件](#item-3) ⭐️ 8.0/10
4. [16 字节演示程序创造视听奇迹](#item-4) ⭐️ 8.0/10
5. [AMD 将在 2026.1 版本中移除免费 Vivado 层级的 Linux 支持](#item-5) ⭐️ 8.0/10
6. [批评 AI 错误报告，提倡简单格式](#item-6) ⭐️ 8.0/10
7. [PapersWithCode 复活版新增多指标支持](#item-7) ⭐️ 8.0/10
8. [BitCPM-CANN：在昇腾 NPU 上实现原生 1.58 位 LLM 训练](#item-8) ⭐️ 8.0/10
9. [DeepSeek 发布 Reasonix：低成本原生编码代理](#item-9) ⭐️ 7.0/10
10. [存储器成本已占 AI 芯片组件成本的近三分之二](#item-10) ⭐️ 7.0/10
11. [格雷格·布罗克曼访谈讨论 OpenAI 与 AI 行业](#item-11) ⭐️ 7.0/10
12. [CBP 加强边境电子设备搜查程序](#item-12) ⭐️ 7.0/10
13. [Usborne 1980 年代计算机书籍激励一代代程序员](#item-13) ⭐️ 7.0/10
14. [社区比较 Qwen3.6 与 Gemma4 模型](#item-14) ⭐️ 7.0/10
15. [无审查模型的实际用途远不止角色扮演](#item-15) ⭐️ 7.0/10
16. [特斯拉在中国将 FSD 更名为“特斯拉辅助驾驶”](#item-16) ⭐️ 7.0/10
17. [视觉 LLM 在长文档问答基准测试中不如 OCR](#item-17) ⭐️ 7.0/10
18. [掌握 Dyalog APL：交互式书籍发布](#item-18) ⭐️ 6.0/10
19. [早期计算体验的怀旧回顾](#item-19) ⭐️ 6.0/10
20. [Ruby for Good：社会公益项目维护者聚会](#item-20) ⭐️ 6.0/10
21. [Datasette 1.0a30 新增可定制的“跳转到”菜单和插件钩子](#item-21) ⭐️ 6.0/10
22. [AI 复活 1980 年代 Usborne 游戏为交互式网页应用](#item-22) ⭐️ 6.0/10
23. [质疑 NVIDIA 在 2026 年本地 LLM 中的主导地位](#item-23) ⭐️ 6.0/10
24. [Qwen3.6-35B-A3B 无审查模型在迷你 PC 上运行 20 万上下文](#item-24) ⭐️ 6.0/10
25. [探索超越 SQL 和 NoSQL 的专用数据库引擎](#item-25) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [LLM 智能体在后端代码生成中表现出约束衰减](https://arxiv.org/abs/2605.06445) ⭐️ 8.0/10

一项系统性研究表明，当 LLM 智能体受到架构规则约束时，其断言通过率平均下降约 30 个百分点，这一现象被称为“约束衰减”。 这揭示了在生产级后端开发中使用 LLM 智能体时存在的关键可靠性差距，因为此类开发通常有严格的架构约束，从而削弱了对 AI 生成复杂系统代码的信任。 该研究在多文件后端生成任务中测试了 LLM 智能体，逐步添加 ORM 模式、框架约定等约束条件，发现性能下降主要集中在约定密集的框架中。

hackernews · wek · May 24, 12:55 · [社区讨论](https://news.ycombinator.com/item?id=48256912)

**背景**: 基于 LLM 的编码智能体是从自然语言提示生成代码的 AI 系统。虽然它们在无约束任务（如原型开发）中表现出色，但在遵循特定架构规则时的可靠性此前研究不足。约束衰减是指随着结构要求增加，生成质量显著下降的现象。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.06445">[2605.06445] Constraint Decay : The Fragility of LLM Agents in...</a></li>
<li><a href="https://www.alphaxiv.org/overview/2605.06445v1">Constraint Decay : The Fragility of LLM Agents in Backend... | alphaXiv</a></li>
<li><a href="https://agentpatterns.ai/verification/constraint-decay-backend-agents/">Constraint Decay in Backend Code Generation - AgentPatterns.ai</a></li>

</ul>
</details>

**社区讨论**: 评论者指出与长周期任务错误的相似性，并建议逐步引入约束或使用外部编排器等缓解策略。部分人批评该研究因成本问题未使用前沿模型，限制了结论的普适性。

**标签**: `#LLM agents`, `#code generation`, `#constraint decay`, `#backend development`, `#AI reliability`

---

<a id="item-2"></a>
## [微软开源最早 DOS 源代码](https://arstechnica.com/gadgets/2026/04/microsoft-open-sources-the-earliest-dos-source-code-discovered-to-date/) ⭐️ 8.0/10

微软开源了已知最早的 DOS 源代码，该代码是由历史学家和保存专家组成的团队通过 OCR 从纸质打印件中恢复的。这标志着对计算历史基础部分的一次重要保存努力。 此次发布保存了塑造个人电脑行业的关键软件历史片段，使其可供开源社区研究和保存。这也体现了微软对透明度和历史保护的承诺。 源代码是从 Tim Paterson（DOS 的原始开发者）提供的纸质打印件转录而来，现代 OCR 软件在处理几十年历史的打印质量时遇到了困难。这项工作由 Yufeng Gao 和 Rich Cini 领导，是“DOS 反汇编小组”的一部分。

hackernews · DamnInteresting · May 24, 01:21 · [社区讨论](https://news.ycombinator.com/item?id=48253386)

**背景**: DOS（磁盘操作系统）是早期 IBM PC 及其兼容机的基础操作系统，由微软在 20 世纪 80 年代初开发。该源代码当时并未以数字形式存储，只能从物理打印件中恢复，因此这次开源是一项非凡的历史成就。

**社区讨论**: 社区普遍称赞这一努力，有用户感谢微软，并指出同时开源的早期 BASIC 代码。另一用户羡慕当时只需几千行汇编代码就能创办成功的软件公司。有评论强调了从旧纸质打印件进行 OCR 的困难。

**标签**: `#open source`, `#DOS`, `#Microsoft`, `#history`, `#preservation`

---

<a id="item-3"></a>
## [诈骗者滥用微软内部账户发送垃圾邮件](https://techcrunch.com/2026/05/21/scammers-are-abusing-an-internal-microsoft-account-to-send-spam/) ⭐️ 8.0/10

诈骗者正利用一个合法的微软内部电子邮件账户发送垃圾邮件和钓鱼链接，从而绕过传统的电子邮件安全过滤。 这一漏洞削弱了对微软电子邮件安全的信任，可能导致大规模的钓鱼攻击，而这些攻击看起来来自可信的来源。 被滥用的账户通常用于发送真实的账户警报，这使得收件人很难区分合法邮件和垃圾邮件。

hackernews · spike021 · May 24, 00:51 · [社区讨论](https://news.ycombinator.com/item?id=48253186)

**背景**: 微软使用多个域名进行官方通信，但管理大量域名资产可能导致安全漏洞。SPF、DKIM 和 DMARC 等电子邮件认证方法旨在防止伪造，但内部账户可能绕过这些检查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/05/21/scammers-are-abusing-an-internal-microsoft-account-to-send-spam/">Scammers are abusing an internal Microsoft account to send ...</a></li>
<li><a href="https://sesamedisk.com/microsoft-internal-account-abuse-2026-cybersecurity/">Microsoft Internal Account Abuse in 2026: Cybersecurity ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论表达了对微软域名管理的不满，指出即使是内部用户也不确定所有合法域名。一些用户分享了个人遭遇钓鱼尝试和微软安全响应不足的经历。

**标签**: `#security`, `#microsoft`, `#spam`, `#phishing`

---

<a id="item-4"></a>
## [16 字节演示程序创造视听奇迹](https://hellmood.111mb.de/wake_up_16b_writeup.html) ⭐️ 8.0/10

一篇分析文章解释了如何通过极致的代码优化和体积编码技术，让一个仅 16 字节的可执行演示程序“Wake up! 16b”产生视听输出。 该演示将体积编码的边界推向极致，证明在仅 16 字节内即可实现复杂的视听效果，激励了演示场景和底层编程社区进一步创新。 该演示体积仅 16 字节，远小于常见的 64k 或 4k intro，却能同时产生声音和画面。文章详细介绍了实现这种极致压缩所使用的具体优化技巧。

hackernews · MaximilianEmel · May 24, 00:30 · [社区讨论](https://news.ycombinator.com/item?id=48253060)

**背景**: 演示场景（demoscene）是一种计算机艺术亚文化，程序员创建自包含的视听演示，通常有严格的体积限制，如 64k 或 4k 字节。体积编码（size coding）是编写极其紧凑代码的实践，常用技术包括指令重叠和自修改代码。这个 16 字节的演示代表了该传统中的一项极致成就。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Demoscene">Demoscene</a></li>
<li><a href="http://www.sizecoding.org/wiki/Main_Page">SizeCoding.org</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了敬畏和钦佩，有人称之为“巫术”，另一个人说这让他们陷入了一个探索深坑。社区参与度很高，对技术成就赞赏有加，有人指出它超越了之前的 32 字节演示，并且包含了声音。

**标签**: `#demoscene`, `#size coding`, `#optimization`, `#low-level programming`

---

<a id="item-5"></a>
## [AMD 将在 2026.1 版本中移除免费 Vivado 层级的 Linux 支持](https://adaptivesupport.amd.com/s/question/0D5Pd00001YQLdMKAX/why-is-vivado-20261-dropping-linux-support-for-free-tier-?language=en_US) ⭐️ 8.0/10

AMD 宣布，从 2026.1 版本开始，免费版 Vivado（Vivado ML Standard）将不再支持 Linux，而 Windows 支持仍将继续。 这一决定疏远了依赖 Linux 进行 FPGA 开发的学生、爱好者和开发者，可能缩小 AMD/Xilinx 生态系统，并推动用户转向 Lattice 等竞争对手。 免费版 Vivado（原 WebPACK）是 AMD FPGA 唯一免费的选择；移除 Linux 支持迫使 Linux 用户要么转向 Windows，要么购买昂贵的付费许可证以获得完整功能版本。

hackernews · zdw · May 24, 04:14 · [社区讨论](https://news.ycombinator.com/item?id=48254309)

**背景**: Vivado 是 AMD（原 Xilinx）的 FPGA 设计套件。免费版 WebPACK/Standard 提供有限功能且无需费用。历史上，Vivado 同时支持 Windows 和 Linux，Linux 因适用于服务器和自动化工作流而受到许多开发者青睐。AMD 收购 Xilinx 引发了关于优先级转向企业许可的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vivado">Vivado - Wikipedia</a></li>
<li><a href="https://wiki.archlinux.org/title/Xilinx_Vivado">Xilinx Vivado - ArchWiki</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了强烈反对：用户批评 AMD 忽视 Linux 用户需求，指出这将损害生态系统并带来许可麻烦，一些人正转向 Lattice 或 Altera。长期 AMD 用户认为，收购后公司不再理解其客户群体。

**标签**: `#FPGA`, `#AMD`, `#Vivado`, `#Linux`, `#EDA tools`

---

<a id="item-6"></a>
## [批评 AI 错误报告，提倡简单格式](https://simonwillison.net/2026/May/24/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Flask 等流行 Python 工具的创建者 Armin Ronacher 发表博客，批评其开源项目 Pi 中泛滥的 AI 生成错误报告，并提倡一种简单的、基于人类观察的问题提交流程。 这一批评凸显了开源维护中日益严重的问题：AI 生成的错误报告以自信但不准确的分析浪费维护者时间。它呼吁回归简洁、由人类撰写的错误报告，以保持项目的健康。 Ronacher 提出的格式仅需四个要素：运行的命令、预期行为、实际行为以及确切的错误或日志。他强调 AI 的重写去掉了人类的声音，并注入了推测性的结论。

rss · Simon Willison · May 24, 18:46

**背景**: 错误报告对开源维护至关重要，它让开发者能够重现并修复问题。随着 AI 编程助手的兴起，许多用户开始提交由大型语言模型（LLM）生成或增强的问题报告，这些报告往往冗长、不准确且过于自信。这种被称为“slop”的现象加重了维护者的负担，损害了协作过程。

**标签**: `#open-source`, `#bug reports`, `#AI`, `#software maintenance`, `#issue tracking`

---

<a id="item-7"></a>
## [PapersWithCode 复活版新增多指标支持](https://www.reddit.com/r/MachineLearning/comments/1tmawv5/paperswithcode_new_features_week_1_p/) ⭐️ 8.0/10

来自 Hugging Face 的 NielsRogge 宣布了复活版 PapersWithCode.co 的新功能，包括每个基准支持多个指标，以及可从 GitHub、博客文章等外部来源提交论文。 此次更新增强了平台追踪最先进模型的实用性，允许在效率和准确性指标上进行更丰富的比较，并使研究人员更容易提交非 Arxiv 的论文。 多指标排行榜现在支持 ASR 的字错误率 (WER) 和逆实时因子 (RTFx) 等指标，以及 COCO 目标检测的 mAP 和 FPS。通过专用表单支持外部论文提交，并自动丰富信息。

reddit · r/MachineLearning · NielsRogge · May 24, 12:31

**背景**: PapersWithCode 曾是跟踪机器学习最先进成果的流行网站，但被前所有者关闭。Hugging Face 以开源社区驱动平台 PapersWithCode.co 的形式将其复活。多指标排行榜允许在准确性和效率上比较模型，这对实际部署越来越重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/inverse-real-time-factor-rtfx">Inverse Real - Time Factor ( RTFx ) in ASR</a></li>
<li><a href="https://huggingface.co/spaces/hf-audio/open_asr_leaderboard">Open ASR Leaderboard - a Hugging Face Space by hf-audio</a></li>
<li><a href="https://arxiv.org/html/2510.06961v1">Open ASR Leaderboard: Towards Reproducible and Transparent ...</a></li>

</ul>
</details>

**社区讨论**: 社区反响热烈，评论者赞扬这项工作，并寻求帮助或功能，例如添加缺失 GitHub 链接的论文认领机制。一位用户询问其与 Hugging Face 每日论文版块相比的优势。

**标签**: `#paperswithcode`, `#open-source`, `#machine-learning`, `#leaderboard`, `#state-of-the-art`

---

<a id="item-8"></a>
## [BitCPM-CANN：在昇腾 NPU 上实现原生 1.58 位 LLM 训练](https://www.reddit.com/r/LocalLLaMA/comments/1tmf63y/bitcpmcann_native_158bit_large_language_model/) ⭐️ 8.0/10

来自 OpenBMB 的研究人员推出 BitCPM-CANN，这是一系列在华为昇腾 NPU 上原生训练的 1.58 位三元 LLM，训练开销仅增加 4.5%，推理时内存节省高达 8 倍。 这项工作表明，极端低位训练在 CUDA 生态之外也是可行的，这使得在昇腾 NPU 等替代硬件上实现高效 AI 成为可能，有助于减少对 Nvidia GPU 的依赖并降低部署成本。 BitCPM-CANN 模型（0.5B 到 8B）在推理基准测试上保留了全精度性能的 90-97%，其中 3B 和 8B 版本在 GSM8K 和 BBH 上几乎达到全精度水平。QAT 集成仅增加 4.5%的训练吞吐量开销，使三元训练成为可行的默认设置。

reddit · r/LocalLLaMA · Aaaaaaaaaeeeee · May 24, 15:24

**背景**: 1.58 位量化（又称三元量化）将权重限制为三个值（-1、0、+1），大幅减少内存和计算。CANN（神经网络计算架构）是华为为昇腾 NPU 打造的异构计算平台。MindSpeed 是面向昇腾 NPU 生态的分布式训练框架，基于 Megatron-LM 适配。此前 1.58 位 LLM 大多在 CUDA 上训练，因此这项工作是将此类模型移植到替代硬件上的重要进展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/1.58-bit_large_language_model">1.58-bit large language model - Wikipedia</a></li>
<li><a href="https://www.hiascend.com/document/detail/en/canncommercial/800/quickstart/index/index.html">Overview-Quick Start- CANN commercial edition8.0.0开发文档-昇腾社区</a></li>
<li><a href="https://deepwiki.com/moguizhizi/MindSpeed-LLM">moguizhizi/ MindSpeed -LLM | DeepWiki</a></li>

</ul>
</details>

**社区讨论**: Reddit 社区表现出浓厚兴趣，评论称赞其极低的训练开销和内存节省，但也指出 0.5B 模型在数学任务上表现欠佳。一些用户测试了模型并认为小规模模型智能有限，但仍承认在不依赖 Nvidia 硬件的情况下实现三元模型运行是重要成就。用户们期待更大规模模型以这种格式推出。

**标签**: `#LLM`, `#quantization`, `#Ascend NPU`, `#ternary`, `#efficient AI`

---

<a id="item-9"></a>
## [DeepSeek 发布 Reasonix：低成本原生编码代理](https://esengine.github.io/DeepSeek-Reasonix/) ⭐️ 7.0/10

DeepSeek 推出了 Reasonix，这是一个终端原生 AI 编码代理，专为 DeepSeek API 设计，具有缓存优先循环以降低 token 成本，并支持通过 Ollama 或 DeepSeek 托管的本地嵌入。 Reasonix 通过优化缓存效率直接解决了 AI 编码助手的 API 成本痛点，可能显著降低使用 DeepSeek 模型的开发者的开支。这也标志着 AI 实验室开始创建定制工具以更好地利用其 API 的独特优势。 该代理围绕前缀缓存稳定性设计，旨在长时间会话中保持低 token 成本。它已在 GitHub 上发布，并与 DeepSeek API 直接集成，但社区评论指出了宣传网站的 UX 问题，并质疑是否有必要专门开发一个代理，因为现有工具已经可以利用 DeepSeek 的缓存。

hackernews · Alifatisk · May 24, 13:02 · [社区讨论](https://news.ycombinator.com/item?id=48256953)

**背景**: 像 GitHub Copilot 和 Codex 这样的 AI 编码代理使用大语言模型辅助代码生成，通常按处理的 token 收费。缓存策略，尤其是前缀缓存，可以减少重复计算并降低 API 费用。DeepSeek 是一家以竞争性定价和高性能模型闻名的 AI 研究实验室。Reasonix 旨在最大化 DeepSeek API 的缓存优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://esengine.github.io/DeepSeek-Reasonix/">Reasonix — DeepSeek -native AI coding agent</a></li>
<li><a href="https://api-docs.deepseek.com/quick_start/agent_integrations/reasonix">Integrate with Reasonix | DeepSeek API Docs</a></li>
<li><a href="https://github.com/esengine/DeepSeek-Reasonix">GitHub - esengine/ DeepSeek - Reasonix : DeepSeek -native AI coding...</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些人赞赏其成本优化潜力，另一些人则批评网站的用户体验（例如动画打字导致内容移动），并认为现有的开源框架如 opencode 已经能有效利用 DeepSeek 的缓存。此外，关于最佳缓存策略以及是否需要专门代理也存在争论。

**标签**: `#AI coding agent`, `#DeepSeek`, `#caching`, `#low cost`, `#software engineering`

---

<a id="item-10"></a>
## [存储器成本已占 AI 芯片组件成本的近三分之二](https://epoch.ai/data-insights/ai-chip-component-cost-shares) ⭐️ 7.0/10

由于 AI 加速器对高带宽存储器（HBM）的需求激增，存储器成本已上升至占 AI 芯片组件总成本的近三分之二。 这一成本结构变化揭示了硬件降本的重要路径：随着 HBM 供需趋于平衡，AI 训练和推理成本可在无技术创新的情况下降低约 3 倍。 高带宽存储器（HBM）通过硅通孔（TSV）垂直堆叠多个 DRAM 晶粒并安装在中介层上，提供极高带宽，但每吉字节消耗的晶圆面积约为 DDR5 的三倍。

hackernews · intelkishan · May 24, 16:31 · [社区讨论](https://news.ycombinator.com/item?id=48258684)

**背景**: HBM 是专为 AI 加速器（如 NVIDIA H100 和 B200）设计的特种 DRAM，提供比传统 RAM 高得多的带宽。AI 带来的空前需求导致 DRAM 价格暴涨——自 2025 年初以来部分涨幅超过 200%——存储器已成为芯片组件中的主要成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/ram/hbm-is-eating-your-ram">Here's why HBM is coming for your PC's RAM — HBM consumes around three times the wafer capacity of DDR5 per gigabyte, as AI supercharges demand for chips and advanced packaging | Tom's Hardware</a></li>
<li><a href="https://introl.com/blog/ai-memory-supercycle-hbm-2026">The AI Memory Supercycle | Introl Blog</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，等待 DRAM 供应稳定可能带来约 3 倍的硬件成本降低；其他人则感受到个人硬件价格上涨（如 96GB 内存从 250 美元涨到 1200 美元）。一些人质疑 DRAM 容量每年约 20-25%的增长能否跟上 AI 需求。

**标签**: `#AI hardware`, `#memory costs`, `#DRAM`, `#semiconductor industry`, `#cost analysis`

---

<a id="item-11"></a>
## [格雷格·布罗克曼访谈讨论 OpenAI 与 AI 行业](https://fs.blog/knowledge-project-podcast/greg-brockman/) ⭐️ 7.0/10

OpenAI 联合创始人格雷格·布罗克曼参加《知识项目》播客，讨论 OpenAI 的发展历程、治理结构和人工智能进展。 此次访谈提供了对 OpenAI 内部动态及更广泛 AI 行业的见解，引发了关于公司治理和非营利组织诚信的社区讨论。 访谈涉及 OpenAI 从非营利向有限利润的转变，并提及埃隆·马斯克诉讼中公开的个人日记，马斯克因提交过晚而败诉。

hackernews · prakashqwerty · May 24, 08:29 · [社区讨论](https://news.ycombinator.com/item?id=48255593)

**背景**: OpenAI 最初是作为非营利性 AI 研究实验室成立的，但后来创建了有限利润部门以吸引资金。这种结构一直存在争议，批评者认为它削弱了非营利原则。社区还讨论了 Ilya Sutskever 等人物以及与 Anthropic 的企业竞争。

**社区讨论**: 评论者对非营利组织的诚信表示怀疑，一位用户质疑非营利组织为何被允许转变为营利实体。另一位指出布罗克曼的个人日记揭示了财务野心，加剧了不信任。一些评论将焦点转向 Anthropic，认为其现在更为重要。

**标签**: `#Greg Brockman`, `#OpenAI`, `#AI interview`, `#AI industry`, `#Hacker News discussion`

---

<a id="item-12"></a>
## [CBP 加强边境电子设备搜查程序](https://www.cbp.gov/document/directives/cbp-directive-no-3340-049b-border-search-electronic-devices) ⭐️ 7.0/10

美国海关与边境保护局（CBP）于 2025 年 1 月发布了第 3340-049B 号指令，更新了在边境搜查电子设备的程序，包括处理密码保护和加密数据的规定。 该指令极大地影响了旅行者在美国边境的数字隐私，因为它正式确立了广泛的搜查权力，同时通过不公开的“国家安全”例外创造了法律漏洞。 指令明确规定旅行者必须提供设备访问权限，但不得使用密码访问仅远程存储的数据（第 5.3.2 条）。它还表示，除非国家安全需要，否则 CBP 不会侵犯隐私，且此类情况无需披露。

hackernews · Ember_Wipe · May 24, 19:12 · [社区讨论](https://news.ycombinator.com/item?id=48260140)

**背景**: CBP 依据第四修正案的“边境搜查例外”运作，允许在国际边境进行无证搜查。本指令更新了 2009 年的政策（第 3340-049 号指令），旨在在加密设备使用日益增多的背景下平衡国家安全与隐私问题。

**社区讨论**: 评论者表达了不信任，指出指令中的国家安全条款实际上允许无限制搜查且无需问责。一些人批评该例外规定的模糊性，而另一些人则指出类似做法自 2009 年就已存在，并建议旅行时使用一次性设备。

**标签**: `#privacy`, `#border search`, `#electronic devices`, `#CBP`, `#digital rights`

---

<a id="item-13"></a>
## [Usborne 1980 年代计算机书籍激励一代代程序员](https://usborne.com/us/books/computer-and-coding-books) ⭐️ 7.0/10

Usborne 出版社将其经典的 1980 年代计算机书籍以免费 PDF 下载形式发布，重新点燃了早期程序员们的回忆和赞赏。 这些书籍通过生动的插图和实际项目向众多年轻读者介绍了编程概念，塑造了早期的计算生态，并激励了无数人的职业生涯。 该系列包括《练习你的 BASIC》、《机器码入门》和机器人制作指南等书籍，最初于 1980 年代出版，现已免费开放。

hackernews · ngram · May 24, 15:43 · [社区讨论](https://news.ycombinator.com/item?id=48258194)

**背景**: 在 20 世纪 80 年代，ZX Spectrum、Commodore 64 和 Amstrad CPC 等家用微型计算机开始流行。Usborne 的书籍教给一代人如何用 BASIC 和机器码编程，通常成为互联网时代之前唯一的教育资源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://retrocomputingforum.com/t/usborne-1980s-computer-books/275">Usborne 1980s computer books - Histories - Retro Computing</a></li>
<li><a href="https://news.ycombinator.com/item?id=32202822">Usborne computer and coding books from the 1980s | Hacker News</a></li>
<li><a href="https://hackaday.com/2017/03/20/usborne-release-more-1980s-computer-books/">Usborne Release More 1980s Computer Books | Hackaday</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者分享了从这些书籍学习编程的真挚故事，许多人将其归功于他们后来的软件工程职业。一些人指出，与现代编程文本相比，这些书籍在视觉吸引力和清晰度上更胜一筹。

**标签**: `#retro computing`, `#programming education`, `#BASIC`, `#nostalgia`, `#hacker news`

---

<a id="item-14"></a>
## [社区比较 Qwen3.6 与 Gemma4 模型](https://www.reddit.com/r/LocalLLaMA/comments/1tmbola/qwen3635ba3b_vs_gemma426ba4b/) ⭐️ 7.0/10

Reddit 用户发帖询问 Qwen3.6-35B-A3B 和 Gemma4-26B-A4B 的使用体验，社区回复显示 Gemma 运行速度更快，但 Qwen 的工具调用更可靠，且 Gemma 在非编程任务中更受欢迎。 此次对比为从业者在本地推理中选择两个流行的开源混合专家（MoE）模型提供了实用见解，突出了速度与工具调用可靠性之间的权衡。 这两个模型都是稀疏 MoE 架构：Qwen3.6-35B-A3B 总参数量为 35B，激活参数为 3B；Gemma4-26B-A4B 总参数量为 26B，激活参数为 4B。讨论基于在 Radeon 9070 XT GPU 上使用 llama.cpp 进行本地推理。

reddit · r/LocalLLaMA · MarcCDB · May 24, 13:05

**背景**: 稀疏混合专家（MoE）模型每次只激活一部分参数，从而在保持推理效率的同时实现更大的总参数量。工具调用（或函数调用）是指 LLM 调用外部工具或 API 的能力，这是构建 AI 智能体的关键能力。该比较与本地运行模型进行编程和通用文本生成任务的用户密切相关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.labellerr.com/blog/qwen3-6-35b-a3b-open-source-ai-model/">Qwen3.6-35B-A3B: The Small Model That Codes Like a Giant</a></li>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B-it">google/gemma-4-26B-A4B-it · Hugging Face</a></li>
<li><a href="https://medium.com/garantibbva-teknoloji/understanding-llm-tool-calling-traditional-vs-embedded-approaches-fc7e576d05de">Understanding LLM Tool Calling: Traditional vs. Embedded ...</a></li>

</ul>
</details>

**社区讨论**: 社区成员报告称，Qwen 在工具调用方面问题显著较少，而 Gemma 速度更快且更适合非编程任务。一位用户总结道：“用 Gemma 做你喜欢的事，用 Qwen 处理其他一切。”

**标签**: `#LLM`, `#Qwen`, `#Gemma`, `#model comparison`, `#local inference`

---

<a id="item-15"></a>
## [无审查模型的实际用途远不止角色扮演](https://www.reddit.com/r/LocalLLaMA/comments/1tlzvfs/is_there_any_reason_for_an_uncensored_model_if/) ⭐️ 7.0/10

一位 Reddit 用户质疑无审查大语言模型除角色扮演外是否还有价值，引发了社区讨论，大家列举了实际用例，如金融建议、医学翻译、代码调试、历史分析和逆向工程。 此次讨论表明，在安全对齐机制阻碍生产力的场景中，无审查模型至关重要，并凸显了在专业领域中对实用性高于安全护栏的模型需求日益增长。 用户指出，无审查模型并不能神奇地解决幻觉或准确性问题，但消除了在股票研究或逆向工程等敏感话题上因拒绝回答而产生的摩擦，这在评论中有明确提及。

reddit · r/LocalLLaMA · vick2djax · May 24, 02:49

**背景**: 无审查语言模型，也称为异端（heretic）或消融（abliterated）模型，是通过微调或修改来移除标准模型内置的拒绝行为（对齐）的版本。Heretic 等工具无需重新训练即可实现此功能。这类模型在需要无限制响应的用户中很受欢迎，如研究、创意写作或安全过滤器适得其反的技术任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://insiderllm.com/guides/best-uncensored-local-llms/">Best Uncensored Local LLMs (And Why You Might Want Them)</a></li>
<li><a href="https://github.com/FemaleGhost/heretic-AI">GitHub - FemaleGhost/ heretic - AI : Fully automatic censorship removal...</a></li>
<li><a href="https://huggingface.co/TheBloke/WizardLM-13B-Uncensored-GGUF">TheBloke/WizardLM-13B-Uncensored-GGUF · Hugging Face</a></li>

</ul>
</details>

**社区讨论**: 高赞评论强烈主张无审查模型在实际使用中不可或缺：一位用户称赞其在提供股票建议时无需免责声明；另一位列举了审查模型失败的多种场景（如医学建议、粗话翻译、代码调试、历史问题）。还有一位强调逆向工程是关键用例。总体情绪支持无审查模型作为必要工具，而不仅仅是角色扮演。

**标签**: `#large language models`, `#uncensored models`, `#AI censorship`, `#model behavior`

---

<a id="item-16"></a>
## [特斯拉在中国将 FSD 更名为“特斯拉辅助驾驶”](https://electrek.co/2026/05/23/tesla-now-calls-fsd-tesla-assisted-driving-in-china-a-more-truthful-name/) ⭐️ 7.0/10

特斯拉在中国将其全自动驾驶（FSD）系统更名为“特斯拉辅助驾驶”，以遵守中国监管机构对更准确命名的要求，反映系统的真实能力。 此举凸显了中国监管机构如何强制推行诚实的营销，与其它地区常见的公司夸大宣传形成对比，并为全球自动驾驶术语树立了先例。 此次更名仅适用于中国市场，中国监管机构已对像“全自动驾驶”这样暗示尚未实现的完全自主性的误导性术语进行了反击。

reddit · r/electricvehicles · SpriteZeroY2k · May 24, 01:59 · [社区讨论](https://www.reddit.com/r/electricvehicles/comments/1tlyt3e/tesla_now_calls_fsd_tesla_assisted_driving_in/)

**背景**: 特斯拉的“全自动驾驶”是一个高级驾驶辅助系统，需要驾驶员主动监督，并非真正的自动驾驶。该术语因过度承诺能力而在全球受到批评。中国的监管环境表现出愿意强制执行准确标签的意愿，正如在固态电池术语方面的类似要求所体现的那样。

**社区讨论**: 评论者赞扬了中国监管机构抵制公司夸大宣传的立场，其中一位指出中国政府会对虚假广告“重拳出击”。另一位认为新名称更现实且品牌明确。

**标签**: `#Tesla`, `#FSD`, `#China`, `#regulations`, `#autonomous driving`

---

<a id="item-17"></a>
## [视觉 LLM 在长文档问答基准测试中不如 OCR](https://www.reddit.com/r/artificial/comments/1tlzy43/visioncapable_llms_vs_ocr_for_longdocument/) ⭐️ 7.0/10

一项基于 MMLongBench-Doc 中 30 个长篇幅、图像密集型 PDF 的基准测试发现，视觉能力 LLM（Claude Sonnet 4.5）的准确率仅为 52.0%，每次查询成本为 0.2552 美元，而基于 OCR 的流程准确率最高达 59.6%，且成本更低。 这挑战了视觉 LLM 可替代 OCR 进行文档理解的流行说法，表明带有布局提取的适当 OCR 在准确性和可靠性上仍然更优，尤其在生产环境中。 视觉 LLM 方案因 PDF 文件大小问题存在 7%的固有故障率，且重试后仍无法恢复，而 OCR 方案的故障率为 0%。视觉模型在图表和表格密集的页面上表现尤为不佳。

reddit · r/artificial · Uiqueblhats · May 24, 02:52

**背景**: MMLongBench-Doc 是一个用于长上下文、多模态文档理解的基准测试，包含超过 1000 个专家标注的问题。OCR 从图像中提取文本，通常结合布局分析以保留文档结构。视觉能力 LLM 可直接将 PDF 作为图像处理，但在复杂布局和大文件大小上可能遇到困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mayubo2333.github.io/MMLongBench-Doc/">MMLongBench - Doc</a></li>
<li><a href="https://pvsravanth.medium.com/mastering-paddleocr-for-layout-detection-d4edb26723d0">Mastering PaddleOCR for Layout Detection | by Sravanth | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍同意这一发现，指出视觉 LLM 在结构化文档上仍无法匹配合适的布局提取。有评论强调，OCR 和编排等系统组件对生产级可靠性至关重要。

**标签**: `#LLM`, `#OCR`, `#Document QA`, `#Benchmarking`, `#RAG`

---

<a id="item-18"></a>
## [掌握 Dyalog APL：交互式书籍发布](https://mastering.dyalog.com/README.html) ⭐️ 6.0/10

一本名为《掌握 Dyalog APL》的综合交互式书籍已经发布，为 APL 数组编程语言提供了基于 Jupyter Notebook 的现代学习体验。 该资源通过提供交互式示例帮助建立对 APL 独特符号记法的肌肉记忆，降低了学习这一强大但小众语言的门槛，可能吸引更多程序员探索数组编程。 该书可免费在线获取，包含可执行代码单元格，方便直接在浏览器中实验 APL 概念。它基于原版《掌握 Dyalog APL》文本，但增加了交互功能。

hackernews · tosh · May 24, 11:42 · [社区讨论](https://news.ycombinator.com/item?id=48256475)

**背景**: APL（一种编程语言）是一种高级的面向数组的编程语言，以其使用特殊符号简洁表达复杂数组操作而闻名。Dyalog APL 是最广泛使用的现代实现，提供企业级功能和跨平台支持。数组编程是一种将操作同时应用于整个数组的范式，能够为数据密集型任务编写表达力强且高效的代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/APL_(programming_language)">APL (programming language) - Wikipedia</a></li>
<li><a href="https://www.dyalog.com/">Home - Dyalog</a></li>
<li><a href="https://aplwiki.com/wiki/Dyalog_APL">Dyalog APL APL (programming language) - Wikipedia A Dyalog workflow. Or two. — Learning APL - GitHub Pages TryAPL Welcome to Dyalog Videos Page Why Are More Engineers Discovering Dyalog APL in 2025?</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了对此交互式 Jupyter Notebook 格式的赞赏，一位用户指出它有助于建立 APL 符号的肌肉记忆。讨论还涉及 APL 的小众地位、企业许可模式以及替代学习资源，如“学习 APL”和在 Kattis 上解题。

**标签**: `#APL`, `#programming languages`, `#array programming`, `#interactive learning`

---

<a id="item-19"></a>
## [早期计算体验的怀旧回顾](https://susam.net/childhood-computing.html) ⭐️ 6.0/10

这篇文章是对童年计算经历的个人回顾，分享了早期个人计算机时代的情感记忆和学习时刻。 它与许多在早期计算机陪伴下成长的读者产生共鸣，突显了亲身体验计算对情感和教育的深远影响。 文章没有提供具体技术细节，但唤起了使用 Commodore 64 和早期 Windows 个人电脑等机器的感官和认知体验。

hackernews · blenderob · May 24, 12:07 · [社区讨论](https://news.ycombinator.com/item?id=48256597)

**背景**: 在 20 世纪 80 年代和 90 年代，像 Commodore 64 和 IBM PC 兼容机这样的家用计算机将数百万人引入了编程和数字创意世界。这些机器硬件有限，但鼓励深入探索和学习，通常在没有互联网的情况下通过试错进行。

**社区讨论**: 评论者分享了他们第一台计算机的怀旧记忆，包括一台磁带磁头配置错误的 C64 和一台 Pentium 166 MHz 机器。一位用户描述了在 RPG Maker 中理解变量时的顿悟，而另一位则对现代儿童屏幕时间政策表达了矛盾心理。

**标签**: `#nostalgia`, `#computing history`, `#programming`, `#childhood`

---

<a id="item-20"></a>
## [Ruby for Good：社会公益项目维护者聚会](https://ti.to/codeforgood/rubyforgood) ⭐️ 6.0/10

Ruby for Good 宣布了其线下活动，明确表示这是一次专注于社会公益项目的开源维护者聚会，而非黑客马拉松，并开放了早鸟注册。 该活动为维护者提供了一个专注于长期社会公益项目协作的专属空间，促进了社区发展并产生超出典型黑客马拉松的持续影响。 根据创始人 Sean Marcia 的说法，该活动不是黑客马拉松，而是开源维护者的友好聚会，他们致力于现有项目，其中一些已运行超过 10 年。

hackernews · mooreds · May 24, 15:49 · [社区讨论](https://news.ycombinator.com/item?id=48258254)

**背景**: Ruby for Good 是一个社区驱动的倡议，汇集 Ruby 开发者共同开发有益社会的开源项目。与通常启动新项目的黑客马拉松不同，该活动专注于维护和改进为非营利组织和社区服务的现有应用程序。

**社区讨论**: 社区表达了感谢和支持，创始人 Sean Marcia 澄清了非黑客马拉松的性质并开放了早鸟注册。一些用户询问赞助商情况，反映了对企业支持社会公益的兴趣。

**标签**: `#Ruby`, `#open source`, `#social good`, `#conference`, `#community`

---

<a id="item-21"></a>
## [Datasette 1.0a30 新增可定制的“跳转到”菜单和插件钩子](https://simonwillison.net/2026/May/24/datasette/#atom-everything) ⭐️ 6.0/10

Datasette 1.0a30 引入了一个可定制的“跳转到”菜单，用户可通过按 “/” 键激活，并新增了 `jump_items_sql()` 插件钩子，用于向菜单添加自定义项。 此更新增强了 Datasette 内的导航，使用户能更快地找到数据库、表格等。该插件钩子使开发者能够扩展菜单以添加自定义搜索，提升了工具的灵活性和生态系统。 跳转到菜单支持用户输入时实时过滤，`jump_items_sql()` 钩子允许插件通过 SQL 查询贡献菜单项。该版本是 alpha 版本（1.0a30），表明仍在开发中。

rss · Simon Willison · May 24, 23:52

**背景**: Datasette 是一款用于探索和发布数据的开源工具，主要使用 SQLite 数据库。它支持基于 pluggy 框架的插件系统，通过钩子允许插件自定义行为。新的跳转到菜单在现有操作菜单模式基础上构建，为数据库、表格和自定义插件条目提供统一的搜索体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.datasette.io/en/stable/plugin_hooks.html">Plugin hooks - Datasette documentation</a></li>
<li><a href="https://github.com/simonw/datasette">GitHub - simonw/datasette: An open source multi-tool for ... datasette-plugins - Skill | Smithery Datasette Adds Semantic Column Types And Plugin Hook Datasette 1.0a8: JavaScript plugins, new plugin hooks and ... Datasette Plugins</a></li>

</ul>
</details>

**标签**: `#datasette`, `#release`, `#plugin`, `#open-source`, `#data exploration`

---

<a id="item-22"></a>
## [AI 复活 1980 年代 Usborne 游戏为交互式网页应用](https://simonwillison.net/2026/May/24/usborne-mad-house/#atom-everything) ⭐️ 6.0/10

Simon Willison 使用 Anthropic 的 Claude 将 1983 年游戏“Mad House”从 Usborne 的《Creepy Computer Games》书籍 PDF 转换为一个可完全运行的 JavaScript 和 HTML 交互版本。 这展示了大型语言模型如何将复古计算怀旧与现代网页开发连接起来，让经典游戏无需用户手动输入代码即可访问。 Willison 向 Claude 提供 PDF 并发送提示，要求生成一个无框架的 JavaScript 项目，具备移动友好设计和复古美学，模型生成了游戏中的 ASCII 风格走廊、门控制和计分逻辑。

rss · Simon Willison · May 24, 17:14

**背景**: Usborne 出版社免费发布了其 1980 年代计算机书籍的 PDF，包括 1983 年的《Creepy Computer Games》，其中包含可输入到 Commodore 64 等平台的游戏。Simon Willison 是一位知名网页开发者，经常尝试 Claude 等 AI 工具。该项目展示了利用 AI 重新诠释历史软件的可能性。

**标签**: `#retro computing`, `#AI`, `#JavaScript`, `#game development`, `#Claude`

---

<a id="item-23"></a>
## [质疑 NVIDIA 在 2026 年本地 LLM 中的主导地位](https://i.redd.it/pzq8x188q43h1.jpeg) ⭐️ 6.0/10

一个获得 168 个点赞和 89%好评率的 Reddit 帖子质疑 NVIDIA 在 2026 年是否仍是运行本地 LLM 的默认最佳 GPU 选择，引发了对定价和替代品的讨论。 这一讨论很重要，因为 NVIDIA 的主导地位影响着消费者硬件决策和 AI 硬件市场的竞争，尤其是在本地 LLM 推理日益普及的背景下。 该帖子指出，建议零售价常常过时，一些用户正在混用 NVIDIA 和 AMD GPU，表明 AMD 等替代品对于本地 LLM 推理正变得可行。

reddit · r/LocalLLaMA · pmv143 · May 24, 18:34 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1tmkaua/is_nvidia_still_the_default_best_choice_for_local/)

**背景**: 本地 LLM 是指在个人硬件上运行的大型语言模型，而非云服务器。GPU 选择至关重要，因为模型推理高度依赖并行处理和 VRAM。NVIDIA 因其成熟的 CUDA 生态以及 Ollama、LM Studio 等工具的广泛软件支持，历史上一直是默认选择。然而，GPU 价格上涨以及 AMD 和 Intel 等竞争硬件的出现，正在挑战这一默认地位。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.starmorph.com/blog/local-llm-inference-tools-guide">Local LLM Inference in 2026: The Complete Guide to Tools ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/CUDA">CUDA - Wikipedia</a></li>
<li><a href="https://www.aitooldiscovery.com/how-to/best-local-llm-models">Best Local LLM Models 2026: Benchmarks & Use Cases</a></li>

</ul>
</details>

**社区讨论**: 评论者对 NVIDIA 的定价表示怀疑，有人指出由于市场价格虚高，建议零售价没有意义。另一位用户分享了 NVIDIA+AMD 混合配置的经验，表明混用不同厂商的硬件是一种实用方法。

**标签**: `#NVIDIA`, `#local LLMs`, `#GPU`, `#AI hardware`

---

<a id="item-24"></a>
## [Qwen3.6-35B-A3B 无审查模型在迷你 PC 上运行 20 万上下文](https://www.reddit.com/r/LocalLLaMA/comments/1tm3toi/qwen3635ba3buncensoredgenesisapexmtp/) ⭐️ 6.0/10

一个新的无审查量化版本 Qwen3.6-35B-A3B（名为 Genesis-V2-APEX-MTP）已发布，支持多令牌预测（MTP），并在 Beelink GTR9 Pro 迷你 PC 上使用 Q8_K_P MTP 量化成功测试了 20 万令牌上下文。 此次发布表明，35B 参数的大语言模型可以在消费级硬件上高效运行，挑战了此类模型需要昂贵数据中心 GPU 的假设。它还通过 MTP 提供了无审查变体并增强了推理速度，有利于本地 AI 应用和隐私保护。 该模型使用 GGUF 格式，支持 APEX 量化和 MTP。同时还提供 Safetensors 版本，方便 Apple MLX 转换。推荐使用 APEX 和 MTP-APEX 量化，并提供了自定义系统提示和聊天模板。

reddit · r/LocalLLaMA · EvilEnginer · May 24, 06:08

**背景**: 大语言模型（LLM）通常太大而无法在个人电脑上运行；量化通过降低数值精度来减小模型大小，多令牌预测（MTP）通过一次预测多个令牌来加速推理。Qwen3.6-35B-A3B 模型是一种稀疏混合专家（MoE）架构，总参数 35B 但仅 3B 激活，从而实现高效的本地推理。Safetensors 是一种安全、快速的文件格式用于存储模型权重，而 GGUF 则针对像 llama.cpp 这样的 CPU 推理工具进行了优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hardware-corner.net/multi-token-prediction-llm-speed/">How Multi-Token Prediction Makes Local LLMs Faster – Without ...</a></li>
<li><a href="https://huggingface.co/docs/safetensors/index">Safetensors · Hugging Face Safetensors – PyTorch File Format | huggingface/safetensors | DeepWiki Safetensors File Format • safetensors - GitHub Pages Package 'safetensors' reference manual SAFETENSORS File - What is it and how do I open it?</a></li>
<li><a href="https://huggingface.co/docs/hub/gguf">GGUF · Hugging Face</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一位用户庆祝在迷你 PC 上运行 35B 模型和 20 万上下文，与大型科技公司需要 8 张 H100 形成对比。另一位用户对 APEX 量化在编码代理中的表现表示怀疑，报告称即使使用质量预设也会出现错误方向和循环问题。

**标签**: `#LLM`, `#Qwen`, `#Quantization`, `#Local Inference`, `#Uncensored`

---

<a id="item-25"></a>
## [探索超越 SQL 和 NoSQL 的专用数据库引擎](https://blog.gaborkoos.com/posts/2025-09-19-The-Database-Zoo-Exotic-Data-Storage-Engines/) ⭐️ 6.0/10

一篇题为《数据库动物园：异域数据存储引擎》的博文指出，通用数据库无法满足所有现代工作负载需求，从而催生了针对时间序列、向量和概率数据的专用引擎。 这很重要，因为它凸显了数据库领域的转变——专用引擎在物联网监控、AI 驱动搜索和不确定性管理等特定应用场景中，可提供显著的性能和效率提升。 该博文是一个系列的第一篇，后续将深入介绍时间序列数据库（TSDB）、向量数据库和概率数据库，强调它们相比通用系统的独特优化。

reddit · r/programming · OtherwisePush6424 · May 24, 02:39 · [社区讨论](https://www.reddit.com/r/programming/comments/1tlzo76/the_database_zoo_exotic_data_storage_engines_why/)

**背景**: 传统 SQL 数据库擅长处理结构化数据和复杂查询，NoSQL 数据库则为半结构化数据提供灵活性。然而，现代应用如实时分析（时间序列数据）、AI 驱动的相似性搜索（向量数据）以及处理不确定数据（概率数据）需要专用存储引擎，它们牺牲通用性以换取特定性能。例如，时间序列数据库对带时间戳的数据使用专用压缩算法；向量数据库支持高效的高维相似性搜索，用于检索增强生成（RAG）；概率数据库则管理带有概率值的数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Time_series_database">Time series database - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Vector_database">Vector database - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Probabilistic_database">Probabilistic database - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区反应褒贬不一：有些用户开玩笑说，任何不使用 SQL 的数据库都是 NoSQL；另一些人批评文章缺乏严谨性，对于“动物园”这个标题来说不够全面；还有少数人对营销术语感到厌倦。

**标签**: `#databases`, `#NoSQL`, `#SQL`, `#time-series`, `#vector databases`

---