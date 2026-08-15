# Athena

**A skill for building rigorous, source-backed study guides — from solid undergraduate overviews to graduate-seminar-equivalent notes.**

**Current process version:** 1.14.1 (2026-08-15)

### Skill file (the actual instructions agents load)

**→ [athena/SKILL.md](https://raw.githubusercontent.com/jackreichert/athena/main/athena/SKILL.md)**  

Raw URL: `https://raw.githubusercontent.com/jackreichert/athena/main/athena/SKILL.md`  
Repo path: `athena/SKILL.md`

---

## Who this is for

You want to go deep on a topic — a book, a painter, a historical episode, a contested idea, a museum — and you don’t want a chatty summary that evaporates the moment you close the tab.

You want something closer to **course notes**: clear learning outcomes, a ranked reading list, structured digests of the core sources, themes that show where claims come from, and a path for what to do next. You care that citations are real, that “consensus” is treated as a claim rather than the floor, and that you can see *where the sources themselves came from* (especially which syllabi and institutional lists signaled them).

If that sounds like you, Athena is built for it. If you only need a quick overview or a bullet list of “key facts,” a normal conversation is enough — you don’t need this skill.

## What you get

Every Athena run produces a **portable Markdown package**, not a single blob of prose. Typical contents:

- **Scope** — topic, mode (Standard or Deep), learning outcomes, constraints  
- **Sources** — ranked Core / Important / Supplementary list with selection criteria, **Syllabi & Discovery Sources Consulted**, provenance notes on entries, citation practice, a compiled full working bibliography, and notable further-reading candidates  
- **Digests** — one structured file per Core source (and selected Important ones)  
- **Themes** — synthesis organized by concept or debate, with back-links to digests  
- **Further reading** — concrete next steps, including notable additional primary or secondary sources discovered during research that are useful for going deeper  
- **Glossary, limitations, learning path** — so the package stays usable weeks later  

For museums and collections, digests treat artworks as primary sources: formal description, zone/panel mapping when relevant, and a **Period-Specialist Analysis** that surfaces symbolism, historical context, visual details, and period color meanings a general visitor is likely to miss.

## Standard vs Deep

| | **Standard** | **Deep** |
|---|---|---|
| **Feel** | Excellent upper-level undergrad overview | Graduate seminar / comps-style notes |
| **Sources** | Focused Core list | Richer Core + Important; more secondary literature |
| **Digests** | Clear, consistent | Denser; methodological and reception sections |
| **Themes** | Solid synthesis + citations | Debates, intellectual genealogy, Seminar Guiding Questions |
| **Bibliography** | Useful annotated list with provenance | Substantially richer, positioned annotations + fuller discovery log |

Same process either way. Deep is higher intensity, not a different method. Trigger Deep with phrases like `Athena go deep`, `Athena deeper`, or `graduate study guide on…`.

## Design commitments (why it exists)

1. **Primary sources first** — digests orient you to the real material; they don’t replace it.  
2. **Provenance is non-negotiable** — major claims in themes back-link to digests or primary sources; the ranked bibliography itself records which syllabi and institutional signals produced it.  
3. **Completeness over ambition** — every Core source gets a full digest before themes are written. Thin digests on an oversized Core list are a process failure.  
4. **Consensus is contestable** — especially on recent or politicized topics. Primary and contemporaneous evidence preferred for disputed facts; recantations and competing claims are surfaced; Wikipedia is a source to check, not an authority.  
5. **Active use** — learning paths, questions, itineraries. Deep mode adds seminar-style prompts.  
6. **Transparent discovery** — sources are not just listed; the package shows the expert signals (syllabi, catalogues, citation patterns) that justified their inclusion and ranking.

## What it is not

- Not a replacement for reading the primary works.  
- Not a guarantee of perfect scholarship — it is a structured research process that makes evidence, gaps, *and source provenance* visible.  
- Not a general chatbot mode. It is a skill with phases, templates, and quality gates.

## How to try it

After the skill is installed (see `INSTALL.md`):

```
Athena on [topic]
Athena go deep on [topic]
Athena museum guide for [museum or collection]
```

Examples that work well: a single major book, a painter and their key works, a historical debate, a museum visit, a contested contemporary claim where primary evidence matters.

## Install

See **[INSTALL.md](INSTALL.md)**. Short version: point your agent at this repo or at the skill file URL above. Other models often fail to find the skill file unless the link is explicit — that is why it is at the top of this README.

## Changelog

See the Changelog section inside `athena/SKILL.md` for full version history. Recent highlights:

- **1.14.1 (2026-08-15):** Explicitly capture and surface notable additional primary or secondary sources useful for further reading (even outside Core/Important); these are flagged in Phase 1 and required in `further-reading.md`.
- **1.14 (2026-08-15):** Source provenance tracking — every syllabus and institutional list consulted is logged; ranked entries carry provenance notes; full working bibliography is compiled during research and required in `01-sources.md`.
- **1.13–1.12:** Dual-layer artwork digests (unit/zone + Period-Specialist Analysis).
- **1.11:** Hard completeness gate (no Phase 3 until every Core source has a full digest).
- **1.9:** Explicit anti-bias practices for contested/politicized domains.
- **1.6:** Standard vs Deep modes.
