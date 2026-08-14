---
name: athena
description: Build rigorous, source-backed, thematically organized study guides for any topic. Supports Standard mode (excellent undergraduate overview) and Deep mode (graduate-level course/seminar notes equivalent that enable productive seminar participation) with denser engagement, positioning annotations, Seminar Guiding Questions, and richer bibliography. Strong emphasis on citations and provenance, especially in themes. Includes explicit anti-bias practices for contested and politicized domains (treat consensus as contestable, prioritize primary evidence for disputed facts, surface corrections and competing claims). Enforces completeness: every Core source must receive a full digest before themes; incomplete Phase 2 is a process failure. Trigger on athena, athena research, athena deep, athena go deep, athena deeper, go deep, deeper, graduate study guide, deep reading list and synthesis, thematic study guide, self-study package, museum or cultural-site guides, or similar requests for structured academic-style learning materials with syllabi mining, chapter digests, and theme synthesis.
---

# Athena (Study Guide Builder)

Create rigorous, source-backed, thematically organized study guides that prioritize primary sources, structured digests, thematic synthesis with provenance, clear and dense citations (especially in themes), and navigable learning paths.

**Process version:** 1.12.1 (2026-08-14)

## Guiding Principles

1. Objectives first — define clear learning outcomes and scope before collecting sources.
2. Syllabi as expert signals — university syllabi, essential-readings lists, and (for museums/cultural sites) official institutional highlights, timed itineraries, and collection catalogues are high-value proxies for core material. For Deep mode, preferentially mine graduate seminar syllabi, comprehensive exam lists, and advanced reading lists.
3. Primary > Secondary, but both matter — prioritize original works (texts, artworks, artifacts); use secondary sources for orientation, context, and debate mapping. Deep mode engages a wider secondary literature including key articles, critical reception, and methodological works. For contested factual claims (especially recent or politicized events), prefer primary, contemporaneous, forensic, or official investigative sources over narrative secondary synthesis.
4. Consistent extraction — every core source receives the same structured treatment.
5. Thematic synthesis with provenance — organize by themes/concepts/debates, not by source. Every major claim must be back-linkable to a specific digest or primary source. Citations and provenance are especially rigorous when building out themes.
6. **Citations, sources, and further research are fundamental** — every package must make its evidence base transparent and give readers concrete next steps. This is non-negotiable. Themes in particular must demonstrate dense, explicit citation practice. Deep mode produces a richer, more in-depth, annotated bibliography throughout.
7. Active and navigable output — recommended reading/visit order, self-test questions, glossary, modular Markdown, practical itineraries when relevant. Deep mode includes higher-order seminar-style prompts and research pathways.
8. Transparency and balance — document selection criteria, note limitations, seek multiple perspectives, surface gaps.
9. Progressive disclosure — support high-level overviews and deep dives.
10. Adaptive rigor — match review type and artifacts (search protocol, matrices, bios, walkthroughs, etc.) to the nature of the topic and learning goals.
11. **Depth modes** — Standard produces an excellent undergraduate-level overview. Deep produces the equivalent of notes from a graduate-level course or seminar: denser source engagement, finer-grained digests, explicit debate and historiographical mapping, and a substantially richer annotated bibliography.
12. **Anti-bias & contested domains** — Treat dominant secondary “consensus” as a claim to be examined, not an unstated baseline, especially on recent, politicized, or rapidly evolving topics. Prefer primary and contemporaneous evidence for disputed facts; note recantations and corrections; treat Wikipedia and similar secondary platforms as sources that can themselves be biased or lag reality; surface competing interpretations with their evidence bases; and document polarization risk in selection criteria and limitations.

## Core Value: Citations, Sources & Further Research

Athena packages exist to help users engage primary material *and* know where the claims come from and how to go further. The following are required practices:

### In `01-sources.md`
- Explicit selection criteria.
- Ranked Core / Important / Supplementary lists with short rationales (Deep mode: more detailed rationales and expanded Core/Important counts when warranted).
- Clear identification of primary institutional or canonical sources (official collection pages, standard editions, key monographs).
- A short “Citation practice in this package” note explaining how digests and themes are sourced.
- Availability notes (open access, library, paywall, physical display).
- **Deep mode addition:** Annotated entries (2–4 sentences) for Core and key Important items that include a positioning or evaluative element (how the source intervenes in debates, relative strengths/limitations, relevance to package themes); optional categorization (Primary / Foundational secondary / Recent scholarship / Methodological-theoretical).

