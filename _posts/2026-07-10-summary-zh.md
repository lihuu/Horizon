---
layout: default
title: "Horizon Summary: 2026-07-10 (ZH)"
date: 2026-07-10
lang: zh
---

> 从 36 条内容中筛选出 19 条重要资讯。

---

1. [OpenAI 发布 GPT-5.6，提供三种模型尺寸](#item-1) ⭐️ 9.0/10
2. [在 32GB 内存上通过 int4 量化和磁盘流式运行 GLM 5.2](#item-2) ⭐️ 8.0/10
3. [欧盟议会通过聊天控制 1.0 法律](#item-3) ⭐️ 8.0/10
4. [美国陆军后勤过于脆弱，无法应对大规模战争](#item-4) ⭐️ 8.0/10
5. [内部服务 TLS 证书的正确做法](#item-5) ⭐️ 8.0/10
6. [GLM 5.2 在记账方面接近人类准确度](#item-6) ⭐️ 8.0/10
7. [OpenAI 将 ChatGPT 与 Codex 合并为 'ChatGPT Work'](#item-7) ⭐️ 8.0/10
8. [谷歌为 Linux KVM 虚拟机逃逸漏洞支付 25 万美元](#item-8) ⭐️ 8.0/10
9. [Postgres 比我们承认的更加够用](#item-9) ⭐️ 8.0/10
10. [腾讯 Hy3 大语言模型引发 OpenRouter 讨论](#item-10) ⭐️ 7.0/10
11. [用 LLM 将 Postgres 用 Rust 重写，通过所有测试](#item-11) ⭐️ 7.0/10
12. [IERS 宣布 2026 年底不增加闰秒](#item-12) ⭐️ 7.0/10
13. [Meta 发布 Muse Spark 1.1 代理 AI 模型并开放 API](#item-13) ⭐️ 7.0/10
14. [中国戈壁太阳能电厂利用熔盐在夜间发电](#item-14) ⭐️ 7.0/10
15. [新泽西法案要求三种传感器，阻碍特斯拉纯视觉 Robotaxi](#item-15) ⭐️ 7.0/10
16. [开发者分享对 Bun 用 Rust 重写的看法](#item-16) ⭐️ 7.0/10
17. [AI 生成内容充斥社交媒体，尤其是 LinkedIn](#item-17) ⭐️ 6.0/10
18. [开发者弃用 GitHub 转向 Codeberg 和自托管替代方案](#item-18) ⭐️ 6.0/10
19. [在 PostgreSQL 中实现非分区列的剪枝](#item-19) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [OpenAI 发布 GPT-5.6，提供三种模型尺寸](https://openai.com/index/gpt-5-6/) ⭐️ 9.0/10

OpenAI 发布了 GPT-5.6 旗舰模型，提供 Luna、Terra 和 Sol 三种尺寸，起价为每百万输入 token 1 美元（Luna）。 GPT-5.6 在每任务成本上相比 Claude Opus 和 Fable 等竞品大幅降低，并在 ARC-AGI-3 基准测试上达到新高度，展现了更强的推理和自主能力。 模型尺寸包括 Luna（最小，每百万输入/输出 token 价格$1/$6）、Terra（$2.50/$15）和 Sol（$5/$30）。Sol 在 ARC-AGI-3 上达到 7.8%，是首个在 ARC-AGI-3 游戏中获胜的前沿模型。

hackernews · logickkk1 · 7月9日 17:04 · [社区讨论](https://news.ycombinator.com/item?id=48849066)

**背景**: ARC-AGI-3 是一个交互式推理基准测试，要求 AI 智能体探索新环境、推断目标并规划行动，旨在衡量类人智能。GPT-5.6 在该基准上的表现表明通用推理能力取得进展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arcprize.org/arc-agi/3">ARC-AGI-3</a></li>
<li><a href="https://arxiv.org/abs/2603.24621">[2603.24621] ARC-AGI-3: A New Challenge for Frontier Agentic Intelligence</a></li>
<li><a href="https://arcprize.org/competitions/2026/arc-agi-3">ARC Prize 2026 - ARC-AGI-3 Competition</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调 GPT-5.6 的 token 效率和成本优势，Sol 每任务成本 1.04 美元，而 Opus 4.8 为 1.80 美元，Fable 为 2.75 美元。开发者还注意到 OpenAI 指南中的语义提示，如意图理解改进。部分用户讨论 Claude Code 和 Codex 等编码助手的模型对比。

**标签**: `#AI`, `#GPT-5.6`, `#OpenAI`, `#Language Models`, `#Machine Learning`

---

<a id="item-2"></a>
## [在 32GB 内存上通过 int4 量化和磁盘流式运行 GLM 5.2](https://github.com/JustVugg/colibri) ⭐️ 8.0/10

作者成功地在配备 25GB 内存的 12 核笔记本上运行了 744B 参数的 MoE 模型 GLM 5.2，通过 int4 量化和从磁盘流式路由专家。引擎 Colibrì在冷启动时达到约 0.1 tokens/s。 这证明了巨大的 LLM 可以在没有 GPU 的消费级硬件上运行，为资源有限的用户实现了本地 AI 推理。它还展示了可应用于其他大型模型的创新缓存和流式技术。 该模型有 744B 参数，但每个 token 仅激活约 40B；密集部分（约 17B 参数）以 int4 格式驻留 RAM（约 9.9 GB），而 21,504 个路由专家从磁盘流式传输（约 370 GB），并配有 LRU 缓存。引擎是单个 C 文件，无运行时依赖。

hackernews · vforno · 7月9日 08:05 · [社区讨论](https://news.ycombinator.com/item?id=48842459)

**背景**: GLM 5.2 是一个混合专家（MoE）模型，总参数 744B，但每个 token 仅激活 40B。int4 量化将内存使用减半，同时保持质量。MoE 模型将 token 路由到专家子集，从而在可控计算下实现大容量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mindstudio.ai/blog/what-is-glm-5-2-open-weight-model">What Is GLM 5.2? The Open-Weight Model Beating GPT 5.5 on Design Benchmarks | MindStudio</a></li>
<li><a href="https://huggingface.co/docs/transformers/quantization/concept_guide">Quantization concepts · Hugging Face</a></li>
<li><a href="https://unsloth.ai/docs/models/glm-5.2">GLM-5.2 - How to Run Locally | Unsloth Documentation</a></li>

</ul>
</details>

**社区讨论**: 社区评论包括一位用户正在为 macOS 进行类似优化，使用 Unsloth 和 Metal；另一位质疑实际 token 速率（例如 0.05–0.1 tok/s vs 1 tok/s）；还有建议使用 mmap 和 Medusa。总体情绪积极且协作，分享了技术见解。

**标签**: `#LLM`, `#optimization`, `#local AI`, `#GLM`, `#quantization`

---

<a id="item-3"></a>
## [欧盟议会通过聊天控制 1.0 法律](https://www.patrick-breyer.de/en/eu-parliament-greenlights-chat-control-1-0-breyer-our-children-lose-out/) ⭐️ 8.0/10

2026 年 7 月 9 日，欧洲议会允许《聊天控制 1.0》成为法律，尽管大多数议员投票反对，该法律允许在 2028 年前无证扫描私人信息。 该法律使得大规模监控私人通信成为可能，威胁端到端加密和隐私权，并为欧盟的数字监控开创了危险先例。 该法律通过程序性伎俩得以通过：否决动议需要绝对多数（361 票），但只有 314 名议员反对，276 票赞成，17 票弃权，113 人缺席。

hackernews · rapnie · 7月9日 11:03 · [社区讨论](https://news.ycombinator.com/item?id=48843923)

**背景**: 《聊天控制 1.0》是一项临时性的欧盟法规，旨在通过科技公司自愿扫描来检测儿童性虐待材料。批评者认为，它实际上强制对所有私人信息进行大规模监控，并破坏端到端加密，侵犯基本隐私权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chat_Control_1.0">Chat Control 1.0</a></li>
<li><a href="https://www.reddit.com/r/europe/comments/1urnadd/european_parliament_greenlights_chat_control_10/">r/europe on Reddit: European Parliament greenlights Chat Control 1.0, will now become law. 276 In Favour, 314 Against, 17 Abstentians.</a></li>

</ul>
</details>

**社区讨论**: 社区评论强烈批评所使用的议会策略，称其为‘愚蠢的议会伎俩’和对民主的威胁，有人警告说欧盟正在走向极权主义。

**标签**: `#privacy`, `#surveillance`, `#EU legislation`, `#encryption`, `#civil liberties`

---

<a id="item-4"></a>
## [美国陆军后勤过于脆弱，无法应对大规模战争](https://mwi.westpoint.edu/the-glass-backbone-why-the-armys-logistics-will-break-in-the-next-war/) ⭐️ 8.0/10

现代战争研究所的一份详细分析指出，美国陆军基于准时制原则构建的后勤系统极其脆弱，在与同等对手的大规模冲突中很可能失败。 如果陆军后勤系统崩溃，前线部队可能耗尽弹药、燃料和食物，导致灾难性的作战失败。这一批评挑战了数十年来以牺牲韧性为代价追求成本效益的做法。 文章强调了“牙尾比”这一衡量作战部队与支持部队比例的概念，并指出现代后勤与脆弱的商业供应链类似。文章警告说，伊朗或中国等对手可能用远程精确打击瞄准后勤节点。

hackernews · baud147258 · 7月9日 13:24 · [社区讨论](https://news.ycombinator.com/item?id=48845442)

**背景**: 准时制后勤在需要时精确交付物资，降低库存成本，但几乎没有应对中断的缓冲。军方采用这种方法以提高和平时期的效率，但在补给线可能被切断的竞争环境中，这成为一个弱点。“牙尾比”是一个旧指标，常常导致对后勤投入不足。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://combataxis.com/just-in-time-logistics-in-warfare/">Enhancing Warfare Efficiency Through Just-in-Time Logistics ...</a></li>
<li><a href="https://www.forbes.com/sites/maryjohnstone-louis/2025/04/25/todays-most-crucial-leadership-skill-is-systems-thinking/">Today's Most Crucial Leadership Skill Is Systems Thinking - Forbes</a></li>

</ul>
</details>

**社区讨论**: 评论者大多同意这一分析，并与历史上对抗汉尼拔的费边战术等策略进行类比。一些人指出，伊朗和乌克兰展示了在现代战争中如何打击后勤，而另一些人则认为 SpaceX 的星舰等新技术可能革新补给输送。

**标签**: `#logistics`, `#military`, `#systems-thinking`, `#supply-chain`, `#strategy`

---

<a id="item-5"></a>
## [内部服务 TLS 证书的正确做法](https://tuxnet.dev/posts/tls-for-internal-services/) ⭐️ 8.0/10

一篇新指南解释了如何使用 split-horizon DNS 与 ACME 来管理内部服务的 TLS 证书，为运行内部 CA 提供了一种替代方案。 这解决了管理内部服务 TLS 的常见运维难题，降低了复杂性并减少了对内部证书颁发机构的依赖。社区的高度参与凸显了其与实践者的相关性。 该指南建议使用 DNS-01 ACME 挑战来避免 HTTP-01 的限制，并承认 split-horizon DNS 可能带来长期复杂性。社区评论主张使用 DNS-01 和 Let's Encrypt 而非内部 CA。

hackernews · mrl5 · 7月9日 14:57 · [社区讨论](https://news.ycombinator.com/item?id=48846995)

**背景**: Split-horizon DNS 是一种 DNS 技术，DNS 服务器根据查询来源返回不同记录，常用于向内部客户端提供内部 IP 地址，向外部客户端提供公网 IP。ACME DNS-01 挑战通过在域名的 DNS zone 中放置特定 TXT 记录来证明域名控制权，从而允许为无法通过 HTTP 访问的服务签发证书。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Split-horizon_DNS">Split-horizon DNS</a></li>
<li><a href="https://letsencrypt.org/docs/challenge-types/">Challenge Types - Let's Encrypt</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍倾向于使用 DNS-01 验证而非 split-horizon DNS 以避免复杂性，有人建议使用带内部 IP 的公网 DNS 记录并通过 VPN 访问。其他评论者对配置 HTTPS 客户端信任内部 CA 的难度表示不满，主张使用 Let's Encrypt 通配符证书。

**标签**: `#TLS`, `#certificates`, `#ACME`, `#DNS`, `#internal services`

---

<a id="item-6"></a>
## [GLM 5.2 在记账方面接近人类准确度](https://toot-books.pages.dev/blog/glm-5-2-vat-benchmark) ⭐️ 8.0/10

GLM 5.2 在增值税记账基准测试中达到了接近人类的准确率，正确录入超过 99%的交易且无错误。但该基准仅测试了真实记账员工作的一部分，缺少发票检索和处理不确定情况等任务。 这一里程碑表明，LLM 可以高可靠性地执行核心会计任务，可能减少人工工作量。但责任归属和工作范围限制意味着完全自动化的记账仍是一个未来目标，而非立即替代。 该模型在基准测试中达到了 99.2%的准确率，错误主要来自模糊的税务规则或缺少上下文。基准测试使用了预先准备的用户备注，简化了真实流程——在现实中，记账员必须查找并整理发票。

hackernews · adamkurkiewicz · 7月9日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=48850414)

**背景**: GLM-5.2 是由 Z.AI 开发的大型语言模型，专为长周期任务设计，支持 100 万 token 的上下文窗口。记账涉及将银行交易与发票匹配并应用税务规则；像 GLM 这样的 LLM 能够处理文本并进行推理，因此适合此类结构化任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://z.ai/blog/glm-5.2">GLM-5.2: Built for Long-Horizon Tasks - z.ai</a></li>
<li><a href="https://openlm.ai/glm-5.2/">GLM-5.2 - openlm.ai</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，该基准低估了更广泛的工作范围（例如查找发票、处理异常），并提出了如果 LLM 出错的责任归属问题。一些人对公司的透明度表示怀疑，并表示将继续使用人工会计。

**标签**: `#AI`, `#bookkeeping`, `#LLM`, `#automation`, `#accounting`

---

<a id="item-7"></a>
## [OpenAI 将 ChatGPT 与 Codex 合并为 'ChatGPT Work'](https://openai.com/index/chatgpt-for-your-most-ambitious-work/) ⭐️ 8.0/10

OpenAI 发布了 'ChatGPT Work'，这是一个统一的应用，将 ChatGPT 聊天机器人与 Codex 编码代理合并，导致用户困惑并对 UI 变化提出批评。 这一统一模糊了日常聊天与编码任务之间的界限，可能会疏远偏好独立体验的用户。这表明 OpenAI 正在向企业级功能推进，但以牺牲用户体验清晰度为代价。 独立的 Codex 应用被 ChatGPT Work 取代；旧版 ChatGPT 应用更名为 'ChatGPT Classic'，暗示最终将被停用。用户报告称，在 Work 和 Codex 模式之间切换时没有可见变化，而日常聊天功能被降级到一个小的弹出窗口中。

hackernews · Tiberium · 7月9日 17:03 · [社区讨论](https://news.ycombinator.com/item?id=48849059)

**背景**: ChatGPT 是 OpenAI 于 2022 年 11 月推出的对话式 AI 聊天机器人，用于通用文本生成。Codex 于 2025 年 5 月推出，是一个能够检查仓库、运行命令和完成编码任务的 AI 编码代理。新的 'ChatGPT Work' 应用旨在将这两个环境合并到一个界面中，但突然的统一导致用户对在不同任务中使用哪种模式感到困惑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI</a></li>
<li><a href="https://openai.com/index/introducing-codex/">Introducing Codex - OpenAI</a></li>

</ul>
</details>

**社区讨论**: 用户评论绝大多数持负面态度，许多人表达了对产品变化的困惑。主要抱怨包括缺乏专门的日常聊天界面、Work 和 Codex 模式之间的差异不明确，以及将旧应用重命名为 'ChatGPT Classic' 暗示其将被弃用。部分用户敦促 OpenAI 保留现有良好功能，转而构建新的周边产品。

**标签**: `#OpenAI`, `#ChatGPT`, `#UX`, `#product-launch`, `#AI-tools`

---

<a id="item-8"></a>
## [谷歌为 Linux KVM 虚拟机逃逸漏洞支付 25 万美元](https://www.reddit.com/r/programming/comments/1urt5ib/google_pays_250k_for_linux_vulnerability_allowing/) ⭐️ 8.0/10

谷歌通过其 kvmCTF 项目奖励 25 万美元，用于发现一个严重的 Linux 内核漏洞（CVE-2026-53359），该漏洞允许客户虚拟机逃逸沙箱并在宿主机上获得 root 权限。 该漏洞被称为“Januscape”，影响 Intel 和 AMD x86 系统上的 KVM，对多租户云环境和虚拟化基础设施构成严重威胁，单个恶意 VM 就可能危及整个宿主机。 该漏洞存在 16 年之久，允许客户 VM 损坏宿主内核的影子页状态，实现完全从客户机到宿主机的逃逸。谷歌 kvmCTF 项目为此类零日提交提供高达 25 万美元奖励。

reddit · r/programming · /u/CircumspectCapybara · 7月9日 15:13

**背景**: KVM（基于内核的虚拟机）是 Linux 内核模块，使内核能够充当虚拟机监控程序，托管多个虚拟机。VM 逃逸是指攻击者突破隔离的客户环境并在宿主机上执行代码。谷歌的 kvmCTF 是针对 KVM 漏洞的漏洞奖励计划，对完全宿主妥协给予更高奖励。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arstechnica.com/security/2026/07/high-severity-guest-vm-escape-is-1-of-2-linux-vulnerabilities-to-surface-this-week/">Google pays $250K for Linux vulnerability allowing guest VM ...</a></li>
<li><a href="https://threat-modeling.com/cve-2026-53359-januscape-linux-kvm-vm-escape-intel-amd/">CVE-2026-53359 'Januscape': 16-Year-Old Linux KVM Guest-to ...</a></li>
<li><a href="https://thehackernews.com/2026/07/16-year-old-linux-kvm-flaw-lets-guest.html">16-Year-Old Linux KVM Flaw Lets Guest VMs Escape to Host on ...</a></li>

</ul>
</details>

**标签**: `#security`, `#Linux kernel`, `#virtualization`, `#vulnerability`, `#bounty`

---

<a id="item-9"></a>
## [Postgres 比我们承认的更加够用](https://www.reddit.com/r/programming/comments/1us129c/postgres_is_enough_for_more_than_we_admit/) ⭐️ 8.0/10

一篇 Reddit 帖子及其关联网站 (postgresisenough.dev) 指出，许多团队过早地采用专门的数据库和服务，而 PostgreSQL 内置的队列、缓存、全文搜索和发布/订阅功能往往足以应对实际工作负载。 这一观点挑战了架构复杂化的趋势，表明团队可以利用 Postgres 的多功能性来降低运维开销，避免多个专用服务的成本和维护负担。 该帖子强调，Postgres 对于队列（例如使用 SKIP LOCKED）、缓存（使用物化视图或 UNLOGGED 表）和全文搜索（使用 tsvector 和 GIN 索引）足够好用，但承认对于极高吞吐量或特殊需求，仍可能需要专用服务。

reddit · r/programming · /u/danieltabrizian · 7月9日 19:52

**背景**: PostgreSQL 是一个功能强大的开源关系型数据库，包含全文搜索、用于发布/订阅的 LISTEN/NOTIFY 以及咨询锁等功能。许多团队默认添加 Redis 用于缓存、Elasticsearch 用于搜索、RabbitMQ 用于队列，即使 Postgres 内置功能足以处理负载。'Postgres 就够了'运动倡导更简单、'无聊'的基础设施，使其更易于调试和维护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://leontrolski.github.io/postgres-as-queue.html">leontrolski - postgres as queue</a></li>
<li><a href="https://www.martinheinz.dev/blog/105">You Don't Need a Dedicated Cache Service - PostgreSQL as a ...</a></li>
<li><a href="https://www.postgresql.org/docs/current/textsearch.html">PostgreSQL: Documentation: 18: Chapter 12. Full Text Search</a></li>

</ul>
</details>

**标签**: `#postgres`, `#database`, `#architecture`, `#simplicity`, `#infrastructure`

---

<a id="item-10"></a>
## [腾讯 Hy3 大语言模型引发 OpenRouter 讨论](https://hy.tencent.com/research/hy3) ⭐️ 7.0/10

腾讯发布了 Hy3，一个开源混合专家（MoE）语言模型，总参数 295B（活跃参数 21B），并推出了预览版。该模型登顶 OpenRouter 排名，并引发了与其定价相比 DeepSeek Flash V4 的讨论。 Hy3 展示了较小模型在能力上能够媲美更大模型，可能重塑 AI 推理的成本效率。它在 OpenRouter 上以有竞争力的价格提供，挑战了现有的提供商如 DeepSeek。 Hy3 在 OpenRouter 上的有效输入价格现在与 DeepSeek 托管的 DeepSeek Flash V4 相同，后者是一个 284B 参数 MoE 模型（13B 活跃参数）。Hy3 包含一个额外的 3.8B MTP 层用于推测解码。

hackernews · andai · 7月9日 15:27 · [社区讨论](https://news.ycombinator.com/item?id=48847552)

**背景**: 混合专家（MoE）模型每个 token 只激活一部分参数，从而在高效计算的同时拥有大总容量。腾讯的 Hy3 是开源的，并收集了 50 多个产品的反馈。OpenRouter 是一个聚合 AI 模型的平台，提供排名和定价比较。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/tencent/Hy3">tencent/Hy3 · Hugging Face</a></li>
<li><a href="https://openrouter.ai/rankings">LLM Rankings | OpenRouter</a></li>
<li><a href="https://api-docs.deepseek.com/news/news260424/">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>

</ul>
</details>

**社区讨论**: 评论者注意到 Hy3 在较小的活跃参数量下具有惊人的能力，一些人将其与 DeepSeek V4 Flash 甚至 V4 Pro 在基准测试中进行了有利比较。然而，其他人质疑其长期价值，因为定价与 DeepSeek Flash V4 持平，且免费套餐即将到期。

**标签**: `#AI model`, `#LLM`, `#Tencent`, `#pricing`, `#open-source`

---

<a id="item-11"></a>
## [用 LLM 将 Postgres 用 Rust 重写，通过所有测试](https://github.com/malisper/pgrust) ⭐️ 7.0/10

一个名为 pgrust 的项目使用大语言模型（LLM）将 PostgreSQL 用 Rust 重写，现已 100%通过 PostgreSQL 回归测试，该消息在 Hacker News 上引起热议。 这表明 LLM 可用于重新实现像数据库这样复杂的、有数十年历史的系统，可能加速创新并实现更安全的重写。但这也引发了关于代码质量、许可证以及超越回归测试的严格验证需求的问题。 该项目将许可证从 PostgreSQL 许可证改为 AGPL，代码由 LLM 生成，在一个月内产生了 7101 次提交，使得手动审查变得困难。作者表示正在开发包含更先进技术的新版本。

hackernews · SweetSoftPillow · 7月9日 06:18 · [社区讨论](https://news.ycombinator.com/item?id=48841676)

**背景**: PostgreSQL 是一个成熟的开源关系型数据库，拥有经过 30 多年发展的全面回归测试套件。用 Rust 这样的内存安全语言重写这样的系统可能会减少漏洞，但是一项巨大的工程。该项目利用 LLM 自动化翻译和代码生成，旨在生成一个干净的 Rust 实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/regress.html">PostgreSQL: Documentation: 18: Chapter 31. Regression Tests</a></li>
<li><a href="https://arxiv.org/abs/2508.00083">A Survey on Code Generation with LLM-based Agents</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人称赞这一技术成就，也有人要求进行像 Jepsen 这样的严格验证，并对许可证变更和缺乏可人工验证的提交历史表示担忧。作者回应称正在开发一个重新架构的新版本。

**标签**: `#Rust`, `#PostgreSQL`, `#database`, `#reimplementation`, `#LLM`

---

<a id="item-12"></a>
## [IERS 宣布 2026 年底不增加闰秒](https://datacenter.iers.org/data/latestVersion/bulletinC.txt) ⭐️ 7.0/10

国际地球自转和参考系统服务（IERS）宣布，2026 年 12 月底不会插入闰秒，自 2016 年 12 月上一次闰秒以来，这一无闰秒期得以延续。 这一决定影响依赖精确时间同步的系统，如金融交易、电信和 GPS。它也加剧了关于闰秒在日益数字化的世界中实用性的持续争论。 UTC-TAI 偏移保持在-37 秒，UTC-GPS 偏移保持在-18 秒，因为不需要闰秒调整。地球自转相对较快，减少了近期对闰秒的需求。

hackernews · ChrisArchitect · 7月9日 14:16 · [社区讨论](https://news.ycombinator.com/item?id=48846281)

**背景**: 闰秒是对协调世界时（UTC）进行的一秒调整，以使其接近基于地球自转的太阳时（UT1），而地球自转存在不规律性。自 1972 年以来，已增加了 27 个正闰秒，均在 6 月 30 日或 12 月 31 日。IERS 监测地球自转，并约提前六个月决定是否插入闰秒。地球自转的不可预测性使得闰秒难以预报，给对时间敏感的数字系统带来挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Leap_second">Leap second</a></li>
<li><a href="https://en.wikipedia.org/wiki/International_Earth_Rotation_Service">International Earth Rotation Service</a></li>

</ul>
</details>

**社区讨论**: 社区成员对地球自转不可预测性的原因表示好奇，并询问闰秒如何影响 UNIX 时间戳，特别是对于维护模式下的系统。一些人指出了 UTC、TAI 和 GPS 之间的恒定偏移，而其他人则对该公告的前言和计时成本发表了轻松评论。

**标签**: `#leap second`, `#timekeeping`, `#UTC`, `#UNIX timestamps`, `#systems`

---

<a id="item-13"></a>
## [Meta 发布 Muse Spark 1.1 代理 AI 模型并开放 API](https://ai.meta.com/blog/introducing-muse-spark-meta-model-api/) ⭐️ 7.0/10

Meta 发布了升级版代理 AI 模型 Muse Spark 1.1，并面向开发者开放了公共 API 预览。该模型定价为每百万输入 token 1.25 美元、每百万输出 token 4.5 美元，缓存输入仅需 0.15 美元。 此次发布使 Meta 在代理 AI 领域直接与 OpenAI 和 Anthropic 竞争，其定价具有竞争力，可能扰乱市场。开源权重和 API 访问鼓励社区广泛实验，但评估方法的争议对基准测试的完整性提出了质疑。 根据评估报告，Muse Spark 1.1 使用了仅限 bash 工具的代理测试框架，配备 6 个 CPU 核心和 8GB 内存，社区成员认为这违反了 Terminal-Bench 2.1 任务的资源限制。开发者 Simon Willison 通过 LLM 插件演示了集成，其定价被认为激进（每百万 token 1.25/4.5 美元）。

hackernews · ot · 7月9日 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48846184)

**背景**: 代理 AI 模型是能够通过使用工具并遵循目标导向指令自主执行多步骤任务的 AI 系统。Meta 于 2026 年 4 月首次推出 Muse Spark 作为其最强大的模型，1.1 版本新增了开发者 API 访问，允许第三方应用集成该模型以执行代码生成和终端自动化等任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.meta.com/blog/introducing-muse-spark-msl/">Introducing Muse Spark: Scaling Towards Personal ...</a></li>
<li><a href="https://www.reuters.com/business/meta-debuts-muse-spark-11-with-preview-open-developers-2026-07-09/">Meta debuts Muse Spark 1.1 model with preview open to ...</a></li>

</ul>
</details>

**社区讨论**: 社区反馈褒贬不一：一些用户称赞其低定价和竞争性能，而另一些则批评评估方法，指出基准测试设置偏离了标准约束。开发者 Simon Willison 分享了积极的集成体验，另有用户建议 Meta 可以通过将编码模型商品化来扮演‘破坏者’角色。

**标签**: `#AI`, `#Meta`, `#agentic model`, `#open-weight`, `#Hacker News discussion`

---

<a id="item-14"></a>
## [中国戈壁太阳能电厂利用熔盐在夜间发电](https://electrek.co/2026/07/09/china-hami-solar-molten-salt-storage/) ⭐️ 7.0/10

中国三峡集团在戈壁沙漠启动了全球最大的太阳能光伏-光热混合电站的商业试运行，该电站利用熔盐储热技术，在日落后可持续发电长达八小时，无需锂电池。 这展示了一种大规模替代电池储能的可行方案，可能减少对锂电池的依赖，实现太阳能的全天候供电。它可能加速全球类似混合电站在阳光充足地区的部署。 位于新疆的 1 吉瓦哈密项目将光伏板与光热发电（CSP）塔相结合，后者加热熔盐以储存热能，可长达八小时。该电站完全避免使用锂电池，而是依靠熔盐热能储存。

rss · Electrek · 7月9日 19:53

**背景**: 熔盐热能储存通过镜子聚焦阳光将盐加热至高温（通常约 500°C），之后热量可用于产生蒸汽驱动涡轮机。光热发电（CSP）厂长期使用这项技术，但将其与光伏结合成混合系统相对较新。这种混合方法可以在不依赖昂贵电池的情况下，实现经济、可调度的可再生能源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Molten_salt_energy_storage">Molten salt energy storage</a></li>
<li><a href="https://en.wikipedia.org/wiki/Concentrated_solar_power">Concentrated solar power - Wikipedia</a></li>

</ul>
</details>

**标签**: `#solar energy`, `#molten salt storage`, `#China`, `#renewable energy`, `#energy storage`

---

<a id="item-15"></a>
## [新泽西法案要求三种传感器，阻碍特斯拉纯视觉 Robotaxi](https://electrek.co/2026/07/09/new-jersey-bill-tesla-camera-robotaxi/) ⭐️ 7.0/10

新泽西州立法者提出法案 S1677，要求无人驾驶商用车辆必须配备摄像头外加两种额外传感器类型（雷达和激光雷达），这将有效阻止特斯拉纯视觉 Robotaxi 在该州运营。 该法案可能为其他州树立先例，重塑特斯拉纯视觉方案与 Waymo 等多传感器策略之间的竞争格局，并重新引发关于纯摄像头是否足以实现安全自动驾驶的辩论。 拟议法律要求任何商用无人驾驶车辆配备摄像头、雷达和激光雷达；特斯拉当前的 Hardware 4.0 和计划中的 Robotaxi 均未搭载激光雷达。埃隆·马斯克一直坚称激光雷达不必要，但许多专家持反对意见。

rss · Electrek · 7月9日 16:45

**背景**: 自动驾驶汽车通常使用摄像头、雷达和激光雷达的组合来感知环境。摄像头提供高分辨率彩色图像，但在恶劣天气和低光照下表现不佳；激光雷达提供精确的 3D 深度数据；雷达在低能见度下表现良好但细节不足。特斯拉一直追求“纯视觉”方法，仅依赖摄像头和神经网络，而 Waymo 等大多数公司采用多传感器融合。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Autopilot">Tesla Autopilot - Wikipedia</a></li>
<li><a href="https://insideevs.com/news/738204/tesla-pure-vision-camera-only/">Tesla Bet On 'Pure Vision' For Self-Driving. That's Why It's In Hot Water</a></li>

</ul>
</details>

**标签**: `#autonomous vehicles`, `#regulation`, `#Tesla`, `#Waymo`, `#sensor technology`

---

<a id="item-16"></a>
## [开发者分享对 Bun 用 Rust 重写的看法](https://www.reddit.com/r/programming/comments/1urmi6h/my_thoughts_on_the_bun_rust_rewrite/) ⭐️ 7.0/10

一位开发者在 Reddit 上发布了对 Bun JavaScript 运行时可能用 Rust 重写的个人看法，引发了编程社区的讨论。 如果 Bun 用 Rust 重写，可能会提高性能和可靠性，影响那些将 Bun 作为 Node.js 替代品以加快启动和执行的开发者。 原帖缺乏详细的技术分析，但讨论凸显了社区对 Bun 架构的兴趣。Bun 目前使用 JavaScriptCore 引擎，并用 Zig 编写，而非 Rust。

reddit · r/programming · /u/simon_o · 7月9日 10:36

**背景**: Bun 是一个快速的一体化 JavaScript 运行时、包管理器和测试运行器，旨在作为 Node.js 的替代品。它使用 Safari 的 JavaScriptCore 引擎而非 V8，以获得更好的启动性能。用 Rust 这样的系统编程语言重写此类工具可以带来内存安全和并发优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://bun.com/docs/runtime">Bun Runtime - Bun</a></li>

</ul>
</details>

**标签**: `#Bun`, `#Rust`, `#Rewrite`, `#JavaScript`, `#Performance`

---

<a id="item-17"></a>
## [AI 生成内容充斥社交媒体，尤其是 LinkedIn](https://www.pangram.com/blog/ai-in-your-feed) ⭐️ 6.0/10

一篇最近的博客文章指出，AI 生成的内容在社交媒体上越来越普遍，尤其是 LinkedIn，其真实性正在被侵蚀。 这一趋势很重要，因为它破坏了社交平台赖以生存的信任和真实性，可能导致用户流失并降低整体在线讨论质量。 该文章是观察性的而非突破性的，但获得了高达 170 分和 149 条评论的社区参与度，表明用户对此有强烈共鸣。

hackernews · mukmuk · 7月9日 15:50 · [社区讨论](https://news.ycombinator.com/item?id=48847940)

**背景**: 像 LinkedIn 这样的社交媒体平台长期以来一直是专业网络和思想领导力的场所。然而，AI 工具现在可以轻松生成帖子，导致大量缺乏个人声音和真实性的通用 AI 撰写内容涌入。

**社区讨论**: 评论者表达了复杂的感受：一些人认为 AI 写作侵蚀了个人声音和真实性，而另一些人指出 LinkedIn 一直存在脚本化或不真实的内容，AI 只是加速了这一趋势。一些用户还提到转向 RSS 订阅和博客以避开 AI 生成的噪音。

**标签**: `#AI`, `#social media`, `#LinkedIn`, `#content quality`, `#authenticity`

---

<a id="item-18"></a>
## [开发者弃用 GitHub 转向 Codeberg 和自托管替代方案](https://www.reddit.com/r/programming/comments/1urm3mh/why_developers_are_ditching_github_for_codeberg/) ⭐️ 6.0/10

越来越多的开发者正从 GitHub 转向非营利 Git 托管平台 Codeberg，或自行托管代码仓库，以获得更多控制权和隐私保护。 这一趋势反映了开发者对供应商锁定、隐私和集中化问题的日益担忧，可能改变开源项目选择协作平台的方式。 Codeberg 是一家德国非营利组织，使用 Forgejo（一款自托管 Git 服务），提供静态页面、CI/CD 和翻译工具；而自托管则让开发者完全掌控基础设施。

reddit · r/programming · /u/Successful_Bowl2564 · 7月9日 10:15

**背景**: GitHub 由微软拥有，是代码托管的主导平台，但部分开发者因隐私问题和社区治理需求而寻求替代方案。Codeberg 作为非营利组织，强调透明度和自由。自托管需要运行自己的服务器，需要技术专长但提供最大的控制权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Codeberg">Codeberg - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Self-hosting_(network)">Self-hosting (network) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#GitHub`, `#Codeberg`, `#self-hosting`, `#developer tools`, `#open source`

---

<a id="item-19"></a>
## [在 PostgreSQL 中实现非分区列的剪枝](https://www.reddit.com/r/programming/comments/1urmnow/how_to_achieve_pruning_when_querying_by/) ⭐️ 6.0/10

一篇 Reddit 帖子讨论了如何在 PostgreSQL 中通过非分区列查询时实现分区剪枝，例如使用约束排除或表达式索引。该帖子旨在帮助用户优化对分区表的查询，其中过滤条件不涉及分区键。 这很重要，因为它将分区剪枝的性能优势扩展到那些不过滤分区键的查询，从而可能改善许多实际场景中的查询性能。拥有大型分区表的 PostgreSQL 用户可以在不更改应用程序逻辑的情况下获得更快的查询响应。 这些技术可能包括为分区添加引用非分区列的 CHECK 约束，使查询规划器能够使用约束排除来跳过不相关的分区。然而，这种方法需要仔细维护，并且可能不如基于分区键的原生分区剪枝高效。

reddit · r/programming · /u/be_haki · 7月9日 10:44

**背景**: PostgreSQL 的分区剪枝会在过滤条件位于分区键上时自动消除不满足查询 WHERE 子句的分区。约束排除是一种类似的机制，可以基于 CHECK 约束跳过表或分区，但效率较低，常用于较旧的 PostgreSQL 版本或特定用例。理解两者有助于设计最优的分区策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.postgresql.org/docs/current/ddl-partitioning.html">PostgreSQL: Documentation: 18: 5.12. Table Partitioning</a></li>
<li><a href="https://www.enterprisedb.com/postgres-tutorials/partition-pruning-during-executionpartition-pruning-during-execution">Partition Pruning During ExecutionPartition Pruning During Execution | EDB</a></li>

</ul>
</details>

**标签**: `#PostgreSQL`, `#database optimization`, `#partitioning`

---