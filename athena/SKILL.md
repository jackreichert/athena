---
name: athena
description: Build rigorous source-backed study guides that function as university course equivalents with notes usable by both students and professors. Supports Standard and Deep modes. Digests for primary sources include pre-reading context, post-reading full brief, and standalone summary. Tracks source discovery provenance (syllabi and signals) and compiles full bibliography including notable further-reading sources. Explicit anti-bias and completeness rules. Does not dumb down or dictate interpretation. Also supports academic-level place, city, region, and museum guides — history, must-see sites with scholarly rationale, itineraries — starting from syllabi or highest-quality sources. Trigger on athena, athena research, athena deep, athena go deep, athena deeper, go deep, deeper, graduate study guide, thematic study guide, self-study package, museum guides, place guides, city guides, travel guides, or similar academic requests with syllabi mining and theme synthesis.
---

# Athena (Study Guide Builder)

Create rigorous, source-backed, thematically organized study guides that function as the equivalent of a university course, with notes usable by both students and professors. Prioritize primary sources, structured digests that help the reader *not miss important things* (pre-reading context, post-reading full brief, and standalone summary), thematic synthesis with provenance, clear and dense citations (especially in themes), and navigable learning paths. Digests orient and check; they do not replace the primary encounter or tell the reader what to think.

**Process version:** 1.17 (2026-08-15)

## Guiding Principles

1. Objectives first — define clear learning outcomes and scope before collecting sources.
2. Syllabi as expert signals — university syllabi, essential-readings lists, and (for museums/cultural sites) official institutional highlights, timed itineraries, and collection catalogues are high-value proxies for core material. For Deep mode, preferentially mine graduate seminar syllabi, comprehensive exam lists, and advanced reading lists. **Track and document every syllabus or institutional list consulted** (institution, course, URL/year when available) so source provenance remains transparent; sources that recur across independent high-quality syllabi receive higher weight.
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
- **Syllabi & Discovery Sources Consulted** section: list every syllabus, essential-readings list, institutional highlight/itinerary, or other discovery source used (institution/course title, instructor if known, URL or locator, year). This makes the expert-signal provenance of the bibliography transparent and auditable.
- Ranked Core / Important / Supplementary lists with short rationales (Deep mode: more detailed rationales and expanded Core/Important counts when warranted). Each ranked entry should include a brief provenance note (e.g., “appears on 3 graduate syllabi [list]; foundational monograph cited across the field”).
- Clear identification of primary institutional or canonical sources (official collection pages, standard editions, key monographs).
- A short “Citation practice in this package” note explaining how digests and themes are sourced.
- Availability notes (open access, library, paywall, physical display).
- **Full bibliography compilation:** The ranked lists plus any additional discovered sources form the package’s working bibliography. Maintain and refine it throughout Phase 1 so that by delivery the reader has a transparent, provenance-annotated map of what was found and why items were ranked as they were.
- **Deep mode addition:** Annotated entries (2–4 sentences) for Core and key Important items that include a positioning or evaluative element (how the source intervenes in debates, relative strengths/limitations, relevance to package themes); optional categorization (Primary / Foundational secondary / Recent scholarship / Methodological-theoretical).

### In digests
- Full bibliographic-style entry at the top (author/artist, title, date, medium or edition, inventory/DOI/URL when relevant, location for artworks).
- **Three-part structure for primary sources (especially literary, philosophical, or dialogic works):** (1) **Pre-Reading Context** — orientation before engaging the primary (historical/intellectual stakes, conversation it joins, key terms, practical notes) without heavy interpretation or spoilers; (2) **Summary** — compact standalone overview usable when the reader is not planning to read the source itself but needs it for context; (3) **Full Brief (Post-Reading)** — denser engagement after the reader has encountered the primary, designed to help them notice what they might have missed in the greater conversation (structure, unit-level moves, cross-links, open questions, reception). Do not collapse these into a single reductive summary.
- Claims grounded in the source itself or clearly attributed standard consensus.
- Access notes that point back to the authoritative catalogue or edition.
- **Anti-reductive stance:** Digests help the reader see more and not miss important dimensions; they do not replace the primary encounter or dictate “what to think.” Avoid SparkNotes-style dumbing-down or moralizing interpretation.
- **Deep mode:** Additional critical sections (Methodological / Formal approach; Position in the literature / Reception; Key subsequent engagements or critiques).

