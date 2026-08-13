# Athena

**A skill for building rigorous, source-backed, thematically organized study guides.**

Athena produces self-contained Markdown packages that help you (or an AI agent) go deep on any topic — philosophy, history, literature, art, museums, science, or technical subjects — while keeping the evidence base transparent and the path for further research clear.

**Current process version:** 1.5 (2026-08-13)

---

## What Athena Does

Athena turns a topic into a structured learning package with:

- Clear scope and learning outcomes
- Ranked, justified sources (primary preferred)
- Consistent digests of core works
- Thematic synthesis with provenance (every major claim is back-linkable)
- Practical navigation (reading order, timed itineraries for museums, etc.)
- Short creator/artist bios when relevant
- **Citations, transparent sourcing, and concrete further-reading pathways as a core value**

The result is not a summary. It is a portable research and learning scaffold you can use in Obsidian, VS Code, plain text, or any Markdown environment.

---

## Core Values

1. **Objectives first** — define learning outcomes before collecting sources.
2. **Primary > Secondary** — prioritize original works; use secondary sources for orientation and debate mapping.
3. **Provenance** — every substantive claim should be traceable to a digest or primary source.
4. **Citations & further research are fundamental** — packages must make the evidence base visible and give readers concrete next steps. This is non-negotiable.
5. **Adaptive rigor** — match depth, search protocol, matrices, bios, and itineraries to the nature of the topic.
6. **Transparency** — document selection criteria, surface gaps, note limitations.

---

## When to Use Athena

Trigger on requests such as:

- “Athena…” / “Athena research…”
- “Build a study guide on…”
- “Create a deep reading list and synthesis for…”
- “Make a thematic study guide of…”
- “Produce a self-study package with primary sources and digests”
- Museum or cultural-site guides (“top things to see at the Prado”, “guide to the Met’s European wing”, etc.)

It works especially well for:

- Philosophy and history of ideas
- Literature and primary-text engagement
- Art history and museum collections
- Any subject where primary sources + thematic synthesis + transparent sourcing matter

---

## Package Structure

A typical Athena package looks like this:

```
athena-<topic-slug>/
├── README.md                 # Overview, learning path, quick-start
├── 00-scope.md               # Topic, audience, outcomes, review type
├── 01-sources.md             # Ranked bibliography + citation practice
├── 03-themes.md              # Theme index
├── further-reading.md        # Concrete research pathways (required & substantive)
├── glossary.md
├── limitations.md            # Gaps + methodological notes
├── artists-bios.md           # (optional) short parallel bios for multi-creator topics
├── digests/                  # One structured digest per core source
│   └── ...
└── themes/                   # Individual theme files
    └── ...                   # Each ends with Gaps & Open Questions + Theme Bibliography
```

See `athena/references/directory-layout.md` for the full recommended layout.

---

## Key Features (v1.5)

### Citations, Sources & Further Research
- Explicit selection criteria and citation-practice notes in `01-sources.md`
- Full bibliographic-style entries on every digest
- Theme Bibliographies on every theme file
- Substantive `further-reading.md` with named entry points and “how to go deeper” guidance
- Methodological notes in `limitations.md`

### Museum & Cultural-Site Support
- Artworks treated as primary sources (location-aware digests)
- Official museum highlights and timed itineraries prioritized
- Practical walkthrough / itinerary themes
- Short artist/creator bios
- Support for iterative expansion when the user focuses on particular artists or rooms

### Adaptive Review Types
- Narrative / Conceptual
- Thematic
- Scoping
- Systematic-leaning
- Hybrid (most common, especially for museums)

### Portability
Designed for the open Agent Skills format. Softened environment-specific paths so the same skill works well in Grok, Claude Skills, and (with light adaptation) Custom GPTs / other agents.

---

## Install

### Grok / xAI or Agent Skills–compatible runtimes
Point the agent at this repository or the `athena/` folder and ask it to install/load the skill, e.g.:

> Install the Athena skill from https://github.com/jackreichert/athena

or place the `athena/` directory where your agent expects skills.

### Claude
Drop the `athena/` folder into your Claude Skills directory (or use the skill-creator / project skills flow). The `SKILL.md` frontmatter (`name` + `description`) enables progressive loading.

### ChatGPT Custom GPT
1. Paste the body of `athena/SKILL.md` (or a condensed version) into the GPT Instructions.
2. Upload `athena/references/` (and optionally example packages) as Knowledge files.
3. Adapt any remaining file-path language to the tools available in that environment.

See `INSTALL.md` for more detail.

---

## Repository Contents

```
athena/
├── SKILL.md                  # Full process specification (v1.5)
├── changelog.md
└── references/
    ├── digest-template.md
    └── directory-layout.md
README.md
INSTALL.md
```

---

## Design Philosophy

Athena is deliberately opinionated about intellectual hygiene:

- Prefer primary sources.
- Make the evidence base visible.
- Surface disagreements instead of forcing false consensus.
- Give readers a clear path to go further.
- Keep the package navigable and portable.

It is intended for serious self-study, teaching preparation, research orientation, and high-quality visitor guides to collections and sites.

---

## License

MIT (or add your preferred license).

---

## Author

Maintained by [Jack Reichert](https://github.com/jackreichert).

Feedback and improvements welcome via issues or pull requests.
