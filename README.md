# Awesome AI Short Drama 🎬

> A curated list of open-source agents, production systems, research, workflows, and resources for AI short dramas, micro-dramas, motion comics, and narrative video production.

**English** · [简体中文](README.zh-CN.md)

## About

This list focuses on projects that address one or more of the following:

- turning a novel, story, or one-line idea into episodic scripts;
- maintaining characters, costumes, scenes, and props across shots;
- generating storyboards, first/last frames, camera motion, and cinematography plans;
- generating images, video, dialogue, music, and sound effects;
- orchestrating multiple director, creator, reviewer, and revision agents;
- producing timelines, subtitles, edits, composites, and final exports;
- evaluating narrative quality, cross-shot consistency, and production readiness.

> [!NOTE]
> GitHub stars and project status were initially verified on **June 29, 2026**.
> Newer additions and refreshed rows include later per-entry verification dates in notes or `projects.yml`.
> Always refer to each repository's `LICENSE` file and author statements for the authoritative license.
> Open source does not automatically mean commercially usable, and a self-hosted application may still
> depend on commercial model APIs.

## Legend

- 🏆: highly relevant to AI short-drama production with a relatively complete pipeline;
- 📄: associated paper or technical report;
- 🏠: supports local or self-hosted deployment;
- 🧩: agent skill, capability component, or integration layer;
- 🧪: research prototype or early-stage project;
- 💳: core generation features require third-party commercial APIs;
- ⚠️: non-commercial license, incomplete source release, or unspecified license.

## Projects

### End-to-End Short-Drama and Motion-Comic Systems

