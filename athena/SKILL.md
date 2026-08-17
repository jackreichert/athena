---
name: athena
description: Build rigorous source-backed study guides that function as university course equivalents with notes usable by both students and professors. Supports Survey (sources + themes foundation, digests deferred), Standard, and Deep modes. Digests for primary sources include pre-reading context, post-reading full brief, and standalone summary. Tracks source discovery provenance (syllabi and signals) and compiles full bibliography including notable further-reading sources. Explicit anti-bias and completeness rules. Does not dumb down or dictate interpretation. Also supports academic-level place, city, region, and museum guides; scientific paper deep dives; and legal case deep dives / case method (briefing, IRAC, Socratic analysis). Default output Markdown (Obsidian-optimized); optional EPUB. Trigger on athena, athena research, athena survey, athena deep, athena go deep, athena deeper, go deep, deeper, graduate study guide, thematic study guide, self-study package, museum guides, place guides, city guides, travel guides, scientific paper, journal club, primary literature, legal case, case brief, case method, IRAC, or similar academic requests with syllabi mining and theme synthesis.
---

# Athena (Study Guide Builder)

Create rigorous, source-backed, thematically organized study guides that function as the equivalent of a university course, with notes usable by both students and professors. Prioritize primary sources, structured digests that help the reader *not miss important things* (pre-reading context, post-reading full brief, and standalone summary), thematic synthesis with provenance, clear and dense citations (especially in themes), and navigable learning paths. Digests orient and check; they do not replace the primary encounter or tell the reader what to think.

**Process version:** 1.26 (2026-08-17) — final packaging cleanup: remove empty directories (especially unused `images/`) before zipping; create `images/` only when images are actually included.

Athena supports three package shapes that share the same research spine (syllabi mining, provenance, ranked sources, themes with citations, further reading) but differ in whether digests are produced now and in density of apparatus:

- **Survey** — Foundation package: scope + ranked sources with full provenance + thematic synthesis. Digests deliberately deferred.
- **Standard** — Full undergraduate-course-equivalent package with digests.
- **Deep** — Full graduate/seminar-equivalent package with denser digests and critical apparatus.

**On every run:** After deciding the package shape in Phase 0, **load the corresponding mode file** from `references/` (`mode-survey.md`, `mode-standard.md`, or `mode-deep.md`) and follow its adaptations for the remainder of the process. Mode files contain only the deltas; the shared spine lives here.

**When the topic is a place, city, region, museum, collection, or travel guide:** Also load `references/place-guides.md`.  
**When the topic is a primary research paper, journal-club analysis, or scientific-paper reading/critique guidance:** Also load `references/science-paper-guides.md`.  
**When the topic is a judicial opinion, case briefing, the case method, Socratic analysis, or legal case study:** Also load `references/legal-case-guides.md`.  
These adaptive applications are orthogonal to package shape.

## Guiding Principles

1. Objectives first — define clear learning outcomes, audience, and package shape before collecting sources.
2. Syllabi as expert signals — university syllabi, essential-readings lists, and (for museums/cultural sites) official institutional highlights, timed itineraries, and collection catalogues are high-value proxies for core material. For Deep mode, preferentially mine graduate seminar syllabi, comprehensive exam lists, and advanced reading lists. **Track and document every syllabus or institutional list consulted** (institution, course, URL/year when available) so source provenance remains transparent; sources that recur across independent high-quality syllabi receive higher weight.
3. Primary > Secondary, but both matter — prioritize original works (texts, artworks, artifacts); use secondary sources for orientation, context, and debate mapping. Deep mode engages a wider secondary literature including key articles and reception.
4. Consistent extraction — every Core source in Full packages receives the same structured treatment (see digest template).
5. Thematic synthesis with provenance — organize by themes/concepts/debates, not by source. Every major claim must be back-linkable (to a digest in Full packages, or to a primary/secondary source in Survey).
6. Active and navigable output — recommended reading order, self-test or seminar questions, glossary, modular Markdown.
7. Transparency and balance — document selection criteria, note limitations, seek multiple perspectives. Explicit anti-bias practices on contested topics.
8. Progressive disclosure — support high-level overviews (Survey) and deep dives (Standard/Deep) within the same spine.
9. Completeness over ambition (Full packages) — every Core source must receive a complete digest before themes are written. If this cannot be done, reduce Core and document the change. Survey packages deliberately omit digests and are not subject to this gate.
10. Anti-reductive — digests help the reader see more, not less. Do not dumb down, moralize, or hand the reader “the meaning.” Prefer the source’s own force and precision; surface tensions and open questions.
11. Visual materials when they help — for artworks, architecture, maps, diagrams, or other visual primary sources, include high-quality reference images (with credit and official links) when they materially aid understanding. Prefer official museum/collection images or public-domain sources. Store under `images/` with relative Markdown links.
12. Citations, provenance, and further research are core values, not optional extras.