### In themes
- **Strong citation emphasis:** Every major claim must be back-linked to a specific digest (or primary source). Themes are the place where provenance is most visible and non-negotiable; dense, explicit citation practice is required.
- Theme Bibliography (Standard: 4–8 key items; Deep: 8–15 items) with short annotations at the end of each theme file.
- **Deep mode:** Explicit “Debates & Contending Interpretations” and/or historiographical / intellectual-genealogy notes within themes. Strongly recommended: open each theme with 2–4 Seminar Guiding Questions that scaffold from reconstruction to critique and application. Annotations in Theme Bibliographies should help position sources relative to debates and to one another.

### In `further-reading.md` (required and substantive)
- Concrete, named entry points (specific books, catalogues, official pages, or well-known surveys) rather than vague “read more about X.”
- **Notable additional sources (primary or secondary)** discovered during research that did not make the Core/Important cut but remain valuable for further reading — flag these explicitly (with short rationale and primary/secondary distinction where helpful). Draw them from the Phase 1 working bibliography and discovery log.
- Organized pathways (official/institutional → core monographs → thematic extensions → addressing gaps).
- Explicit guidance on “how to go deeper.”
- Note major gaps the further reading helps fill.
- **Deep mode:** Structured research pathways including specialization tracks, key journals or databases, and guidance on following citation trails or identifying open research questions. Include a richer set of notable further-reading sources with positioning notes.

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

## Adaptive Applications (Place / Location / Travel & Museum Guides)

Athena supports **place-based guides** at academic depth — cities, regions, historic landscapes, and museums — modeled on the best scholarly and high-cultural practice (Blue Guides’ “understand more fully what one sees,” university “History of [City] / Biography of a City” syllabi, Harvard-style layered city histories, cultural-landscape approaches). These are not tourist-brochure or “top 10 Instagram” lists. They aim for the knowledge a serious traveler or student would want: historical layers, why sites matter in the scholarly conversation, what not to miss and *why*, and a transparent evidence base.

### Shared requirements for all place / location guides
- **Start with syllabi and highest-quality sources.** Preferentially mine university syllabi and reading lists for “History of [Place],” “Art & Architecture of [Place],” urban history, or equivalent courses. When syllabi are thin or unavailable, fall back to the strongest scholarly monographs, architectural histories, official institutional catalogues, and classic cultural guides (e.g., Blue Guide tradition). Log every syllabus or discovery source consulted (as in Phase 1 provenance rules). Compile a full working bibliography with provenance notes.
- Treat major **sites, monuments, neighborhoods, landscapes, and (when relevant) artworks** as primary sources. Digests or site entries emphasize historical context, significance, formal or spatial character, and current condition/location.
- Produce a practical but scholarly **walkthrough / itinerary / “what not to miss”** theme or section grounded in the historical and critical literature, not popularity rankings.
- Include a clear **historical orientation** (layered chronology or key periods) so the reader understands the place as a sequence of transformations, not a static set of attractions.
- Support iterative expansion: a first guide can be high-level; the user can later request deeper treatment of a neighborhood, museum, or theme.
- Hybrid review type is usually optimal.
- Always note that physical conditions, openings, and hangings can change.
- Deep mode adds denser historiography, debates about the place, and specialist literature.

### Museum / collection / exhibition specializations (retained and required when applicable)
- Treat individual **artworks, objects, or spaces** as primary sources. Digests emphasize formal description, iconography/symbolism, historical context, provenance, and current location (room/floor when known).
- **Dual-layer treatment for artworks (required for major and complex works):** (1) Unit-by-unit / zone-by-zone summaries that map the object (including exterior panels, wings, or distinct spatial zones for triptychs and similar formats); (2) a dedicated Period-Specialist Analysis that situates style, technique, iconography, patronage, workshop practice, and meaning in period context and explicitly surfaces symbolism a general viewer is likely to miss, period-specific historical context, significant visual details or objects, and the meaning of colors as understood in that period. Both layers are required for complex works — do not substitute one for the other. In Deep mode, ground the specialist analysis more explicitly in named specialists or standard period literature.
- Prioritize **official museum resources** (collection pages, official highlights/itineraries, floor plans) alongside scholarly consensus lists. Link to official collection pages wherever possible.
- When multiple creators are central, add **`artists-bios.md`** (or `creators-bios.md`) with short parallel biographies.

