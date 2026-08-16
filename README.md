# Athena

**A skill for building rigorous, source-backed study guides that function as the equivalent of a university course — with notes usable by both students and professors. Also builds academic-level place, city, region, and museum guides, and scientific-paper deep dives.**

**Current process version:** 1.21 (2026-08-16)

### Skill file (the actual instructions agents load)

**→ [athena/SKILL.md](athena/SKILL.md)**  

Raw URL: `https://raw.githubusercontent.com/jackreichert/athena/main/athena/SKILL.md`  
Repo path: `athena/SKILL.md`

The skill is modular:
- `athena/SKILL.md` — shared research spine (lean)
- `athena/references/mode-*.md` — package-shape deltas (Survey / Standard / Deep)
- `athena/references/place-guides.md` — place / city / museum overlays
- `athena/references/science-paper-guides.md` — scientific paper deep dives (new in 1.21)
- `athena/references/digest-template.md` + `directory-layout.md`

---

## Who this is for

You want the equivalent of a university course on a topic — Plato’s dialogues, Shakespeare, a historical episode, a contested idea — **or** a serious academic-level guide to a place you are visiting or studying, **or** a rigorous deep dive into primary scientific papers (reading, critique, and positioning). Not a chatty summary, not a tourist brochure, and not a SparkNotes-style reduction that tells you what to think.

You want materials that help you **not miss important things**: clear learning outcomes, a ranked and provenance-tracked reading list drawn from real syllabi (or the highest-quality scholarly sources when syllabi are thin), digests that give pre-reading orientation, a full post-reading brief, and a compact summary for reference, thematic units that drive discussion, and further-reading pathways. For places: historical layers, why sites matter, images for key works/sites. For scientific papers: independent figure interpretation, results vs interpretation, limitations, alternative explanations, and generative next-experiment thinking. The notes work for students *and* for professors.

## Package shapes

| Shape | What you get | Digests |
|-------|--------------|---------|
| **Survey** | Scope + ranked sources (full provenance) + themes + further reading | Deferred |
| **Standard** | Full undergrad-course equivalent | Required + `02-digests.md` index |
| **Deep** | Full graduate/seminar equivalent | Required + denser apparatus + `02-digests.md` |

All three share the same research spine. Mode-specific behavior lives in the reference files so the main skill stays lean.

## What you get

Every Athena run produces a **portable Markdown package** (Obsidian-optimized by default). Typical contents:

- **Scope** — topic, package shape, learning outcomes, digests in/out of scope  
- **Sources** — ranked list with **Syllabi & Discovery Sources Consulted**, provenance notes, full working bibliography  
- **Digests** (Full packages) for primary texts and, when relevant, scientific papers or artworks  
- **`02-digests.md`** — index + recommended reading order (Full packages)  
- **Themes** — synthesis by concept or debate  
- **Further reading**, glossary, limitations, learning path  
- **Images** (when relevant) under `images/`

**Optional:** EPUB when requested.

## How to try it

```
Athena on [topic]
Athena survey of [topic]
Athena go deep on [topic]
Athena museum guide for [museum or collection]
Athena place guide for [city or region]
Athena deep dive on [scientific paper or set of papers]
Athena journal club on [paper]
```

## Install

Point your agent at this repo or at the skill directory (`athena/`). The skill is self-contained under `athena/`.

## Structure

```
athena/
├── SKILL.md
├── CHANGELOG.md
├── DEVELOPMENT.md
└── references/
    ├── mode-survey.md
    ├── mode-standard.md
    ├── mode-deep.md
    ├── place-guides.md
    ├── science-paper-guides.md   ← new in 1.21
    ├── digest-template.md
    └── directory-layout.md
```

## Changelog (selected)

- **1.21 (2026-08-16):** First Discovery-first adaptive application — scientific paper deep dives.
- **1.20 (2026-08-16):** Modularized. Modes and place guides extracted; DEVELOPMENT.md requires Discovery-first before new domains.
- **1.19–1.17:** Images, Survey shape, full place/location guides.
- Earlier: Pre-Reading / Summary / Full Brief digests, Deep mode, anti-bias, provenance, museum dual-layer digests.

Full history: [athena/CHANGELOG.md](athena/CHANGELOG.md)  
How to expand the skill: [athena/DEVELOPMENT.md](athena/DEVELOPMENT.md)
