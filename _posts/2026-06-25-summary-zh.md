---
layout: default
title: "Horizon Summary: 2026-06-25 (ZH)"
date: 2026-06-25
lang: zh
---

> 从 28 条内容中筛选出 19 条重要资讯。

---

1. [OpenAI 携手博通发布首款定制 AI 芯片 'Jalapeno'](#item-1) ⭐️ 9.0/10
2. [高通以 40 亿美元收购 AI 初创公司 Modular](#item-2) ⭐️ 9.0/10
3. [自对弈强化学习智能体登顶 Generals.io 排行榜](#item-3) ⭐️ 9.0/10
4. [NVIDIA 45°C 冷却方案大幅降低数据中心用水](#item-4) ⭐️ 8.0/10
5. [Nub：面向 Node.js 的类 Bun 一体化工具包](#item-5) ⭐️ 8.0/10
6. [Rust 社区推动 crates.io 与 GitHub 解耦](#item-6) ⭐️ 8.0/10
7. [LLM 生成的求职申请掩盖了候选人的真实自我](#item-7) ⭐️ 8.0/10
8. [HDD-RoPE：高维动态旋转位置编码](#item-8) ⭐️ 8.0/10
9. [DeepSWE：前沿编码智能体的新基准](#item-9) ⭐️ 8.0/10
10. [LLM 推理定价对比揭示缓存成本惊人差异](#item-10) ⭐️ 8.0/10
11. [RubyLLM：面向主要 AI 提供商的统一 Ruby 框架](#item-11) ⭐️ 7.0/10
12. [Bunny DNS 免费：无查询费，支持 500 个域名](#item-12) ⭐️ 7.0/10
13. [开源项目中的 PR 垃圾信息与早期邮件垃圾信息如出一辙](#item-13) ⭐️ 7.0/10
14. [卡马克反思 id Software 早期失误](#item-14) ⭐️ 7.0/10
15. [Papers with Code 推出精选 OCR 模型中心](#item-15) ⭐️ 7.0/10
16. [MuJoFil：面向视觉强化学习的开源 GPU 原生模拟器](#item-16) ⭐️ 7.0/10
17. [谷歌 Gemini 3.5 Flash 新增计算机使用功能](#item-17) ⭐️ 6.0/10
18. [Xteink X4 墨水屏阅读器评测：可破解但屏幕太小](#item-18) ⭐️ 6.0/10
19. [Simon Willison 将 MDN 浏览器兼容数据转为 SQLite 数据库](#item-19) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI 携手博通发布首款定制 AI 芯片 'Jalapeno'](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI 与博通共同发布了 Jalapeno，这是 OpenAI 首款定制 AI 推理芯片，由博通和台积电合作设计与制造，借助 OpenAI 自身模型加速，从设计到量产仅用九个月。 这标志着 OpenAI 减少对英伟达 GPU 依赖、优化自身模型推理性能与成本的重要战略举措，可能重塑 AI 硬件格局。 Jalapeno 是专用于推理而非训练的处理器，由台积电制造。OpenAI 基于对 LLM 原理的深刻理解从零设计芯片，博通负责芯片实现、板卡及机架系统集成。

hackernews · jamdesk · 6月24日 17:47 · [社区讨论](https://news.ycombinator.com/item?id=48663324)

**背景**: AI 芯片大致分为训练芯片（如英伟达 GPU）和推理芯片（如谷歌 TPU）。推理芯片针对高效运行已训练模型进行优化，常采用 ASIC 形式。OpenAI 此举追随谷歌长期的 TPU 策略，反映了 AI 公司为提升成本与性能而开发定制芯片的趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip</a></li>
<li><a href="https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/">OpenAI unveils its first custom chip, built by Broadcom</a></li>
<li><a href="https://investors.broadcom.com/news-releases/news-release-details/openai-and-broadcom-unveil-llm-optimized-intelligence-processor">OpenAI and Broadcom Unveil LLM-Optimized Intelligence ...</a></li>

</ul>
</details>

**社区讨论**: 评论者对 OpenAI 模型如何加速芯片设计表示好奇，部分人怀疑这可能是营销噱头。其他人讨论了专用推理芯片的技术优势，包括将权重固化到 ROM 以实现极高吞吐量的想法，并指出谷歌 TPU 的前瞻性。

**标签**: `#AI hardware`, `#OpenAI`, `#custom chip`, `#inference`, `#Broadcom`

---

<a id="item-2"></a>
## [高通以 40 亿美元收购 AI 初创公司 Modular](https://www.reuters.com/business/qualcomm-buy-ai-startup-modular-2026-06-24/) ⭐️ 9.0/10

高通于 2026 年 6 月 24 日宣布以 40 亿美元收购 AI 基础设施初创公司 Modular，该公司是 Mojo 编程语言的开发者。 此次收购标志着高通大举进军 AI 计算领域，可能挑战英伟达在高性能 AI 硬件和软件栈方面的主导地位。 Modular 的 Mojo 语言专为高性能 AI 基础设施和异构硬件设计，交易包括由 LLVM 和 Swift 创始人 Chris Lattner 领导的整个团队。

hackernews · timmyd · 6月24日 13:49 · [社区讨论](https://news.ycombinator.com/item?id=48659798)

**背景**: Modular 开发的 Mojo 是一种系统编程语言，结合了类似 Python 的语法和 C 级别的性能，适用于 AI 工作负载。高通传统上是移动芯片制造商，近年来通过收购 Tenstorrent 和 Ventana 等公司，正在向 AI 和 RISC-V 领域扩张。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Mojo_(programming_language)">Mojo (programming language)</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了复杂情绪：一些人质疑高通在高端 AI 领域与英伟达竞争的能力，而另一些人则认为这是构建全面 AI 产品组合的大胆战略举措。还有人对 Mojo 的发展方向表示怀疑，并指出 Modular 被一家硬件公司收购与其创始人此前对硬件公司的批评形成讽刺。

**标签**: `#acquisition`, `#AI`, `#hardware`, `#Qualcomm`, `#Modular`

---

<a id="item-3"></a>
## [自对弈强化学习智能体登顶 Generals.io 排行榜](https://www.reddit.com/r/MachineLearning/comments/1uei2yg/i_made_a_superhuman_generalsio_agent_with/) ⭐️ 9.0/10

一个使用 JAX 和 Vision Transformer 的自对弈强化学习智能体在 Generals.io 的人类 1v1 排行榜上达到第一名，超越了顶尖人类玩家。开发者开源了代码并发布了详细指南，介绍了整个流程。 这表明在非完全信息实时策略游戏中，扩展计算量和模型架构（Vision Transformer）可以超越人工设计的启发式规则。开源发布为构建类似游戏 AI 系统提供了宝贵参考。 智能体从 NumPy/Torch 重新实现为 JAX 以加速模拟，并将 CNN 替换为 Vision Transformer 以更好地捕捉空间依赖。项目包含一个基于 JAX 的快速游戏模拟器，可用于其他非完全信息 RTS 环境。

reddit · r/MachineLearning · /u/shrekofspeed · 6月24日 16:18

**背景**: Generals.io 是一款实时策略游戏，玩家在二维网格上控制军队夺取敌方将军，战争迷雾造成非完全信息。自对弈强化学习指智能体通过与自己对战进行训练，此前已在围棋、Dota 2 等游戏中达到超人类水平。JAX 是一个高性能数值计算库，支持高效的 GPU/TPU 加速；Vision Transformer（ViT）将 Transformer 架构应用于图像块以实现视觉理解。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://iogameslist.org/generals-io/">Generals.io - .io Games List - Play Online Free Games</a></li>
<li><a href="https://github.com/brunoleej/RL-with-JAX">GitHub - brunoleej/RL-with-JAX: Reinforcement Learning with ...</a></li>
<li><a href="https://pub.aimind.so/playing-pong-with-vision-transformer-dd8818b2ccba">Playing Pong With Vision Transformer | by Dohyeong Kim | AI Mind</a></li>

</ul>
</details>

**标签**: `#reinforcement learning`, `#self-play`, `#game AI`, `#JAX`, `#vision transformer`

---

<a id="item-4"></a>
## [NVIDIA 45°C 冷却方案大幅降低数据中心用水](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 8.0/10

NVIDIA 宣布了一种用于 AI 数据中心的新型液冷架构，其冷却液温度可达 45°C（113°F），通过消除蒸发冷却需求，实现了近乎零的用水量。 这一创新大幅降低了 AI 工厂（大量耗水设施）的环境影响，并开启了利用废热进行区域供暖的可能性，使数据中心成为社区资产。 该设计采用直接到芯片的液冷方式，冷却液温度高达 45°C，高于传统液冷系统通常低于 30°C 的运行温度。更高的温度允许在不蒸发水的情况下散热，在气候适宜的地区，系统甚至可以无需冷水机组运行。

hackernews · nitin_flanker · 6月24日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48660178)

**背景**: 传统数据中心依赖空气冷却或带冷水机组和冷却塔的液冷，通过蒸发散热消耗大量水。随着 AI 工作负载提高机架密度，液冷变得必不可少，但大多数现有系统仍需要水来冷却。NVIDIA 的方法将冷却液温度提高到废热可用于区域供暖的水平，这种协同作用虽已被探索但尚未广泛实施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.guru3d.com/story/nvidia-unveils-liquid-cooling-design-for-ai-data-centers/">NVIDIA Unveils 45 ° C Liquid Cooling Design for AI Data Centers</a></li>
<li><a href="https://www.techbuzz.ai/articles/nvidia-s-45-c-liquid-cooling-redefines-ai-data-center-energy">NVIDIA's 45 ° C Liquid Cooling Redefines AI Data Center Energy</a></li>
<li><a href="https://www.allthingsdistributed.com/2024/03/district-heating-using-data-centers-to-heat-communities.html">District heating: Using data centers to heat communities | All</a></li>

</ul>
</details>

**社区讨论**: 评论者对这一创新表示好奇，有人质疑为何之前没有使用更高的冷却液温度，并指出 NASA Ames 设施已经采用了温水冷却。其他人则强调了区域供暖的潜力，但也有人对气候依赖性以及不同气候下效率细节的缺乏表示担忧。

**标签**: `#data center cooling`, `#liquid cooling`, `#AI infrastructure`, `#energy efficiency`, `#sustainability`

---

<a id="item-5"></a>
## [Nub：面向 Node.js 的类 Bun 一体化工具包](https://github.com/nubjs/nub) ⭐️ 8.0/10

Colin McDonnell 发布了 Nub，这是一个一体化工具包，通过预加载钩子为 Node.js 添加转译、模块解析和 polyfill，在原生 Node 上运行，无需替换运行时。 Nub 将类似 Bun 的开发体验引入 Node.js，使开发者无需切换运行时即可使用 TypeScript 和现代 API，这可能惠及数百万 Node.js 开发者。 Nub 使用基于 oxc 的转译器（打包为 Node-API 插件），注册模块解析钩子，并为 Worker 和 Temporal 等 API 注入 polyfill。它完全是附加性的，不修改 Node 的引擎或标准库。

hackernews · colinmcd · 6月24日 14:14 · [社区讨论](https://news.ycombinator.com/item?id=48660267)

**背景**: Bun 是一个一体化 JavaScript 运行时，包含转译器、包管理器和测试运行器，但切换运行时可能带来破坏性。Node.js 的原生 TypeScript 支持尚处于实验阶段，且缺乏对新 API 的内置 polyfill。Nub 通过预加载钩子增强 Node.js，在不离开 Node 生态的前提下提供类似体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/oxc-project/oxc">GitHub - oxc-project/oxc: ⚓ A collection of high-performance</a></li>
<li><a href="https://nodejs.org/api/addons.html">C++ addons | Node.js v25.7.0 Documentation</a></li>
<li><a href="https://rodneylab.com/temporal-api-time-zones/">Temporal API Time Zones: Convert Times | Rodney Lab</a></li>

</ul>
</details>

**社区讨论**: 社区反应积极，有用户将整个 monorepo 迁移到 Nub 且零问题。部分讨论涉及技术细节，如 ESM 支持以及选择 --require 而非 --import 的原因；还有用户提到作者是 Zod 的创建者且曾在 Bun 工作。

**标签**: `#Node.js`, `#tooling`, `#TypeScript`, `#developer-experience`, `#open-source`

---

<a id="item-6"></a>
## [Rust 社区推动 crates.io 与 GitHub 解耦](https://infosec.exchange/@mttaggart/116806641273303255) ⭐️ 8.0/10

Rust 社区正在积极讨论并推动 crates.io 与 GitHub 解耦，相关 RFC 已合并，实现工作正在进行中。 这一变化消除了单点故障，降低了供应链风险，使 Rust 生态系统更具韧性，不再依赖 GitHub 的基础设施。 RFC（rust-lang/rfcs#3963）提议将 GitHub 账户重命名与 crates.io 用户名解耦，官方 crates.io 问题（rust-lang/crates.io#326）列出了路线图。

hackernews · speckx · 6月24日 19:40 · [社区讨论](https://news.ycombinator.com/item?id=48664733)

**背景**: 目前，crates.io 依赖 GitHub 进行身份验证和身份管理，这意味着 GitHub 的中断或政策变更可能影响 Rust 包的发布。Rust 项目主要由志愿者驱动，因此此类基础设施改造进展缓慢，依赖于资金和审查者的可用性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/rust-lang/rfcs/blob/master/text/3946-crates-io-username-identity.md">3946-crates-io-username-identity.md - GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区成员普遍认同解耦的必要性，但也承认其难度和资源限制。有人将其与 PHP 的 Packagist 等其他生态系统进行比较，后者强制基于源的打包，并强调应建设性地加固系统而非指责。

**标签**: `#Rust`, `#crates.io`, `#supply chain`, `#open source infrastructure`, `#GitHub`

---

<a id="item-7"></a>
## [LLM 生成的求职申请掩盖了候选人的真实自我](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 8.0/10

Tom MacWright 观察到，许多求职申请现在由 LLM 共同撰写，链接到 LLM 生成的作品集和 GitHub 项目，提交信息也是 AI 写的，这使得候选人变得难以区分且缺乏个性。 这一趋势削弱了招聘过程的真实性，使雇主更难评估候选人的真实技能和个性，并引发了关于在职业领域滥用 AI 的伦理担忧。 MacWright 指出，经过完善和生成的简历除了表明候选人使用了特定工具外，无法提供任何关于其本人的信息，实际上造成了“意外匿名”，候选人消失在 AI 生成的内容背后。

rss · Simon Willison · 6月24日 18:13

**背景**: 像 GPT-4 这样的 LLM 可以生成简历、求职信甚至代码。虽然它们提高了生产力，但在求职申请中的使用可能掩盖个人表达。MacWright 的评论凸显了 AI 时代对真实性的日益担忧。

**标签**: `#AI`, `#careers`, `#ethics`, `#hiring`, `#LLM`

---

<a id="item-8"></a>
## [HDD-RoPE：高维动态旋转位置编码](https://www.reddit.com/r/MachineLearning/comments/1uelcm9/high_dimensional_dynamic_rotary_positional/) ⭐️ 8.0/10

一种名为 HDD-RoPE（高维动态旋转位置编码）的新型位置编码方法被提出，它利用累积矩阵乘积实现多维、数据依赖的旋转。在 TinyStories 数据集上，其验证损失收敛速度比 xPos 更快。 这一进展可通过加速收敛来提高 Transformer 模型的效率，从而可能减少训练时间和计算成本。它还引入了一种更灵活的位置概念，可能捕捉段落或句子等层次结构。 HDD-RoPE 将查询和键向量分成任意大小的块（例如 4），而不是标准的 2，从而允许多个旋转轴。旋转速率是数据依赖的，意味着模型根据层激活学习如何推进位置。

reddit · r/MachineLearning · /u/mikayahlevi · 6月24日 18:16

**背景**: 旋转位置编码（RoPE）通过以固定速率旋转查询和键的维度对来编码相对位置。xPos 通过引入指数衰减因子扩展了 RoPE，以实现更好的外推。HDD-RoPE 通过使用累积矩阵乘积创建高维动态旋转，对 RoPE 进行了泛化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/mikayahlevi/hdd-rope/">GitHub - mikayahlevi/hdd-rope</a></li>
<li><a href="https://shreyashkar-ml.github.io/posts/rope/">A deep-dive into RoPE, and why it matters? | Shreyashkar Lal Sahu</a></li>
<li><a href="https://medium.com/@anitha6g/understanding-rotational-position-embeddings-rope-in-transformers-95d879dd7b4b">Understanding Rotational Position Embeddings (RoPE) in ...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论包括关于该方法计算开销以及与其他位置编码比较的技术问题。作者积极参与，承认 HDD-RoPE 比 xPos 或 RoPE 更慢，但强调了收敛优势。

**标签**: `#positional embedding`, `#transformer`, `#machine learning`, `#NLP`, `#RoPE`

---

<a id="item-9"></a>
## [DeepSWE：前沿编码智能体的新基准](https://www.reddit.com/r/MachineLearning/comments/1ue0hlp/deepswe_new_benchmark_looking_at_how_well_todays/) ⭐️ 8.0/10

DeepSWE 是一个新的开源基准测试，旨在评估前沿编码智能体在无污染、多样化且真实的软件工程任务上的表现，其任务从头编写并配有手工编写的验证器。 该基准解决了现有基准中的数据污染和缺乏真实世界复杂性等关键问题，为衡量 AI 编码智能体在实际软件工程工作中的表现提供了更可靠的指标。 DeepSWE 任务涵盖 5 种语言的 91 个仓库，所需代码量是 SWE-bench Pro 任务的 5.5 倍，并使用手工编写的验证器来测试软件行为而非实现细节。

reddit · r/MachineLearning · /u/we_are_mammals · 6月24日 02:03

**背景**: 现有的基准测试（如 SWE-bench）常存在数据污染问题，即模型可能在预训练期间见过解决方案，且任务多样性不足。DeepSWE 通过创建原创任务和使用多样化仓库来解决这些问题，从而更准确地评估编码智能体的真实能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://deepswe.datacurve.ai/">DeepSWE measures frontier coding agents on original, long-horizon...</a></li>
<li><a href="https://deepswe.lol/">DeepSWE — Long-Horizon Software Engineering Benchmark</a></li>
<li><a href="https://scale.com/leaderboard/swe_bench_pro_public">SWE-Bench Pro (Public Dataset)</a></li>

</ul>
</details>

**社区讨论**: 未提供 Reddit 社区讨论内容，但该帖子评分高且评论活跃，表明机器学习社区对此有浓厚兴趣且可能反响积极。

**标签**: `#benchmark`, `#code generation`, `#AI agents`, `#software engineering`, `#open-source`

---

<a id="item-10"></a>
## [LLM 推理定价对比揭示缓存成本惊人差异](https://www.reddit.com/r/MachineLearning/comments/1ueavxn/i_compiled_llm_inference_pricing_across_7/) ⭐️ 8.0/10

一位 Reddit 用户整理并比较了七家提供商（包括 OpenRouter、DeepSeek、Together AI、Fireworks 和 Groq）的 LLM 推理定价，发现缓存输入成本差异巨大——有时缓存命中比缓存未命中便宜数十倍。 这一对比凸显出，对于带有大型系统提示的智能体、RAG 流水线以及多轮对话等应用，缓存策略可能比标称的 token 价格更为重要，有望大幅节省成本。 该电子表格记录了输入/输出 token 定价、上下文窗口、缓存输入定价以及支持的模型，但不包括实际吞吐量、冷启动时间或量化细节。同一模型在不同提供商之间的成本可能相差数倍。

reddit · r/MachineLearning · /u/Technomadlyf · 6月24日 11:28

**背景**: LLM 推理缓存会存储中间结果（如 KV 缓存），以避免对重复提示进行重新计算，从而降低延迟和成本。各提供商提供不同的缓存策略和定价，这对于具有可复用上下文的应用程序的总成本影响巨大。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.aimactgrow.com/the-full-information-to-inference-caching-in-llms/">The Full Information to Inference Caching in LLMs –</a></li>
<li><a href="https://llm-d.ai/blog/kvcache-wins-you-can-see">KV-Cache Wins You Can See: From Prefix Caching in vLLM to</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-pro">DeepSeek V 4 Pro - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**标签**: `#LLM`, `#pricing`, `#caching`, `#inference`, `#providers`

---

<a id="item-11"></a>
## [RubyLLM：面向主要 AI 提供商的统一 Ruby 框架](https://rubyllm.com/) ⭐️ 7.0/10

RubyLLM 是一个新的开源 Ruby 框架，为多个主要 AI 提供商（包括 OpenAI、Anthropic、Google 和 xAI）提供统一接口，支持聊天、流式传输、图像生成和工具调用。 该框架简化了 Ruby 开发者的 AI 集成工作，减少了学习多个提供商 SDK 的需求，其活跃的社区表明对 Ruby 原生 AI 工具的需求强劲。 RubyLLM 将流式传输格式标准化为统一的 Chunk 对象，并维护已知模型注册表，但用户报告了与 xAI 等提供商的缓存问题以及可观测性工具化方面的困难。

hackernews · doener · 6月24日 14:41 · [社区讨论](https://news.ycombinator.com/item?id=48660711)

**背景**: Ruby 开发者历来缺乏 LLM API 的统一抽象层，通常需要为每个提供商使用单独的 SDK。RubyLLM 通过提供一个对 Rails 友好的 gem 来抽象提供商差异，类似于 Fog 抽象云存储提供商的方式，填补了这一空白。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rubyllm.com/overview/">Overview | RubyLLM</a></li>
<li><a href="https://rubyllm.com/streaming/">Stream Responses | RubyLLM</a></li>
<li><a href="https://mljourney.com/llm-response-caching-how-to-cut-costs-and-latency-in-production/">LLM Response Caching: How to Cut API Costs and Latency with ...</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞 RubyLLM 易于使用，将其与 Vercel 的 AI 框架相提并论，但也指出缓存不一致和缺乏原生响应 API 支持是痛点。一些用户还提到可观测性困难以及重试模式会删除底层模型的问题。

**标签**: `#Ruby`, `#AI`, `#framework`, `#LLM`, `#open-source`

---

<a id="item-12"></a>
## [Bunny DNS 免费：无查询费，支持 500 个域名](https://bunny.net/blog/were-making-bunny-dns-free/) ⭐️ 7.0/10

Bunny.net 宣布 Bunny DNS 现已免费，取消了所有 DNS 查询费用，并为每个账户提供最多 500 个域名的免费 DNS 托管，包括智能记录和健康监控等功能。 此举使 Bunny DNS 成为 Cloudflare DNS 服务的强大欧盟替代方案，可能吸引那些关注美欧地缘政治并寻求有竞争力的欧洲技术选项的用户。 免费层包括无查询限制、无按请求计费，且企业计划中不隐藏关键功能；但像 Diti 这样的用户担心其他 Bunny 产品会产生意外费用，因为计费上限仅适用于 Bunny CDN。

hackernews · dabinat · 6月24日 08:50 · [社区讨论](https://news.ycombinator.com/item?id=48657030)

**背景**: Bunny.net 是一个全球边缘平台，提供 CDN、安全和计算服务。DNS（域名系统）将域名转换为 IP 地址；权威 DNS 托管管理域名的 DNS 记录。Bunny DNS 运行在支持 IPv4 和 IPv6 的双栈任播网络上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bunny.net/dns/">Bunny DNS | The #1 Scriptable DNS Platform | bunny.net</a></li>
<li><a href="https://docs.bunny.net/dns">Bunny DNS - bunny.net Documentation</a></li>
<li><a href="https://bunny.net/">bunny.net - The Global Edge Platform that truly Hops</a></li>

</ul>
</details>

**社区讨论**: 社区情绪总体积极，用户称赞其作为欧盟替代方案和有机增长方式。但一些用户担心其他 Bunny 产品可能产生意外费用，因为计费上限仅适用于 Bunny CDN，而非其他服务。

**标签**: `#DNS`, `#cloud`, `#free-tier`, `#EU-tech`, `#networking`

---

<a id="item-13"></a>
## [开源项目中的 PR 垃圾信息与早期邮件垃圾信息如出一辙](https://www.greptile.com/blog/prs-on-openclaw) ⭐️ 7.0/10

Greptile 的一篇博客文章将开源项目中日益严重的垃圾拉取请求问题比作 21 世纪初的垃圾邮件泛滥，呼吁改进维护者工具和社区规范。 这种比较凸显了开源可持续性面临的系统性威胁，垃圾 PR 浪费维护者时间并降低信任，可能阻碍贡献并损害项目健康。 文章指出，与垃圾邮件不同，PR 垃圾信息针对的是个人维护者而非组织，使得基于声誉的过滤更加困难。GitHub 最近引入了可配置的 PR 限制来帮助缓解这一问题。

hackernews · dakshgupta · 6月24日 14:32 · [社区讨论](https://news.ycombinator.com/item?id=48660579)

**背景**: 拉取请求（PR）是在 GitHub 等平台上为开源项目做出贡献的核心机制。垃圾 PR 是低质量或自动化的提交，浪费维护者审查和拒绝它们的时间。21 世纪初垃圾邮件激增，催生了过滤器、声誉系统和 CAN-SPAM 等法律。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/SSWConsulting/SSW.Rules.Content/wiki/Handling-spam-Pull-Requests">Handling spam Pull Requests · SSWConsulting/SSW.Rules.Content</a></li>

</ul>
</details>

**社区讨论**: 评论者提出了解决方案，包括在合并第一个 PR 之前进行非文本验证、向项目捐赠代币，并指出 GitHub 的新 PR 限制是向前迈出的一步。一些人将其与依赖服务器声誉的垃圾邮件相类比，但这不适用于个人 PR。

**标签**: `#open-source`, `#spam`, `#maintainer-tools`, `#community`

---

<a id="item-14"></a>
## [卡马克反思 id Software 早期失误](https://twitter.com/ID_AA_Carmack/status/2069799283369345247) ⭐️ 7.0/10

约翰·卡马克在 Twitter 上发文反思他在 id Software 早期的失误，包括对团队施加过大压力以及未能随着公司成熟调整企业文化。 这位传奇游戏开发者的反思为职业倦怠和企业文化提供了宝贵教训，对整个游戏开发行业乃至更广泛的领域都具有重要意义。 卡马克特别提到，持续以创业强度要求员工会让他们精疲力竭，而成熟的公司需要更多的宽松空间。该帖子获得了 469 个点赞和 235 条评论，互动量很高。

hackernews · shadowtree · 6月24日 15:56 · [社区讨论](https://news.ycombinator.com/item?id=48661825)

**背景**: 约翰·卡马克是传奇程序员、id Software 联合创始人，以创作《毁灭战士》和《雷神之锤》等开创性游戏而闻名。id Software 早期以高强度工作文化和快速创新为特点，但也导致了职业倦怠和关键创意人才的流失。

**社区讨论**: 评论者普遍认同卡马克的自我批评，有人指出《雷神之锤》的开发耗尽了公司精力，但为了这款游戏的遗产是值得的。其他人则指出，在《毁灭战士 2》之后，id Software 失去了创意优势，技术成就超越了关卡设计。

**标签**: `#game development`, `#company culture`, `#burnout`, `#leadership`, `#id Software`

---

<a id="item-15"></a>
## [Papers with Code 推出精选 OCR 模型中心](https://www.reddit.com/r/MachineLearning/comments/1ueiam6/find_the_best_opensource_ocr_models_in_one_place/) ⭐️ 7.0/10

Papers with Code 上发布了一个精选页面，列出了带有基准测试的顶级开源 OCR 模型，其中包括百度（采用 R-SWA 的 Unlimited OCR）和 Mistral（OCR 4 API）的最新发布。 该资源帮助 AI 从业者快速找到最适合文档数字化的 OCR 模型，这对于实现代理式 RAG 和其他需要将杂乱 PDF 转换为机器可读 Markdown 的 AI 代理工作流至关重要。 该页面重点介绍了 OlmOCRBench 和 OmniDocBench 等基准测试，并推荐了 Chandra OCR 2（开源，可自托管）和 Mistral OCR v4（API）。百度的 Unlimited OCR 引入了参考滑动窗口注意力（R-SWA）以实现高效的长序列解码。

reddit · r/MachineLearning · /u/NielsRogge · 6月24日 16:26

**背景**: 光学字符识别（OCR）将扫描文档和 PDF 转换为机器可读文本。代理式 RAG（检索增强生成）使用 AI 代理从公司数据中检索并生成答案，通常需要 OCR 来数字化文档。Papers with Code 是一个跟踪机器学习论文、代码和基准测试的平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.emergentmind.com/topics/reference-sliding-window-attention-r-swa">Reference Sliding Window Attention (R-SWA)</a></li>
<li><a href="https://sebastianraschka.com/llms-from-scratch/ch04/06_swa/">SWA Chapter 4 Guide | Sebastian Raschka, PhD</a></li>
<li><a href="https://arxiv.org/abs/2501.00321">[2501.00321] OCRBench v2: An Improved Benchmark for Evaluating</a></li>

</ul>
</details>

**标签**: `#OCR`, `#open-source`, `#benchmarks`, `#AI agents`, `#document digitization`

---

<a id="item-16"></a>
## [MuJoFil：面向视觉强化学习的开源 GPU 原生模拟器](https://www.reddit.com/r/MachineLearning/comments/1uemrch/mujoco_derived_simulator_for_high_fidelity_vision/) ⭐️ 7.0/10

一款名为 MuJoFil 的新型开源模拟器，结合了 Nvidia 的 Newton 物理引擎和 Google 的 Filament 渲染引擎，实现了高保真、GPU 加速的视觉强化学习训练。 MuJoFil 填补了 GPU 加速视觉强化学习模拟的空白，提供了 NVIDIA Isaac 等专有解决方案的开源替代方案，使高保真并行训练对研究人员和开发者更加可及。 MuJoFil 支持 PBR 纹理和多种环境格式（GLB、OpenUSD），可通过 pip 安装'mujofil'（CPU 版）和'mujofil-warp'（GPU CUDA 版）。该项目仍处于早期开发阶段，存在已知 bug。

reddit · r/MachineLearning · /u/MT1699 · 6月24日 19:07

**背景**: MuJoCo 是机器人学和强化学习中常用的物理模拟器，但其 CPU 依赖性限制了并行化。虽然 MJX 提供了 GPU 加速，但并未针对视觉流水线优化。Nvidia 的 Isaac 生态系统需要强大的 GPU 和许可证，降低了可访问性。MuJoFil 通过结合开源的 GPU 原生物理引擎（Newton）和渲染引擎（Filament）来解决这些限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/newton-physics">Newton Physics Engine | NVIDIA Developer</a></li>
<li><a href="https://github.com/google/filament">GitHub - google/filament: Filament is a real-time physically ...</a></li>
<li><a href="https://github.com/newton-physics/newton">GitHub - newton - physics / newton : An open-source, GPU-accelerated...</a></li>

</ul>
</details>

**标签**: `#reinforcement learning`, `#simulation`, `#GPU`, `#MuJoCo`, `#open-source`

---

<a id="item-17"></a>
## [谷歌 Gemini 3.5 Flash 新增计算机使用功能](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/) ⭐️ 6.0/10

谷歌宣布 Gemini 3.5 Flash 现已支持内置的计算机使用功能，使开发者能够构建可跨浏览器、移动和桌面环境进行观察、推理和采取行动的定制化智能体。 此举使 Gemini 能够与其他提供类似智能体能力的 AI 模型竞争，但社区反馈凸显了其可靠性问题以及与 OpenAI 的 Codex 和 Anthropic 的 Claude 等竞争对手之间的差距。 该计算机使用功能内置于 Gemini 3.5 Flash 中，使其能够与图形用户界面交互，但用户报告频繁出现错误、幻觉，甚至无法完成从 PDF 提取数据等简单任务。

hackernews · swolpers · 6月24日 17:21 · [社区讨论](https://news.ycombinator.com/item?id=48662999)

**背景**: 像 Gemini 这样的大型语言模型（LLM）越来越多地被用于智能体任务，即自主控制软件界面。然而，LLM 容易出现幻觉和错误，尤其是在执行多步骤操作时。谷歌的公告旨在将 Gemini 的实用性从文本生成扩展到实际自动化领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/">Introducing computer use in Gemini 3 . 5 Flash</a></li>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3 . 5 Flash — Google DeepMind</a></li>
<li><a href="https://9to5google.com/2026/06/24/gemini-chrome-select-screen/">Gemini in Chrome adds ‘Select from screen’ tool</a></li>

</ul>
</details>

**社区讨论**: 社区评论对 Gemini 的可靠性表示失望，用户报告模型会放弃任务或编造数据。其他人则指出缺乏 MCP 支持以及与 Codex 或 Claude Code 相当的编码工具，还有人质疑谷歌基准测试图的准确性。

**标签**: `#Gemini`, `#AI`, `#computer use`, `#Google`, `#LLM`

---

<a id="item-18"></a>
## [Xteink X4 墨水屏阅读器评测：可破解但屏幕太小](https://blog.omgmog.net/post/xteink-x4-e-ink-reader/) ⭐️ 6.0/10

一篇关于 Xteink X4 墨水屏阅读器的评测强调了其开放性和可破解性，但批评了其 4.3 英寸的小屏幕和缺乏背光。 这款设备表明，基于微控制器的电子阅读器可以功能齐全且开放，挑战了像 Kindle 这样的封闭生态系统，但其小尺寸限制了主流吸引力。 X4 采用 4.3 英寸墨水屏，重 74 克，支持 USB-C 充电和 MagSafe 吸附。它运行开放固件，并允许安装 CrossPoint 等自定义软件。

hackernews · felixdoerp · 6月24日 16:35 · [社区讨论](https://news.ycombinator.com/item?id=48662381)

**背景**: 像 Kindle 和 Kobo 这样的电子阅读器使用专有软件和封闭生态系统。基于 ESP32 等开源硬件的电子阅读器提供可破解性和定制化，但通常不够精致。Xteink X4 是一款面向爱好者的 niche 产品，他们更看重开放性而非便利性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.xteink.com/products/xteink-x4">Xteink X 4 Pocket eReader</a></li>
<li><a href="https://indianexpress.com/article/technology/gadgets/xteink-x4-ebook-reader-specs-features-price-10405563/">Meet Xteink X 4 , a tiny e - reader that magnetically... - The Indian Express</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍喜欢 X4 的便携性和可破解性，但许多人指出屏幕太小，阅读不舒适，尤其对年龄较大的用户。有人报告购买过程中存在信用卡安全问题。

**标签**: `#e-reader`, `#hardware`, `#open-source`, `#review`

---

<a id="item-19"></a>
## [Simon Willison 将 MDN 浏览器兼容数据转为 SQLite 数据库](https://simonwillison.net/2026/Jun/24/browser-compat-db/#atom-everything) ⭐️ 6.0/10

Simon Willison 将 MDN 的浏览器兼容数据转换为 SQLite 数据库，托管在 GitHub 上并开放 CORS 头，可通过 Datasette Lite 访问。构建过程使用 GitHub Actions 工作流，将数据库强制推送到一个孤立分支。 这使得浏览器兼容数据更易于查询和集成到工具中，降低了开发者检查跨浏览器功能支持的障碍。它展示了一种通过 GitHub CDN 分发支持 CORS 的 SQLite 数据库的实用模式。 生成的数据库约 66MB，使用 sqlite-utils 和 Claude Code for web (Opus 4.8) 生成的脚本构建。数据库存储在专用的 'db' 孤立分支上，以利用 GitHub 的 CORS 头实现直接下载。

rss · Simon Willison · 6月24日 23:59

**背景**: MDN Web Docs 维护着一个全面的浏览器兼容数据仓库 (mdn/browser-compat-data)，开发者用它来检查不同浏览器支持哪些 Web 功能。Mozilla 最近推出了 MDN 的 MCP 服务器，这启发了该项目。SQLite 是一个轻量级的基于文件的数据库引擎，Datasette Lite 是一个基于 Web 的工具，用于在浏览器中探索 SQLite 数据库。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/mdn/mcp">GitHub - mdn/mcp: MDN's prototype MCP server · GitHub</a></li>
<li><a href="https://sqlite-utils.datasette.io/">sqlite - utils</a></li>

</ul>
</details>

**标签**: `#browser-compat`, `#sqlite`, `#data-engineering`, `#developer-tools`

---