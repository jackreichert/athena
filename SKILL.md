---
name: athena
description: Build rigorous, source-backed, thematically organized study guides for any topic. Trigger on athena, athena research, build a study guide, create a deep reading list and synthesis, make a thematic study guide, produce a self-study package with primary sources and digests, museum or cultural-site guides, or similar requests for structured academic-style learning materials with syllabi mining, chapter digests, and theme synthesis.
---

# Athena (Study Guide Builder)

Create rigorous, source-backed, thematically organized study guides that prioritize primary sources, structured digests, thematic synthesis with provenance, clear citations, and navigable learning paths.

**Process version:** 1.4 (2026-08-13)

## Guiding Principles

1. Objectives first — define clear learning outcomes and scope before collecting sources.
2. Syllabi as expert signals — university syllabi, essential-readings lists, and (for museums/cultural sites) official institutional highlights, timed itineraries, and collection catalogues are high-value proxies for core material.
3. Primary > Secondary, but both matter — prioritize original works (texts, artworks, artifacts); use secondary sources for orientation, context, and debate mapping.
4. Consistent extraction — every core source receives the same structured treatment.
5. Thematic synthesis with provenance — organize by themes/concepts/debates, not by source. Every claim must be back-linkable.
6. **Citations, sources, and further research are fundamental** — every package must make its evidence base transparent and give readers concrete next steps. This is non-negotiable.
7. Active and navigable output — recommended reading/visit order, self-test questions, glossary, modular Markdown, practical itineraries when relevant.
8. Transparency and balance — document selection criteria, note limitations, seek multiple perspectives, surface gaps.
9. Progressive disclosure — support high-level overviews and deep dives.
10. Adaptive rigor — match review type and artifacts (search protocol, matrices, bios, walkthroughs, etc.) to the nature of the topic and learning goals.

## Core Value: Citations, Sources & Further Research (Elevated in 1.4)

Athena packages exist to help users engage primary material *and* know where the claims come from and how to go further. The following are required practices:

### In `01-sources.md`
- Explicit selection criteria.
- Ranked Core / Important / Supplementary lists with short rationales.
- Clear identification of primary institutional or canonical sources (official collection pages, standard editions, key monographs).
- A short “Citation practice in this package” note explaining how digests and themes are sourced.
- Availability notes (open access, library, paywall, physical display).

### In digests
- Full bibliographic-style entry at the top (author/artist, title, date, medium or edition, inventory/DOI/URL when relevant, location for artworks).
- Claims grounded in the source itself or clearly attributed standard consensus.
- Access notes that point back to the authoritative catalogue or edition.

### In themes
- Every major claim back-linked to a digest (or primary source).
- Theme Bibliography (4–8 key items) with short annotations at the end of each theme file.

### In `further-reading.md` (required and substantive)
- Concrete, named entry points (specific books, catalogues, official pages, or well-known surveys) rather than vague “read more about X.”
- Organized pathways (official/institutional → core monographs → thematic extensions → addressing gaps).
- Explicit guidance on “how to go deeper.”
- Note major gaps the further reading helps fill.

### In `limitations.md`
- Methodological notes on how sources were selected and what was *not* done (e.g., no original archival research).
- Clear statement that digests are orientations, not substitutes for the primary works or full scholarly apparatus.

These elements turn the package from a useful summary into a trustworthy research and learning scaffold.

## Adaptive Applications (Museum / Cultural Sites — from 1.3)

When the topic is a **museum, collection, exhibition, historic site, or cultural itinerary**:

- Treat individual **artworks, objects, or spaces** as primary sources. Digests emphasize formal description, iconography/symbolism, historical context, provenance, and current location (room/floor when known).
- Prioritize **official museum resources** (collection pages, official highlights/itineraries, floor plans) alongside scholarly consensus lists. Link to official collection pages wherever possible.
- Produce a practical **walkthrough / timed itinerary** theme or section.
- When multiple creators are central, add **`artists-bios.md`** (or `creators-bios.md`) with short parallel biographies.
- Support iterative expansion based on user focus.
- Hybrid review type is usually optimal.
- Always caveat that room numbers and hangings can change.

## Workflow

Execute the phases in order, with explicit iteration checkpoints. Write all artifacts as Markdown files under a dedicated directory in the working artifacts folder (e.g., `artifacts/athena-<topic-slug>/` or `artifacts/study-guide-<topic-slug>/`). Keep the package self-contained and portable.

