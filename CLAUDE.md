# The Melanin Guardians — Project Context for Claude Code

## Project Overview

**The Melanin Guardians** is a multimedia IP developed by **Quantum Melanin Media**. The project spans:

- Graphic novel series (Volumes 1 & 2, in production)
- AI-generated cinematic video content
- Expanded universe world-building assets

Core themes draw from **African diaspora heritage**, warrior traditions, ancestral knowledge systems, and the ongoing fight against cultural erasure (epistemicide). The IP is designed to center Black excellence, spiritual resilience, and intergenerational strength as the primary narrative engine.

---

## Creative Universe

### Core Themes

- African diaspora identity and warrior heritage
- Epistemicide — the systematic destruction of cultural knowledge — as the central antagonistic force
- Ancestral memory as power source
- Community, strategy, and spiritual grounding as heroic virtues
- Warm vs. cold color symbolism (life/culture vs. void/erasure)

### Named Characters

| Character | Role | Color Identity |
|---|---|---|
| Zara | Lead Guardian | Warm gold |
| Marcus | Strategist | Earth tones |
| Jamal | Warrior | Deep amber |
| Dr. Imani Osei | Scholar | Indigo |
| Amara | Spiritual Anchor | Rose gold |
| Darius | Field Commander | Burnt sienna |
| Epistemicide Agents | Antagonists | Cold void-green |
| Shadow Leader | Primary Villain | Obsidian |

### Visual Rule

> **Heroes = warm gold / amber palette. Enemies = cold void-green palette.**

This rule is non-negotiable across all generated assets. Never mix hero warmth with enemy coldness on the same character. Backgrounds may blend, but character color identity must hold.

---

## Production Stack

| Tool | Role | Priority |
|---|---|---|
| Kling 3.0 | Primary video generation | 1st |
| Runway Gen 4.5 | Cinematic sequences | 2nd |
| Dreamina / Seedance (via CapCut) | Secondary generation | 3rd |

Platform selection per shot depends on motion complexity, character fidelity requirements, and current API availability.

---

## Prompt Engineering Standards

### Energy Dissolution FX Language

When writing destruction, transition, or power FX prompts use this vocabulary:

- "dissolves into cascading light fragments"
- "energy unravels into void-green particles"
- "ancestral fire consumes the frame"
- "the figure fractures into dispersing embers"
- "warm amber pulse overwhelms cold static"

### Platform Tags

Always prefix prompts with the target platform tag:

```
[KLING] — Kling 3.0 prompt
[RUNWAY] — Runway Gen 4.5 prompt
[DREAMINA] — Dreamina/Seedance via CapCut prompt
```

### Hero / Enemy Block Separation

Write hero and enemy prompts in separate labeled blocks. Never describe both in the same prompt block — keep generation contexts clean.

```
// HERO BLOCK
[KLING] Zara advances, warm gold light radiating from her silhouette...

// ENEMY BLOCK
[KLING] Epistemicide Agents emerge from void-green static, cold and fragmented...
```

---

## Post-Production

- **Primary editor:** CapCut
- **Structure per volume:** 49 clips / 19 scenes
- **Audio anchor:** 90 BPM (all music, SFX, and cut timing references this tempo)
- Scene transitions should respect the 90 BPM grid — cuts on beat or half-beat

---

## File Management

```
/prompts/       — Raw and refined generation prompts, organized by scene
/scenes/        — Scene-level breakdowns, shot lists, narrative beats
/characters/    — Character reference sheets, color guides, design notes
/assets/video/  — Generated video clips, organized by vol and scene number
/assets/panels/ — Graphic novel panel art, layered files, exports
/exports/       — Final rendered sequences, deliverables, release cuts
```

---

## Coding Conventions

### Markdown Files

Name files using platform and scene references:

```
vol1_scene03_kling_zara-entry.md
vol2_scene11_runway_shadowleader-reveal.md
```

### Commit Messages

- Imperative mood, under 72 characters
- Include scene and volume reference where applicable

```
Add Vol1 Scene 04 Kling prompts for Jamal battle sequence
Update Zara character color guide for amber consistency
Fix energy FX language in Vol2 Scene 07 enemy block
```

### Branch Prefixes

| Prefix | Use |
|---|---|
| `vol1/` | Volume 1 content |
| `vol2/` | Volume 2 content |
| `video/` | Video generation work |
| `prompts/` | Prompt writing and refinement |

---

## Session Priorities for Claude Code

When starting a session, default priority order:

1. Prompt writing / refinement for scheduled generation runs
2. Scene structure and shot list development
3. Character consistency checks across assets
4. File organization and naming cleanup
5. Documentation and world-building notes

---

## Key Commands

```bash
# List all prompt files
ls prompts/

# Check scene structure for a volume
ls scenes/

# Review character references
ls characters/

# Find all Kling-tagged prompts
grep -r "\[KLING\]" prompts/

# Find all Runway-tagged prompts
grep -r "\[RUNWAY\]" prompts/
```

---

## Team

| Person | Role |
|---|---|
| Rob | Creative Director, Quantum Melanin Media |
| Mahal | Creative Partner |
| Claude Code | AI production assistant |

---

## Notes for Claude Code

This is **active production**, not a prototype or experiment. Assets generated here are intended for publication and distribution.

**Cultural significance:** The Melanin Guardians carries specific cultural weight as an Afrocentric IP. Treat character integrity, color symbolism, and thematic consistency with the same rigor you would apply to any production-grade system. Do not flatten, genericize, or neutralize the cultural specificity of this project.

**When in doubt on creative decisions:** ask Rob or Mahal before generating or committing. Consistency across volumes matters more than speed.

**Prompt quality over quantity.** A well-crafted prompt that generates one usable clip beats five rushed prompts that produce unusable output.
