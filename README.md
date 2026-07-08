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
> GitHub stars and project status were verified on **June 29, 2026**. Star counts change over time.
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
| 🏆🏠 [Jellyfish](https://github.com/Forget-C/Jellyfish) | Forget-C / community | Production workspace centered on script breakdown, reusable assets, consistency management, generation jobs, and export | Apache-2.0 | 4.6k | Docker Compose stack with MySQL, Redis, and object storage |
| 🏆🏠 [ArcReel](https://github.com/ArcReel/ArcReel) | ArcReel | Agent-powered novel-to-video workspace covering characters, scenes, props, normalized scripts, storyboard frames, and video | AGPL-3.0 | 3.0k | Built on Claude Agent SDK; review AGPL obligations for network services |
| 🏆 [VideoClaw](https://github.com/HITsz-TMG/VideoClaw) | HITsz-TMG / Lychee Agent | AI video coworker covering concepts, scripts, assets, storyboards, reference images, video generation, editing, and export | MIT | 1.5k | OpenClaw Skill and multi-episode continuation; demos include an eight-episode live-action drama and a five-episode motion comic |
| 🏆 [LumenX Studio](https://github.com/alibaba/lumenx) | Alibaba | Novel-to-motion-comic pipeline for asset extraction, style definition, asset generation, storyboard scripts, frames, and video | MIT | 764 | Native integration with Qwen and Wan models |
| ⚠️🏠 [AI Story](https://github.com/xhongc/ai_story) | xhongc | Self-hosted story-video production platform covering script creation, storyboards, image generation, camera planning, image-to-video, and project management | CC BY-NC-SA 4.0 (README) | 987 | Directly relevant and source-complete, but non-commercial; explicit multi-episode continuity mechanisms are less documented |
| 🏆🏠 [LocalMiniDrama](https://github.com/xuanyustudio/LocalMiniDrama) | Xuanyu Studio | Local-first short-drama and comic-drama workflow from story to storyboard and video | MIT | 738 | “Local” describes the workspace and project data; cloud generation may still require APIs |
| 🧪💳 [Open AI Micro Drama Generator](https://github.com/Anil-matcha/Open-AI-Micro-Drama-Generator) | Anil Matcha | Multi-agent pipeline: screenwriter → storyboard → frames → video | MIT (README) | 359 | Lightweight reference implementation; primarily calls video models through muapi.ai |
| 🧩 [OnlyShot](https://github.com/A-cat-with-carrots/OnlyShot) | Shenxianyu / independent developer | Industrial AI short-drama Claude Skill from one idea to scripts, storyboards, storyboard images, video, and editing package | MIT | 158 | Includes short-drama hooks, pacing, story bibles, Dreamina/Seedance integration, and 17 documented failure modes |
| 🧪🏠 [dramai](https://github.com/hyyyyyyz/dramai) | Independent developer | Zero-backend browser studio: text → storyboard → images → video → CapCut | Apache-2.0 | 19 | Early-stage project and useful pure-browser workflow reference |
| 🧪💳 [AIDrama Studio](https://github.com/EvoLinkAI/ai-short-drama) | EvoLinkAI | Story or novel to script analysis, storyboards, images, video, voiceover, and final output | Previously declared MIT | — | **Repository unavailable on June 28, 2026**; the previous release depended on EvoLink API |

### Workflow References and Adjacent Video Systems

| Project | Team | What it does | License | Stars | Short-drama relevance |
|---|---|---|---:|---:|---|
| ⚠️ [BigBanana AI Director](https://github.com/shuyu-labs/BigBanana-AI-Director) | Shuyu Labs | Script-to-Asset-to-Keyframe workflow with seasons/episodes, asset libraries, nine-grid boards, first/last frames, and rough cuts | CC BY-NC-SA 4.0 | 1.5k | Highly relevant, but non-commercial; the public repo is now a historical reference version, and future updates are released through official Docker images |
| 🏠 [Pixelle-Video](https://github.com/AIDC-AI/Pixelle-Video) | AIDC-AI | Fully automated AI short-video engine for creative planning, asset generation, and composition | Apache-2.0 | 23.7k | General short-video system, but its automation and skill architecture are reusable |
| 🏠 [OpenMontage](https://github.com/calesthio/OpenMontage) | Calesthio AI Labs | Full agent-driven production system for research, scripts, assets, editing, composition, and quality gates | AGPL-3.0 | 25.9k | Not drama-specific; strong reference for provider selection, budget governance, review, and reproducibility |
| 🏠 [VibeFrame](https://github.com/vericontext/vibeframe) | VeriContext | CLI-first, MCP-ready AI video editor driven by storyboard and design files | MIT | 140 | Useful infrastructure for storyboard builds, asset generation, timelines, and render inspection |

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
