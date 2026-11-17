# Mallss 3D Motion — Project Guide

This repository contains project-level Claude Code skills in `.claude/skills/`.

## Skill selection

Do not load every skill for every request. Identify the task, select only the matching skill or small combination, then read its complete `SKILL.md` and any linked references before implementation.

| Task | Start with |
|---|---|
| Vertical short-form video | `short-form-video` |
| Word-timed / karaoke captions | `caption-animation` |
| Countdown or timer graphics | `countdown-video` |
| Names, roles, speaker labels | `lower-thirds` |
| Podcast / voiceover waveform | `audiogram` |
| YouTube branded intro / outro | `youtube-intro-outro` |
| AI presenter / talking-head workflow | `talking-head` |
| Graphics over presenter footage | `talking-head-b-roll` |
| Animated chat / message story | `text-message-animation` |
| Editorial geographic sequence | `map-animation` |

## Working rules

1. Establish the deliverable first: platform, aspect ratio, resolution, frame rate, duration, audio source, visual direction, and output format.
2. Inspect the repository and available runtime before selecting dependencies or rewriting existing files.
3. Prefer the skill's documented workflow and preserve its references, templates, and helper scripts.
4. Avoid generic template output. Build around the actual brief, supplied assets, narrative beats, and visual hierarchy.
5. Verify the result: render representative frames, inspect a contact sheet, check timing and safe areas, and probe the encoded video where the workflow supports it.
6. Do not claim a render is correct until its output has been inspected. Report unavailable dependencies or credentials clearly.
7. Never write API keys, tokens, or private credentials into plans, source files, logs, or commits.

## 3D Animation reference pack

The SkillDB 3D Animation collection is catalogued in `docs/SKILLDB-3D-ANIMATION.md`. Its full skill text is hosted by SkillDB and is not bundled in this repository. Do not invent its contents; use the source link or an authorised SkillDB installation when access is available.
