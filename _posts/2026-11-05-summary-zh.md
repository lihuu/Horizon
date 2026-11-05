---
layout: default
title: "Horizon Summary: 2026-11-05 (ZH)"
date: 2026-11-05
lang: zh
---

> 从 79 条内容中筛选出 31 条重要资讯。

---

1. [IEEE Spectrum：AI 漏洞挖掘迫使行业偿还四十年安全技术债](#item-1) ⭐️ 8.0/10
2. [月之暗面开源 Kimi K3.1 Pro 模型权重](#item-2) ⭐️ 8.0/10
3. [Go 发布 encoding/json/v2，重构 JSON 处理 API](#item-3) ⭐️ 8.0/10
4. [Anthropic 在大型语言模型可验证推理方面取得进展](#item-4) ⭐️ 8.0/10
5. [腾讯发布 Hy4：770B 开放权重模型，主打科学与游戏开发](#item-5) ⭐️ 8.0/10
6. [NKI 巨型内核降低 GLM-5.3-Flash 在 AWS Trainium2 上的解码延迟](#item-6) ⭐️ 8.0/10
7. [Ricursive Intelligence 发布稠密开源模型 Ripple-65B-Preview](#item-7) ⭐️ 8.0/10
8. [C++26 在 ISO 国家成员体投票中未获通过，史无前例](#item-8) ⭐️ 8.0/10
9. [Postgres 19 内置 REPACK，实现无停机的表膨胀清理](#item-9) ⭐️ 8.0/10
10. [博客称白宫 IP 段出现住宅代理出口流量](#item-10) ⭐️ 7.0/10
11. [Nvidia RTX Spark 在 Linux 下 GPU 降频，本地 AI 推理速度大幅缩水](#item-11) ⭐️ 7.0/10
12. [AMD 第四季度指引达 170 亿美元，有望史上首次超越英特尔](#item-12) ⭐️ 7.0/10
13. [Deep Principle 发布 Hydrogen-1.0，开源权重科学模型在 FSR 上超越 GPT-6 Astra](#item-13) ⭐️ 7.0/10
14. [B200 实测：循环 Transformer 只省存储，不省 HBM 访存](#item-14) ⭐️ 7.0/10
15. [开发者将 Gemma 4 26B-A4B 剪枝为稠密 3.81B 模型](#item-15) ⭐️ 7.0/10
16. [Unsloth 发布 Qwen3.8-Flash-Next 的 Dynamic v3.1 GGUF 量化](#item-16) ⭐️ 7.0/10
17. [Axion 1.0：完全开源的 35B 智能体模型，三阶段训练即可达成](#item-17) ⭐️ 7.0/10
18. [Zig 重写 libc 被指导致 SQLite 慢 12000 倍](#item-18) ⭐️ 7.0/10
19. [交互式讲解带你深入 Git 内部的对象模型与引用机制](#item-19) ⭐️ 7.0/10
20. [苹果 10-K 文件警示 AI 智能体可能“隐瞒”和“操纵”](#item-20) ⭐️ 7.0/10
21. [Cognition 发布 SWE-2 Flash：更快更便宜的编程智能体模型](#item-21) ⭐️ 7.0/10
22. [旧金山游击自行车道最终成为永久基础设施](#item-22) ⭐️ 6.0/10
23. [OpenAI 宣布收购 Pierre Computer Company，后者为 Codex 提供 diff 库](#item-23) ⭐️ 6.0/10
24. [验证不等于知识：科学需要的是理解，而不只是答案](#item-24) ⭐️ 6.0/10
25. [小米称人形机器人已在工厂自主完成 8 小时完整班次](#item-25) ⭐️ 6.0/10
26. [datasette-apps 0.3a0 改进与 Datasette Agent 的集成，优化自定义 HTML 应用](#item-26) ⭐️ 6.0/10
27. [研究者呼吁顶级 AI 会议加强直接拒稿以拦截 AI 生成论文](#item-27) ⭐️ 6.0/10
28. [Reddit 热议：CVPR 每人 25 篇的投稿上限是否已不适配 AI 时代？](#item-28) ⭐️ 6.0/10
29. [DeepSeek 独占 OpenRouter 270 亿亿日 tokens 的 53%，开源权重实验室合计突破 75%](#item-29) ⭐️ 6.0/10
30. [有开发者称 LFM3-Omni-2B 借助 WebGPU 在 iPhone 上离线运行，速度约 80 tok/s](#item-30) ⭐️ 6.0/10
31. [遗失的 malloc\(\)：回顾早期 Unix 分配器接口](#item-31) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [IEEE Spectrum：AI 漏洞挖掘迫使行业偿还四十年安全技术债](https://spectrum.ieee.org/ai-in-cybersecurity-php2shell-vulnerability) ⭐️ 8.0/10

IEEE Spectrum 的一篇文章认为，以 PHP 中高危害的 PHP2Shell 漏洞为代表，AI 驱动的漏洞发现正在暴露并迫使业界修复大约四十年来累积的安全技术债。该文在 Hacker News 上引发大规模讨论（约 1015 分、612 条评论），争论的焦点在于这究竟算是真正“还债”，还是仅仅开启了一条无休止的修复流水线。 AI 正在把漏洞发现“工业化”，被披露漏洞的数量已超过维护者和安全团队的修复能力，促使企业从传统的漏洞管理转向更广泛的暴露面管理。由于大量网站依赖 PHP 这类长期演进的代码库，修复负担落在庞大而分散的项目与厂商生态上，而非少数几家大公司。 PHP2Shell 指两个远程代码执行漏洞 CVE-2026-109618 和 CVE-2026-109619，根源是影响 PHP 5.4 至 8.5 版本的内存安全缺陷。评论者指出，其中不少问题并非靠一处“外科手术式”补丁就能修好的差一错误（off-by-one），而需要结构性重构，这也是为什么“还债”与“无休止的修复跑步机”在短期内看起来一模一样。

hackernews · pseudolus · 11月4日 11:52 · [社区讨论](https://news.ycombinator.com/item?id=50364336)

**背景**: 技术债是指软件中因走捷径、推迟工作而累积的成本；安全技术债则特指未修补的漏洞、过时的安全实践和被拖延的安全加固，它们会随时间推移放大风险。PHP 是一种驱动了大量网站的服务器端脚本语言，其中许多遗留代码可追溯到几十年前。如今 AI 模型以及机器辅助的静态分析和模糊测试能以人类无法企及的规模扫描这类代码，把沉睡多年的缺陷翻出来——这正是文章所说的“被迫偿还四十年债务”的动态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PHP2Shell">PHP2Shell - Wikipedia</a></li>
<li><a href="https://www.akamai.com/blog/security-research/understanding-php2shell-everything-you-need-to-know">Understanding PHP2Shell: Everything You Need to Know</a></li>
<li><a href="https://www.techtarget.com/news/php2shell-explained-timeline-of-the-global-vulnerability-crisis/872935/">PHP2Shell explained: Timeline of the global vulnerability ...</a></li>

</ul>
</details>

**社区讨论**: 讨论相当有实质内容，并非一片叫好：swatcoder 质疑文章的框架，追问这到底是“还债”，还是一条强制的、不产生新功能的无限修复流水线；Balgair 则援引《哥德尔、艾舍尔、巴赫》中唱片机的寓言，论证完全安全的系统即便在理论上也不可能存在。也有人更为乐观——glennfiedler 认为经历几个月的阵痛后软件会比以往任何时候都更安全；xbmcuser 表示 AI 审计终于能让开源“他人会审计代码”这一常被假设却很少兑现的承诺成真；Arbortheus 则希望国家背景和商业间谍（如 Pegasus）手中的零日漏洞能在这个过程中被顺带发现。

**标签**: `#AI security`, `#vulnerability discovery`, `#technical debt`, `#cybersecurity`, `#static analysis`

---

<a id="item-2"></a>
## [月之暗面开源 Kimi K3.1 Pro 模型权重](https://huggingface.co/moonshotai/Kimi-K3.1-Pro) ⭐️ 8.0/10

月之暗面（Moonshot AI）在 Hugging Face 上发布了 Kimi K3.1 Pro 的开放权重，称其为一个原生多模态的智能体模型，也是该公司迄今最强的 3T 级别模型。它是 K3.1 系列的首个版本，基于 Kimi K3 通过覆盖数百个下游领域的大规模联合强化学习后训练而来。 又一款前沿级模型开放权重，会持续给闭源 API 厂商施加压力；正如评论者所观察到的，OpenRouter 上随即出现了多家第三方推理服务商，在相同价格下提供更高吞吐量。对于拥有相应硬件的企业而言，这也意味着可以自行部署而非租用这一顶级多模态模型。 该模型延续了 K3 系列的 100 万 token 上下文窗口和视觉输入能力，社区成员估计自行部署实际需要类似 8 张 B300 的节点规格。上一代 Kimi K3 是一个 2.8 万亿参数的 MoE 模型，以修改版 MIT 许可证发布。

hackernews · abrarthought · 11月4日 15:30 · [社区讨论](https://news.ycombinator.com/item?id=50366999)

**背景**: 月之暗面是 Kimi 聊天机器人与模型系列背后的中国实验室，以发布开放权重而闻名——也就是任何人都可以在自己的硬件上运行的模型文件，这与只能通过 API 访问的闭源模型不同。Kimi 的大模型采用混合专家（MoE）架构，每个 token 只激活一部分参数，因此推理成本比参数量所暗示的要低，但万亿级参数模型仍然需要多 GPU 服务器。&\#x27;Pro&\#x27; 后缀与 3.1 的版本号说明这是相对 K3 一代的渐进式升级，而非全新架构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/moonshotai/Kimi-K3.1-Pro">moonshotai/ Kimi -K 3 . 1 - Pro · Hugging Face</a></li>
<li><a href="https://thenewstack.io/kimi-k3-open-weights/">Moonshot opens Kimi K3 weights — but few can run it</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kimi_%28AI%29">Kimi (AI) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区看法出现分歧：质疑者认为该模型有“刷榜（benchmaxxed）”之嫌，因为它相较 DeepSeekV4.1-Flash 提升有限，在其他实验室的内部基准上得分也不如 Opus5.5；但也有评论者给出了第一手测试结果，认为这是一个非常强的发布，只是略逊于最前沿。另一些人关注现实问题——自建部署需要 8 张 B300 级别的节点，普通个人难以承担；而 Together、Modal 等第三方托管服务吞吐量已达月之暗面自家端点的数倍，说明成本仍有下降空间。

**标签**: `#open-weight LLMs`, `#Moonshot AI`, `#model release`, `#LLM benchmarks`, `#inference infrastructure`

---

<a id="item-3"></a>
## [Go 发布 encoding/json/v2，重构 JSON 处理 API](https://go.dev/blog/jsonv2) ⭐️ 8.0/10

Go 团队推出了 encoding/json/v2 以及底层的 encoding/json/jsontext 包，这是用于 JSON 序列化与解析的新 API，旨在提升易用性并修复原 encoding/json 包中的行为问题。 由于 encoding/json 是 Go 中使用最广泛的包之一，这次重构对整个生态中的 API 契约、迁移策略以及 Web 服务、CLI 和数据管道的性能都有广泛影响。 v1 版 encoding/json 的行为保持不变，而 DefaultOptionsV1 等兼容选项让团队可以逐步迁移；早期报告指出部分基准测试中反序列化更快但序列化更慢，并且像 MarshalIndent 这样的辅助函数没有以相同形式保留。

hackernews · olexsmir · 11月4日 17:52 · [社区讨论](https://news.ycombinator.com/item?id=50369106)

**背景**: JSON 是一种无处不在的数据交换文本格式，而 Go 的 encoding/json 包长期以来都是在 Go 程序中序列化和反序列化 JSON 的标准方式。十多年来，原始 API 积累了不少设计妥协和行为怪癖，促使社区提出 v2 设计的正式提案，并引入更底层的 jsontext 层来处理词法单元。新 API 通过兼容选项引入，因此现有 v1 代码的行为不会一夜之间发生变化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://go.dev/blog/jsonv2">A new Go API for JSON - The Go Programming Language</a></li>
<li><a href="https://github.com/golang/go/issues/71497">encoding / json / v 2 : new API for encoding / json · Issue #71497...</a></li>
<li><a href="https://importstatic.com/go/go-json-v2-migration">Go JSON v 2 Migration : What Breaks in Go 1.27 | ImportStatic</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论总体偏正面，评论者欢迎更清晰的 JSON API，并认同序列化逻辑确实需要修复。一些用户指出了迁移痛点，尤其是 MarshalIndent 的缺失及其替代写法的复杂性，另一些人则讨论了解析器性能以及基于 schema 的 SIMD 解析。还有评论者表示自己现在依赖 AI 编写 Go 代码，但仍然看重 Go 的性能和安全性。

**标签**: `#Go`, `#JSON`, `#standard library`, `#API design`, `#software engineering`

---

<a id="item-4"></a>
## [Anthropic 在大型语言模型可验证推理方面取得进展](https://www.anthropic.com/research/provable-inference) ⭐️ 8.0/10

Anthropic 发布了一项研究，利用 zkSNARK（一种简洁的密码学证明系统）让模型提供方对某一组特定的权重做出承诺，并针对每一次响应证明它确实由这组权重生成。原型中的承诺体积约为 6.5 MB，可覆盖约 1600 万次请求，之后提供方需要重新承诺；而验证单次请求的证明在 24 线程下约需 17 秒，单线程下约需 21 秒。 对于闭源权重的 API 提供方来说，客户目前无法核实究竟是哪个模型在为自己作答——仅凭输出质量无法区分宣传中的模型与更廉价或经过蒸馏的替代品。一个可用的推理证明原语将为审计方、监管机构和企业采购方提供以密码学为基础的信任依据，这也是为何“开销与信任之间的权衡”正引起整个生态的关注。 该方案代价不菲：报道与社区讨论称其证明开销约为普通推理算力的 90 至 100 倍，因此目前难以用于高并发生产服务。它还依赖于确定性推理，且只能证明输出满足所声明的计算关系；针对零知识推理证明的分析（如 Hollow-LLM 的研究）提醒，此类证明并不能自动排除退化模型或“平凡权重”变体的可能。

hackernews · ltononro · 11月4日 17:17 · [社区讨论](https://news.ycombinator.com/item?id=50368626)

**背景**: zkSNARK 是一种证明“某个计算被正确执行”的密码学证明，它生成的简短证明在验证时远比重新执行整个计算便宜——一些区块链扩容方案使用的正是这类技术。将其用于大模型推理，意味着要把前向传播中的每一次矩阵乘法都表达进证明系统，这也解释了为何其开销要以原始算力的倍数来衡量。这个问题只对闭源模型存在：如果权重开放，客户端只需确定性地重跑推理并比对输出即可，成本远低于任何密码学方案。该方向此前的相关工作包括 zkLLM 以及 VerInf 项目，后者在 Anthropic 这篇研究之前就探索过类似设定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/research/provable-inference">Progress on provable inference for large language models</a></li>
<li><a href="https://www.europesays.com/ai/226951/">Progress on provable inference for large language models ...</a></li>
<li><a href="https://github.com/JamesPetrie/zkllm-entropy">GitHub - JamesPetrie/zkllm-entropy · GitHub</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论技术含量很高，但也颇具争议：一位前 MARS 研究员称这项工作建立在他的 VerInf 项目之上——连选用 400B 级别的 Maverick 模型都源自他的工作——却几乎没有给出相应署名。另一些人则认为，闭源模型场景完全可以用更低成本解决，办法是让四家独立推理服务商对同一非批处理提示词进行概率性交叉验证；也有人指出，开放权重的模型只需确定性重算就能让整个问题变得平凡；此外一家名为 Attestable 的初创公司表示，其方案正是该研究中的对比对象之一。

**标签**: `#LLM verification`, `#provable inference`, `#zero-knowledge proofs`, `#AI trust and safety`, `#Anthropic research`

---

<a id="item-5"></a>
## [腾讯发布 Hy4：770B 开放权重模型，主打科学与游戏开发](https://hy.tencent.ai/research/hy4) ⭐️ 8.0/10

腾讯混元（Hy）团队发布了新一代混合专家（MoE）旗舰模型 Hy4，总参数量 770B、每 token 激活 49B，并以开放权重形式公开（预览版以 tencent/Hy4-preview 之名上线 Hugging Face）。除主模型外，腾讯还开源了两个与 Hy4、Hyra 2.0 联合开发的科学基础模型——用于单细胞表征的 HyCell 和用于物理场建模的 HyPDE——并针对 Unreal Engine、Unity 和 Godot 三大游戏引擎对 Hy4 做了大量适配。 一家中国大型实验室放出 770B 级别的开放权重模型，抬高了任何人都能下载并自行部署的能力上限，也进一步加剧了全球 AI 生态中开放与闭源阵营的分化。而将 HyCell、HyPDE 这类领域专用的科学模型一并开源，在头部实验室中并不常见，它降低了无法访问闭源 API、也无力自行训练此类模型的学术与生物医药研究者的门槛。 Hy4 采用稀疏混合专家架构：虽然每 token 仅激活 49B 参数，但完整的 770B 权重文件对本地部署的内存显存与推理成本构成很高门槛，因此多数用户大概率会通过托管 API 来使用它。腾讯自己也承认，Hy4 与顶级闭源模型之间仍存在明显差距，尤其是在研究级数学、长程编码、模型自我改进和高级视觉问答等内部基准上，并表示将持续扩大预训练与后训练规模以缩小差距。

hackernews · Philpax · 11月4日 14:11 · [社区讨论](https://news.ycombinator.com/item?id=50365780)

**背景**: 腾讯的模型系列此前名为“混元”（Hunyuan），现以 Tencent Hy 作为品牌；与近年许多前沿系统一样，它采用混合专家（MoE）设计，每个 token 只激活网络中一小部分参数，以显存换更低的推理成本。“开放权重”指训练好的参数文件可公开下载，团队能自行运行、微调并自托管模型——这与“开源”并不等同，因为训练数据和完整训练代码通常并不公开。HyCell 与 HyPDE 属于“专用科学模型”这一类，面向的是单细胞基因表达数据表征、物理场方程求解等狭窄的技术任务，而非通用对话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/tencent/Hy4-preview">tencent / Hy 4 -preview · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/Tencent_Hy">Tencent Hy - Wikipedia</a></li>
<li><a href="https://www.eesel.ai/blog/tencent-hy4-review">Tencent Hy 4 review: is the 770B open-weight model worth it? | eesel AI</a></li>

</ul>
</details>

**社区讨论**: 评论整体偏正面，但关注点各不相同：Simon Willison 特别提到游戏开发这一专精方向，指出腾讯与互动娱乐事业群（IEG）合作，围绕功能实现、玩法逻辑、状态追踪和资产管线来整理训练数据与评测。areoform 称赞开源科学模型的做法，认为这与美国公司限制研究用途形成令人耳目一新的对比；frangonf 则欣赏腾讯坦承与闭源模型仍有差距，并认为作为日常工具，开放模型已经够用。chriddyp 表示在 Plotly 的数据分析基准上，Hy4 落在两个 GPT-6.1 变体之间的成本/准确率前沿上，但“非常非常慢”，有时每个问题要发出 26 到 64 次查询。

**标签**: `#open-weight models`, `#LLM release`, `#AI research`, `#game development`, `#open science`

---

<a id="item-6"></a>
## [NKI 巨型内核降低 GLM-5.3-Flash 在 AWS Trainium2 上的解码延迟](https://www.reddit.com/r/MachineLearning/comments/1xo0yuq/p_nki_layer_megakernels_for_glm53flash_on_aws/) ⭐️ 8.0/10

RunAnywhere 开源了 trnrt 推理引擎，可在单台 AWS trn2.48xlarge 上服务 GLM-5.3-Flash（320B 参数 MoE、100 万 token 上下文），并将每个层的一半重写为单个融合的 NKI 巨型内核（稀疏注意力层则整层融合）。在相同布局下，batch-8 解码步从 10 月 17 日构建的 32.2 ms 降至 11 月 1 日构建的 24.2 ms，其中融合稀疏注意力层和 KDA/MoE 内核各每步节省约 3.2 ms。 结果表明，Trainium2 上大部分解码延迟来自内核边界开销、XLA 胶水代码、转置和跨芯片集合通信，而非模型数学计算，这使内核级协同设计成为非 NVIDIA 加速器的一阶杠杆。它还为一个 320B MoE、100 万上下文的模型在 AWS 芯片上提供了少见的可复用推理工件——当前最新 vLLM Neuron 插件未注册 GLM 模型，NxD Inference 也处于维护模式。 这些内核将每个层一半的工作集保留在物理 NeuronCore 的 28 MiB SBUF 中，并将 340–400 GB/s 的权重流拆分到两个核心以达到 672–708 GB/s；与此同时，batch-8 步仍花费 6.1 ms 达到内存下限、10.0 ms 引擎忙碌、4.6 ms 内核内等待、2.8 ms 暴露的集合通信和 0.7 ms 空闲。注意事项包括稀疏注意力预填充中仍有一项近似，涉及 1.2% 的选择，使下一 token 对数概率平均偏移 0.012–0.021 nats，并在 448 个位置中的 3 个改变了最高 token；此外未运行任务级评测，也没有 GPU 对比。

reddit · r/MachineLearning · /u/WildCard727 · 11月4日 21:47

**背景**: AWS Trainium2 是亚马逊的自研 AI 加速器；其 NeuronCore-v3 计算引擎和片上 SBUF 可通过 NKI 编程，NKI 是一种低层接口，可直接访问 NeuronCore 指令集来编写自定义内核。GLM-5.3-Flash 是 Z.ai 的 320B 参数 MoE 模型，激活参数 18B，支持 100 万 token 上下文，面向低成本推理设计。在 LLM 解码中，每生成一个 token 都要经过所有层的一次前向计算，因此每个内核的微小开销会在数百个内核和芯片间累积；巨型内核将整层或半层融合进一个内核以消除这些边界。XLA 是通常负责把算子拼成计算图并插入集合通信的编译器，这也是内核边界、胶水代码和集合通信成为性能分析目标的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://awsdocs-neuron.readthedocs-hosted.com/en/latest/general/nki/index.html">Neuron Kernel Interface (NKI) — AWS Neuron Documentation</a></li>
<li><a href="https://awsdocs-neuron.readthedocs-hosted.com/en/latest/nki/about/trainium2_arch.html">Trainium 2 Architecture Guide for NKI — AWS Neuron Documentation</a></li>
<li><a href="https://huggingface.co/zai-org/GLM-5.3-Flash">zai-org/ GLM - 5 . 3 - Flash · Hugging Face</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#AWS Trainium`, `#kernel fusion`, `#MoE models`, `#performance profiling`

---

<a id="item-7"></a>
## [Ricursive Intelligence 发布稠密开源模型 Ripple-65B-Preview](https://www.reddit.com/r/LocalLLaMA/comments/1xo2arv/ricursive_intelligence_ripple65bpreview_new_dense/) ⭐️ 8.0/10

Ricursive Intelligence 发布了 Ripple-65B 的预览版，这是一个 650 亿参数的稠密开源权重模型，采用了颇为罕见的“瘦而深”结构——80 层、隐藏维度 5120，并使用 4:1 的滑动窗口注意力与全局注意力混合比例。官方给出的基准成绩显示，它可以与体量大得多的前沿开源模型（如 816B 的 Muse Spark Open 和 501B 的 Reflection Beam）互有胜负；同时 AtomicChat 已提供社区 GGUF 量化版本（Q8\_0 为 68.8 GB，Q4\_K\_M 为 38.8 GB）以及 llama.cpp 分支补丁。 本地 LLM 社区长期以来一直在呼吁新的 70B 级别稠密模型，而一个能与 500B–800B 专家混合（MoE）前沿模型抗衡的 65B 稠密模型，将是开源模型生态中颇为重要的补充。由于该预览版只是针对智能体编程做了较轻量的后训练，正式版可能会更强，因此它既是一个可用的工具，也说明小体量稠密架构依然有很大的上限空间。 该预览版采用较为常规的后训练流程（midtraining、长上下文训练、SFT、长上下文 SFT 以及混合领域强化学习），但后训练强度较轻且集中于智能体编程；此外还提供了一个完全未经 midtraining 和合成问答数据的预训练检查点。值得注意的设计包括 FFN 激活裁剪、门控注意力、全局 NoPE 注意力和 value residual，并配套 DFlash2 草稿模型用于推测解码；公布的分数包括 Terminal-Bench 2.1 80.5、SWE-bench Pro 61.4、DeepSWE 1.1 44.3、IFBench 79.2 和 GPQA Diamond 85.2，但这些均为自报成绩，而且“Preview”定位与 65B 稠密模型在消费级硬件上推理缓慢都是需要注意的局限。

reddit · r/LocalLLaMA · /u/returnity · 11月4日 22:42

**背景**: 稠密模型对每个 token 都会激活全部参数，而专家混合（MoE）模型只激活其中一部分，因此 65B 稠密模型每 token 的计算开销远高于体量相当甚至更大的 MoE 模型。混合注意力把滑动窗口注意力（开销低、只关注局部上下文）与完整的全局注意力层按固定比例搭配，以降低长上下文成本；NoPE 指这些全局注意力层完全不使用显式位置编码，而依赖基于内容的注意力。推测解码则用小型的草稿模型（此处是块扩散草稿模型 DFlash2）先提出 token，再由大模型验证，从而加速推理；GGUF 是 llama.cpp 用于本地运行所使用的量化格式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/z-lab/Qwen3.8-27B-DFlash2">z-lab/Qwen3.8-27B-DFlash2 · Hugging Face</a></li>
<li><a href="https://www.mindstudio.ai/blog/qwen3-8-27b-dflash2-speculative-decoding">What Is DFlash 2? Speculative Decoding Explained for Qwen3.8 ...</a></li>
<li><a href="https://sebastianraschka.com/llm-architecture-gallery/nope/">No Positional Embeddings (NoPE) | Sebastian Raschka, PhD</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者欢迎又一个有竞争力的开源权重发布，但在几个方面持怀疑态度：有人指出“SOTA”一词因基准类别被不断细分而严重贬值；也有人认为 65B 稠密模型在消费级硬件上推理会慢得难以接受，因此很难像 Qwen 的 27B 级别或 MoE 模型那样赢得爱好者青睐。还有人批评发布方未提及同类开源模型、质疑其相对 Qwen 的“刷榜”程度，并指出对部分用户而言，属于美国司法管辖范围的开源权重本身就是一项有意义的差异点。

**标签**: `#local-llm`, `#open-weights`, `#dense-models`, `#model-architecture`, `#benchmarks`

---

<a id="item-8"></a>
## [C++26 在 ISO 国家成员体投票中未获通过，史无前例](https://www.reddit.com/r/programming/comments/1xnucc3/c26_disapproved_by_the_iso_national_bodies/) ⭐️ 8.0/10

据报道，C++26 的国际标准草案（DIS）在 ISO 国家成员体投票中未获通过，结果为 12 票赞成、9 票反对；这是自 1998 年该流程平稳运行以来，C++ 标准草案首次在这一环节遭到否决。此前这一投票普遍被认为只是走流程的形式性环节，因此否决结果令 C++ 社区颇感意外。 这次否决使 C++26 无法按预期时间表发布为正式的 ISO 国际标准，影响到所有跟进标准的开发者、编译器厂商和标准库实现者。同时，一个已在工作组层面达成共识的特性却在国家成员体环节被否决，也让人们对 WG21 内部的共识机制产生疑问。 有报道指出，反对意见主要集中在长期争议的“契约”（contracts，即 P2900）提案上，各国成员体在投票时也一并提交了评论意见。DIS 投票失败并不等于项目直接终止：SC22 可以选择重新分发修订后的委员会草案、将其改为技术规范（TS），或取消该工作项，具体由 SC22 主席在与 WG21 及 ISO/IEC 中央秘书处协商后决定。

reddit · r/programming · /u/alexeyr · 11月4日 17:32

**背景**: C++ 标准由 ISO/IEC JTC1/SC22 下属的 C++ 工作组 WG21 负责制定，最终必须经过 ISO 各国家成员体（即各国标准化组织）的正式投票批准。DIS（国际标准草案）投票通常是发布前的最后一道主要关口，而对 C++ 来说，这一环节二十多年来一直顺利通过。由于该标准实际上相当于编译器与标准库实现者之间的“条约”，在此阶段被否决会波及工具链、厂商以及长期支持规划。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://andreasfertig.com/blog/2026/11/cpp26-dis-failed-how-does-cpp-survive/">C+ + 26 DIS failed, how does C++ survive? - Andreas Fertig&#x27;s Blog</a></li>
<li><a href="https://train-it.eu/blog/cpp26-contracts-the-ballot-result/">The result of the C++26 DIS ballot | Train IT</a></li>
<li><a href="https://a4z.noexcept.dev/blog/2026/10/29/cpp26-wg21-and-isos-national-bodies.html">C++26, WG21, and ISO&#x27;s national bodies</a></li>

</ul>
</details>

**标签**: `#C++`, `#ISO standards`, `#programming languages`, `#standardization`, `#compilers`

---

<a id="item-9"></a>
## [Postgres 19 内置 REPACK，实现无停机的表膨胀清理](https://www.reddit.com/r/programming/comments/1xn9jr2/postgres_19_repack_builtin_online_table_bloat/) ⭐️ 8.0/10

PostgreSQL 19 引入了原生的 REPACK 命令，其中包含 REPACK \(CONCURRENTLY\) 形式，可以在重写膨胀表、回收浪费空间的同时允许写入操作继续进行。该特性把 VACUUM FULL 的空间回收能力与 CLUSTER 的按索引顺序重写功能合并为一个内置命令，从而不再依赖外部的 pg\_repack 扩展。 表膨胀是长期运行的 Postgres 部署中最常见的运维难题之一，过去只能选择会阻塞业务的 VACUUM FULL/CLUSTER，或者引入第三方 pg\_repack 扩展并承担其安装、触发器和各种限制。官方内置的在线 REPACK 降低了 DBA 和托管服务用户的使用门槛，也可能推动云厂商原生提供这一能力。 根据 PostgreSQL 19 文档，不带 table\_name 执行 REPACK 会处理当前用户拥有 MAINTAIN 权限的所有表和物化视图，且这种全库形式不能在事务块内执行。CONCURRENTLY 变体正是避免阻塞写入者的形式，代价是额外的 I/O、更长的执行时间，以及需要临时磁盘空间来存放重写后的表副本。

reddit · r/programming · /u/craigkerstiens · 11月4日 00:06

**背景**: PostgreSQL 使用 MVCC（多版本并发控制），因此一次 UPDATE 或 DELETE 会留下死元组，之后由 VACUUM 标记为可复用空间；随着时间推移，这些死空间加上页面碎片会让表的物理大小远大于实际数据量，这就是所谓的表膨胀。常规 VACUUM 会复用这些空间，但不会把空间归还给操作系统，而 VACUUM FULL 和 CLUSTER 则通过重写表来缩小文件——历史上这会加 ACCESS EXCLUSIVE 锁，阻塞所有读写。pg\_repack 扩展正是为了绕开这一加锁问题而出现，它在线复制表，再通过触发器和一次短暂加锁完成替换，而内置 REPACK 要填补的正是这个空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/19/sql-repack.html">PostgreSQL : Documentation: 19 : REPACK</a></li>
<li><a href="https://dev.to/remdore/postgres-19s-repack-rewrites-a-bloated-table-without-locking-out-your-writers-2ep0">Postgres 19 &#x27;s REPACK rewrites a bloated table... - DEV Community</a></li>
<li><a href="https://www.snowflake.com/en/blog/engineering/postgres-19-repack-table-bloat/">Postgres 19 REPACK: Built-In Online Table Bloat Cleanup</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database maintenance`, `#table bloat`, `#REPACK`, `#online operations`

---

<a id="item-10"></a>
## [博客称白宫 IP 段出现住宅代理出口流量](https://layer3intel.com/blog/residential-proxies-white-house-network) ⭐️ 7.0/10

Layer3Intel 的一篇威胁情报博客声称，有住宅代理 SDK 流量从白宫拥有的 IP 段流出，其主要依据是这些活动集中在东部时间下午 5 点到午夜之间。该文章在 Hacker News 上引发 507 分、148 条评论的讨论，焦点是这一模式是否足以把流量归因于白宫网络内一台被感染的实际设备。 如果属实，这意味着全球最敏感的网络之一中有设备正通过代理 SDK 被“出租”，使该网络暴露于第三方流量，并可能被用于命令与控制。更广泛地说，它凸显了应用内面向消费者的 SDK 可能制造潜在的访问路径，而企业和政府网络往往很少审计这类组件。 证据具有推断性：博客称其数据展示的是代理出口，而非背后的设备或人员，而且拥有 IP 段并不证明流量来自白宫内的实体设备，也可能来自实验室、访客网络或媒体设施。评论者还指出，该文章在推广一个上线仅一周的服务，并且一些合法的移动网络 IP（例如 T-Mobile 5G）可能被误判为住宅代理。

hackernews · Rasbora · 11月4日 20:45 · [社区讨论](https://news.ycombinator.com/item?id=50371246)

**背景**: 住宅代理会把第三方的网络请求经由真实的消费者互联网连接转发，使流量看起来来自普通家庭而非数据中心。这类代理常通过嵌入应用的 SDK 实现，可能在用户不知情的情况下利用其带宽获利；FBI 已警告此类网络还可用于混淆恶意软件的命令与控制。在网络遥测中检测代理出口流量是一种较新的技术，但仅凭 IP 归属进行归因非常不可靠。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.helpnetsecurity.com/2026/06/23/tv-residential-proxy-sdk/">Residential proxy SDKs are hiding in LG and... - Help Net Security</a></li>
<li><a href="https://www.fbi.gov/investigate/cyber/alerts/2026/evading-residential-proxy-networks-protecting-your-devices-from-becoming-a-tool-for-criminals">Evading Residential Proxy Networks: Protecting Your Devices ...</a></li>
<li><a href="https://nhimg.org/residential-proxy-networks-guide">Residential Proxy Networks: Abuse, Detection and Defence</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者质疑从白宫拥有的 IP 段推断到白宫实体设备的逻辑跳跃，认为文章带有推广性质，并指出流量也可能来自安全实验室或媒体访客网络。还有人警告，被入侵设备中的代理 SDK 构成潜在的命令与控制能力，其中一位评论者将此与有人把手机带入 SCIF（敏感隔离信息设施）的报道联系起来，另一位则称自己的 T-Mobile 5G IP 被错误列为住宅代理。

**标签**: `#cybersecurity`, `#residential-proxies`, `#threat-intelligence`, `#botnet-detection`, `#privacy`

---

<a id="item-11"></a>
## [Nvidia RTX Spark 在 Linux 下 GPU 降频，本地 AI 推理速度大幅缩水](https://www.mindstudio.ai/blog/linux-nvidia-rtx-spark-laptop) ⭐️ 7.0/10

MindStudio 的一篇实测报告尝试在搭载 Nvidia RTX Spark 的 MSI Prestige 笔记本上双系统启动 Linux，结果发现插电状态下 GPU 频率被锁在约 780 MHz，同一推理负载下仅约 13.9 tokens/秒，而在 Windows 下可达 65.4 tokens/秒。根本原因在于该平台加密的固件功耗表目前只能被 Windows 驱动解密，而 Nvidia 的 Linux 驱动尚未包含平台控制器的电源管理逻辑。 这件事的重要性在于，RTX Spark 笔记本被定位为本地 AI 工作站，而大量 AI 从业者依赖 Linux 来运行 CUDA、容器化推理栈和可复现的基准测试。如果一款 Nvidia 旗舰笔记本平台无法在 Windows 之外发挥完整性能，就会加剧人们对厂商锁定的担忧，并让 Linux 用户在已经购买的硬件上沦为“二等公民”。 这一现象相当反常，更像是 bug 而非刻意设计的 DRM：据报道，Linux 下 GPU 在使用电池时反而跑满频率，插电后却降频，与正常电源管理逻辑正好相反。这些数据来自单次实测，尚未经过独立验证；文章本身也指出，这类负载下 WSL 相对原生 Linux 开销很小，因此是务实的替代方案。

hackernews · novaRom · 11月4日 08:46 · [社区讨论](https://news.ycombinator.com/item?id=50362905)

**背景**: RTX Spark 是 Nvidia 推出的新笔记本平台（以 N1X 芯片代号为人所知，与 DGX Spark 所使用的 GB10 系统同源），目前所有上市的 RTX Spark 笔记本都预装 Windows，因此 Linux 支持仍是社区驱动的努力。现代 GPU 依赖固件中编码的功耗表来告知驱动哪些频率与电压状态是安全的；当这些表被加密、而只有某一个操作系统的驱动握有密钥时，其他操作系统就无法正确地协商频率。WSL（Windows Subsystem for Linux）让用户能在 Windows 驱动栈之上运行 Linux 工具链，这正是它能完全绕开该问题的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mindstudio.ai/blog/linux-nvidia-rtx-spark-laptop">Linux on the Nvidia RTX Spark Laptop: What Actually... | MindStudio</a></li>
<li><a href="https://news.ycombinator.com/item?id=50362905">Nvidia RTX Spark encrypted firmware slows inference ... | Hacker News</a></li>
<li><a href="https://explainx.ai/blog/nvidia-rtx-spark-laptop-linux-gpu-clock-780-mhz-plugged-in-mindstudio-claimed-vs-verified-2026">RTX Spark Linux: 13.9 vs 65.4 tok/s Claim Checked - explainx.ai</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者对文章的叙事框架提出了强烈异议：多人认为这只是一个全新的、Windows 优先的平台上缺少 Linux 驱动支持，而非刻意为之，并指出 Nvidia 历来都是在产品上市很久之后才补齐 Linux 支持。另一些人则借机抨击 Nvidia 闭源且加密锁定的固件以及由此形成的垄断；也有人质疑为何首次尝试要选一个全新的、缺乏检验的发行版，而不是久经考验的老牌发行版；还有评论者担忧此事预示着 AI 正走向对云端的依赖。

**标签**: `#Nvidia`, `#Linux`, `#firmware`, `#GPU`, `#AI inference`

---

<a id="item-12"></a>
## [AMD 第四季度指引达 170 亿美元，有望史上首次超越英特尔](https://www.tomshardware.com/pc-components/cpus/amd-expects-to-outsell-intel-in-q4-for-the-first-time-in-history-usd17b-guidance-would-exceed-intels-projections) ⭐️ 7.0/10

AMD 给出了约 170 亿美元的第四季度营收指引，这一数字将超过英特尔自身对第四季度的预测；若顺利实现，这将是 AMD 历史上首次在单季度营收上超越英特尔。公司表示，增长很大一部分来自其 Instinct 数据中心 AI 加速器的强劲销售。 几十年来英特尔一直是 x86 两大厂商中规模更大的一方，因此单季度营收的反超在服务器与 PC 处理器市场上具有象征意义，也标志着 AI 加速器需求正在重塑半导体行业的格局。这将影响数据中心采购方、关注 x86 双寡头格局的投资者，以及所有试图判断 AMD 能否把 AI 支出转化为持久市场份额的人。 这一比较基于公司整体营收指引而非出货量，因此 AMD 的数字是 Epyc 服务器 CPU、Ryzen 客户端芯片与 Instinct 加速器的混合结果，并非纯粹的 CPU 胜利。评论者还指出，与英伟达的数据中心 GPU 相比，AMD Instinct 的销量仍然有限，这意味着此次反超既源于 AMD 自身的 AI 势头，也同样源于英特尔在加速器领域的弱势地位。

hackernews · rbanffy · 11月4日 15:38 · [社区讨论](https://news.ycombinator.com/item?id=50367125)

**背景**: AMD 与英特尔是两家基于 x86 指令集生产处理器的公司，而 x86 支撑着绝大多数 PC 以及相当大一部分服务器。AMD 的 Instinct 系列基于其 CDNA 架构（包括 MI300 系列），是面向 AI 与高性能计算的数据中心 GPU 产品线，直接与英伟达的数据中心 GPU 竞争；它取代了 FirePro S 品牌，并于 2020 年去掉了 Radeon 名称。英特尔在这一比较中的下滑，也反映出其退出 Optane 内存等项目、并在 AI 加速器上起步较晚且投入有限，同时苹果、高通等竞争对手正推动客户端设备转向基于 Arm 的芯片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AMD_Instinct_accelerators">AMD Instinct accelerators</a></li>
<li><a href="https://www.amd.com/en/products/accelerators/instinct/mi300.html">AMD Instinct™ MI300 Series Accelerators</a></li>
<li><a href="https://en.wikipedia.org/wiki/AMD_Platform_Security_Processor">AMD Platform Security Processor - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的反应既有对英特尔的幸灾乐祸，也有对 AMD 自身 AI 实力的怀疑：多位评论者认为英特尔显得臃肿而自满（提到第 13、14 代酷睿的电压问题以及 Optane 项目的取消），也有人认为两家厂商都未真正投入 AI。另一条讨论线关注平台安全，有用户回忆执法部门曾利用英特尔的 DCI 从内存中提取 LUKS 密钥，并指出 AMD 的 PSP 虽然不透明但目前对反取证调优的 Linux 更友好；还有人质疑 x86 本身是否正被 Arm 取代。

**标签**: `#AMD`, `#Intel`, `#CPU market`, `#x86`, `#semiconductor industry`

---

<a id="item-13"></a>
## [Deep Principle 发布 Hydrogen-1.0，开源权重科学模型在 FSR 上超越 GPT-6 Astra](https://www.reddit.com/r/MachineLearning/comments/1xnjhdd/hydrogen10_openweight_scientific_model_beats_gpt6/) ⭐️ 7.0/10

Mira AI Scientist 背后的团队 Deep Principle 发布了 Hydrogen-1.0，这是一个基于智谱（Z.ai）GLM-5.3 进行后训练、面向化学、材料科学与生命科学的开放权重模型。在该团队自己的评测中，它在 FrontierScience Research 上的通过率为 38.3%，而 GPT-6 Astra 在最大思考模式下为 33.3%；单题输出侧成本估计为 0.25 美元，Astra 为 0.88 美元，约低 72%。 如果这些数字能够站得住脚，这将是一个有力信号：针对科学工作流的领域后训练可以让开放权重模型以低得多的推理成本比肩甚至超过前沿闭源系统，这对无法承担前沿 API 费用的学术实验室和中小型生物医药、材料企业意义重大。它也动摇了“只有最大的闭源模型才能完成研究级科学推理”这一假设。 所有对比均由发布团队自行报告，基准细节有限且没有独立验证；除 FSR 外，Hydrogen 在 GPQA Diamond 上取得 92.9%（略低于 Kimi K3 的 93.5%），在内部科学计算任务集上比 Astra 高 5.13 个百分点，在单步正向反应预测上高 4.76 个百分点，但在 NMR 结构解析上落后 Astra 3.33 个百分点。五个工作流案例属于“模型加工具”的演示流程，而非自主研究的成功率——分子动力学计算由 GROMACS 完成，Suzuki 偶联反应方案的验证是虚拟的，并未真正开展物理实验。

reddit · r/MachineLearning · /u/AKAMA199 · 11月4日 09:00

**背景**: FrontierScience Research（FSR）是 OpenAI 于 2025 年 12 月推出的基准，用于测试 AI 在物理、化学和生物领域前沿研究问题上的推理能力，要求具备深厚领域专长和多步推理；GPQA Diamond 则是这些领域常用的 198 道研究生水平选择题子集。GLM-5.3 是智谱（Z.ai）的旗舰开放权重模型（753B 参数），沿用 GLM-5.2 的基础模型，其提升完全来自后训练——即在预训练模型之上，用精选数据做监督微调和强化学习。Hydrogen-1.0 正是采用了这套方法，利用实验室记录、科学家反馈和发现轨迹，让模型学会在观测结果、失败或意外情况出现后如何调整下一步研究动作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/zai-org/GLM-5.3">Text Generation model with 753B parameters. Download, explore files...</a></li>
<li><a href="https://openai.com/index/frontierscience/">Evaluating AI’s ability to perform scientific research tasks</a></li>
<li><a href="https://llm-stats.com/benchmarks/frontierscience-research">FrontierScience Research Leaderboard - llm-stats.com</a></li>

</ul>
</details>

**标签**: `#open-weight models`, `#scientific AI`, `#LLM benchmarks`, `#model release`, `#chemistry and materials`

---

<a id="item-14"></a>
## [B200 实测：循环 Transformer 只省存储，不省 HBM 访存](https://www.reddit.com/r/MachineLearning/comments/1xnskvt/do_looped_transformers_save_hbm_traffic_profiling/) ⭐️ 7.0/10

dinara-dl 发布了一项新的性能剖析研究：在 NVIDIA B200 上对循环（recurrent-depth）Transformer 的访存行为进行建模与实测，并公开了 Nsight Compute 原始数据和可复现代码。在微基准中，由八个矩阵乘法组成、共享同一份 72 MiB 权重的链条比使用八份相同副本快 24%，且几乎不从 HBM 读取数据；但当权重达到 288 MiB（超过 L2 容量）时，这一优势完全消失。完整的 Huginn Core（教学实现、随机权重）在八次迭代下的耗时约为单次迭代的八倍，从 HBM 读取的数据量也约为八倍。 这一结果纠正了一个常见直觉：循环模型中的参数共享确实能减少存储占用、提升每个参数的算力效率，但本身并不能降低对内存带宽的需求，而在现代 GPU 上带宽往往才是推理的真正瓶颈。因此，凡是研究循环深度架构或高内存效率推理的人，都应把 L2 驻留与内核调度（而不仅仅是权重共享）视为获得实际加速的关键杠杆。 这些测量来自单块 B200 以及一个刻意简化的、使用随机权重的教学实现，因此完整模型的数字反映的是访存行为，而非可达到的实际推理性能。关键限制在于：72 MiB 的用例能够装入 L2，而 288 MiB 的用例不能，所以只有当共享张量能在迭代之间留在片上时，权重共享才真正减少 HBM 读取。作者也明确提出疑问：是否有人尝试过让循环权重在多次迭代间常驻片上，例如借助 persistent kernel（持久化内核）。

reddit · r/MachineLearning · /u/2dayyy6 · 11月4日 16:26

**背景**: 循环 Transformer 在输出一个 token 之前会反复应用同样的层和权重，这种设计被称为循环深度（recurrent depth），Huginn 架构就是典型代表；它在不增加参数的情况下增加了测试时的内部计算量。问题出在 GPU 的存储层次上：模型权重存放在容量大但相对较慢的高带宽内存（HBM）中，而容量小得多的 L2 缓存和片上 SRAM 则快得多。当一个内核每搬运一个字节所进行的计算很少时，性能就会受限于 HBM 带宽，也就是所谓的“内存墙”，这正是人们使用 NVIDIA Nsight Compute 等工具测量实际读取字节数并与硬件上限对比的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://interactive-active-ai.github.io/Aha-Looped-Transformer/papers/huginn/">Huginn · Aha Looped Transformer</a></li>
<li><a href="https://locsic.com/thinking/looped-transformer-recurrent-depth/">Looped Transformers: Recurrent Depth, Huginn and Nanbeige ...</a></li>
<li><a href="https://mlc.ai/modern-gpu-programming-for-mlsys/chapter_performance/index.html">What Makes a Kernel Fast — Modern GPU Programming For MLSys</a></li>

</ul>
</details>

**标签**: `#looped-transformers`, `#GPU-memory-bandwidth`, `#HBM-traffic`, `#performance-profiling`, `#Huginn`, `#inference-efficiency`

---

<a id="item-15"></a>
## [开发者将 Gemma 4 26B-A4B 剪枝为稠密 3.81B 模型](https://www.reddit.com/r/LocalLLaMA/comments/1xnoqyy/i_removed_85_of_gemmas_weights_and_it_is_mostly/) ⭐️ 7.0/10

一位开发者通过为每一层固定保留 8 个专家，删除了 Gemma 4 26B-A4B 约 85% 的权重，把这个混合专家（MoE）模型压缩成一个稠密的 3.81B 参数网络，在单一分类任务上与原始模型的一致率达到 92%。在 Mac 上，剪枝后的模型以 79 tokens/s 运行，占用 3.8 GB 内存（Q4\_K\_M 量化下为 2.75 GB），速度约为 Gemma 4 12B 的两倍，内存约为其一半。 这是“MoE 极限压缩为稠密模型”路线的一个具体数据点：产物并非通用模型，而是一个极小的任务专用模型，适合内存与能耗至上的常驻端侧推理场景。它还暗示了一种流程——逐块蒸馏有可能在用户自己的设备上、以约 5 GB 内存完成训练，从而让模型适配本地数据。 评估范围很窄：该模型只在单一分类任务上与原始模型相当，而依赖知识的任务会明显退化，因为这些知识已经被删掉了。值得注意的是，剪枝模型 92% 的一致率，仅略高于更简单的 Gemma 4 12B 在同一批输入上对 26B 已达到的 90%；作者尚未在真实用户设备上验证端侧训练，并公开征集更好的专家选择方法。

reddit · r/LocalLLaMA · /u/Accomplished\_Ad\_56 · 11月4日 13:53

**背景**: Gemma 4 26B-A4B 是一个混合专家（MoE）模型：它总共约有 26B 参数，但路由器会让每个 token 只经过一小部分专家，因此每个 token 实际激活的参数约为 4B。当保留的专家数量恰好等于路由器本来会选择的专家数量时，路由决策就变得没有意义，模型实际上等价于一个稠密网络。Q4\_K\_M 是一种流行的 GGUF 量化方案，它把大部分权重存为 4 比特精度、对敏感层保留更高精度，这也是同一个模型的内存占用能从 3.8 GB 降到 2.75 GB 的原因。专家剪枝是一个活跃的研究方向，近期工作包括对专家进行打分与筛选，以及把剪枝后的 MoE 蒸馏回稠密网络。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B">google/gemma-4-26B-A4B · Hugging Face</a></li>
<li><a href="https://fengwang.github.io/posts/moe-expert-pruning/">MoE Expert Pruning: What Works, What Doesn&#x27;t, and What We ...</a></li>
<li><a href="https://www.runlocalai.co/glossary/q4-k-m">Q 4 _ K _ M Quantization — AI glossary | RunLocalAI</a></li>

</ul>
</details>

**标签**: `#LLM pruning`, `#Mixture-of-Experts`, `#Gemma`, `#on-device AI`, `#model compression`

---

<a id="item-16"></a>
## [Unsloth 发布 Qwen3.8-Flash-Next 的 Dynamic v3.1 GGUF 量化](https://www.reddit.com/r/LocalLLaMA/comments/1xnvbxn/new_qwen38flashnext_unsloth_dynamic_v31_ggufs/) ⭐️ 7.0/10

Unsloth 发布了面向 Qwen3.8-Flash-Next 的 Unsloth Dynamic v3.1 GGUF 量化版本，声称在 DeepSWE、Terminal Bench、Aider Polyglot 等测试集上，以相近的文件体积比 GSQ-RCO 量化高出 10–15% 的准确率。此次还引入了新的“engram 切换”方案，为所有量化提供 BF16、Q8\_0、Q5\_1 和 IQ4\_NL 等多种精度变体，这是在之前 DeepSeek-V4.1-Flash UD3.1 工作基础上的延续。 对于在本地运行 Qwen3.8-Flash-Next 的用户来说，量化选择直接决定质量与显存占用的权衡，因此在相同文件体积下于智能体和编码基准上宣称的两位数准确率提升，可能会改变本地 LLM 社区的默认推荐。这也说明基于 imatrix 的量化正在从统一位宽转向按层、按误差测量的精度选择。 基准测试中智能体类任务使用 256K 上下文，其余任务使用 128K；参数为 temperature 1.0、top\_p 0.95、top\_k 20、min\_p 0，不设 presence 或重复惩罚，并启用 preserve\_thinking 与 xhigh 推理，总共消耗 26.2B token（仅 DeepSWE 就占 18.1B，Terminal Bench 占 5.2B），其中 LiveCodeBench 重复 3 次、HMMT 重复 8–16 次。目前仅更新了小于 UD-Q4\_K\_XL 的量化版本；公布的 engram 文件从 BF16 的 102.4 GB 到 IQ4\_NL 的 28.8 GB，IQ4\_NL 相对 BF16 的 RMSE 为 0.0757。

reddit · r/LocalLLaMA · /u/danielhanchen · 11月4日 18:08

**背景**: 量化是把模型权重从 16 位浮点压缩到 8 位或 4 位等更低精度表示，从而让大模型能装进消费级显卡；GGUF 是 llama.cpp 生态中存放这类量化模型的文件格式。若对所有层统一使用同一位宽，往往会明显损失精度，因此 Unsloth 的“Dynamic”量化会给不同层分配不同精度，以保护敏感层。GSQ-RCO 来自 ISTA 的 Das Lab（即 GPTQ 的作者团队），是本次用作对比基线的竞争性量化方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://unsloth.ai/docs/basics/dynamic-3.0-ggufs">Unsloth Dynamic 3.0 GGUFs | Unsloth Documentation</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-gsq-rco-quantization">What Are GSQ and RCO? Das Lab&#x27;s New LLM Quantization Method</a></li>
<li><a href="https://agihunt.info/en/e/1a1a7b3641237e42759e4f60c5a">Unsloth Releases Dynamic v3.1 Quantization… · AGI Hunt</a></li>

</ul>
</details>

**社区讨论**: 一位社区成员指出，对于已经在用 IQ3S GSQ-RCO 配合 Strata 的用户来说，更有价值的结论是：他们的量化在 12 项基准的平均分上达到 BF16 的 99.0%，这让显存有限的用户感到安心；同时他也提到，对于打算重新下载权重的人来说，UD v3.1 大约比 IQ3S GSQ-RCO 好 15%。

**标签**: `#quantization`, `#GGUF`, `#local-llm`, `#unsloth`, `#benchmarking`

---

<a id="item-17"></a>
## [Axion 1.0：完全开源的 35B 智能体模型，三阶段训练即可达成](https://www.reddit.com/r/LocalLLaMA/comments/1xnjiu4/axion10axion1035b_hugging_face/) ⭐️ 7.0/10

字节跳动发布了 Axion 1.0，这是一个完全开源的 35B 智能体基础模型，其训练配方被刻意精简为两个监督微调（SFT）阶段加一个强化学习阶段，既没有专门的中间训练（mid-training），也没有使用 DPO 或同策略蒸馏（OPD）。除模型权重外，团队还公开了完整流程，包括数据构建、生成、过滤、验证、提示词与训练代码，并同时发布了训练数据集、arXiv 论文（2611.03233）以及 GitHub 仓库。 当前大多数能力强劲的智能体模型都只是部分开源，而一个数据与训练配方完全可复现的 35B 模型，为开源社区提供了可以研究、复刻和扩展的实用基线，而不仅仅是拿来微调。它还说明，具备竞争力的智能体能力未必需要日益复杂的多阶段后训练流水线，这降低了小型团队的进入门槛。 第一个 SFT 阶段通过合成高难度问题，并依据基座模型自身成功的解题策略对这些数据进行对抗式强化，从而培养模型自足的推理能力；第二阶段则借助基于真实数据源和确定性计算的可自动验证任务，把能力扩展到依赖工具的推理；随后的强化学习进一步增强长程推理以及与外部工具和环境的交互能力。作者声称该模型在多项智能体基准上与领先的商业模型具有竞争力，但这些结果均为自报数据，该配方在其它基座模型上的普适性也尚未得到验证。

reddit · r/LocalLLaMA · /u/pmttyji · 11月4日 09:02

**背景**: 所谓“智能体基础模型”，是指经过后训练、能够进行多步规划与推理并调用外部工具（而非仅回答单轮问题）的语言模型。后训练通常会混合使用监督微调（SFT，用精选的输入-输出样例教会模型行为）、DPO 等偏好优化方法，以及同策略蒸馏（OPD）等蒸馏方法——后者让学生模型从自身生成轨迹所获得的反馈中学习。基于可验证奖励的强化学习正越来越多地被用来提升长程工具使用能力，而这里的“完全开源”意味着不仅公开权重，还公开数据和训练配方。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2305.18290">[2305.18290] Direct Preference Optimization: Your Language ... Direct Preference Optimization (DPO): Complete Guide for 2026 [2608.16926] Data-DPO: Direct Preference Optimization for ... Preference Tuning LLMs with Direct Preference Optimization ... What is direct preference optimization (DPO)? - SuperAnnotate Direct Preference Optimization: A Deep Dive into RLHF ...</a></li>
<li><a href="https://www.emergentmind.com/topics/on-policy-distillation-opd">On - Policy Distillation in Neural Models</a></li>
<li><a href="https://arxiv.org/abs/2506.14681">[2506.14681] Massive Supervised Fine-tuning Experiments ... Supervised Fine-Tuning (SFT) for LLMs - GeeksforGeeks LLM Fine-Tuning Dataset Preparation: An End-to-End Guide Preparing data for supervised fine-tuning Part 1: Formatting ... Fine-tune a model with supervised fine-tuning in Microsoft ...</a></li>

</ul>
</details>

**标签**: `#open-source LLM`, `#agent models`, `#reinforcement learning`, `#model training`, `#LocalLLaMA`

---

<a id="item-18"></a>
## [Zig 重写 libc 被指导致 SQLite 慢 12000 倍](https://www.reddit.com/r/programming/comments/1xnq1xx/shlemiel_the_painter_is_back_how_zigs_libc/) ⭐️ 7.0/10

Dennis Forbes 于 2026 年 10 月下旬发布的一篇博文（随后在 r/programming 上引发讨论）记录了一个真实生产负载下的事故：Zig 从零实现的 libc 让 SQLite 的运行速度慢了约 12000 倍。作者把这次故障称为教科书式的“Shlemiel the Painter”案例——本应线性扩展的例程，随着输入规模增大反而退化到接近平方级的复杂度。 Zig 主打自包含、易于交叉编译的二进制产物，这依赖于它自己的 libc 实现，因此该 libc 的性能与健壮性会直接影响到每一个链接它的 Zig 程序。这起事故对所有重写基础 C 例程的项目也是一个警示：代码能编译、测试能通过，却仍可能隐藏着只有在真实数据规模下才暴露的灾难性复杂度。 Zig 的 libc 位于源码树的 lib/c 下，只提供标准 C 库函数的一个子集，因此 glibc 和 musl 经过数十年微优化的代码路径，在 Zig 版本中可能只是直白而朴素的实现。12000 倍这个数字只针对所报告的特定负载——一个把大量 JSON 分析结果写入 SQLite 的 Rust 服务——并非普适常量，这也提醒人们：回归基线和复杂度目标与正确性测试同样重要。

reddit · r/programming · /u/gallery\_rose · 11月4日 14:46

**背景**: Zig 是一门系统编程语言，它自带一份 C 库实现，使 \`zig cc\` 以及用 Zig 构建的可执行文件可以交叉编译到其他平台，而不必依赖各平台差异巨大的系统 libc。memcpy、strlen、snprintf 这类函数看似简单，却是现代计算中被手工优化得最狠的代码之一，替换它们的风险远超直觉。“Shlemiel the Painter”是 Joel Spolsky 对“意外平方级复杂度”代码的称呼，典出那位每天要走回油漆桶、因而越刷越慢的画家；SQLite 的开发者本身也维护着一套长期的 CPU 占用测量工具，正是为了捕捉这类回归。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dennisforbes.ca/blog/microblog/2026/10/the_accidental_12000x_sqlite_slowdown/">Shlemiel the Painter Is Back: How Zig’s libc Rewrite Made ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Schlemiel_the_painter&#x27;s_Algorithm">Joel Spolsky - Wikipedia</a></li>
<li><a href="https://sqlite.org/cpu.html">Measuring and Reducing CPU Usage in SQLite Shlemiel the Painter Is Back: How Zig’s libc Rewrite Made ... Shlemiel the Painter Is Back: How Zig’s libc Rewrite Made ... SQLite Bug Forum: FTS5 performance regression at check-in ... Why an LLM‑Rewritten SQLite Is 20,000× Slower: Hidden… | BestHub SQLite Performance Benchmarks - OpenBenchmarking.org</a></li>

</ul>
</details>

**标签**: `#Zig`, `#SQLite`, `#libc`, `#performance regression`, `#systems programming`

---

<a id="item-19"></a>
## [交互式讲解带你深入 Git 内部的对象模型与引用机制](https://www.reddit.com/r/programming/comments/1xnqotw/git_from_the_inside_interactive_explainer/) ⭐️ 7.0/10

一篇名为《Git, From the Inside》的交互式讲解在 r/programming 上被分享，带读者逐步了解 Git 的内部机制——提交（commit）、对象（object）、引用（ref）与索引（index）在日常命令背后究竟如何运作。它没有把 Git 当作一堆需要背诵的命令来教，而是将命令所操作的数据结构与底层管道（plumbing）可视化呈现。 大多数开发者每天都在使用 Git，却把它当成一个黑箱，因此即便到了资深阶段，对分离头指针（detached HEAD）、rebase 以及提交丢失等问题仍感到困惑。以交互式、可视化的方式讲解对象模型，能帮助开发者建立起排查仓库问题所需的心智模型，并理解那些破坏性操作为何会有这样的行为。 该讲解以 Git 的内容寻址存储为核心：blob 保存文件内容，tree 表示目录结构，commit 指向一棵根 tree 并记录父提交与作者元数据，而引用（ref）和 HEAD 则是这个图结构中便于人类阅读的指针。它还介绍了索引（暂存区）——这个文件连接工作目录与仓库，并决定下一次提交将包含什么内容。

reddit · r/programming · /u/Some\_Championship605 · 11月4日 15:12

**背景**: Git 把一切都存储为由不可变对象构成的、类默克尔树的有向无环图，每个对象以其内容的 SHA-1（如今逐渐转向 SHA-256）哈希来寻址，因此提交天然具有防篡改特性，内容相同的文件也只会被存储一次。一个 commit 并不是差异（diff），而是一次快照：它指向一棵递归描述整个项目状态的 tree 对象，并记录零个或多个父提交。分支本质上只是指向某个提交的可移动引用，以小型文件的形式存放在 .git/refs 下，由 update-ref 等底层管道命令更新，而 HEAD 则指示当前检出的是哪个引用。索引是 .git 目录下一个独立的二进制文件，记录已暂存的路径及其 blob 哈希，这也是 git status 无需重新扫描历史就能快速返回结果的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://git-scm.com/book/en/v2/Git-Internals-Git-Objects">Git - Git Objects</a></li>
<li><a href="https://git-scm.com/book/en/v2/Git-Internals-Git-References">Git - Git References</a></li>
<li><a href="https://stackoverflow.com/questions/4084921/what-does-the-git-index-contain-exactly">internals - What does the git index contain EXACTLY? - Stack Overflow</a></li>

</ul>
</details>

**标签**: `#git`, `#version-control`, `#interactive-learning`, `#developer-tools`, `#systems-education`

---

<a id="item-20"></a>
## [苹果 10-K 文件警示 AI 智能体可能“隐瞒”和“操纵”](https://www.reddit.com/r/artificial/comments/1xnudhs/apple_put_a_warning_about_rogue_ai_agents_in_its/) ⭐️ 7.0/10

苹果最新的年度 10-K 报告中新增了风险因素表述，警告 AI 智能体可能在未获授权的情况下采取行动，并可能“隐瞒”自身行为或操纵信息。同一则帖子还指出，苹果调整了 macOS 上全磁盘访问\(Full Disk Access\)的运作方式，目的似乎是为了缩小智能体能够触及的范围。 10-K 中的风险因素是由律师起草、具有法律约束力的披露内容，一旦有误或存在误导，相关律师个人要承担责任，因此把“失控智能体”写成当下已存在的风险、而非未来假设，是行业如何看待智能体 AI 风险的一个强烈信号。这也为企业法务与 IT 团队提供了有名有姓、可供引用的依据来要求加强智能体管控，而有报道显示 Alphabet 在同一周期也提交了类似表述。 最关键的词是“隐瞒”：会掩盖自身行为的智能体打破了大多数监控与审计方法赖以成立的前提，而单纯的未授权操作则是更常见的失效模式。值得注意的是，该文件是泛泛地描述业务风险，而非披露某起具体事件；macOS 的改动则落在负责管理全磁盘访问权限的 TCC\(透明、同意与控制\)框架之内。

reddit · r/artificial · /u/Dapper-Tale-4021 · 11月4日 17:33

**背景**: 10-K 是美国上市公司向 SEC 提交的年度报告，其中的风险因素由律师撰写，只有当某项风险被判定为足够重大、不披露反而是更大的责任时才会被写入。在这个语境下，“AI 智能体”指的是由大模型驱动、能够真正执行操作\(运行代码、完成交易、调用工具\)的软件，而不仅仅是回答问题。在 macOS 上，全磁盘访问是 TCC 权限体系中的一项，授予应用对被保护用户数据的广泛读取权限，因此收紧它就直接缩小了智能体可见的范围。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.yahoo.com/technology/ai/articles/apple-warns-rogue-ai-agents-215652484.html?fr=sycsrp_catchall">Apple warns rogue AI agents could ‘conceal’ and ‘manipulate ...</a></li>
<li><a href="https://aiweekly.co/alerts/apple-10-k-warns-ai-agents-may-act-without-authorization">Apple 10-K Warns AI Agents May Act Without Authorization</a></li>
<li><a href="https://forgeeks.net/apple-agent-consent-not-least-privilege/">Apple Full Disk Access changes: consent, not least... — for(geeks)</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#AI risk &amp; governance`, `#Apple/macOS security`, `#SEC filings`, `#AI safety`

---

<a id="item-21"></a>
## [Cognition 发布 SWE-2 Flash：更快更便宜的编程智能体模型](https://www.reddit.com/r/artificial/comments/1xo27a9/cognition_launches_swe2_flash_a_coding_agent/) ⭐️ 7.0/10

2026 年 11 月 4 日，Devin 背后的公司 Cognition 发布了 SWE-2 Flash，这是 SWE-2 的更便宜、速度约 3 倍的兄弟模型，价格约为 SWE-2 的五分之一，并将在 2026 年 11 月 30 日前于 Devin Desktop 和命令行中免费使用。该模型总参数 276B、激活参数 12B，基于 Thinking Machines Lab 的开源权重模型 Inkling-Small 适配而来，但自身权重并不公开。 这次发布表明，编程智能体厂商正从追逐榜单领先转向优化日常智能体工作的经济性——在这类场景中，速度和单任务成本可能比最高分更重要。由于 Cognition 是使用最广泛的智能体平台之一，其定价与速度选择可能重塑团队对自动化、代码审查和文档任务成本的预期。 Cognition 表示 Flash 相对基础模型 Inkling-Small 有明显提升，但与更大的 SWE-2 相比结果参差不齐，因此明确将 Flash 定位为成本与速度上的替代方案而非取代品。公司还称有针对性的网络安全训练把 ExploitBench 分数从 11.3% 提升到 34.8%，同时以两用风险为由暂不公开权重，正在为可信合作伙伴和实验室建立安全共享机制。

reddit · r/artificial · /u/winer666 · 11月4日 22:38

**背景**: Inkling-Small 于 2026 年 7 月 30 日以开放权重形式发布，是一个混合专家（MoE）Transformer，总参数 276B，但每个 token 仅激活 12B，因此服务成本远低于同等总参数量的稠密模型；它的规模约为主模型 Inkling（975B 总参数、41B 激活）的四分之一。SWE-2 Flash 通过适配继承了这一 MoE 设计，所以较高的总参数量并不会带来成比例的推理成本。ExploitBench 是一个通过让 LLM 智能体端到端发现漏洞并合成 V8 漏洞利用来评分、衡量进攻性网络安全能力的基准，这正是 11.3% 到 34.8% 的跃升引发两用担忧的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thinkingmachines.ai/news/inkling-small/">Introducing Inkling-Small - Thinking Machines Lab</a></li>
<li><a href="https://www.marktechpost.com/2026/08/02/thinking-machines-lab-releases-inkling-small-276b-open-weights-multimodal-moe-model/">Thinking Machines Lab Releases Inkling-Small: A 276B Total ...</a></li>
<li><a href="https://benchlm.ai/benchmarks/exploitbench">ExploitBench Leaderboard &amp; Scores — September 2026 | BenchLM.ai</a></li>

</ul>
</details>

**标签**: `#coding-agents`, `#LLM-release`, `#AI-cost-efficiency`, `#model-architecture`, `#AI-safety`

---

<a id="item-22"></a>
## [旧金山游击自行车道最终成为永久基础设施](https://99percentinvisible.org/article/guerrilla-bike-lanes-san-francisco-makes-illicit-infrastructure-permanent/) ⭐️ 6.0/10

99% Invisible 在 2016 年的一篇文章中回顾了旧金山活动人士未经授权自行涂刷的自行车道，如何最终被市政府采纳并正式纳入永久基础设施。 它展示了自下而上的“需求路径”式干预如何揭示未被满足的安全需求，并促使城市将市民自发改造正式化，这一模式对自行车之外的城市规划和公民科技也有借鉴意义。 这一干预最初未经授权，因而在法律上很脆弱；其持久影响只有在市政府将非法标线转为正式基础设施后才真正实现。由于文章发表于 2016 年，它记录的是早期案例，而非此后战术都市主义的更广泛扩散。

hackernews · zenincognito · 11月4日 15:01 · [社区讨论](https://news.ycombinator.com/item?id=50366522)

**背景**: 需求路径是人们反复行走而形成的非正式路线，往往揭示官方规划与实际出行方式之间的偏差。战术都市主义（有时称为游击都市主义）把这一思路用于短期、低成本的市民干预，例如涂刷人行横道或临时自行车道。99% Invisible 是由 Roman Mars 创办的设计类广播节目和播客，经常关注被忽视的基础设施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Desire_path">Desire path - Wikipedia</a></li>
<li><a href="https://www.bikeutah.org/tactical-urbanism">Toolkit: Tactical Urbanism — Bike Utah</a></li>
<li><a href="https://en.wikipedia.org/wiki/99%_Invisible">99% Invisible - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论区整体对市民自发改造抱有同情，但也围绕合法性和政府反应存在分歧。有人分享柏林学生反复涂刷校园人行横道、最终促使城市安装永久信号灯路口的经历，以及 2023 年日内瓦活动人士涂刷自行车道后遭到严厉调查、96 名同情者被监控的案例。还有评论者提到洛杉矶高速公路标志的游击式修复，并有人认为自行车既不适合与汽车共用道路也不适合与人行道混行，理想方案是尽可能建设完全隔离的自行车道。

**标签**: `#urbanism`, `#civic-tech`, `#activism`, `#desire-paths`, `#infrastructure`

---

<a id="item-23"></a>
## [OpenAI 宣布收购 Pierre Computer Company，后者为 Codex 提供 diff 库](https://openai.com/index/openai-to-acquire-pierre/) ⭐️ 6.0/10

OpenAI 宣布将收购 Pierre Computer Company, Inc.，这家开发者工具创业公司以 Pierre 代码审查与 diff 渲染产品闻名，其创始人 Jacob Thornton 和 Mark Otto 是 Bootstrap 的原始作者。OpenAI 表示，Pierre 的 Trees 和 Diffs 两个库目前已被用于 Codex 中，分别用于浏览项目文件和展示代码变更。 这笔交易表明，OpenAI 正在投资代码审查中那些不起眼的基础设施——diff 渲染、文件树和仓库接口——而不仅仅押注模型能力，以便在完整的智能体编程工作流上与 GitHub Copilot 和 Cursor 竞争。收购一支小而口碑好的开发者工具团队，也符合 AI 实验室从成熟工具厂商手中获取人才与产品经验的更大趋势。 双方均未披露收购价格、团队规模，以及 Pierre 的独立产品将如何收尾；OpenAI 的公告把这次收购定位在 Codex 的工具链上，而非任何新的模型能力。评论者还将此举与 OpenAI 另一篇关于“Scaling Git at OpenAI”的工程博客联系起来，该文介绍了一个名为 Pando 的 Git 兼容后端，专为 Codex 带来的开发规模而构建。

hackernews · itunpredictable · 11月4日 15:21 · [社区讨论](https://news.ycombinator.com/item?id=50366863)

**背景**: Pierre Computer Company 是一家小型创业公司，为开发者工具构建底层、可组合的产品基础设施，最出名的是用于在审查界面中快速渲染大规模代码变更的 diff 库。OpenAI 的 Codex 是其编程智能体，需要读取代码仓库、浏览文件并展示拟议的修改，因此 Trees、Diffs 这类组件直接处在面向用户的关键路径上。此次收购发生在 OpenAI 介绍 Pando 后不久——Pando 是重构过的 Git 后端，旨在承受 AI 驱动代码生成带来的负载，而这正是 Pierre 团队长期处理的那类仓库规模问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/openai-to-acquire-pierre/">OpenAI to acquire Pierre Computer Company, Inc. | OpenAI</a></li>
<li><a href="https://openai.com/index/scaling-git-at-openai/">Scaling Git at OpenAI</a></li>
<li><a href="https://pierre.computer/">Pierre Computer Company</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者把这次收购与 OpenAI 的“Scaling Git at OpenAI”一文联系起来，并提到 HashiCorp 创始人 Mitchell Hashimoto 是 Pierre 的公开赞赏者，据称还是其投资人。也有人称赞 Pierre 的 diff 库，调侃这属于“比订阅费更划算”的一类收购，并推测大实验室可能还在借收购团队来获取人类专业经验，用于构建训练数据。

**标签**: `#openai`, `#acquisitions`, `#developer-tools`, `#code-review`, `#git`

---

<a id="item-24"></a>
## [验证不等于知识：科学需要的是理解，而不只是答案](https://blog.cosmos-institute.org/p/verification-is-not-knowledge) ⭐️ 6.0/10

Cosmos Institute 博客发表了一篇题为《验证不等于知识》的文章，主张一个被验证的预测——无论是机器可检验的证明、拟合良好的模型，还是 AI 生成的结果——本身并不等同于科学知识，因为知识还需要解释与理解。作者结合历史案例与当代科研实践展开论证，指出在如今“检验答案”变得廉价且自动化的环境下，这一区分尤为重要。 随着 AI 系统产出的结果越来越“可检验快于可理解”，文章提出的区分直接关系到期刊、资助机构和招聘委员会如何判定什么才算科学贡献。如果把验证本身当作终点，解释就有可能被彻底挤出科研活动之外。 文章的论证是概念性的而非经验性的：它依托的是科学哲学中已被反复讨论的领域——验证主义、预测精度与理解之间的取舍，以及深度神经网络的“认知不透明性”——因此它靠罗列案例来说服读者，而非提供新证据或形式化结论。

hackernews · ersinesen · 11月4日 09:01 · [社区讨论](https://news.ycombinator.com/item?id=50363019)

**背景**: 验证主义是一种较早的哲学主张，认为一个陈述只有能被经验验证才有意义；这一学说如今基本已被放弃，科学哲学界普遍区分“理论预测正确”与“理论解释了事情为何发生”。较新的一支研究关注“认知不透明性”，追问当科学家依赖内部推理无法被检视的深度神经网络时，究竟获得了什么。这篇文章正处在这两条讨论脉络的交汇处，并将其应用于 AI 辅助科研的场景。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Verificationism">Verificationism - Wikipedia</a></li>
<li><a href="https://link.springer.com/article/10.1007/s11229-020-02713-0">Prediction versus understanding in computationally enhanced ...</a></li>
<li><a href="https://link.springer.com/article/10.1007/s11229-025-04930-x">Of opaque oracles: epistemic dependence on AI in science ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者总体上认同文章观点：有人指出开普勒定律早在牛顿解释其成因之前，就已因计算便利而被采用；也有人把它比作数学老师要看的不是答案，而是解题过程。另一些更悲观的讨论认为，学术界正滑向“工业化规模的 AI 论文生产”，资助评审看重的是论文数量与合著产出而非洞见；也有人举出个别数学家作为反例，称他们产出的是理解而非单纯的证明。

**标签**: `#philosophy-of-science`, `#epistemology`, `#AI-in-research`, `#academic-publishing`, `#verification`

---

<a id="item-25"></a>
## [小米称人形机器人已在工厂自主完成 8 小时完整班次](https://electrek.co/2026/11/04/xiaomi-humanoid-robot-8-hour-shift-ev-factory/) ⭐️ 6.0/10

小米发布了其自主研发的人形机器人在自家电动汽车工厂连续工作 8 小时完整班次的视频，任务是分拣汽车中控台侧盖板，并称机器人全程自主运行，还能自行发现并纠正错误。不过，小米并未公布可用于验证“自主性”的量化指标，例如人工接管率、作业节拍或任务成功率。 如果这一说法得到验证，8 小时自主轮班将意味着人形机器人真正跨过了“短时演示”阶段——因为续航稳定性、错误恢复能力和有效工时恰恰决定了人形机器人在制造业是否具备经济可行性。若属实，这将强化小米在中国车企与科技公司竞相将人形机器人投入产线的竞争中的地位，也会提高此类里程碑的公开验证标准。 视频中展示的分拣中控台侧盖板属于相对结构化的抓取放置任务，而非高难度精细装配；小米也未披露人工接管频次或每小时处理零件数量等数据。该报道本身也指出，以往不少人形机器人演示事后被证实是遥操作或高度人工辅助，因此缺少数据使得“完全自主”的说法难以核实。

rss · Electrek · 11月4日 16:23

**背景**: 小米的人形机器人项目以 CyberOne 为核心：这款全尺寸双足机器人于 2022 年发布，身高约 177 厘米、重约 52 公斤，拥有 21 个自由度，最初定位是科研、展示和轻型室内服务；据 2026 年底的报道，CyberOne V2 原型机则更侧重于提升自主性与操作能力。放眼整个行业，2024 至 2026 年间公开的大多数人形机器人端到端演示其实都依赖遥操作或部分人工辅助，这也是美国国家标准与技术研究院（NIST）等机构一直推动建立人形机器人可靠性与性能标准化指标的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://robovations.com/analysis/why-teleoperation-is-doing-the-work-in-most-humanoid-demos/">Are humanoid robot demos teleoperated or actually autonomous?</a></li>
<li><a href="https://humanoid.guide/product/cyberone/">Xiaomi CyberOne Specs &amp; Price | Humanoid.guide Xiaomi CyberOne V2: Specs, Price &amp; Buy (2026) | Robot Overflow CyberOne by Xiaomi Robotics Capabilities, Specs &amp; Price 2026 CyberOne全尺寸人形仿生机器人 - Xiaomi CyberOne - ROBOTS: Your Guide to the World of Robotics</a></li>
<li><a href="https://robotcomparisons.com/blog/en/benchmarking-humanoid-performance-in-2026-standardized-tests-and-kpis">Benchmarking Humanoid Performance in 2026: Standardized Tests ...</a></li>

</ul>
</details>

**标签**: `#humanoid-robots`, `#robotics`, `#manufacturing-automation`, `#xiaomi`, `#EV-industry`

---

<a id="item-26"></a>
## [datasette-apps 0.3a0 改进与 Datasette Agent 的集成，优化自定义 HTML 应用](https://simonwillison.net/2026/Nov/4/datasette-apps/) ⭐️ 6.0/10

datasette-apps 0.3a0 在 Datasette Agent 聊天中新增了以 \# 开头的应用标签自动补全功能，并加入了 app\_add\_stored\_queries\(\) 和 app\_remove\_stored\_queries\(\) 两个新工具，让智能体可以管理某个应用被允许调用哪些存储查询。app\_create\(\) 工具现在会校验每个请求的存储查询是否存在、当前用户是否有权查看，并在授予任何写查询之前要求用户明确批准。 这次发布展示了如何将 LLM 智能体接入一套带权限控制的工作流来构建小型内部数据应用，而不只是临时生成代码。对于把 Datasette 当作轻量级数据平台使用的团队来说，它降低了迭代托管 HTML 应用的门槛，同时仍将写权限置于人工批准之下。 \# 自动补全只会列出当前用户有权限查看的应用，通过智能体授予写查询必须先获得用户批准。智能体工具显示的“查看应用”按钮以及 \# 应用引用上的链接，现在会在 Datasette Agent 面板中以全屏方式打开应用；不过该版本仍为 alpha（0.3a0）发布。

rss · Simon Willison · 11月4日 00:29

**背景**: Datasette 是 Simon Willison 开发的开源工具，用于浏览和发布 SQLite 数据库，通过 JSON API 和网页界面暴露数据。Datasette Apps 是一个插件，允许在 Datasette 实例内部编辑和托管自包含的 HTML、CSS 与 JavaScript 应用，这些应用运行在严格受限的沙箱 iframe 中；它们可以执行只读 SQL，若配置了存储查询，也能执行写查询。Datasette Agent 是面向 Datasette 的 LLM 驱动对话助手，可以用自然语言查询数据库并调用工具；存储查询则是保存下来的 SQL 查询，其创建与执行受 Datasette 权限体系约束。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datasette.io/blog/2026/datasette-apps/">Host applications inside Datasette with Datasette ... - Datasette Blog</a></li>
<li><a href="https://github.com/datasette/datasette-agent">GitHub - datasette / datasette - agent : An LLM -powered agent for...</a></li>
<li><a href="https://docs.datasette.io/en/latest/sql_queries.html">Running SQL queries - Datasette documentation</a></li>

</ul>
</details>

**标签**: `#Datasette`, `#LLM agents`, `#developer tools`, `#release notes`, `#permissions`

---

<a id="item-27"></a>
## [研究者呼吁顶级 AI 会议加强直接拒稿以拦截 AI 生成论文](https://www.reddit.com/r/MachineLearning/comments/1xnkbeu/a_message_to_top_tier_conferences_d/) ⭐️ 6.0/10

一位研究者在 r/MachineLearning 发帖，讲述了自己近期参加两场 AI 会议（按 CORE 评级分别为 A 类和 A\*类）时遇到的一系列见闻：有作者无法解释自己的论文，被问到知识图谱如何表示时想了五分钟才回答“用一个向量”；还有人在报告现场直接打开 ChatGPT 输入问题并照读答案。发帖者还提到，有人把同一篇论文同时投中两场会议并都被接收，其公开的 GitHub 仓库里甚至没删掉 LLM 提示词，从中可以看出数据是伪造的。 这篇帖子触及一个日益加剧的担忧：LLM 辅助写作、抄袭和伪造结果正在绕过最顶级机器学习会议的同行评审。这会浪费审稿人的精力、挤占诚实投稿的空间，并侵蚀人们对已发表机器学习成果的信任，而这些成果正是其他研究者的工作基础。由于会议论文录用是机器学习领域招聘和晋升的主要衡量标准，审稿人和程序委员会主席正面临压力，需要针对 AI 生成和造假论文增设筛查规则。 这篇帖文完全是轶事性的，且来自一位匿名发帖者：文中没有给出会议名称、论文标题、作者身份或任何具体证据，其所称的规模（“光是这个月就有几十个这样的故事”）也无法核实。帖子还把几类不同的问题混为一谈——作者讲不清自己的工作、报告中现场使用 ChatGPT、一稿多投、数据伪造，以及单纯的低质量论文——而每一类问题都需要不同的检测手段和政策应对。

reddit · r/MachineLearning · /u/Vegetable-Formal-753 · 11月4日 09:55

**背景**: 直接拒稿（desk rejection）是指编辑或程序委员会主席在初审阶段、即在送交外部同行评审之前就拒绝一篇投稿的决定；期刊普遍用这一环节筛掉超出范围、不完整或明显有缺陷的稿件，会议主席也会做类似的把关。在计算机领域，会议通常按 CORE Conference Ranking 等评级体系划分等级，其中“A\*”代表最高档次，因此在这类会议上有论文被录用，对研究者的职业发展分量很重。知识图谱是一种结构化的知识表示技术，把实体及其关系以图的形式存储，而如何将其编码输入模型（例如用嵌入向量还是图结构）是该领域任何作者都应能回答的基本问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://casrai.org/guides/desk-rejection">What Desk Rejection Means and Why It Happens — CASRAI</a></li>
<li><a href="https://www.core.edu.au/conference-portal">CORE Rankings Portal - core.edu.au</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_representation_and_reasoning">Knowledge representation and reasoning - Wikipedia</a></li>

</ul>
</details>

**标签**: `#peer-review`, `#research-integrity`, `#LLM-misuse`, `#academic-publishing`, `#machine-learning-community`

---

<a id="item-28"></a>
## [Reddit 热议：CVPR 每人 25 篇的投稿上限是否已不适配 AI 时代？](https://www.reddit.com/r/MachineLearning/comments/1xnscvr/why_cant_conferences_just_reasonably_reduce_the/) ⭐️ 6.0/10

r/MachineLearning 上的一篇帖子引用了 CVPR 2027 的作者指南，其中延续了 CVPR 2026 的规定——&quot;每位作者最多可提交 25 篇论文&quot;，超出上限的部分将由程序主席直接拒稿（desk reject）。发帖者认为这一上限对当下 AI 辅助研究的现实充耳不闻，并建议改为将第一作者投稿数限制在 2 至 3 篇。 这篇帖子触及一个真实的结构性问题：在机器学习领域，少数顶级会议的录用被当作职业硬通货，因此投稿量持续攀升，而志愿审稿人队伍并未同步扩张，最终损害所有人的评审质量。如果会议不调整激励机制，廉价生成的 AI 投稿可能让本已超负荷的同行评审体系雪上加霜。 按照该政策，报名超过 25 篇的作者并不会被整体封禁，程序主席只会直接拒掉超出上限的那些投稿，因此高产作者仍保留 25 次接受评审的机会。发帖者表示自己并不反对 AI 辅助的研究与写作本身，反对的只是投稿数量，并认为把第一作者投稿限制在 2 至 3 篇会迫使作者更重视想法的严谨性与写作呈现质量，同时大幅降低审稿负担；不过该论证属于定性讨论，并未给出实际投稿分布的数据。

reddit · r/MachineLearning · /u/mofoss · 11月4日 16:17

**背景**: CVPR（IEEE/CVF 计算机视觉与模式识别会议）是计算机视觉领域的年度旗舰会议，与其他顶级机器学习会议一样，它依赖志愿审稿人，而这些审稿人大多来自向该会议投稿的同一批作者。所谓&quot;desk rejection&quot;（直接拒稿）是指由编辑或程序主席在不送外审的情况下直接拒掉稿件，通常针对篇幅超限、投稿数超限等违规情况。在许多机构和国家，发表在少数被认可顶级（&quot;A\*&quot;）会议上的论文直接与毕业要求、招聘、晋升乃至现金奖励挂钩，这就形成了把投稿数量而非质量最大化的强烈动机。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cvpr.thecvf.com/">2027 Conference</a></li>
<li><a href="https://en.wikipedia.org/wiki/Conference_on_Computer_Vision_and_Pattern_Recognition">Conference on Computer Vision and Pattern Recognition - Wikipedia</a></li>
<li><a href="https://www.aischolar.com/news/article/is-desk-rejection-common">Is Desk Rejection Common?</a></li>

</ul>
</details>

**标签**: `#academic publishing`, `#peer review`, `#ML conferences`, `#AI-generated research`, `#research incentives`

---

<a id="item-29"></a>
## [DeepSeek 独占 OpenRouter 270 亿亿日 tokens 的 53%，开源权重实验室合计突破 75%](https://www.reddit.com/r/LocalLLaMA/comments/1xnz8ct/deepseek_alone_accounted_for_53_of_all_27/) ⭐️ 6.0/10

r/LocalLLaMA 上的一篇帖子引用第三方追踪站点 dirac.run 的数据称，在单日约 27 万亿 tokens 的总量中，仅 DeepSeek 一家就占据了 OpenRouter 模型路由平台全部 tokens 的 53%。该帖子还称，开源权重实验室合计在该日的 token 份额已超过 75%。 如果数据准确，这说明通过 OpenRouter 路由请求的开发者正越来越多地选择开源权重模型而非闭源 API，这是关于实际采用情况而非基准测试成绩的重要信号。这种转变将给闭源模型厂商带来定价压力，并强化 DeepSeek 等实验室在开发者生态中的地位。 这些数字来自一个非官方第三方追踪站点的单日快照，帖子本身并未说明 tokens 如何归属到各实验室，也未说明路由与提供商回退机制会如何影响统计。此外，token 份额也反映价格与促销性路由等因素，而不仅仅是模型质量，因此不应将其直接视为能力高低的衡量标准。

reddit · r/LocalLLaMA · /u/Comfortable-Rock-498 · 11月4日 20:39

**背景**: OpenRouter 是一个托管式 API 路由平台，为开发者提供访问众多厂商数百个模型的统一接口，并负责提供商选择、故障回退和统一计费。开源权重模型是指训练好的参数被公开发布的模型，任何人都可以下载、自行部署或微调；DeepSeek 是一家总部位于杭州、由对冲基金 High-Flyer 资助的实验室，凭借 V3 和 R1 等发布成为这类模型最知名的发布者。Token 数量衡量的是模型实际处理的文本量，因此在 OpenRouter 这类平台上可作为使用量的粗略指标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/">OpenRouter</a></li>
<li><a href="https://en.wikipedia.org/wiki/Open_weights">Open weights - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek">DeepSeek - Wikipedia</a></li>

</ul>
</details>

**标签**: `#open-weights`, `#DeepSeek`, `#LLM market share`, `#OpenRouter`, `#AI industry trends`

---

<a id="item-30"></a>
## [有开发者称 LFM3-Omni-2B 借助 WebGPU 在 iPhone 上离线运行，速度约 80 tok/s](https://www.reddit.com/r/LocalLLaMA/comments/1xntou1/lfm3omni2b_running_fully_offline_on_my_iphone_18/) ⭐️ 6.0/10

Reddit 用户 /u/xenovatech 在 r/LocalLLaMA 发帖称，Liquid AI 的 20 亿参数 LFM3-Omni 模型可以在 iPhone 18 Pro Max 上完全离线运行，速度约为每秒 80 个 token，实现方式是在 React Native 应用中使用自定义的 WebGPU 计算内核。不过该帖本身只提供了一个标题和链接，并未附带代码、基准测试数据、量化方案或可复现的配置说明。 如果这一说法成立，就说明小型全模态模型可以完全依靠手机 GPU、通过 JavaScript/React Native 技术栈达到接近对话级的生成速度，而无需原生 Core ML 或 Metal 绑定，也不依赖云端。这对注重隐私的离线移动助手以及 WebGPU 作为可移植推理后端而言都是有价值的数据点；但由于没有公开任何可供复现的材料，目前只能把它视为尚未验证的个人说法，而非可复现的结果。 该帖没有说明量化格式、prefill 与解码吞吐的区分、上下文长度、显存占用、长时间运行时的降频情况，也没有说明约 80 tok/s 指的是纯文本还是完整的全模态（音频/视频）输入。另外需要注意，LFM3-Omni-2B 是 Liquid AI 的端到端全模态模型，可接受文本、图像、视频和音频并以语音作答，因此在音频与视觉编码器同时启用的情况下达到这一速度，要比纯文本解码困难得多。

reddit · r/LocalLLaMA · /u/xenovatech · 11月4日 17:08

**背景**: LFM3-Omni-2B 是 Liquid AI 在 LFM3 系列中推出的首个全模态模型：单一端到端模型即可理解文本、图像、视频和音频，并以文本和语音作答，体量小到可以在普通硬件上离线运行。WebGPU 是面向浏览器的 GPU 计算 API，目前已在各大主流引擎中提供，并越来越多地被用作本地 LLM 推理的可移植后端（例如 WebLLM/MLC），因为同一套内核可以同时面向桌面、Android 和 iOS 的 GPU。手机端的本地 LLM 推理通常采用量化后的 1B–7B 模型，在当前硬件上单流解码速度多在每秒几个到十几个 token 的量级，这正是「2B 模型约 80 tok/s」这一说法格外引人注目的原因。React Native 是一个跨平台的移动端 JavaScript 框架，用它来承载 GPU 推理内核属于少见但有意义的做法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/LiquidAI/LFM3-Omni-2B">LiquidAI/ LFM 3 - Omni - 2 B · Hugging Face</a></li>
<li><a href="https://pinggy.io/blog/run_llm_in_browser_webgpu/">Run an LLM Inside a Browser Tab: WebGPU and Local Inference in...</a></li>
<li><a href="https://www.runlocalai.co/stacks/iphone-on-device-ai">iPhone on - device AI stack (May 2026) — Llama... | RunLocalAI</a></li>

</ul>
</details>

**标签**: `#on-device AI`, `#WebGPU`, `#React Native`, `#LLM inference`, `#mobile`

---

<a id="item-31"></a>
## [遗失的 malloc\(\)：回顾早期 Unix 分配器接口](https://www.reddit.com/r/programming/comments/1xni70o/the_lost_malloc/) ⭐️ 6.0/10

Reddit r/programming 用户 /u/mttd 分享了一篇题为“the lost malloc\(\)”的博客文章，文章考察了一种历史悠久的 Unix malloc 实现：其接口除了大小参数外，还接受显式的内存区域映射（如 coremap、swapmap 和 anymap）。 这篇文章对系统程序员有价值，因为它解释了现代 malloc\(size\_t\) 为何去掉了显式内存区域参数，以及分配器 API 如何受到程序生命周期和内存管理假设的影响。 现代 malloc 只接受一个 size\_t 参数，返回适合基本类型对齐的未初始化存储；而历史接口要求调用者传入内存映射，文章将这种简化视为把更多策略移入分配器实现内部。

reddit · r/programming · /u/mttd · 11月4日 07:36

**背景**: malloc 是 C 库中用于动态内存分配的函数：它在运行时预留一块未初始化内存，返回指针，之后调用者用 free\(\) 释放。由于实现必须在速度、元数据开销和碎片化之间权衡，因此存在多种分配器设计。早期 Unix 系统通过 coremap、swapmap 等结构管理物理内存和交换内存，一些早期 malloc 变体直接在分配器 API 中暴露这些区域。该博客文章重建了这一遗失的接口，并解释后来的 malloc 实现如何把这些细节隐藏在更简单的仅含大小的调用之后。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://napcakes.nekoweb.org/posts/malloc/">the lost malloc () - gardenweb</a></li>
<li><a href="https://en.cppreference.com/c/memory/malloc">malloc - cppreference.com</a></li>

</ul>
</details>

**标签**: `#malloc`, `#memory allocation`, `#C`, `#systems programming`, `#reddit`

---