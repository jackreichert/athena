---
name: athena
description: Build rigorous source-backed study guides that function as university course equivalents with notes usable by both students and professors. Supports Survey, Standard, and Deep modes. Digests include pre-reading context, standalone summary, and post-reading brief. Tracks syllabus provenance and compiles a full bibliography. After a draft Core list exists, mines the scholarly apparatus of Core works that have one as a bounded second discovery pass. Supports a follow-up citation-network expansion against a finished package. Anti-bias and completeness rules. Does not dumb down or dictate interpretation. Also supports place, city, museum, and travel guides (Markdown package first, then a high-class visitor EPUB that contains all the original dual-layer content, reorganized for on-site use, with elegant cover, TOC, ranked must-see checklist, and location/institution history); scientific paper deep dives; legal case method; and practical hands-on course supplements (workbooks, lab and studio companions, practicums). Default Markdown; optional EPUB. Trigger on athena, athena survey, athena deep, go deep, graduate study guide, self-study package, museum or place or city or travel guides, journal club, legal case, case brief, case method, IRAC, practical guide, workbook, lab manual, studio handbook, practicum, implementation companion, expand from bibliographies, citation network, next ring from Core, or similar academic requests with syllabi mining and theme synthesis.
---

# Athena (Study Guide Builder)

Create rigorous, source-backed, thematically organized study guides that function as the equivalent of a university course, with notes usable by both students and professors. Prioritize primary sources, structured digests that help the reader *not miss important things* (pre-reading context, post-reading full brief, and standalone summary), thematic synthesis with provenance, clear and dense citations (especially in themes), and navigable learning paths. Digests orient and check; they do not replace the primary encounter or tell the reader what to think.

**Process version:** 1.35 (2026-09-28) — After a draft Core list exists, Phase 1 runs a **bounded apparatus / bibliography pass** on Core works that have scholarly apparatus. Extracted citations enter the working bibliography with provenance; they do not auto-promote to Core. Deep mode expects a richer version. User language such as “expand from bibliographies,” “citation network,” or “next ring from Core” runs a Phase 1b addendum against a finished package (`01c-citation-network.md`) without reopening the digest completeness gate unless the user explicitly reopens ranking. Shared-spine change; no new mode or adaptive application.

Athena supports three package shapes that share the same research spine (syllabi mining, provenance, ranked sources, themes with citations, further reading) but differ in whether digests are produced now and in density of apparatus:

- **Survey** — Foundation package: scope + ranked sources with full provenance + thematic synthesis. Digests deliberately deferred.
- **Standard** — Full undergraduate-course-equivalent package with digests.
- **Deep** — Full graduate/seminar-equivalent package with denser digests and critical apparatus.

**On every run:** After deciding the package shape in Phase 0, **load the corresponding mode file** from `references/` (`mode-survey.md`, `mode-standard.md`, or `mode-deep.md`) and follow its adaptations for the remainder of the process. Mode files contain only the deltas; the shared spine lives here.

**When the topic is a place, city, region, museum, collection, or travel guide:** Also load `references/place-guides.md`.  
**When the topic is a primary research paper, journal-club analysis, or scientific-paper reading/critique guidance:** Also load `references/science-paper-guides.md`.  
**When the topic is a judicial opinion, case briefing, the case method, Socratic analysis, or legal case study:** Also load `references/legal-case-guides.md`.  
**When the user asks for a practical / hands-on / workbook / lab / studio / practicum / implementation / job-aid companion, or the topic is itself that kind of course:** Also load `references/practical-guides.md`. Do not auto-add this overlay to ordinary study-guide runs.  
These adaptive applications are orthogonal to package shape.

## Guiding Principles

