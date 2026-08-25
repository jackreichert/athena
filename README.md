# Athena

A skill that builds rigorous, source-backed study guides that function as university-course equivalents — with notes usable by both students and professors.

It also produces academic-level place, city, region, and museum guides; scientific-paper deep dives; and legal case deep dives / case method.

**Process version:** 1.32 (2026-08-25)

---

## What it produces

Athena does not generate chatty summaries or reductive paraphrases. It produces structured, portable packages of Markdown files designed so the reader can engage primary sources without missing important things.

Typical deliverables include:

- Clear learning outcomes and scope
- **Primary university department / program** (decided after research from sources, syllabi, and themes)
- Ranked, provenance-tracked sources (syllabi and discovery signals are logged)
- Structured digests of primary sources (pre-reading orientation + standalone summary + full post-reading brief)
- Thematic synthesis with citations and “what is easy to miss” sections
- Further-reading pathways
- Glossary and limitations

Three package shapes share the same research spine:

| Shape        | Focus                                      | Digests                  |
|--------------|--------------------------------------------|--------------------------|
| **Survey**   | Map the field (sources + themes)           | Deferred                 |
| **Standard** | Undergraduate-course equivalent            | Required                 |
| **Deep**     | Graduate / seminar equivalent              | Required + denser apparatus |

The final output is a **self-contained directory of Markdown files** (Obsidian-friendly, relative links) that is zipped for delivery.

### Output package layout

```
athena-<topic-slug>/
├── README.md                 # Includes primary university department
├── 00-scope.md               # Includes primary university department (+ secondary if interdisciplinary)
├── 01-sources.md             # Ranked bibliography + full provenance
├── 02-digests.md             # Index + reading order (Full packages only)
├── 03-themes.md
├── further-reading.md
├── glossary.md
├── limitations.md
├── digests/                  # One complete digest per Core & Important source
├── themes/                   # One file per theme
├── source-materials/         # Optional archival Markdown of key syllabi
└── images/                   # Only when images are included
```

Survey packages omit `digests/` and `02-digests.md`. Full packages (Standard / Deep) require complete digests for every Core and Important source and complete theme files for every listed theme. A mandatory integrity audit runs before the package is considered finished.

---

## Process & philosophy

Athena treats study-guide construction as a disciplined research process rather than free-form summarization.

It achieves this by enforcing a fixed sequence of phases (scope → source discovery with syllabus provenance → consistent digests → thematic synthesis → departmental home decision → integrity audit) and by refusing to advance until completeness and citation standards are met.

**Core stance**
- Primary sources come first. Digests orient and help the reader notice structure, moves, and open questions; they do not replace the primary encounter or hand the reader “the meaning.”
- Completeness over ambition. In full packages every Core *and* Important source receives a complete digest before themes are written. Missing content fails a hard integrity audit.
- Provenance is required. Every syllabus or discovery source consulted is logged with institution, course, year, durable link, and what was extracted from it.
- Themes are synthetic, not sequential. They organize by concept or debate and back every major claim to a digest or source. Each theme includes a concrete “Across the Sources: What Is Easy to Miss” checklist.
- Anti-reductive by design. The skill explicitly refuses to dumb down, moralize, or collapse contested material into a single approved interpretation.
- **Departmental home is decided after research.** Once sources and themes are established, Athena identifies the primary university department or program that would most naturally house a course of this kind and records it in `00-scope.md` and `README.md`.

**High-level workflow**
1. **Scope** — Define topic, audience, package shape (Survey / Standard / Deep), and learning outcomes.
2. **Sources** — Mine syllabi and high-quality discovery signals; rank Core / Important / Supplementary with full provenance.
3. **Digests** (Full packages) — Produce consistent three-part digests for every Core and Important source.
4. **Themes** — Synthesize across sources with citations, gaps, and open questions.
5. **Departmental home** — After research is complete, decide the primary university department (and any secondary affiliations) that would house the course; record in scope and README.
6. **Assembly & audit** — Build the navigable package, then actively verify that every index entry points to real, complete content. Only then is a zip offered.

The same spine supports ordinary study guides, place/museum guides, scientific-paper deep dives, and legal case-method packages. Adaptive reference files supply the domain-specific overlays.

---

## How to use it

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

---

## For agents (installation)

The skill file agents should load is:

**`athena/SKILL.md`**

Raw URL:  
`https://raw.githubusercontent.com/jackreichert/athena/main/athena/SKILL.md`

Repo path: `athena/SKILL.md`

The skill is modular. After deciding package shape in Phase 0, load the matching mode file and any applicable adaptive overlay:

```
athena/
├── SKILL.md                          # Shared research spine
├── CHANGELOG.md
├── DEVELOPMENT.md
└── references/
    ├── mode-survey.md
    ├── mode-standard.md
    ├── mode-deep.md
    ├── place-guides.md               # Place / city / museum
    ├── science-paper-guides.md       # Scientific paper deep dives
    ├── legal-case-guides.md          # Legal case / case method
    ├── digest-template.md
    └── directory-layout.md
```

---

## Further reading

- Full process history: [CHANGELOG.md](athena/CHANGELOG.md)
- Expanding the skill: [DEVELOPMENT.md](athena/DEVELOPMENT.md)
