# Athena

**A skill for building rigorous, source-backed study guides that function as the equivalent of a university course — with notes usable by both students and professors. Also builds academic-level place, city, region, and museum guides.**

**Current process version:** 1.19 (2026-08-16)

### Skill file (the actual instructions agents load)

**→ [athena/SKILL.md](athena/SKILL.md)**  

Raw URL (after push): `https://raw.githubusercontent.com/jackreichert/athena/main/athena/SKILL.md`  
Repo path: `athena/SKILL.md`

---

## Who this is for

You want the equivalent of a university course on a topic — Plato’s dialogues, Shakespeare, a historical episode, a contested idea — **or** a serious academic-level guide to a place you are visiting or studying: a city, region, historic landscape, or museum. Not a chatty summary, not a tourist brochure, and not a SparkNotes-style reduction that tells you what to think.

You want materials that help you **not miss important things**: clear learning outcomes, a ranked and provenance-tracked reading list drawn from real syllabi (or the highest-quality scholarly sources when syllabi are thin), digests that give pre-reading orientation, a full post-reading brief, and a compact summary for reference, thematic units that drive discussion, and further-reading pathways. For places: historical layers, why sites matter in the scholarly conversation, what not to miss and *why*, images for key works/sites, and transparent sources. The notes work for students *and* for professors.

## Package shapes

| Shape | What you get | Digests |
|-------|--------------|---------|
| **Survey** | Scope + ranked sources (full provenance) + themes + further reading | Deferred |
| **Standard** | Full undergrad-course equivalent | Required + `02-digests.md` index |
| **Deep** | Full graduate/seminar equivalent | Required + denser apparatus + `02-digests.md` |

All three share the same research spine (syllabi mining, provenance, ranked sources, themes with citations, further reading).

## What you get

Every Athena run produces a **portable Markdown package** (Obsidian-optimized by default). Typical contents:

- **Scope** — topic, package shape, learning outcomes, digests in/out of scope  
- **Sources** — ranked list with **Syllabi & Discovery Sources Consulted**, provenance notes, full working bibliography, notable further-reading candidates  
- **Digests** (Full packages) for primary texts: Pre-Reading Context + Summary + Full Brief (Post-Reading); for artworks: dual-layer + images  
- **`02-digests.md`** — index + recommended reading order (Full packages)  
- **Themes** — synthesis by concept or debate  
- **Further reading**, glossary, limitations, learning path  
- **Images** (when relevant) under `images/`

**Optional:** EPUB when requested.

**For place / city / region / museum guides** (academic depth, Blue Guide / university-city-history spirit):

- Historical orientation (layered chronology or key periods)  
- Must-see sites with scholarly rationale (not popularity rankings)  
- Practical itineraries grounded in historical and spatial logic  
- Images for key artworks and sites  
- Full provenance and bibliography (starts with syllabi when available; otherwise strongest monographs, architectural histories, institutional catalogues)  
- Museum specializations retained (dual-layer artwork digests, Period-Specialist Analysis, artist bios, official collection links)

## How to try it

```
Athena on [topic]
Athena survey of [topic]
Athena go deep on [topic]
Athena museum guide for [museum or collection]
Athena place guide for [city or region]
Athena city guide for [city]
Athena travel guide for [destination]
```

## Install

Point your agent at this repo or at the skill file. See any accompanying INSTALL.md if present.

## Changelog (selected)

- **1.19 (2026-08-16):** Images for visual primary sources; default Markdown (Obsidian) + optional EPUB.
- **1.18 (2026-08-16):** Survey package shape + `02-digests.md`; softened completeness gate.
- **1.17 (2026-08-15):** Full place / location / travel guides at academic depth.
- Earlier: Pre-Reading / Summary / Full Brief digests, Deep mode, anti-bias rules, provenance tracking, museum dual-layer digests.

See full changelog inside `athena/SKILL.md`.