## Core Value: Citations, Sources & Further Research

Athena packages exist to help users engage primary material *and* know where the claims come from and how to go further.

### In `01-sources.md`
- Explicit selection criteria.
- **Syllabi & Discovery Sources Consulted** section: list every syllabus, essential-readings list, institutional highlight/itinerary, or other discovery source used.
- Ranked Core / Important / Supplementary lists with short rationales and provenance notes.
- Clear identification of primary institutional or canonical sources.
- A short “Citation practice in this package” note.
- Availability notes.
- **Full bibliography compilation** of the ranked lists plus additional discovered sources. Maintain and refine it throughout Phase 1.
- Deep mode: richer annotations (positioning/evaluative) and optional categorization. See mode-deep.md.

### In digests
- Every major claim or observation is grounded. High-signal quotes with locators where possible.
- For empirical findings that are contested or revised: brief status note (original claim / later challenges / present standing).

### In themes
- **Citation practice is especially rigorous here:** every major claim in a theme narrative must be back-linked to a specific digest (Full packages) or to a primary/secondary source (Survey packages). Themes are the primary site where provenance and evidence transparency are demonstrated.
- **Across the Sources: What Is Easy to Miss** required: a short, concrete checklist (typically 4–7 bullets) of structural/formal parallels, devices that change function across texts, inter-source tensions, or hinges visible only in comparison. This is the thematic parallel to the digest “After Reading: What Is Easy to Miss” section.
- Gaps & Open Questions subsection required.
- Theme Bibliography required.
- Deep mode: Seminar Guiding Questions, debate mapping / intellectual genealogy, longer annotated bibliographies. See mode-deep.md.

### In `further-reading.md` (required and substantive)
- Concrete, named next steps and pathways, not vague suggestions.
- Include notable additional primary or secondary sources discovered during research that did not make Core/Important but remain valuable.
- Deep mode expands this into multi-track research pathways.

### In `limitations.md`
- Document package shape, digests in/out of scope, access issues, methodological notes, and any narrowing of Core.
- On contested topics, note polarization risk in selection.

### Anti-bias practices for contested or politicized domains
- Prefer primary evidence for disputed facts.
- Surface competing interpretations with their evidence bases.
- Document polarization risk in selection criteria and limitations.
- In Deep mode, add claim-genealogy guidance where relevant.

## Package Shapes (high-level)

All three shapes share the research spine. Decide the shape in Phase 0 from user language and topic, declare it in `00-scope.md`, then **load the mode file**.

- **Survey**: Digests out of scope by design. Foundation / map-the-field package. See `references/mode-survey.md`.
- **Standard** (default for full packages): Undergrad-course equivalent with complete digests. See `references/mode-standard.md`.
- **Deep**: Graduate/seminar equivalent with denser apparatus. See `references/mode-deep.md`.

Default to Standard unless Survey language (“survey”, “overview”, “sources and themes only”, “no digests yet”) or Deep language (“deep”, “graduate”, “seminar”, “go deep”, “deeper”) is present.

