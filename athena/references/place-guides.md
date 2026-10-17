# Place / Location / Travel & Museum Guides (Athena Adaptive Application)

Athena supports **place-based guides** at academic depth — cities, regions, historic landscapes, and museums — modeled on the best scholarly and high-cultural practice (Blue Guides’ “understand more fully what one sees,” university “History of [City] / Biography of a City” syllabi, Harvard-style layered city histories, cultural-landscape approaches). These are not tourist-brochure or “top 10 Instagram” lists. They aim for the knowledge a serious traveler or student would want: historical layers, why sites matter in the scholarly conversation, what not to miss and *why*, and a transparent evidence base.

The process has two mandatory stages for museum and major site guides:

1. **Step 1 — Markdown package (always first).** Full research, ranked sources with provenance, dual-layer digests for every Core and Important space/work, themes, glossary, further reading, limitations. Delivered as a zip.
2. **Step 2 — Visitor EPUB.** After the Markdown package is complete and audited, produce a polished sequential EPUB that restructures *the same content* for on-site use. The EPUB does not abbreviate the dual-layer analysis. Delivered alongside the Markdown zip.

## Shared requirements for all place / location guides

- **Start with syllabi and highest-quality sources.** Preferentially mine university syllabi and reading lists for “History of [Place],” “Art & Architecture of [Place],” urban history, or equivalent courses. When syllabi are thin or unavailable, fall back to the strongest scholarly monographs, architectural histories, official institutional catalogues, and classic cultural guides (e.g., Blue Guide tradition). Log every syllabus or discovery source consulted (as in Phase 1 provenance rules). Compile a full working bibliography with provenance notes.
- Treat major **sites, monuments, neighborhoods, landscapes, and (when relevant) artworks** as primary sources. Digests or site entries emphasize historical context, significance, formal or spatial character, and current condition/location.
- Produce a practical but scholarly **walkthrough / itinerary / “what not to miss”** theme or section grounded in the historical and critical literature, not popularity rankings.
- **Historical overview / orientation is required.**
  - For city, region, location, and travel guides: include a clear historical overview (layered chronology or key periods) so the reader understands the place as a sequence of transformations, not a static set of attractions.
  - For museum / collection guides: always include location and institutional context — the building’s history, the institution’s founding and later development, the dynasty or patronage system that shaped the collection, and any major political or cultural settlements that frame the works. This is not optional.
- **Images when they enhance understanding:** Include maps, site plans, exterior/interior photographs, or key artworks when visual reference materially helps the reader. Prefer official or public-domain sources; store under `images/` with relative links and captions that credit the source. Especially valuable for complex sites, floor plans, and works discussed in digests.
- Support iterative expansion: a first guide can be high-level; the user can later request deeper treatment of a neighborhood, museum, or theme.
- Hybrid review type is usually optimal.
- Always note that physical conditions, openings, and hangings can change.
- Deep mode adds denser historiography, debates about the place, and specialist literature.

## Unmissable works and spaces (ranking, not capping)

For museum and major site guides, the goal is to give the visitor everything they would regret missing on a single visit, without overwhelming them. The selection should feel opinionated and practical (Rick Steves style: “if you have time, do this; if not, do that; skip this overhyped thing”), not encyclopedic or Lonely Planet comprehensive.

- **Do not artificially cap the number of digests.** Prioritize the works and spaces a careful visitor would most regret missing, grounded in institutional highlights, official “must-see” lists, and scholarly consensus.
- **Cover the principal strengths, not the entire collection.** A museum’s famous unique object (Dead Sea Scrolls, a single masterpiece, a historic room) is Core, but so are the major collections that sit beside it. Do not treat “unmissable” as synonymous with “one-of-a-kind,” and do not attempt to digest every work. Survey the institution’s principal departments and select the strongest, most regret-missing works or spaces from each — opinionated and limited, not comprehensive. Document the selection in `01-sources.md`.
- **Rank them opinionatedly.** Present a clear priority order so the visitor can decide depth:
  - **Must-see** (do not leave without these).
  - **If you have time** (strong, worth it when the schedule allows).
  - **Skip or deprioritize** (overhyped, repetitive, or lower priority relative to the above).
  - Offer both a short route (“one focused hour”) and a fuller route (“you may never return”).
- Expand beyond an initial Core list when additional major works or departmental strengths (key Rembrandts, Caravaggios, Rubens, Titians, major galleries, essential objects, archaeological or design holdings) are clearly part of the collection’s essential offerings. Document the expanded selection in `01-sources.md` and `limitations.md`.
- For each ranked item that receives a digest, supply the full dual-layer treatment (zone-by-zone + period-specialist analysis) so the visitor can look with precision.

## Museum / collection / exhibition specializations