1. Objectives first — define clear learning outcomes, audience, and package shape before collecting sources.
2. Syllabi as expert signals — university syllabi, essential-readings lists, and (for museums/cultural sites) official institutional highlights, timed itineraries, and collection catalogues are high-value *teaching* proxies for core material. For Deep mode, preferentially mine graduate seminar syllabi, comprehensive exam lists, and advanced reading lists. **Track and document every syllabus or institutional list consulted** with rich provenance (institution, course, year/term, URL or stable identifier, retrieval date, and a short note on what was extracted). Prefer archive.org or other durable mirrors when the original is fragile. Full Markdown archival under `source-materials/` is optional and recommended only for especially valuable or unstable syllabi (and, when relevant and rights-permissive, short accessible sources); when created, link the local copy from the Syllabi section of `01-sources.md`. **After a draft Core list exists, treat the scholarly apparatus of those Core works as a second expert signal** (bibliographies, endnotes, recommended-reading chapters, editors’ notes in critical editions). Syllabi are a teaching-canon signal; book apparatus is a research-canon signal. Log apparatus sources with the same provenance discipline. Do not copy entire bibliographies. Extracted citations compete for Important / Supplementary / further-reading slots; they do not auto-promote to Core.
3. Primary > Secondary, but both matter — prioritize original works (texts, artworks, artifacts); use secondary sources for orientation, context, and debate mapping. Deep mode engages a wider secondary literature including key articles and reception.
4. Consistent extraction — every Core source in Full packages receives the same structured treatment (see digest template).
5. Thematic synthesis with provenance — organize by themes/concepts/debates, not by source. Every major claim must be back-linkable (to a digest in Full packages, or to a primary/secondary source in Survey).
6. Active and navigable output — recommended reading order, self-test or seminar questions, glossary, modular Markdown.
7. Transparency and balance — document selection criteria, note limitations, seek multiple perspectives. Explicit anti-bias practices on contested topics.
8. Progressive disclosure — support high-level overviews (Survey) and deep dives (Standard/Deep) within the same spine.
9. Completeness over ambition (Full packages) — every Core *and* Important source must receive a complete digest before themes are written. If this cannot be done, reduce the lists and document the change in limitations. Survey packages deliberately omit digests and are not subject to this gate. **After assembly, a package integrity audit is mandatory:** (a) the top-level index files themselves (`02-digests.md`, `03-themes.md`) must be complete and accurate; (b) every Core and Important source must have a corresponding complete digest file under `digests/`; (c) every theme topic listed in `03-themes.md` must have a corresponding complete theme file under `themes/`. Missing or incomplete files trigger an immediate return to the relevant phase until the audit passes. A package that only has overview/index files without the referenced content is incomplete and must not be delivered.
10. Anti-reductive — digests help the reader see more, not less. Do not dumb down, moralize, or hand the reader “the meaning.” Prefer the source’s own force and precision; surface tensions and open questions.
11. Visual materials when they help — for artworks, architecture, maps, diagrams, or other visual primary sources, include high-quality reference images (with credit and official links) when they materially aid understanding. Prefer official museum/collection images or public-domain sources. Store under `images/` with relative Markdown links.
12. Citations, provenance, and further research are core values, not optional extras.

## Core Value: Citations, Sources & Further Research

Athena packages exist to help users engage primary material *and* know where the claims come from and how to go further.

### In `01-sources.md`
- Explicit selection criteria.
- **Syllabi & Discovery Sources Consulted** section: list every syllabus, essential-readings list, institutional highlight/itinerary, or other discovery source used, with rich provenance (institution, course, year/term, URL or stable identifier, retrieval date, short extraction note). Prefer durable links (e.g. archive.org). When an optional local Markdown copy was created under `source-materials/`, include a relative link to it alongside the original.
- **Apparatus & Bibliographies Consulted** section (required when any Core work with apparatus was mined; otherwise a one-line “none applicable / not yet run” note): list each mined Core source, what kind of apparatus it offered, how many citations were pulled, and the selection rule used. Each extracted item in the working bibliography carries a provenance note of the form *cited in [Core work], ch./pp., why pulled*.
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
- Theme Bibliography required. When a Core source’s apparatus cites a work *on this theme*, that citation is eligible for the theme bibliography with a back-link (“cited as decisive in X”).
- Deep mode: Seminar Guiding Questions, debate mapping / intellectual genealogy, longer annotated bibliographies. See mode-deep.md.

