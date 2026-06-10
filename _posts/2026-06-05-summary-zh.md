---
layout: default
title: "Horizon Summary: 2026-06-05 (ZH)"
date: 2026-06-05
lang: zh
---

> From 25 items, 14 important content pieces were selected

---

1. [Anthropic 发布开源 AI 漏洞发现测试框架](#item-1) ⭐️ 8.0/10
2. [VoidZero 加入 Cloudflare](#item-2) ⭐️ 8.0/10
3. [Anthropic 探讨 AI 递归自我改进的进展](#item-3) ⭐️ 8.0/10
4. [Meta 在雷朋智能眼镜上加入面部识别](#item-4) ⭐️ 8.0/10
5. [华为 KVarN：原生 vLLM 后端实现 KV 缓存量化](#item-5) ⭐️ 7.0/10
6. [复古科技育儿：为孩子精心选择技术](#item-6) ⭐️ 7.0/10
7. [欧盟版 Kagi 替代品 Uruky 新增图片搜索和 URL 重写功能](#item-7) ⭐️ 7.0/10
8. [高斯点溅射：扩展到大规模场景](#item-8) ⭐️ 7.0/10
9. [谷歌员工嘲讽自家 AI，公司撤回人类监督承诺](#item-9) ⭐️ 7.0/10
10. [休斯顿推出太阳能储能电力捆绑套餐，每千瓦时 6 美分](#item-10) ⭐️ 6.0/10
11. [日产与 Gelion 合作开发低成本固态电动汽车电池](#item-11) ⭐️ 6.0/10
12. [宝马 iX3 在 NAF 测试中创下 485 英里续航纪录](#item-12) ⭐️ 6.0/10
13. [xAI 一个月内为 AI 数据中心购买价值 2.69 亿美元的特斯拉 Megapack](#item-13) ⭐️ 6.0/10
14. [Waymo 将退役自动驾驶出租车电池用于电网储能](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Anthropic 发布开源 AI 漏洞发现测试框架](https://github.com/anthropics/defending-code-reference-harness) ⭐️ 8.0/10

Anthropic 在 GitHub 上发布了一个用于 AI 驱动漏洞发现的开源测试框架，该框架利用大型语言模型自动检测安全缺陷。 此次发布降低了安全研究人员尝试基于 AI 的漏洞发现的门槛，但专家评论指出，实际应用中仍需要大量定制且成本不菲。 该仓库标记为未维护且不接受贡献，成本估计根据使用的模型（Opus vs. Mythos）每次运行需数百至数千美元。

hackernews · binyu · Jun 4, 20:11 · [社区讨论](https://news.ycombinator.com/item?id=48403980)

**背景**: AI 驱动的漏洞发现测试框架通过编排多个 AI 代理来分析代码并识别安全漏洞。典型方法涉及一个编排器代理，根据执行日志分派专门的代理。Anthropic 的贡献作为一家领先 AI 公司的开源实现值得关注，尽管该领域仍处于早期阶段，需要定制化设置。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://undercodetesting.com/ai-zero-day-hunter-finding-undiscovered-vulnerabilities-for-0-per-codebase-with-open-source-orchestration-video/">AI Zero‑Day Hunter: Finding Undiscovered... - Undercode Testing</a></li>
<li><a href="https://thinkml.ai/9-ai-powered-vulnerability-assessment-tools-for-modern-pentesters/">9 AI -Powered Vulnerability Assessment Tools for Modern Pentesters</a></li>

</ul>
</details>

**社区讨论**: tptacek 和 baby 等专家强调，这类框架最好作为定制的灵感来源，而非即插即用的工具。simonw 提出成本问题，还有人指出该仓库已不再维护。

**标签**: `#AI`, `#security`, `#vulnerability discovery`, `#open-source`, `#frameworks`

---

<a id="item-2"></a>
## [VoidZero 加入 Cloudflare](https://blog.cloudflare.com/voidzero-joins-cloudflare/) ⭐️ 8.0/10

Cloudflare 收购了 VoidZero，这是一家开源公司，旗下拥有 Vite、Vitest 及其他 JavaScript 工具。VoidZero 团队将加入 Cloudflare，并设立 100 万美元基金以支持 Vite 生态系统。 此次收购将核心 Vite 团队及其广泛使用的构建工具纳入 Cloudflare 的基础设施，可能加速边缘前端的工具创新。同时，这也引发了关于大型企业收购后开源项目独立性的疑问。 Cloudflare 承诺投入 100 万美元用于独立的 Vite 生态系统基金。公告称，这些工具将继续保持开源和供应商中立。

hackernews · coloneltcb · Jun 4, 13:00 · [社区讨论](https://news.ycombinator.com/item?id=48398055)

**背景**: Vite 是一个现代 JavaScript 构建工具，以其快速的开发服务器和优化的生产构建而闻名，在前端社区中得到广泛采用。VoidZero 是维护 Vite、Vitest 及相关工具的公司，由 Vue.js 创始人尤雨溪创立。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cloudflare.com/press/press-releases/2026/cloudflare-acquires-voidzero-to-build-the-future-of-the-ai-native-web/">Cloudflare Acquires VoidZero to Build the Future of the AI ...</a></li>
<li><a href="https://www.morningstar.com/news/business-wire/20260604108073/cloudflare-acquires-voidzero-to-build-the-future-of-the-ai-native-web">Cloudflare Acquires VoidZero to Build the Future of the AI ...</a></li>
<li><a href="https://www.heise.de/en/news/Cloudflare-acquires-VoidZero-Team-behind-Vite-switches-completely-11319023.html">Cloudflare acquires VoidZero – Team behind Vite switches ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论情绪复杂：有人赞赏 Vite 的历史和团队，但许多人对收购模式及 Cloudflare 领导下的优先级变化感到不安。对继续独立和供应商中立的承诺仍存怀疑。

**标签**: `#web development`, `#JavaScript`, `#Vite`, `#Cloudflare`, `#acquisitions`

---

<a id="item-3"></a>
## [Anthropic 探讨 AI 递归自我改进的进展](https://www.anthropic.com/institute/recursive-self-improvement) ⭐️ 8.0/10

Anthropic 发布了一篇文章，详细介绍了他们在 AI 递归自我改进方面的进展，其中像 Claude 这样的模型能够生成并改进代码以增强自身能力。 递归自我改进可能导致智能爆炸，使 AI 系统能力大幅提升，甚至可能超越人类控制，引发关键的安全和对齐问题。 文章指出，虽然 AI 现在可以编写自己大部分代码并持续改进，但循环中的关键部分仍由人类控制，而且这一进展尚未在 AI 领域之外产生突破。

hackernews · meetpateltech · Jun 4, 16:20 · [社区讨论](https://news.ycombinator.com/item?id=48400842)

**背景**: 递归自我改进（RSI）是 AI 系统重写自身代码以变得更强大的过程，可能导致快速的智能爆炸。这一概念引发了重大的伦理和安全担忧，因为此类系统可能不可预测地进化，并超越人类的理解或控制。Anthropic 作为一家 AI 安全公司，一直在代码生成和自我修改的背景下探索 RSI。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement</a></li>
<li><a href="https://spectrum.ieee.org/recursive-self-improvement">Recursive Self-Improvement Edges Closer In AI Labs - IEEE Spectrum</a></li>

</ul>
</details>

**社区讨论**: 社区评论持怀疑态度：用户指出可靠性问题（服务中断、API 错误），并质疑除了 vibe coding 之外缺乏突破。有人认为全力追求 RSI 与 Anthropic 宣称的安全目标相矛盾，还有人嘲讽 Anthropic 将模型命名为“Mythos”（源自洛夫克拉夫特式恐怖），暗示品牌与安全理念脱节。

**标签**: `#AI`, `#recursive self-improvement`, `#AI safety`, `#Anthropic`, `#code generation`

---

<a id="item-4"></a>
## [Meta 在雷朋智能眼镜上加入面部识别](https://www.buchodi.com/meta-glasses-facial-recognition/) ⭐️ 8.0/10

Meta 已在雷朋智能眼镜上推出面部识别功能，使用户能够识别所看到的人。 此举重新引发了关于可穿戴摄像头和生物识别数据的隐私担忧和伦理争论，重蹈十年前谷歌眼镜的争议。 据报道，该功能需要互联网连接并使用 Meta 的云端 AI，引发了对数据存储和同意的疑问。

hackernews · buchodi · Jun 4, 19:36 · [社区讨论](https://news.ycombinator.com/item?id=48403588)

**背景**: 面部识别技术通过分析面部特征来识别或验证个人。Meta 是一家有隐私争议历史的社交媒体巨头。雷朋智能眼镜是一种消费级可穿戴设备，可以免提拍摄照片和视频。

**社区讨论**: 评论表达了不同的反应：有人希望离线使用以辅助识别面孔失认症，也有人担心隐私侵犯。评论提及过去谷歌眼镜开发者限制的对比，并强调了对 Meta 隐私记录的担忧。

**标签**: `#facial recognition`, `#privacy`, `#meta`, `#smart glasses`, `#ethics`

---

<a id="item-5"></a>
## [华为 KVarN：原生 vLLM 后端实现 KV 缓存量化](https://github.com/huawei-csl/KVarN) ⭐️ 7.0/10

华为发布了 KVarN，这是一个开源的、原生于 vLLM 的 KV 缓存量化后端，声称其性能优于 TurboQuant（TQ），质量优于 FP16。 KV 缓存量化对于减少 LLM 推理中的内存占用至关重要；KVarN 声称的改进可以在不牺牲质量的情况下实现更长的上下文长度和更高的吞吐量。 KVarN 是一个原生的 vLLM 后端，意味着它与 vLLM 的架构直接集成，并在华为-CSL 组织下开源在 GitHub 上。该项目仍处于早期阶段，尚未合并到主流 vLLM 中。

hackernews · theanonymousone · Jun 4, 15:18 · [社区讨论](https://news.ycombinator.com/item?id=48399974)

**背景**: KV 缓存量化减少了 LLM 推理过程中存储键值缓存所需的内存，从而支持更长的上下文长度。vLLM 是一个流行的高吞吐量 LLM 推理引擎，支持多种量化方法。TurboQuant（TQ）是谷歌最近推出的一种量化算法，可实现极致压缩。KVarN 旨在结合两者的优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/features/quantization/quantized_kvcache/">Quantized KV Cache - vLLM</a></li>
<li><a href="https://github.com/0xSero/turboquant">GitHub - 0xSero/turboquant: TurboQuant: Near-optimal KV cache ...</a></li>

</ul>
</details>

**社区讨论**: 社区反应好奇且怀疑。有评论者询问是否看对了，KVarN 声称性能优于 TQ 且质量优于 FP16。另一人质疑为何不向 vLLM 提交 PR，还有一人用中文赞赏其遥遥领先。

**标签**: `#LLM inference`, `#KV-cache quantization`, `#vLLM`, `#Huawei`, `#open-source`

---

<a id="item-6"></a>
## [复古科技育儿：为孩子精心选择技术](https://havenweb.org/2026/05/28/retro-tech.html) ⭐️ 7.0/10

一位家长分享了他们为孩子提供复古技术的做法——包括书籍、离线笔记本电脑和机器人套件——引发了社区关于有意使用技术育儿的讨论。 这种方法为现代广告驱动平台提供了实用的替代方案，帮助孩子培养独立性、创造力，并对技术的演变有扎实的理解。 这位家长的具体选择包括一台无互联网连接的 2012 年 MacBook Pro、乐高 Spike 机器人套件和超过 1500 本书。社区成员还建议使用复古游戏、固定电话，并观察技术随时间的发展。

hackernews · mawise · Jun 4, 16:02 · [社区讨论](https://news.ycombinator.com/item?id=48400588)

**背景**: 复古科技育儿是指使用较旧、更可控的技术，为孩子提供丰富的体验，同时避免现代在线平台的负面影响。这一趋势已引起关注，因为家长希望平衡数字接触与动手学习和家庭联系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://havenweb.org/2026/05/28/retro-tech.html">Haven Blog: Retro-Tech Parenting</a></li>
<li><a href="https://flipso.com/p/yswx16r8b?ref=rss">Retro-Tech Parenting · Flipso</a></li>
<li><a href="https://www.businessinsider.com/millennial-mom-shares-nostalgic-parenting-vhs-tin-can-trading-cards-2026-1?op=1">I'm Raising My Kids on '90s and Retro-Style Tech. They Love It ...</a></li>

</ul>
</details>

**社区讨论**: 评论普遍支持这种有意为之的方式，许多家长分享了他们自己的例子，如复古游戏机和社区 PBX 系统。一个反复出现的主题是，体验技术的进步有助于孩子理解核心原理。

**标签**: `#parenting`, `#retro-tech`, `#education`, `#technology`, `#community`

---

<a id="item-7"></a>
## [欧盟版 Kagi 替代品 Uruky 新增图片搜索和 URL 重写功能](https://uruky.com/?il=en) ⭐️ 7.0/10

Uruky，一款基于欧盟的付费搜索引擎，作为 Kagi 的替代品，现已支持图片搜索和 URL 重写。它还通过工作量证明验证码提供 2 小时免费试用。 这一扩展使 Uruky 成为 Kagi 更具竞争力的替代品，尤其对注重隐私的欧盟用户而言。但社区指出，它在 UI/UX 和功能对等方面仍有差距，这可能限制其普及。 Uruky 计划采用 PolyForm Shield 源代码可用许可证（禁止竞争）共享源代码，并考虑取消 NDA 要求。该公司已超过 100 个月活跃账户，并计划向 12 个月以上的账户提供代码下载。

hackernews · BrunoBernardino · Jun 4, 08:56 · [社区讨论](https://news.ycombinator.com/item?id=48396004)

**背景**: Uruky 是一款注重隐私、基于欧盟的付费搜索引擎，定位为 Kagi 的替代品。Kagi 是一款流行的付费搜索引擎，以简洁的 UI 和高级功能著称。Uruky 使用工作量证明验证码来验证用户而不进行追踪，并计划采用源代码可用许可证，在透明度和商业保护之间取得平衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Proof_of_work">Proof of work - Wikipedia</a></li>
<li><a href="https://polyformproject.org/licenses/shield/1.0.0">PolyForm Shield License 1.0.0 - Polyform Project</a></li>
<li><a href="https://altcha.org/docs/v2/proof-of-work-captcha/">Proof Of Work Captcha | ALTCHA</a></li>

</ul>
</details>

**社区讨论**: 社区反馈不一：有人称赞其欧盟隐私保护重点，但批评 UI/UX 对非技术用户不够友好。其他人则将其与 Kagi 进行功能对比（缺少 AI 回复、小部件、索引），并询问搜索结果来源。总体而言，态度是谨慎支持，但要求大幅改进。

**标签**: `#search engine`, `#privacy`, `#EU`, `#Kagi alternative`, `#image search`

---

<a id="item-8"></a>
## [高斯点溅射：扩展到大规模场景](https://momentsingraphics.de/Siggraph2026.html) ⭐️ 7.0/10

研究人员提出高斯点溅射，一种随机渲染方法，从高斯采样不透明点并使用 64 位原子操作渲染大规模 3D 高斯溅射场景，无需排序或基于瓦片的渲染。 该技术显著提升了包含大量高斯场景的可扩展性，实现了大规模 3D 场景的实时渲染且质量损失极小，有望推动游戏、VR 和 3D 可视化等领域的进步。 该方法通过采样像素大小的不透明点并应用随机透明度，消除了排序和基于瓦片渲染的需求。它基于 Inria 团队在 2023 年提出的开创性 3D 高斯溅射技术，并将在 SIGGRAPH 2026 上展示。

hackernews · ibobev · Jun 4, 10:48 · [社区讨论](https://news.ycombinator.com/item?id=48396792)

**背景**: 传统 3D 渲染使用网格和多边形，计算成本较高。高斯溅射将场景表示为 3D 高斯原语的集合，为新颖视图合成提供了更快的渲染。然而，由于内存和排序要求，扩展到大量高斯场景一直具有挑战性。高斯点溅射通过采样点而非渲染完整高斯来解决这一问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://momentsingraphics.de/Siggraph2026.html">Gaussian Point Splatting - momentsingraphics.de</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gaussian_splatting">Gaussian splatting - Wikipedia</a></li>
<li><a href="https://jorisar.nl/gaussian_point_splatting/">Gaussian Point Splatting - jorisar.nl</a></li>

</ul>
</details>

**社区讨论**: 评论表达了对将该技术应用于 AAA 游戏的兴趣，并与 1994 年使用椭球溅射的游戏《Ecstatica》进行了比较。一些用户指出高斯溅射已经掩盖了较旧的点溅射技术，并请求教程。一位评论者将其与网格溅射进行比较，认为网格可能更擅长表示锐利特征。

**标签**: `#computer graphics`, `#rendering`, `#gaussian splatting`, `#3D visualization`

---

<a id="item-9"></a>
## [谷歌员工嘲讽自家 AI，公司撤回人类监督承诺](https://simonwillison.net/2026/Jun/4/a-slightly-different-version/#atom-everything) ⭐️ 7.0/10

谷歌员工内部传播嘲讽自家 AI 性能低下的表情包，随后谷歌撤回了此前关于“将人类置于反馈循环中至关重要”的声明。 这一事件揭示了谷歌内部对其 AI 质量的怀疑态度，以及公司在人类监督问题上令人担忧的透明度转变，引发了关于 AI 伦理和问责制的重要问题。 最初的声明强调了人类参与反馈循环的重要性，但在媒体报道后，谷歌发言人要求发布删除了这一承诺的修订版本。

rss · Simon Willison · Jun 4, 16:38

**背景**: “人类参与反馈循环”是 AI 开发中的一项原则，旨在通过人类监督来捕捉错误并确保合乎道德的操作。谷歌等公司经常公开承诺此类做法，但内部表情包和声明修改暗示了言辞与现实之间的差距。

**标签**: `#ai-ethics`, `#google`, `#ai`, `#journalism`, `#human-in-the-loop`

---

<a id="item-10"></a>
## [休斯顿推出太阳能储能电力捆绑套餐，每千瓦时 6 美分](https://electrek.co/2026/06/04/houston-solar-storage-electricity-bundle-6-cents-per-kwh/) ⭐️ 6.0/10

Terra Energy 推出了 TerraOne，这是一项为期三年的订阅服务，将屋顶太阳能、最高 40 千瓦时的电池储能和电力服务捆绑在一起，固定费率为每千瓦时 6 美分，无需前期费用或贷款。 这一低价捆绑套餐可能使休斯顿更多房主用上太阳能加储能，有望加速可再生能源普及，并在电力市场放松管制的地区挑战传统公用事业模式。 TerraOne 订阅为期三年，包含一个 40 千瓦时电池用于全屋备用，整个捆绑套餐的固定电价为每千瓦时 6 美分。无需前期费用、贷款或留置权。

rss · Electrek · Jun 4, 19:42

**背景**: 传统上，住宅太阳能和电池系统需要大笔前期投资或长期贷款，这对许多房主来说是一大障碍。将这些与电力服务捆绑成订阅模式，降低了财务门槛并简化了客户体验。休斯顿处于得克萨斯州电力市场放松管制的环境中，允许零售电力供应商提供此类创新计划。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.morningstar.com/news/business-wire/20260604683487/terra-energy-launches-lowest-cost-home-energy-plan-in-houston-for-bundled-solar-battery-backup-and-retail-electricity">Terra Energy Launches Lowest-Cost Home Energy Plan in Houston for Bundled Solar, Battery Backup, and Retail Electricity | Morningstar</a></li>
<li><a href="https://electrek.co/2026/06/04/houston-solar-storage-electricity-bundle-6-cents-per-kwh/">Houston gets a solar, storage + electricity bundle for 6¢ per kWh | Electrek</a></li>

</ul>
</details>

**标签**: `#solar`, `#energy storage`, `#renewable energy`, `#electricity`

---

<a id="item-11"></a>
## [日产与 Gelion 合作开发低成本固态电动汽车电池](https://electrek.co/2026/06/04/nissan-solid-state-ev-battery-project-aims-for-cheaper-than-china/) ⭐️ 6.0/10

日产宣布与 Gelion 开展为期三年的合作，共同开发低成本固态电动汽车电池，目标是在价格上超越中国制造商。该项目利用了 Gelion 的纳米封装硫阴极技术。 此次合作有助于非中国汽车制造商减少对亚洲电池供应商的依赖并降低电动汽车成本，可能重塑全球电池供应链。固态电池具有更高的能量密度和安全性，对电动汽车的大规模普及至关重要。 合作聚焦于固态电解质和 Gelion 的硫基阴极技术以实现成本目标。Gelion 在伦敦证券交易所 AIM 上市，2015 年从悉尼大学孵化，专注于锂硫和锌溴储能技术。

rss · Electrek · Jun 4, 17:26

**背景**: 固态电池用固体材料取代液体电解质，具有更高的能量密度、更好的安全性和更长的寿命。它们被视为电动汽车的下一个前沿，但生产成本高昂。中国制造商目前主导全球电池市场，促使日产等汽车制造商寻求价格合理的替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://electrek.co/2026/06/04/nissan-solid-state-ev-battery-project-aims-for-cheaper-than-china/">Nissan solid-state EV battery project aims for 'Cheaper Than ...</a></li>
<li><a href="https://gelion.com/">Next-Generation Sulfur Battery Technologies | Gelion</a></li>
<li><a href="https://battery-tech.net/company/gelion/">Gelion - Battery-Tech Network</a></li>

</ul>
</details>

**标签**: `#solid-state batteries`, `#EV`, `#battery technology`, `#Nissan`

---

<a id="item-12"></a>
## [宝马 iX3 在 NAF 测试中创下 485 英里续航纪录](https://electrek.co/2026/06/04/bmws-new-ix3-drove-485-miles-longest-range-ev-naf-test/) ⭐️ 6.0/10

宝马新款 iX3 在一次充电后行驶了 485 英里，在 NAF 和 Motor 的夏季续航测试中成为续航最长的电动汽车。 这一里程碑表明宝马的新一代电动车平台可以超越卢西德和特斯拉等当前续航领先者，可能改变消费者对宝马电动车的偏好。 NAF 测试以真实驾驶条件著称，因此 485 英里的结果反映了现实续航而非乐观的实验室数据。iX3 很可能采用了宝马的第六代圆柱电池技术。

rss · Electrek · Jun 4, 14:26

**背景**: NAF（挪威汽车联合会）每年夏季和冬季进行续航测试，被公认为全球最真实的电动车续航评估之一。宝马 iX3 是 2025 年推出的基于 Neue Klasse 平台的全电动 SUV。此前 NAF 测试的续航纪录由卢西德 Air Grand Touring 保持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.naf.no/elbil/elprix">El Prix 2026 – verdens største elbiltest | NAF</a></li>
<li><a href="https://insideevs.com/news/762220/summer-group-range-test-norway/">This Big EV Range Test In Norway Had A Winner, In A Strange Way</a></li>

</ul>
</details>

**标签**: `#electric vehicles`, `#BMW`, `#range test`, `#automotive`

---

<a id="item-13"></a>
## [xAI 一个月内为 AI 数据中心购买价值 2.69 亿美元的特斯拉 Megapack](https://electrek.co/2026/06/04/spacex-xai-269-million-tesla-megapack-purchase-s1-filing/) ⭐️ 6.0/10

SpaceX 修改后的 S-1 上市文件显示，xAI 在 2026 年 4 月单月内又购买了价值 2.69 亿美元的特斯拉 Megapack 产品，使得自 2024 年以来对 Megapack 的总支出达到约 10 亿美元。 这笔巨额储能投资凸显了 AI 数据中心巨大的电力消耗，并强调了埃隆·马斯克旗下公司之间日益加深的业务联系，对电网和可再生能源整合具有重要意义。 单月 2.69 亿美元的支出超过了 xAI 在 2024 年全年的 Megapack 总支出。这些采购是 xAI 建设 Colossus 超级计算机的一部分，该计算机需要大量电力。

rss · Electrek · Jun 4, 12:58

**背景**: 特斯拉 Megapack 是一种大型锂离子电池储能系统，专为电网和公用事业用途设计，每台可储存高达 3.9 MWh 的电量。AI 数据中心（例如 xAI 运营的数据中心）需要大量能源，因此现场电池存储对于稳定供电和降低成本至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Megapack">Tesla Megapack</a></li>
<li><a href="https://www.tesla.com/megapack">Megapack - Tesla</a></li>

</ul>
</details>

**标签**: `#AI`, `#Energy`, `#Tesla`, `#SpaceX`, `#Data Centers`

---

<a id="item-14"></a>
## [Waymo 将退役自动驾驶出租车电池用于电网储能](https://electrek.co/2026/06/04/waymo-retired-robotaxi-batteries-are-heading-back-to-work-b2u/) ⭐️ 6.0/10

Waymo 宣布，其自动驾驶出租车车队中退役的电池将被重新利用，用于支持加利福尼亚州和得克萨斯州的电网，而不是立即进行回收。 这一举措展示了电动汽车电池二次利用的实际应用场景，有望减少电池浪费，并为电网提供低成本储能方案。 这些重新利用的电池将被部署在加利福尼亚和得克萨斯州的固定式储能系统中，但具体合作方、容量和时间表尚未公布。

rss · Electrek · Jun 4, 11:00

**背景**: 电动汽车电池在车用寿命结束后通常仍保留 70%-80%的容量，使其适用于要求较低的固定式储能。其他汽车制造商也曾探索过电池二次利用项目，但 Waymo 庞大的自动驾驶出租车车队提供了源源不断的退役电池组，进一步验证了该模式。

**标签**: `#EV batteries`, `#grid storage`, `#Waymo`, `#robotaxi`, `#energy`

---