### In digests
- Full bibliographic-style entry at the top (author/artist, title, date, medium or edition, inventory/DOI/URL when relevant, location for artworks).
- Claims grounded in the source itself or clearly attributed standard consensus.
- Access notes that point back to the authoritative catalogue or edition.
- **Deep mode:** Additional critical sections (Methodological approach; Position in the literature / Reception; Key subsequent engagements or critiques).

### In themes
- **Strong citation emphasis:** Every major claim must be back-linked to a specific digest (or primary source). Themes are the place where provenance is most visible and non-negotiable; dense, explicit citation practice is required.
- Theme Bibliography (Standard: 4–8 key items; Deep: 8–15 items) with short annotations at the end of each theme file.
- **Deep mode:** Explicit “Debates & Contending Interpretations” and/or historiographical / intellectual-genealogy notes within themes. Strongly recommended: open each theme with 2–4 Seminar Guiding Questions that scaffold from reconstruction to critique and application. Annotations in Theme Bibliographies should help position sources relative to debates and to one another.

### In `further-reading.md` (required and substantive)
- Concrete, named entry points (specific books, catalogues, official pages, or well-known surveys) rather than vague “read more about X.”
- Organized pathways (official/institutional → core monographs → thematic extensions → addressing gaps).
- Explicit guidance on “how to go deeper.”
- Note major gaps the further reading helps fill.
- **Deep mode:** Structured research pathways including specialization tracks, key journals or databases, and guidance on following citation trails or identifying open research questions.

### In `limitations.md`
- Methodological notes on how sources were selected and what was *not* done (e.g., no original archival research).
- Clear statement that digests are orientations, not substitutes for the primary works or full scholarly apparatus.
- Note the mode (Standard or Deep) and any resulting scope limits.
- **For active, recent, or highly polarized topics:** Explicitly note that secondary consensus can lag, resist correction, or reflect coordinated narrative pressure; treat early framings as provisional; and encourage checking primary/updated evidence.

### Anti-bias practices for contested or politicized domains
When the topic involves recent events, active conflicts, highly polarized public debates, or claims that have shifted significantly after initial reporting:
- Treat the dominant secondary framing as a *claim to be examined*, not the default reality.
- Prioritize primary sources, contemporaneous accounts, official investigations, forensic/OSINT work, and later corrections or recantations over narrative secondary synthesis for disputed factual claims.
- In themes (and when warranted in 01-sources or limitations), include a **Contested Claims & Corrections** subsection listing major claims that have been significantly revised, recanted, or remain sharply disputed, with evidence links.
- In Deep mode, include brief genealogy of charged framings themselves (when/how they entered mainstream secondary literature, key promoters, evidence cited at the time vs later).
- Treat Wikipedia and similar platforms as secondary sources that can be subject to coordinated editing or source-selection bias; cross-check contested claims against primary material and alternative high-quality sources. Note this in selection criteria or limitations when relevant.
- Selection criteria in `01-sources.md` should address polarization risk (how the package avoids one-sided secondary capture).

These elements turn the package from a useful summary into a trustworthy research and learning scaffold.

## Adaptive Applications (Museum / Cultural Sites)

When the topic is a **museum, collection, exhibition, historic site, or cultural itinerary**:

- Treat individual **artworks, objects, or spaces** as primary sources. Digests emphasize formal description, iconography/symbolism, historical context, provenance, and current location (room/floor when known).
- **Period-specialist analysis (required for major paintings and key works):** Include a dedicated section that analyzes the work as an art historian specializing in its period would — situating style, technique, iconography, patronage, workshop practice, and meaning within the artistic and cultural conventions of that time (e.g., Spanish Golden Age for Velázquez, early-19th-century Spanish contexts for Goya). Explicitly surface symbolism a general viewer is likely to miss, period-specific historical context, significant visual details or objects, and the meaning of colors as understood in that period. This goes beyond general formal description and later reception; it synthesizes or emulates period-focused scholarly interpretation. In Deep mode, draw more explicitly on named specialists or standard period literature.
- Prioritize **official museum resources** (collection pages, official highlights/itineraries, floor plans) alongside scholarly consensus lists. Link to official collection pages wherever possible.
- Produce a practical **walkthrough / timed itinerary** theme or section.
- When multiple creators are central, add **`artists-bios.md`** (or `creators-bios.md`) with short parallel biographies.
- Support iterative expansion based on user focus.
- Hybrid review type is usually optimal.
- Always caveat that room numbers and hangings can change.
- Deep mode remains available and adds denser scholarly literature on the works, artists, collecting history, and period-specialist debates.