### In `further-reading.md` (required and substantive)
- Concrete, named next steps and pathways, not vague suggestions.
- Include notable additional primary or secondary sources discovered during research that did not make Core/Important but remain valuable.
- Prefer items that recur across two Core apparatuses, or that a Core author flags as decisive, when those were harvested in the Phase 1 apparatus pass.
- Deep mode expands this into multi-track research pathways. When `01c-citation-network.md` exists, point to it from further-reading.

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
- **Historical overview and location/institution context are required.** For city and travel guides this is a layered chronology. For museum guides it includes the building’s history, the institution’s founding and development, the dynasty or patronage system, and major political or cultural settlements that frame the works.
- **Rank unmissable works and spaces.** Do not artificially cap digests. Prioritize what a careful visitor would most regret missing on a single visit, present a clear priority order (short route and full route), and let the visitor decide depth.
- Produce must-see sites with scholarly rationale + practical itineraries grounded in the literature.
- Include images when they enhance understanding.
- Museum specializations (dual-layer artwork digests, Period-Specialist Analysis, artists-bios.md) are retained and required when applicable.
- **Two-step delivery (default for museum and major site guides):**  
  1. Markdown package first — full research, ranked sources, complete dual-layer digests, themes, glossary, further reading, limitations. Delivered as a zip.  
  2. Visitor EPUB — after the Markdown package is audited, a polished sequential EPUB that restructures *the same content* for on-site use. The EPUB does not abbreviate the dual-layer analysis. It includes an elegant cover, Table of Contents, ranked must-see checklist, location and institutional history, linear walk-through chapters with full dual-layer briefs, themes, visitor information, and practical notes. Both the Markdown zip and the EPUB are delivered.  
  See `references/place-guides.md` for the full process.

### Scientific Paper Deep Dives
When the topic is a primary research paper (or tightly related set), a journal-club style analysis, or an explicit request for guidance on reading / critiquing / positioning scientific papers, load `references/science-paper-guides.md`. Grounded in how strong scientific training programs actually teach these skills (CREATE, active-reading checklists, critical-appraisal traditions, genre/positioning analysis). Key overlays: independent figure interpretation, results-vs-interpretation distinction, limitations and alternative explanations, generative “next experiment” moves, and CARS-style positioning awareness. Full digest adaptations and theme emphases are in the reference file.

### Legal Case Deep Dives / Case Method
When the topic is a judicial opinion or set of opinions, case briefing, the case method, Socratic analysis, or legal case study, load `references/legal-case-guides.md`. Grounded in the pedagogy of the Langdellian case method and its evolutions (case briefing / IRAC practice, Socratic classroom dynamics, contextual and problem-solving reforms). Key overlays: precise issue formulation, rule extraction, fact materiality, application/analogical reasoning, holding vs. dicta, scope notes, and generative hypotheticals. Full digest adaptations and theme emphases are in the reference file.

### Practical Guides / Hands-on Course Supplements
When the user asks for a practical companion to a course (workbook, lab or studio manual, practicum, implementation guide, job aid) or the topic is itself that kind of course, load `references/practical-guides.md`. Grounded in a Discovery-first Deep run on practical-guide pedagogy (cognitive apprenticeship, 4C/ID, worked examples and fading, Schön’s practicum, backward design / constructive alignment, laboratory genre critique, checklists as performance support). The companion is a supplement that makes the reader *do* the work the course claims to teach — a task sequence with declared guidance states (modeled / faded / independent / exploratory-with-scaffolds), not a quiz on the digests and not an auto-added exercise dump. Full file requirements and quality gates are in the reference file.

## Workflow

Execute the phases in order, with explicit iteration checkpoints. Write all deliverables as Markdown files in a dedicated, self-contained directory (commonly `artifacts/athena-<topic-slug>/` — adapt the root path to the current environment). Keep the package portable with relative links only.

### Phase 0: Scope Definition
Before any searching:
- Write a concise topic statement.
- Specify target audience / level and **package shape** (Survey / Standard / Deep). Explicitly state whether digests are in scope.
- Define learning outcomes.
- Note review type (e.g., hybrid) and any constraints.
- Decide output format (default Markdown/Obsidian; EPUB if requested).
- **Load the mode file** for the chosen shape. Also load any applicable adaptive-application file (place-guides, science-paper-guides, legal-case-guides, or practical-guides).
- Note that the primary university department affiliation will be decided later (after research and themes) and recorded in the final `00-scope.md` and package `README.md`.
Deliverable: `00-scope.md` (initial; departmental home added in Phase 4).

