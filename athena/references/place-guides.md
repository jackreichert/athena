# Place / Location / Travel & Museum Guides (Athena Adaptive Application)

## Adaptive Applications (Place / Location / Travel & Museum Guides)

Athena supports **place-based guides** at academic depth — cities, regions, historic landscapes, and museums — modeled on the best scholarly and high-cultural practice (Blue Guides’ “understand more fully what one sees,” university “History of [City] / Biography of a City” syllabi, Harvard-style layered city histories, cultural-landscape approaches). These are not tourist-brochure or “top 10 Instagram” lists. They aim for the knowledge a serious traveler or student would want: historical layers, why sites matter in the scholarly conversation, what not to miss and *why*, and a transparent evidence base.

### Shared requirements for all place / location guides
- **Start with syllabi and highest-quality sources.** Preferentially mine university syllabi and reading lists for “History of [Place],” “Art & Architecture of [Place],” urban history, or equivalent courses. When syllabi are thin or unavailable, fall back to the strongest scholarly monographs, architectural histories, official institutional catalogues, and classic cultural guides (e.g., Blue Guide tradition). Log every syllabus or discovery source consulted (as in Phase 1 provenance rules). Compile a full working bibliography with provenance notes.
- Treat major **sites, monuments, neighborhoods, landscapes, and (when relevant) artworks** as primary sources. Digests or site entries emphasize historical context, significance, formal or spatial character, and current condition/location.
- Produce a practical but scholarly **walkthrough / itinerary / “what not to miss”** theme or section grounded in the historical and critical literature, not popularity rankings.
- **Historical overview / orientation:**
  - **Required** for city, region, location, and travel guides: include a clear historical overview (layered chronology or key periods) so the reader understands the place as a sequence of transformations, not a static set of attractions.
  - **For museum / collection guides:** required when the museum itself is historically important (as a building, institution with significant history, founding context, or site of historical events); otherwise optional. In the optional case the focus may remain on collections, artworks, and institutional highlights without a full place-history section.
- **Images when they enhance understanding:** Include maps, site plans, exterior/interior photographs, or key artworks when visual reference materially helps the reader. Prefer official or public-domain sources; store under `images/` with relative links and captions that credit the source. Especially valuable for complex sites, floor plans, and works discussed in digests.
- Support iterative expansion: a first guide can be high-level; the user can later request deeper treatment of a neighborhood, museum, or theme.
- Hybrid review type is usually optimal.
- Always note that physical conditions, openings, and hangings can change.
- Deep mode adds denser historiography, debates about the place, and specialist literature.

### Museum / collection / exhibition specializations (retained and required when applicable)
- Treat individual **artworks, objects, or spaces** as primary sources. Digests emphasize formal description, iconography/symbolism, historical context, provenance, and current location (room/floor when known).
- **Dual-layer treatment for artworks (required for major and complex works):** (1) Unit-by-unit / zone-by-zone summaries that map the object (including exterior panels, wings, or distinct spatial zones for triptychs and similar formats); (2) a dedicated Period-Specialist Analysis that situates style, technique, iconography, patronage, workshop practice, and meaning in period context and explicitly surfaces symbolism a general viewer is likely to miss, period-specific historical context, significant visual details or objects, and the meaning of colors as understood in that period. Both layers are required for complex works — do not substitute one for the other. In Deep mode, ground the specialist analysis more explicitly in named specialists or standard period literature.
- **Images (required when they enhance understanding):** For major artworks and key visual objects, include at least one high-quality reference image in the digest (and additional detail images when useful for panels, zones, or iconographic points). Prefer official museum collection images or public-domain high-resolution sources. Place the primary image near the top of the digest (after the bibliographic entry). Always caption with credit, inventory number when known, and a link to the official collection page. Store images under an `images/` subdirectory with relative Markdown links so the package remains portable. Note that physical hangings and lighting can change; the image is a study reference, not a substitute for seeing the work.
- Prioritize **official museum resources** (collection pages, official highlights/itineraries, floor plans) alongside scholarly consensus lists. Link to official collection pages wherever possible.
- **Do not artificially cap the number of digests.** For museum and collection guides, prioritize the works a careful visitor would most regret missing, grounded in institutional highlights, official “must-see” lists, and scholarly consensus. Expand beyond an initial Core list when additional major works (e.g., key Rembrandts, Caravaggios, Rubens, Titians) are clearly part of the collection’s essential holdings. Document the expanded selection in `01-sources.md` and `limitations.md`.
- When multiple creators are central, add **`artists-bios.md`** (or `creators-bios.md`) with short parallel biographies.
- When the museum itself is historically important, the historical overview of the institution/building is required (see shared rule above).

### Optional Step 2: Visitor-Oriented EPUB (Museum / Collection Guides)

After the Standard (or Deep) Markdown package is complete and audited, the user may request a second deliverable: a polished, sequential, visitor-friendly EPUB that restructures the same content for use before and during a visit. This is an optional enhancement, not a replacement for the Markdown package. Both versions are delivered.

**Process distilled from the Kunsthistorisches Museum guide (2026):**

1. **Preserve the Athena package** — The Markdown zip remains the scholarly base (scope, ranked sources with provenance, full dual-layer digests, themes, artists-bios, glossary, further-reading, limitations).

2. **Restructure into a linear walk-through** — Convert digests and themes into sequential chapters that follow a practical route through the building or site:
   - How to Use + suggested routes (short highlights / half-day / full day) up front.
   - Arrival and building (when historically important).
   - Collecting or institutional history.
   - Room-by-room or highlight-by-highlight chapters with the full dual-layer treatment for every Core and Important artwork.
   - Condensed briefs for any additional referenced works.
   - Themes chapter (full synthesis with “Across the Sources: What Is Easy to Miss”).
   - Reference chapters at the end: Artists and Creators, Glossary, Bibliography and Further Reading, Limitations and Practical Notes.
   - Explicit Table of Contents page with internal links.

3. **Embed images** — Locate high-quality public-domain or official images of key works and interiors. Embed them with captions in the relevant chapters. Note that images are study references.

4. **Design for the visitor** — Elegant, restrained typography (serif, generous leading, warm off-white ground, deep navy headings, subtle gold rules). Include a refined cover (navy and gold architectural linework works well for major museum buildings). Keep watch-fors and “what is easy to miss” lists with each work for on-site looking.

5. **Deliver both** — Offer the Markdown zip (Step 1) and the finished EPUB (Step 2). The EPUB restructures and presents the same analytical content; it does not replace or dumb down the dual-layer briefs.

This Step 2 process is especially suited to major museum collections where the user wants both a research package and a polished, portable guide for an actual visit. It is invoked when the user asks for an ebook, walk-through guide, visitor edition, or similar after (or alongside) the Athena package.

### Location / city / region / travel guide emphases
- Frame the package as the equivalent of a short university course or serious independent study of the place (history, built environment, cultural layers).
- **Historical overview is required.** Core deliverables include: historical orientation (periodized or thematic), ranked must-see sites with scholarly rationale (not just fame), practical itineraries that respect historical and spatial logic, and further-reading pathways into deeper literature.
- Site digests or entries should give the reader enough context to stand in front of a building, square, or landscape and understand *why it matters* and what conversations it participates in — without reducing it to a caption.
- Prefer primary evidence and high-quality secondary synthesis for contested local histories; surface competing claims about the place when they exist.
- The guide remains portable and useful both before travel (orientation + planning) and on site (reference + deeper notice).