---
layout: default
title: "Horizon Summary: 2026-06-05 (EN)"
date: 2026-06-05
lang: en
---

> From 25 items, 14 important content pieces were selected

---

1. [Anthropic Releases Open-Source AI Vulnerability Discovery Harness](#item-1) ⭐️ 8.0/10
2. [VoidZero Joins Cloudflare](#item-2) ⭐️ 8.0/10
3. [Anthropic Discusses Progress in AI Recursive Self-Improvement](#item-3) ⭐️ 8.0/10
4. [Meta adds facial recognition to Ray-Ban smart glasses](#item-4) ⭐️ 8.0/10
5. [Huawei KVarN: Native vLLM Backend for KV-Cache Quantization](#item-5) ⭐️ 7.0/10
6. [Retro-Tech Parenting: Intentional Tech Choices for Kids](#item-6) ⭐️ 7.0/10
7. [Uruky, EU-based Kagi alternative, adds image search and URL rewrites](#item-7) ⭐️ 7.0/10
8. [Gaussian Point Splatting: Scaling to Massive Scenes](#item-8) ⭐️ 7.0/10
9. [Google employees mock AI; company retracts human oversight pledge](#item-9) ⭐️ 7.0/10
10. [Houston Solar-Storage-Electricity Bundle at 6¢/kWh](#item-10) ⭐️ 6.0/10
11. [Nissan partners with Gelion for low-cost solid-state EV batteries](#item-11) ⭐️ 6.0/10
12. [BMW iX3 sets record 485-mile range in NAF test](#item-12) ⭐️ 6.0/10
13. [xAI buys $269M Tesla Megapacks in single month for AI data centers](#item-13) ⭐️ 6.0/10
14. [Waymo Repurposes Retired Robotaxi Batteries for Grid Storage](#item-14) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Anthropic Releases Open-Source AI Vulnerability Discovery Harness](https://github.com/anthropics/defending-code-reference-harness) ⭐️ 8.0/10

Anthropic has released an open-source harness for AI-driven vulnerability discovery on GitHub, providing a framework that uses large language models to automate the detection of security flaws. This release lowers the barrier for security researchers to experiment with AI-based vulnerability discovery, but expert commentary indicates that significant customization and cost considerations remain for practical use. The repository is labeled as not maintained and not accepting contributions, and cost estimates suggest hundreds to thousands of dollars per run depending on the model used (Opus vs. Mythos).

hackernews · binyu · Jun 4, 20:11 · [Discussion](https://news.ycombinator.com/item?id=48403980)

**Background**: AI-powered vulnerability discovery harnesses orchestrate multiple AI agents to analyze code and identify security vulnerabilities. Typical approaches involve an orchestrator agent that dispatches specialized agents based on an execution journal. Anthropic's contribution is notable as an open-source implementation from a leading AI company, though the field is still nascent and requires tailored setups.

<details><summary>References</summary>
<ul>
<li><a href="https://undercodetesting.com/ai-zero-day-hunter-finding-undiscovered-vulnerabilities-for-0-per-codebase-with-open-source-orchestration-video/">AI Zero‑Day Hunter: Finding Undiscovered... - Undercode Testing</a></li>
<li><a href="https://thinkml.ai/9-ai-powered-vulnerability-assessment-tools-for-modern-pentesters/">9 AI -Powered Vulnerability Assessment Tools for Modern Pentesters</a></li>

</ul>
</details>

**Discussion**: Experts like tptacek and baby emphasize that such harnesses are best used as inspiration for custom builds, not as plug-and-play tools. Simonw raises cost concerns, and others note the repository is unmaintained.

**Tags**: `#AI`, `#security`, `#vulnerability discovery`, `#open-source`, `#frameworks`

---

<a id="item-2"></a>
## [VoidZero Joins Cloudflare](https://blog.cloudflare.com/voidzero-joins-cloudflare/) ⭐️ 8.0/10

Cloudflare has acquired VoidZero, the open-source company behind Vite, Vitest, and other JavaScript tooling. The VoidZero team will join Cloudflare, and a $1 million fund will be established to support the Vite ecosystem. This acquisition brings the core Vite team and its widely-used build tool into Cloudflare's infrastructure, potentially accelerating frontend tooling innovation at the edge. It also raises questions about the independence of open-source projects acquired by large corporations. Cloudflare commits $1 million to an independent Vite ecosystem fund. The tools are promised to remain open-source and vendor-neutral, according to the announcement.

hackernews · coloneltcb · Jun 4, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48398055)

**Background**: Vite is a modern JavaScript build tool known for its fast development server and optimized production builds, widely adopted in the frontend community. VoidZero was the company maintaining Vite, Vitest, and related tools, founded by Evan You, the creator of Vue.js.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cloudflare.com/press/press-releases/2026/cloudflare-acquires-voidzero-to-build-the-future-of-the-ai-native-web/">Cloudflare Acquires VoidZero to Build the Future of the AI ...</a></li>
<li><a href="https://www.morningstar.com/news/business-wire/20260604108073/cloudflare-acquires-voidzero-to-build-the-future-of-the-ai-native-web">Cloudflare Acquires VoidZero to Build the Future of the AI ...</a></li>
<li><a href="https://www.heise.de/en/news/Cloudflare-acquires-VoidZero-Team-behind-Vite-switches-completely-11319023.html">Cloudflare acquires VoidZero – Team behind Vite switches ...</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed emotions: some admire Vite's history and team, but many are uneasy about the acqui-hire model and potential shift in priorities under Cloudflare. Skepticism remains about promises of continued independence and vendor neutrality.

**Tags**: `#web development`, `#JavaScript`, `#Vite`, `#Cloudflare`, `#acquisitions`

---

<a id="item-3"></a>
## [Anthropic Discusses Progress in AI Recursive Self-Improvement](https://www.anthropic.com/institute/recursive-self-improvement) ⭐️ 8.0/10

Anthropic published an article detailing their progress toward recursive self-improvement in AI, where models like Claude generate and refine code to enhance their own capabilities. Recursive self-improvement could lead to an intelligence explosion, making AI systems vastly more capable and potentially surpassing human control, raising critical safety and alignment concerns. The article highlights that while AI can now write most of its own code and continuously improve, key parts of the loop remain human-controlled, and progress has not yet yielded breakthroughs outside of AI itself.

hackernews · meetpateltech · Jun 4, 16:20 · [Discussion](https://news.ycombinator.com/item?id=48400842)

**Background**: Recursive self-improvement (RSI) is a process where an AI system rewrites its own code to become more capable, potentially leading to a rapid intelligence explosion. The concept raises significant ethical and safety concerns, as such systems could evolve unpredictably and surpass human understanding or control. Anthropic, an AI safety company, has been exploring RSI in the context of code generation and self-modification.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement</a></li>
<li><a href="https://spectrum.ieee.org/recursive-self-improvement">Recursive Self-Improvement Edges Closer In AI Labs - IEEE Spectrum</a></li>

</ul>
</details>

**Discussion**: Community comments are skeptical: users note reliability issues (outages, API errors) and question the lack of breakthroughs beyond vibe coding. Some argue that pursuing RSI at full speed contradicts Anthropic's stated safety goals, while others mock the naming of Anthropic's model 'Mythos' after Lovecraftian horrors, suggesting a disconnect between branding and safety ethos.

**Tags**: `#AI`, `#recursive self-improvement`, `#AI safety`, `#Anthropic`, `#code generation`

---

<a id="item-4"></a>
## [Meta adds facial recognition to Ray-Ban smart glasses](https://www.buchodi.com/meta-glasses-facial-recognition/) ⭐️ 8.0/10

Meta has shipped facial recognition capabilities on its Ray-Ban smart glasses, allowing users to identify people they look at. This move reignites privacy concerns and ethical debates around wearable cameras and biometric data, following the controversy of Google Glass a decade ago. The feature reportedly requires internet connectivity and uses Meta's cloud-based AI, raising questions about data storage and consent.

hackernews · buchodi · Jun 4, 19:36 · [Discussion](https://news.ycombinator.com/item?id=48403588)

**Background**: Facial recognition technology identifies or verifies a person by analyzing facial features. Meta is a social media giant with a history of privacy controversies. The Ray-Ban smart glasses are a consumer wearable that can capture photos and videos hands-free.

**Discussion**: Comments express mixed reactions: some desire offline use for accessibility (e.g., prosopagnosia), while others fear privacy invasion. Past comparisons to Google Glass' developer restrictions are noted, and concerns about Meta's privacy record are highlighted.

**Tags**: `#facial recognition`, `#privacy`, `#meta`, `#smart glasses`, `#ethics`

---

<a id="item-5"></a>
## [Huawei KVarN: Native vLLM Backend for KV-Cache Quantization](https://github.com/huawei-csl/KVarN) ⭐️ 7.0/10

Huawei has released KVarN, an open-source native vLLM backend for KV-cache quantization, claiming superior performance compared to TurboQuant (TQ) and better quality than FP16. KV-cache quantization is critical for reducing memory footprint in LLM inference; KVarN's claimed improvements could enable longer context lengths and higher throughput without sacrificing quality. KVarN is a native vLLM backend, meaning it integrates directly with vLLM's architecture, and it is open-sourced on GitHub under the Huawei-CSL organization. The project is still early-stage and not yet merged into mainstream vLLM.

hackernews · theanonymousone · Jun 4, 15:18 · [Discussion](https://news.ycombinator.com/item?id=48399974)

**Background**: KV-cache quantization reduces the memory required to store key-value cache during LLM inference, enabling longer context lengths. vLLM is a popular high-throughput LLM inference engine that supports various quantization methods. TurboQuant (TQ) is a recent quantization algorithm from Google that achieves extreme compression. KVarN aims to combine the benefits of both.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/features/quantization/quantized_kvcache/">Quantized KV Cache - vLLM</a></li>
<li><a href="https://github.com/0xSero/turboquant">GitHub - 0xSero/turboquant: TurboQuant: Near-optimal KV cache ...</a></li>

</ul>
</details>

**Discussion**: The community reacted with curiosity and skepticism. One commenter asked if they read correctly that KVarN claims better performance than TQ and better quality than FP16. Another wondered why it is not a pull request for vLLM, while a third made a positive remark in Chinese praising its leading edge.

**Tags**: `#LLM inference`, `#KV-cache quantization`, `#vLLM`, `#Huawei`, `#open-source`

---

<a id="item-6"></a>
## [Retro-Tech Parenting: Intentional Tech Choices for Kids](https://havenweb.org/2026/05/28/retro-tech.html) ⭐️ 7.0/10

A parent shares their approach to providing retro-tech—such as books, an offline laptop, and robotics kits—to their children, sparking a community discussion about deliberate technology use for kids. This approach offers a practical alternative to modern ad-driven platforms, helping children develop independence, creativity, and a grounded understanding of technology's evolution. The parent's specific choices include a 2012 MacBook Pro without internet, Lego Spike robotics sets, and over 1,500 books. Community members also suggest using retro games, landline phones, and observing tech progression over time.

hackernews · mawise · Jun 4, 16:02 · [Discussion](https://news.ycombinator.com/item?id=48400588)

**Background**: Retro-tech parenting involves using older, more controllable technologies to give children enriching experiences while avoiding negative aspects of modern online platforms. This trend has gained attention as parents seek ways to balance digital exposure with hands-on learning and family connection.

<details><summary>References</summary>
<ul>
<li><a href="https://havenweb.org/2026/05/28/retro-tech.html">Haven Blog: Retro-Tech Parenting</a></li>
<li><a href="https://flipso.com/p/yswx16r8b?ref=rss">Retro-Tech Parenting · Flipso</a></li>
<li><a href="https://www.businessinsider.com/millennial-mom-shares-nostalgic-parenting-vhs-tin-can-trading-cards-2026-1?op=1">I'm Raising My Kids on '90s and Retro-Style Tech. They Love It ...</a></li>

</ul>
</details>

**Discussion**: Comments generally support this intentional approach, with many parents sharing their own examples such as retro gaming consoles and neighborhood PBX systems. A recurring theme is that experiencing technology's progression helps children understand core principles.

**Tags**: `#parenting`, `#retro-tech`, `#education`, `#technology`, `#community`

---

<a id="item-7"></a>
## [Uruky, EU-based Kagi alternative, adds image search and URL rewrites](https://uruky.com/?il=en) ⭐️ 7.0/10

Uruky, a EU-based paid search engine and alternative to Kagi, now offers image search and URL rewrites. It also provides a 2-hour free trial via a proof-of-work captcha. This expansion makes Uruky a more viable competitor to Kagi, especially for EU privacy-conscious users. However, the community highlights that it still lags in UI/UX and feature parity, which could limit adoption. Uruky plans to share source code under the PolyForm Shield source-available license, which prohibits competition, and is considering dropping the NDA requirement. The company has surpassed 100 monthly active accounts and aims to offer a code download to 12-month-old accounts.

hackernews · BrunoBernardino · Jun 4, 08:56 · [Discussion](https://news.ycombinator.com/item?id=48396004)

**Background**: Uruky is a privacy-focused, EU-based search engine that charges a subscription fee, positioning itself as an alternative to Kagi. Kagi is a popular paid search engine known for its clean UX and advanced features. Uruky uses a proof-of-work captcha to verify users without tracking, and plans a source-available license to balance transparency with business protection.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Proof_of_work">Proof of work - Wikipedia</a></li>
<li><a href="https://polyformproject.org/licenses/shield/1.0.0">PolyForm Shield License 1.0.0 - Polyform Project</a></li>
<li><a href="https://altcha.org/docs/v2/proof-of-work-captcha/">Proof Of Work Captcha | ALTCHA</a></li>

</ul>
</details>

**Discussion**: Community feedback is mixed: some praise the EU privacy focus but criticize the UI/UX as not user-friendly enough for non-technical users. Others compare feature gaps (missing AI response, widgets, indexing) to Kagi and ask about search result sources. Overall, sentiment is cautiously supportive but demanding significant improvements.

**Tags**: `#search engine`, `#privacy`, `#EU`, `#Kagi alternative`, `#image search`

---

<a id="item-8"></a>
## [Gaussian Point Splatting: Scaling to Massive Scenes](https://momentsingraphics.de/Siggraph2026.html) ⭐️ 7.0/10

Researchers propose Gaussian point splatting, a stochastic rendering method that samples opaque points from Gaussians and uses 64-bit atomics to render massive 3D Gaussian splatting scenes without sorting or tile-based rendering. This technique significantly improves scalability for scenes with many Gaussians, enabling real-time rendering of massive 3D scenes with minimal quality loss, which could advance applications in games, VR, and 3D visualization. The method eliminates the need for sorting and tile-based rendering by sampling pixel-sized opaque points and applying stochastic transparency. It builds on the seminal 3D Gaussian splatting from Inria (2023) and is set to be presented at SIGGRAPH 2026.

hackernews · ibobev · Jun 4, 10:48 · [Discussion](https://news.ycombinator.com/item?id=48396792)

**Background**: Traditional 3D rendering uses meshes and polygons, which can be computationally expensive. Gaussian splatting represents scenes as a collection of 3D Gaussian primitives, offering faster rendering for novel view synthesis. However, scaling to massive numbers of Gaussians has been challenging due to memory and sorting requirements. Gaussian point splatting addresses this by sampling points instead of rendering full Gaussians.

<details><summary>References</summary>
<ul>
<li><a href="https://momentsingraphics.de/Siggraph2026.html">Gaussian Point Splatting - momentsingraphics.de</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gaussian_splatting">Gaussian splatting - Wikipedia</a></li>
<li><a href="https://jorisar.nl/gaussian_point_splatting/">Gaussian Point Splatting - jorisar.nl</a></li>

</ul>
</details>

**Discussion**: Comments express interest in applying the technique to AAA games, with comparisons to the 1994 game Ecstatica that used ellipsoid splats. Some users note that Gaussian splatting has overshadowed older point splatting techniques and ask for tutorials. One commenter compares it to mesh splatting, suggesting meshes may better represent sharp features.

**Tags**: `#computer graphics`, `#rendering`, `#gaussian splatting`, `#3D visualization`

---

<a id="item-9"></a>
## [Google employees mock AI; company retracts human oversight pledge](https://simonwillison.net/2026/Jun/4/a-slightly-different-version/#atom-everything) ⭐️ 7.0/10

Google employees internally shared memes criticizing the poor performance of the company's AI, and after the story broke, Google retracted its previous statement that maintaining humans in the loop was critical. This incident reveals internal skepticism about Google's AI quality and a troubling shift in corporate transparency regarding human oversight, raising important questions about AI ethics and accountability. The original statement emphasized the importance of human-in-the-loop, but after media coverage, Google's spokesperson requested publication of a revised version that omitted that commitment entirely.

rss · Simon Willison · Jun 4, 16:38

**Background**: Human-in-the-loop is a principle in AI development where human oversight is maintained to catch errors and ensure ethical operation. Companies like Google often publicly commit to such practices, but internal memes and statement changes suggest a gap between rhetoric and reality.

**Tags**: `#ai-ethics`, `#google`, `#ai`, `#journalism`, `#human-in-the-loop`

---

<a id="item-10"></a>
## [Houston Solar-Storage-Electricity Bundle at 6¢/kWh](https://electrek.co/2026/06/04/houston-solar-storage-electricity-bundle-6-cents-per-kwh/) ⭐️ 6.0/10

Terra Energy launched TerraOne, a three-year subscription bundling rooftop solar, up to 40 kWh of battery storage, and electricity service at a fixed rate of 6¢ per kWh with no upfront fees or loans. This low bundled price could make solar-plus-storage accessible to more homeowners in Houston, potentially accelerating renewable energy adoption and challenging traditional utility models in deregulated electricity markets. The TerraOne subscription covers three years, includes a 40 kWh battery for whole-home backup, and offers a fixed electricity rate of 6¢ per kWh for the entire bundle. No upfront costs, no loans, and no liens are required.

rss · Electrek · Jun 4, 19:42

**Background**: Traditionally, residential solar and battery systems require large upfront investments or long-term loans, which can be a barrier for many homeowners. Bundling these with electricity service as a subscription lowers the financial barrier and simplifies the customer experience. Houston operates in Texas's deregulated electricity market, allowing retail energy providers to offer innovative plans like this.

<details><summary>References</summary>
<ul>
<li><a href="https://www.morningstar.com/news/business-wire/20260604683487/terra-energy-launches-lowest-cost-home-energy-plan-in-houston-for-bundled-solar-battery-backup-and-retail-electricity">Terra Energy Launches Lowest-Cost Home Energy Plan in Houston for Bundled Solar, Battery Backup, and Retail Electricity | Morningstar</a></li>
<li><a href="https://electrek.co/2026/06/04/houston-solar-storage-electricity-bundle-6-cents-per-kwh/">Houston gets a solar, storage + electricity bundle for 6¢ per kWh | Electrek</a></li>

</ul>
</details>

**Tags**: `#solar`, `#energy storage`, `#renewable energy`, `#electricity`

---

<a id="item-11"></a>
## [Nissan partners with Gelion for low-cost solid-state EV batteries](https://electrek.co/2026/06/04/nissan-solid-state-ev-battery-project-aims-for-cheaper-than-china/) ⭐️ 6.0/10

Nissan has announced a three-year collaboration with Gelion to develop low-cost solid-state EV batteries aimed at undercutting Chinese manufacturers. The project leverages Gelion's nano-encapsulated sulfur cathode technology. This partnership could help non-Chinese automakers reduce dependence on Asian battery suppliers and lower EV costs, potentially reshaping the global battery supply chain. Solid-state batteries promise higher energy density and safety, which are critical for mass EV adoption. The collaboration focuses on solid-state electrolytes and Gelion's sulfur-based cathode technology to achieve cost targets. Gelion, listed on the London Stock Exchange's AIM, was founded in 2015 from the University of Sydney and specializes in lithium-sulfur and zinc-bromide energy storage.

rss · Electrek · Jun 4, 17:26

**Background**: Solid-state batteries replace liquid electrolytes with solid materials, offering higher energy density, improved safety, and longer life. They are considered the next frontier for EVs but are expensive to produce. Chinese manufacturers currently dominate the global battery market, prompting automakers like Nissan to seek affordable alternatives.

<details><summary>References</summary>
<ul>
<li><a href="https://electrek.co/2026/06/04/nissan-solid-state-ev-battery-project-aims-for-cheaper-than-china/">Nissan solid-state EV battery project aims for 'Cheaper Than ...</a></li>
<li><a href="https://gelion.com/">Next-Generation Sulfur Battery Technologies | Gelion</a></li>
<li><a href="https://battery-tech.net/company/gelion/">Gelion - Battery-Tech Network</a></li>

</ul>
</details>

**Tags**: `#solid-state batteries`, `#EV`, `#battery technology`, `#Nissan`

---

<a id="item-12"></a>
## [BMW iX3 sets record 485-mile range in NAF test](https://electrek.co/2026/06/04/bmws-new-ix3-drove-485-miles-longest-range-ev-naf-test/) ⭐️ 6.0/10

BMW's new iX3 drove 485 miles on a single charge, achieving the longest range of any electric vehicle in the NAF and Motor summer range test. This milestone demonstrates that BMW's new generation EV platform can compete with and surpass current range leaders like Lucid and Tesla, potentially shifting consumer preferences toward BMW's electric offerings. The NAF test is known for realistic driving conditions, so the 485-mile result reflects real-world range rather than optimistic lab figures. The iX3 likely uses BMW's Gen6 battery technology with cylindrical cells.

rss · Electrek · Jun 4, 14:26

**Background**: The NAF (Norwegian Automobile Federation) conducts biannual summer and winter range tests, widely regarded as among the most realistic EV range assessments globally. BMW's iX3 is an all-electric SUV built on the Neue Klasse platform, which launched in 2025. The previous range record in NAF tests was held by Lucid Air Grand Touring.

<details><summary>References</summary>
<ul>
<li><a href="https://www.naf.no/elbil/elprix">El Prix 2026 – verdens største elbiltest | NAF</a></li>
<li><a href="https://insideevs.com/news/762220/summer-group-range-test-norway/">This Big EV Range Test In Norway Had A Winner, In A Strange Way</a></li>

</ul>
</details>

**Tags**: `#electric vehicles`, `#BMW`, `#range test`, `#automotive`

---

<a id="item-13"></a>
## [xAI buys $269M Tesla Megapacks in single month for AI data centers](https://electrek.co/2026/06/04/spacex-xai-269-million-tesla-megapack-purchase-s1-filing/) ⭐️ 6.0/10

SpaceX's amended S-1 IPO filing reveals that xAI purchased another $269 million worth of Tesla Megapack products in April 2026 alone, bringing total spending on Megapacks since 2024 to approximately $1 billion. This massive energy storage investment highlights the enormous power consumption of AI data centers and underscores the deepening business ties among Elon Musk's companies, with significant implications for the grid and renewable energy integration. The $269 million expenditure in a single month exceeds xAI's total Megapack spending for all of 2024. The purchases are part of xAI's buildout of the Colossus supercomputer, which demands massive amounts of electricity.

rss · Electrek · Jun 4, 12:58

**Background**: The Tesla Megapack is a large-scale lithium-ion battery energy storage system designed for grid and utility use, capable of storing up to 3.9 MWh per unit. AI data centers, such as those operated by xAI, require vast amounts of energy, making on-site battery storage essential for stabilizing power supply and reducing costs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tesla_Megapack">Tesla Megapack</a></li>
<li><a href="https://www.tesla.com/megapack">Megapack - Tesla</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Energy`, `#Tesla`, `#SpaceX`, `#Data Centers`

---

<a id="item-14"></a>
## [Waymo Repurposes Retired Robotaxi Batteries for Grid Storage](https://electrek.co/2026/06/04/waymo-retired-robotaxi-batteries-are-heading-back-to-work-b2u/) ⭐️ 6.0/10

Waymo announced that retired batteries from its robotaxi fleet will be repurposed to support the power grid in California and Texas, instead of being recycled immediately. This initiative demonstrates a practical, real-world use case for second-life EV batteries, potentially reducing battery waste and providing low-cost energy storage for the grid. The repurposed batteries will be deployed in stationary energy storage systems in California and Texas, though specific partners, capacity, and timelines have not yet been disclosed.

rss · Electrek · Jun 4, 11:00

**Background**: Electric vehicle batteries typically retain 70-80% of their capacity after their automotive life ends, making them suitable for less-demanding stationary storage. Second-life battery projects have been explored by other automakers, but Waymo's large robotaxi fleet provides a consistent stream of retired packs, adding validation to the model.

**Tags**: `#EV batteries`, `#grid storage`, `#Waymo`, `#robotaxi`, `#energy`

---