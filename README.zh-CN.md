# Awesome AI Short Drama 🎬

> AI 短剧、微短剧、动态漫及叙事视频创作相关的开源智能体、生产系统、研究论文、工作流与资源精选。

[English](README.md) · **简体中文**

## About

**Awesome AI Short Drama** is a curated list of open-source agents, tools, research,
workflows, models, and resources for AI short-drama and micro-series production.

本目录重点关注能够解决下列一个或多个问题的项目：

- 小说、故事或一句话创意到多集剧本；
- 角色、服装、场景和道具的跨镜头一致性；
- 分镜、首尾帧、镜头运动和摄影机规划；
- 图像、视频、配音、音乐及音效生成；
- 多智能体导演、审核与返工机制；
- 时间线、字幕、剪辑、合成及成片导出；
- 面向短剧的评测基准、数据集和生产方法论。

> [!NOTE]
> GitHub Stars 和项目状态核验于 **2026-06-29**。Stars 会持续变化；许可证以项目仓库
> 中的 `LICENSE` 和作者声明为准。`开源` 不等于 `可免费商用`，依赖商业模型 API 的项目
> 也不等于完全本地运行。

## 标记说明

- 🏆：与 AI 短剧高度相关、链路较完整；
- 📄：有对应论文或技术报告；
- 🏠：支持本地或自托管部署；
- 🧩：Agent Skill、能力组件或集成层；
- 🧪：研究原型或早期项目；
- 💳：主要生成能力需要第三方商业 API；
- ⚠️：非商用许可、源码不完整或许可证未声明。

## 项目分类

### 端到端短剧与动态漫生产系统

