# Recommended Directory Layout

```
artifacts/athena-<kebab-topic>/   (or study-guide-<kebab-topic>/)
├── README.md                 # Master overview, review type, learning path, quick-start
├── 00-scope.md               # Topic statement, audience, learning outcomes, review type
├── 01-sources.md             # Ranked bibliography, selection criteria, citation practice, availability
├── 01b-search-protocol.md    # Optional/conditional: questions, search strategy, inclusion/exclusion
├── 03-themes.md              # Theme index
├── matrix.md                 # Optional/recommended: synthesis matrix (themes × sources)
├── further-reading.md        # REQUIRED & substantive: concrete pathways, named sources, how to go deeper
├── glossary.md               # Key terms with source origins
├── limitations.md            # Gaps, access issues, methodological/sourcing notes, version
├── artists-bios.md           # Recommended for multi-creator / museum topics: short parallel bios
├── digests/
│   ├── author-year-short-title.md
│   └── ...
└── themes/
    ├── 01-theme-name.md      # Includes Gaps & Open Questions + Theme Bibliography
    ├── 02-theme-name.md
    └── ...
```

Notes:
- `further-reading.md` is a core value of Athena (v1.4+): it must offer concrete, named next steps rather than vague suggestions.
- `01-sources.md` must include selection criteria and a short citation-practice note.
- `01b-search-protocol.md` is strongly encouraged for empirical / systematic-leaning topics; may be a section inside `01-sources.md` when light.
- `matrix.md` is strongly recommended; required when ≥4 core sources or substantial disagreement.
- Each theme file must contain a **Gaps & Open Questions** subsection and end with a **Theme Bibliography**.
- `artists-bios.md` (or `creators-bios.md`) is recommended when multiple makers are central, especially for museum or collection guides.
- All internal links should be relative so the package remains portable.
