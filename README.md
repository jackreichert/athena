# Athena

Rigorous, source-backed study guides that function as university-course equivalents. Notes usable by both students and professors.

Athena produces Survey, Standard, and Deep packages with transparent provenance, ranked sources, thematic synthesis, and (in full packages) structured digests that help the reader notice what is easy to miss. It does not dumb down or dictate interpretation.

## Package Shapes

- **Survey** — Foundation package: scope, ranked sources with full provenance, thematic synthesis. Digests deferred.
- **Standard** — Full undergraduate-course equivalent with complete digests.
- **Deep** — Full graduate/seminar equivalent with denser apparatus and critical engagement.

After a draft Core list exists, Phase 1 runs a bounded apparatus/bibliography pass on Core works that have scholarly apparatus. Extracted citations enter the working bibliography with provenance; they do not auto-promote to Core.

## Adaptive Applications

Load the relevant reference file when the topic matches:

- **Place / city / museum / travel guides** — `references/place-guides.md`  
  Academic-depth guides (Blue Guide / university city-history spirit). Dual-layer treatment required for major artworks. Do not artificially cap the number of digests; prioritize works a careful visitor would most regret missing. Optional Step 2: after the Markdown package is complete, produce a polished sequential visitor EPUB that restructures the same content for on-site use (linear walk-through, full dual-layer briefs, themes, TOC, embedded images, refined cover and typography). Deliver both the Markdown zip and the EPUB.

- **Scientific paper deep dives** — `references/science-paper-guides.md`  
  Journal-club and critical-reading guidance grounded in CREATE and related pedagogies.

- **Legal case method** — `references/legal-case-guides.md`  
  Case briefing, IRAC, Socratic analysis, holding vs. dicta.

- **Practical / hands-on supplements** — `references/practical-guides.md`  
  Workbooks, lab and studio companions, practicums. Task sequences with declared guidance states. Not auto-added to ordinary study guides.

## Output

Default: portable Markdown (relative links, Obsidian-friendly).  
Optional: EPUB when requested.  
Museum/collection guides may include a second visitor-oriented EPUB after the Markdown package is audited.

## Structure

- `SKILL.md` — shared spine, principles, workflow, integrity audit.
- `references/` — mode files, adaptive applications, digest template, directory layout.
- `CHANGELOG.md` — version history.
- `DEVELOPMENT.md` — notes on extending the skill.

## Version

Process version 1.35 (2026-09-28) with subsequent updates for museum visitor EPUB and expanded digest selection (2026-10-16). See `CHANGELOG.md`.

Repository: https://github.com/jackreichert/athena
