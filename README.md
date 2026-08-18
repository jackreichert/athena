# Athena

**A skill for building rigorous, source-backed study guides that function as the equivalent of a university course — with notes usable by both students and professors. Also builds academic-level place, city, region, and museum guides; scientific-paper deep dives; and legal case deep dives / case method.**

**Current process version:** 1.28 (2026-08-18)

### Skill file (the actual instructions agents load)

**→ [athena/SKILL.md](athena/SKILL.md)**  

Raw URL: `https://raw.githubusercontent.com/jackreichert/athena/main/athena/SKILL.md`  
Repo path: `athena/SKILL.md`

The skill is modular:
- `athena/SKILL.md` — shared research spine (lean)
- `athena/references/mode-*.md` — package-shape deltas (Survey / Standard / Deep)
- `athena/references/place-guides.md` — place / city / museum overlays
- `athena/references/science-paper-guides.md` — scientific paper deep dives
- `athena/references/legal-case-guides.md` — legal case deep dives / case method
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
    ├── legal-case-guides.md
    ├── digest-template.md
    └── directory-layout.md
```

## Recent changes (1.26–1.28)

- **1.28:** Provenance-first. Rich metadata + durable links are required for every consulted syllabus. Full Markdown archival under `source-materials/` is optional and recommended only for high-value or unstable sources.
- **1.27:** Introduced optional `source-materials/` folder for Markdown reformats of syllabi/sources.
- **1.26:** Final packaging cleanup — create `images/` only when images are included; remove empty directories before zipping.
- **1.25:** Themes require **Across the Sources: What Is Easy to Miss**.
- **1.24:** Digests require **After Reading: What Is Easy to Miss**.
- **1.23:** Density improvements against TA-shorthand digests; formalized `author-context.md`.

## Changelog (selected)

- **1.28 (2026-08-18):** Provenance-first refinement of syllabus handling.
- **1.27 (2026-08-18):** Source-materials archival support.
- **1.26 (2026-08-17):** Packaging cleanup for empty directories.
- **1.25 (2026-08-16):** Themes — “Across the Sources: What Is Easy to Miss.”
- **1.24 (2026-08-16):** Digests — “After Reading: What Is Easy to Miss.”
- **1.23 (2026-08-16):** Digest & theme density; author-context consistency.
- **1.22 (2026-08-16):** Legal case deep dives / case method.
- **1.21 (2026-08-16):** Scientific paper deep dives.
- **1.20 (2026-08-16):** Modularized; DEVELOPMENT.md requires Discovery-first before new domains.
- Earlier: Images, Survey shape, full place/location guides, Pre-Reading/Summary/Full Brief digests, Deep mode, anti-bias, provenance.

Full history: [athena/CHANGELOG.md](athena/CHANGELOG.md)  
How to expand the skill: [athena/DEVELOPMENT.md](athena/DEVELOPMENT.md)
