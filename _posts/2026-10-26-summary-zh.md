---
layout: default
title: "Horizon Summary: 2026-10-26 (ZH)"
date: 2026-10-26
lang: zh
---

> 从 53 条内容中筛选出 17 条重要资讯。

---

1. [Lean-QwenFlash 让 125B 的 Qwen3.8-Flash-Next 在 16GB 显存加 8GB 内存下跑到约 20 tok/s](#item-1) ⭐️ 8.0/10
2. [十年前的 CNN 在皮肤癌诊断上胜过前沿大模型](#item-2) ⭐️ 7.0/10
3. [尤金警方对一名警官的记录报价 250 万美元](#item-3) ⭐️ 7.0/10
4. [菲尔兹奖得主博切尔兹称：AI 让批改数学作业失去意义](#item-4) ⭐️ 7.0/10
5. [Cerebras 详解在晶圆级硬件上部署万亿参数模型](#item-5) ⭐️ 7.0/10
6. [南壁开源 Nanbeige4.3-33B：33B Apache 2.0 智能体教师模型](#item-6) ⭐️ 7.0/10
7. [MemT-1.0 架构解析：门控 DeltaNet-2 与混合存储打造智能体记忆](#item-7) ⭐️ 7.0/10
8. [改装版 RTX 3080 20GB 解锁 P2P 与 ReBAR，vLLM 预填充提速最高 115%](#item-8) ⭐️ 7.0/10
9. [HTMX 作者 Carson Gross 称业界误解了 REST 的本意](#item-9) ⭐️ 7.0/10
10. [Izwi 0.1.0 发布：跨平台全本地语音 AI 应用](#item-10) ⭐️ 7.0/10
11. [Solidigm 撤回 IPO，新云厂商信用利差走阔，超大规模厂商财报成焦点](#item-11) ⭐️ 7.0/10
12. [FOSDEM 27 演讲呼吁拒绝接受被审查的互联网，引发热议](#item-12) ⭐️ 6.0/10
13. [DreamHost 因文件管理器安全事件强制用户重置密码](#item-13) ⭐️ 6.0/10
14. [JetBrains 实验性智能体 IDE「ThinkRail」引发战略质疑](#item-14) ⭐️ 6.0/10
15. [Claude 拦截“逆向工程一切”工作流，再度引发护栏争议](#item-15) ⭐️ 6.0/10
16. [Reddit 提醒：在 Hugging Face 删除前备份量化模型](#item-16) ⭐️ 6.0/10
17. [开发者预览 4B Qwen3.5 微调模型：兼顾编程与 3D 场景生成](#item-17) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Lean-QwenFlash 让 125B 的 Qwen3.8-Flash-Next 在 16GB 显存加 8GB 内存下跑到约 20 tok/s](https://www.reddit.com/r/LocalLLaMA/comments/1xev6bo/leanqwenflash_qwen38flashnext_125b_running_at_20/) ⭐️ 8.0/10

一位 Reddit 用户（MaxDev0）发布了 lean-qwenflash 项目，把 sybil-solutions 的 glm-flash-lite 中的 NVMe 卸载设计移植到了 125B 参数的稀疏 MoE 模型 Qwen3.8-Flash-Next 上。在仅有 16GB 显存和 8GB 系统内存的 RTX 4090 上，配合 3.05bpw 的 EXL3 量化和 Q4 KV 缓存，它在 100k 至 262k 上下文下仍能维持约 20 tok/s 的解码速度。 目前 Qwen3.8-Flash-Next 的常见方案（如 Strata）会把全部 2.4 万个专家常驻在系统内存中，占用约 48–64GB，普通台式机和笔记本基本无缘。该方法把内存需求压到 8GB，改为从 NVMe SSD 按需流式加载专家，使 125B 级别的模型能在主流消费级硬件上运行，对本地 LLM 社区而言是很有价值的实用进展。 公布的基准数据包括：8k 上下文下散文类生成 28–33 tok/s、代码 19–22 tok/s，预填充约 1,080 tok/s；100k 上下文下解码 20.8 tok/s、预填充约 1,536 tok/s；在完整的 262k 窗口下解码 20.0 tok/s、预填充约 1,627 tok/s。一台配备 16GB 显存和 32GB 内存的 RTX 3080 笔记本在 100k 上下文下达到约 18–21 tok/s 解码和约 650–700 tok/s 预填充，峰值显存占用 15.5GB。整套方案依赖 turboderp 的 ExLlamaV3 运行时和 3.05bpw\_h5\_ng5 的 EXL3 量化包，安装说明、模型下载器和打包脚本均已发布在 GitHub 上。

reddit · r/LocalLLaMA · /u/MaxDev0 · 10月25日 06:41

**背景**: Qwen3.8-Flash-Next 是一个稀疏混合专家（MoE）模型，总参数 125B，但每个 token 仅激活约 6B 参数，另有 51B 参数的 n-gram 嵌入表不放在加速器上，并支持 262K 原生上下文。由于 MoE 推理必须让所有专家都可用，而每个 token 只用到其中少数几个，本地用户真正的瓶颈通常是内存容量而非算力。NVMe 卸载的思路就是把大部分专家存放在高速 SSD 上，按需把需要的专家流式载入显存，用存储带宽换取内存空间。EXL3 是 ExLlamaV3 的量化格式，其中 bpw 指每权重比特数，3.05bpw 属于相当激进的量化，可把模型体积压缩到消费级硬件能承受的范围。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/QwenLM/Qwen3.8-Flash-Next/">Qwen3.8-Flash-Next - GitHub</a></li>
<li><a href="https://arxiv.org/abs/2608.30320">[2608.30320] On the Design of Qwen3.8-Next Architecture ...</a></li>
<li><a href="https://huggingface.co/doth4580/Qwen3.8-Flash-Next-EXL3-3.05bpw">doth4580/Qwen3.8-Flash-Next-EXL3- 3 . 05 bpw · Hugging Face</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#model-inference`, `#nvme-offloading`, `#quantization`, `#qwen`

---

<a id="item-2"></a>
## [十年前的 CNN 在皮肤癌诊断上胜过前沿大模型](https://lynchlab.net/llm-skin-cancer) ⭐️ 7.0/10

皮肤科医生 Magnus Lynch 测试了 GPT-6 Astra 和 Claude Fable 5.1 在皮肤癌诊断上的表现，发现两者的准确率都低于他的预期，而一个十年前训练、经微调的 Inception v3 卷积神经网络反而更胜一筹。该对比结果于 2026 年 10 月 25 日发布在其实验室网站上，测试使用了 200 个病灶的留出集，这些样本已从 CNN 的训练集和验证集中完全剔除。 这一结果加剧了一场争论：在专业医疗任务上，究竟应直接使用通用前沿大模型，还是专用的小模型仍是更优的工程选择。同时它也引出方法学层面的疑问——大模型的医疗基准该如何构建，以及一个基于单一数据集的小规模对比应当被赋予多大权重。 该 CNN 采用在普通照片上预训练的 Inception v3，并在单块 H100 GPU 上对来自 ISIC Archive 的 68,011 张皮肤镜与临床图像进行了全层微调；200 个测试病灶及同一患者的所有图像都已从训练集和验证集中移除，测试集也未用于模型选择或阈值设定。不过该对比规模较小（仅 200 个病灶）、来源单一数据集，且只评估纯图像分类，未纳入病史、元数据或临床背景信息。

hackernews · sungam · 10月25日 17:15 · [社区讨论](https://news.ycombinator.com/item?id=50233779)

**背景**: 卷积神经网络（CNN）是一类专为图像数据设计的深度学习模型，Inception v3 是 2015 年前后广泛使用的图像分类架构。微调是指先在大规模通用数据集上预训练网络，再用较小的任务专用数据集继续训练，这也是大多数医学影像模型的构建方式。ISIC Archive 是由国际皮肤影像协作组织维护的大型公开皮肤图像库，基于它构建的 HAM10000 等数据集已成为皮肤病灶分类的标准基准。相比之下，前沿大语言模型是通用模型，训练数据以广泛的文本与多模态数据为主，而非经过整理的皮肤病学图像集。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lynchlab.net/llm-skin-cancer">A 10-year-old CNN outperforms frontier LLMs for skin cancer ...</a></li>
<li><a href="https://www.nature.com/articles/sdata2018161">The HAM10000 dataset, a large collection of multi-source ...</a></li>
<li><a href="https://www.isic-archive.com/">ISIC | International Skin Imaging Collaboration</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为这一结果并不意外：有人将其比作参数仅 3000 万的 KataGo 网络能在围棋上超越人类，而参数量大上万倍的大模型却下不好围棋；也有人指出计算器在乘除法上同样胜过 LLM。一个重要的反驳观点认为，这个 CNN 的结果本质上是“刷榜”（benchmaxxing）——专门针对该基准调优的模型自然会赢；另一些人则认为该对比忽略了 LLM 的真正潜力，例如结合病历记录、主动向患者追问信息，或处理纹身等分布外图像。还有评论指出，LLM 恰恰让构建专用分类器的成本降到极低。

**标签**: `#AI/ML`, `#medical imaging`, `#LLMs`, `#specialized models`, `#benchmark evaluation`

---

<a id="item-3"></a>
## [尤金警方对一名警官的记录报价 250 万美元](https://theintercept.com/2026/10/01/oregon-police-misconduct-public-records-cost-fee/) ⭐️ 7.0/10

尤金警察局估计，处理本地媒体 Double Sided Media 就警官 Justin Peckels 的持续不当行为记录提出的公共记录请求，需要 44,816 个员工工时，费用为 2,484,599.04 美元。另一项针对前警官 Eric Klinko 的类似请求被报价 195,869.52 美元，两项合计接近 270 万美元。 这一报价把常规的透明度请求变成了事实上的障碍，因为如此高昂的费用可能让新闻机构无力承担，并使警方不当行为记录逃避公众监督。它还凸显出，州级公共记录制度可以在不正式拒绝公开的情况下，被用来阻碍新闻自由和问责报道。 44,816 小时的估算相当于一个人约 21 年的全职工作量，而俄勒冈州公共记录法允许机构收取员工工时费用，新闻媒体并不自动获得费用豁免。该请求寻求的是持续不当行为记录，因此这一成本估算直接关系到公众能否了解涉事警官的纪律处分历史。

hackernews · tdeck · 10月25日 18:04 · [社区讨论](https://news.ycombinator.com/item?id=50234232)

**背景**: FOIA 是美国联邦《信息自由法》，但针对地方警察的大多数请求实际上受俄勒冈州等州级公共记录法管辖。这类法律通常允许机构向请求者收取处理请求所需的员工工时费和复制费，而围绕费用和拖延的争议一直是开放政府斗争的长期主题。Double Sided Media 是一家位于尤金的地方媒体，正在寻求有关当地警察行为的记录。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://theintercept.com/2026/10/01/oregon-police-misconduct-public-records-cost-fee/">Oregon Police Are Charging a Local News Outlet $2.5M for ...</a></li>
<li><a href="https://lookouteugene-springfield.com/story/justice/2026/10/09/epds-2-5-million-estimate-to-fulfill-public-records-request-prompts-discussion/">EPD&#x27;s $2.5 million estimate to fulfill public records request ...</a></li>
<li><a href="https://eugeneweekly.com/2016/05/26/hide-and-seek/">Hide And Seek - Eugene Weekly</a></li>

</ul>
</details>

**社区讨论**: 评论者谴责这一估算荒谬，指出 44,816 小时约等于 21 年的工作量，并分享了机构拖延请求或设置高得令人望而却步的费用的经历。有人将美国制度与英国 FOIA 30 天答复的规定对比，并警告德国正在讨论类似的收费限制；还有人提到 2015 年国防部曾报价 1500 万小时和 6.6 亿美元。

**标签**: `#FOIA`, `#public records`, `#government transparency`, `#press freedom`, `#police accountability`

---

<a id="item-4"></a>
## [菲尔兹奖得主博切尔兹称：AI 让批改数学作业失去意义](https://www.dailycal.org/news/campus/academics/ai-use-leads-uc-berkeley-math-professor-to-see-no-point-in-grading-homework/article_bdf1eae2-c08b-491f-b9f1-81a7cea177de.html) ⭐️ 7.0/10

据《Daily Cal》报道，加州大学伯克利分校数学教授、菲尔兹奖得主理查德·博切尔兹（Richard Borcherds）公开表示，AI 已经让批改作业变得毫无意义；该报道在 Hacker News 上引发热议，帖子获得 184 分、267 条评论。这是一位知名数学家罕见地不是去“抓作弊”，而是直接质疑作业评分这一长期教学惯例本身的价值。 当一位菲尔兹奖得主断言评分作业已无法衡量任何东西时，这为“大学必须围绕线下考试、口头答辩或抗 AI 任务重新设计评估方式”提供了有力论据。这一转变将影响全球数学系如何安排课程作业、教师如何判断学生是否真正掌握知识，以及学生如何养成作业本应培养的循序渐进的练习习惯。 有评论者指出其中的讽刺之处：博切尔兹本人恐怕多年没有亲自批改过作业，因为拥有科研经费的终身教授通常把批改工作交给研究生助教。讨论还强调，真正的损失不只是作弊，而是那种在考试前迫使学生循序渐进接触材料的“强制机制”消失了。

hackernews · romanhn · 10月25日 16:28 · [社区讨论](https://news.ycombinator.com/item?id=50233304)

**背景**: 理查德·博切尔兹因证明“魔群月光”（Monstrous Moonshine）猜想而获得 1998 年菲尔兹奖，该猜想揭示了模函数与魔群之间的深刻联系。如今 GPT 级别的大语言模型已能解出许多常规的本科数学习题，这动摇了“课外完成的作业能反映学生自身理解水平”这一传统假设。长期以来，作业评分既是一种促进学习的过程性工具，也是课程总评成绩的组成部分。

**社区讨论**: Hacker News 上的讨论颇具实质内容而非情绪化反应：一些评论者为作业辩护，认为即便存在合作或抄袭，作业仍是一种迫使学生接触材料的强制机制；另一些人则认为对大学生而言，仅凭考试就足以判定掌握程度。多位评论者提到这位教授本人从不亲自批改作业的讽刺之处，还有人主张高等教育应回归学术本身，而非职业技能培训。

**标签**: `#AI in education`, `#LLMs`, `#academic integrity`, `#grading`, `#higher education`

---

<a id="item-5"></a>
## [Cerebras 详解在晶圆级硬件上部署万亿参数模型](https://www.cerebras.ai/blog/how-we-deploy-trillion-parameter-frontier-models-on-cerebras) ⭐️ 7.0/10

Cerebras 发布技术博客，详细说明如何在其晶圆级硬件上部署万亿参数前沿 AI 模型，展示了一条不依赖 GPU 集群的推理路径。 以低延迟服务万亿参数模型是 AI 基础设施中最困难的工作负载之一，因此可用的晶圆级部署将增强 Cerebras 相对 GPU 云服务的竞争力，并可能改变前沿推理算力的采购与定价方式。 Cerebras 的 WSE-3 由几乎整片 300 毫米晶圆制成，边长约 21.5 厘米，其内存与互连架构与传统 GPU 截然不同；不过评论者指出，大规模复制这种算力需要极强的制造能力，可能限制服务的普及程度。

hackernews · gmays · 10月25日 01:33 · [社区讨论](https://news.ycombinator.com/item?id=50227356)

**背景**: Cerebras Systems 以晶圆级芯片著称，其 Wafer-Scale Engine（WSE）把整片硅晶圆作为一个大芯片使用，而不是切割成许多小裸片。该公司销售 CS 系列系统，并提供推理云服务，让客户无需购买硬件即可使用其算力。万亿参数模型属于规模最大的大语言模型，需要巨大的内存和计算资源，因此实现快速服务是一项重大的基础设施挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cerebras">Cerebras Systems - Wikipedia</a></li>
<li><a href="https://www.cerebras.ai/chip">Cerebras WSE - 3 Turbo | Wafer - Scale AI Chip</a></li>
<li><a href="https://spectrum.ieee.org/cerebras-chip-cs3">Cerebras WSE - 3 : Third Generation Superchip for AI - IEEE Spectrum</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者大多赞赏 Cerebras 的工程技术，但怀疑其能否制造足够多的晶圆级硬件来满足需求；一些人抱怨实际可访问的模型虽然速度快，却过时或容易出错。也有人预计更新模型很快会推出，并对芯片的二维网格通信以及公司的招聘与执行力提出更深层疑问。

**标签**: `#AI infrastructure`, `#wafer-scale computing`, `#LLM inference`, `#hardware`, `#Cerebras`

---

<a id="item-6"></a>
## [南壁开源 Nanbeige4.3-33B：33B Apache 2.0 智能体教师模型](https://www.reddit.com/r/MachineLearning/comments/1xf6x35/nanbeige_releases_nanbeige4333b_an_apache_20/) ⭐️ 7.0/10

南壁（Nanbeige）发布了 Nanbeige4.3-33B，这是一个采用 Apache 2.0 许可的 33B 稠密开源权重模型，支持 512K（524,288 token）上下文窗口，定位为其后续更小智能体（包括即将推出的 3B 模型）的教师模型。团队报告称在同一测试框架与推理设置下，该模型在 Terminal-Bench 2.1 上取得 80.9 分，高于 Qwen3.8-27B 的 73.0 分，但在 SWE-Bench Pro 上以 60.3 比 61.7 落后。 一个以宽松许可证发布、针对智能体编程与多轮工具调用调优的 33B 模型，为团队提供了可自行部署、替代更大闭源模型的选择，同时还能作为教师模型把能力蒸馏到更小的智能体中。如果这些指标经得起验证，它将进一步强化“中等规模开源权重模型在智能体基准上正面竞争 Qwen 级别模型”这一趋势。 所报告的智能体成绩依赖 preserve\_thinking=true 设置，即在上下文中保留此前的推理内容；模型卡建议在多轮工具调用时启用该设置，但不建议用于普通对话。所有数字均来自发布团队自己的评测，而非独立复现，并且 512K 上下文窗口在满长度下会带来相当可观的 KV 缓存显存开销。

reddit · r/MachineLearning · /u/jatingargiitk · 10月25日 16:32

**背景**: 南壁是中国招聘平台 BOSS 直聘旗下的 LLM 实验室，此次还发布了 Nanbeige4.3-33B-Base 变体，供用户自行做后训练。Terminal-Bench 2.1 是一个评测智能体命令行任务能力的基准，模型需要操作终端来完成任务目标，因此分数反映的是工具使用与多步规划能力，而非单纯的文本生成水平。preserve\_thinking 开关会把模型的思维链保留在对话历史中，使其能在多轮工具调用之间引用自己此前的推理；若将其剥离，智能体往往会反复重规划相同步骤。像这样的教师模型通常用于生成轨迹或 logits，供更小的学生模型训练使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.marktechpost.com/2026/10/25/nanbeige-releases-nanbeige4-3-33b-open-agentic-coding-model/">Nanbeige Releases Nanbeige4.3-33B, a 33B Open Agentic Coding ...</a></li>
<li><a href="https://www.datastudios.org/post/nanbeige-4-3-33b-open-weight-dense-agentic-model-512k-context">Nanbeige4.3-33B: Apache 2.0 dense agentic coding model with ...</a></li>
<li><a href="https://github.com/open-webui/open-webui/discussions/23895">Qwen 3.6 preserve_thinking breaks because Open WebUI ... - GitHub</a></li>

</ul>
</details>

**标签**: `#LLM`, `#open-weight models`, `#AI agents`, `#benchmarks`, `#model release`

---

<a id="item-7"></a>
## [MemT-1.0 架构解析：门控 DeltaNet-2 与混合存储打造智能体记忆](https://www.reddit.com/r/MachineLearning/comments/1xeu0ht/memt10_architecture_breakdown_gated_deltanet2/) ⭐️ 7.0/10

一篇 Reddit r/MachineLearning 帖子详细拆解了 MemT-1.0 的“记忆原生”架构，说明它如何在每一轮对话内结合 Gated DeltaNet-2 与稳定的 token 级记忆更新机制，并叠加 Mixture-of-Storage（MoS，混合存储）层来扩展记忆容量。帖子称，在 128k token 的历史长度下，MemT-1.0-nano 版本相比全上下文 KV 缓存方案可实现约 1.86 倍的端到端推理加速，持久化存储占用降低 66 倍。 长周期智能体正越来越受制于上下文窗口以及维持不断增长的 KV 缓存所带来的成本，因此一种把记忆内化到模型计算层的架构，有可能取代“只追加”的提示堆叠和外部 RAG 流水线。如果帖中给出的数字能够站得住脚，它将直接改变所有构建多轮智能体系统者在延迟、内存占用和推理服务成本上的考量。 帖子强调了其两阶段训练流程（继续预训练加后训练，共使用 340 亿 token），目的是在超越现有参数化记忆基线的同时保持通用推理能力，因为训练参数化记忆层通常会削弱基础大模型的能力。需要注意的是：所有数字均来自 Reddit 帖子的自述，且仅针对较小的 MemT-1.0-nano 版本在 128k 上下文下的表现，尚未经过独立复现验证。

reddit · r/MachineLearning · /u/Mrs-Grumpy23 · 10月25日 05:31

**背景**: 常规的大模型推理服务会维护一份 KV 缓存，即保存所有历史 token 的键值张量，以避免在生成时重复计算历史，但这份缓存会随上下文长度线性增长，这正是长时智能体会话成本高昂的原因。DeltaNet 等线性注意力模型用一个固定大小的循环状态取代不断增长的缓存，并通过 delta 规则更新该状态；Gated DeltaNet-2 则进一步用相互独立的逐通道门控把“擦除”和“写入”解耦，从而实现更细粒度的记忆控制。根据 arXiv 论文 2610.26825，MemT-1.0 构建于 Metis 之上，把这些思路用于智能体记忆：用 Gated DeltaNet-2 完成 token 级记忆更新，并用 Mixture-of-Storage 层扩展记忆容量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2610.26825">[2610.26825] MemT-1.0: Towards Memory-Native Evolution</a></li>
<li><a href="https://github.com/MemTensor/MemT-1.0/">GitHub - MemTensor/MemT-1.0: Official repository for MemT-1.0</a></li>
<li><a href="https://arxiv.org/abs/2605.22791">[2605.22791] Gated DeltaNet-2: Decoupling Erase and Write in ...</a></li>

</ul>
</details>

**标签**: `#agent memory`, `#LLM architecture`, `#KV cache`, `#mixture-of-storage`, `#DeltaNet`

---

<a id="item-8"></a>
## [改装版 RTX 3080 20GB 解锁 P2P 与 ReBAR，vLLM 预填充提速最高 115%](https://www.reddit.com/r/LocalLLaMA/comments/1xf9kmd/rtx_3080_20gb_got_rebar_and_p2p_unlock_70_prompt/) ⭐️ 7.0/10

社区贡献者 u/nathannguyennng 为改装版 20GB RTX 3080 解锁了 P2P 与 Resizable BAR，另一位用户在 Threadripper 1920X 双卡平台上以 vLLM 0.32.0、--tensor-parallel-size 2 进行了实测。与完全原厂状态相比，同时开启 GPU 解锁、ReBAR 和 P2P 后，提示词处理吞吐量按提示长度不同提升了约 70% 至 115%。 消费级 GeForce 显卡做张量并行推理时，通常必须经由 CPU 和系统内存通过 PCIe 在两张卡之间搬运激活值，长提示词场景下这成为明显瓶颈。消除这一开销后，RAG、长文档分析和智能体编程等以预填充为主的本地负载，在廉价的改装 20GB 显卡上变得实用得多，而不必依赖数据中心级 GPU。 提速几乎全部集中在预填充阶段：解码阶段的 token 间延迟变化基本落在噪声范围内（约 ±5%），只有 26.1 万 token 的超长测试出现可测量的提升，而且收益随上下文变长而收窄（8k token 时约 115%，26.19 万 token 时降至 71%）。测试平台为 Proxmox VE 9.2.21、内核 6.14.11-9-pve，两张 RTX 3080 20GB 插在 PCIe 3.0 x16 插槽并限制在 240W，模型为 Qwen3-27B AWQ INT4，启用了 MTP 投机解码与 FP8 KV 缓存。

reddit · r/LocalLLaMA · /u/No-Refrigerator-1672 · 10月25日 18:16

**背景**: GPUDirect 点对点（P2P）允许一块 GPU 通过 PCIe 或 NVLink 直接读写另一块 GPU 的显存，绕过 CPU 与系统内存；NVIDIA 并未在 GeForce 显卡上官方开放该功能，因此社区此前已为 RTX 4090 等型号做出解锁方案。Resizable BAR（ReBAR）则让 CPU 一次性寻址显卡的整个帧缓冲，而不是通过 256MB 的小窗口分块搬运。vLLM 的张量并行会把同一个模型切分到多张 GPU 上，卡间需要持续进行 all-reduce 通信，而这正是 P2P 所加速的流量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/gpudirect">GPUDirect | NVIDIA Developer</a></li>
<li><a href="https://charlie0129.github.io/blog/p/rtx4090-p2p-unlocked/">RTX4090 GPUDirect P 2 P Unlocked! | Charlie Chiang&#x27;s blog</a></li>
<li><a href="https://docs.vllm.ai/en/latest/serving/parallelism_scaling/">Parallelism and Scaling - vLLM</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#gpu-modding`, `#p2p`, `#tensor-parallel`, `#vllm`

---

<a id="item-9"></a>
## [HTMX 作者 Carson Gross 称业界误解了 REST 的本意](https://www.reddit.com/r/programming/comments/1xezyoh/htmx_creator_on_the_history_of_rest_and_why_he/) ⭐️ 7.0/10

在一档面向资深工程师的播客访谈中，HTMX 作者 Carson Gross 回顾了 Roy Fielding 最初如何定义 REST、业界又是如何把 JSON-over-HTTP 称作“REST”的，并解释了他为何认为由服务器直接返回 HTML 更接近最初的超媒体理念。访谈还涉及 HTMX 4、什么情况下才真正需要单页应用（SPA），以及 AI 如何改变“简单代码”与“聪明代码”之间的取舍。 Gross 是 JSON API 主流做法最知名的批评者之一，他对 REST 历史的重新讲述，直接挑战了当今大多数前端与 API 技术栈中默认的前提假设。他对 HTMX 4 以及 AI 辅助编码的看法，也暗示了在大模型降低复杂客户端代码编写成本之后，超媒体优先的开发方式可能处在什么位置。 这本质上是一期播客的宣传帖而非技术发布，因此关于 HTMX 4 的信息相当模糊——没有给出具体版本号、发布时间或功能清单。Gross 的论点建立在 Fielding 2000 年的博士论文以及 HATEOAS／超媒体约束之上，而绝大多数所谓的“RESTful”JSON API 实际上并不满足这一约束。

reddit · r/programming · /u/creasta29 · 10月25日 11:28

**背景**: REST 由 Roy Fielding 在其 2000 年的博士论文中提出，是一种建立在六项约束之上的架构风格，其中之一便是“超媒体作为应用状态引擎”（HATEOAS）。但在实践中，大多数被标称为“REST”的 API 只是采用资源式 URL 的 JSON-over-HTTP 接口，早已完全舍弃了超媒体约束。htmx 是 Carson Gross 开发的开源 JavaScript 库，于 2020 年 11 月首次发布，是 intercooler.js 的后继者；它通过自定义 HTML 属性扩展 HTML，让服务器可以返回 HTML 片段而非 JSON，从而免去大量手写 JavaScript 的工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/REST">REST - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Htmx">Htmx</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hypermedia">Hypermedia</a></li>

</ul>
</details>

**标签**: `#htmx`, `#rest`, `#web-development`, `#hypermedia`, `#podcast`

---

<a id="item-10"></a>
## [Izwi 0.1.0 发布：跨平台全本地语音 AI 应用](https://www.reddit.com/r/artificial/comments/1xf7dyg/izwi_010_fully_local_voice_ai_tts_asr_voice_chat/) ⭐️ 7.0/10

Izwi 0.1.0 正式发布，这是经过数月公开测试后的首个稳定版本，以 Apache-2.0 协议免费提供，形态为桌面应用，并附带 Web UI、CLI 和本地服务器。它集成了实时本地语音对话（ASR → LLM → TTS）、文本转语音、基于短样本的声音克隆、用文字描述设计音色、长音频制作工作室、带说话人分离与强制对齐的转写，以及兼容 OpenAI 的 /v1 API。 它把大量开源语音模型打包进一个跨平台安装包，推理基于 Candle 用 Rust 原生运行，免去了通常让非专业用户望而却步的 Python 环境管理。由于内置 API 与 OpenAI 的 chat completions、audio/speech、audio/transcriptions 接口保持一致，现有代码只需把地址指向 localhost 即可复用，这降低了隐私敏感的转写与语音工作流的使用门槛。 该版本列出的 TTS 模型包括 Qwen3-TTS、Kokoro-82M、Fish Audio S2 Pro、VibeVoice、Voxtral TTS 和 LFM2.5 Audio；ASR 支持 Parakeet TDT v3、Whisper large-v3-turbo、Qwen3-ASR、Granite Speech 4.1、Nemotron 3.5 ASR 和 Voxtral Mini；说话人分离使用 Sortformer 与 Nemotron 3；对话模型为 Qwen3.5、3.6、3.8 以及 LFM2.5。它仍是 0.1.0 版本，作者也明确征集在不同硬件上出现问题的反馈，因此模型覆盖范围与稳定性会因机器和 GPU 后端而异。

reddit · r/artificial · /u/zinyando · 10月25日 16:50

**背景**: 本地语音 AI 通常由三类模型组成：ASR（语音转文字，例如 NVIDIA 的 Parakeet TDT 这类面向流式推理的 transducer 模型，或 Whisper）、TTS（文本转语音，例如仅有 8200 万参数、可在笔记本上运行的 Kokoro-82M），以及说话人分离（判断“谁在什么时候说话”，例如 Sortformer）。Candle 是 Hugging Face 推出的 Rust 机器学习框架，可让这些模型无需 Python 运行时即可运行；Metal 和 CUDA 分别是苹果与 NVIDIA 的 GPU 计算接口，用于加速推理。所谓“兼容 OpenAI 的 API”，是指该服务器接受与 OpenAI 接口相同的请求格式，因此现有客户端库无需修改即可指向本地地址。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/hexgrad/Kokoro-82M">hexgrad/ Kokoro - 82 M · Hugging Face</a></li>
<li><a href="https://arxiv.org/abs/2409.06656">[2409.06656] Sortformer: A Novel Approach for Permutation ...</a></li>
<li><a href="https://localaimaster.com/models/parakeet-tdt">NVIDIA Parakeet TDT : Fastest Local Speech -to-Text 2026</a></li>

</ul>
</details>

**标签**: `#local-ai`, `#voice-ai`, `#text-to-speech`, `#speech-recognition`, `#open-source`

---

<a id="item-11"></a>
## [Solidigm 撤回 IPO，新云厂商信用利差走阔，超大规模厂商财报成焦点](https://www.reddit.com/r/artificial/comments/1xf68po/solidigm_pulled_its_ipo_and_neocloud_credit/) ⭐️ 7.0/10

本周 Solidigm 取消了原定的 IPO，与此同时，多家新云（neocloud）公司的信用违约互换利差走阔、股价下跌，而这一切恰好发生在几家最大超大规模云厂商发布季度财报的前几天。该帖将这两件事视为 AI 基建在融资层面遭遇的第一次真正压力测试。 如果新云厂商的借贷成本继续攀升、新的股权融资渠道持续关闭，英伟达硬件的最大买家们可能开始出现可支配现金不足的问题，进而反向冲击整条 AI 供应链。资金本周已转向防御性资产，说明市场正在重新定价“资本开支指引不及预期”的风险。 英伟达已不再只是卖芯片，而是在实质上为 AI 基建的部分环节提供融资，这使异常沉重的资产负债表压力集中在单一公司身上。市场认为，一旦超大规模厂商的资本开支指引令人失望，新云厂商借贷方将是最缺乏缓冲的一群，由此引出疑问：是英伟达先承受冲击，还是信用利差先于股价崩裂。

reddit · r/artificial · /u/perspicacity\_ai · 10月25日 16:06

**背景**: Solidigm 是一家 NAND 闪存与固态硬盘厂商，源自英特尔此前的存储业务，现由 SK 海力士持有，因此其上市计划的取消被视为市场对硬件相关股权融资兴趣的风向标。新云（neocloud）是一类较新的专业化云服务商，围绕面向 AI 与高性能计算负载的“GPU 即服务”模式构建，与 AWS、微软 Azure 等通用型超大规模云厂商形成区别。信用违约互换利差是衡量市场所感知违约风险的指标：利差走阔意味着投资者为防范借款人违约而索要更高的保费，而这正是当前新云厂商身上发生的情况。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.solidigm.com/who-we-are.html">About Solidigm: SSD Innovation &amp; Company Story</a></li>
<li><a href="https://rcrtech.com/semiconductor-news/neocloud-explainer-main-players/">What is a NeoCloud and who are the main players?</a></li>
<li><a href="https://builtin.com/articles/ai-neocloud-demand">What Is a Neocloud? How AI Compute Is Changing Cloud ...</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#Nvidia`, `#neoclouds`, `#credit markets`, `#industry analysis`

---

<a id="item-12"></a>
## [FOSDEM 27 演讲呼吁拒绝接受被审查的互联网，引发热议](https://talkweb.eu/openweb/4558/) ⭐️ 6.0/10

talkweb.eu 上的一篇博文宣布将在 FOSDEM 2027 带来一场题为“我拒绝接受被审查的互联网”的演讲，主张用户和开发者不应默认接受一个被审查的网络。该公告在 Hacker News 上引发约 364 分、180 条评论的热烈讨论，争论焦点是“无审查的互联网”究竟是否可能实现。 这场演讲把审查问题重新定义为基础设施与政治经济学问题，而不只是纯技术问题，这对开发翻墙工具、VPN 和隐私保护软件的人尤其重要。讨论中的分歧也说明，即便在开放网络与隐私社区内部，对于“无审查互联网”能否守住也并无共识。 这本质上是一则倡导性演讲的公告，而非技术深度文章，因此并未提供新的测量数据或工具。评论者指出，加密的规避流量仍然跑在被审查的同一套基础设施之上，既可能被封锁，也可能被资本收买；此外，“内容审核”与“审查”经常被混为一谈。

hackernews · Tomte · 10月25日 17:30 · [社区讨论](https://news.ycombinator.com/item?id=50233929)

**背景**: FOSDEM（欧洲自由及开源软件开发者会议）是每年在布鲁塞尔举办的非商业、由志愿者组织的开源软件大会，设有主会场演讲和多个开发者主题房间，议题涵盖隐私、网络与开放网络。这场争论反映了一个长期存在的张力：端到端加密以及 VPN、Tor 等规避系统可以绕开封锁，但它们仍依赖物理链路和服务提供商，而这些都可能被国家和企业掌控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/FOSDEM">FOSDEM - Wikipedia</a></li>
<li><a href="https://fosdem.org/">FOSDEM 2027</a></li>

</ul>
</details>

**社区讨论**: 持怀疑态度的评论者认为，无审查的互联网可能根本不存在，因为规避流量仍然跑在被审查的网络上，而企业只要付钱给基础设施提供商就能让其听命。也有人认为如今多数人更愿意接受一个与自己政治立场一致的被审查互联网；一位评论者区分了内容审核与审查，还有人称赞 FOSDEM 是一个没有推销、技术内容一流的非商业会议。

**标签**: `#internet-censorship`, `#privacy`, `#open-web`, `#fosdem`, `#net-neutrality`

---

<a id="item-13"></a>
## [DreamHost 因文件管理器安全事件强制用户重置密码](https://www.dreamhoststatus.com/) ⭐️ 6.0/10

DreamHost 正在对受影响的邮箱和 FTP/SFTP 用户强制重置密码，起因是一起仍在处理中的安全事件，最初表现为其文件管理器（File Manager）和网页邮箱（Webmail）出现连接故障。官方尚未公开说明根本原因，其状态页上文件管理器、网页邮箱和邮箱托管服务仍被标记为中断。 主机商集中保管着成千上万个小网站的登录凭据，一旦 FTP/SFTP 账号泄露，影响可能外溢到大量客户站点被入侵或被篡改，远不止 DreamHost 自身。这起事件也凸显了主机商在面板中集成第三方 Web 应用所带来的供应链风险。 DreamHost 提醒，在重置流程完成之前所做的任何密码修改都会被覆盖，因此用户应等重置结束后再设置新密码。官方仅确认正在重置邮箱与 FTP/SFTP 密码，并未说明攻击者究竟访问或窃取了哪些数据。

hackernews · greenchair · 10月25日 13:09 · [社区讨论](https://news.ycombinator.com/item?id=50231166)

**背景**: Monsta FTP 是一款用 PHP 编写的商业浏览器端文件管理器，许多主机商会安装它，让客户无需桌面客户端即可通过 FTP/SFTP 传输文件。由于它在面向 Web 的应用中处理 FTP 凭据，其自身漏洞（例如近期 CVE 中记录的远程代码执行和服务端请求伪造问题）可能导致已保存的登录信息外泄。DreamHost 的状态页最初把问题描述为“影响文件管理器的连接故障”，这正是评论者把注意力集中到该组件上的原因。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.dreamhoststatus.com/">Investigating an incident affecting File Manager and Webmail</a></li>
<li><a href="https://zeli.app/story/50231166">DreamHost resets customer passwords · Hacker News | Zeli</a></li>
<li><a href="https://www.sentinelone.com/vulnerability-database/cve-2025-34299/">CVE-2025-34299: Monsta FTP RCE Vulnerability - SentinelOne</a></li>

</ul>
</details>

**社区讨论**: 评论者进行了“纸上谈兵”式的事故分析：duskwuff 推断该文件管理器是 Monsta FTP 的部署实例，很可能被近期公开的某个 PHP 漏洞攻破，从而导致用户的 FTP 凭据被窃取。其他人则分享了迁移主机的经历，并质疑 DreamHost 是否正变得越来越不可靠；还有用户表示自己起初以为只是本地网络问题。

**标签**: `#security-incident`, `#web-hosting`, `#vulnerability`, `#credential-leak`, `#hackernews-discussion`

---

<a id="item-14"></a>
## [JetBrains 实验性智能体 IDE「ThinkRail」引发战略质疑](https://github.com/JetBrains/thinkrail) ⭐️ 6.0/10

JetBrains 在其 InnovationHub 孵化项目下发布了一个名为 ThinkRail 的实验性开源仓库，将其描述为一款轻量级智能体 IDE，围绕隔离的 git worktree 工作区、Monaco 编辑器标签页、终端与 diff 构建，并把项目意图记录在「spec graph」中。该仓库在 Hacker News 上获得约 159 分和 111 条评论，讨论很快从代码本身转向它折射出的 JetBrains AI 路线图问题。 该项目表明 JetBrains 愿意在其长期依赖的 IntelliJ 平台之外进行试验，而它与近期推出的 JetBrains Air 之间明显的功能重叠，让人怀疑公司究竟是在收敛出一套连贯的「智能体优先」战略，还是在同时推出相互竞争的原型。对开发者而言，这是一个早期信号：IDE 厂商正设想一种以 git worktree 而非聊天面板作为主要工作单元的开发流程。 ThinkRail 以 Apache-2.0 协议开源，定位为 InnovationHub 孵化项目而非旗舰产品，它把真实编辑器与智能体（README 中提到「pi」）结合，覆盖 Monaco 标签页、终端和 diff。评论者指出其 README 似乎是 AI 生成的，而且编辑器层看起来更接近 VS Code/Monaco 基础，而非 JetBrains 自家的 IntelliJ 引擎。

hackernews · hmokiguess · 10月25日 16:27 · [社区讨论](https://news.ycombinator.com/item?id=50233294)

**背景**: JetBrains 是一家创立于布拉格的公司，其 IntelliJ 平台支撑着 IntelliJ IDEA、PyCharm、WebStorm 和 Rider，公司还创造了 Kotlin 语言。在 AI 时代，它推出了 Junie 编码智能体和 JetBrains Air 等产品，后者用于跨项目运行和审阅多个编码智能体。Monaco 是支撑 VS Code 的开源编辑器组件，因此基于它构建意味着偏离 JetBrains 自研的编辑器技术；而 git worktree 允许开发者把同一个仓库的多个分支同时检出到不同目录中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/JetBrains/thinkrail">GitHub - JetBrains/thinkrail: Vibe code with pi in a ...</a></li>
<li><a href="https://thinkrail.ai/">ThinkRail — the agentic IDE that gets better every time you ...</a></li>
<li><a href="https://www.jetbrains.com/air/">JetBrains Air: One system for building software with agents</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的反应以质疑为主：有评论者因为 README 似乎是完全由 AI 生成而直接否定该仓库，另一些人则质疑 JetBrains 为何要在推出高度相似的 JetBrains Air 之后再做 ThinkRail。长期用户表达了对公司分散的 AI 战略和不透明 token 定价的不满，有人表示如今已很少打开 JetBrains IDE，并更希望看到像 Zed 那样的原生方案，而不是基于 VS Code 的衍生品。

**标签**: `#JetBrains`, `#IDEs`, `#developer tools`, `#AI coding agents`, `#open source`

---

<a id="item-15"></a>
## [Claude 拦截“逆向工程一切”工作流，再度引发护栏争议](https://www.reddit.com/r/LocalLLaMA/comments/1xer30z/openai_and_anthropic_blocked_the_reverse/) ⭐️ 6.0/10

r/LocalLLaMA 上的一篇帖子称，Anthropic 的 Claude 在“逆向工程一切”（REA）智能体工作流搭建完成约一天后便将其拦截，触发点似乎是让它分析智能电视的数据采集行为；发帖者还表示 OpenAI 的模型也拒绝了类似请求。该帖将此视为商业大模型安全护栏阻断正当逆向工程与安全研究工作的又一案例。 对安全研究员和逆向工程师来说，这是一个反复出现的摩擦点：如果托管模型拒绝看起来像攻击的任务，相关工作要么停滞，要么转向可在本地运行、没有服务商拒绝层的开放权重模型。这种趋势直接强化了本地大模型的合理性，也会影响安全工具生态在多大程度上转向开放权重。 REA 是一套智能体工作流加 MCP 服务器，可安装进 Claude Code、Codex、Cursor、Gemini CLI 等编程智能体中，因此拒绝发生在模型层而非工具本身。该报告只是单个用户的轶事，没有日志或提示词记录；其根本问题在于护栏判断的是对话的“形状”而非经过验证的用户意图，导致正当研究难以与攻击区分开来。

reddit · r/LocalLLaMA · /u/kroggens · 10月25日 02:51

**背景**: REA（“逆向工程一切”）是一个开源项目，它把逆向工程的操作指令与一个 MCP（模型上下文协议）服务器打包在一起，让编程智能体能够以证据驱动的方式检查二进制文件、Electron ASAR 归档和应用入口点。MCP 是让大模型智能体调用外部工具和数据源的接口标准。Claude 和 OpenAI 的 GPT 系列等商业模型都带有安全分类器，会对被认为有风险的请求予以拒绝或降级处理；而逆向工程——即拆解软件以理解其运作方式——即便目的是隐私研究（例如审计智能电视向家中回传了哪些数据），也常常触发这些分类器。开放权重模型（Llama、Qwen、DeepSeek、Mistral 等）可通过 Ollama、LM Studio 等工具在本地运行，让研究者获得一个没有服务商拒绝层的模型版本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/morluto/rea">GitHub - morluto/rea: Reverse engineer anything with agents ...</a></li>
<li><a href="https://www.toxsec.com/p/why-ai-guardrails-cant-tell-your">Why AI Guardrails Can’t Tell Your Research From an Attack</a></li>
<li><a href="https://dev.to/synsun/running-local-llms-in-2026-ollama-lm-studio-and-jan-compared-121c">Running Local LLMs in 2026: Ollama, LM Studio... - DEV Community</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#LLM guardrails`, `#reverse engineering`, `#privacy`, `#local LLMs`

---

<a id="item-16"></a>
## [Reddit 提醒：在 Hugging Face 删除前备份量化模型](https://www.reddit.com/r/LocalLLaMA/comments/1xf11qj/backup_your_quants/) ⭐️ 6.0/10

r/LocalLLaMA 上的一篇帖子呼吁用户立即备份量化 LLM 文件并制作 torrent，理由是 mradermacher 的 Hugging Face 模型请求页面出现相关提示，并警告其他量化模型制作者也可能面临类似下架。 量化 GGUF 文件通常是普通用户在消费级硬件上运行本地模型的最实用方式，因此社区制作的量化版本一旦消失，可能打断现有工作流，并抹去原模型作者未必会重新上传的可复现产物。 帖子指向 mradermacher 的 model\_requests 页面，并建议通过 llama.garden、pirateface.co 和 huggingbay.xyz 分享 torrent；但它没有说明上传可能被删除的具体原因，也没有列出受影响的模型。

reddit · r/LocalLLaMA · /u/Kahvana · 10月25日 12:25

**背景**: GGUF 是一种自包含的模型文件格式，被 llama.cpp 等本地推理工具广泛使用；量化通过压缩模型权重，让大模型能在有限的显存或内存上运行。mradermacher 是 Hugging Face 上非常活跃的上传者，为社区模型制作了大量 GGUF 量化版本。由于 Hugging Face 是中心化托管平台，单个账号或仓库被删除就可能让这些文件难以获取，因此一些用户会通过 Pirate Face、Hugging Bay 等站点以 torrent 形式做镜像备份。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.promptquorum.com/local-llms/llm-quantization-explained">Q4_K_M vs Q4_0 vs Q8_0: LLM Quantization Explained (2026)</a></li>
<li><a href="https://pirateface.co/">Pirate Face - Turn AI into torrents that live forever</a></li>
<li><a href="https://huggingbay.xyz/">Hugging Bay | Find and Download AI Models</a></li>

</ul>
</details>

**标签**: `#model-preservation`, `#quantized-models`, `#local-llm`, `#huggingface`, `#decentralized-distribution`

---

<a id="item-17"></a>
## [开发者预览 4B Qwen3.5 微调模型：兼顾编程与 3D 场景生成](https://www.reddit.com/r/LocalLLaMA/comments/1xeuo7t/a_4b_coding_model_that_can_generate_3d_scenes/) ⭐️ 6.0/10

一位开发者发布了基于 Qwen3.5-4B 独立微调模型的早期预览版，目标是通用编程与 3D 场景生成，并已在 Hugging Face 上提供 Q4\_K\_M 和 Q8\_0 两种 GGUF 量化版本。训练仍在进行中，作者表示将在接下来几天内更新最终模型并公开训练数据集。 小参数模型在 3D 场景生成上普遍表现不佳，因此一个真正可用的 4B 微调模型有望让场景创作在消费级硬件上跑起来，而不必依赖数据中心级 GPU。提前放出 GGUF 量化版本也让本地大模型用户能立刻在 llama.cpp 类运行时中试用，而不必等待正式版发布。 这明确只是一个预览版：训练数据集、基准测试和评测数据均尚未公布，作者也承认小模型在其测试中的 3D 表现一直“相当粗糙”。Q4\_K\_M 是约 4 比特的量化，适合显存较小的机器；Q8\_0 接近无损，但内存占用大约翻倍。

reddit · r/LocalLLaMA · /u/ConfidentDinner6648 · 10月25日 06:10

**背景**: Qwen3.5-4B 是阿里 Qwen 系列中的 4B 参数稠密模型，原生上下文长度达 262,144 个 token，并采用统一的视觉-语言联合训练方案。GGUF 是 llama.cpp 及其衍生运行时（如 Ollama、LM Studio）使用的模型文件格式，用于在 CPU 或消费级 GPU 上本地运行模型。Q4\_K\_M、Q8\_0 这类量化方案把权重压缩到更低位宽，使模型能塞进有限的内存，以少量质量损失换取体积的大幅下降。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lmstudio.ai/models/qwen/qwen3.5-4b">qwen/qwen3.5-4b • LM Studio</a></li>
<li><a href="https://localmodel.run/guides/quantization">Quantization explained: Q4_K_M vs Q8_0 vs FP16 · localmodel.run</a></li>
<li><a href="https://www.secondstate.io/articles/convert-pytorch-to-gguf/">How do I create a GGUF model file?</a></li>

</ul>
</details>

**标签**: `#local-llm`, `#model-fine-tuning`, `#3d-scene-generation`, `#qwen`, `#gguf`

---