## Depth Modes

### Standard Mode (default)
Excellent undergraduate overview. Focused Core list, clear digests, thematic synthesis suitable for a solid upper-level undergrad course or serious self-study. Theme bibliographies of moderate length. Learning path and active questions calibrated for building foundational mastery and independent further reading.

### Deep Mode
Graduate-level course / seminar notes equivalent. Same overall Athena research process and phase structure, executed at higher intensity. The design goal is materials that enable a reader to participate productively in a graduate seminar discussion (or to design one): accurately reconstruct arguments, identify methods and assumptions, locate sources in debates and intellectual genealogies, critique evidence, and propose extensions or alternative research designs.

Refinements drawn from graduate seminar pedagogy and syllabus analysis (discussion-based formats, scaffolded questions progressing through levels of engagement, annotated bibliographies that position sources, explicit attention to historiography/genealogy of ideas, and structured reading notes/memos):

- **Scope & outcomes:** Learning outcomes emphasize critical evaluation, debate synthesis, methodological awareness, intellectual genealogy, and identification of research frontiers. Assume greater prior knowledge. Explicit goals remain essential even at seminar level.
- **Sources:** Preferentially mine graduate seminar syllabi, PhD reading lists, comprehensive exam bibliographies, annual reviews, field-defining / paradigm-shifting works, and highly-cited or recent articles that map or challenge debates. Aim for a richer ranked bibliography (typically larger Core + Important sets). Produce more detailed selection rationales and annotations that include a positioning or evaluative element (how the source intervenes in conversations, relative strengths/limitations, relevance to package themes).
- **Digests:** Finer grain where productive; mandatory additional critical apparatus (methodology, reception, subsequent engagements). Digests function as seminar-memo equivalents: after reading one, a user should be able to open a discussion of the source’s contribution, methods, and place in ongoing debates.
- **Themes:** Explicit mapping of debates, contending interpretations, and (where relevant) intellectual genealogy or historiography. Longer, research-oriented Gaps & Open Questions. Richer annotated Theme Bibliographies (8–15 items) with positioning annotations. **Strongly recommended:** open each theme file with 2–4 Seminar Guiding Questions that progress from accurate reconstruction of arguments to critique, comparison, and application/research design.
- **Further reading & pathways:** More extensive, multi-track research pathways rather than simple “next books.” Can gesture toward exam-list density for key specializations.
- **Active learning:** Prefer seminar-style discussion questions (usable as openers or short response prompts), comparative critiques, historiographical notes, and optional short research-design or paper-prompt exercises.
- **Bibliography overall:** Substantially richer and more in-depth across `01-sources.md`, theme files, and `further-reading.md`. Annotations are the norm and should help the reader situate sources relative to one another and to the package’s themes.

Declare the mode explicitly in `00-scope.md` and surface it in the README. Default to Standard unless the user requests deep, graduate, seminar, advanced, or equivalent language.

## Workflow

Execute the phases in order, with explicit iteration checkpoints. Write all deliverables as Markdown files in a dedicated, self-contained directory (commonly `artifacts/athena-<topic-slug>/` or `study-guide-<topic-slug>/` — adapt the root path to whatever working or output directory is available in the current environment). Keep the package portable with relative links only.

### Phase 0: Scope Definition
Before any searching:
- Write a concise topic statement.
- Specify target audience / level.
- **Declare mode: Standard or Deep** (and briefly justify).
- List 3–7 concrete learning outcomes (Deep: higher-order — critique, synthesize debates, apply methods, identify open questions).
- Decide depth vs. breadth, time horizon, language constraints, and access preferences.
- **Declare the primary review / guide type** and briefly justify it (Narrative/Conceptual, Thematic, Scoping, Systematic-leaning, or Hybrid).
- Note whether a formal search protocol will be produced.
- For museum/site topics, note whether practical navigation (itineraries, bios) will be emphasized.
- **If the topic is recent, active, or highly polarized:** Note the polarization risk and that secondary consensus will be treated as contestable rather than baseline.
- **Scope realism:** If declaring Deep mode on a broad topic, either commit to producing complete digests for every Core source or consciously narrow the Core list. An ambitious Core paired with thin or missing digests is worse than a tighter, fully digested Core. Document any narrowing in `01-sources.md` and `limitations.md`.

