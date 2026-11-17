# Mallss 3D Motion

<p align="center">
  <strong>A practical skill library for AI-assisted 3D animation, motion graphics, and video production.</strong>
  <br />
  Curated for Claude Code with reusable workflows, production references, and render-verification helpers.
</p>

<p align="center">
  <img alt="Claude Code" src="https://img.shields.io/badge/Claude_Code-project_skills-6B5CFF" />
  <img alt="Motion Design" src="https://img.shields.io/badge/Motion-Graphics-111827" />
  <img alt="3D Animation" src="https://img.shields.io/badge/3D-Animation-0F766E" />
</p>

## What this is

Mallss 3D Motion brings together focused agent skills for creating short-form videos, YouTube graphics, talking-head visuals, b-roll overlays, animated captions, text-message scenes, and editorial map sequences.

The included iart-ai skills are stored in Claude Code's project skill directory, so the agent can discover them from this repository without manually downloading each pack during a task.

## Included skills

| Collection | Skills | Focus |
|---|---:|---|
| TikTok / Reels / Shorts | 4 | Short-form pacing, word-timed captions, countdowns, lower thirds |
| YouTube | 2 | Audiograms and branded intro / outro sequences |
| Talking Head | 1 | Presenter video workflow and rendering pipeline |
| B-roll | 1 | Word-timed graphics over talking-head footage |
| Text Message Video | 1 | Animated chat conversations and message-story videos |
| Map Animation | 1 | Editorial map sequences and geographic motion |

**10 ready-to-use skills** are included in `.claude/skills/`, along with their available references, templates, scripts, and package metadata.

### 3D animation catalogue

The repository also tracks the 21-skill [SkillDB 3D Animation pack](https://skilldb.dev/skills/3d-animation-skills). Its skill bodies are not mirrored here: SkillDB marks full-pack access as Pro, and this repository does not claim a redistribution licence for that material.

See **[docs/SKILLDB-3D-ANIMATION.md](docs/SKILLDB-3D-ANIMATION.md)** for the complete index and source links. Bring the full pack into your own project through SkillDB if your account has access.

## Use with Claude Code

Open this repository as the project in Claude Code. Project skills live under `.claude/skills/` and are available by their skill names.

You can ask naturally:

- "Turn this narration into a polished 9:16 short with readable word-timed captions."
- "Create a branded YouTube intro and outro using this logo and audio sting."
- "Add explanatory b-roll over this talking-head recording without cutting the speaker's original audio."
- "Build an editorial map sequence that follows these locations."
- "Create a believable 3D character walk cycle and review the animation curves."

Claude should load only the skills relevant to the task. Each skill's `SKILL.md` points to its supporting references and tools where applicable.

## Repository layout

```text
.claude/
  skills/
    audiogram/
    talking-head/
    talking-head-b-roll/
    caption-animation/
    countdown-video/
    lower-thirds/
    short-form-video/
    text-message-animation/
    map-animation/
    youtube-intro-outro/
scripts/                 # Shared frame-sheet and MP4 verification helpers
docs/
  SKILLDB-3D-ANIMATION.md
licenses/
  iart-ai-MIT-LICENSE.txt
CLAUDE.md
README.md
THIRD_PARTY_NOTICES.md
```

## Production notes

- Read the selected skill's full `SKILL.md` and linked references before building.
- Check the actual project environment and available tools before choosing a rendering pipeline.
- Keep text, timing, safe areas, and audio synchronization deliberate; do not rely on placeholder visuals.
- Render representative frames and inspect them before exporting the final video.
- Use the shared scripts and the skill-specific verification steps to inspect encoded output.
- Some workflows require external tools or services such as Node.js, FFmpeg, Playwright, Remotion, Whisper, or provider API credentials. Requirements are documented inside each skill. Never commit secrets or API keys.

## Sources and licensing

The included video and motion skills are mirrored from the upstream iart-ai repositories listed in [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md). Their upstream MIT licence is preserved in [licenses/iart-ai-MIT-LICENSE.txt](licenses/iart-ai-MIT-LICENSE.txt).

SkillDB content is linked, not republished. Check each upstream source's terms and licence before redistributing any additional material.

---

<p align="center">
  <sub>Curated by <a href="https://github.com/ItsMeMal">ItsMeMal</a> · Built for practical creative workflows, not one-click generic output.</sub>
</p>