## Adaptive Applications

### Place / Location / Travel & Museum Guides
When the request is for a place, city, region, historic landscape, museum, collection, or serious travel guide, load `references/place-guides.md` and follow its requirements. These guides operate at academic depth (Blue Guide / university city-history spirit), not tourist-brochure style. They can be produced in any package shape. Short shared rules:

- Start with syllabi or highest-quality scholarly sources; full provenance required.
- Treat sites, monuments, neighborhoods, landscapes, and artworks as primary sources.
- Produce historical orientation + must-see sites with scholarly rationale + practical itineraries grounded in the literature.
- Include images when they enhance understanding.
- Museum specializations (dual-layer artwork digests, Period-Specialist Analysis, artists-bios.md) are retained and required when applicable.

Full details are in the reference file.

### Scientific Paper Deep Dives
When the topic is a primary research paper (or tightly related set), a journal-club style analysis, or an explicit request for guidance on reading / critiquing / positioning scientific papers, load `references/science-paper-guides.md`. Grounded in how strong scientific training programs actually teach these skills (CREATE, active-reading checklists, critical-appraisal traditions, genre/positioning analysis). Key overlays: independent figure interpretation, results-vs-interpretation distinction, limitations and alternative explanations, generative “next experiment” moves, and CARS-style positioning awareness. Full digest adaptations and theme emphases are in the reference file.

### Legal Case Deep Dives / Case Method
When the topic is a judicial opinion or set of opinions, case briefing, the case method, Socratic analysis, or legal case study, load `references/legal-case-guides.md`. Grounded in the pedagogy of the Langdellian case method and its evolutions (case briefing / IRAC practice, Socratic classroom dynamics, contextual and problem-solving reforms). Key overlays: precise issue formulation, rule extraction, fact materiality, application/analogical reasoning, holding vs. dicta, scope notes, and generative hypotheticals. Full digest adaptations and theme emphases are in the reference file.

## Workflow

Execute the phases in order, with explicit iteration checkpoints. Write all deliverables as Markdown files in a dedicated, self-contained directory (commonly `artifacts/athena-<topic-slug>/` — adapt the root path to the current environment). Keep the package portable with relative links only.

### Phase 0: Scope Definition
Before any searching:
- Write a concise topic statement.
- Specify target audience / level and **package shape** (Survey / Standard / Deep). Explicitly state whether digests are in scope.
- Define learning outcomes.
- Note review type (e.g., hybrid) and any constraints.
- Decide output format (default Markdown/Obsidian; EPUB if requested).
- **Load the mode file** for the chosen shape. Also load any applicable adaptive-application file (place-guides, science-paper-guides, or legal-case-guides).
Deliverable: `00-scope.md`.

### Phase 1: Source Discovery & Selection
- Mine syllabi and high-quality discovery sources; log every one consulted.
- Rank Core / Important / Supplementary with provenance notes and rationales.
- Compile the full working bibliography.
- Selection criteria, citation-practice note, availability notes required.
- Deep mode: denser annotations. See mode file.
Deliverable: `01-sources.md` (and optional `01b-search-protocol.md`).

**Iteration checkpoint:** Confirm Core list is realistic for the shape. For Full packages, ensure digests are feasible. For Survey, confirm digests remain out of scope.

### Phase 2: Structured Source Digests (Full packages only)
**Skip entirely for Survey** (see mode-survey.md). For Standard and Deep, produce a consistent digest for every Core source (and selected Important) using `references/digest-template.md`.

Primary-text structure (literary, philosophical, dialogic works): three-part treatment required —
1. **Pre-Reading Context** — lean, non-spoiling orientation.
2. **Summary** — compact standalone overview.
3. **Full Brief (Post-Reading)** — denser engagement after the reader has encountered the primary; helps notice structure, moves, cross-links, open questions.

