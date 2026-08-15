# Athena

**A skill for building rigorous, source-backed study guides that function as the equivalent of a university course — with notes usable by both students and professors. Also builds academic-level place, city, region, and museum guides.**

**Current process version:** 1.17 (2026-08-15)

### Skill file (the actual instructions agents load)

**→ [athena/SKILL.md](https://raw.githubusercontent.com/jackreichert/athena/main/athena/SKILL.md)**  

Raw URL: `https://raw.githubusercontent.com/jackreichert/athena/main/athena/SKILL.md`  
Repo path: `athena/SKILL.md`

---

## Who this is for

You want the equivalent of a university course on a topic — Plato’s dialogues, Shakespeare, a historical episode, a contested idea — **or** a serious academic-level guide to a place you are visiting or studying: a city, region, historic landscape, or museum. Not a chatty summary, not a tourist brochure, and not a SparkNotes-style reduction that tells you what to think.

You want materials that help you **not miss important things**: clear learning outcomes, a ranked and provenance-tracked reading list drawn from real syllabi (or the highest-quality scholarly sources when syllabi are thin), digests that give pre-reading orientation, a full post-reading brief, and a compact summary for reference, thematic units that drive discussion, and further-reading pathways. For places: historical layers, why sites matter in the scholarly conversation, what not to miss and *why*, and transparent sources. The notes work for students *and* for professors.

## What you get

Every Athena run produces a **portable Markdown package**. Typical contents:

- **Scope** — topic, mode (Standard or Deep), learning outcomes  
- **Sources** — ranked list with **Syllabi & Discovery Sources Consulted**, provenance notes, full working bibliography, notable further-reading candidates  
- **Digests** for primary texts: Pre-Reading Context + Summary + Full Brief (Post-Reading)  
- **Themes** — synthesis by concept or debate  
- **Further reading**, glossary, limitations, learning path  

**For place / city / region / museum guides** (academic depth, Blue Guide / university-city-history spirit):

- Historical orientation (layered chronology or key periods)  
- Must-see sites with scholarly rationale (not popularity rankings)  
- Practical itineraries grounded in historical and spatial logic  
- Full provenance and bibliography (starts with syllabi when available; otherwise strongest monographs, architectural histories, institutional catalogues)  
- Museum specializations retained (dual-layer artwork digests, Period-Specialist Analysis, artist bios, official collection links)

## Standard vs Deep

| | **Standard** | **Deep** |
|---|---|---|
| **Feel** | Upper-level undergrad course equivalent | Graduate course / seminar notes |
| **Place guides** | Solid academic orientation + must-sees + itinerary | Denser historiography, debates about the place, specialist literature |

Trigger Deep with `Athena go deep`, `Athena deeper`, or `graduate study guide on…`.  
Trigger place guides with `Athena place guide for [city/region]`, `Athena city guide for…`, `Athena travel guide for…`, or `Athena museum guide for…`.

## Design commitments

1. University-course equivalent with dual-use notes (student + professor).  
2. Help you not miss things — Pre-Reading Context, Full Brief, Summary are distinct.  
3. Anti-reductive — digests do not dumb down or dictate interpretation.  
4. Primary sources first; provenance non-negotiable; full bibliography.  
5. Completeness over ambition.  
6. Consensus contestable.  
7. Place guides start from syllabi or highest-quality scholarly sources and stay at academic depth.

## How to try it

```
Athena on [topic]
Athena go deep on [topic]
Athena museum guide for [museum or collection]
Athena place guide for [city or region]
Athena city guide for [city]
Athena travel guide for [destination]
```

## Install

See **[INSTALL.md](INSTALL.md)**. Short version: point your agent at this repo or at the skill file URL above.

## Changelog

See the Changelog section inside `athena/SKILL.md`. Recent highlights:

- **1.17 (2026-08-15):** Expanded to full place / location / travel guides at academic depth (cities, regions, historic landscapes). Starts with syllabi when available; otherwise highest-quality scholarly sources. Historical orientation + must-see sites with scholarly rationale + itineraries. Museum specializations retained.
- **1.16:** Primary-source digests: Pre-Reading Context + Summary + Full Brief (Post-Reading). Anti-SparkNotes stance.
- **1.15:** University-course framing with notes for both students and professors.
- **1.14.x:** Provenance tracking, full working bibliography, notable further-reading sources.
