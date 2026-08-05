---
layout: default
title: "Horizon Summary: 2026-08-05 (ZH)"
date: 2026-08-05
lang: zh
---

> 从 57 条内容中筛选出 28 条重要资讯。

---

1. [LLM 0.32 发布：新增推理痕迹、服务端工具与 OpenAI Responses 支持](#item-1) ⭐️ 9.0/10
2. [DeepSeek V4 Flash 在单块 AMD MI300X 上每秒跑出 150+ Tokens](#item-2) ⭐️ 8.0/10
3. [感谢联邦快递：正规公司如何让用户更容易被骗](#item-3) ⭐️ 8.0/10
4. [Keyv 及相关包在活跃的 Shai-Hulud npm 供应链攻击中遭入侵](#item-4) ⭐️ 8.0/10
5. [Xbox 宕机致玩家无法玩已拥有的光盘游戏](#item-5) ⭐️ 8.0/10
6. [Waymo CEO：纯摄像头自动驾驶触及安全天花板](#item-6) ⭐️ 8.0/10
7. [用户用 16 块 GB10 集群以 20+ tps 运行完整版 Kimi K3](#item-7) ⭐️ 8.0/10
8. [llama.cpp 新 PR 将热门 MoE 专家缓存到 GPU，速度提升最高达 2 倍](#item-8) ⭐️ 8.0/10
9. [InclusionAI 开源 Ling-3.0-flash：127B MoE 含官方 FP8](#item-9) ⭐️ 8.0/10
10. [呼吁 Lua 社区停止支持旧版本](#item-10) ⭐️ 8.0/10
11. [Mistral 推出 Shieldstral：3B 开放权重多模态内容审核模型](#item-11) ⭐️ 7.0/10
12. [生成多样化肤色的简单算法与色彩空间](#item-12) ⭐️ 7.0/10
13. [Waymo 在达拉斯向所有人开放无人驾驶网约车服务](#item-13) ⭐️ 7.0/10
14. [Oxide Computer 完成 4.45 亿美元 D 轮融资](#item-14) ⭐️ 7.0/10
15. [MiniMax-H3 全模态模型移植 MLX，支持 Apple Silicon 本地运行](#item-15) ⭐️ 7.0/10
16. [Hugging Face CEO 称中国凭借开源模型与供应链领跑 AI 竞赛](#item-16) ⭐️ 7.0/10
17. [通义千问开放权重模型下周发布，含 Qwen3.8-27B](#item-17) ⭐️ 7.0/10
18. [SK 海力士与闪迪发布 HBF 标准，瞄准 3TB/s 带宽](#item-18) ⭐️ 7.0/10
19. [美国新 AI 指南豁免开放模型政府审查](#item-19) ⭐️ 7.0/10
20. [Liquid AI 2.6B 工具调用模型在手机上可达 30 tok/s](#item-20) ⭐️ 7.0/10
21. [美国 AI 让 5 万架乌克兰自杀式无人机自主追踪目标](#item-21) ⭐️ 7.0/10
22. [国际刑警组织：人工智能驱动非洲超半数网络犯罪，诈骗激增](#item-22) ⭐️ 6.0/10
23. [Revoy 混动串列挂车获 2700 万美元融资，加速柴油卡车电动化](#item-23) ⭐️ 6.0/10
24. [Steve Yegge 称 Opus 4.7 的“再来两件事”毛病毁了 Gas Town](#item-24) ⭐️ 6.0/10
25. [Gemma 4 在 500MB 上运行：惊人的压缩与存疑的实用性](#item-25) ⭐️ 6.0/10
26. [中国电动汽车出口热潮开始影响全球汽油需求](#item-26) ⭐️ 6.0/10
27. [苹果诉 OpenAI 窃取机密遭反转：前员工仍被苹果咨询](#item-27) ⭐️ 6.0/10
28. [Reddit 股价下跌，CEO 质疑 Google AI Overviews 价值](#item-28) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [LLM 0.32 发布：新增推理痕迹、服务端工具与 OpenAI Responses 支持](https://simonwillison.net/2026/Aug/4/new-release-of-llm/#atom-everything) ⭐️ 9.0/10

LLM 0.32 作为该项目自发布以来最重要的更新正式推出，新增了对推理痕迹向标准错误输出的显示、服务端提供商工具，以及对 OpenAI Responses API 的支持。该版本还引入了新的 GPT-5.6 模型系列，默认模型改为性价比高的 GPT-5.6 Luna，并新增了 &\#x27;llm openai endpoint&\#x27; 命令，可向任意兼容 OpenAI 的端点发起一次性提示。Anthropic、Gemini 和 OpenRouter 的插件更新也带来了 WebSearch、WebFetch、CodeExecution 和 AnthropicMCP 等功能。 此次发布实质性地升级了开发者广泛使用的命令行工具 LLM，让模型推理过程变得透明，并支持直接在 CLI 中调用服务端工具。对于任何使用 LLM 编写脚本或构建智能体工作流的人来说，这些变更意义重大：工具调用更简单，调试和日志能力也更强。 默认情况下，推理痕迹会显示在标准错误输出中，并可用 -R/--hide-reasoning 参数关闭，从而保证管道中标准输出的干净。新增的服务端工具包括 OpenAI 的 CodeInterpreter 和 WebSearch；llm-anthropic 插件新增了 WebSearch、WebFetch、CodeExecution 和 AnthropicMCP，后者可对远程 datasette-mcp 端点执行 MCP 调用。重新设计的 SQLite 日志采用内容寻址方式，而 &\#x27;llm openai endpoint&\#x27; 命令为了支持一次性端点测试则完全不记录日志。

rss · Simon Willison · 8月4日 23:58

**背景**: LLM 是 Simon Willison 开发的一个命令行工具，通过插件系统在多种大语言模型上运行提示词。推理痕迹是 GPT-5.6 等模型生成的逐步中间推理内容；将其显示到标准错误输出可以避免混入管道数据。服务端工具是由提供商而非本地执行的工具，例如 OpenAI 的代码解释器，它们由较新的 OpenAI Responses API 暴露；该 API 支持有状态交互和内置工具。本次更新使 LLM 能更好地利用这些新一代模型功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2502.12289">Evaluating Step-by-step Reasoning Traces: A Survey Reasoning Traces: Analysis &amp; Applications Evaluating Step-by-step Reasoning Traces: A Survey - ACL ... lambda/hermes-agent-reasoning-traces - Hugging Face Structured Reasoning Traces - emergentmind.com ReasonTrace — Chain-of-Thought Reasoning Visualizer</a></li>
<li><a href="https://developers.openai.com/api/reference/responses/overview">Responses Overview | OpenAI API Reference</a></li>

</ul>
</details>

**标签**: `#LLM`, `#release`, `#OpenAI`, `#CLI`, `#AI tools`

---

<a id="item-2"></a>
## [DeepSeek V4 Flash 在单块 AMD MI300X 上每秒跑出 150+ Tokens](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 8.0/10

一篇新帖子展示了如何在单块 AMD MI300X 加速器上运行 DeepSeek V4 Flash，在保留原始权重的情况下实现每秒超过 150 个 token 的速度，但上下文窗口缩减至 256k。该方案利用 MI300X 的 192GB HBM，装下了原生 MXFP4 量化的 MoE 模型。 这一演示降低了在本地运行大型 MoE 推理模型的硬件门槛，使单块高端 GPU 即可胜任，而无需多 GPU 服务器。它凸显了 AMD MI300X 大显存在推理场景中的优势，并可能推动 AMD 加速器在 LLM 服务中的更广泛应用。 该模型的 256 个 MoE expert 原生采用 MXFP4 量化，使其能够装入 MI300X 的 192GB HBM，但上下文窗口从原始的 1M 缩减至 256k。评论者还指出，MI300X 是 OAM 模块，而即将推出的 MI350P 是 PCIe 卡，显存为 144GB。

hackernews · zhoutong · 8月4日 10:00 · [社区讨论](https://news.ycombinator.com/item?id=49166386)

**背景**: DeepSeek V4 Flash 是一个 Mixture-of-Experts \(MoE\) 模型，设计目标是能在商用或消费级硬件上本地运行，但即使经过重度量化，其权重也可能超过 141GB。AMD Instinct MI300X 是 AMD 的旗舰 AI 加速器，配备 192GB HBM3，对标 Nvidia 的 H100/H200，通常以 8 卡整机而非单卡形式销售。MoE 模型使用多个专门的子网络（expert）和一个门控网络，将每个输入只路由给少数几个 expert，从而实现高效的规模化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html">AMD Instinct™ MI300X Accelerators</a></li>
<li><a href="https://github.com/ggml-org/llama.cpp/issues/22319">Model request: DeepSeek V4 Series · Issue #22319 · ggml-org/llama.cpp</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 MI300X 不单独出售，通常以 8 卡整机形式销售，价格约 25 万欧元，并建议 MI350P PCIe 卡作为更易获取的选择。有人质疑为何没有与先前工作 DwarfStar 进行对比，也有人赞赏将上下文从 1M 缩减到 256k 的折衷方案，并指出 Codex 也处于类似范围。

**标签**: `#DeepSeek`, `#AMD MI300X`, `#LLM inference`, `#quantization`, `#MoE`

---

<a id="item-3"></a>
## [感谢联邦快递：正规公司如何让用户更容易被骗](https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/) ⭐️ 8.0/10

在 2024 年的博文中，安全研究员 Troy Hunt 指出，联邦快递等正规公司使用不安全且令人困惑的沟通方式——例如由个别员工发送附带 PDF 的电子邮件——这使得用户习惯了网络钓鱼攻击所利用的行为。他强调，这些做法等于在“训练”用户信任本应警惕的消息。 这一点很重要，因为网络钓鱼仍然是最常见的攻击手段之一，而只有当正规发件人也遵守安全的邮件规范时，用户才能有效保护自己。当知名品牌的行为方式与钓鱼者相似时，就会削弱人们区分真实消息和恶意消息的能力，影响到从消费者到安全团队的每一个人。 这篇文章举例说明，正规的通知邮件往往缺乏 SPF、DKIM 和 DMARC 等标准身份验证标记，还可能引导客户点击短链接或联系模糊的“支持”地址。这使得用户几乎无法区分真正的联邦快递邮件与冒充的钓鱼邮件。

hackernews · stymaar · 8月4日 21:09 · [社区讨论](https://news.ycombinator.com/item?id=49175192)

**背景**: 网络钓鱼攻击的核心是诱骗人们信任虚假消息，而 SPF、DKIM 和 DMARC 等电子邮件身份验证标准正是为了帮助接收方确认消息确实来自所声称的发件人。然而，这些协议配置起来有一定难度，正规公司也不总是强制启用，因此他们的邮件仍可能看起来未经验证或像自动发送。邮件转发服务还可能破坏或削弱这些保护机制，使问题更加复杂。Troy Hunt 的文章认为，当可信品牌发出令人困惑、信任度低的通信时，它们会无意中训练用户接受真正的钓鱼攻击所利用的警示信号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DMARC">DMARC - Wikipedia</a></li>
<li><a href="https://www.csoonline.com/article/564563/mastering-email-security-with-dmarc-spf-and-dkim.html">What are DMARC, SPF and DKIM ? How to master email security with...</a></li>
<li><a href="https://cs.stanford.edu/~gakiwate/papers/eurosp23-forwarding.pdf">Forward Pass: On the Security Implications of Email ...</a></li>

</ul>
</details>

**社区讨论**: 评论区大多赞同 Hunt 的观点，并分享了各自遇到的正规机构行为看起来像诈骗的例子：Chase 的欺诈部门会主动来电核实身份、联邦快递用个别员工的邮箱发送带 PDF 附件的海关通知、Google 的存储空间通知使用了连技术用户都困惑的 c.gle 链接，以及某市警报牌照续费短信看起来像骗局。整体情绪是无奈和认同，认为这些做法非常普遍；还有人提到，为了联系上联邦快递的人工客服，不得不进行一番“提示工程”。

**标签**: `#security`, `#phishing`, `#social engineering`, `#cybersecurity`

---

<a id="item-4"></a>
## [Keyv 及相关包在活跃的 Shai-Hulud npm 供应链攻击中遭入侵](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 8.0/10

安全研究人员报告称，广泛使用的键值存储库 Keyv 及多个相关 npm 包在一个活跃的“Shai-Hulud”供应链攻击中遭到入侵。Aikido.dev 发布了紧急安全通告，强调该攻击仍在进行中，需要立即处理。 由于 Keyv 是 Node.js 生态中广泛使用的依赖包，该包被入侵可能导致恶意代码扩散到成千上万的下游应用。Shai-Hulud 攻击活动此前曾窃取云凭证，因此这是一起严重事件，也再次凸显了 npm 依赖链的脆弱性。 在之前的 Shai-Hulud 攻击波中，一个名为“atool”的单一攻击者账户在 22 分钟内批量投毒 317 个包、共 637 个版本，并窃取云凭证。社区报告显示，本次攻击利用了 pre-install 挂钩（hooks），且可能具有蠕虫式传播行为，给检测和清理带来了极大困难。

hackernews · cimi\_ · 8月4日 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49166874)

**背景**: npm 包可以通过 pre-install 和 post-install 钩子在安装时执行任意脚本，攻击者经常利用这一机制投放恶意代码。Shai-Hulud 是一个针对 npm 生态的知名供应链攻击活动，其早期攻击波通过伪造相似包名（typo-squatting）和恶意安装脚本投毒了数百个包。Keyv 是 Node.js 中一个简单且广泛使用的键值存储包，因此此次入侵受到高度关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://slowmist.medium.com/threat-intelligence-shai-hulud-supply-chain-poisoning-cloud-credential-theft-and-1b8a3a4edd12">Threat Intelligence | Shai - Hulud Supply Chain Poisoning... | Medium</a></li>
<li><a href="https://www.wiz.io/blog/shai-hulud-npm-supply-chain-attack">Shai - Hulud npm Supply Chain Attack | Wiz Blog</a></li>
<li><a href="https://www.npmjs.com/package/keyv">keyv - npm</a></li>

</ul>
</details>

**社区讨论**: 评论者对此表示担忧，但态度务实，并提出了多种防御工具和工作流建议。有人呼吁彻底取消 pre-install 钩子或对新钩子实施暂停，也有人建议使用 devcontainer 来隔离环境；还有用户认为 GitHub 应该主动拦截 Shai-Hulud 创建的用以导出数据的仓库。总体情绪承认此次攻击的严重性，并指出现有依赖体系很难清理级联式的连锁危害。

**标签**: `#supply chain security`, `#npm`, `#security`, `#malware`, `#open source`

---

<a id="item-5"></a>
## [Xbox 宕机致玩家无法玩已拥有的光盘游戏](https://birchtree.me/blog/xbox-goes-down-you-cant-play-games-you-own-on-disc/) ⭐️ 8.0/10

一次长达 16 小时的 Xbox 宕机让玩家无法启动自己拥有的光盘版游戏，因为主机进行 DRM 许可证验证需要联网。微软已承认该问题并承诺修复。 这次宕机表明，即使是实体光盘游戏也不再保证可游玩，因为现代主机将所有权与在线验证绑定。这加剧了业界关于 DRM 和玩家所有权被侵蚀的持续争论。 根据宕机报道，数字版和光盘版游戏均受影响，微软承诺修复。即使是实体光盘版也常常需要额外的网络下载或许可验证；一项分析发现，测试的实体游戏中有 34%需要额外下载。

hackernews · surprisetalk · 8月4日 12:01 · [社区讨论](https://news.ycombinator.com/item?id=49167448)

**背景**: 数字版权管理（DRM）利用技术限制受版权保护内容的访问或复制方式，在游戏中通常将软件与在线服务器或账户绑定。像 Xbox Series X 这样的现代主机需要一次性的联网设置，并定期验证许可证，因此即使是光盘也可能在宕机期间无法游玩。这反映出游戏行业向数字发行和始终在线要求的整体转变，削弱了传统意义上“拥有”一款游戏的概念。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_rights_management">Digital rights management - Wikipedia</a></li>
<li><a href="https://www.digitalcitizen.life/microsoft-promises-xbox-fix-after-16-hour-outage-blocked-digital-and-disc-games/">Microsoft Promises Xbox Fix After 16 Hour Outage Blocked Digital and...</a></li>
<li><a href="https://thegeek.games/2026/08/03/many-games-need-internet-to-download-even-if-theyre-physical-disc-releases/">Many Games Need Internet to Download, Even If They’re Physical...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对 DRM 和所有权丧失表示不满。有用户描述在 PC 上玩《光环：士官长合集》时被迫创建账号并遭遇登录墙；还有人回忆起旧主机支持离线、局域网和二手光盘游玩，并呼吁玩家应拥有保留、转售和存档已购游戏的权利。

**标签**: `#DRM`, `#Xbox`, `#digital ownership`, `#gaming`, `#outage`

---

<a id="item-6"></a>
## [Waymo CEO：纯摄像头自动驾驶触及安全天花板](https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/) ⭐️ 8.0/10

Waymo 联合首席执行官 Dmitri Dolgov 指出，仅靠摄像头的自动驾驶系统（如特斯拉的方案）无法实现完全自动驾驶，因为“弱感知”会让安全曲线过早趋于平缓。他虽然没有直接点名特斯拉，但这番话显然是对特斯拉纯摄像头路线的批评。 此事意义重大，因为 Waymo 是使用激光雷达的领先 Robotaxi 运营商，而特斯拉则完全押注摄像头。传感器方案之争是自动驾驶安全的核心，也是哪条技术路线能率先实现完全自动驾驶的关键，影响整个自动驾驶行业。 Dolgov 表示，如果目标只是接近人类驾驶水平，纯摄像头方案是合理的；但若要实现完全自动驾驶或超越人类的表现，“弱感知会让安全曲线过早趋于平缓”。这番话是在关于激光雷达与纯摄像头 Robotaxi 的更广泛讨论中提出的。

rss · Electrek · 8月4日 15:31

**背景**: 自动驾驶汽车依赖摄像头、雷达、激光雷达等传感器。特斯拉倡导的纯摄像头方案依靠神经网络解读视觉数据，而 Waymo 等公司则将摄像头与激光雷达、雷达结合，以获得更可靠的三维感知。激光雷达通过激光进行测距，在复杂环境下可能更加可靠。争论的核心在于，仅靠视觉是否能够达到完全自动驾驶所需的安全水平。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://electrek.co/2026/08/04/waymo-co-ceo-camera-only-self-driving-tesla/">Waymo CEO explains why Tesla’s camera-only self- driving ... | Electrek</a></li>
<li><a href="https://www.fiercesensors.com/sensors-fusion/lidar-robotaxi-debate-continues-updated-waymos-dolgov">The lidar robotaxi debate continues, updated by Waymo’s ...</a></li>
<li><a href="https://www.msn.com/en-us/technology/tech-companies/musk-called-lidar-a-fool-s-errand-waymo-s-ceo-says-good-luck-without-it/ar-AA29p5KZ">Musk called lidar a fool’s errand, Waymo’s CEO says ... - MSN</a></li>

</ul>
</details>

**标签**: `#autonomous driving`, `#Waymo`, `#Tesla`, `#sensor technology`, `#AI safety`

---

<a id="item-7"></a>
## [用户用 16 块 GB10 集群以 20+ tps 运行完整版 Kimi K3](https://i.redd.it/x4w1912fyehh1.jpeg) ⭐️ 8.0/10

一名 Reddit 用户报告称，在 16 节点 NVIDIA GB10 集群上成功运行了完整版 Kimi K3 模型，平均每秒生成超过 20 个 token，峰值达 38 tps，预填充达 750 tps。该用户计划在进一步测试后发布 vLLM 镜像和使用说明。 这一成果表明，前沿规模的开权重模型可以在多节点消费级硬件上运行，有望降低本地部署的成本门槛。社区的高度关注也反映出人们对超越云端 API 的实用大型模型推理方案有强烈兴趣。 基准测试使用了 llama-benchy 连贯语料库，这也是该用户集群上首次使用 dspark 运行完整版 Kimi K3。Kimi K3 是一个 2.8 万亿参数的混合专家模型，拥有 100 万 token 的上下文窗口和原生视觉能力。

reddit · r/LocalLLaMA · ciprianveg · 8月4日 19:56 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1vfl525/kimi_k3_full_model_running_on_16x_gb10_cluster_at/)

**背景**: Kimi K3 是月之暗面（Moonshot AI）的旗舰开放权重模型，于 2026 年 7 月发布，是全球首个开放的三万亿参数级别模型，基于 Kimi Delta Attention 构建。NVIDIA GB10 是 Grace Blackwell 超级芯片，为 Project DIGITS 桌面个人 AI 超级计算机提供动力。dspark 是 DeepSeek 开源的推理加速框架，利用投机解码（speculative decoding）提升 LLM 推理速度，帮助该集群以实用的速度运行如此大的模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kimi.com/blog/kimi-k3">Kimi K3 Tech Blog: Open Frontier Intelligence</a></li>
<li><a href="https://www.tomsguide.com/ai/nvidia-drops-new-personal-ai-supercomputer-digits-costs-usd3-000-and-is-out-in-may">Nvidia reveals Project DIGITS AI supercomputer... | Tom&#x27;s Guide</a></li>
<li><a href="https://www.emergentmind.com/topics/dspark">DSpark : Speculative Decoding</a></li>

</ul>
</details>

**社区讨论**: 评论者好奇硬件成本与回本周期，还有人开玩笑说，用树莓派驱动周围价值约 5 万美元硬件的仪表盘真是“绝了”。另一位用户批评 NVIDIA 的 GB10 设计“真是捡了芝麻丢西瓜”。总体情绪是眼前一亮，但对性价比和硬件局限性仍存疑虑。

**标签**: `#LocalLLM`, `#Inference`, `#Kimi K3`, `#vLLM`, `#Hardware`

---

<a id="item-8"></a>
## [llama.cpp 新 PR 将热门 MoE 专家缓存到 GPU，速度提升最高达 2 倍](https://www.reddit.com/r/LocalLLaMA/comments/1vfhns3/a_llamacpp_pr_caches_hot_moe_experts_on_the_gpu/) ⭐️ 8.0/10

llama.cpp 的一个拉取请求（\#26563）新增了一个热力图，跟踪哪些混合专家（MoE）专家被最频繁使用，并将这些“热门”专家缓存到 GPU 显存中，而冷专家继续留在 CPU 上。作者在 8GB 显存的 Qwen3.6-35B-A3B 模型上测得：Q2\_M 从 33.25 tok/s 提高到 56.0 tok/s，Q5\_K\_P 从 17.34 tok/s 提高到 35.93 tok/s，并启用了 autofit。 这项优化有望让更大的 MoE 模型在显存有限的消费级 GPU 上变得实用，此前全部回退到 CPU 推理是主要瓶颈。但由于部分模型出现减速，收益取决于模型是否高度集中于少数专家。 该 PR 仅支持 CUDA，只在单 token 解码期间生效，并且由于缓存了哪些专家不同，输出可能会略有变化。在 Qwen3.5-122B-A10B 和 Laguna-S-2.1 上的负结果显示，当专家复用率低时，额外开销会抵消收益；该 PR 尚未合并。

reddit · r/LocalLLaMA · BTA\_Labs · 8月4日 17:52

**背景**: 混合专家（MoE）模型包含许多专门的子网络（即专家），但每个 token 只会激活其中一小部分，从而在不按比例增加计算量的情况下扩大模型容量。在 llama.cpp 中，当 MoE 模型超过显存容量时，部分层或专家会被卸载到 CPU，频繁的 CPU-GPU 数据交换成为性能瓶颈。该 PR 引入了一个专家缓存，让频繁使用的专家常驻显存。Q2\_M 和 Q5\_K\_P 是 GGUF 量化方案，在体积、速度和输出质量之间做不同取舍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2507.11181">[2507.11181] Mixture of Experts in Large Language Models Mixture of Experts in Large Language Models - arXiv.org A Closer Look into Mixture-of-Experts in Large Language Models A Survey on Mixture of Experts in Large Language Models Mixture of Experts Explained - Hugging Face Mixture of Experts in Large Language Models - ADS A Closer Look into Mixture-of-Experts in Large Language Models</a></li>
<li><a href="https://deepwiki.com/ggml-org/llama.cpp/7.3-quantization-techniques">Quantization Techniques | ggml-org/llama.cpp | DeepWiki</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极但保持谨慎。有用户哀叹“NOOOOO Cuda only :\(”，另一位用户分享了 PR 直链；还有用户建议将此类缓存与不常用专家的磁盘流式加载结合，并优先支持 Vulkan，希望能在多 GPU 设备上无需费心内存即可运行原生精度模型。

**标签**: `#llama.cpp`, `#MoE`, `#GPU optimization`, `#local LLM`, `#inference performance`

---

<a id="item-9"></a>
## [InclusionAI 开源 Ling-3.0-flash：127B MoE 含官方 FP8](https://v.redd.it/we8sse65ldhh1) ⭐️ 8.0/10

InclusionAI 在 Hugging Face 上以 MIT 许可证发布了 Ling-3.0-flash 权重，BF16（约 255GB）和官方 FP8（约 128GB）两个仓库均已开放，无需申请即可下载。该稀疏 MoE 模型总参数量为 127.5B（1275 亿），激活参数为 5.1B（51 亿），采用 512 个专家、每 token 激活 8 个专家。 这是一次重要的开源权重发布：细粒度专家架构（512 个专家、每 token 激活 8 个）与官方 FP8 权重，使其在大型统一内存设备或多 GPU 机器上更具可运行性。MIT 许可证消除了商业使用的法律障碍，官方 FP8 相比 BF16 将存储和内存需求减半。 该模型采用 BailingMoeV3 架构，model\_type 为 bailing\_hybrid，并使用自定义代码，与 Ling-2.6-flash 同属一个系列。FP8 版本是官方量化而非社区转换；思考模式是聊天模板内的按请求开关，默认开启。

reddit · r/LocalLLaMA · derspenti · 8月4日 15:21 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1vfdeek/inclusionailing30flash_weights_are_up_on_hugging/)

**背景**: 稀疏混合专家（MoE）模型的总参数量很大，但每个 token 只激活少量&\#x27;专家&\#x27;子集，从而降低推理时的计算成本。FP8 是一种 8 位浮点格式，相比 BF16 占用更少内存和带宽，但需要仔细选择缩放以避免精度下降。本次发布同时提供两种格式，用户可根据硬件在质量与资源占用之间取舍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://agihunt.info/en/e/19fcd5e1d55d6d0b5b5a2e6a166">inclusionAI Open-Sources 127B MoE Model … · AGI Hunt</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://arxiv.org/html/2309.17224">Training and inference of large language models using 8-bit ...</a></li>

</ul>
</details>

**社区讨论**: 评论区总体表示欢迎，有人说等这个模型比等 Qwen3.8-27B 还久，也有人询问 llama.cpp 是否已支持 bailing\_hybrid，还是目前仅支持 vLLM 和 SGLang。还有几位用户把它与 DeepSeek-Flash 0731 比较，并指出其基准图相对最新的 DeepSeek preview 可能已过时。

**标签**: `#LLM`, `#Open Source`, `#Mixture of Experts`, `#Hugging Face`, `#FP8`

---

<a id="item-10"></a>
## [呼吁 Lua 社区停止支持旧版本](https://hisham.hm/2026/08/04/the-lua-community-needs-to-learn-to-move-on/) ⭐️ 8.0/10

hisham.hm 上一篇题为《The Lua community needs to learn to move on》的博文呼吁 Lua 社区停止支持非常旧的解释器版本。文章认为，持续支持这些旧版本会导致维护者过度劳累，并阻碍生态系统的前进。 Lua 生态的版本碎片化严重，包括 Lua 5.1 到 5.4 以及 LuaJIT，这迫使库维护者需要对横跨二十多年的旧版本进行测试和调试。如果核心解释器维护者已经表明旧版本将停止支持，社区也应跟进，以减轻维护者负担并保持项目可持续性。 社区评论显示，核心解释器维护者 Roberto Ierusalimschy 和 Mike Pall 据称正在逐步停止对旧版 Lua 和 LuaJIT 的支持。评论者还强调，库也应停止支持非常旧的 Lua 版本，并且报告 bug 的人应事先对照最新版本和源代码进行确认。

reddit · r/programming · f311a · 8月4日 18:52 · [社区讨论](https://www.reddit.com/r/programming/comments/1vfjdqy/the_lua_community_needs_to_learn_to_move_on/)

**背景**: Lua 是一种轻量级、可嵌入的脚本语言，广泛应用于游戏和应用程序中。它有多个主要版本，而 LuaJIT 作为一种独立的即时编译器实现，在版本更新上落后于主发行版。这篇文章讨论的是保持向后兼容与 Lua 开源生态系统中有限的志愿者精力之间的张力。

**社区讨论**: 评论者大多赞同这一观点，认为希望使用旧版 Lua 的用户也应该使用旧版配套生态，以免给维护者带来负担。还有人建议，报告 bug 前应先检查最新版本和源代码；也有人指出一个 LuaJIT 的 issue 是很好的首个 PR。

**标签**: `#Lua`, `#open source`, `#maintenance`, `#legacy support`, `#community`

---

<a id="item-11"></a>
## [Mistral 推出 Shieldstral：3B 开放权重多模态内容审核模型](https://mistral.ai/news/shieldstral/) ⭐️ 7.0/10

Mistral 发布了 Shieldstral，一个 3B 参数、开放权重的多模态内容审核模型。它通过自然语言策略问题执行提示词和回复审核、拒答检测以及安全性过滤，并返回是/否判断。 这为开发者提供了一种经济、可定制的替代方案，来替代封闭的审核 API，尤其适合图像分享或社交平台。由于权重开放，团队可以自行部署并根据自身策略调整审核规则。 据 Mistral 介绍，Shieldstral 只有 3B 参数，但性能可超越最大为其 7 倍的模型。它是一个紧凑的多模态模型，可处理文本和图像输入，并使用自然语言策略问题而非固定类别标签。

hackernews · r/LocalLLaMA · riadsila · 8月4日 16:36 · [社区讨论](https://news.ycombinator.com/item?id=49171268)

**背景**: 开放权重模型意味着训练好的网络权重会公开发布，但训练代码、数据集和架构通常不完全开放，且许可协议可能限制使用。内容审核模型将文本和图像分类为安全或不安全，帮助平台过滤有害内容。Mistral 是一家 AI 公司，近期发布了紧凑的多模态模型 Shieldstral 用于此目的，为大型封闭审核服务提供了一个小巧高效的替代选择。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>
<li><a href="https://docs.mistral.ai/models/model-cards/shieldstral-1-0">Shieldstral 1.0 - docs.mistral.ai</a></li>
<li><a href="https://www.ai21.com/glossary/open-weights-model/">What is an Open - Weights Model ? | AI21</a></li>

</ul>
</details>

**社区讨论**: 评论者好奇 Shieldstral 是否能调整为任意规则集，还是只匹配固定审核风格；也有人开玩笑说其命名以及用它来“关住 AGI”。一些开发者欢迎它，称它是图像分享与社交平台现实且经济的解决方案；还有人询问它与 OpenAI 的 omni-moderation 模型对比如何，并指出非确定性模型只是第一道防线，仍需要人工复核。

**标签**: `#AI`, `#content-moderation`, `#open-source`, `#Mistral`, `#multimodal`

---

<a id="item-12"></a>
## [生成多样化肤色的简单算法与色彩空间](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 7.0/10

开发者 toneyalexander 发布了一个新的色彩空间和一组简单方程，用于生成多样化且逼真的肤色，并附带了交互式取色器、程序化生成算法和详细文档。该色彩空间使用两个轴：一个明暗轴和一个红黄轴。 该项目为数字艺术和游戏开发中的一个常见难题提供了实用且易用的解决方案：如何挑选可信且多样化的肤色。同时，它也推动了关于色彩科学、人类感知以及数字媒体中包容性表现的持续讨论。 该实现基于 JavaScript，页面中的交互演示均由这些方程驱动。作者承认其方法论可能不太严谨，并在 Future Work 部分列出了改进方向；评论者也指出其未参考 Pantone Skin Tones 等标准，并观察到部分生成的颜色带有绿、蓝或紫色调。

hackernews · automatoney · 8月4日 15:16 · [社区讨论](https://news.ycombinator.com/item?id=49170165)

**背景**: 肤色并不是一个简单的物理量，它还受到人类感知、光照等多种因素的影响。大多数色彩空间（如 sRGB）是为显示设备设计的，并不适合直观地探索人类肤色；在 Oklab 等感知均匀的色彩空间中，肤色往往呈月牙形分布。作者尝试定义一个自定义色彩空间，让艺术家更容易选择多样化的肤色，并借鉴了关于肤色行为方式的现有研究和观察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49170165">Show HN: Simple algorithm and color space to generate diverse skin tones</a></li>
<li><a href="https://www.reddit.com/r/proceduralgeneration/comments/1vdcgbe/simple_algorithm_and_color_space_to_generate/">Simple algorithm and color space to generate diverse skin tones - Reddit</a></li>
<li><a href="https://creativecalvert.com/digital-art/digital-art-skin-color-palette-master-realistic-tones-like-a-pro/">Digital Art Skin Color Palette: Master Realistic Tones Like a ...</a></li>

</ul>
</details>

**社区讨论**: 整体反响积极，评论者称赞其展示方式和“巧妙”的函数拟合思路。也有人提出了建设性批评，例如缺少对 Pantone Skin Tones 等现有标准的参考，以及部分输出颜色出现绿、蓝、紫等色调；还有人指出生成的颜色与真实粉底色号数据中呈现的月牙形分布一致。

**标签**: `#color space`, `#skin tones`, `#digital art`, `#procedural generation`, `#algorithm`

---

<a id="item-13"></a>
## [Waymo 在达拉斯向所有人开放无人驾驶网约车服务](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 7.0/10

Waymo 已在德克萨斯州达拉斯向所有用户开放其自动驾驶网约车服务，使达拉斯成为又一个公众可随时呼叫无人驾驶汽车的大城市。该服务现已面向普通公众，而非仅限候补名单或特定乘客。 这一扩张是自动驾驶汽车商业化部署的重要里程碑，将无人驾驶网约车带入达拉斯-沃斯堡这样低密度、高度依赖汽车的大都会区。这可能重塑城市出行方式，并加剧与优步、来福车等人工驾驶网约车服务的竞争。 该服务此前仅面向候补名单或特定乘客，此次向公众全面开放，使达拉斯成为拥有全无人驾驶网约车的最大美国都会区之一。公告中未提及车队规模或定价等信息。

hackernews · xnx · 8月4日 18:29 · [社区讨论](https://news.ycombinator.com/item?id=49172836)

**背景**: Waymo 是 Alphabet 旗下的自动驾驶技术公司，运营商业自动驾驶出租车服务。其车辆配备激光雷达、雷达和摄像头等传感器，并结合 AI 软件实现无需人类司机的道路导航。该公司已从凤凰城和旧金山逐步扩展到其他美国城市，旨在证明无人驾驶出行的安全性和可行性。

**社区讨论**: 评论者观点各异：有人称赞无人驾驶汽车是被忽视的经济适用房政策，有人分享了在洛杉矶的正面体验，称 Waymo 的预测性和安全性很好。但也有人担心其对本地经济的影响，认为付给 Waymo 的钱可能不像付给人类司机那样在本地流通。

**标签**: `#autonomous-vehicles`, `#waymo`, `#ride-hailing`, `#dallas`, `#ai`

---

<a id="item-14"></a>
## [Oxide Computer 完成 4.45 亿美元 D 轮融资](https://www.sec.gov/Archives/edgar/data/1795071/000179507126000002/xslFormDX01/primary_doc.xml) ⭐️ 7.0/10

Oxide Computer 是一家构建机架级云基础设施的初创公司，根据 SEC Form D 备案，该公司已完成 4.45 亿美元的 D 轮融资。此前该公司已相继完成 4400 万美元 A 轮、1 亿美元 B 轮和 2 亿美元 C 轮融资。 这笔大规模融资验证了 Oxide 将整个机架作为一台软件定义计算机来销售的愿景，对现有云服务提供商和传统服务器厂商构成挑战。这也表明投资者认为，能够提供类似云体验的本地机架级系统拥有可观的市场。 该备案文件显示本轮为 D 轮融资，提交日期见 SEC 文件。Oxide 的做法是将整个机架（包括计算、存储、网络和管理软件）作为集成产品交付，而不是让用户从不同厂商组装组件。

hackernews · depr · 8月4日 20:13 · [社区讨论](https://news.ycombinator.com/item?id=49174407)

**背景**: 机架级计算将整个服务器机架视为单一的基础设施单元，跨节点池化资源以提高效率并简化运维。Oxide Computer 由前 Joyent 工程师创立，旨在通过交付包含完整软硬件栈的单机架，将云架构引入本地数据中心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacenterknowledge.com/servers/what-is-rack-scale-computing-and-why-is-it-relevant-again-">What Is Rack-Scale Computing? - datacenterknowledge.com</a></li>

</ul>
</details>

**社区讨论**: 社区反应从兴奋到建设性批评不一。有人称赞产品理念和创始人，也有人质疑 Oxide 是否真的出货硬件，并指出销售跟进不佳——一位评论者说他们每年在 AWS 上花费 90 万美元，但填写 Oxide 销售表单后从未收到回复。

**标签**: `#funding`, `#hardware`, `#systems`, `#cloud`, `#oxide`

---

<a id="item-15"></a>
## [MiniMax-H3 全模态模型移植 MLX，支持 Apple Silicon 本地运行](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 7.0/10

MiniMax 两天前发布了全模态生成系统 MiniMax-H3；一个社区 Python 包现已将其移植到 Apple 的 MLX 框架。Simon Willison 在 M5 Max MacBook Pro 上运行了它，通过文本提示生成了一个带音频的 15 秒视频片段。 这个移植让开发者和研究人员可以在 Apple Silicon 上本地运行先进的 omni-modal 视频生成模型，而无需依赖云端 API。它使动手实验更加便捷，不过这是一个增量发布而非范式转变。 该模型需要下载约 115 GB 的文件，生成示例视频耗时近 45 分钟。由于未遵循提示词编写指南，生成的音频是奇怪的类似语音的噪音；该指南提供了实现更好音视频对齐的说明。

rss · Simon Willison · 8月4日 19:10

**背景**: MLX 是 Apple Machine Learning Research 开发的开源数组框架，用于在 Apple Silicon 上进行机器学习，提供类似 NumPy 的 Python API。Omni-modal（全模态）AI 模型旨在将文本、图像、音频和视频的感知统一到单一模型中。MiniMax-H3 是一个通用全模态生成模型，可以生成最高 2K 分辨率、最长 15 秒、带原生立体声音频的视频。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/ml-explore/mlx">GitHub - ml-explore/ mlx : MLX : An array framework for Apple silicon</a></li>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H 3 : An Open Model Breaking the Boundaries Between Tasks...</a></li>
<li><a href="https://grokipedia.com/page/MLX_machine_learning_framework">MLX ( machine learning framework )</a></li>

</ul>
</details>

**标签**: `#MiniMax-H3`, `#MLX`, `#Apple Silicon`, `#omni-modal`, `#generative model`

---

<a id="item-16"></a>
## [Hugging Face CEO 称中国凭借开源模型与供应链领跑 AI 竞赛](https://www.cnbc.com/2026/08/03/hugging-face-china-ai-race-open-models.html) ⭐️ 7.0/10

在 2026 年 8 月的一次访谈中，Hugging Face 的 CEO 表示，中国正凭借开源权重模型以及覆盖原材料、国产光刻设备、自研 GPU 制造、廉价能源和模型开发的独立供应链，赢得 AI 竞赛。 这一说法挑战了以美国为中心的 AI 主导假设，并凸显了 Qwen、DeepSeek 等中国开源模型日益增长的全球影响力。这可能会影响资金投入重点、出口管制以及西方实验室对待开源 AI 的方式。 CEO 提到了原材料、国产光刻设备、自产 GPU 制造、廉价能源以及首个聚变反应堆的进展。社区评论者指出，美国仍有强大的开源权重模型，但数量远少于中国。

reddit · r/LocalLLaMA · Miriel\_z · 8月4日 18:42 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1vfj3q7/hugging_face_ceo_says_china_is_winning_the_ai/)

**背景**: 开源权重 AI 模型会公开发布训练好的参数，允许开发者下载、微调并在本地运行，例如 Qwen、DeepSeek、Llama 和 Kimi K3。光刻设备（如 ASML 的 EUV 光刻机）是制造先进半导体的关键，中国一直在努力构建国产替代方案。中国的 EAST 托卡马克和规划中的 CFETR 是其发展聚变能源计划的一部分，未来可能为 AI 训练提供丰富低碳电力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.asml.com/en/technology">ASML technology | Supplying the semiconductor industry</a></li>
<li><a href="https://indianexpress.com/article/explained/explained-what-is-chinas-artificial-sun-experimental-fusion-reactor-that-has-set-a-new-record-7341397/">Explained: What is China ’s ‘artificial sun’ experimental fusion reactor ...</a></li>
<li><a href="https://huggingface.co/blog/daya-shankar/open-source-llms">Best Open - Source LLM Models in 2026: Coding, Local, Agentic AI ...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对美国的竞争力感到悲观，认为削减资金和过度依赖大型实验室损害了开放创新。有人称赞 Thinking Machines Lab 的 Inkling 等美国特定模型，而一名欧盟用户表示自己会“吃着爆米花”在家运行 Qwen 这样的中国模型。

**标签**: `#AI race`, `#China`, `#open models`, `#geopolitics`, `#Hugging Face`

---

<a id="item-17"></a>
## [通义千问开放权重模型下周发布，含 Qwen3.8-27B](https://i.redd.it/85mvexgsaehh1.jpeg) ⭐️ 7.0/10

阿里巴巴通义千问团队宣布，开放权重模型将于下周发布，首先推出 270 亿参数的 Qwen3.8-27B，后续还有更多尺寸。该消息由 xiong\_hui\_chen 在推特上发布，随后在 Reddit 上迅速传播。 这一消息意义重大，因为本地部署和自托管大模型社区一直担忧开源小语言模型正走向衰落。此次发布表明，小尺寸开放权重模型仍是优先事项，能为用户提供更易获得、成本更低且可在设备端运行的 AI 方案。 公告具体提到了 Qwen3.8-27B，并承诺稍后还会发布更多模型。社区成员希望看到其他尺寸，例如 122B 版本，但团队尚未确认究竟会发布哪些额外规格。

reddit · r/LocalLLaMA · Capital-Remove-6150 · 8月4日 17:45 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1vfhhpq/no_more_slm_opensource/)

**背景**: 通义千问（Qwen）是阿里巴巴的大语言模型系列，于 2023 年 4 月以“通义千问”之名首次推出。小语言模型（SLM）的参数量远少于大语言模型，因此更适合在单台电脑或移动设备上运行。阿里巴巴此前已发布过 Qwen 72B、7B 和 1.8B 等开放权重模型，社区常将其用于自托管和微调。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Qwen">Qwen - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Small_language_model">Small language model</a></li>

</ul>
</details>

**社区讨论**: Reddit 用户总体反响积极，但也指出这一公告本可以放在更显眼的位置。有人猜测团队可能尚未开发出其他尺寸的模型，并将其与谷歌 Gemini 3.5 Pro 的情况相类比；还有用户开玩笑说，如果发布 Qwen 122B，今后就只从 AliExpress 购物。

**标签**: `#Qwen`, `#open-source`, `#LLM`, `#SLM`, `#AI`

---

<a id="item-18"></a>
## [SK 海力士与闪迪发布 HBF 标准，瞄准 3TB/s 带宽](https://wccftech.com/sk-hynix-sandisk-high-bandwidth-flash-hbf-standard-3tbs/) ⭐️ 7.0/10

SK 海力士与闪迪公布了新一代存储技术高带宽闪存（HBF）的首份标准规范，旨在弥合 AI 系统中 HBM 与 SSD 之间的性能差距，目标带宽高达 3TB/s。 这很重要，因为 AI 推理的瓶颈通常在于内存容量和带宽；HBF 可以通过提供高容量、高带宽的存储来大幅加速本地推理。它还可能重塑 AI 加速器的内存层级，影响模型部署方式。 HBF 被定位为 HBM 与 SSD 之间的“冷/温层级”，在提供远高于 HBM 容量的同时保持接近的性能。该规范于 2026 年未来存储与内存大会上公布，目前尚未有量产产品发布。

reddit · r/LocalLLaMA · giveen · 8月4日 13:17 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1vfa3tq/sk_hynix_in_collaboration_with_sandisk_unveils/)

**背景**: AI 加速器面临快速但容量小的 HBM 与大容量但速度慢的 SSD 之间的性能差距。HBF 旨在通过高带宽配置的闪存来填补这一空白，并与 HBM 形成分层内存架构，用于 AI 训练、推理和边缘计算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wccftech.com/sk-hynix-sandisk-high-bandwidth-flash-hbf-standard-3tbs/">SK hynix, In Collaboration With SanDisk, Unveils The New High ...</a></li>
<li><a href="https://www.koreajoongangdaily.com/business/sk-hynix-sandisk-unveil-first-hbf-standard-for-ai-storage/12807551">SK hynix, SanDisk unveil first high bandwidth flash standard for AI...</a></li>
<li><a href="https://www.lovechip.com/blog/hbm-vs-hbf-vs-hbs">HBM VS HBF VS HBS: Building the Memory Hierarchy for AI ...</a></li>

</ul>
</details>

**社区讨论**: 社区反响积极，一位用户表示“终于不用拿内存来做这种事了”，对使用 RAM 承担大上下文表示不满。另一位用户则担心 SSD 产线会被转用于 HBF，导致 SSD 价格上涨，尽管这能缓解显存压力。

**标签**: `#AI hardware`, `#memory`, `#storage`, `#inference`, `#HBF`

---

<a id="item-19"></a>
## [美国新 AI 指南豁免开放模型政府审查](https://www.wsj.com/tech/ai/white-houses-ai-guidelines-exempt-u-s-open-models-from-government-review-74924eb8) ⭐️ 7.0/10

白宫发布了新的 AI 指南，豁免美国开发的开放模型在接受政府安全审查。这是一个重大的政策转向，使开源 AI 开发者能够更自由地发布模型，而无需事先获得批准。 这一政策可能通过取消一层监管监督来加速美国开源 AI 的创新。但它也引发了对全球竞争的担忧，因为包括中国公司在内的外国实体可以分叉美国的开放模型，并可能从同样的豁免中受益。 豁免特别适用于“美国开放模型”，这表明了国内来源的要求。指南没有明确说明不包含训练数据和代码的开放权重模型是否符合条件，这使社区中的一个关键区别仍未得到解决。

reddit · r/LocalLLaMA · realmvp77 · 8月4日 23:35 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1vfqqdb/white_house_ai_guidelines_exempt_us_open_models/)

**背景**: 开放模型公开了 AI 模型的权重，使开发者能够运行、微调并在此基础上构建。与完全开源的 AI 不同，开放权重模型通常不包含训练数据和训练代码，这影响了透明度和可复现性。各国政府一直在讨论如何监管开放模型，在创新与潜在滥用之间取得平衡。新指南似乎对美国模型采取了更宽松的态度。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/glossary/open-models/">What are Open Models? | NVIDIA Glossary</a></li>
<li><a href="https://www.linkedin.com/pulse/open-weights-vs-source-llms-why-difference-matters-more-kapil-uthra-6kanf">Open Weights vs . Open Source in LLMs: Why the Difference Matters...</a></li>
<li><a href="https://opensource.org/ai/open-weights">Open Weights : not quite what you’ve been told – Open Source Initiative</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，通常从美国开放模型分叉出来的中国模型也可能从豁免中受益。一位评论者认为，该政策可能是试图对中国公司施压，而另一位则分享了文章的无付费墙链接。

**标签**: `#AI policy`, `#open source`, `#regulation`, `#US government`

---

<a id="item-20"></a>
## [Liquid AI 2.6B 工具调用模型在手机上可达 30 tok/s](https://i.redd.it/xxbkpo9jcfhh1.jpeg) ⭐️ 7.0/10

Liquid AI 发布了 LFM2.5-2.6B，这是一个 2.69B 参数的模型，支持 128K 上下文和工具调用，并针对多步智能体工作流进行了优化。其 Q4\_K\_M GGUF 约为 1.67 GB，在手机上可达 30 tok/s，在 Ryzen AI Max+ 395 上为 113 tok/s，在 M5 Max 上为 220 tok/s。 这一发布意义重大，因为它表明强大的工具调用和智能体行为可以在消费级硬件上完全本地运行，而不只依赖大型云端模型。这类小尺寸本地模型可以作为廉价的“工作代理”处理信息抽取、搜索和重复性工具调用，而更大模型负责规划。 厂商基准测试显示，ToolSandbox 为 77.83、IFBench 为 59.17、BFCLv4 为 56.88、LiveCodeBench 为 59.41，工具使用分数接近 Qwen3.5-9B 但并非全面超越。模型卡提示不推荐用于 agentic 编程，且 128K 上下文声明仍需在真实负载下进行独立验证。

reddit · r/LocalLLaMA · BTA\_Labs · 8月4日 21:15 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1vfn9vc/a_26b_model_with_tool_calling_and_128k_context/)

**背景**: GGUF 是一种文件格式，将张量、分词器和元数据打包到单个自包含文件中，是运行量化本地 LLM 的主流格式。Q4\_K\_M 等量化方式会降低模型权重的精度，以较小的精度损失换取更低内存占用和更高速度。工具调用（tool calling）让 LLM 可以请求外部函数和 API，从而在语言生成与现实操作之间建立桥梁。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GGUF">GGUF - Wikipedia</a></li>
<li><a href="https://www.datacamp.com/tutorial/gguf-format-a-complete-guide">GGUF Format: A Complete Guide to Local LLM Inference</a></li>
<li><a href="https://www.ibm.com/think/topics/tool-calling">What is tool calling? - IBM</a></li>

</ul>
</details>

**社区讨论**: 早期用户反馈称，在 RX 6650 XT 上工具调用很稳定，但该模型在多步文件任务中“仍然有些不聪明”，即使尝试多种量化级别仍然如此。一位基准测试评测者计划将该模型加入测试，另一位用户则表示其旧笔记本难以运行此前的 1.2B 和 8b1b 模型，且 Qwen 4B 在能力上更胜一筹。总体态度谨慎乐观，同时赞赏 Liquid 对小语言模型的投入。

**标签**: `#local-ai`, `#LLM`, `#tool-calling`, `#efficient-models`, `#edge-computing`

---

<a id="item-21"></a>
## [美国 AI 让 5 万架乌克兰自杀式无人机自主追踪目标](https://arstechnica.com/ai/2026/08/ukraines-drones-get-ai-upgrades-for-kamikaze-strikes-future-swarm-attacks/) ⭐️ 7.0/10

一家美国公司签署了一份价值 1 亿美元的合同，为 5 万架乌克兰自杀式无人机配备可自主追踪目标的人工智能。这套 AI 让廉价的游荡弹药能够自行锁定并跟踪目标，而不只依赖人工操作员。 这标志着 AI 驱动的自主目标锁定技术在实际战斗中大规模部署，使乌克兰的无人机从遥控武器转向半自主武器。这可能改变无人机战争的成本结构，并加剧国际社会对自主武器做出杀伤决定的担忧。 据报道，这笔交易涵盖 5 万枚游荡弹药，单价约 2000 美元；该 AI 被设计用于在 GPS 受限和不确定环境中进行实时目标锁定。自主目标跟踪结合传感器、机器学习与实时数据处理，可在无需人工持续操控的情况下跟踪目标。

reddit · r/artificial · ControlCAD · 8月4日 05:22 · [社区讨论](https://www.reddit.com/r/artificial/comments/1vf144v/us_companys_ai_lets_ukraines_cheap_kamikaze/)

**背景**: 自杀式无人机又称游荡弹药，是一种一次性无人机，可在目标区域上空盘旋，然后俯冲撞击目标并引爆。传统上，它们需要操作员通过摄像头画面和数据链来识别并指定目标。加入 AI 后，无人机可自行探测并跟踪目标，从而降低操作员负担，也使无人机蜂群作战更可行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Loitering_munition">Loitering munition - Wikipedia Loitering Munitions 101: What They Are and Why They Matter Loitering munitions explained | Unmanned Aerial Weapons Loitering Munitions in Modern Combat: Addressing Tactical ... L-297 Loitering Munitions - Munitions Safety Information ... Loitering Munitions - Uvision What Is a Loitering Munition and How Does It Work?</a></li>
<li><a href="https://defenceagenda.com/ai-enabled-drone-targeting">AI-enabled drone targeting systems - Defence Agenda</a></li>
<li><a href="https://www.idga.org/command-and-control/articles/loitering-munitions-101-what-they-are-why-they-matter">Loitering Munitions 101: What They Are and Why They Matter</a></li>

</ul>
</details>

**社区讨论**: 评论者总体持批评态度，有人说当机器能挑选要杀害的人类时，‘我们为自己制造了一个地狱’；还有人指责这笔交易是‘为了生意而助燃战争’。另有评论者对价格提出质疑，调侃说 2000 美元一架的单价应该争取批量折扣。

**标签**: `#AI`, `#military`, `#autonomous weapons`, `#drones`, `#ethics`

---

<a id="item-22"></a>
## [国际刑警组织：人工智能驱动非洲超半数网络犯罪，诈骗激增](https://www.africanews.com/2026/08/04/ai-fuels-more-than-half-of-cybercrime-in-africa-as-digital-scams-surge-interpol/) ⭐️ 6.0/10

国际刑警组织《2026 年非洲网络威胁评估》报告称，人工智能驱动的技术现已占非洲网络犯罪的一半以上。这一激增主要归因于由生成式 AI 工具助力的数字诈骗。 这表明非洲已成为 AI 相关网络犯罪的主要前沿，即使是低技能犯罪分子也能部署极具迷惑性的自动化攻击。全球的政策制定者和安全团队都需要适应这一变化，因为这些手法可能迅速扩散到非洲以外地区。 该结论来自国际刑警组织发布的《2026 年非洲网络威胁评估报告》，发布于 interpol.int。文章未明确&\#x27;AI 驱动&\#x27;的确切定义，但很可能包括 AI 生成的钓鱼内容、深度伪造以及机器人驱动的社会工程攻击。

hackernews · bookofjoe · 8月4日 22:01 · [社区讨论](https://news.ycombinator.com/item?id=49175826)

**背景**: 非洲互联网和手机使用量快速增长，扩大了网络犯罪分子的攻击面。AI 工具可以生成逼真的消息、伪造文件和虚假音视频，使传统诈骗更具说服力、更难以识别。国际刑警组织的区域评估旨在帮助执法部门了解并应对这些新兴威胁。

**社区讨论**: 评论者分享了实际经验：一位 SaaS 运营者称 AI 机器人数量惊人，并感谢 Cloudflare 的保护；另一人认为互联网、手机和社交媒体才是真正的燃料，AI 只是让骗局更可信。也有人指出 AI 是一把双刃剑，还有人开玩笑说 AI 在西方也是最大的骗局，暗指 OpenAI 未来 IPO。

**标签**: `#cybersecurity`, `#AI`, `#cybercrime`, `#Africa`, `#Interpol`

---

<a id="item-23"></a>
## [Revoy 混动串列挂车获 2700 万美元融资，加速柴油卡车电动化](https://electrek.co/2026/08/04/revoy-ev-promises-to-electrify-diesel-semis-in-minutes/) ⭐️ 6.0/10

Revoy 已融资 2700 万美元，以推进其混合动力串列挂车概念，该装置可安装在传统半挂卡车与挂车之间。该公司称该系统可为柴油车队“电动化”并将燃油费用减半，距离量产又近一步。 如果成功，Revoy 的方案可为减少柴油卡车排放提供更快、更廉价的路径，无需更换卡车或为每辆车新建充电设施。该方案瞄准存量巨大的柴油半挂车队，有望加速长途货运的脱碳进程。 该混合动力装置将电池和电驱动桥集成到一个串列挂车/小车（dolly）中，置于卡车与挂车之间。文章还提到“尚余 11 吨的疑问”，暗示在量产前仍面临重量、成本和集成等方面的挑战。

rss · Electrek · 8月4日 11:20

**背景**: 传统半挂卡车由牵引车头牵引挂车，而增加小车（dolly）或串列挂车会多出一个车轴。Revoy 的概念是为该车轴配备电动机和电池，使电机在加速时辅助驱动，制动时通过再生制动回收能量。这种混合动力方式无需全电动卡车或每处场站新建充电设施，即可降低柴油消耗。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://electrek.co/2026/08/04/revoy-ev-promises-to-electrify-diesel-semis-in-minutes/">Revoy hybrid tandem trailer rolls towards reality with $27 ...</a></li>
<li><a href="https://electrek.co/2024/01/31/revoy-ev-promises-to-electrify-diesel-semis-in-minutes/">Revoy EV promises to electrify diesel semis in minutes</a></li>
<li><a href="https://www.newsbreak.com/news/4808511122439-revoy-hybrid-tandem-trailer-rolls-towards-reality-with-27-million-raise">Revoy hybrid tandem trailer rolls towards reality with $27 ...</a></li>

</ul>
</details>

**标签**: `#EV`, `#trucking`, `#hybrid`, `#funding`, `#technology`

---

<a id="item-24"></a>
## [Steve Yegge 称 Opus 4.7 的“再来两件事”毛病毁了 Gas Town](https://simonwillison.net/2026/Aug/4/steve-yegge/#atom-everything) ⭐️ 6.0/10

Steve Yegge 表示，他的 AI 编程智能体工具包 Gas Town 在 Claude Opus 4.7 上不再可靠，而此前在 Opus 4.6 之前一直运行良好。他说该模型出现了一种持续的“再来两件事”毛病，使它始终无法收敛并进入实际工作。 这件事凸显了 AI 编程智能体在实际可靠性上的挑战：即便是重大模型升级，也可能引入细微的行为怪癖，进而破坏整个智能体工作流。它也说明，除了能力提升，模型回退同样会影响开发者对智能体工具的信任与设计。 Gas Town 是 Yegge 的开源工具包，用于编排多智能体编码工作流；它本应可复用，但最终只被用来构建自身。Yegge 表示，在遇到其他问题之后，Opus 4.7 是“压垮骆驼的最后一根稻草”，导致 Gas Town“实际上被烧毁”。

rss · Simon Willison · 8月4日 00:42

**背景**: Gas Town 是 Steve Yegge 公开构建的开源工具包，用于在多智能体工作区中编排 AI 编码智能体。Claude Opus 4.7 是 Anthropic 的旗舰模型版本，官方称其在长任务处理、精确遵循指令和自我验证方面表现更好。Yegge 的这番话出自他的文章《The Shape of Things to Come》，并由 Simon Willison 引用转发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://yegge.ai/gastown">Gas Town — Steve Yegge</a></li>
<li><a href="https://github.com/gastownhall/gastown">GitHub - gastownhall/gastown: Gas Town - multi-agent ...</a></li>
<li><a href="https://steve-yegge.medium.com/welcome-to-gas-town-4f25ee16dd04">Welcome to Gas Town - steve-yegge.medium.com</a></li>

</ul>
</details>

**标签**: `#steve-yegge`, `#coding-agents`, `#generative-ai`, `#opus`

---

<a id="item-25"></a>
## [Gemma 4 在 500MB 上运行：惊人的压缩与存疑的实用性](https://i.redd.it/xo71biijsdhh1.jpeg) ⭐️ 6.0/10

Reddit 上 r/LLMDevs 的一篇帖子展示了谷歌 Gemma 4 仅用 500MB 内存运行，体现了极端的模型压缩。该帖子附带一条推文链接，并引发关于这么小的模型在设备上是否仍具实用性的讨论。 如果属实，这表明高度量化的 Gemma 4 模型可以在智能手机等内存受限设备上运行，扩大端侧 AI 的应用。这也凸显了模型压缩的发展趋势，但其实际可用性和质量仍是未解之谜。 500MB 这个数字很可能来自对最小 Gemma 4 变体（如面向边缘设备的 E4B 或 E2B 模型）进行激进量化的结果。讨论区用户还担心电池消耗，有人估计每次请求耗电 5%。

reddit · r/LocalLLaMA · jacek2023 · 8月4日 16:01 · [社区讨论](https://www.reddit.com/r/LocalLLaMA/comments/1vfeick/gemma_4_on_500mb/)

**背景**: Gemma 4 是谷歌于 2026 年 4 月 2 日发布的开源权重模型系列，采用 Apache 2.0 许可证，是 Gemini 的开放对应版本。量化通过降低模型数值精度来缩小体积和内存占用，使大语言模型得以在消费级硬件上运行。端侧 AI 性能常常受内存限制，因此激进压缩对手机和边缘设备很有吸引力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.google.dev/gemma/docs/core/model_card_4">Gemma 4 model card | Google AI for Developers</a></li>
<li><a href="https://theairankings.com/google/gemma-4/">Gemma 4: Google&#x27;s Open-Weight Models — Sizes, Specs &amp; Review ...</a></li>
<li><a href="https://giznova.in/on-device-ai-memory-limits/">On-Device AI Memory Limits: Performance, Thermal, and Memory ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人对这一成就感到兴奋，也有人质疑这么小的模型是否仍有可用性，还是‘笨得像门板’。热评提到每次请求耗电 5% 的问题，还有一位用户毫不掩饰地表达了对这一消息的喜悦。

**标签**: `#LLM`, `#Gemma`, `#edge computing`, `#model compression`, `#on-device AI`

---

<a id="item-26"></a>
## [中国电动汽车出口热潮开始影响全球汽油需求](https://www.reuters.com/commentary/reuters-open-interest/chinas-ev-export-boom-is-starting-show-up-gasoline-market-2026-08-04/) ⭐️ 6.0/10

一篇路透评论文章指出，中国电动汽车出口的快速增长开始抑制全球汽油需求。这标志着电动汽车普及正在推动能源市场出现显著转变。 这一趋势可能加速全球石油需求见顶，对产油国和炼油行业产生影响，同时凸显交通运输业加速向电动化转型。 这篇文章属于评论性质，而非技术分析。有评论者指出，美国高燃油效率汽油车对汽油需求的影响更大；另有人提出因果关系可能相反，是燃料供应减少推动了电动汽车普及。

reddit · r/electricvehicles · Biodieselisthefuture · 8月4日 14:08 · [社区讨论](https://www.reddit.com/r/electricvehicles/comments/1vfbesw/chinas_ev_export_boom_is_starting_to_show_up_in/)

**背景**: 电动汽车以电力代替汽油为动力，因此其普及会减少汽油需求。中国已成为全球最大的电动汽车生产国和出口国，其出口热潮的规模已足以影响全球汽油消费。这一点很重要，因为汽油是主要石油产品，其需求变化会牵动整个石油供应链。

**社区讨论**: 评论意见褒贬不一但讨论热烈。一位电动汽车车主表示欢迎，另一人则称这是老生常谈，并指出美国燃油效率提升的影响更大。还有评论者认为因果关系可能相反：汽油供应受限、价格高企，正在推动消费者转向廉价的中国电动汽车。

**标签**: `#electric vehicles`, `#energy markets`, `#China`, `#gasoline`, `#economics`

---

<a id="item-27"></a>
## [苹果诉 OpenAI 窃取机密遭反转：前员工仍被苹果咨询](https://i.redd.it/ywjrw864cbhh1.jpeg) ⭐️ 6.0/10

OpenAI 公布了内部消息，显示苹果员工在工程师 Chang Liu 离职数周后仍向他请教文件位置和产品决策等问题，这令苹果的商业机密指控受到挑战。 这场法律交锋使苹果对 OpenAI 的诉讼变得更加复杂，并凸显了离职流程管理不善如何削弱科技行业中的商业机密主张。 OpenAI 称苹果谎称已联系该公司并未获回复，并列举邮件显示苹果外聘律师误感谢 OpenAI 总法律顾问一次从未发生的通话。已公布的消息并不能推翻苹果更广泛的商业机密指控。

reddit · r/artificial · Left-Hotel904 · 8月4日 07:46 · [社区讨论](https://www.reddit.com/r/artificial/comments/1vf3ow5/apple_sued_openai_for_stealing_hardware_secrets/)

**背景**: 在科技行业纠纷中，企业常以涉嫌窃取机密为由起诉前员工及其新雇主。此类案件的一个关键争点是原雇主是否妥善保护了自身机密并执行了规范的离职流程。

**社区讨论**: 评论者对苹果的诉讼持怀疑态度，有人指出苹果员工只是在询问该工程师在苹果期间的旧工作，而非其新工作中的机密。还有人认为这些消息“太弱了”。整体情绪倾向于认为这些披露削弱了苹果的指控。

**标签**: `#Apple`, `#OpenAI`, `#legal`, `#trade-secrets`

---

<a id="item-28"></a>
## [Reddit 股价下跌，CEO 质疑 Google AI Overviews 价值](https://arstechnica.com/ai/2026/08/reddit-ceo-on-ai-overviews-were-still-looking-for-that-win-win/) ⭐️ 6.0/10

随着 Reddit 股价下跌，其 CEO 公开质疑 Google AI Overviews 的价值，并表示仍在寻找所谓的“双赢”。这一表态凸显了 AI 生成摘要与原创内容平台流量之间的紧张关系。 AI Overviews 正在减少内容网站的引荐流量，而 Reddit 长期依赖 Google 搜索获取用户。如果 Reddit 这样的大型平台公开反击，可能会影响 AI 公司与内容发布者之间关于内容使用和收入分成的谈判格局。 Google 的 AI Overviews 会在搜索结果顶部生成 AI 答案，每条回复引用 4-7 个来源链接；据 2026 年 5 月的数据，这些摘要出现在约 47%的美国搜索中。相关研究显示，AI Overviews 可使排名第一的普通搜索结果点击率下降 15%-30%，使内容网站流量减少 15%-40%。

reddit · r/artificial · NISMO1968 · 8月4日 11:13 · [社区讨论](https://www.reddit.com/r/artificial/comments/1vf7dob/as_reddit_stock_falls_ceo_questions_value_of/)

**背景**: Google AI Overviews 是集成在 Google 搜索中的人工智能功能，会在搜索结果顶部生成 AI 回答。该功能因错误信息、幻觉、减少网站流量以及无法选择退出而受到批评。包括 Reddit 在内的许多内容发布者依赖搜索引荐来获取受众和收入，因此直接在搜索结果中作答的 AI 摘要会威胁他们的流量和广告收入。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_Overviews">AI Overviews - Wikipedia</a></li>
<li><a href="https://growbydata.com/google-ai-overviews/">What Are Google AI Overviews? (2026 Guide with Examples)</a></li>
<li><a href="https://www.aeocheck.co/blog/google-ai-overviews-organic-traffic">How Google AI Overviews Affect Organic Traffic ... - AEOCheck</a></li>

</ul>
</details>

**社区讨论**: 评论整体负面且带有不满情绪。有用户辱骂 Reddit CEO（Spez）毁了平台，有人认为 Reddit 不应依赖第三方流量，应该做好站内搜索，还有人表示要离开 Reddit。

**标签**: `#AI`, `#Reddit`, `#Google`, `#AI Overviews`, `#Web Traffic`

---