Anti-reductive rule applies. For artworks/visual objects: dual-layer (Unit/Zone + Period-Specialist Analysis) + images as specified in place-guides.md and the template. Deep mode adds methodological/reception sections.

**Completeness gate (Full packages):** Do not begin Phase 3 until every Core source has a complete digest. If the planned Core is not feasible, reduce it, update sources, and note in limitations.

Deliverable: `digests/` + `02-digests.md` (index + recommended reading order).

### Phase 3: Thematic Synthesis & Cross-Referencing
Extract themes, build at least one synthesis matrix (strongly recommended; required when ≥4 core sources or substantial disagreement; Deep almost always detailed), write theme narratives with Gaps & Open Questions and Theme Bibliography.

Citation practice is rigorous: every major claim back-linked. In Survey, cite sources directly and note that digests can be added later.

Deep mode enhancements (Seminar Guiding Questions, debate mapping, richer Theme Bibliographies, Contested Claims subsections on polarized topics) are in mode-deep.md.

For museum/site guides, include a practical Navigating / Walkthrough / Practical Paths theme.

Deliverable: `03-themes.md` + `themes/` + `matrix.md` (or embedded).

### Phase 4: Study Guide Assembly
Required structure (adapt per mode and directory-layout.md):
- `README.md` — topic, package shape, review type, outcomes, how to use, learning path, theme index, quick-start. Point to `02-digests.md` when present.
- `00-scope.md`, `01-sources.md`, theme files, `further-reading.md`, `glossary.md`, `limitations.md`.
- Full packages also include digests and `02-digests.md`.
- Place guides may include `artists-bios.md` and `images/`.

### Phase 5: Quality Assurance
- Completeness check (Full packages): every Core has a digest that meets quality expectations; `02-digests.md` correct.
- Survey: digests correctly omitted; themes still cite sources.
- Provenance and Syllabi section present and accurate.
- Citations dense in themes.
- Further-reading substantive.
- Relative links only; images credited.
- Package shape declared and consistent.
- Deep packages recognizably denser; Survey packages clean and complete as foundations.
- Empty directories (especially an unused `images/`) have been removed before packaging.

## Output Conventions
- Default: portable Markdown optimized for Obsidian (relative links, clean headings).
- Optional EPUB when requested.
- Images under `images/` with relative links and captions (credit + official link). Create the `images/` directory only when at least one image is actually included; do not leave an empty `images/` folder in the final package.
- **Final packaging cleanup (required):** Before zipping, remove any empty directories that were created during construction (most commonly an unused `images/` folder). The delivered package should contain only directories that hold files.
- At the end, offer a downloadable zip of the finished package when the environment supports it.
- Survey packages are not “incomplete Standard packages.”
- Deep packages remain navigable despite density.

## Constraints & Notes
- Do not invent sources or fabricate quotes, page numbers, inventory numbers, or room locations.
- Favor open-access and official institutional resources when quality is comparable.
- Keep digests dense but readable; abstract-only digests are not acceptable in Deep mode.
- Completeness over ambition for Full packages.
- Citations, provenance, and further research are part of the definition of a finished Athena package.
- Anti-bias is structural on contested topics.
- This skill is designed to be portable across agents that support the Agent Skills format. Adapt file-system paths and tool calls to the current runtime.
- See `DEVELOPMENT.md` for how to expand the skill without breaking the modular contract.

## Resources
- Mode files (load after Phase 0 decision):
  - `references/mode-survey.md`
  - `references/mode-standard.md`
  - `references/mode-deep.md`
- Adaptive applications:
  - Place / museum / location: `references/place-guides.md`
  - Scientific paper deep dives: `references/science-paper-guides.md`
  - Legal case deep dives / case method: `references/legal-case-guides.md`
- Digest template: `references/digest-template.md` (includes Deep adaptations)
- Example directory layout: `references/directory-layout.md`
- Skill maintenance notes: `DEVELOPMENT.md`
- Changelog (package top level, not required at runtime): `CHANGELOG.md`