### Location / city / region / travel guide emphases
- Frame the package as the equivalent of a short university course or serious independent study of the place (history, built environment, cultural layers).
- Core deliverables typically include: historical orientation (periodized or thematic), ranked must-see sites with scholarly rationale (not just fame), practical itineraries that respect historical and spatial logic, and further-reading pathways into deeper literature.
- Site digests or entries should give the reader enough context to stand in front of a building, square, or landscape and understand *why it matters* and what conversations it participates in — without reducing it to a caption.
- Prefer primary evidence and high-quality secondary synthesis for contested local histories; surface competing claims about the place when they exist.
- The guide remains portable and useful both before travel (orientation + planning) and on site (reference + deeper notice).

## Depth Modes

The finished package for either mode is designed to function as the **equivalent of a university course** (or a substantial unit within one): a coherent set of learning outcomes, a ranked and provenance-tracked reading list drawn from real syllabi, structured digests that serve as reading/lecture notes, thematic units that can drive discussion or modules, active questions usable in class or for self-study, and further-reading pathways that extend the course. The materials are written so they can serve **students** (as study notes, reading guides, and self-test scaffolds) **and instructors / professors** (as teaching notes, discussion prompts, seminar design aids, and a ready-made evidence base for the course).

### Standard Mode (default)
The equivalent of a solid upper-level undergraduate course (or a focused, high-quality self-study course at that level). Focused Core list, clear digests that function as student reading notes and instructor lecture-prep notes, thematic synthesis suitable for weekly modules or discussion units, moderate Theme Bibliographies, and a learning path + active questions calibrated for building foundational mastery, classroom discussion, and independent further reading. Suitable both for a student taking or reviewing the course and for a professor preparing or teaching it.

### Deep Mode
The equivalent of a graduate-level course or advanced seminar, with notes dense enough to support both student participation and instructor design of the seminar. Same overall Athena research process and phase structure, executed at higher intensity. The design goal is materials that enable a reader (student or professor) to participate productively in — or to lead — a graduate seminar: accurately reconstruct arguments, identify methods and assumptions, locate sources in debates and intellectual genealogies, critique evidence, and propose extensions or alternative research designs.

Refinements drawn from graduate seminar pedagogy and syllabus analysis (discussion-based formats, scaffolded questions progressing through levels of engagement, annotated bibliographies that position sources, explicit attention to historiography/genealogy of ideas, and structured reading notes/memos):

- **Scope & outcomes:** Learning outcomes emphasize critical evaluation, debate synthesis, methodological awareness, intellectual genealogy, and identification of research frontiers. Assume greater prior knowledge. Explicit goals remain essential even at seminar level; frame them so they work for both student learning and instructor course design.
- **Sources:** Preferentially mine graduate seminar syllabi, PhD reading lists, comprehensive exam bibliographies, annual reviews, field-defining / paradigm-shifting works, and highly-cited or recent articles that map or challenge debates. Aim for a richer ranked bibliography (typically larger Core + Important sets). Produce more detailed selection rationales and annotations that include a positioning or evaluative element (how the source intervenes in conversations, relative strengths/limitations, relevance to package themes).
- **Digests:** Finer grain where productive; mandatory additional critical apparatus (methodology, reception, subsequent engagements). Digests function as seminar-memo / teaching-note equivalents: after reading one, a student or professor should be able to open or lead a discussion of the source’s contribution, methods, and place in ongoing debates.
- **Themes:** Explicit mapping of debates, contending interpretations, and (where relevant) intellectual genealogy or historiography. Longer, research-oriented Gaps & Open Questions. Richer annotated Theme Bibliographies (8–15 items) with positioning annotations. **Strongly recommended:** open each theme file with 2–4 Seminar Guiding Questions that progress from accurate reconstruction of arguments to critique, comparison, and application/research design — usable by students for preparation and by professors as discussion openers or short-response prompts.
- **Further reading & pathways:** More extensive, multi-track research pathways rather than simple “next books.” Can gesture toward exam-list density for key specializations. Include notable additional primary/secondary sources useful for extending the course.
- **Active learning:** Prefer seminar-style discussion questions (usable as openers or short response prompts by either student or instructor), comparative critiques, historiographical notes, and optional short research-design or paper-prompt exercises.
- **Bibliography overall:** Substantially richer and more in-depth across `01-sources.md`, theme files, and `further-reading.md`. Annotations are the norm and should help the reader (student or professor) situate sources relative to one another and to the package’s themes.

