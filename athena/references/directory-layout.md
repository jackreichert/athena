# Recommended Directory Layout

```
athena-<kebab-topic>/   (or study-guide-<kebab-topic>/)
├── README.md                 # Master overview, mode (Standard/Deep), review type, learning path, quick-start
├── 00-scope.md               # Topic statement, audience, mode, learning outcomes, review type
├── 01-sources.md             # Ranked bibliography with provenance notes, selection criteria, Syllabi & Discovery Sources Consulted section, citation practice, availability, full working bibliography
│                             # (Deep: richer annotations + optional Primary/Secondary/Methodological categorization)
├── 01b-search-protocol.md    # Optional/conditional: questions, search strategy, inclusion/exclusion
├── 03-themes.md              # Theme index
├── matrix.md                 # Optional/recommended: synthesis matrix (themes × sources); more detailed in Deep
├── further-reading.md        # REQUIRED & substantive: concrete pathways, named sources, how to go deeper
│                             # (Deep: multi-track research pathways, specialization tracks, journals/databases)
├── glossary.md               # Key terms with source origins
├── limitations.md            # Gaps, access issues, methodological/sourcing notes, mode, version
├── artists-bios.md           # Recommended for multi-creator / museum topics: short parallel bios
├── digests/
│   ├── author-year-short-title.md
│   └── ...                   # Primary texts: Pre-Reading Context + Summary + Full Brief (Post-Reading). Deep: + Methodological / Reception / Subsequent Engagements
└── themes/
    ├── 01-theme-name.md      # Includes Gaps & Open Questions + Theme Bibliography
    │                         # (Deep: Seminar Guiding Questions; Debates & Contending Interpretations / genealogy; longer annotated Theme Bib 8–15 items with positioning)
    ├── 02-theme-name.md
    └── ...
```

Notes:
- Place the package root under an `artifacts/`, project, or working directory as available in the current environment.
- `further-reading.md` is a core value of Athena (v1.4+): it must offer concrete, named next steps rather than vague suggestions, and must include notable additional primary or secondary sources discovered during research that did not make Core/Important but remain valuable (with short rationales). Deep mode expands this into research pathways.
- `01-sources.md` must include selection criteria, a Syllabi & Discovery Sources Consulted section (listing every syllabus/institutional list used), provenance notes on ranked entries, a short citation-practice note, the compiled full working bibliography, and notes on notable further-reading candidates identified during discovery. Deep mode requires richer annotations for Core and key Important sources.
- `01b-search-protocol.md` is strongly encouraged for empirical / systematic-leaning topics (and more often in Deep mode); may be a section inside `01-sources.md` when light.
- `matrix.md` is strongly recommended; required when ≥4 core sources or substantial disagreement. Deep mode almost always produces a detailed matrix.
- Each theme file must contain a **Gaps & Open Questions** subsection and end with a **Theme Bibliography**. Every major claim in theme narratives must be back-linked to a digest or primary source (strong citation emphasis). Deep mode themes strongly recommend opening with Seminar Guiding Questions, add explicit debate mapping / intellectual genealogy, and use longer annotated bibliographies (typically 8–15 items) with positioning elements.
- For contested or politicized topics: strongly recommend a **Contested Claims & Corrections** subsection in relevant themes (and note polarization risk in limitations and selection criteria).
- `artists-bios.md` (or `creators-bios.md`) is recommended when multiple makers are central, especially for museum or collection guides.
- All internal links should be relative so the package remains portable.
- Deep mode packages are recognizably denser in critical apparatus and bibliography while preserving the same navigable structure.