### Phase 1: Source Discovery & Selection
- Mine syllabi and high-quality discovery sources; log every one consulted with rich provenance (institution, course, year/term, URL or stable identifier, retrieval date, short extraction note). Prefer durable links (e.g. archive.org) when originals are fragile.
- **Optional archival:** For especially valuable or unstable syllabi (and, when relevant and rights-permissive, short accessible sources), create clean Markdown reformats under `source-materials/syllabi/` (or `source-materials/sources/`). Each archived file must open with a header containing original URL, institution/course (or title), retrieval date, and reformatting notes. Prefer open/public materials; never archive paywalled or restricted content. Full-length copyrighted monographs are never copied—link only.
- Rank a *draft* Core / Important / Supplementary list with provenance notes and rationales.
- **Bounded apparatus / bibliography pass (required when any draft-Core work has usable apparatus):** After the draft Core list exists, mine the scholarly apparatus of those Core works that actually have one — secondary monographs, handbooks, survey books, annotated translations, critical editions (editors’ notes / recommended reading). Do **not** treat a bare primary (dialogue, lyric, untreated treatise, single opinion) as if it had a research bibliography; use a standard commentary or critical edition only when that edition is itself in Core or clearly identified. Cap extraction at about **5–15 high-signal citations per mined Core source**. Prefer items that (a) recur across two or more Core apparatuses, or (b) the author flags as decisive, foundational, or the position being answered. Log each mined apparatus in **Apparatus & Bibliographies Consulted**. Each extracted title enters the working bibliography with provenance *cited in [Core work], locator, why pulled*. **Do not copy entire bibliographies** into `source-materials/` or `01-sources.md`. **Do not auto-promote** extracted titles to Core. They compete for Important / Supplementary / further-reading (and, when a theme already exists or is taking shape, for that theme’s bibliography). Recurrence in bibliographies is evidence, not proof of canonicity — authors cite allies; cross-check against syllabi and a second Core book.
- Compile the full working bibliography (ranked lists + apparatus harvest + other discoveries).
- Selection criteria, citation-practice note, availability notes required.
- Deep mode: denser annotations and a richer apparatus pass. See mode file.
Deliverable: `01-sources.md` (and optional `01b-search-protocol.md`); `source-materials/` only when copies were actually created.

**Iteration checkpoint:** Confirm Core list is realistic for the shape. For Full packages, ensure digests are feasible. For Survey, confirm digests remain out of scope. Confirm the apparatus pass either ran on eligible Core works or recorded why it did not apply.

### Phase 1b: Citation-network expansion (on request, against a finished package)
Trigger language: “expand from bibliographies,” “citation network,” “next ring from Core,” “mine the Core apparatuses,” or an explicit request to thicken further-reading from the books already chosen.

This is a **reopen of discovery only**. Input is the current package’s Core + Important lists in `01-sources.md`. Output is `01c-citation-network.md`: clustered next-ring sources, recurrence counts, which Core book pointed where, and short notes on why an item is or is not a candidate for later promotion. Point to the new file from `further-reading.md` and add an Apparatus subsection to `01-sources.md` if it was missing.

**Do not reopen the digest completeness gate** and do not move titles into Core or Important unless the user explicitly asks to reopen ranking. If ranking is reopened on a Full package, treat newly promoted Important items as new digest obligations and return to Phase 2 before re-auditing.

Survey and Standard run this pass only on request. Deep may run a richer version during initial Phase 1 (see `mode-deep.md`) and should still produce `01c-citation-network.md` when the user asks for the addendum later.

### Phase 2: Structured Source Digests (Full packages only)
**Skip entirely for Survey** (see mode-survey.md). For Standard and Deep, produce a consistent digest for **every Core source and every Important source** using `references/digest-template.md`.

Primary-text structure (literary, philosophical, dialogic works): three-part treatment required —
1. **Pre-Reading Context** — lean, non-spoiling orientation, including Watch-fors and, when the source is long, composite, or formally odd, a **How to read this source (first encounter)** route (named units + stopping rule). See `references/digest-template.md`.
2. **Summary** — compact standalone overview.
3. **Full Brief (Post-Reading)** — denser engagement after the reader has encountered the primary; helps notice structure, moves, cross-links, open questions. Deep mode may add a short second-pass route after the Full Brief when the first pass postponed material.

Anti-reductive rule applies. For artworks/visual objects: dual-layer (Unit/Zone + Period-Specialist Analysis) + images as specified in place-guides.md and the template. Deep mode adds methodological/reception sections.

**Completeness gate (Full packages):** Do not begin Phase 3 until every Core *and* Important source has a complete digest. If the planned lists are not feasible, reduce them, update `01-sources.md`, and note the change in limitations.