**Deliverable:** `00-scope.md`

### Phase 1: Source Discovery & Selection
**Goal:** Ranked, justified bibliography of core primary + high-value secondary sources.

**Methods:** Syllabus mining (undergraduate +, for Deep mode, graduate seminar / exam lists), official institutional lists (especially for museums), canonical signals, citation patterns, high-quality secondary literature. Deep mode additionally draws on review articles, recent monographs, critical editions, and methodological works. For contested or politicized topics, actively seek primary/contemporaneous/forensic sources and sources that challenge the dominant secondary framing.

**Selection criteria:** Relevance, influence/frequency, quality, representativeness, accessibility, recency or classic status, practical visibility (for physical collections). Deep mode weights debate centrality and scholarly reception more heavily. **For polarized topics:** explicitly address how selection avoids one-sided secondary capture (balance of positions, primary priority for disputed facts, awareness of institutional or platform bias).

**Ranking:** Core / Important / Supplementary. Deep mode typically expands the Core and Important sets and requires richer rationales + annotations. Prefer a Core list that can be fully digested at the required quality over an ambitious list that will be only partially covered.

**Search protocol (adaptive):** Produce `01b-search-protocol.md` when the topic is empirical or reproducibility is requested; otherwise a brief note inside `01-sources.md` is sufficient. Deep mode more often warrants a formal protocol.

**Deliverable:** `01-sources.md` (must include selection criteria, ranked lists, citation-practice note, and availability notes; Deep mode adds annotations and optional categorization).  
**Optional:** `01b-search-protocol.md`

**Iteration checkpoint:** Revisit scope and sources if needed. Confirm that the planned Core list is realistic given the commitment to complete digests.

### Phase 2: Structured Source Digests
For every Core source (and selected Important sources), produce a consistent digest using the template in `references/digest-template.md`.

For artworks/visual objects, adapt: include medium, dimensions, inventory number, room; emphasize formal, iconographic, and spatial description; note that hangings can change. **For major paintings and key works, include a Period-Specialist Analysis section** (analysis as by an art historian specializing in the work’s period — style, technique, iconography, patronage, meaning in period context, plus symbolism a viewer may miss, historical context, key visual details/objects, and period color meanings).

**Deep mode:** Apply the Deep adaptations in the template (Methodological approach; Position in the literature / Reception; Key subsequent engagements or critiques). Produce denser unit-level coverage where the source warrants it. The goal is that a reader can engage the material at seminar level.

**Digest quality expectations (minimum):**
- Thesis / central project and overall structure
- Key units or arguments with evidence/examples
- Strengths and limitations (or critiques from the literature)
- For empirical findings that are contested or revised: brief status note (original claim / later challenges / present standing)
- Preliminary cross-links
- Deep mode additionally requires the methodological and reception sections

Abstract-only or severely truncated digests are not acceptable in Deep mode.

**Hard completeness gate:** Do **not** begin Phase 3 until every Core source has a complete digest that follows the template (including Deep-mode sections when mode = Deep). If producing full digests for the current Core list is not feasible, reduce the Core list, update `01-sources.md`, and note the change in `limitations.md`. Incomplete Phase 2 is a process failure.

**Deliverable:** One file per Core source under `digests/`.

### Phase 3: Thematic Synthesis & Cross-Referencing
Extract themes, build at least one synthesis matrix (strongly recommended; required when ≥4 core sources or substantial disagreement; Deep mode almost always produces a detailed matrix), write theme narratives with Gaps & Open Questions and Theme Bibliography.

**Citation practice is especially rigorous here:** every major claim in a theme narrative must be back-linked to a specific digest or primary source. Themes are the primary site where provenance and evidence transparency are demonstrated.

For museum/site guides, include a practical Navigating / Walkthrough / Practical Paths theme.

**Topic-sensitive artifacts:** When the topic’s core objects are named lists of phenomena (heuristics, fallacies, biases, cognitive effects, argument schemes, etc.), strongly recommend an overview/reference theme that maps the main items with primary sources and canonical examples. This is often the most practically useful theme for readers.

