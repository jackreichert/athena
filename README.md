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

**Example:**  
“Athena teach me cognitive behavioral therapy” → pulls syllabi, ranks primary & secondary sources, digests them, cross-references themes, builds bibliography + citations, and outputs a folder ready for Obsidian.  
Works the same way for museum collections and visitor guides.

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
- Museum or cultural-site guides (“top things to see at the Prado”, etc.)

---

## Install & Try

### Quick install phrases
> Install the Athena skill from https://github.com/jackreichert/athena

> Load the Athena study-guide skill from this repo

### Try without permanently installing
Some platforms support remote / one-shot loading directly from GitHub so you can evaluate the approach before committing it to your system prompt or skill library.

**AdaL / Adalagent example** (thanks to [@panda_liyin](https://x.com/panda_liyin)):
```
skills:gh:jackreichert/athena
```
(or with a leading `@` depending on the client). This reads the skill straight from the repo — nothing is saved and nothing is permanently added to the system prompt.

Other agents may offer similar `skills:gh:owner/repo` or “load skill from URL” patterns. Prefer those when you want to experiment first.

### Platform notes
- **Grok / xAI** — Point the agent at the repo or the `athena/` folder.
- **Claude** — Drop `athena/` into the Skills location (or use skill-creator / Projects). The YAML `name` + `description` enable progressive loading.
- **ChatGPT Custom GPT** — Paste the body of `SKILL.md` into Instructions; upload `references/` as Knowledge. Adapt file paths to available tools.
- See **INSTALL.md** for more detail.

---

## Package Structure

```
athena-<topic-slug>/
├── README.md
├── 00-scope.md
├── 01-sources.md          # ranked bibliography + citation practice
├── further-reading.md     # concrete research pathways (required)
├── glossary.md
├── limitations.md
├── artists-bios.md        # optional, for multi-creator / museum topics
├── digests/
└── themes/                # each ends with Gaps & Open Questions + Theme Bibliography
```

---

## Key Features

- **Citations & further research as first-class requirements**
- Museum / cultural-site adaptations (artworks as primary sources, timed itineraries, artist bios)
- Adaptive review types (Narrative, Thematic, Scoping, Systematic-leaning, Hybrid)
- Portable Agent Skills format (works across Grok, Claude, and adaptable to others)

---

## Repository Contents

```
athena/
├── SKILL.md
├── changelog.md
└── references/
    ├── digest-template.md
    └── directory-layout.md
README.md
INSTALL.md
```

---

## Design Philosophy

Prefer primary sources. Make the evidence base visible. Surface disagreements. Give readers a clear path to go further. Keep the package navigable and portable.

---

## License

MIT

## Author

[Jack Reichert](https://github.com/jackreichert)
