# Recommended Directory Layout

```
athena-<kebab-topic>/   (or study-guide-<kebab-topic>/)
├── README.md                 # Master overview, package shape (Survey/Standard/Deep), review type, learning path, quick-start
├── 00-scope.md               # Topic statement, audience, package shape, learning outcomes, review type, digests in/out of scope, output format
├── 01-sources.md             # Ranked bibliography with provenance notes, selection criteria, Syllabi & Discovery Sources Consulted section, citation practice, availability, full working bibliography
│                             # (Deep: richer annotations + optional Primary/Secondary/Methodological categorization)
├── 01b-search-protocol.md    # Optional/conditional: questions, search strategy, inclusion/exclusion
├── 02-digests.md             # Index + recommended reading order for digests (only when digests are produced)
├── 03-themes.md              # Theme index
├── matrix.md                 # Optional/recommended: synthesis matrix (themes × sources); more detailed in Deep
├── further-reading.md        # REQUIRED & substantive: concrete pathways, named sources, how to go deeper
│                             # (Deep: multi-track research pathways, specialization tracks, journals/databases)
├── glossary.md               # Key terms with source origins
├── limitations.md            # Gaps, access issues, methodological/sourcing notes, package shape, version
├── author-context.md         # Recommended for single-author literary/philosophical packages: lean intellectual biography + relevant reception and positioning of Core works (source-backed)
├── artists-bios.md           # Recommended for multi-creator / museum topics: short parallel bios
├── digests/                  # Only present in Full packages (Standard or Deep)
│   ├── author-year-short-title.md
│   └── ...                   # Primary texts: Pre-Reading Context + Summary + Full Brief (Post-Reading). Deep: + Methodological / Reception / Subsequent Engagements
│                             # Artworks: dual-layer (Unit/Zone + Period-Specialist Analysis) + images
├── themes/
│   ├── 01-theme-name.md      # Includes Gaps & Open Questions + Theme Bibliography
│   │                         # (Deep: Seminar Guiding Questions; Debates & Contending Interpretations / genealogy; longer annotated Theme Bib 8–15 items with positioning)
│   ├── 02-theme-name.md
│   └── ...
└── images/                   # Reference images for artworks, sites, maps, diagrams (only when images are actually included)
    ├── inventory-or-short-title.jpg
    └── ...                   # Caption + credit + official link live in the consuming Markdown file
```

Notes:
- **Do not leave an empty `images/` directory** in the final package. Create the folder only when at least one image is present; as a last step before packaging, remove any empty directories created during construction.
- Place the package root under an `artifacts/`, project, or working directory as available in the current environment.
- **Default output is Markdown optimized for Obsidian** (relative links, portable folder structure). EPUB is an optional additional deliverable when requested.
- **Survey packages** omit `digests/` and `02-digests.md`. They still produce a full ranked + provenance-tracked bibliography and thematic synthesis; digests are deliberately deferred for later deep dives.
- **Full packages** (Standard or Deep) include both the `digests/` folder and `02-digests.md` (index + recommended reading order with links into the individual digests).
- **Images:** Include when they materially enhance understanding (especially artworks, architecture, maps, floor plans). Prefer official museum/collection images or public-domain high-resolution sources. Store under `images/` with relative Markdown links and captions that include credit + official collection page link. Images are study references; physical conditions and hangings can change.
- `further-reading.md` is a core value of Athena (v1.4+): it must offer concrete, named next steps rather than vague suggestions, and must include notable additional primary or secondary sources discovered during research that did not make Core/Important but remain valuable (with short rationales). Deep mode expands this into research pathways.
- `01-sources.md` must include selection criteria, a Syllabi & Discovery Sources Consulted section (listing every syllabus/institutional list used), provenance notes on ranked entries, a short citation-practice note, the compiled full working bibliography, and notes on notable further-reading candidates identified during discovery. Deep mode requires richer annotations for Core and key Important sources.
- `01b-search-protocol.md` is strongly encouraged for empirical / systematic-leaning topics (and more often in Deep mode); may be a section inside `01-sources.md` when light.
- `matrix.md` is strongly recommended; required when ≥4 core sources or substantial disagreement. Deep mode almost always produces a detailed matrix.
- Each theme file must contain: (1) a short synthetic narrative; (2) **Across the Sources: What Is Easy to Miss** — a concrete checklist (typically 4–7 bullets) of structural/formal parallels, repeated devices that change function, inter-source tensions, or hinges that become visible only when sources are read together (the thematic parallel to the digest “After Reading: What Is Easy to Miss” section); (3) **Gaps & Open Questions**; (4) **Theme Bibliography**. Every major claim in theme narratives must be back-linked to a digest (Full packages) or to a primary/secondary source (Survey packages). Deep mode themes strongly recommend opening with Seminar Guiding Questions, add explicit debate mapping / intellectual genealogy, and use longer annotated bibliographies (typically 8–15 items) with positioning elements.
- For contested or politicized topics: strongly recommend a **Contested Claims & Corrections** subsection in relevant themes (and note polarization risk in limitations and selection criteria).
- `artists-bios.md` (or `creators-bios.md`) is recommended when multiple makers are central, especially for museum or collection guides.
- `author-context.md` (or `biography.md`) is recommended for single-author literary or philosophical packages (Plato, Poe, Kant, Shakespeare, etc.). Keep it lean and source-backed: intellectual biography + reception/positioning relevant to the package’s Core works. It supplies the larger conversation without becoming a full life story. Use consistently when the package centers on one primary author.
- All internal links (including images) should be relative so the package remains portable.
- Deep mode packages are recognizably denser in critical apparatus and bibliography while preserving the same navigable structure.
- Digests and theme narratives must meet density expectations (see digest-template.md Writing Rules and mode files). High-level shorthand that functions mainly as TA reminders fails the quality bar for student use.