**Deep mode enhancements:**
- Include explicit “Debates & Contending Interpretations” (or equivalent) and, where the topic warrants, intellectual genealogy / historiography subsections (including genealogy of charged framings themselves when relevant).
- Strongly recommend opening each theme file with 2–4 Seminar Guiding Questions that progress from accurate reconstruction of key arguments to critique, comparison across sources, and application or research-design prompts.
- Make Gaps & Open Questions research-oriented (unresolved issues, methodological frontiers, opportunities for original work).
- Theme Bibliographies: 8–15 annotated items with positioning/evaluative elements, distinguishing source types where useful.
- Longer, more analytically dense theme narratives oriented toward enabling seminar-level discussion, with dense explicit citations.
- **For contested/politicized topics (Standard or Deep):** Strongly recommend a **Contested Claims & Corrections** subsection listing major claims that have been significantly revised, recanted, or remain sharply disputed, with back-links to evidence.

**Deliverable:** `03-themes.md` + `themes/` + `matrix.md` (or embedded).

### Phase 4: Study Guide Assembly
**Required structure:**
- `README.md` — topic, mode, review type, outcomes, how to use, learning path, theme index, quick-start.
- Theme files with synthesis, backlinks, active learning, Gaps & Open Questions, Theme Bibliography.
- `01-sources.md` with clear citation practice (and Deep-mode annotations).
- **`further-reading.md`** — substantive, concrete, pathway-oriented (this is a core value, not an afterthought). Deep mode: multi-track research pathways.
- `glossary.md`, `limitations.md` (including methodological/sourcing notes and mode).
- **When multiple creators are central:** `artists-bios.md` or equivalent.

**Format:** Linked Markdown, portable.

**Deep mode active learning:** Prefer seminar-style discussion questions (usable as openers or short response-paper prompts), comparative critiques, historiographical notes, and optional short research-design or paper-prompt exercises over basic recall questions. Questions should help the user practice the discursive moves expected in a graduate seminar.

### Phase 5: Quality Assurance
- **Completeness check:** Confirm every Core source has a digest file and that each digest meets the quality expectations above (not abstract-only). If any are missing or thin, return to Phase 2 or narrow Core.
- Spot-check digests for fidelity and correct bibliographic data.
- Verify backlinks.
- Confirm Gaps & Open Questions are substantive (and research-oriented in Deep mode).
- Confirm `further-reading.md` offers concrete next steps and `01-sources.md` makes the evidence base transparent (and richly annotated in Deep mode).
- For museum packages, verify itineraries are coherent and room data is caveated.
- Confirm mode declaration is consistent across scope, README, and limitations.
- For topics centered on named phenomena (heuristics, fallacies, etc.), confirm an overview/reference theme exists or is explicitly scoped out.
- Record version and date.

## Output Conventions

- Root directory: a dedicated folder such as `athena-<kebab-topic>/` or `study-guide-<kebab-topic>/` (place it under an `artifacts/`, project, or working directory as available in the current environment).
- Core files: `00-scope.md`, `01-sources.md`, `README.md`, `03-themes.md`, `glossary.md`, `limitations.md`, `further-reading.md`
- Recommended for multi-creator / museum topics: `artists-bios.md`
- Optional: `01b-search-protocol.md`, `matrix.md`
- Subdirs: `digests/`, `themes/`
- Relative links only.
- At the end, offer a downloadable zip of the finished package when the environment supports it.
- Deep mode packages should feel recognizably denser in bibliography, critical apparatus, and research orientation while remaining navigable.

## Constraints & Notes

- Do not invent sources or fabricate quotes, page numbers, inventory numbers, or room locations.
- Favor open-access and official institutional resources when quality is comparable.
- Keep digests dense but readable; Deep mode digests may be longer but must remain structured and usable. Abstract-only digests are not acceptable in Deep mode.
- **Completeness over ambition:** Every Core source must receive a complete digest before themes are written. If this cannot be done, reduce Core and document the change. Incomplete Phase 2 is a process failure.
- Match search-protocol and matrix depth to the topic and mode.
- For physical collections, always note that display locations can change.
- **Citations and further research are not optional extras; they are part of the definition of a finished Athena package.** Deep mode makes the bibliography and annotations a central strength.
- **Anti-bias is structural:** On contested or politicized topics, do not let secondary consensus silently become the baseline. Prefer primary evidence for disputed facts, surface corrections and competing claims, and document polarization risk.
- This skill is designed to be portable across agents that support the Agent Skills format (or equivalent system-prompt + knowledge loading). Adapt file-system paths and tool calls to the capabilities of the current runtime.

