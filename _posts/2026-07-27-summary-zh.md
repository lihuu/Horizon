---
layout: default
title: "Horizon Summary: 2026-07-27 (ZH)"
date: 2026-07-27
lang: zh
---

> 从 39 条内容中筛选出 24 条重要资讯。

---

1. [GrapheneOS 锁定设备数据提取保护](#item-1) ⭐️ 8.0/10
2. [欧盟提议基于浏览器的隐私设置以消灭 Cookie 横幅](#item-2) ⭐️ 8.0/10
3. [LLM 代币中继黑市调查](#item-3) ⭐️ 8.0/10
4. [在树莓派 4 上使用 ARM64 汇编从零实现 YOLO26n 推理](#item-4) ⭐️ 8.0/10
5. [OpenAI 与 Anthropic 游说限制开源 AI 模型](#item-5) ⭐️ 8.0/10
6. [Kimi K3 开源权重模型在 HuggingFace 发布](#item-6) ⭐️ 8.0/10
7. [Minimax M3 与 MSA 支持已合并至 llama.cpp](#item-7) ⭐️ 8.0/10
8. [Decker：用 1 位图形复兴 HyperCard 的现代项目](#item-8) ⭐️ 7.0/10
9. [专注与跟进：AI 新时代的超能力](#item-9) ⭐️ 7.0/10
10. [将技术细节交给 AI 并非赋能](#item-10) ⭐️ 7.0/10
11. [Reddit 帖子暗示谷歌新 Gemma 模型即将发布](#item-11) ⭐️ 7.0/10
12. [MiniMax 发文支持开放权重](#item-12) ⭐️ 7.0/10
13. [基准测试显示 AI 编码工具质量相近，效率差异巨大](#item-13) ⭐️ 7.0/10
14. [Karpathy 疑似离开 Anthropic](#item-14) ⭐️ 7.0/10
15. [23 个 Gemma 4 E4B 模型对比：下载最多的性能最差](#item-15) ⭐️ 7.0/10
16. [极氪承诺减少锁车事件，此前车主被困海外](#item-16) ⭐️ 7.0/10
17. [用户称 Opus 5 审查以色列/巴勒斯坦话题，呼吁开源 AI](#item-17) ⭐️ 7.0/10
18. [反转版扫雷网页游戏颠覆谜题机制](#item-18) ⭐️ 6.0/10
19. [LTT 实验室将两块 Ryzen AI Halo 芯片组集群，效果不佳](#item-19) ⭐️ 6.0/10
20. [使用领域事件建模事实与反应](#item-20) ⭐️ 6.0/10
21. [Rivian R2 效率比特斯拉 Model Y 低 18-26%](#item-21) ⭐️ 6.0/10
22. [电动卡车司机 YT 将驾驶定制 eActros 600 开启环球之旅](#item-22) ⭐️ 6.0/10
23. [无脸 AI 账号实验揭穿被动收入神话](#item-23) ⭐️ 6.0/10
24. [男子因 ChatGPT 致命的医疗建议提起诉讼](#item-24) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [GrapheneOS 锁定设备数据提取保护](https://discuss.grapheneos.org/d/40700-grapheneos-protections-against-data-extraction-from-locked-devices) ⭐️ 8.0/10

GrapheneOS 论坛上的一场讨论强调了该操作系统对锁定设备数据提取的强大保护，包括自动重启和胁迫密码等功能，社区成员就这些功能的有效性和可用性展开了辩论。 这些保护对于面临设备扣押和被迫解锁威胁的记者、活动人士及注重隐私的用户至关重要，它们能够防止即使是有经验的黑客进行数据提取。 GrapheneOS 的 18 小时自动重启可将设备恢复到首次解锁前（BFU）模式，此时加密密钥不可访问；而胁迫密码则能静默擦除设备。社区还讨论了密码熵，指出图案锁仅提供约 18.57 比特的熵。

hackernews · Cider9986 · 7月26日 05:57 · [社区讨论](https://news.ycombinator.com/item?id=49055169)

**背景**: GrapheneOS 是一个注重安全的基于 Android 的操作系统。“首次解锁前”（BFU）状态是一种安全模式，此时设备加密密钥未加载到内存中，使得数据提取无法进行。自动重启和胁迫密码等功能通过限制在胁迫或长时间不活动情况下的数据暴露来增强保护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.androidauthority.com/grapheneos-duress-pin-3584795/">I use a duress PIN to protect my data — here’s how it works and why everyone needs one</a></li>
<li><a href="https://debugging.works/blog/grapheneos-auto-reboot-feature-for-linux/">GrapheneOS&#x27;s auto reboot feature for Linux laptops</a></li>
<li><a href="https://discuss.grapheneos.org/d/14722-using-duress-password-example">Using duress password example - GrapheneOS Discussion Forum</a></li>

</ul>
</details>

**社区讨论**: 社区普遍赞扬了 GrapheneOS 的保护措施，一位用户提到自动重启功能如何帮助记者保护信息来源。其他人讨论了需要完整的备份解决方案以便在过境前擦除设备，并辩论了密码熵——批评图案锁安全性低。一些人将之与苹果设备相比较，指出苹果也有类似功能且不受偏见。

**标签**: `#GrapheneOS`, `#mobile security`, `#data extraction`, `#locked device`, `#privacy`

---

<a id="item-2"></a>
## [欧盟提议基于浏览器的隐私设置以消灭 Cookie 横幅](https://killthecookiebanner.eu/) ⭐️ 8.0/10

欧盟委员会提出一项新法规，允许用户直接在浏览器中设置隐私偏好，从而消除每个网站上的 Cookie 横幅。 该提案可能最终结束网络上令人烦恼的 Cookie 横幅体验，同时为像 Global Privacy Control（GPC）这样的基于浏览器的隐私信号建立一个具有法律约束力的框架。 欧盟计划效仿现有的努力，例如加利福尼亚州的法律要求网站尊重用户启用的全球隐私控制信号，并建立在多个组织支持的 Global Privacy Control 规范之上。

hackernews · rapnie · 7月26日 11:53 · [社区讨论](https://news.ycombinator.com/item?id=49057175)

**背景**: Cookie 横幅是 GDPR 要求在放置非必要 Cookie 前获得知情同意的结果。之前的尝试如“请勿追踪”因缺乏法律执行而失败，但 Global Privacy Control（GPC）信号在 CCPA 下具有法律约束力。欧盟提案旨在将基于浏览器的信号标准化到整个欧洲。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Global_Privacy_Control">Global Privacy Control - Wikipedia</a></li>
<li><a href="https://globalprivacycontrol.org/">Global Privacy Control — Take Control Of Your Privacy</a></li>
<li><a href="https://secureprivacy.ai/blog/browser-signals-explained">Browser Signals Explained: Privacy, Consent &amp; Compliance</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍支持这一想法，但也批评其不够彻底——有人主张将所有非必要 Cookie 定为非法，而另一些人指出，干脆停止追踪会更简单。也有人赞扬加利福尼亚州更为果断的行动。

**标签**: `#privacy`, `#GDPR`, `#web standards`, `#browser`, `#regulation`

---

<a id="item-3"></a>
## [LLM 代币中继黑市调查](https://simonwillison.net/2026/Jul/26/relay-market/#atom-everything) ⭐️ 8.0/10

马特·伦哈德的调查揭示了一个以折扣价转售 LLM 代币的市场，其手段包括滥用免费试用、未受保护的支持机器人、盗刷信用卡等，主要在中国运作，使用开源代理软件如 one-api 和 new-api。 这种欺诈生态系统威胁 LLM 供应商的收入，并增加开发者暴露 API 端点的安全风险，可能阻碍公开 LLM 应用的推广。 转售者通过汇集来自免费试用或窃取凭证的 API 密钥提供大幅折扣，使用负载均衡代理如 one-api 和 new-api；买家寻求低价代币、绕过地理限制，或为模型蒸馏收集数据。

rss · Simon Willison · 7月26日 19:30

**背景**: LLM 代币是大型语言模型处理的文本单元，API 调用按 token 计费。代理软件 one-api 和 new-api 是合法的开源工具，用于管理多个 API 凭证，但被滥用来汇集被盗密钥并转售访问权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/songquanpeng/one-api">GitHub - songquanpeng/one-api: LLM API 管理 &amp; 分发系统，支持 Open... oneAPI: A New Era of Heterogeneous Computing - Intel APIARY oneAPI Programming Model One API download | SourceForge.net</a></li>
<li><a href="https://learn.microsoft.com/en-us/dotnet/ai/conceptual/understanding-tokens">Understanding tokens - .NET | Microsoft Learn</a></li>

</ul>
</details>

**社区讨论**: 评论者指出这并非新现象，将其比作广告和云计算积分的转售市场，并强调供应商定价低于市场出清价格时产生的套利机会。还有人探讨在代理型代币使用中防止订阅滥用的难度。

**标签**: `#AI`, `#security`, `#fraud`, `#LLM`, `#API`

---

<a id="item-4"></a>
## [在树莓派 4 上使用 ARM64 汇编从零实现 YOLO26n 推理](https://i.redd.it/wiyelkfpsifh1.jpeg) ⭐️ 8.0/10

一个学士项目仅使用 ARM64 汇编和 C 语言从零实现了 YOLO26n 推理，不依赖任何现有深度学习框架，并集成了 NEON SIMD、Winograd 卷积和算子融合等优化技术。 该项目展示了深度神经网络推理的底层理解，并为树莓派 4 等资源受限设备上的边缘 AI 提供了实用优化，可能激励 ARM 平台上高效推理的进一步研究。 实现包括自定义 ARM64 微内核、缓存感知分块以及自定义二进制格式的模型参数。尽管检测结果正确，但性能提升低于预期，作者寻求社区反馈。

reddit · r/MachineLearning · Forward\_Confusion902 · 7月26日 06:43 · [社区讨论](https://www.reddit.com/r/MachineLearning/comments/1v6w394/i_implemented_the_yolo26n_model_inference_from/)

**背景**: YOLO（You Only Look Once）是一种流行的实时目标检测系统。ARM64 是用于树莓派 4 等许多移动和嵌入式设备的 64 位 ARM 架构。NEON SIMD 是 ARM 的高级 SIMD 扩展，用于并行处理。Winograd 卷积是一种减少卷积所需乘法次数的算法，但以增加加法次数为代价。算子融合将多个操作合并为一个，以减少内存流量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2201.10369">[2201.10369] Winograd Convolution for Deep Neural Networks ... Winograd&#x27;s Convolution Theorem [Explained] - OpenGenus IQ Chapter 8: Fast Convolution - College of Science and Engineering The Winograd Convolution Method - DiVA Winograd Convolution for Deep Neural Networks: Efficient ... Winograd Convolution for Deep Neural Networks: Efficient ... Winograd Convolution: A Perspective from Fault Tolerance</a></li>
<li><a href="https://en.wikipedia.org/wiki/ARM_architecture_family">ARM architecture family - Wikipedia</a></li>
<li><a href="https://medium.com/@enerzai/optimium-101-3-optimium-utilized-operator-fusion-the-attack-was-super-effective-f2fc43d47d9b">Optimium 101 (3): Optimium utilized Operator Fusion ! | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者对项目表现出兴趣，其中一位询问基线、NEON 和 Winograd 之间的时间对比，以了解每项优化在树莓派 4 上的影响。

**标签**: `#ARM64`, `#Assembly`, `#YOLO`, `#Edge AI`, `#Optimization`

---

<a id="item-5"></a>
## [OpenAI 与 Anthropic 游说限制开源 AI 模型](https://www.nytimes.com/2026/07/25/technology/open-source-silicon-valley-china.html?unlocked_article_code=1.0lA.PyR-.7o3SR4ESvf3P&amp;smid=url-share) ⭐️ 8.0/10

据报道，OpenAI 和 Anthropic 正在游说华盛顿监管机构限制开源 AI 模型，尽管它们公开表示支持开源 AI。 这揭示了这些公司的私人利益与公开倡导之间的重大冲突，可能影响 AI 监管和开源开发的未来。 游说旨在限制开源模型，可能是为了保持竞争优势，而 Altman 等 CEO 公开声称支持开放性。

reddit · r/LocalLLaMA · pscoutou · 7月26日 13:53 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1v74j62/sources_openai_and_anthropic_quietly_lobby/)

**背景**: 开源 AI 模型允许任何人访问、修改和分发技术，促进创新但引发误用担忧。OpenAI 和 Anthropic 等公司建立了专有系统，同时也推广开源项目。这一消息凸显了商业利益与开源精神之间的紧张关系。

**社区讨论**: 社区评论表达了怀疑：一位用户暗示 Sam Altman 可能有欺骗行为，另一位则认为游说在意料之中。

**标签**: `#AI`, `#open-source`, `#regulation`, `#OpenAI`, `#Anthropic`

---

<a id="item-6"></a>
## [Kimi K3 开源权重模型在 HuggingFace 发布](https://huggingface.co/moonshotai/Kimi-K3) ⭐️ 8.0/10

Moonshot AI 于 2026 年 7 月 16 日在 HuggingFace 上发布了开源权重的 Kimi K3 模型，这是一个拥有 2.8 万亿参数、原生视觉能力和 100 万 token 上下文窗口的大型语言模型。 Kimi K3 是世界上首个开放权重的 3 万亿参数级模型，为编程、知识工作和推理方面的前沿智能设立了新标杆，其开源权重发布极大地推动了开源 AI 的发展。 该模型采用了 Kimi Delta Attention 和 Attention Residuals 技术，支持工具调用和群体智能，并通过 Kimi API 平台与 K2.7 Code 等其他模型一同提供。

reddit · r/LocalLLaMA · Unusual\_Guidance2095 · 7月26日 19:51 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1v7e5ck/kimi_k3_countdown_has_been_released/)

**背景**: Kimi 是由中国公司 Moonshot AI 开发的一系列大型语言模型，首个版本于 2023 年发布，支持 12.8 万 token 上下文。之前的 Kimi K2 于 2025 年 7 月开源。K3 在此基础上以更大的规模和改进的架构构建。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kimi_%28AI%29">Kimi (AI)</a></li>

</ul>
</details>

**社区讨论**: 社区反应非常热烈，称赞该模型的智能水平，称其为‘给世界的礼物’。用户对 GGUF 量化版本和新的推理提供商充满期待，但也有用户提醒早期量化版本可能存在缺陷。

**标签**: `#AI`, `#LLM`, `#open-source model`, `#HuggingFace`, `#Kimi`

---

<a id="item-7"></a>
## [Minimax M3 与 MSA 支持已合并至 llama.cpp](https://github.com/ggml-org/llama.cpp/pull/24908) ⭐️ 8.0/10

Minimax M3 模型及其 MiniMax 稀疏注意力（MSA）已通过拉取请求 \#24908 正式合并到 llama.cpp 项目中，从而支持本地推理这一开源前沿模型。 此次合并使得拥有 1M 上下文长度、原生多模态理解和前沿编码性能的 Minimax M3 模型可在消费级硬件上本地部署，极大地扩展了本地大语言模型生态系统的能力。 MSA 是一种专为超长上下文窗口设计的新型稀疏注意力架构。合并的拉取请求包含性能数据和量化支持，但用户报告称像 UD-IQ4\_XS 这样的 unsloth 量化需要 208 GB 存储空间。

reddit · r/LocalLLaMA · Time\_Reaper · 7月26日 17:54 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1v7ay5h/minimax_m3_support_with_msa_has_been_merged_into/)

**背景**: llama.cpp 是一个轻量级 C++ 实现，用于在 CPU 和 GPU 上高效运行大语言模型。Minimax M3 由 MiniMax 于 2026 年 6 月发布，是一个开源权重模型，结合了前沿编码和智能体性能，通过其专有的 MSA 机制支持 1M token 上下文窗口。该模型还原生支持图像和视频输入，能够操作桌面计算机。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-m3">MiniMax M3: Frontier Coding, 1M Context, Native Multimodality — All in One Model - MiniMax Research | MiniMax</a></li>
<li><a href="https://huggingface.co/MiniMaxAI/MiniMax-M3">MiniMaxAI/MiniMax-M3 · Hugging Face</a></li>

</ul>
</details>

**社区讨论**: 社区反应非常积极，用户表达了感谢。一些用户报告现有 unsloth 量化版本存在问题，并询问最佳量化选项以及不同硬件上的性能数据。

**标签**: `#llama.cpp`, `#local-llm`, `#model-support`, `#open-source`, `#inference`

---

<a id="item-8"></a>
## [Decker：用 1 位图形复兴 HyperCard 的现代项目](https://beyondloom.com/decker/) ⭐️ 7.0/10

Decker 是一个复兴 HyperCard 理念的新平台，提供 1 位图形和内置脚本语言的复古计算体验，已作为可下载应用发布。 Decker 重新点燃了对直观、易用的超媒体创作工具的兴趣，这种工具曾赋予非程序员强大的创作能力，有望激励新一代探索交互设计与个人计算的创造力。 Decker 采用仅限于黑白的 1 位图形，包含类似 HyperTalk 的脚本语言；可在现代系统上运行，面向复古计算爱好者。

hackernews · tosh · 7月26日 18:23 · [社区讨论](https://news.ycombinator.com/item?id=49060856)

**背景**: HyperCard 是苹果公司于 1987 年发布的先驱性超媒体工具，它将数据库与图形界面及 HyperTalk 编程语言相结合，使用户能轻松创建交互式堆栈。在 2004 年停售前，它被广泛用于快速应用开发和教育领域。Decker 从中汲取灵感，采用现代工具和 1 位图形美学，以唤起早期 Macintosh 的体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HyperCard">HyperCard</a></li>
<li><a href="https://en.wikipedia.org/wiki/Binary_image">Binary image - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者们表达了对 HyperCard 的怀旧之情，有人指出其革命性的易用性让孩子们和非程序员也能构建真正的应用。但也有人质疑 Decker 的现代相关性，认为如果没有现代图形和部署支持，它仍然只是一个怀旧小众项目，而非今天的实用工具。

**标签**: `#HyperCard`, `#retro computing`, `#visual programming`, `#interactive design`

---

<a id="item-9"></a>
## [专注与跟进：AI 新时代的超能力](https://www.rickmanelius.com/p/the-new-ai-superpowers-focus-and) ⭐️ 7.0/10

一篇文章探讨了随着 AI 加速软件开发，关键技能从技术熟练度转向专注与跟进，这提高了生产力，但也带来了重复造轮子和项目不完整的风险。 这一转变影响了软件开发者与团队，强调了在利用 AI 提速的同时管理认知负荷、避免倦怠的必要性。社区讨论了 AI 代理带来的生产力提升，以及构建不兼容的同类工具的陷阱。 文章引用了使用 AI 编码代理进行副业项目、修复配置问题的例子，而社区成员注意到“99%完成”项目的激增以及避免外部依赖的倾向。速度与重复发明之间的权衡是核心。

hackernews · mooreds · 7月26日 13:13 · [社区讨论](https://news.ycombinator.com/item?id=49057877)

**背景**: GPT-4 和编码代理等 AI 工具越来越被用于生成代码、修复错误和处理配置，减少了构建软件的时间。然而，这种便利可能导致开发者构建许多小型的重叠工具，而不是利用现有解决方案，并且项目可能因专注力下降而在完全完成前停滞。

**社区讨论**: 评论者分享了混合的体验：一些人报告称通过以固定周期使用 AI 代理，减少了倦怠感并增加了功能产出；其他人警告说 AI 鼓励每个人都构建自己版本的相同工具，导致不兼容和浪费精力。还有人担心许多项目达到 99%完成度却从未彻底完成。

**标签**: `#AI`, `#productivity`, `#software development`, `#focus`, `#followthrough`

---

<a id="item-10"></a>
## [将技术细节交给 AI 并非赋能](https://davidnicholaswilliams.com/its-not-empowering-to-hand-off-the-details/) ⭐️ 7.0/10

David Nicholas Williams 发表观点文章，认为将技术细节交给 AI 与普遍认知相反，实际上可能削弱开发者的能力。 这篇文章在软件工程社区引发激烈辩论，探讨 AI 委托对开发者自主性和生产力的真实影响，尤其在 AI 编程助手普及的背景下。 该文章在 Hacker News 上获得 7.0/10 分，166 个点赞和 91 条评论，显示出关于 AI 委托是否有益的强烈参与和多样化观点。

hackernews · davnicwil · 7月26日 17:58 · [社区讨论](https://news.ycombinator.com/item?id=49060592)

**背景**: Vibecoding 指使用 AI 助手生成代码而不深入理解。许多开发者越来越多地将技术细节委托给 AI 工具，认为这节省时间并赋能他们专注于更高层次的任务。

**社区讨论**: 评论者表达了不同观点：一些人同意 AI 委托可能导致疲劳和失控，另一些人则认为验证不需要完全理解，且如果管理者具备技术判断力，委托可以是赋能的。

**标签**: `#AI`, `#software engineering`, `#productivity`, `#programming`, `#delegation`

---

<a id="item-11"></a>
## [Reddit 帖子暗示谷歌新 Gemma 模型即将发布](https://i.redd.it/8htsr5smelfh1.jpeg) ⭐️ 7.0/10

知名研究员 hackerllama 在 Reddit 上发布了一个帖子（链接到 X 平台），引发了对谷歌 Gemma 开源模型家族可能发布新版本的猜测，可能包括一个 124B 参数且具备视觉能力的变体。 谷歌的 Gemma 模型是其 Gemini 模型的轻量级开源替代品，因此新版本的发布可能会影响开源 AI 格局，尤其是在提供更大规模或增加多模态能力方面具有竞争力时。 原帖是一个指向 X（原 Twitter）的链接，现已无法访问，但 Reddit 讨论暗示了一个 124B 模型以及带有视觉能力的“gpt-oss”后继者。该帖子获得了 627 分和 97%的赞率，hackerllama 积极在评论中互动。

reddit · r/LocalLLaMA · jacek2023 · 7月26日 15:29 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1v770ee/do_you_want_new_gemma/)

**背景**: 谷歌于 2024 年 2 月推出了 Gemma，这是一系列基于 Gemini 模型相同研究的开源大语言模型。初始版本包括 2B 和 7B 参数两种规模，旨在为开发者社区提供轻量级开放模型。新发布的 124B 参数模型将代表该系列的重大规模升级。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gemma_%28language_model%29">Gemma (language model) - Wikipedia</a></li>
<li><a href="https://deepmind.google/models/gemma/">Gemma — Google DeepMind</a></li>

</ul>
</details>

**社区讨论**: 最高赞评论者 ResidentPositive4122 对潜在的 124B 模型表示好奇，怀疑它是否令人失望或与较小的 Gemini 过于接近，并指出谷歌发布带视觉能力的 GPT-OSS 后继者将非常出色。另一个评论者说“Make no mistakes”，可能是赞同这种兴奋。Hackerllama 回复了大家的反馈。

**标签**: `#Gemma`, `#Google`, `#open-source models`, `#AI news`, `#large language models`

---

<a id="item-12"></a>
## [MiniMax 发文支持开放权重](https://xcancel.com/MiniMax_AI/status/2081167102753517574) ⭐️ 7.0/10

中国 AI 公司 MiniMax 在 X 平台发文支持开放权重、开放研究和开放创新，与开源 AI 运动立场一致。社区回应中提到 Hugging Face 的 Clement Delangue 原计划在旧金山组织一场支持开放权重的游行，但因许可证问题改为举办活动。 这表明企业对开放权重运动的支持日益增长，可能影响 AI 的可及性和透明度。作为中国主要 AI 公司，MiniMax 的立场为这场辩论增添了国际分量。 该推文专门回应了社区对开放权重的呼声，一条评论开玩笑地问“Hailuo 视频何时开放权重？”原计划的游行未获许可，因此改为举办替代活动。

reddit · r/LocalLLaMA · RhubarbSimilar1683 · 7月26日 18:28 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1v7bwg7/minimax_official_on_x_open_weights_open_research/)

**背景**: 开放权重模型公开已训练好的参数（权重），但通常不包含训练数据、代码或方法论，这与完全开源 AI 有所区别。MiniMax 是中国的“AI 六虎”之一，以多模态模型和 Hailuo 视频生成服务闻名。开放权重运动倡导提高 AI 透明度，但尚未达到完全开源的标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opensource.org/ai/open-weights">Open Weights : not quite what you’ve been told – Open Source Initiative</a></li>
<li><a href="https://en.wikipedia.org/wiki/MiniMax_Group">MiniMax Group</a></li>
<li><a href="https://www.microsoft.com/en-us/corporate-responsibility/topics/open-weight/">Open Weights and American AI Leadership</a></li>

</ul>
</details>

**社区讨论**: 评论总体积极，有用户幽默地提到“解放参数”，并戏谑 OpenAI 和 Anthropic（“你们所有的 AI 都归我们了！”）。也有人指出了组织游行的实际困难，最终改为活动形式。

**标签**: `#open-source`, `#AI`, `#open weights`, `#community`, `#MiniMax`

---

<a id="item-13"></a>
## [基准测试显示 AI 编码工具质量相近，效率差异巨大](https://i.redd.it/93nz4nc02gfh1.png) ⭐️ 7.0/10

一位开发者将 DeepSeek V4 Flash 分别通过 Claude Code、OpenCode 和 Pi 三个 AI 编码工具运行，发现输出质量几乎相同，但 Claude Code 耗时几乎是速度最快的工具的 4 倍，且消耗了更多的 token。 这一对比表明，工具或脚手架的选择会显著影响成本和速度，而不会影响代码质量，这对优化 AI 辅助工作流的开发者至关重要。 基准测试使用了在 vLLM 上以约 180 tok/s 运行的 DeepSeek V4 Flash，唯一变化的是工具。Claude Code 通过 CLIProxyAPI 路由到 DeepSeek，而 OpenCode 和 Pi 则采用了不同的工具调用结构。

reddit · r/LocalLLaMA · xquarx · 7月26日 19:17 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1v7d8px/harness_showdown_claude_code_vs_opencode_vs_pi/)

**背景**: AI 编码工具是基于终端的工具，为语言模型提供与代码库交互、管理工具调用和生成差异的框架。CLIProxyAPI 是一个开源网关，允许在原本为 Claude 设计的工具上使用 DeepSeek V4 等替代模型。DeepSeek V4 Flash 是一种高效的混合专家模型，总参数量 284B，激活参数 13B，支持 1M token 上下文窗口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/router-for-me/CLIProxyAPI">GitHub - router-for-me/CLIProxyAPI: Wrap Antigravity, ChatGPT Codex, Claude Code, Grok Build as an OpenAI/Gemini/Claude/Codex compatible API service, allowing you to enjoy the free Gemini 3.1 Pro, GPT 5.5, Grok 4.3, Claude model through API · GitHub</a></li>
<li><a href="https://github.com/earendil-works/pi">GitHub - earendil-works/pi: AI agent toolkit: unified LLM API, agent loop, TUI, coding agent CLI · GitHub</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek -ai/ DeepSeek - V 4 - Flash · Hugging Face</a></li>

</ul>
</details>

**社区讨论**: 一些评论者希望看到多维图表来展示速度、质量和成本之间的权衡。有用户推荐 Kimi Code CLI 作为更优选择。还有人询问人们为何使用终端工具而非集成开发环境的工具（如 Cline 或 Roo），表明对优势存在疑惑。

**标签**: `#AI coding harnesses`, `#DeepSeek V4`, `#benchmarking`, `#developer tools`

---

<a id="item-14"></a>
## [Karpathy 疑似离开 Anthropic](https://www.reddit.com/gallery/1v6pkji) ⭐️ 7.0/10

知名 AI 研究员、OpenAI 联合创始人 Andrej Karpathy 似乎已从其 X 个人资料中移除 Anthropic 相关信息，暗示他可能在加入仅数月后便离开了该公司。 若属实，这对 Anthropic 将是重大损失，尤其考虑到 Karpathy 对开源 AI 的倡导与 Anthropic 日益封闭的策略相悖。 这一动向尚属猜测，但时间点恰逢 Anthropic 愈发反对开放权重和开源 AI 模型，可能与 Karpathy 公开立场相冲突。

reddit · r/LocalLLaMA · ResearchCrafty1804 · 7月26日 01:12 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1v6pkji/karparthy_removed_anthropic_from_his_bio/)

**背景**: 开放权重 AI 模型指公开训练后权重的模型，用户可运行、微调并分发，但常附商业或分发限制。这与开源模型不同，后者通常有更宽松的许可并包含源代码。Anthropic 正转向更严格的模型发布政策，而 Karpathy 一直是开放性的公开支持者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/xigh/open-weight-models">GitHub - xigh/open-weight-models: Curated list of open-weight ...</a></li>
<li><a href="https://openai.com/open-models/">Open models by OpenAI</a></li>

</ul>
</details>

**社区讨论**: 社区评论对 Karpathy 可能离职表示理解，有用户称 Anthropic 工作文化严苛，资深研究员也疲于应对技术债务和超长工时。另有用户猜测签证限制或出口禁令是原因，还有人简言“这份工作可能不再有趣”。

**标签**: `#Andrej Karpathy`, `#Anthropic`, `#AI industry`, `#work culture`

---

<a id="item-15"></a>
## [23 个 Gemma 4 E4B 模型对比：下载最多的性能最差](https://www.reddit.com/r/LocalLLaMA/comments/1v73ux4/23_gemma4e4b_models_compared_with_abliterlitics/) ⭐️ 7.0/10

一项使用 abliterlitics 基准工具对 23 个 Gemma 4 E4B 模型的全面比较发现，下载量最高的无审查模型（obliteratus）在基准保留率上表现最差，退化程度最高。完整日志和张量比较结果已发布在 HuggingFace 和 abliterlitics 网站上。 这项比较通过揭示流行度不代表质量，帮助从业者为本地部署选择可靠模型。同时，它强调了系统性消融取证的重要性，以避免使用退化模型。 基准套件对 23 个模型（包括消融版、微调版和推理追踪模型）进行了基准保留率、KL 散度和权重级别 SVD 分析。下载量最高的模型（obliteratus）在保留率上得分最低，表明知识严重丢失。

reddit · r/LocalLLaMA · nathandreamfast · 7月26日 13:25

**背景**: Gemma 4 E4B 是 Google 开源的 44 亿参数多模态模型，专为高效本地部署设计。消融是指从 LLM 中移除安全对齐以减少拒绝回答，但可能会降低模型性能。Abliterlitics 是一个开源取证工具包，通过基准测试、KL 散度和 SVD 分析系统性地比较消融模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://abliterlitics.dev/">Abliterlitics: Open-Source Abliteration Forensics Toolkit</a></li>
<li><a href="https://huggingface.co/google/gemma-4-E4B">google/gemma-4-E4B · Hugging Face</a></li>
<li><a href="https://abliterlitics.dev/methodology/">Methodology | Abliterlitics</a></li>

</ul>
</details>

**社区讨论**: 评论指出，这些发现证实了对某些模型创作者（如 pliny 和 obliteratus）的偏见，而像&\#x27;obese\_coder&\#x27;这样的用户庆幸自己偏好的模型（TrevorJS）表现良好。另一位评论者质疑为何未测试 HauhauCS 的版本（下载量 52.7 万），暗示&\#x27;下载最多&\#x27;的说法可能具有误导性。

**标签**: `#Gemma 4`, `#LLM comparison`, `#abliterlitics`, `#uncensored models`, `#benchmarks`

---

<a id="item-16"></a>
## [极氪承诺减少锁车事件，此前车主被困海外](https://carnewschina.com/2026/07/26/zeekr-promises-less-lockouts-after-chinese-9x-owner-gets-stranded-abroad/) ⭐️ 7.0/10

极氪就一位中国 9X 车主在哈萨克斯坦被锁车超过 30 小时事件道歉，并承诺采取“用户控制、厂商保护”的新方案。 此事件凸显了软件定义汽车和地区限制的关键问题，可能削弱消费者信任并引发监管关注。 锁车是由于车辆离开中国网络（根据 GB/T 32960 标准）触发，导致智能驾驶、导航和储物箱解锁等功能受限。

reddit · r/electricvehicles · mightyopik · 7月26日 15:06 · [社区讨论](https://www.reddit.com/r/electricvehicles/comments/1v76enh/zeekr_promises_less_lockouts_after_chinese_9x/)

**背景**: 软件定义汽车依赖于云连接和区域合规性。如本例所示，当车辆跨越国境时，可能会丧失功能或锁住车主。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://carnewschina.com/2026/07/26/zeekr-promises-less-lockouts-after-chinese-9x-owner-gets-stranded-abroad/">Zeekr promises less lockouts after Chinese 9X owner gets ...</a></li>
<li><a href="https://finance.biggo.com/news/147d3813-dd8c-49cb-84bb-eae5fbe12550">Zeekr Responds to &quot;Overseas Lockout&quot; Controversy: Location ...</a></li>
<li><a href="https://en.tengrinews.kz/electromobiles/tourists-car-locked-itself-after-entering-kazakhstan-272473/">Zeekr 9X: problems at the Kazakhstan border - en.tengrinews.kz</a></li>

</ul>
</details>

**社区讨论**: 评论者就所有权问题展开辩论，有人认为防盗话术是公关手段。另有人指出，除了锁车，导航和 OTA 等功能在国外也会悄然停止工作。

**标签**: `#EV`, `#software-defined vehicles`, `#vehicle ownership`, `#Zeekr`, `#lockouts`

---

<a id="item-17"></a>
## [用户称 Opus 5 审查以色列/巴勒斯坦话题，呼吁开源 AI](https://www.reddit.com/r/artificial/comments/1v6ptgz/anthropics_opus_5_and_probably_more_recent_ai/) ⭐️ 7.0/10

一名 Reddit 用户声称，Anthropic 的 Claude Opus 5 模型在以色列/巴勒斯坦问题上拒绝表明立场，而之前的 Opus 4.x 则不同，并认为这证明了开源 AI 的必要性。 这一轶事报告突显了人们对专有模型中 AI 审查和地缘政治偏见的持续担忧，引发了关于透明度以及开源替代方案在 AI 开发中的重要性的辩论。 该用户发布了对比 Opus 4.x 和 Opus 5 回复的截图，显示新模型拒绝得出结论并表现出明显的偏见。Anthropic 于 2026 年 7 月 24 日发布了 Opus 5，将其定位为比 Fable 5 更便宜且限制更少的模型。

reddit · r/artificial · NinjaOne5173 · 7月26日 01:24

**背景**: AI 对齐是指引导 AI 系统符合人类价值观和目标。像 Anthropic 的 Claude 这样的专有模型通过对齐技术训练，这可能在敏感地缘政治话题上引入偏见或审查。批评者认为，开源模型允许公开审查和修改，可以减少这种隐藏的偏见。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/opus">Claude Opus \ Anthropic</a></li>
<li><a href="https://techcrunch.com/2026/07/24/anthropic-launches-opus-5/">Anthropic launches Opus 5 | TechCrunch</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_alignment">AI alignment</a></li>

</ul>
</details>

**社区讨论**: 评论大多同意存在审查，但对其程度有争议。一些人指出其他模型如 Grok 甚至更偏颇，而另一些人则指出像 DeepSeek 这样的开源模型也会审查话题（例如天安门广场事件），表明问题比模型开放性更广泛。

**标签**: `#AI censorship`, `#Anthropic`, `#open source`, `#AI alignment`, `#Israel-Palestine`

---

<a id="item-18"></a>
## [反转版扫雷网页游戏颠覆谜题机制](https://sunflowersgame.com/) ⭐️ 6.0/10

一款名为 Reverse Minesweeper（sunflowersgame.com）的新网页游戏颠覆了经典扫雷的规则，玩家需要放置向日葵而非躲避地雷，社区对其可解性和设计的评价褒贬不一。 该游戏试图刷新经典谜题格式，但其反响不一且缺乏明确的逻辑可解性限制了其影响力。它凸显了在成熟类型中设计真正新颖谜题的挑战。 该游戏可在 sunflowersgame.com 上玩，并设有难度选项。部分玩家反馈某些谜题缺乏足够的逻辑约束，可能需要猜测。开发者可能需要解决可解性和提示系统问题。

hackernews · pompomsheep · 7月26日 12:51 · [社区讨论](https://news.ycombinator.com/item?id=49057666)

**背景**: 扫雷是一款经典谜题游戏，玩家点击格子以显示数字提示周围地雷数量，目标是在不引爆地雷的情况下标记所有地雷。反转扫雷颠覆了这一前提：&\#x27;地雷&\#x27;（或花朵）是已知的，玩家必须推断出在哪里放置数字线索。这种变体在其他游戏（如 Itch.io 和 Roblox 上的 &\#x27;Minesweeper Reverse&\#x27;）中已有探索，但这个网页版使用了向日葵主题并自有特色。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m039.itch.io/minesweeper-reverse">Minesweeper Reverse by Dmitry Mozgin - Itch.io</a></li>
<li><a href="https://www.roblox.com/games/18325991183/Reverse-Minesweeper">Reverse Minesweeper | Play on Roblox</a></li>

</ul>
</details>

**社区讨论**: 社区反应褒贬不一。Ryukoposting 和家人觉得好玩；pillmillipedes 称赞 UI 和挑战性，但建议改进提示处理；hyperhello 质疑&quot;反转&quot;标签，认为只是换成了花朵的扫雷；ltsSmitty 报告因信息不足导致无解的谜题；greazy 喜欢该游戏并好奇线索是否是手工编制的。

**标签**: `#gaming`, `#puzzles`, `#web game`, `#minesweeper`

---

<a id="item-19"></a>
## [LTT 实验室将两块 Ryzen AI Halo 芯片组集群，效果不佳](https://www.lttlabs.com/articles/2026/07/24/amd-ryzen-ai-halo-cluster) ⭐️ 6.0/10

LTT 实验室尝试使用 AMD 的 RPC 集群方案将两块 Ryzen AI Halo 处理器组成集群，但推理性能不理想。 这一实验凸显了用消费级硬件构建经济高效 AI 集群的挑战，并表明 RPC 不适合低延迟推理；社区反馈指出 RDMA 是更优的选择。 该设置使用两块运行 Linux 的 Ryzen AI Halo 芯片通过网络连接，并依赖 AMD 的 RPC 集群方案，存在高延迟问题。评论者指出，像 NVIDIA DGX Spark 这样的生产集群使用 RDMA（例如 ConnectX-7 网卡）来实现低延迟。

reddit · r/LocalLLaMA · LabsLucas · 7月26日 16:09 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1v783ii/worlds_first_underwhelming_amd_ryzen_ai_halo/)

**背景**: 远程过程调用（RPC）是分布式计算的常见方法，但对 AI 推理来说，它会引入显著的开销，因为涉及 CPU 和操作系统。远程直接内存访问（RDMA）绕过操作系统和 CPU，实现内存到内存的直接传输，大幅降低延迟。将 AI 加速器组成集群可以运行比单个设备所能容纳的更大模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.amd.com/playbooks/clustering-rpc-server/">Clustering Two Ryzen™ AI Halos with RPC | AMD AI Playbooks</a></li>
<li><a href="https://en.wikipedia.org/wiki/Remote_direct_memory_access">Remote direct memory access - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍批评 RPC 方案，用户 Tyme4Trouble 表示&\#x27;RPC 很糟糕&\#x27;，并推荐使用 vLLM 通过 USB4 实现 RDMA。Potential-Leg-639 分享了一份 Strix Halo 上 RDMA 集群的指南，建议作者遵循该指南以节省时间。用户 1ncehost 为实验辩护，认为尽管不实用，但仍很有趣。

**标签**: `#AMD`, `#AI cluster`, `#Ryzen AI Halo`, `#LLM inference`, `#RPC vs RDMA`

---

<a id="item-20"></a>
## [使用领域事件建模事实与反应](https://deniskyashif.com/2026/07/25/modeling-facts-and-reactions-with-domain-events/) ⭐️ 6.0/10

文章提议使用领域事件将不可变的事实（如 OrderPlaced）与其后果（反应，例如发送通知或更新库存）分离开来。 这种分离有助于开发者构建更清晰、更易维护的事件驱动架构，避免副作用掩盖核心领域逻辑。 文章可能对比了领域事件与集成事件，强调反应应作为单独的关注点处理，而不是嵌入事件本身。

reddit · r/programming · deniskyashif · 7月26日 08:21 · [社区讨论](https://www.reddit.com/r/programming/comments/1v6xuqc/modeling_facts_and_reactions_with_domain_events/)

**背景**: 领域事件是领域驱动设计（DDD）中的一种战术模式，用于捕获有界上下文内有意义的事件。它们通过允许系统其他部分异步响应来实现松耦合。文章扩展了这一思想，主张严格区分事件（事实）和任何后续操作（反应）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Domain-driven_design">Domain-driven design</a></li>
<li><a href="https://learn.microsoft.com/en-us/dotnet/architecture/microservices/microservice-ddd-cqrs-patterns/domain-events-design-implementation">Domain events : Design and implementation - .NET | Microsoft Learn</a></li>

</ul>
</details>

**社区讨论**: 一位评论者认为，与其混合事件，团队应为每个部门创建单独的文档，因为代码是技术产物，无需对所有业务关注点进行建模。

**标签**: `#domain events`, `#domain-driven design`, `#software architecture`, `#event-driven architecture`

---

<a id="item-21"></a>
## [Rivian R2 效率比特斯拉 Model Y 低 18-26%](https://youtu.be/oT6Pd4udPZg?is=HvAFK8lc1PXP_sDL) ⭐️ 6.0/10

在效率测试中，Rivian R2 的效率比特斯拉 Model Y 低 18%至 26%，这归因于其方正外形和较高的离地间隙。 这一对比凸显了电动车型在越野能力和效率之间的空气动力学权衡，展现了特斯拉对低风阻设计的专注，而 Rivian 则在实用性和续航之间寻求平衡。 效率差距通过标准化测试测得；R2 更高的空气阻力显著增加了高速行驶时的能耗，而 Model Y 则得益于较低的风阻系数和迎风面积。

reddit · r/electricvehicles · PsychologicalBike · 7月26日 17:05 · [社区讨论](https://www.reddit.com/r/electricvehicles/comments/1v79n33/the_r2_is_18_to_26_less_efficient_than_the_model/)

**背景**: 空气阻力是影响电动汽车效率的主要因素，由风阻系数（Cd）和迎风面积决定。特斯拉的设计理念优先考虑低风阻系数以最大化续航，而 Rivian 的方正外形和较高离地间隙（旨在越野使用）则固有地增加了阻力。即便如此，考虑到其设计限制，R2 18-26%的效率差距被认为是适中的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://web.archive.org/web/20060903023114/http://www.cs.wmich.edu/~bhardin/cs106/AerodynamicDrag.htm">Aerodynamic Drag</a></li>
<li><a href="https://autozine.org/technical_school/aero/tech_aero.htm">AutoZine Technical School - Aerodynamics</a></li>

</ul>
</details>

**社区讨论**: 社区评论普遍认为，鉴于 R2 的方正设计，效率差异是意料之中的；有人甚至认为差距仅为 18-26%令人印象深刻。评论者指出，虽然特斯拉在效率上占优，但 R2 可能更适合需要越野能力或载物空间的生活方式需求。

**标签**: `#electric vehicles`, `#efficiency`, `#Rivian R2`, `#Tesla Model Y`, `#aerodynamics`

---

<a id="item-22"></a>
## [电动卡车司机 YT 将驾驶定制 eActros 600 开启环球之旅](https://www.youtube.com/watch?v=H4qTi3AOhWY) ⭐️ 6.0/10

YouTube 频道 Electric Trucker YT 将驾驶定制版梅赛德斯-奔驰 eActros 600 电动卡车于 2023 年 9 月中旬从汉诺威 IAA 车展出发，开启环球探险之旅。 这次环球之旅展示了电动长途卡车在全球范围内的可行性，通过实际行驶里程和充电能力，可能加速电动卡车的推广。 eActros 600 配备 621 kWh 电池，续航约 310 英里，支持最高 1000 kW 直流快充。定制卡车还携带了便携充电站，体现了充分的准备工作。

reddit · r/electricvehicles · ruralcricket · 7月26日 17:54 · [社区讨论](https://www.reddit.com/r/electricvehicles/comments/1v7ayop/electric_trucker_yt_to_start_world_tour/)

**背景**: 梅赛德斯-奔驰 eActros 600 是一款电池电动长途卡车，配备 800 伏电驱桥和两个电机。它旨在证明电动卡车可以取代柴油卡车进行长途运输，在使用可再生能源充电时，大约行驶 83,000 公里即可实现碳排放平衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://electronsx.com/ev-truck-model.php?EV=105">Mercedes-Benz eActros 600 electric long-haul truck | specifications | Electronsx</a></li>
<li><a href="https://www.daimlertruck.com/en/newsroom/pressrelease/mercedes-benz-trucks-celebrates-world-premiere-of-the-battery-electric-long-haul-truck-eactros-600-52428265">Mercedes-Benz Trucks celebrates world premiere of the battery electric long-haul truck eActros 600 | Daimler Truck</a></li>

</ul>
</details>

**社区讨论**: 评论中对这个项目表示兴奋，指出驾驶员准备充分，路线看起来安全。一条评论确认了 9 月中旬的出发日期以及在汉诺威 IAA 的亮相。

**标签**: `#electric trucks`, `#world tour`, `#Mercedes eActro`, `#EV demonstration`, `#sustainability`

---

<a id="item-23"></a>
## [无脸 AI 账号实验揭穿被动收入神话](https://www.reddit.com/r/artificial/comments/1v6ytlg/i_ran_a_faceless_ai_persona_account_for_six_weeks/) ⭐️ 6.0/10

一位用户进行了为期六周的实验，使用 APOB AI 的面部锁定功能、ElevenLabs 生成语音、CapCut 进行剪辑，创建了一个无脸 AI 人物账号，结果发现该过程需要大量人工投入，并非真正的被动收入。 该实验揭穿了流行的说法，即 AI 生成的无脸账号可以轻松产生被动收入，表明这仍然是带有 AI 中间件的劳动密集型零工工作。它为那些考虑在社交媒体上采用这种方式的人提供了现实检验。 ElevenLabs 免费层（每月 10,000 字符）和 CapCut 的免费层存在严重限制：语音配额在四天内耗尽，CapCut 免费层超时两次导致编辑会话丢失。APOB AI 免费层的水印虽小但清晰可见，且无法干净地裁剪掉。

reddit · r/artificial · Mental-Telephone3496 · 7月26日 09:16

**背景**: 无脸 AI 人物账号是指使用 AI 生成的面孔和声音发布内容的社交媒体账户，常被宣传为一种赚取被动收入的方式。该实验通过从头构建并运营这样一个账号六周，记录了所花费的每一小时，来检验这一说法。APOB AI、ElevenLabs 和 CapCut 等工具是此类工作流程中常用的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://besttooltips.com/apob-ai/">APOB AI: How to Create Viral AI Influencers Fast</a></li>
<li><a href="https://elevenlabs.io/text-to-speech-api">Text to Speech (TTS) API - ElevenLabs</a></li>
<li><a href="https://www.capcut.com/tools/online-video-editor">Free Online Video Editor: Create Videos Easily | CapCut</a></li>

</ul>
</details>

**社区讨论**: 社区评论大多持怀疑态度：一位用户指出帖子本身的文字看起来像 AI 写的，缺乏个性；另一位总结该实验是“为了赚钱制造无趣的 AI 垃圾，结果失败”；还有一位感谢作者做了这项工作，证实了这不值得去做。

**标签**: `#AI content generation`, `#social media`, `#passive income`, `#experiment`

---

<a id="item-24"></a>
## [男子因 ChatGPT 致命的医疗建议提起诉讼](https://www.bbc.com/news/videos/cx2dgyy5lg7o) ⭐️ 6.0/10

一名男子起诉 OpenAI，称 ChatGPT 提供的医疗建议几乎导致其死亡，突显依赖人工智能获取关键健康信息的危险。 这起诉讼可能为 AI 责任设定先例，并强调在医疗等高风险领域防范 AI 幻觉的迫切需求。 该事件涉及 ChatGPT 给出虚假医疗建议，男子采纳后陷入生命危险。此案引发对 AI 公司因其输出造成实际损害所应承担责任的质疑。

reddit · r/artificial · gamersecret2 · 7月26日 00:43 · [社区讨论](https://www.reddit.com/r/artificial/comments/1v6oyin/man_sues_chatgpt_for_nearfatal_medical_advice/)

**背景**: AI 幻觉是指大型语言模型（如 ChatGPT）生成虚假或误导性信息并当作事实呈现的现象。在医疗场景中，此类错误可能导致严重后果。检测和缓解幻觉仍是可靠部署 AI 的主要挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_hallucination">AI hallucination</a></li>

</ul>
</details>

**社区讨论**: 评论大多带有嘲讽意味：一名用户指出 ChatGPT 的免责声明，另一条开玩笑说应在提示中加入“不要犯错”，还有一条将其比作达尔文奖候选人。整体情绪倾向于用户本应更加谨慎，而非归咎于 AI。

**标签**: `#ChatGPT`, `#AI safety`, `#lawsuit`, `#medical advice`

---