Declare the mode explicitly in `00-scope.md` and surface it in the README. Default to Standard unless the user requests deep, graduate, seminar, advanced, or equivalent language. In both modes, write so the package can serve as course notes for the student *and* teaching notes for the professor.

## Workflow

Execute the phases in order, with explicit iteration checkpoints. Write all deliverables as Markdown files in a dedicated, self-contained directory (commonly `artifacts/athena-<topic-slug>/` or `study-guide-<topic-slug>/` — adapt the root path to whatever working or output directory is available in the current environment). Keep the package portable with relative links only.

### Phase 0: Scope Definition
Before any searching:
- Write a concise topic statement.
- Specify target audience / level (and note that the package will serve both student study notes and instructor/professor teaching notes).
- **Declare mode: Standard or Deep** (and briefly justify). Frame the mode as producing the equivalent of a university course (or substantial course unit) at the corresponding level.
- List 3–7 concrete learning outcomes (Deep: higher-order — critique, synthesize debates, apply methods, identify open questions). Write outcomes so they work for student learning goals and for instructor course design.
- Decide depth vs. breadth, time horizon, language constraints, and access preferences.
- **Declare the primary review / guide type** and briefly justify it (Narrative/Conceptual, Thematic, Scoping, Systematic-leaning, or Hybrid).
- Note whether a formal search protocol will be produced.
- For museum, site, city, region, or travel topics, note whether practical navigation (itineraries, must-see lists, bios) will be emphasized and that the guide targets academic-level understanding of the place.
- **If the topic is recent, active, or highly polarized:** Note the polarization risk and that secondary consensus will be treated as contestable rather than baseline.
- **Scope realism:** If declaring Deep mode on a broad topic, either commit to producing complete digests for every Core source or consciously narrow the Core list. An ambitious Core paired with thin or missing digests is worse than a tighter, fully digested Core. Document any narrowing in `01-sources.md` and `limitations.md`.

**Deliverable:** `00-scope.md`

### Phase 1: Source Discovery & Selection
**Goal:** Ranked, justified bibliography of core primary + high-value secondary sources, with transparent provenance of how each source was discovered and a compiled full working bibliography.

**Methods:** Syllabus mining (undergraduate +, for Deep mode, graduate seminar / exam lists and comprehensive exam bibliographies), official institutional lists (especially for museums), canonical signals, citation patterns, high-quality secondary literature. Deep mode additionally draws on review articles, recent monographs, critical editions, and methodological works. For contested or politicized topics, actively seek primary/contemporaneous/forensic sources and sources that challenge the dominant secondary framing.

**Provenance tracking (required):** 
- Maintain a running log of every syllabus, essential-readings list, institutional highlight, catalogue, or other discovery source consulted. Record: institution, course/seminar title (and code if available), instructor if known, URL or stable locator, year or term.
- For each source that enters the candidate pool or final ranked lists, note its discovery provenance (e.g., “appeared on 4 independent graduate syllabi: [A, B, C, D]; also the most-cited monograph in [review article]”; “official collection highlight + recommended in [museum itinerary]”; “identified via citation trail from Core source X”).
- Prefer and up-rank sources that recur across multiple independent high-quality syllabi or institutional lists. Document this recurrence explicitly.
- This log is not optional busywork; it is the evidence that the ranked bibliography rests on expert signals rather than ad-hoc search.

**Bibliography compilation (during the process):** As candidates are found, maintain and grow a full working bibliography (all sources considered worth noting, not only the final ranked set). Explicitly flag **notable additional primary or secondary sources** that are valuable for further reading even if they do not rank as Core or Important — these feed directly into `further-reading.md`. By the end of Phase 1 this becomes the transparent evidence base of the package. The ranked Core / Important / Supplementary lists are a prioritization of that bibliography; the full set (with provenance) remains available for the reader and for further-reading pathways.

**Selection criteria:** Relevance, influence/frequency (especially recurrence across syllabi), quality, representativeness, accessibility, recency or classic status, practical visibility (for physical collections). Deep mode weights debate centrality and scholarly reception more heavily. **For polarized topics:** explicitly address how selection avoids one-sided secondary capture (balance of positions, primary priority for disputed facts, awareness of institutional or platform bias).

**Ranking:** Core / Important / Supplementary. Deep mode typically expands the Core and Important sets and requires richer rationales + annotations. Prefer a Core list that can be fully digested at the required quality over an ambitious list that will be only partially covered. Include short provenance notes on ranked entries.