Deliverable: `digests/` (one complete file per Core and Important source) + `02-digests.md` (complete index + recommended reading order that accurately lists every digest).

### Phase 3: Thematic Synthesis & Cross-Referencing
Extract themes, build at least one synthesis matrix (strongly recommended; required when ≥4 core sources or substantial disagreement; Deep almost always detailed), write theme narratives with Gaps & Open Questions and Theme Bibliography.

Citation practice is rigorous: every major claim back-linked. In Survey, cite sources directly and note that digests can be added later.

Deep mode enhancements (Seminar Guiding Questions, debate mapping, richer Theme Bibliographies, Contested Claims subsections on polarized topics) are in mode-deep.md.

For museum/site guides, include a practical Navigating / Walkthrough / Practical Paths theme.

Deliverable: `03-themes.md` + `themes/` + `matrix.md` (or embedded).

**Departmental home decision (required, post-research, pre-packaging):** After Phase 3 is complete (sources ranked, themes synthesized), decide the primary university department or program that would most naturally house a course of this kind. Base the decision on the Core sources, the syllabi actually mined, the thematic focus, and the learning outcomes. Prefer the single strongest departmental home indicated by the material (e.g., Philosophy, Classics, History, Religious Studies, Political Science, Comparative Literature, Art History, English, Law, Biology, etc.). If the package is genuinely interdisciplinary, name the primary department and note secondary affiliations. This step occurs after research so the sources and themes inform the placement; do not invent a department early. Record the decision in both the final `00-scope.md` and the package `README.md`.

### Phase 4: Study Guide Assembly
Required structure (adapt per mode and directory-layout.md):
- `README.md` — topic, package shape, **primary university department / program**, review type, outcomes, how to use, learning path, theme index, quick-start. Point to `02-digests.md` when present.
- `00-scope.md` — must include the departmental home (primary + any secondary affiliations) decided after Phase 3, along with topic statement, audience, package shape, learning outcomes, review type, digests in/out of scope, and output format.
- `01-sources.md`, theme files, `further-reading.md`, `glossary.md`, `limitations.md`.
- Full packages also include digests and `02-digests.md`.
- Place guides may include `artists-bios.md` and `images/`.
- Practical companions, when in scope, include `practical/` (see `references/practical-guides.md` and directory-layout.md).

### Phase 5: Quality Assurance & Package Integrity Audit (mandatory)
This phase is not a passive checklist. After Phase 4 assembly, **perform an active filesystem audit** of the package directory using available tools (ls, find, read_file, or equivalent). The package is incomplete and must not be declared finished until every check below passes. If any check fails, **immediately return to the responsible earlier phase**, create or repair the missing/incomplete content, re-assemble as needed, and re-run the full audit.

**Integrity audit steps (execute in order):**

1. **Shape consistency:** Confirm `00-scope.md` declares the correct package shape and that digests are present or absent accordingly (Survey: no `digests/` and no `02-digests.md`; Full packages: both present).

2. **Required top-level files exist, are non-empty, and are complete:**
   - `README.md`, `00-scope.md`, `01-sources.md`, `03-themes.md`, `further-reading.md`, `glossary.md`, `limitations.md`.
   - Full packages also require a complete `02-digests.md`.
   - `matrix.md` when required by the mode/layout; `author-context.md` or `artists-bios.md` when the topic warrants them.
   - **Top-level index completeness:** `02-digests.md` (when present) and `03-themes.md` must themselves be fully written — accurate lists, working relative links, recommended reading order / theme index, and no placeholder or stub content. An incomplete index file fails the audit even if some child files exist.

3. **Themes integrity (critical):**
   - Parse `03-themes.md` (and the theme index section of `README.md`) for the complete list of theme topics / files.
   - Verify **every** listed theme has a corresponding complete file under `themes/` (non-empty, not a stub).
   - Spot-check that each theme file contains the required sections: synthetic narrative, **Across the Sources: What Is Easy to Miss**, Gaps & Open Questions, Theme Bibliography (plus Deep-mode extras when applicable).
   - If any theme topic lacks a complete file or required sections → return to Phase 3, write the missing/incomplete themes, update indexes, and re-audit.

