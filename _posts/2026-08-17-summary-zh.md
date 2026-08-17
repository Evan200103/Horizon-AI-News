---
layout: default
title: "Horizon Summary: 2026-08-17 (ZH)"
date: 2026-08-17
lang: zh
---

> 从 46 条内容中筛选出 5 条重要资讯。

---

**科技新闻**
1. [Qwen 3.8 27B 性能出色但默认过度思考](#item-tech-news-1) ⭐️ 8.0/10
2. [Anthropic 公开 Claude 系统提示词](#item-tech-news-2) ⭐️ 8.0/10
3. [Direct File 项目兴衰记：政府科技与政治的交锋](#item-tech-news-3) ⭐️ 8.0/10
4. [SSOG-Attention：可分离高斯和实现次二次复杂度注意力](#item-tech-news-4) ⭐️ 8.0/10

**科技博客**
1. [Qwen 3.8 27B：强大但默认过度思考](#item-tech-blog-1) ⭐️ 8.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Qwen 3.8 27B 性能出色但默认过度思考](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 8.0/10

Qwen 3.8 27B 模型在消费级硬件上表现出色，但默认启用过度思考行为，引发社区广泛讨论。用户指出，当前所有主流模型都存在过度思考问题，这源于强化学习激励或蒸馏机制，导致模型在简单任务上产生不必要的冗长推理。社区成员分享了多种解决方案，包括修改推理努力参数、使用自定义提示词，以及开发专门的 llama.cpp 分支来控制推理过程。尽管存在这一缺陷，用户仍对本地模型在消费级硬件上的性能提升表示惊叹，认为其已接近一年前高端模型的推理水平。

hackernews · bilsbie · 8月16日 23:45 · [社区讨论](https://news.ycombinator.com/item?id=49324985)

**「背景」** Qwen 3.8 27B 是阿里巴巴 Qwen 研究实验室于 2026 年 8 月发布的一款 Apache 2.0 许可的 27B 参数视觉语言模型，属于 Qwen 开源模型系列的最新成员。该模型因其在消费级硬件上的出色性能而受到关注，但社区反馈指出其默认行为倾向于过度推理（overthinking），即生成不必要的冗长思考过程。

**「影响」** 对于在消费级硬件上运行 Qwen 3.8 27B 的开发者，过度思考行为会增加推理时间和计算资源消耗，但社区提供的 workaround（如调整推理努力参数或使用定制分支）可有效缓解，同时保持模型性能。

**「社区讨论」** 社区普遍认为过度思考是当前模型的通病，源于强化学习激励，但用户对本地模型的进步表示兴奋，并分享了多种控制推理过程的实用方案，包括修改 llama.cpp 分支和调整推理努力参数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://simonwillison.net/2026/Aug/16/qwen-38-27b/">Qwen 3.8 27B is excellent, but it defaults to wildly overthinking things</a></li>

</ul>
</details>

**标签**: `#Qwen`, `#LLM`, `#local models`, `#reasoning`, `#llama.cpp`

---

<a id="item-tech-news-2"></a>
### [Anthropic 公开 Claude 系统提示词](https://platform.claude.com/docs/en/release-notes/system-prompts) ⭐️ 8.0/10

Anthropic 在 Claude 平台文档中发布了 Claude 模型的系统提示词，公开了模型运行所依据的指令细节，这是提升透明度的重要举措。社区开发者 Simon Willison 将这些提示词整理成 Git 提交历史，便于追踪版本间的变化，例如 Opus 4.8 与 Opus 5 之间的差异，其中新增了关于“Claude Fable 5”和“Claude Mythos 5”的说明。有评论者指出，系统提示词中包含了诸如“提示词暗示有图片并不代表真有图片，Claude 需自行检查”等常识性指令，这引发了对模型“智能”本质的讨论。同时，也有开发者认为这些提示词篇幅过长，可能分散模型注意力，与业界建议的简洁指令相悖。

hackernews · tosh · 8月16日 12:48 · [社区讨论](https://news.ycombinator.com/item?id=49319556)

**「背景」** Anthropic 于 2024 年 8 月 26 日首次公开发布了其 Claude 模型的系统提示词，这些提示词用于指导模型在 Claude.ai 及移动应用中的行为。此前，Anthropic 研究员 Amanda Askell 曾在 2024 年 3 月详细解析过系统提示词，但此次是官方首次正式发布。系统提示词是模型运行的核心指令，通常被视为商业机密，因此 Anthropic 的这一透明度举措在 AI 社区中引起了广泛关注。

**「影响」** 对于使用 Claude API 的开发者而言，公开的系统提示词提供了更清晰的模型行为预期，有助于优化提示词设计和调试；同时，社区对提示词内容的分析也可能促使 Anthropic 进一步调整其提示策略。

**「社区讨论」** 社区对系统提示词的公开反应积极，Simon Willison 的 Git 历史整理尤其受到好评，方便了版本对比。然而，也有评论者质疑提示词的长度和具体性，认为这可能与业界倡导的简洁指令相悖，并引发了对模型智能本质的讨论。此外，有用户担忧论坛存在对 AI 负面新闻的压制，但这一观点与本文主题关联不大。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2024/Aug/26/anthropic-system-prompts/">Anthropic Release Notes : System Prompts | Simon Willison’s Weblog</a></li>
<li><a href="https://beamstart.com/news/google-amazon-backed-openai-rival-17248365922191">Google, Amazon-Backed OpenAI-Rival Anthropic Releases &#x27; System ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#system prompts`, `#transparency`

---

<a id="item-tech-news-3"></a>
### [Direct File 项目兴衰记：政府科技与政治的交锋](https://www.ischool.berkeley.edu/sites/default/files/vinton_report_5.pdf) ⭐️ 8.0/10

这份由伯克利信息学院发布的报告，对美国政府直接报税系统 Direct File 项目进行了全面复盘，详细记录了其从构想到被终止的全过程。报告由项目团队成员撰写，虽带有主观视角，但力求客观平衡，既肯定了项目在简化报税流程、提升用户体验方面的成功，也剖析了其在政治博弈、官僚决策和开发时间压缩等方面的失败原因。项目因政治因素而非技术或绩效问题被终止，其开发周期因决策延误而缩短了 18 个月，最终未能持续运营。报告为政府科技项目与政治环境的互动提供了深刻教训，对软件工程师和科技行业从业者具有重要参考价值。

hackernews · ronbenton · 8月17日 00:17 · [社区讨论](https://news.ycombinator.com/item?id=49325185)

**「背景」** Direct File 是美国国税局（IRS）推出的一项免费在线报税服务，允许符合条件的纳税人直接向 IRS 提交联邦纳税申报表。该项目于 2024 年在 12 个州试点，随后扩展到 25 个州。然而，该计划面临政治和预算方面的不确定性，尤其是在特朗普政府时期，其未来受到质疑。

**「影响」** 该报告为政府科技项目管理者提供了关于政治风险、决策效率与开发时间压缩的实证案例，可能影响未来类似项目的规划与执行策略。

**「社区讨论」** 社区评论普遍认为报告写得精彩且平衡，但有人指出项目失败并非基于绩效，而是政治原因。有评论者关注到开发时间被压缩 18 个月的问题，并推测 AI 可能在未来改善此类决策效率。另有评论引用数据称政府每次申报成本约 226 美元，远高于私营公司的 40 美元，质疑其成本效益，但也表示愿意听取相反观点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/IRS_Direct_File">IRS Direct File - Wikipedia</a></li>
<li><a href="https://money.usnews.com/money/personal-finance/taxes/articles/these-states-can-now-file-taxes-directly-with-the-irs">These 25 States Can Now File Taxes Directly With the IRS | U.S. News</a></li>
<li><a href="https://www.kiplinger.com/taxes/will-irs-direct-file-continue-under-trump">IRS Direct File program is on Trump&#x27;s Chopping Block | Kiplinger</a></li>

</ul>
</details>

**标签**: `#government technology`, `#project management`, `#post-mortem`, `#politics`, `#software development`

---

<a id="item-tech-news-4"></a>
### [SSOG-Attention：可分离高斯和实现次二次复杂度注意力](https://www.reddit.com/r/MachineLearning/comments/1vpt6ay/ssogattention_sum_of_separable_gaussians_as_a/) ⭐️ 8.0/10

SSOG-Attention 提出了一种新的注意力机制，通过为每个头学习少量高斯原子，并根据查询令牌进行几何引导，将标准缩放点积注意力（SDPA）的复杂度从 O\(N²·d\) 降低到 O\(N·√N·d\)。实验表明，在 CIFAR-100 上 SSOG 明显优于 SDPA，在 ImageNet（IN1k）上性能相当且收敛更快，同时在大规模下具有更高的速度和内存效率。该工作提供了博客文章和开源代码仓库，并声明部分代码和博客内容由 AI 辅助生成。

reddit · r/MachineLearning · /u/4rtemi5 · 8月16日 10:06

**「背景」** 标准缩放点积注意力（SDPA）需要计算所有查询与键的相似度，导致计算复杂度为 O\(N²·d\)，在处理高分辨率图像或长序列时成为瓶颈。可分离高斯函数是一种可以分解为多个一维高斯乘积的数学形式，能够近似复杂的注意力分布，同时保持较低的计算成本。

**「影响」** 对于需要处理高分辨率图像或长序列的视觉模型，SSOG-Attention 提供了一种更高效的注意力替代方案，能在保持性能的同时显著降低计算和内存开销，尤其适合资源受限或大规模部署场景。

**标签**: `#attention mechanisms`, `#efficient transformers`, `#machine learning`, `#computer vision`, `#open source`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [Qwen 3.8 27B：强大但默认过度思考](https://simonwillison.net/2026/Aug/16/qwen-38-27b/) ⭐️ 8.0/10

rss · Simon Willison · 8月16日 22:00

**「背景」** Simon Willison 评测了阿里 Qwen 实验室新发布的 Qwen 3.8 27B，这是一个 Apache 2 许可的 27B 参数视觉语言模型，大小适合在笔记本电脑上运行。作者对其前代产品印象深刻，并期待这一代的性能提升。

**「方案」** 作者发现该模型默认的推理强度为“xhigh”，导致在简单任务上过度思考，消耗大量上下文和生成时间。例如，生成一个 SVG 图像用了 21 分钟和 22,276 个推理 token。他建议将推理强度调低或关闭，以获得更快的响应。模型在边界框标注和编码代理任务上表现出色，但速度较慢（约 15-30 token/秒）。作者尝试了多 token 预测（MTP）优化，通过 llama.cpp 的 --spec-type draft-mtp 参数，在 DGX Spark 上获得了约 72% 的性能提升。

**「启示」** Qwen 3.8 27B 展示了开放权重模型在 17GB 文件大小内实现长上下文、工具调用、视觉和代码生成能力的潜力，但默认的过度思考设置和速度是实际使用的瓶颈。

**标签**: `#Qwen 3.8 27B`, `#local LLM`, `#reasoning effort`, `#performance optimization`, `#vision model`

---