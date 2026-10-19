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
| 🏆🏠 [Story Claw](https://github.com/ZC89757/story-claw) | ZC89757 | Novel-to-episode pipeline with stage-aware assets, persistent voices, storyboards, audio, VLM clip checks, self-hosted ComfyUI/LTX rendering, and optional MG animation templates | MIT | 28 | Checked October 13, 2026 Beijing time; Windows desktop and CLI; MG pack installs separately; GPU/ComfyUI and LLM/image/TTS APIs required; failed clips may be accepted after the retry limit |
| 🏆🏠 [Toonflow](https://github.com/HBAI-Ltd/Toonflow-app) | HBAI Ltd | Converts novels and scripts into animated short dramas with writing, storyboarding, character, video, three-layer agents, and an infinite-canvas workspace | Apache-2.0 | 10.6k | Desktop/server deployment; model services must be configured separately |
| 🏆⚠️ [Huobao Drama](https://github.com/chatfire-AI/huobao-drama) | Chatfire AI | One-line idea to script, characters, storyboards, voice, video, and episode export | CC BY-NC-SA 4.0 | 13.0k | **Non-commercial license**; Mastra agents and multiple model providers |
| 🏆🏠 [Huobao Drama AI](https://github.com/dav-niu474/huobao-drama-ai) | dav-niu474 | MIT-licensed full-stack AI short-drama studio with script upload/rewrite, character and scene extraction, storyboarding, image/video/TTS generation, and multi-provider model routing | MIT | 77 | Stars checked on August 21, 2026 Beijing time; active Aug 21 feature and security updates; inspired by Huobao Drama but independently implemented and more commercial-friendly |
| 🏆⚠️🏠 [waoowaoo AI Studio](https://github.com/waooAI/waoowaoo) | waooAI | Novel text to storyboarded short drama or comic video with script analysis, character/scene generation, voice, and complete video production | CC BY-NC-SA 4.0 | 13.4k | Source-complete Next.js studio with Docker/local deployment; **non-commercial license**; README describes the project as an early beta under rapid iteration |
| 🏆🏠 [Jellyfish](https://github.com/Forget-C/Jellyfish) | Forget-C / community | Production workspace centered on script breakdown, reusable assets, consistency management, generation jobs, and export | Apache-2.0 | 4.6k | Docker Compose stack with MySQL, Redis, and object storage |
| 🏆🏠 [ArcReel](https://github.com/ArcReel/ArcReel) | ArcReel | Agent-powered novel-to-video workspace covering characters, scenes, props, normalized scripts, storyboard frames, and video | AGPL-3.0 | 3.0k | Built on Claude Agent SDK; review AGPL obligations for network services |
| 🏆 [VideoClaw](https://github.com/HITsz-TMG/VideoClaw) | HITsz-TMG / Lychee Agent | AI video coworker covering concepts, scripts, assets, storyboards, reference images, video generation, editing, and export | MIT | 1.5k | OpenClaw Skill and multi-episode continuation; demos include an eight-episode live-action drama and a five-episode motion comic |
| 🏆⚠️🏠 [DramaClaw](https://github.com/dramaclaw/dramaclaw) | Neo Flying AI Laboratory | Short-drama and motion-comic pipeline with asset consistency, storyboards, voice, canvas exploration, export, video extension, and model-backed quality/frame-rate enhancement | Elastic-2.0 | 6,862 | Checked October 13, 2026 Beijing time; latest release v2.0.6 (September 28); source-available and self-hostable; hosted-service offering restricted; retain required Powered by DramaClaw branding and notices |
| 🏆🏠 [ai-fusion-video](https://github.com/Stonewuu/ai-fusion-video) | Stonewu | Agent-based short-drama/motion-comic platform with episodic scripts, storyboards, image/video generation, ComfyUI workflows, optional music/sound effects, and media task management | MIT | 1,613 | Checked October 13, 2026 Beijing time; v1.2.0 released October 11 with media persistence and storyboard refresh fixes; amd64/arm64 Docker images; model APIs or self-hosted ComfyUI required |
| 🏆🏠 [AID Studio](https://github.com/gzxx-2025/aid-studio) | gzxx-2025 / Photon Info (Hangzhou) Technology | Unified source repository for short-drama, motion-comic, and AI-film production, including scripts, assets, storyboards, image/video generation, dubbing, billing, admin, and upgrades | MIT | 880 | Checked October 13, 2026 Beijing time; migrated from aid-server; server, creator/admin fronts and deployment tooling now share one repo; latest release v2.2.4; model services, storage and backend infrastructure configured separately |
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
| 🧩🏠 [ReShot](https://github.com/maosika-ai/reshot) | Maosika | Converts reference video into depth, pose, or edge control clips to reuse blocking and camera movement with different characters | Apache-2.0 | 51 | Checked October 13, 2026 Beijing time; v0.5.0; local CLI/Web UI, Colab and ComfyUI; outputs control media, not finished films; downstream video models and model-weight licenses must be considered separately |
| 🏠 [Inline Studio](https://github.com/inlineresearch/Inline-Studio) | Inline Research | Desktop AI filmmaking canvas with versioned takes, timeline composition, and hybrid fal/ComfyUI generation | MIT | 160 | Adjacent rather than drama-specific; strong fit for storyboard-driven narrative iteration and shot management |
| 🏠 [VibeFrame](https://github.com/vericontext/vibeframe) | VeriContext | CLI-first, MCP-ready AI video editor driven by storyboard and design files | MIT | 140 | Useful infrastructure for storyboard builds, asset generation, timelines, and render inspection |
| 🧩🏠 [PenShot / Story Shot Agent](https://github.com/neopen/story-shot-agent) | neopen | Script, novel, film, animation, or short drama to coherent shot lists and video-model prompts, with cross-segment character, scene, and plot continuity | MIT | 228 | Checked October 20, 2026 Beijing time; v0.3.11; Docker, PyPI, MCP, REST, Function Calling, and A2A; a pre-production/storyboard agent rather than a video renderer |

### Editing and Post-Production

| Project | Team | What it does | License | Stars | Notes |
|---|---|---|---:|---:|---|
| 🧩🏠 [FireRed-OpenStoryline](https://github.com/FireRedTeam/FireRed-OpenStoryline) | FireRedTeam | Natural-language video editing agent with planning, media search, voice/BGM/font recommendations, and reusable Style Skills | Apache-2.0 | 3.0k | OpenClaw, Claude Code, and Codex skills; [official demo](https://fireredteam.github.io/demos/firered_openstoryline/) |
| 🏠 [VibeFrame](https://github.com/vericontext/vibeframe) | VeriContext | Generation, editing, captions, voice, music, rendering, and automated inspection | MIT | 140 | Primary entry is listed above |
| 🏠 [OpenMontage](https://github.com/calesthio/OpenMontage) | Calesthio AI Labs | Remotion/HyperFrames/FFmpeg composition, captions, audio mixing, color work, and delivery checks | AGPL-3.0 | 25.9k | Primary entry is listed above |

### Agent Skills and Model Integrations

| Project / Skill | Team | Capability | License / Stars | Caveats |
|---|---|---|---|---|
| 🧩 [Short-Drama Director Suite / Manju Laoli](https://github.com/lixiaoxiao9888-create/manju-laoli-skill) | lixiaoxiao9888-create | Short-drama director skill with four-view assets, spatial blocking, dialogue, segment continuity, Seedance/H3 prompt adapters, prompt lint, and an offline storyboard board | MIT / 1,158 | Checked October 13, 2026 Beijing time; latest release remains v6.9.8 (September 20); recent commits mainly update sponsorship documentation; beta integrating modified open-source content; external generation tools required |
| 🧩 [Dramake](https://github.com/xixihhhh/ai-short-drama-skill) | xixihhhh | Director/production skill with series memory, continuity and voice ledgers, budgets, recoverable jobs, acceptance gates, editing plans, and validation scripts | MIT / 50 | Checked October 13, 2026 Beijing time; latest push August 29; generation tools must be connected separately; examples are production plans rather than verified finished films |
| 🧩 [Open Film Skills](https://github.com/62656456/ai-film-skills) | 62656456 | 21 filmmaking skills for writing, directing, assets, storyboards, cinematography, optional 3D previs, production handoff, and playback review | Apache-2.0 / 66 | Checked October 13, 2026 Beijing time; v1.4.0 synchronizes source and standalone downloads; 18 regular + 3 opt-in experimental packages; external generation tools required; packaging/tests do not establish finished-film quality |
| 🧩💳 [StarReel MCP](https://github.com/starreel/starreel-mcp) | StarReel | Open MCP client exposing a commercial script-to-final-cut service with assets, storyboards, video, and TTS tools | MIT / 0 | Checked October 13, 2026 Beijing time; October 12 source sync labels v0.1.138; only the thin client is open source; generation, consistency checks, auditing, and billing run on the prepaid proprietary server |
| 🧩 [libtv-skills](https://github.com/libtv-labs/libtv-skills) | LibTV Labs | OpenClaw-compatible wrappers for the LibLib.tv image and video APIs | MIT / 781 | Capability adapter rather than a complete drama system |
| 🧩 [VideoClaw Skill](https://github.com/HITsz-TMG/VideoClaw) | HITsz-TMG | Starts full video and short-drama production through OpenClaw chat | MIT / 1.5k | Available through ClawHub; still requires API and permission review |
| 🧩 [Drama Skills](https://github.com/zenstory-ai/drama-skills) | ZenStory AI | Eleven short-drama/motion-comic skills for novel adaptation, episodic scripts, consistency locks, storyboards, prompts, production, editing, and review | MIT / ~2.8k | Checked October 13, 2026 Beijing time (rounded GitHub display); migrated from worldwonderer/drama-skills; v0.8.1 adds still/video mixed editing and character reference-audio binding; external generation tools and FFmpeg required |
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

- **[DramaChain Bench: An End-to-End Benchmark for Short-Drama Generation](https://arxiv.org/abs/2609.00646)**
  Haoyuan Shi, Mingtao Chen et al., Tencent Hunyuan and collaborators, 2026. Evaluates script,
  storyboard, keyframe, shot video and assembled episodes with 63 dimensions and localized defect
  attribution. Revised October 3 (v2); a research benchmark, not a verified open-source production engine.

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

- **[MVAgent: Multi-Agent Video Generation via Consistent Condition Construction and Shot-Level Policy Optimization](https://arxiv.org/abs/2609.30609)**
  Xiangyu Kong et al., 2026. Combines spatial grounding, end-of-shot continuity memory and transition
  references with shot-level Trunk-GDPO optimization for multi-shot consistency; submitted September 24.
  Paper inclusion does not imply a verified source/weight release.
- **[VideoGen-Agent: Reinforcing Video Generation Agents](https://arxiv.org/abs/2609.24997)**
  Binxu Li et al., 2026. Trains multimodal tool use across augmentation, generation and verification;
  introduces the 600-prompt VABench. Revised October 5 (v3).
  [Official project](https://andyca111.github.io/VideoGen_Agent/) still labels code and benchmark data
  as coming soon as checked October 13, 2026 Beijing time.

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
| [MangaStudio](https://github.com/bo961386926/manga-studio) | bo961386926 | Script-to-asset-to-keyframe workbench with costume variants, first/last frames, shot splitting, and Web/Electron/Docker deployment | MIT / 25 | Checked October 13, 2026 Beijing time; latest main commit remains August 18 despite newer push metadata; defaults to GitCC API; episodic memory, complete audio, and automated editing evidence remains limited |
| [Qingshan Short Drama Engine](https://github.com/rogerwu188/qingshan-short-drama-production-line) | rogerwu188 | Python/CLI pipeline for scripts, continuity, generation, FFmpeg editing, QA, durable jobs, and release receipts | MIT / 2 | Checked October 13, 2026 Beijing time; October 12 adds source acquisition and original-story fallback; latest release candidate explicitly UNVALIDATED; provider/publishing adapters need real-environment verification |
| [Dralo Studio](https://github.com/lnblfkj-del/Dralo-Studio) | lnblfkj-del | Local short-drama workspace with episodic scripts, reusable assets, infinite canvas, 3D previs, generation, and multitrack editing | Apache-2.0 / 7 | Checked October 13, 2026 Beijing time; v0.1.0-preview.2; standalone source excludes cloud operations; cross-platform and paid generation not fully validated |
| [Juliu Studio](https://github.com/JerrIsTheBesta/AI-Short-Drama-Studio) | JerrIsTheBesta | Electron/Vue workspace with scripts, assets, storyboards, ComfyUI/model adapters, voice, subtitles, and editing | MIT / 17 | Checked October 13, 2026 Beijing time; v0.1.7 and Windows installer available; multi-episode continuity and reproducible finished-film evidence remain limited |
| [AI Short Drama Workbench](https://github.com/CZ3744/ai-short-drama-workbench) | CZ3744 | Local-first short-drama/motion-comic workbench for scripts, storyboards, assets, and FFmpeg composition | MIT / 1 | Checked October 13, 2026 Beijing time; created October 8; BYO APIs; early source release with little independent validation |
| [Huohuo Drama](https://github.com/appolloqin/huohuo-drama) | appolloqin | Novel-to-script/storyboard/assets/TTS/episode export with claimed layered narrative memory | Unspecified / 11 | Checked October 13, 2026 Beijing time; no declared license; source access does not grant reuse or commercial permission; memory claims need independent validation |
| [AI Canvas Tauri](https://github.com/Tenney95/AI-Canvas-tauri) | Tenney95 | Local visual canvas with episode workspaces, shared assets, ComfyUI, agents, MCP, and Blender | Custom source-available / 219 | Checked October 13, 2026 Beijing time; current license restricts commercial redistribution/SaaS and requires separate authorization; planned MIT conversion at 10k stars is not the current license |
| [ShotPlan](https://github.com/Pensioner-11/ShotPlan) | Su Guo et al. / `Pensioner-11` | Multi-shot cinematic video generation with explicit cut control and stronger inter-shot consistency; source, paper, and weights were released on July 20, 2026 | Apache-2.0 / 72 stars | Research prototype rather than a full short-drama pipeline; still no releases and no new code pushes after July 21, 2026 as rechecked on August 4, 2026 Beijing time; depends on Wan 2.1/2.2 weights, and the dataset has research-only terms |
| [Seedance Drama Maker](https://github.com/wanglongxiao/seedance-drama-maker) | wanglongxiao | Full short-drama pipeline with storyboard/shot review flow and character consistency tooling, but currently hard-coupled to BytePlus, SeeDance, SeeDream, Seed-Speech, and TOS APIs; no public release page found | MIT / 10 stars | Rechecked on August 20, 2026 Beijing time; source-complete and feature-rich, but API lock-in and limited release evidence keep it in Observation Zone |
| [AI Showrunner](https://github.com/Yanjin-ai/showrunner) | `Yanjin-ai` | Vertical short-drama agent covering script, story bible, storyboard, per-shot generation, critic-driven regeneration, editing, and multilingual subtitles | Unspecified / 0 stars | Source-complete hackathon prototype and directly relevant to micro-dramas, but it had no declared license or release as checked on July 23, 2026 Beijing time and depends on Qwen Cloud plus third-party video services |
| [my-adrama](https://github.com/hellomrli/my-adrama) | `hellomrli` | Newly public GUI + CLI short-drama workflow covering script, assets, storyboard, video, stage approval, and local packaging; release `v0.5.0` was published on July 26, 2026 | MIT / 0 stars | Directly relevant and source-complete, but it is still an early public release with no community validation as rechecked on August 4, 2026 Beijing time, and it hard-depends on commercial OpenAI/Gemini/Grok APIs |
| [guided-story-video-agent](https://github.com/1667001332/guided-story-video-agent) | `1667001332` | One-line idea to creative cards, 30-60s script, storyboard, and gated video render flow with tests and offline fallback; release `v1.0.1` was published on August 3, 2026 | MIT / 1 star | Promising story-to-video research MVP, but still closer to short-film ideation than a full short-drama production system as rechecked on August 4, 2026 Beijing time; real rendering still depends on external paid providers |
| [Plein](https://github.com/hoobnn/plein) | hoobnn | Local-first AI infinite canvas for developing ideas into scripts, storyboards, shots, voice, and multitrack edits | AGPL-3.0 / 2 | Checked October 20, 2026 Beijing time; v0.2.3; source-complete with preview, partial redo, recovery, and project packages, but very new with little independent finished-film evidence |
| [Daoyan CLI](https://github.com/yuanbaobaoo/daoyan-cli) | yuanbaobaoo | ComfyUI-oriented production CLI with shot retry, validation, resumable jobs, and assembly | Apache-2.0 / 0 | Checked October 20, 2026 Beijing time; v0.0.7; remote/GPU generation integrations remain incomplete, so it is not yet an end-to-end deployment option |
| [AI Short Drama](https://github.com/ceoifung/ai-short-drama) | ceoifung | Materials or novel to writing/review/storyboard/reference-image/production package, QA, and FFmpeg edit workflow | MIT / 0 | Checked October 20, 2026 Beijing time; no release and only a short public history; actual video generation still requires manual UpDream work |
| [SoloDrama](https://github.com/Hejunlong27/SoloDrama) | Hejunlong27 | Local CLI batch-production toolkit from development to finished short dramas and cost ledger | Apache-2.0 / 2 | Checked October 20, 2026 Beijing time; supports resumable runs, delivery-material gates, local ComfyUI assets, and RunningHub rendering, but is newly public and tightly coupled to RunningHub |
| [ShotForward](https://github.com/shotforward/shotforward) | ShotForward | Local-first desktop filmmaking workspace with scripts, versioned assets, storyboards, undoable agent changes, video providers, and FFmpeg export | Apache-2.0 / 1 | Checked October 20, 2026 Beijing time; v0.2.63; broad filmmaking scope rather than short drama only, macOS ARM is the primary installer, and some providers are paid |
| [AI Short Play Video Creation](https://github.com/ADC1920/AI-short-play-video-creation) | ADC1920 | Agent skill with storyboard/grid planning, continuity, clip-junction checks, dubbing, troubleshooting scripts, and a minimal multi-episode example | MIT / 0 | Checked October 20, 2026 Beijing time; source includes self-check scripts but has no release or community validation; final rendering depends on Jimeng/Seedance |
| [Video Factory](https://github.com/LordVayron/video-factory) | LordVayron | Coding-agent-operated studio for micro-drama series, with cast lock, storyboards, audio-first timing, hard budget gates, continuity QA, and FFmpeg delivery | MIT / 0 | Checked October 20, 2026 Beijing time; v1.0.0; also targets ads and ambient video, with core rendering and voices tied to Kie.ai and ElevenLabs |

### Official Tutorials, Project Pages, and Articles

- [ZenStory: novel-to-short-drama adaptation](https://zenstory.ai/zh/drama-skills/novel-to-short-drama);
- [ZenStory: character consistency](https://zenstory.ai/zh/drama-skills/character-consistency);
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