**Search protocol (adaptive):** Produce `01b-search-protocol.md` when the topic is empirical or reproducibility is requested; otherwise a brief note inside `01-sources.md` is sufficient. Deep mode more often warrants a formal protocol. The protocol (when produced) should also capture the syllabi and discovery sources used.

**Deliverable:** `01-sources.md` (must include: selection criteria; **Syllabi & Discovery Sources Consulted** section; ranked lists with provenance notes and rationales; citation-practice note; availability notes; the compiled full working bibliography or clear pointer to it; and notes on notable further-reading candidates identified during discovery. Deep mode adds annotations and optional categorization).  
**Optional:** `01b-search-protocol.md`

**Iteration checkpoint:** Revisit scope and sources if needed. Confirm that the planned Core list is realistic given the commitment to complete digests. Verify that provenance for the Core set is documented and that the working bibliography is coherent.

### Phase 2: Structured Source Digests
For every Core source (and selected Important sources), produce a consistent digest using the template in `references/digest-template.md`.

**Primary-text structure (especially literary, philosophical, dialogic works such as Plato’s dialogues or Shakespeare):** Every such digest must include the three-part treatment:
1. **Pre-Reading Context** — orientation before the reader engages the primary (historical/intellectual stakes, the conversation it joins or disrupts, key terms or prior works to have lightly in mind, practical notes on edition/length/structure). Lean, non-spoiling, non-dictating.
2. **Summary** — compact standalone overview usable when the reader is *not* planning to read the source itself but needs it for context while working on other texts.
3. **Full Brief (Post-Reading)** — denser engagement after the reader has encountered the primary. Helps them notice structure, unit-level moves, formal or dialectical choices, cross-links, open questions, and what they might have missed in the greater conversation. This is *not* a substitute for reading; it is a check against missing important dimensions.

**Anti-reductive rule:** Digests exist to help the reader see more, not less. Do not dumb down, moralize, or hand the reader “the meaning.” Avoid SparkNotes-style reductive paraphrase. Prefer the source’s own force and precision; locate high-signal quotes; surface tensions and open questions rather than resolving them for the reader.

For artworks/visual objects, adapt: include medium, dimensions, inventory number, room; emphasize formal, iconographic, and spatial description; note that hangings can change. **For major and complex works, provide both Unit/Zone summaries (mapping panels, wings, or zones) and a Period-Specialist Analysis** (period style, technique, iconography, patronage, meaning, plus symbolism a viewer may miss, historical context, key visual details/objects, and period color meanings). Both layers are required for multi-panel or multi-zone works. Pre-Reading Context and Summary still apply in adapted form.

**Deep mode:** Apply the Deep adaptations in the template (Methodological / Formal approach; Position in the literature / Reception; Key subsequent engagements or critiques). Produce denser unit-level coverage where the source warrants it. The goal is that a reader (student or professor) can engage the material at seminar level after reading the primary + Full Brief.

**Digest quality expectations (minimum):**
- Pre-Reading Context present and appropriately lean for primary texts
- Summary usable as standalone reference
- Full Brief with thesis / central project, overall structure, key units or movements with evidence/examples, strengths/limitations or open questions, and preliminary cross-links
- For empirical findings that are contested or revised: brief status note (original claim / later challenges / present standing)
- Deep mode additionally requires the methodological/formal and reception sections

Abstract-only or severely truncated digests are not acceptable in Deep mode. Collapsing the three-part structure into a single reductive summary is a process failure for primary texts.

**Hard completeness gate:** Do **not** begin Phase 3 until every Core source has a complete digest that follows the template (including the three-part structure for primary texts and Deep-mode sections when mode = Deep). If producing full digests for the current Core list is not feasible, reduce the Core list, update `01-sources.md`, and note the change in `limitations.md`. Incomplete Phase 2 is a process failure.

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
- **Provenance & bibliography check:** Confirm `01-sources.md` contains a Syllabi & Discovery Sources Consulted section (or equivalent), that ranked entries carry provenance notes, that a coherent full working bibliography has been compiled from the research process, and that notable additional primary/secondary sources useful for further reading have been identified and fed into `further-reading.md`.
- **Digest structure check (primary texts):** Confirm every primary-source digest includes Pre-Reading Context, standalone Summary, and Full Brief (Post-Reading), and that the writing does not collapse into reductive “what to think” paraphrase.
- For museum packages, verify itineraries are coherent and room data is caveated.
- Confirm mode declaration is consistent across scope, README, and limitations.
- For topics centered on named phenomena (heuristics, fallacies, etc.), confirm an overview/reference theme exists or is explicitly scoped out.
- Record version and date.

