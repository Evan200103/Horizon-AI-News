---
layout: default
title: "Horizon Summary: 2026-08-04 (ZH)"
date: 2026-08-04
lang: zh
---

> 从 53 条内容中筛选出 5 条重要资讯。

---

**科技新闻**
1. [Swiftlet：在 Mac 和 iPhone 上高效运行大模型](#item-tech-news-1) ⭐️ 8.0/10
2. [OpenAI 公布数学与理论计算机科学十项进展](#item-tech-news-2) ⭐️ 8.0/10
3. [FFmpeg 9.0 发布：新增硬件加速与滤镜支持](#item-tech-news-3) ⭐️ 8.0/10
4. [探索性建模：预训练第三轴与端到端生成](#item-tech-news-4) ⭐️ 8.0/10

**科技博客**
1. [在共享 GPU 上运行隔离租户 Kubernetes 集群](#item-tech-blog-1) ⭐️ 7.0/10

---

## 科技新闻

<a id="item-tech-news-1"></a>
### [Swiftlet：在 Mac 和 iPhone 上高效运行大模型](https://github.com/leonickson1/Swiftlet) ⭐️ 8.0/10

Swiftlet 项目展示了在消费级硬件上运行大型语言模型的技术突破，能够在 Mac 上以 4.3GB 内存运行 80B 参数的 Qwen 模型，在 iPhone 上运行 35B 模型。该项目基于 TurboFieldfare 开发，并在 README 中致谢了该基础项目。这一成就通过高效的模型量化和内存管理实现，使得大模型推理不再依赖高端服务器硬件。尽管存在实际限制，如速度较慢和依赖外部存储，但社区认为这是迈向高效端侧 AI 的重要一步。

hackernews · leonickson · 8月3日 16:54 · [社区讨论](https://news.ycombinator.com/item?id=49158333)

**「背景」** Swiftlet 是一个开源项目，基于 llama.cpp 实现，旨在通过内存映射和流式加载等技术，在资源受限的设备上高效运行大型语言模型。它支持在 Mac 上以 4.3 GB 内存运行 80B 参数的 Qwen 模型，在 iPhone 上运行 35B 模型。该项目还衍生出 iOS 应用 Priv AI，该应用将 SwiftletCore 作为其流式模型引擎，用户可直接下载模型进行聊天。

**「影响」** 对于拥有 Mac 或 iPhone 的开发者，Swiftlet 使得在本地运行大型语言模型成为可能，降低了硬件门槛，并可能推动更多端侧 AI 应用的发展。

**「社区讨论」** 社区普遍持积极态度，认为尽管当前方案存在不实用之处，但这是进步的过程，并期待未来更大模型能在低成本硬件上运行。有用户指出苹果可能押注于未来 LLM 的高效性，使其能在 iPhone 上运行。同时，也有用户关注本地模型无法访问网络索引的问题，认为这是主要限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/leonickson1/Swiftlet">GitHub - leonickson1/Swiftlet · GitHub</a></li>

</ul>
</details>

**标签**: `#on-device AI`, `#LLM inference`, `#efficient memory`, `#Apple Silicon`, `#open source`

---

<a id="item-tech-news-2"></a>
### [OpenAI 公布数学与理论计算机科学十项进展](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 8.0/10

OpenAI 发布文章，宣称在数学和理论计算机科学领域取得十项最新进展，但具体细节未在提供的内容中说明。这一消息在 Hacker News 上引发热烈讨论，帖子获得 563 分和 850 条评论，反映出 AI 社区对 AI 在数学发现中作用的广泛关注。讨论中，有评论者认为 AI 正在以指数级速度提升数学证明的生成与验证能力，但也有人指出 AI 仍无法像人类数学家那样进行直觉性猜想。整体来看，该事件标志着 AI 在数学推理方面的显著进步，并可能对相关领域的研究方式产生深远影响。

hackernews · milkshakes · 8月3日 16:27 · [社区讨论](https://news.ycombinator.com/item?id=49157930)

**「背景」** OpenAI 发布了一份 249 页的手稿，声称在纯数学和理论计算机科学领域取得了十项新成果，涵盖几何、密码学和复杂性理论等方向，并计划为每项成果提供 Lean 4 形式的机器可验证证书。这些成果针对长期未解决的开放问题，标志着 AI 在数学推理和证明验证方面的重要进展。

**「影响」** 对于数学和理论计算机科学领域的研究者而言，OpenAI 的这十项进展可能意味着 AI 辅助证明和问题求解将变得更加可行，从而加速某些计算性问题的解决，但具体影响程度取决于这些进展的实际内容和可复现性。

**「社区讨论」** 社区讨论中，有评论者将 AI 的发展比作指数级增长，认为数学领域正被这种增长所“吞噬”，而写作等领域则相对顽固；也有评论者指出，尽管当前模型无法进行直觉性猜想，但可以快速证伪某些猜想，这可能会颠覆一些数学家的研究计划。此外，还有人认为 AI 的影响已不可否认，呼吁人们正视并认真对待这一趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/ten-advances-in-mathematics/">Ten advances in mathematics and theoretical computer ... | OpenAI</a></li>
<li><a href="https://beyondtmrw.org/article/ten-advances-in-mathematics-and-theoretical-computer-science">OpenAI Mathematics Advances : Ten Breakthroughs in 2026</a></li>

</ul>
</details>

**标签**: `#AI research`, `#mathematics`, `#theoretical computer science`, `#OpenAI`, `#machine learning`

---

<a id="item-tech-news-3"></a>
### [FFmpeg 9.0 发布：新增硬件加速与滤镜支持](https://github.com/FFmpeg/FFmpeg/blob/n9.0/RELEASE_NOTES) ⭐️ 8.0/10

FFmpeg 9.0 作为这一广泛使用的多媒体框架的重大更新版本正式发布，引入了多项新特性。新版本新增了 ProRes RAW 的 VideoToolbox 硬件加速和 APV Vulkan 硬件加速，以及 AMF 帧率转换滤镜（vf\_frc\_amf）和 v360\_vulkan 滤镜。此外，还增加了对 HE-AAC 960（DAB+）解码、SMPTE 2094-50 元数据支持与透传、动画 WebP 解码器和分离器，以及 Playdate 视频编码器和封装器的支持。同时，FFmpeg 9.0 扩展了 AMF 颜色转换器（vf\_vpp\_amf）的 HDR 能力，并在 MP4 封装器中加入了 LCEVC 轨道复用支持。值得注意的是，该版本移除了 CELT 解码支持（不影响 Opus CELT）。

hackernews · gyan · 8月4日 09:30 · [社区讨论](https://news.ycombinator.com/item?id=49166202)

**「背景」** FFmpeg 是一个广泛使用的开源多媒体框架，提供录制、转换以及流式传输音频和视频的功能。它包含一系列库和命令行工具，支持几乎所有已知的编解码器和格式。FFmpeg 9.0 是该项目的重大版本更新，引入了新的编码器、解码器、滤镜以及硬件加速支持，例如 ProRes RAW 的 VideoToolbox 硬件加速和 APV Vulkan 硬件加速。此次发布延续了 FFmpeg 持续演进的传统，为多媒体处理提供更强大的功能和更广泛的兼容性。

**「影响」** 对于依赖 FFmpeg 进行视频处理和转码的开发者与组织，此次更新提供了更广泛的硬件加速选项和新的滤镜功能，有助于提升处理效率并扩展格式支持。

**「社区讨论」** 社区普遍对 FFmpeg 9.0 表示赞赏，认为该开源项目对多媒体领域至关重要。部分用户表达了未来改进的期望，例如在 Windows 笔记本上启用 Intel QSV 编码，以及探索用描述性语言自动生成多媒体格式代码的可能性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/FFmpeg-9.0-Released">FFmpeg 9 . 0 Released With More Vulkan Acceleration... - Phoronix</a></li>

</ul>
</details>

**标签**: `#FFmpeg`, `#multimedia`, `#video encoding`, `#hardware acceleration`, `#open source`

---

<a id="item-tech-news-4"></a>
### [探索性建模：预训练第三轴与端到端生成](https://www.reddit.com/r/MachineLearning/comments/1vf6r6f/explorative_modeling_unlocking_a_third/) ⭐️ 8.0/10

一篇新论文提出了“探索性建模”作为预训练的第三轴，并引入端到端生成方法，旨在扩展传统预训练范式。该概念可能为机器学习领域带来重要的概念性进展，但帖子中缺乏详细技术内容，限制了验证。Reddit 机器学习社区对此展开了讨论，表明社区对该方向感兴趣。论文作者为 Gladstone 等人，发表于 2026 年。

reddit · r/MachineLearning · /u/Benlus · 8月4日 10:42

**「背景」** 传统生成模型的预训练主要沿两个轴扩展：参数规模和数据量。该论文提出“探索性建模”（Explorative Modeling, XM）作为第三个预训练轴，通过增加探索程度来提升模型性能，并在图像、视频和语言等连续与离散领域均观察到单调改进。此外，XM 支持端到端的重建式生成，在控制任务上能以比扩散模型少 16 至 256 倍的推理步骤达到相当性能，且生成过程保持单步、训练与推理一致。

**「影响」** 如果该概念得到验证，可能为预训练研究开辟新方向，影响生成模型的设计和训练方式。但目前缺乏具体技术细节，实际影响尚不确定。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://alexiglad.github.io/blog/2026/explorative_modeling/">Explorative Modeling -- Unlocking a Third Pretraining Axis and...</a></li>
<li><a href="https://paperswithcode.co/paper/2607.27372">Explorative Modeling : Unlocking a Third Pretraining Axis and...</a></li>
<li><a href="https://www.alphaxiv.org/abs/2607.27372">Explorative Modeling : Unlocking a Third Pretraining Axis ... | alphaXiv</a></li>

</ul>
</details>

**标签**: `#pretraining`, `#machine learning`, `#generative models`, `#research`, `#AI`

---

## 科技博客

<a id="item-tech-blog-1"></a>
### [在共享 GPU 上运行隔离租户 Kubernetes 集群](https://developer.nvidia.com/blog/how-to-run-isolated-tenant-kubernetes-clusters-on-shared-gpu-infrastructure/) ⭐️ 7.0/10

rss · NVIDIA Technical Blog · 8月3日 16:00

**「背景」** 为每个团队运行专用 Kubernetes 集群往往导致过度隔离，而共享单个集群又面临协调成本高、CRD 版本冲突、RBAC 重叠以及难以将 GPU 容量划分为团队预算等问题。作者提出了一种模式，在保持团队自主性的同时不拆分硬件。

**「方案」** 该方案结合了 KAI Scheduler 和 vCluster 两个开源工具。KAI Scheduler 负责 GPU 资源的公平分配，支持层级队列、保证配额和超配额能力；vCluster 则为每个团队提供独立的控制平面，包括 API 服务器、CRD 和 RBAC，但共享底层节点和 GPU。教程详细演示了在单块 NVIDIA L40S GPU 上为三个团队（NLP、视觉、推荐系统）创建隔离集群的过程。关键步骤包括：安装 KAI Scheduler 并启用 GPU 共享，定义层级队列（父队列 ml-org 配额为 1 GPU，子队列各保证 0.33 GPU），创建 vCluster 时设置 setOwner: false 以保留所有权链，然后每个团队通过自己的 vCluster 部署带有 schedulerName: kai-scheduler 和队列标签的 Pod。验证结果显示三个 Pod 运行在同一物理节点上，每个团队只能看到自己的 Pod，队列状态显示分配了 330m GPU。作者指出，KAI Scheduler 不提供硬件级内存隔离，应用需自行限制内存使用，如需硬隔离可结合 MIG。

**「启示」** 作者的核心论点是，通过 KAI Scheduler 和 vCluster 的组合，可以在共享 GPU 基础设施上为多个团队提供专用集群的体验，实现零浪费，答案不是增加 GPU，而是更好地利用现有基础设施。

**标签**: `#Kubernetes`, `#GPU sharing`, `#multi-tenancy`, `#KAI Scheduler`, `#vCluster`

---