### Phase 0: Scope Definition
Before any searching:
- Write a concise topic statement.
- Specify target audience / level.
- List 3–7 concrete learning outcomes.
- Decide depth vs. breadth, time horizon, language constraints, and access preferences.
- **Declare the primary review / guide type** and briefly justify it (Narrative/Conceptual, Thematic, Scoping, Systematic-leaning, or Hybrid).
- Note whether a formal search protocol will be produced.
- For museum/site topics, note whether practical navigation (itineraries, bios) will be emphasized.

**Deliverable:** `00-scope.md`

### Phase 1: Source Discovery & Selection
**Goal:** Ranked, justified bibliography of core primary + high-value secondary sources.

**Methods:** Syllabus mining, official institutional lists (especially for museums), canonical signals, citation patterns, high-quality secondary literature.

**Selection criteria:** Relevance, influence/frequency, quality, representativeness, accessibility, recency or classic status, practical visibility (for physical collections).

**Ranking:** Core / Important / Supplementary.

**Search protocol (adaptive):** Produce `01b-search-protocol.md` when the topic is empirical or reproducibility is requested; otherwise a brief note inside `01-sources.md` is sufficient.

**Deliverable:** `01-sources.md` (must include selection criteria, ranked lists, citation-practice note, and availability notes).  
**Optional:** `01b-search-protocol.md`

**Iteration checkpoint:** Revisit scope and sources if needed.

### Phase 2: Structured Source Digests
For every Core source (and selected Important sources), produce a consistent digest using the template in `references/digest-template.md`.

For artworks/visual objects, adapt: include medium, dimensions, inventory number, room; emphasize formal, iconographic, and spatial description; note that hangings can change.

**Deliverable:** One file per source under `digests/`.

### Phase 3: Thematic Synthesis & Cross-Referencing
Extract themes, build at least one synthesis matrix (strongly recommended; required when ≥4 core sources or substantial disagreement), write theme narratives with Gaps & Open Questions and Theme Bibliography.

For museum/site guides, include a practical Navigating / Walkthrough / Practical Paths theme.

**Deliverable:** `03-themes.md` + `themes/` + `matrix.md` (or embedded).

### Phase 4: Study Guide Assembly
**Required structure:**
- `README.md` — topic, review type, outcomes, how to use, learning path, theme index, quick-start.
- Theme files with synthesis, backlinks, active learning, Gaps & Open Questions, Theme Bibliography.
- `01-sources.md` with clear citation practice.
- **`further-reading.md`** — substantive, concrete, pathway-oriented (this is a core value, not an afterthought).
- `glossary.md`, `limitations.md` (including methodological/sourcing notes).
- **When multiple creators are central:** `artists-bios.md` or equivalent.

**Format:** Linked Markdown, portable.

### Phase 5: Quality Assurance
- Spot-check digests for fidelity and correct bibliographic data.
- Verify backlinks.
- Confirm Gaps & Open Questions are substantive.
- Confirm `further-reading.md` offers concrete next steps and `01-sources.md` makes the evidence base transparent.
- For museum packages, verify itineraries are coherent and room data is caveated.
- Record version and date.

## Output Conventions

- Root: `artifacts/athena-<kebab-topic>/` or `artifacts/study-guide-<kebab-topic>/`
- Core files: `00-scope.md`, `01-sources.md`, `README.md`, `03-themes.md`, `glossary.md`, `limitations.md`, `further-reading.md`
- Recommended for multi-creator / museum topics: `artists-bios.md`
- Optional: `01b-search-protocol.md`, `matrix.md`
- Subdirs: `digests/`, `themes/`
- Relative links only.
- Offer a downloadable zip at the end.

## Constraints & Notes

- Do not invent sources or fabricate quotes, page numbers, inventory numbers, or room locations.
- Favor open-access and official institutional resources when quality is comparable.
- Keep digests dense but readable.
- Match search-protocol and matrix depth to the topic.
- For physical collections, always note that display locations can change.
- **Citations and further research are not optional extras; they are part of the definition of a finished Athena package.**

## Resources

- Digest template: `references/digest-template.md`
- Example directory layout: `references/directory-layout.md`

## Changelog (selected)

- **1.4 (2026-08-13):** Elevated citations, transparent sourcing, and substantive further-reading to core guiding principles and required package elements. Explicit “Citation practice” expectations for `01-sources.md`, digests, themes, and `further-reading.md`. Methodological notes required in `limitations.md`. This responds directly to the need for guides that are not only useful but also research-scaffolding.
- **1.3 (2026-08-13):** Adaptive guidance for museum / cultural-site guides (artworks as primary sources, official itineraries, artist bios, walkthrough themes, iterative expansion).
- **1.2 (2026-08-12):** Prior baseline.