- Treat individual **artworks, objects, or spaces** as primary sources. Digests emphasize formal description, iconography/symbolism, historical context, provenance, and current location (room/floor when known).
- **Dual-layer treatment for artworks and complex spaces (required):** (1) Unit-by-unit / zone-by-zone summaries that map the object or room (including exterior panels, wings, or distinct spatial zones); (2) a dedicated Period-Specialist Analysis that situates style, technique, iconography, patronage, workshop practice, and meaning in period context and explicitly surfaces symbolism a general viewer is likely to miss, period-specific historical context, significant visual details or objects, and the meaning of colors as understood in that period. Both layers are required — do not substitute one for the other. In Deep mode, ground the specialist analysis more explicitly in named specialists or standard period literature.
- **Images (required when they enhance understanding):** For major artworks and key visual objects, include at least one high-quality reference image in the digest (and additional detail images when useful). Prefer official museum collection images or public-domain high-resolution sources. Place the primary image near the top of the digest (after the bibliographic entry). Always caption with credit, inventory number when known, and a link to the official collection page. Store images under `images/` with relative Markdown links. Note that physical hangings and lighting can change; the image is a study reference.
- Prioritize **official museum resources** (collection pages, official highlights/itineraries, floor plans) alongside scholarly consensus lists. Link to official collection pages wherever possible.
- When multiple creators are central, add **`artists-bios.md`** (or `creators-bios.md`) with short parallel biographies.
- Always include location and institutional history (see shared rule above).

## Step 1 — Markdown package (always first)

Produce the full Standard (or Deep) package before any EPUB work:

- `00-scope.md`, `01-sources.md` (with ranked Core / Important / Supplementary and provenance),
- complete dual-layer digests under `digests/` for every Core and Important space or work,
- `02-digests.md` index,
- themes under `themes/` (including a navigating / walkthrough theme and a location-and-institution theme),
- glossary, further-reading, limitations,
- artists-bios when relevant,
- images when they help.

Deliver the audited Markdown package as a zip. Do not begin the EPUB until this package is complete.

## Step 2 — Visitor-Oriented EPUB

After the Markdown package is complete and audited, produce a polished sequential EPUB that restructures the *same* content for use before and during a visit. This is a required second deliverable for museum and major site guides unless the user explicitly declines it.

**The EPUB must contain all the analytical content of the original digests and themes.** It reorganizes and presents; it does not abbreviate, summarize, or dumb down the dual-layer briefs. When converting, transcribe the full Pre-Reading Context, Summary, Full Brief (including “What Is Easy to Miss,” zone-by-zone, and Period-Specialist Analysis), and theme narratives. Do not substitute shorter paraphrases.

### Structure of the EPUB

- Elegant title page and a refined, high-class cover (navy and gold architectural linework or equivalent site-appropriate design; generate or source a proper cover image — do not omit or use a plain placeholder).
- Explicit Table of Contents page with internal links.
- How to Use This Guide (suggested routes: short focused visit / half-day / full; practical notes on hours, tickets, audioguide, photography).
- Location and institutional history chapter(s) — building, dynasty or patronage, founding of the museum, major political or cultural context.
- Ranked Must-See Checklist with opinionated tiers (Must-see / If you have time / Skip or deprioritize) so the visitor can choose depth without being overloaded.
- Linear walk-through chapters that follow a practical route through the site (organized as a walking guide). Each major work or space receives its full dual-layer treatment transcribed from the Markdown digests (not a condensation).
- Themes chapter (full synthesis with “Across the Sources: What Is Easy to Miss”).
- Reference chapters at the end: Artists and Creators (when relevant), Glossary, Bibliography and Further Reading, Limitations and Practical Notes.
- Embedded high-quality images with captions in the relevant chapters. Note that images are study references.
- Important visitor information and walkthrough help integrated throughout (watch-fors, what is easy to miss, route suggestions, practical constraints, opinionated skips).

### Design

- High-class museum-catalogue aesthetic: serif typography, generous leading, warm off-white ground, deep navy headings, subtle gold rules.
- Refined cover is required (navy and gold architectural linework works well for major buildings; adapt to the site). Do not deliver an EPUB without a proper cover.
- Watch-fors and “what is easy to miss” lists kept with each work for on-site looking.
- Explicit Table of Contents.
- Organized as a walking guide (linear route, practical pacing) while retaining every dual-layer brief from the Athena package.

### Delivery

Offer both the Markdown zip (Step 1) and the finished EPUB (Step 2). The EPUB restructures and presents the same analytical content for a visitor; it does not replace the Markdown package and does not reduce its depth.

This two-step process was distilled from the Kunsthistorisches Museum guide and refined with the Sisi Museum / Imperial Apartments guide (2026). It is the default for any serious museum or major historic-site request.

## Location / city / region / travel guide emphases

- Frame the package as the equivalent of a short university course or serious independent study of the place (history, built environment, cultural layers).
- **Historical overview is required.** Core deliverables include: historical orientation (periodized or thematic), ranked must-see sites with scholarly rationale (not just fame), practical itineraries that respect historical and spatial logic, and further-reading pathways into deeper literature.
- Site digests or entries should give the reader enough context to stand in front of a building, square, or landscape and understand *why it matters* and what conversations it participates in — without reducing it to a caption.
- Prefer primary evidence and high-quality secondary synthesis for contested local histories; surface competing claims about the place when they exist.
- The guide remains portable and useful both before travel (orientation + planning) and on site (reference + deeper notice).
- The same two-step process (Markdown package first, then visitor EPUB) applies when the user wants a polished on-site guide.