| Project | Team | What it does | License | Stars | Notes |
|---|---|---|---:|---:|---|
| 🏆🏠 [Toonflow](https://github.com/HBAI-Ltd/Toonflow-app) | HBAI Ltd | Converts novels and scripts into animated short dramas with writing, storyboarding, character, video, three-layer agents, and an infinite-canvas workspace | Apache-2.0 | 10.6k | Desktop/server deployment; model services must be configured separately |
| 🏆⚠️ [Huobao Drama](https://github.com/chatfire-AI/huobao-drama) | Chatfire AI | One-line idea to script, characters, storyboards, voice, video, and episode export | CC BY-NC-SA 4.0 | 13.0k | **Non-commercial license**; Mastra agents and multiple model providers |
| 🏆🏠 [Huobao Drama AI](https://github.com/dav-niu474/huobao-drama-ai) | dav-niu474 | MIT-licensed full-stack AI short-drama studio with script upload/rewrite, character and scene extraction, storyboarding, image/video/TTS generation, and multi-provider model routing | MIT | 77 | Stars checked on August 21, 2026 Beijing time; active Aug 21 feature and security updates; inspired by Huobao Drama but independently implemented and more commercial-friendly |
| 🏆⚠️🏠 [waoowaoo AI Studio](https://github.com/waooAI/waoowaoo) | waooAI | Novel text to storyboarded short drama or comic video with script analysis, character/scene generation, voice, and complete video production | CC BY-NC-SA 4.0 | 13.4k | Source-complete Next.js studio with Docker/local deployment; **non-commercial license**; README describes the project as an early beta under rapid iteration |
| 🏆🏠 [Jellyfish](https://github.com/Forget-C/Jellyfish) | Forget-C / community | Production workspace centered on script breakdown, reusable assets, consistency management, generation jobs, and export | Apache-2.0 | 4.6k | Docker Compose stack with MySQL, Redis, and object storage |
| 🏆🏠 [ArcReel](https://github.com/ArcReel/ArcReel) | ArcReel | Agent-powered novel-to-video workspace covering characters, scenes, props, normalized scripts, storyboard frames, and video | AGPL-3.0 | 3.0k | Built on Claude Agent SDK; review AGPL obligations for network services |
| 🏆 [VideoClaw](https://github.com/HITsz-TMG/VideoClaw) | HITsz-TMG / Lychee Agent | AI video coworker covering concepts, scripts, assets, storyboards, reference images, video generation, editing, and export | MIT | 1.5k | OpenClaw Skill and multi-episode continuation; demos include an eight-episode live-action drama and a five-episode motion comic |
| 🏆⚠️🏠 [DramaClaw](https://github.com/dramaclaw/dramaclaw) | Neo Flying AI Laboratory | Industrial short-drama and motion-comic pipeline covering novel parsing, asset consistency, storyboards, voice, scene locking, canvas exploration, and final export | Elastic-2.0 | 3.0k | Source-available and self-hostable; hosted-service resale is restricted; release `v1.2.1` was published on August 3, 2026 |
| 🏆🏠 [ai-fusion-video](https://github.com/Stonewuu/ai-fusion-video) | Stonewu | Agent-based end-to-end platform for short dramas, motion comics, and videos with episodic script management, storyboard generation, image/video generation, asset management, and Docker deployment | MIT | 1.2k | Java backend + Next.js frontend; self-hostable; release `v1.0.0` was published on August 3, 2026; core generation still depends on third-party model providers |
| 🏆🏠 [AID](https://github.com/gzxx-2025/aid-server) | gzxx-2025 / Photon Info (Hangzhou) Technology | Open-source production platform for AI motion comics, short dramas, AI films, and narrative video with story/episode management, assets, storyboards, image/video generation, dubbing, billing, admin, and online upgrades | MIT | 23 | Primary repo is `aid-server`; `aid-web` and `aid-admin` complete the three-part stack; stars rechecked on August 16, 2026; early community validation, but unusually complete private-deployment and operations capabilities |
| 🏆 [LumenX Studio](https://github.com/alibaba/lumenx) | Alibaba | Novel-to-motion-comic pipeline for asset extraction, style definition, asset generation, storyboard scripts, frames, and video | MIT | 764 | Native integration with Qwen and Wan models |
| ⚠️🏠 [AI Story](https://github.com/xhongc/ai_story) | xhongc | Self-hosted story-video production platform covering script creation, storyboards, image generation, camera planning, image-to-video, and project management | CC BY-NC-SA 4.0 (README) | 987 | Directly relevant and source-complete, but non-commercial; explicit multi-episode continuity mechanisms are less documented |
| 🏆🏠 [LocalMiniDrama](https://github.com/xuanyustudio/LocalMiniDrama) | Xuanyu Studio | Local-first short-drama and comic-drama workflow from story to storyboard and video | MIT | 738 | “Local” describes the workspace and project data; cloud generation may still require APIs |
| 🧪💳 [Open AI Micro Drama Generator](https://github.com/Anil-matcha/Open-AI-Micro-Drama-Generator) | Anil Matcha | Multi-agent pipeline: screenwriter → storyboard → frames → video | MIT (README) | 359 | Lightweight reference implementation; primarily calls video models through muapi.ai |
| 🏆🏠 [Wind Comic](https://github.com/ChrisChen667788/wind-comic) | ChrisChen667788 | One-line idea or novel to finished short-form drama with reusable characters, storyboards, voiceover, timeline, and mp4 export | MIT | 434 | Self-hostable Next.js studio with Docker and BYO-model support; stars rechecked on August 4, 2026; core generation still depends on third-party video/image models |
| 🏆⚠️🏠 [ZJT](https://github.com/jeffstric/ZJT) | jeffstric / ZhiJuTong | Multi-agent short-drama production platform with script writing, storyboard canvas, video synthesis, TTS, browser collaboration, and per-user compute governance | Apache-2.0 with additional terms | 181 | Custom license restricts multi-space hosted services and branding removal; strong fit for education and team scenarios |
| 🧩 [OnlyShot](https://github.com/A-cat-with-carrots/OnlyShot) | Shenxianyu / independent developer | Industrial AI short-drama Claude Skill from one idea to scripts, storyboards, storyboard images, video, and editing package | MIT | 158 | Includes short-drama hooks, pacing, story bibles, Dreamina/Seedance integration, and 17 documented failure modes |
| 🧪🏠 [dramai](https://github.com/hyyyyyyz/dramai) | Independent developer | Zero-backend browser studio: text → storyboard → images → video → CapCut | Apache-2.0 | 19 | Early-stage project and useful pure-browser workflow reference |
| 🧪💳 [AIDrama Studio](https://github.com/EvoLinkAI/ai-short-drama) | EvoLinkAI | Story or novel to script analysis, storyboards, images, video, voiceover, and final output | Previously declared MIT | — | **Repository unavailable on June 28, 2026**; the previous release depended on EvoLink API |

### Workflow References and Adjacent Video Systems

| Project | Team | What it does | License | Stars | Short-drama relevance |
|---|---|---|---:|---:|---|
| ⚠️ [BigBanana AI Director](https://github.com/shuyu-labs/BigBanana-AI-Director) | Shuyu Labs | Script-to-Asset-to-Keyframe workflow with seasons/episodes, asset libraries, nine-grid boards, first/last frames, and rough cuts | CC BY-NC-SA 4.0 | 1.5k | Highly relevant, but non-commercial; the public repo is now a historical reference version, and future updates are released through official Docker images |
| 🏠 [Pixelle-Video](https://github.com/AIDC-AI/Pixelle-Video) | AIDC-AI | Fully automated AI short-video engine for creative planning, asset generation, and composition | Apache-2.0 | 23.7k | General short-video system, but its automation and skill architecture are reusable |
| 🏠 [OpenMontage](https://github.com/calesthio/OpenMontage) | Calesthio AI Labs | Full agent-driven production system for research, scripts, assets, editing, composition, and quality gates | AGPL-3.0 | 25.9k | Not drama-specific; strong reference for provider selection, budget governance, review, and reproducibility |
| 🏠 [Inline Studio](https://github.com/inlineresearch/Inline-Studio) | Inline Research | Desktop AI filmmaking canvas with versioned takes, timeline composition, and hybrid fal/ComfyUI generation | MIT | 160 | Adjacent rather than drama-specific; strong fit for storyboard-driven narrative iteration and shot management |
| 🏠 [VibeFrame](https://github.com/vericontext/vibeframe) | VeriContext | CLI-first, MCP-ready AI video editor driven by storyboard and design files | MIT | 140 | Useful infrastructure for storyboard builds, asset generation, timelines, and render inspection |
| 💳 [PowerTokens Video Studio](https://github.com/PowerTokens/video-studio) | PowerTokens | Video Studio 1.12 (Windows desktop + web) that batch-renders an Excel/CSV shot list with Wan · Seedance · Kling · and more, keeps a shared cast sheet on every prompt, and resumes interrupted jobs by Task ID without resubmitting | MIT | 0 | Runs on the PowerTokens API |

### Editing and Post-Production

| Project | Team | What it does | License | Stars | Notes |
|---|---|---|---:|---:|---|
| 🧩🏠 [FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline) | FireRedTeam | Natural-language video editing agent with planning, media search, voice/BGM/font recommendations, and reusable Style Skills | Apache-2.0 | 3.0k | OpenClaw, Claude Code, and Codex skills; [official demo](https://fireredteam.github.io/demos/firered_openstoryline/) |
| 🏠 [VibeFrame](https://github.com/vericontext/vibeframe) | VeriContext | Generation, editing, captions, voice, music, rendering, and automated inspection | MIT | 140 | Primary entry is listed above |
| 🏠 [OpenMontage](https://github.com/calesthio/OpenMontage) | Calesthio AI Labs | Remotion/HyperFrames/FFmpeg composition, captions, audio mixing, color work, and delivery checks | AGPL-3.0 | 25.9k | Primary entry is listed above |

### Agent Skills and Model Integrations

| Project / Skill | Team | Capability | License / Stars | Caveats |
|---|---|---|---|---|
| 🧩 [libtv-skills](https://github.com/libtv-labs/libtv-skills) | LibTV Labs | OpenClaw-compatible wrappers for the LibLib.tv image and video APIs | MIT / 781 | Capability adapter rather than a complete drama system |
| 🧩 [VideoClaw Skill](https://github.com/HITsz-TMG/VideoClaw) | HITsz-TMG | Starts full video and short-drama production through OpenClaw chat | MIT / 1.5k | Available through ClawHub; still requires API and permission review |
| 🧩 [drama-skills](https://github.com/worldwonderer/drama-skills) | worldwonderer | Skill suite for short-drama project init, writing, assets, storyboard, video prompts, and independent review in Codex and Claude Code | MIT / 375 | Strong production-method layer rather than a standalone generation app |
| 🧩 [shuohao-skills](https://github.com/eternityspring/shuohao-skills) | eternityspring | Skill suite for novel adaptation, character/scene/prop bibles, screenplay writing, and storyboard production packages for AI short-drama workflows in Codex and Claude Code | Apache-2.0 / 1.5k | Strong pre-production and quality-gated workflow with built-in selftests; not a standalone video generation or editing app |
| 🧩 [Drama Generator](https://clawhub.ai/zhenstaff/drama-generator) | ClawHub community | Multi-character scripts, OpenAI TTS, Whisper, and Remotion composition | Unverified | Closer to motion graphics or audio drama than cinematic generation |
| 🧩 [One Click Video Creation](https://clawhub.ai/zuoyuting214/skills/zyt-one-click-video-creation) | ClawHub community | Copy, storyboards, TTS, digital humans, and mixed AI footage | Unverified | Depends on external models and FFmpeg |
| 🧩 [Video Cog](https://clawhub.ai/nitishgargiitd/video-cog) | ClawHub community | Topic to script, voice, music, and edit | Unverified | Hosted-service dependency; review data and billing terms |
| 🧩 [Image Storyboard](https://clawhub.ai/dlazyai/image-storyboard) | ClawHub community | Plan-first, render-later image storyboard skill | Unverified | Third-party API dependency |
| 🧩 [canghe-skills](https://github.com/freestylefly/canghe-skills) | Canghe / community | Skill collection that includes Seedance-based comic-drama generation | Unspecified / 356 | Quality varies; audit each script and dependency separately |

> [!WARNING]
> Agent skills may execute scripts, access the filesystem and network, and read API keys. Review source
> code, pin versions, use least privilege, and run in an isolated environment. “Installable from ClawHub”
> should not be treated as equivalent to “security audited.”

### Multi-Agent Film and Storytelling Research

| Project | Team | Research focus | License | Stars | Paper |
|---|---|---|---:|---:|---|
| 📄 [ViMax](https://github.com/HKUDS/ViMax) | HKU Data Science Lab | Agentic video generation with director, screenwriter, producer, and video generator roles | MIT | 10.7k | See repository |
| 📄 [MovieAgent](https://github.com/showlab/MovieAgent) | Show Lab / NUS | Hierarchical multi-agent CoT planning for scenes, cinematography, and character interactions | Unspecified | 345 | [Paper](https://arxiv.org/abs/2503.07314) · [Project](https://weijiawu.github.io/MovieAgent/) |
| 📄 [MM-StoryAgent](https://github.com/X-PLUG/MM_StoryAgent) | Alibaba X-PLUG, SJTU, ECNU | Multi-agent story videos with text, character-consistent images, narration, music, and effects | Apache-2.0 | 307 | [Paper](https://arxiv.org/abs/2503.05242) |
| 📄 [Anim-Director & AniMaker](https://github.com/HITsz-TMG/Anim-Director) | HITsz-TMG | LMM animation direction and MCTS-driven long-form multi-agent animation | Unspecified | 253 | [Anim-Director](https://arxiv.org/abs/2408.09787) · [AniMaker](https://arxiv.org/abs/2506.10540) |
| 📄 [DramaDirector](https://github.com/iLearn-Lab/DramaDirector) | iLearn-Lab | Geometry-guided short-drama generation with storyboard planning, text-visual reward learning, depth/pose retrieval, and the DramaBoard benchmark | MIT | 1 | [Paper](https://arxiv.org/abs/2606.24107) |
| 📄 [FilmAgent](https://arxiv.org/abs/2501.12909) | HITsz-TMG et al. | Simulated directors, screenwriters, actors, and cinematographers for production in virtual 3D spaces | — | — | The original GitHub URL now redirects to VideoClaw, so repository stars are not counted separately |

## Research Papers and Benchmarks

### Short-Drama-Specific Research

- **[DramaDirector: Geometry-Guided Short Drama Generation](https://arxiv.org/abs/2606.24107)**  
  Hengji Zhou et al., 2026. Uses storyboard planning, text-visual alignment rewards, and depth/pose
  retrieval from real short-drama shots to guide first-frame and image-to-video generation; also
  introduces **DramaBoard**, a benchmark built from 35 live-action dramas, 2.8K episodes, and 81K shots.
- **[SAGE / PROSE: Self-Evolving Storyboard Skills via Attribution-Guided Rule Evolution](https://arxiv.org/abs/2608.17468)**  
  Maolin Ran et al., 2026. Proposes SAGE, which evolves storyboard director skills from professional examples and releases **PROSE**, a paired screenplay–storyboard dataset (68 episodes, 3 productions) under CC BY 4.0 at  
  [https://github.com/creDreams/PROSE](https://github.com/creDreams/PROSE).
- **[One Sentence, One Drama: Personalized Short-Form Drama Generation via Multi-Agent Systems](https://arxiv.org/abs/2605.22144)**  
  Yufei Shi et al., 2026. Uses multi-agent debate to improve short-drama pacing, 3D-grounded
  first-frame generation for spatial consistency, and multi-stage reviewer loops for script,
  visual, and video revisions. It also introduces **Short-Drama-Bench**.

### Agentic Video and Film Storytelling

- **[Co-Director: Agentic Generative Video Storytelling](https://arxiv.org/search/?query=Co-Director%3A+Agentic+Generative+Video+Storytelling&searchtype=title)**  
  Yale Song et al., 2026. Combines hierarchical agents, global multi-armed-bandit search, and
  local multimodal self-refinement; introduces the 400-scenario **GenAD-Bench**.
  [Project page](https://co-director-agent.github.io/)
- **[MovieAgent: Automated Movie Generation via Multi-Agent CoT Planning](https://arxiv.org/abs/2503.07314)**  
  Automatically plans scenes, shots, cinematography, and character interactions from scripts and character banks.
- **[FilmAgent: A Multi-Agent Framework for End-to-End Film Automation in Virtual 3D Spaces](https://arxiv.org/abs/2501.12909)**  
  Studies multi-role agent collaboration and intermediate review in virtual 3D production.
- **[Mind-of-Director: Multi-modal Agent-Driven Film Previsualization via Collaborative Decision-Making](https://arxiv.org/abs/2603.14790)**  
  Film previsualization across script development, virtual scenes, character behavior, and camera planning.
- **[Agentic Video Generation: From Text to Executable Event Graphs via Tool-Constrained LLM Planning](https://arxiv.org/abs/2604.10383)**  
  Uses executable spatiotemporal event graphs and a 3D engine to enforce physical and semantic constraints.

### Animation, Story Video, and Multimodal Research

- **[Anim-Director: A Large Multimodal Model Powered Agent for Controllable Animation Video Generation](https://arxiv.org/abs/2408.09787)**  
  SIGGRAPH Asia 2024; controllable animation direction powered by an LMM.
- **[AniMaker: Multi-Agent Animated Storytelling with MCTS-Driven Clip Generation](https://arxiv.org/abs/2506.10540)**  
  SIGGRAPH Asia 2025; uses MCTS to select and improve long-form animation clips.
- **[MM-StoryAgent: Immersive Narrated Storybook Video Generation with a Multi-Agent Paradigm across Text, Image and Audio](https://arxiv.org/abs/2503.05242)**  
  Multi-stage writing, character-consistent imagery, and multichannel audio with replaceable modality tools.
- **[ViStoryBench: Comprehensive Benchmark Suite for Story Visualization](https://openaccess.thecvf.com/content/CVPR2026/html/Zhuang_ViStoryBench_Comprehensive_Benchmark_Suite_for_Story_Visualization_CVPR_2026_paper.html)**  
  CVPR 2026 benchmark relevant to cross-shot consistency evaluation.

## Observation Zone

The following items are promising and directly relevant, but are **not yet part of the main list**.
Typical reasons include early public release, low maintenance history, or value that is still more
component-level than end-to-end short-drama production.

| Project | Team | Why watch | License / Stars | Current caveats |
|---|---|---|---|---|
| [ShotPlan](https://github.com/Pensioner-11/ShotPlan) | Su Guo et al. / `Pensioner-11` | Multi-shot cinematic video generation with explicit cut control and stronger inter-shot consistency; source, paper, and weights were released on July 20, 2026 | Apache-2.0 / 72 stars | Research prototype rather than a full short-drama pipeline; still no releases and no new code pushes after July 21, 2026 as rechecked on August 4, 2026 Beijing time; depends on Wan 2.1/2.2 weights, and the dataset has research-only terms |
| [Seedance Drama Maker](https://github.com/wanglongxiao/seedance-drama-maker) | wanglongxiao | Full short-drama pipeline with storyboard/shot review flow and character consistency tooling, but currently hard-coupled to BytePlus, SeeDance, SeeDream, Seed-Speech, and TOS APIs; no public release page found | MIT / 10 stars | Rechecked on August 20, 2026 Beijing time; source-complete and feature-rich, but API lock-in and limited release evidence keep it in Observation Zone |
| [AI Showrunner](https://github.com/Yanjin-ai/showrunner) | `Yanjin-ai` | Vertical short-drama agent covering script, story bible, storyboard, per-shot generation, critic-driven regeneration, editing, and multilingual subtitles | Unspecified / 0 stars | Source-complete hackathon prototype and directly relevant to micro-dramas, but it had no declared license or release as checked on July 23, 2026 Beijing time and depends on Qwen Cloud plus third-party video services |
| [my-adrama](https://github.com/hellomrli/my-adrama) | `hellomrli` | Newly public GUI + CLI short-drama workflow covering script, assets, storyboard, video, stage approval, and local packaging; release `v0.5.0` was published on July 26, 2026 | MIT / 0 stars | Directly relevant and source-complete, but it is still an early public release with no community validation as rechecked on August 4, 2026 Beijing time, and it hard-depends on commercial OpenAI/Gemini/Grok APIs |
| [guided-story-video-agent](https://github.com/1667001332/guided-story-video-agent) | `1667001332` | One-line idea to creative cards, 30-60s script, storyboard, and gated video render flow with tests and offline fallback; release `v1.0.1` was published on August 3, 2026 | MIT / 1 star | Promising story-to-video research MVP, but still closer to short-film ideation than a full short-drama production system as rechecked on August 4, 2026 Beijing time; real rendering still depends on external paid providers |

### Official Tutorials, Project Pages, and Articles

- [Toonflow: 12-minute quick start](https://www.bilibili.com/video/BV1oXD7BqEqJ);
- [FireRed-OpenStoryline official demo](https://fireredteam.github.io/demos/firered_openstoryline/);
- [MovieAgent project page](https://weijiawu.github.io/MovieAgent/);
- [AniMaker project page](https://animaker-dev.github.io/);
- [Co-Director project page](https://co-director-agent.github.io/);
- [Wondershare ReelClaw launch coverage](https://stock.10jqka.com.cn/20260320/c675451429.shtml) and
  [testing update](https://www.nbd.com.cn/articles/2026-04-17/4345080.html).

When no credible official blog or public-account article was found, this list uses the repository README,
paper, or official project page as the primary source rather than filling the gap with unattributed reposts.

## Awesome Lists and Discovery Sources

| Resource | Description | Stars / Status |
|---|---|---:|
| [GitHub `ai-short-drama` topic](https://github.com/topics/ai-short-drama) | Most direct dynamic discovery source for open-source short-drama projects | Dynamic |
| [GitHub `ai-storyboard` topic](https://github.com/topics/ai-storyboard) | Storyboards, story bibles, and script-to-video tools | Dynamic |
| [GitHub `openclaw-skills` topic](https://github.com/topics/openclaw-skills) | OpenClaw video, image, audio, and automation skills | Dynamic |
| [ClawHub](https://clawhub.ai/) | Search for `drama`, `storyboard`, and `video creation` skills | Dynamic |
| [awesome-ai-short-drama-tools](https://github.com/clipcurator/awesome-ai-short-drama-tools) | Existing short-drama tools list | 6; small and product-oriented, so use as a lead source |
| [awesome-openclaw](https://github.com/rylena/awesome-openclaw) | General OpenClaw resource list | 29; not drama-specific |
| [awesome-seedance](https://github.com/ZeroLu/awesome-seedance) | Seedance prompts, workflows, and film/drama examples | 2.0k |

The GitHub `ai-short-drama` topic also includes production workflow, budget, greenlight committee,
concept validation, and casting kits published by [clipcurator](https://github.com/clipcurator).
They can be useful production checklists, but have limited community validation and are not ranked
alongside complete generation systems.

## Commercial and Closed-Source Watchlist

The following projects are relevant to the field, but no complete and verifiable open-source repository
was found. They are therefore **excluded from the open-source main list**.

| Project | Team | Positioning | Current assessment |
|---|---|---|---|
| [ShortClaw](https://shortapi.ai/claws/shortclaw/) | ShortAPI | OpenClaw desktop runtime for multiple agents, schedules, and skill management | General runtime rather than a drama tool; no clearly verified public source repository |
| [ShortAPI VideoClaw](https://shortapi.ai/claws/videoclaw/) | ShortAPI | Director, image, video, audio, and VFX agents | **Different from HITsz-TMG VideoClaw**; currently treated as a commercial product |
| ReelClaw | Wondershare | OpenClaw-based idea-to-video agent | Still under testing; [launch coverage](https://stock.10jqka.com.cn/20260320/c675451429.shtml) · [update](https://www.nbd.com.cn/articles/2026-04-17/4345080.html) |
| [CreatorClaw](https://creatorclaw.ai/) | CreatorClaw | End-to-end creator agent | Private beta/commercial product; no complete open-source repository found |
| [AivoClaw](https://www.aivoclaw.cn/) | AivoClaw | Enterprise short-video and digital-human agent | Commercial product |
| [Ima Claw](https://www.imaclaw.bot/) | Ima Claw | Multi-shot, storyboard, and creative-generation skill ecosystem | Adjacent ecosystem rather than a core open-source drama system |
| [PlotParty](https://www.plotparty.ai/) | PlotParty | Character-consistent, plot-coherent, multi-minute narrative video | Commercial platform |
| Zopia | Unverified | Multi-agent video director for drama, film, and branded video | Primarily covered by media reports; no verifiable open-source repository |

## Commonly Confused Names

| Name | Finding |
|---|---|
| **VideoClaw** | At least two distinct entities exist: the HITsz-TMG open-source project and the ShortAPI commercial product. Always include the team name |
| **FilmClaw** | No credible, mature open-source project with this exact name was found as of the verification date; do not confuse it with FilmAgent |
| **MovieClaw** | No credible open-source project with this exact name was found; the related research project is MovieAgent |
| **ShortClaw** | An existing product, but it is a general OpenClaw desktop runtime—not a short-drama system |
| **ReelClaw** | The name is used by both Wondershare's video agent and unrelated UGC/Reels skills; verify the publisher |

## Project Evaluation Checklist

1. **License:** MIT and Apache-2.0 are generally friendlier for reuse; AGPL, CC BY-NC-SA, and unspecified licenses require careful review.
2. **Source completeness:** confirm the repository contains more than a frontend, Docker image, installer, or historical code.
3. **Model dependencies:** distinguish fully local operation, optional cloud APIs, and hard dependencies on a single commercial aggregator.
4. **Production loop:** verify that the project produces shot video, audio, captions, and complete episode exports—not only prompts or still images.
5. **Continuity:** look for explicit mechanisms covering identity, costumes, spatial layout, visual style, and multi-episode context.
6. **Recoverability:** long-running jobs should support persisted state, retries, partial regeneration, and cost controls.
7. **Maintenance:** inspect recent commits, issue responses, releases, and documentation.
8. **Security and privacy:** understand where unreleased scripts, local media, and API keys are sent.

## Contributing

Pull requests and issues are welcome. A suggested project should meet at least one of these criteria:

- provide accessible public source code or a paper;
- solve a meaningful part of the short-drama production pipeline;
- include reproducible setup instructions, a demo, or experimental results;
- add value beyond a base text-to-video model through agents, workflows, consistency, or evaluation.

Please provide:

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

Machine-readable project metadata is available in [`projects.yml`](projects.yml).