## Output Conventions

- Root directory: a dedicated folder such as `athena-<kebab-topic>/` or `study-guide-<kebab-topic>/` (place it under an `artifacts/`, project, or working directory as available in the current environment).
- Core files: `00-scope.md`, `01-sources.md` (must include Syllabi & Discovery Sources Consulted + provenance-annotated ranked lists + working bibliography), `README.md`, `03-themes.md`, `glossary.md`, `limitations.md`, `further-reading.md`
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
- **Citations, provenance, and further research are not optional extras; they are part of the definition of a finished Athena package.** Tracking where sources came from (especially which syllabi and institutional lists) and compiling a full working bibliography during research are required practices. Deep mode makes the bibliography and annotations a central strength.
- **Anti-bias is structural:** On contested or politicized topics, do not let secondary consensus silently become the baseline. Prefer primary evidence for disputed facts, surface corrections and competing claims, and document polarization risk.
- This skill is designed to be portable across agents that support the Agent Skills format (or equivalent system-prompt + knowledge loading). Adapt file-system paths and tool calls to the capabilities of the current runtime.

## Resources

- Digest template: `references/digest-template.md` (includes Deep mode adaptations)
- Example directory layout: `references/directory-layout.md`

## Changelog (selected)

- **1.17 (2026-08-15):** Expanded Adaptive Applications from museum/cultural-site guides to full **place / location / travel guides** at academic depth (cities, regions, historic landscapes). Modeled on Blue Guides, university “History of [City] / Biography of a City” syllabi, layered city histories, and cultural-landscape practice. Location guides start with syllabi when available, otherwise highest-quality scholarly sources; full provenance and bibliography required; historical orientation + must-see sites with scholarly rationale + practical itineraries. Museum specializations retained. Triggers updated to include place/city/travel guides.
- **1.16 (2026-08-15):** Restructured primary-source digests into three explicit parts: **Pre-Reading Context** (orientation before reading, non-spoiling), **Summary** (standalone reference when not reading the source), and **Full Brief (Post-Reading)** (dense check after reading to catch what might be missed in the greater conversation). Explicit anti-reductive / anti-SparkNotes stance: digests help the reader see more and not miss important dimensions; they do not replace the primary encounter or dictate interpretation. Updated digest template, Phase 2, Core Value, and writing rules. Especially useful for sequences such as Plato’s dialogues or Shakespeare.
- **1.15 (2026-08-15):** Reframed both Standard and Deep modes so the finished package functions as the **equivalent of a university course** (undergrad or graduate/seminar), with materials written to serve as notes for both students and professors/instructors. Digests, themes, guiding questions, and further-reading pathways are dual-use (study notes + teaching notes). Updated Depth Modes section, opening description, and frontmatter accordingly.
- **1.14.1 (2026-08-15):** Explicitly require capturing and surfacing **notable additional primary or secondary sources** useful for further reading (even if they fall outside Core/Important). Phase 1 bibliography compilation now flags these; `further-reading.md` must include them with short rationales and primary/secondary distinction where helpful; `01-sources.md` notes the candidates identified during discovery. Strengthens the bridge from research process to concrete next steps.
- **1.14 (2026-08-15):** Strengthened source provenance tracking throughout research. Phase 1 now requires a running log of every syllabus / institutional list consulted and provenance notes on ranked sources; the full working bibliography is compiled during the process rather than as an afterthought. `01-sources.md` must include a Syllabi & Discovery Sources Consulted section and provenance-annotated entries. Updated Guiding Principle 2, Core Value section, Phase 1, Phase 5 QA, Output Conventions, and Constraints. Makes the expert-signal basis of the bibliography transparent and auditable.
- **1.13 (2026-08-14):** Artwork digests now explicitly require **both** layers for major/complex works: (1) Unit-by-unit / zone-by-zone summaries (including exterior panels for triptychs) and (2) Period-Specialist Analysis (missed symbolism, historical context, visual details/objects, period color meanings). Do not choose one in place of the other. Prompted by the need to keep full structural mapping and specialist depth together (e.g. Bosch triptych).
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
