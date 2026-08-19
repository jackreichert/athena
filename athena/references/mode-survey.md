# Survey Mode (Athena)

Load this file when the package shape is **Survey**.

## Purpose
A rigorous **foundation package**. Produces scope, a full ranked + provenance-tracked bibliography, thematic synthesis, further reading, glossary, and limitations. Digests are **deliberately out of scope** so the reader can later request individual digests or a Standard/Deep treatment of particular works. Themes still carry dense citations, but they point to primary sources and secondary literature directly rather than to digests.

Ideal language triggers: “survey of…”, “overview of…”, “sources and themes only”, “no digests yet”, “foundation for later deep dives”, “map the field first”. Use this shape when the user wants the map before committing to close reading of every Core text.

## Key differences from Standard / Deep
- **Phase 2 is skipped entirely.** Record the deferral explicitly in `00-scope.md` and `limitations.md`. Proceed directly to Phase 3 after sources are ranked.
- No `digests/` directory and no `02-digests.md`.
- In themes (Phase 3): every major claim is back-linked to a primary or secondary source (not to a digest). Note in theme files or limitations that full digests can be requested later for closer engagement.
- Completeness gate does **not** apply. Survey packages are complete when the research spine (scope + ranked provenance-tracked sources + themes with citations + further reading) is solid.
- `further-reading.md` should explicitly note that digests of Core works can be requested later.
- Digests remain available as a future expansion path; do not treat Survey as an “incomplete Standard.”

## Phase adaptations
### Phase 0
Declare package shape = Survey. Explicitly state “Digests: out of scope (deferred).” Learning outcomes focus on orientation, source map, and thematic overview rather than close reading mastery.

### Phase 1
Identical research spine. Rank sources carefully; the ranked list *is* the main deliverable of this phase for Survey.

### Phase 2
**Skip.** Do not produce digests. Do not create `02-digests.md`.

### Phase 3
Themes cite sources directly. Still require Gaps & Open Questions and Theme Bibliography. Matrix recommended when useful.

### Phase 4 / 5
Assemble without digests. The mandatory Phase 5 integrity audit still applies: every theme file listed in `03-themes.md` must exist on disk; digests must be correctly absent. QA focuses on provenance transparency, citation density in themes, and whether the package functions as a solid foundation the user can expand later.
