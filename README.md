# Athena

**A skill for building rigorous, source-backed study guides that function as the equivalent of a university course — with notes usable by both students and professors. Also builds academic-level place, city, region, and museum guides; scientific-paper deep dives; and legal case deep dives / case method.**

**Current process version:** 1.22 (2026-08-16)

### Skill file (the actual instructions agents load)

**→ [athena/SKILL.md](athena/SKILL.md)**  

Raw URL: `https://raw.githubusercontent.com/jackreichert/athena/main/athena/SKILL.md`  
Repo path: `athena/SKILL.md`

The skill is modular:
- `athena/SKILL.md` — shared research spine (lean)
- `athena/references/mode-*.md` — package-shape deltas (Survey / Standard / Deep)
- `athena/references/place-guides.md` — place / city / museum overlays
- `athena/references/science-paper-guides.md` — scientific paper deep dives
- `athena/references/legal-case-guides.md` — legal case deep dives / case method (new in 1.22)
- `athena/references/digest-template.md` + `directory-layout.md`

---

## Who this is for

You want the equivalent of a university course on a topic — Plato’s dialogues, Shakespeare, a historical episode, a contested idea — **or** a serious academic-level guide to a place, **or** a rigorous deep dive into primary scientific papers, **or** a rigorous deep dive into judicial opinions and the case method. Not a chatty summary and not a reductive paraphrase that tells you what to think.

You want materials that help you **not miss important things**: clear learning outcomes, ranked and provenance-tracked sources, digests with pre-reading orientation + full post-reading brief + standalone summary, thematic units that drive discussion, and further-reading pathways. For legal cases: precise issue formulation, rule extraction, fact materiality, application, holding vs. dicta, and generative hypotheticals. The notes work for students *and* for professors.

## Package shapes

| Shape | What you get | Digests |
|-------|--------------|---------|
| **Survey** | Scope + ranked sources (full provenance) + themes + further reading | Deferred |
| **Standard** | Full undergrad-course equivalent | Required + `02-digests.md` index |
| **Deep** | Full graduate/seminar equivalent | Required + denser apparatus + `02-digests.md` |

## How to try it

```
Athena on [topic]
Athena survey of [topic]
Athena go deep on [topic]
Athena museum / place / city guide for [location]
Athena deep dive on [scientific paper]
Athena journal club on [paper]
Athena case brief / case method on [judicial opinion]
Athena legal case deep dive on [case or doctrine]
```

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
    ├── science-paper-guides.md
    ├── legal-case-guides.md      ← new in 1.22
    ├── digest-template.md
    └── directory-layout.md
```

## Changelog (selected)

- **1.22 (2026-08-16):** Second Discovery-first adaptive application — legal case deep dives / case method.
- **1.21 (2026-08-16):** First Discovery-first adaptive application — scientific paper deep dives.
- **1.20 (2026-08-16):** Modularized. Modes and place guides extracted; DEVELOPMENT.md requires Discovery-first before new domains.
- Earlier: Images, Survey shape, full place/location guides, Pre-Reading/Summary/Full Brief digests, Deep mode, anti-bias, provenance.

Full history: [athena/CHANGELOG.md](athena/CHANGELOG.md)  
How to expand the skill: [athena/DEVELOPMENT.md](athena/DEVELOPMENT.md)