| 项目 | 出品团队 | 简介 | 许可证 | Stars | 备注 |
|---|---|---|---:|---:|---|
| 🏆🏠 [Toonflow](https://github.com/HBAI-Ltd/Toonflow-app) | HBAI Ltd | 小说/剧本到动画短剧；提供编剧、分镜、角色、视频生成、三层 Agent 和无限画布工作台 | Apache-2.0 | 10.6k | 桌面端/服务器部署；实际生成需要配置模型服务 |
| 🏆⚠️ [Huobao Drama](https://github.com/chatfire-AI/huobao-drama) | Chatfire AI | 一句话到剧本、角色、分镜、配音、视频与整集导出的自动化平台 | CC BY-NC-SA 4.0 | 13.0k | **非商用许可**；内置 Mastra Agents，支持多家模型 API |
| 🏆🏠 [Jellyfish](https://github.com/Forget-C/Jellyfish) | Forget-C / 社区 | 面向 AI 短剧的生产工作区，强调剧本拆解、资产复用、一致性管理、生成任务和导出 | Apache-2.0 | 4.6k | Docker Compose；MySQL、Redis、对象存储等完整后端 |
| 🏆🏠 [ArcReel](https://github.com/ArcReel/ArcReel) | ArcReel | Agent 驱动的小说到视频工作台，覆盖角色/场景/道具、标准剧本、分镜图与视频 | AGPL-3.0 | 3.0k | Claude Agent SDK；需关注 AGPL 网络服务义务 |
| 🏆 [VideoClaw](https://github.com/HITsz-TMG/VideoClaw) | HITsz-TMG / Lychee Agent | 从创意、剧本、角色场景、分镜和参考图到视频生成、剪辑及导出的 AI 视频员工 | MIT | 1.5k | 支持 OpenClaw Skill、多集续写；展示 8 集真人短剧和 5 集动态漫 |
| 🏆 [LumenX Studio](https://github.com/alibaba/lumenx) | Alibaba | 小说到短漫剧：资产提取、风格定义、资产生成、分镜脚本、分镜图和视频生成 | MIT | 764 | 原生集成 Qwen 与 Wan 系列能力 |
| ⚠️🏠 [AI Story](https://github.com/xhongc/ai_story) | xhongc | 自托管故事视频生产平台，覆盖文案创作、分镜、图片生成、运镜规划、图生视频和项目管理 | CC BY-NC-SA 4.0（README） | 987 | 与短剧直接相关、源码较完整，但为非商用许可；多集叙事和一致性机制公开说明较弱 |
| 🏆🏠 [LocalMiniDrama](https://github.com/xuanyustudio/LocalMiniDrama) | Xuanyu Studio | 本地短剧/漫剧工作流，从故事、分镜到视频，项目数据保存在本机 | MIT | 738 | “本地”主要指数据和工作台；云端生成仍需相应 API |
| 🧪💳 [Open AI Micro Drama Generator](https://github.com/Anil-matcha/Open-AI-Micro-Drama-Generator) | Anil Matcha | 编剧→分镜→画面→视频的多智能体微短剧流水线 | MIT（README） | 359 | 轻量参考实现；主要通过 muapi.ai 调用视频模型 |
| 🧩 [OnlyShot](https://github.com/A-cat-with-carrots/OnlyShot) | 神仙鱼 / 独立开发者 | 面向工业化 AI 短剧流程的 Claude Skill，从一句想法到剧本、分镜、分镜图、视频和剪辑包 | MIT | 158 | 沉淀短剧钩子、节奏、Story Bible，并集成 Dreamina/Seedance 与 17 类失败模式 |
| 🧪🏠 [dramai](https://github.com/hyyyyyyz/dramai) | 独立开发者 | 浏览器内的零后端短剧工作台：文本→分镜→图片→视频→剪映 | Apache-2.0 | 19 | 早期项目，适合作为纯前端工作流参考 |
| 🧪💳 [AIDrama Studio](https://github.com/EvoLinkAI/ai-short-drama) | EvoLinkAI | 小说/故事到剧本分析、分镜、图片、视频、配音和成片 | 曾声明 MIT | — | **2026-06-28 仓库无法访问**；此前版本依赖 EvoLink API，暂不列为可用项目 |

### 工作流标杆与相邻视频生产系统

| 项目 | 出品团队 | 简介 | 许可证 | Stars | 与短剧的关系 |
|---|---|---|---:|---:|---|
| ⚠️ [BigBanana AI Director](https://github.com/shuyu-labs/BigBanana-AI-Director) | Shuyu Labs | Script-to-Asset-to-Keyframe 工业化流程，覆盖季/集管理、资产库、九宫格、首尾帧和粗剪 | CC BY-NC-SA 4.0 | 1.5k | 高度相关，但非商用；公开仓库现为历史参考版本，后续更新通过官方 Docker 镜像发布 |
| 🏠 [Pixelle-Video](https://github.com/AIDC-AI/Pixelle-Video) | AIDC-AI | AI 全自动短视频引擎，执行创意规划、素材生成与视频合成 | Apache-2.0 | 23.7k | 更偏通用短视频，但其自动化架构和 Skill 设计值得复用 |
| 🏠 [OpenMontage](https://github.com/calesthio/OpenMontage) | Calesthio AI Labs | 面向编码智能体的完整视频生产系统，含研究、剧本、素材、剪辑、合成和质量门禁 | AGPL-3.0 | 25.9k | 非短剧专用；适合借鉴 provider 选择、成本治理、审核和可复现流水线 |
| 🏠 [VibeFrame](https://github.com/vericontext/vibeframe) | VeriContext | CLI-first、MCP-ready 的 AI 原生视频编辑器，使用 Storyboard/Design 文件驱动生成和修订 | MIT | 140 | 可作为短剧分镜、素材构建、时间线和成片检查的基础设施 |

### 剪辑与后期制作

| 项目 | 出品团队 | 简介 | 许可证 | Stars | 备注 |
|---|---|---|---:|---:|---|
| 🧩🏠 [FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline) | FireRedTeam | 自然语言驱动的 AI 视频剪辑 Agent，包含规划、素材检索、配音/BGM/字体推荐和可复用 Style Skills | Apache-2.0 | 3.0k | 支持 OpenClaw、Claude Code、Codex Skill；[官方演示](https://fireredteam.github.io/demos/firered_openstoryline/) |
| 🏠 [VibeFrame](https://github.com/vericontext/vibeframe) | VeriContext | 生成、编辑、字幕、配音、音乐、渲染与自动检查 | MIT | 140 | 主条目位于上一节，此处作为后期能力索引 |
| 🏠 [OpenMontage](https://github.com/calesthio/OpenMontage) | Calesthio AI Labs | Remotion/HyperFrames/FFmpeg 合成、字幕、音频混合、颜色和交付质量检查 | AGPL-3.0 | 25.9k | 主条目位于上一节 |

### Agent Skills 与模型能力集成

| 项目/Skill | 团队 | 能力 | 许可证 / Stars | 注意事项 |
|---|---|---|---|---|
| 🧩 [libtv-skills](https://github.com/libtv-labs/libtv-skills) | LibTV Labs | 将 LibLib.tv 图片/视频 OpenAPI 封装为 OpenClaw 兼容 Skill | MIT / 781 | 是能力适配层，不是完整短剧系统 |
| 🧩 [VideoClaw Skill](https://github.com/HITsz-TMG/VideoClaw) | HITsz-TMG | 在 OpenClaw 中通过对话启动完整视频/短剧生成 | MIT / 1.5k | 可通过 ClawHub 安装；执行前仍需审核配置及 API 权限 |
| 🧩 [Drama Generator](https://clawhub.ai/zhenstaff/drama-generator) | ClawHub 社区 | 多角色剧本、OpenAI TTS、Whisper 和 Remotion 合成 | 未核验 | 更接近动态图形/有声剧，非电影级生成 |
| 🧩 [One Click Video Creation](https://clawhub.ai/zuoyuting214/skills/zyt-one-click-video-creation) | ClawHub 社区 | 文案、分镜、TTS、数字人与 AI 素材混剪 | 未核验 | 依赖外部模型与 FFmpeg |
| 🧩 [Video Cog](https://clawhub.ai/nitishgargiitd/video-cog) | ClawHub 社区 | 主题到脚本、配音、音乐和剪辑 | 未核验 | 依赖托管服务，需检查数据和计费条款 |
| 🧩 [Image Storyboard](https://clawhub.ai/dlazyai/image-storyboard) | ClawHub 社区 | 先规划、后渲染的图片分镜 Skill | 未核验 | 第三方 API 依赖 |
| 🧩 [canghe-skills](https://github.com/freestylefly/canghe-skills) | 苍何 / 社区 | Skills 合集，包含 Seedance 漫剧生成技能 | 未声明 / 356 | 合集质量不一，应逐个检查脚本和依赖 |

> [!WARNING]
> Agent Skill 可能执行脚本、访问文件系统和网络，并读取 API Key。安装前应阅读源码、固定版本、
> 使用最小权限和隔离环境，不要把 ClawHub 页面上的“可安装”直接等同于“已安全审计”。

### 多智能体影视与叙事研究原型

| 项目 | 出品团队 | 研究方向 | 许可证 | Stars | 论文 |
|---|---|---|---:|---:|---|
| 📄 [ViMax](https://github.com/HKUDS/ViMax) | HKU Data Science Lab | 导演、编剧、制片和生成器一体化的 Agentic Video Generation | MIT | 10.7k | 仓库内研究说明 |
| 📄 [MovieAgent](https://github.com/showlab/MovieAgent) | Show Lab / NUS | 导演、编剧、分镜师和场景经理多 Agent，通过分层 CoT 生成多场景长视频 | 未声明 | 345 | [论文](https://arxiv.org/abs/2503.07314) · [项目页](https://weijiawu.github.io/MovieAgent/) |
| 📄 [MM-StoryAgent](https://github.com/X-PLUG/MM_StoryAgent) | Alibaba X-PLUG、上海交大、华东师大 | 文字、角色一致图像、旁白、音乐和音效的多智能体故事视频 | Apache-2.0 | 307 | [论文](https://arxiv.org/abs/2503.05242) |
| 📄 [Anim-Director & AniMaker](https://github.com/HITsz-TMG/Anim-Director) | HITsz-TMG | LMM 动画导演与 MCTS 驱动的多 Agent 长篇动画生成 | 未声明 | 253 | [Anim-Director](https://arxiv.org/abs/2408.09787) · [AniMaker](https://arxiv.org/abs/2506.10540) |
| 📄 [DramaDirector](https://github.com/iLearn-Lab/DramaDirector) | iLearn-Lab | 几何引导的短剧生成研究原型，结合分镜规划、文图奖励学习、深度/姿态检索和 DramaBoard 基准 | MIT | 1 | [论文](https://arxiv.org/abs/2606.24107) |
| 📄 [FilmAgent](https://arxiv.org/abs/2501.12909) | HITsz-TMG 等 | 在 3D 虚拟空间中模拟导演、编剧、演员和摄影师完成影视预演 | — | — | 原 GitHub 地址目前重定向至 VideoClaw，故不重复统计仓库 Stars |

## 研究论文与基准

### 直接面向短剧

- **[DramaDirector: Geometry-Guided Short Drama Generation](https://arxiv.org/abs/2606.24107)**  
  Hengji Zhou 等，2026。通过分镜规划、文图对齐奖励以及从真实短剧镜头中检索深度/姿态条件，
  引导首帧与图生视频生成；同时提出 **DramaBoard**，由 35 部真人短剧、2.8K 集、81K 镜头构成。
- **[One Sentence, One Drama: Personalized Short-Form Drama Generation via Multi-Agent Systems](https://arxiv.org/abs/2605.22144)**  
  Yufei Shi 等，2026。使用多 Agent 辩论改进短剧节奏，以 3D 场景约束首帧空间一致性，
  并通过多阶段 Reviewer 返工剧本、视觉和视频；同时提出 **Short-Drama-Bench**。

### Agentic Video / 电影叙事

- **[Co-Director: Agentic Generative Video Storytelling](https://arxiv.org/search/?query=Co-Director%3A+Agentic+Generative+Video+Storytelling&searchtype=title)**  
  Yale Song 等，2026。分层多 Agent、全局多臂老虎机搜索与局部多模态自修订；
  提出 400 个虚构商品场景组成的 **GenAD-Bench**。[项目页](https://co-director-agent.github.io/)
- **[MovieAgent: Automated Movie Generation via Multi-Agent CoT Planning](https://arxiv.org/abs/2503.07314)**  
  从剧本和角色库自动规划场景、镜头、摄影与角色交互。
- **[FilmAgent: A Multi-Agent Framework for End-to-End Film Automation in Virtual 3D Spaces](https://arxiv.org/abs/2501.12909)**  
  在 3D 空间中研究多工种 Agent 协同和中间结果审核。
- **[Mind-of-Director: Multi-modal Agent-Driven Film Previsualization via Collaborative Decision-Making](https://arxiv.org/abs/2603.14790)**  
  聚焦剧本、虚拟场景、角色行为和摄影机规划的电影预演。
- **[Agentic Video Generation: From Text to Executable Event Graphs via Tool-Constrained LLM Planning](https://arxiv.org/abs/2604.10383)**  
  使用可执行的时空事件图和 3D 引擎保证物理及语义约束。

### 动画、故事视频与多模态

- **[Anim-Director: A Large Multimodal Model Powered Agent for Controllable Animation Video Generation](https://arxiv.org/abs/2408.09787)**  
  SIGGRAPH Asia 2024；LMM 驱动的可控动画导演。
- **[AniMaker: Multi-Agent Animated Storytelling with MCTS-Driven Clip Generation](https://arxiv.org/abs/2506.10540)**  
  SIGGRAPH Asia 2025；使用 MCTS 选择和优化长篇动画片段。
- **[MM-StoryAgent: Immersive Narrated Storybook Video Generation with a Multi-Agent Paradigm across Text, Image and Audio](https://arxiv.org/abs/2503.05242)**  
  多阶段故事写作、角色一致图像和多声道音频；可替换各模态工具。
- **[ViStoryBench: Comprehensive Benchmark Suite for Story Visualization](https://openaccess.thecvf.com/content/CVPR2026/html/Zhuang_ViStoryBench_Comprehensive_Benchmark_Suite_for_Story_Visualization_CVPR_2026_paper.html)**  
  CVPR 2026 故事可视化评测资源，可用于补充短剧的跨镜头一致性评价。

### 官方教程、项目页与文章

- [Toonflow 12 分钟快速上手](https://www.bilibili.com/video/BV1oXD7BqEqJ)；
- [FireRed-OpenStoryline 官方演示与说明](https://fireredteam.github.io/demos/firered_openstoryline/)；
- [MovieAgent 官方项目页](https://weijiawu.github.io/MovieAgent/)；
- [AniMaker 官方项目页](https://animaker-dev.github.io/)；
- [Co-Director 官方项目页](https://co-director-agent.github.io/)；
- [万兴科技 ReelClaw 发布报道](https://stock.10jqka.com.cn/20260320/c675451429.shtml)及
  [测试进展报道](https://www.nbd.com.cn/articles/2026-04-17/4345080.html)。

没有找到可信官方博客或公众号原文的项目，暂以项目 README、论文和项目主页作为一手资料；
不使用无法确认出处的转载文章补位。

## Awesome Lists 与持续发现入口

| 资源 | 说明 | Stars / 状态 |
|---|---|---:|
| [GitHub `ai-short-drama` Topic](https://github.com/topics/ai-short-drama) | 当前最直接的短剧开源项目动态入口 | 动态 |
| [GitHub `ai-storyboard` Topic](https://github.com/topics/ai-storyboard) | 分镜、Story Bible 和剧本到视频工具 | 动态 |
| [GitHub `openclaw-skills` Topic](https://github.com/topics/openclaw-skills) | OpenClaw 视频、图像、音频和自动化 Skills | 动态 |
| [ClawHub](https://clawhub.ai/) | 搜索 `drama`、`storyboard`、`video creation` 等 Skill | 动态 |
| [awesome-ai-short-drama-tools](https://github.com/clipcurator/awesome-ai-short-drama-tools) | 已有同类短剧工具列表 | 6；内容较少且偏产品推广，只作为线索源 |
| [awesome-openclaw](https://github.com/rylena/awesome-openclaw) | 通用 OpenClaw 资源列表 | 29；非短剧专属 |
| [awesome-seedance](https://github.com/ZeroLu/awesome-seedance) | Seedance 提示词、工作流和电影/短剧案例 | 2.0k |

GitHub `ai-short-drama` Topic 中还出现了一组由
[clipcurator](https://github.com/clipcurator) 发布的制作模板，包括 production workflow、
budget、greenlight committee、concept validation 和 casting kits。它们适合作为生产清单参考，
但当前社区验证较少，不与完整生成系统同级推荐。

## 商业与闭源项目观察

以下项目与赛道相关，但未找到可验证的完整开源仓库，**不计入开源主榜**。

| 项目 | 团队 | 定位 | 当前判断 |
|---|---|---|---|
| [ShortClaw](https://shortapi.ai/claws/shortclaw/) | ShortAPI | OpenClaw 桌面运行环境，多 Agent、定时任务和 Skill 管理 | 通用运行时，不是短剧专用；未核实到清晰的公开源码仓库 |
| [ShortAPI VideoClaw](https://shortapi.ai/claws/videoclaw/) | ShortAPI | 导演、图像、视频、音频、特效多 Agent 视频生产 | 与 HITsz-TMG VideoClaw **不是同一项目**；暂按商业产品处理 |
| ReelClaw | Wondershare / 万兴科技 | 基于 OpenClaw 的创意到成片视频 Agent | 尚处测试打磨阶段；[发布报道](https://stock.10jqka.com.cn/20260320/c675451429.shtml) · [后续进展](https://www.nbd.com.cn/articles/2026-04-17/4345080.html) |
| [CreatorClaw](https://creatorclaw.ai/) | CreatorClaw | 面向创作者的全流程 Agent | 内测/商业产品，未发现完整开源仓库 |
| [AivoClaw](https://www.aivoclaw.cn/) | AivoClaw | 企业短视频、数字人与内容生产 Agent | 商业产品 |
| [Ima Claw](https://www.imaclaw.bot/) | Ima Claw | 多镜头、分镜和创意生成 Skills 生态 | 可作为能力生态观察，非核心开源短剧系统 |
| [PlotParty](https://www.plotparty.ai/) | PlotParty | 角色一致、剧情连贯和多分钟叙事视频 | 商业平台 |
| Zopia | 未核实 | 多 Agent 视频导演，主打短剧、电影和品牌视频 | 目前主要为媒体报道，缺少可验证开源仓库 |

## 容易混淆的项目名称

| 名称 | 核查结果 |
|---|---|
| **VideoClaw** | 至少存在 HITsz-TMG 开源项目和 ShortAPI 商业产品两个不同实体，引用时必须带团队名 |
| **FilmClaw** | 截至核验日未发现可信、成熟的同名开源短剧项目；不要与 FilmAgent 混淆 |
| **MovieClaw** | 未发现可信的同名开源项目；相关学术项目是 MovieAgent |
| **ShortClaw** | 已有产品，但定位是通用 OpenClaw 桌面端，不应因名称中的 `Short` 误判为短剧工具 |
| **ReelClaw** | 至少有万兴视频 Agent 和其他 UGC/Reels Skill 使用该名称，需核对出品方 |

## 选择项目时建议检查

1. **许可证**：MIT/Apache-2.0 通常更利于二次开发；AGPL、CC BY-NC-SA 和未声明许可证需重点审查。
2. **源码完整性**：确认仓库不是只有前端、Docker 镜像、安装器或历史代码。
3. **模型依赖**：区分完全本地、可选云 API 和强绑定单一商业聚合服务。
4. **生产闭环**：检查是否真的完成分镜视频、音频、字幕和整集导出，而非只生成提示词或图片。
5. **连续性**：角色身份、服装、空间布局、画风和多集上下文是否有显式机制。
6. **可恢复性**：长耗时生成任务是否支持状态保存、失败重试、局部重生成和成本控制。
7. **维护状态**：最近提交、Issue 响应、Release 和文档是否仍然活跃。
8. **安全与隐私**：本地素材、未发布剧本和 API Key 是否会上传第三方平台。

## 贡献指南

欢迎通过 Issue 或 Pull Request 推荐项目。建议项目至少满足以下条件之一：

- 有可访问的公开源码或论文；
- 明确解决短剧生产链中的一个关键环节；
- 有可复现的安装说明、演示或实验结果；
- 相比通用文生视频模型提供了 Agent、工作流、一致性或评测方面的增量价值。

推荐条目请提供：

```yaml
name:
repo:
team:
category:
description:
tags: []
license:
deployment: []
commercial_api_required:
paper:
official_blog:
status:
last_verified:
notes:
```

项目结构化数据见 [`projects.yml`](projects.yml)。