## Resources

- Digest template: `references/digest-template.md` (includes Deep mode adaptations)
- Example directory layout: `references/directory-layout.md`

## Changelog (selected)

- **1.12.1 (2026-08-14):** Sharpened Period-Specialist Analysis to explicitly require: symbolism a general viewer is likely to miss; period-specific historical context; significant visual details/objects and their meaning; and colors with their period associations/meanings.
- **1.12 (2026-08-14):** For museum/artwork digests, added required **Period-Specialist Analysis** section for major paintings and key works: analysis as by an art historian specializing in the work’s period (style, technique, iconography, patronage, meaning in period context). Distinct from formal description and later reception. Updated Adaptive Applications (Museum), Phase 2, and digest template. Prompted by feedback on the Prado package.
- **1.11 (2026-08-14):** Hardened process against incomplete execution. Added hard completeness gate: do not begin Phase 3 until every Core source has a complete digest; if infeasible, reduce Core and document. Added digest quality minimums (reject abstract-only in Deep mode). Added scope-realism notes in Phase 0/1. Added topic-sensitive artifact prompt for named-phenomena topics (heuristics, fallacies, etc.). Strengthened Phase 5 completeness check. Response to under-execution observed on the bias & critical thinking package.
- **1.10 (2026-08-14):** After running a full Deep-mode package on “bias and critical thinking,” refined the digest template to encourage explicit status notes (original claim / later challenges / present standing) for contested empirical findings. This makes Contested Claims & Corrections subsections easier to populate accurately and tightens the link between digests and anti-bias theme practices. Minor self-application stress test of the v1.9 anti-bias rules.
- **1.9 (2026-08-14):** Added explicit anti-bias practices for contested and politicized domains. New Guiding Principle 12. Treat dominant secondary “consensus” as a claim to be examined; prioritize primary/contemporaneous/forensic evidence for disputed facts; require or strongly recommend Contested Claims & Corrections subsections; note Wikipedia and platform bias risk; strengthen selection criteria and limitations language for polarized topics; add claim-genealogy guidance in Deep mode. Updated phases 0, 1, 3, Core Value, constraints, and description.
- **1.8 (2026-08-14):** Expanded triggers to include “athena go deep”, “athena deeper”, “go deep”, “deeper”. Strengthened emphasis on citations and provenance, especially in themes: every major claim must be back-linked; themes are the primary site of dense, explicit citation practice. Updated principles, Core Value, and Phase 3 accordingly.
- **1.7 (2026-08-14):** Refined Deep mode after research into graduate seminar design and pedagogy (syllabus structures, discussion formats, annotated bibliography practices, scaffolded questions, historiography/genealogy emphasis, and student note-taking expectations). Clarified the design goal as enabling productive seminar participation. Added strong recommendation for Seminar Guiding Questions in themes; required positioning/evaluative elements in Deep annotations; strengthened language around intellectual genealogy, seminar-memo function of digests, and discursive moves in active learning. Process version bumped; principles and phase instructions updated for consistency.
- **1.6 (2026-08-14):** Introduced explicit Standard vs Deep depth modes. Deep mode delivers graduate-level course/seminar-equivalent notes using the same research process: expanded source mining (grad syllabi, key articles, reception literature), denser digests with critical apparatus, debate/historiographical mapping in themes, richer annotated bibliographies throughout, and research-oriented further-reading pathways. Updated description, principles, all phases, and core-value sections accordingly. Default remains Standard (excellent undergrad overview).
- **1.5 (2026-08-13):** Portability improvements for cross-agent use. Softened hard-coded output paths; added explicit environment-adaptation note. Skill remains fully effective in Grok while being easier to install in Claude Skills, Custom GPTs (via instructions + knowledge), and other Agent Skills–compatible runtimes. Ready for “install this repo” workflows.
- **1.4 (2026-08-13):** Elevated citations, transparent sourcing, and substantive further-reading to core guiding principles and required package elements.
- **1.3 (2026-08-13):** Adaptive guidance for museum / cultural-site guides (artworks as primary sources, official itineraries, artist bios, walkthrough themes, iterative expansion).
- **1.2 (2026-08-12):** Prior baseline.