4. **Digests integrity (Full packages only):**
   - Parse `01-sources.md` for the full Core list **and** the full Important list.
   - Parse `02-digests.md` (and any digest lists in `README.md`) for the digest files it claims to cover.
   - Verify **every Core source and every Important source** has a corresponding complete digest file under `digests/` (non-empty, not a stub).
   - Verify every digest listed in `02-digests.md` actually exists and is complete.
   - Spot-check that digests follow the template (Pre-Reading Context + Summary + Full Brief for primary texts; required “After Reading: What Is Easy to Miss”; **How to read this source** present when the source is long, composite, or formally odd; density expectations).
   - If any Core or Important source lacks a complete digest, or if `02-digests.md` is incomplete/mismatched → return to Phase 2, complete the digests and the index, and re-audit.

5. **Cross-links and provenance:**
   - Relative links only; no broken internal links to digests or themes.
   - Syllabi & Discovery Sources section in `01-sources.md` is present with rich provenance; any `source-materials/` copies are linked and properly headed.
   - Apparatus & Bibliographies Consulted is present in `01-sources.md` (a completed subsection, or a one-line note that no eligible Core apparatus existed / the pass was not applicable). Extracted items that were used carry *cited in [Core work]* provenance.
   - If Phase 1b ran, `01c-citation-network.md` exists, is non-empty, and is linked from `further-reading.md`. Do not treat a missing `01c` as an audit failure on an ordinary first-assembly run.
   - Citations in themes are dense and back-linkable.

6. **Content quality gates:**
   - Further-reading is substantive (named sources and concrete pathways).
   - Deep packages show denser apparatus; Survey packages are clean foundations with digests correctly omitted.
   - No fabricated sources, quotes, or locators.

7. **Final packaging cleanup:** Remove any empty directories (`images/`, `source-materials/`, `practical/`, etc.) that were created but unused. The delivered package must contain only directories that hold files.

8. **Adaptive-application extras:** If an overlay required additional files (for practical companions, `practical/` plus every task listed in `practical/01-sequence.md`), include those in this audit and follow that overlay’s extra gates. An empty or stub `practical/` fails the same way a missing digest fails.

**Only after the integrity audit fully passes** may the package be considered complete. Offer the downloadable zip of the finished package. Do not stop early with only overview/index files present.

## Output Conventions
- Default: portable Markdown optimized for Obsidian (relative links, clean headings).
- Optional EPUB when requested.
- Images under `images/` with relative links and captions (credit + official link). Create the `images/` directory only when at least one image is actually included; do not leave an empty `images/` folder in the final package.
- Optional source materials (high-value syllabi and short sources) under `source-materials/` when created. Each file carries a header with the original link. Create the directory only when at least one file is present.
- **Final packaging cleanup (required):** Before zipping, remove any empty directories that were created during construction (most commonly an unused `images/` or `source-materials/` folder). The delivered package should contain only directories that hold files.
- **Package integrity is a hard gate:** The integrity audit in Phase 5 must pass before any zip is offered or the package is declared complete. This includes: (1) complete top-level index files (`02-digests.md`, `03-themes.md`); (2) a complete digest file for every Core *and* Important source; (3) a complete theme file for every theme topic listed in `03-themes.md`. Overview/index files without their referenced content do not constitute a finished package.
- At the end, offer a downloadable zip of the finished package when the environment supports it.
- Survey packages are not “incomplete Standard packages.”
- Deep packages remain navigable despite density.

## Constraints & Notes
- Do not invent sources or fabricate quotes, page numbers, inventory numbers, or room locations.
- Favor open-access and official institutional resources when quality is comparable.
- Keep digests dense but readable; abstract-only digests are not acceptable in Deep mode.
- Completeness over ambition for Full packages. The post-assembly integrity audit is non-negotiable: incomplete top-level indexes, any Core or Important source without a complete digest, or any theme topic without a complete theme file makes the package incomplete.
- Citations, provenance, and further research are part of the definition of a finished Athena package. Apparatus mining is a discovery method on the shared spine, not a new adaptive application. Entire bibliographies are never copied.
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
  - Practical guides / hands-on supplements: `references/practical-guides.md`
- Digest template: `references/digest-template.md` (includes Deep adaptations)
- Example directory layout: `references/directory-layout.md`
- Skill maintenance notes: `DEVELOPMENT.md`
- Changelog (package top level, not required at runtime): `CHANGELOG.md`
