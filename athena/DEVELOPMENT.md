# Athena Skill Development & Expansion Notes

These notes exist so the modular structure of Athena stays intentional as the skill grows. Read this before adding a new mode, a new adaptive application (e.g. another domain like the place guides), or significantly expanding the research spine.

## Design contract (how the skill is structured)

Athena is treated as a **code module**:

- **SKILL.md** (the loaded instructions) contains **only what is common to every run**:
  - Frontmatter + high-level purpose
  - Guiding Principles (shared)
  - Core Value rules (citations, provenance, further research, anti-bias)
  - High-level Package Shapes decision rules + one-paragraph summaries
  - Shared Workflow (Phases 0–5) with pointers — Phase 5 is the mandatory post-assembly package integrity audit
  - Output Conventions + Constraints
  - Resource pointers

- **Mode-specific behavior** lives in `references/mode-*.md`. These are *deltas* only:
  - Purpose of the shape
  - What is in / out of scope
  - Phase adaptations
  - Quality expectations unique to that shape
  - Do **not** duplicate the shared spine.

- **Adaptive applications** (currently Place / Location / Travel & Museum Guides) live in `references/place-guides.md`. They are orthogonal to modes (a place guide can be Survey, Standard, or Deep). The main file has a short pointer; the full requirements are loaded when the topic is place-based.

- **Templates and layouts** stay in `references/` (`digest-template.md`, `directory-layout.md`).

- **Changelog** is *not* part of the runtime skill. It lives at package top level (`CHANGELOG.md`) so maintainers and users can see history without bloating the agent’s context.

This matches the progressive-disclosure model of Agent Skills: metadata always visible → SKILL.md body loaded on trigger (keep lean) → references loaded on demand.

## How the agent is expected to work with this structure

1. On trigger, load SKILL.md.
2. In Phase 0, decide the package shape (Survey / Standard / Deep) from user language and topic.
3. Immediately load the corresponding `references/mode-*.md` and follow its adaptations for the rest of the run.
4. If the topic is a place, city, region, museum, or travel guide, also load `references/place-guides.md`.
5. Load digest-template.md and directory-layout.md when needed in Phase 2 / assembly.

If a mode file is not loaded, behavior drifts. The main SKILL.md therefore contains explicit “Load the mode file” instructions.

## Adding or expanding

### Discovery-first rule (required before any new mode or adaptive application)

Before writing a new mode file or a new adaptive-application reference, **run Athena’s own Deep (or at least Survey) process on the pedagogy of the domain itself**.

Treat “how the best programs and practitioners study / teach this subject” as the topic:

- Mine real syllabi, teaching guides, pedagogical literature, bar-exam or graduate-method resources, lab-notebook standards, case-method materials, scientific-paper reading guides used in top departments, etc.
- Rank the core sources on *method* (not just content).
- Extract the themes that define rigorous practice in that field (e.g., for legal cases: issue-spotting, holding vs. dicta, procedural posture, subsequent treatment; for scientific papers: study design, statistical claims, limitations, reproducibility, related-work positioning).
- Only after that foundation exists should you design the Athena overlays (digest adaptations, required sections, quality gates, further-reading pathways).

This is non-negotiable. Skipping it produces generic or superficial modules that feel bolted on rather than grounded in how the discipline actually works. The place/museum guides succeeded because they were informed by Blue Guide practice, university city-history syllabi, and museum education literature. New domains deserve the same treatment.

### New package shape / mode
1. Perform the Discovery-first process above if the new shape has distinctive pedagogical goals.
2. Create `references/mode-<name>.md` following the existing pattern (purpose, key differences, phase adaptations only).
3. Add a one-paragraph summary + decision language to the Package Shapes section in SKILL.md.
4. Update the description frontmatter triggers if new language is needed.
5. Bump process version and add an entry to CHANGELOG.md.
6. Test that a Survey-style request and a Deep-style request still produce recognizably different packages.

### New adaptive application (new domain, e.g. “legal case study guides” or “scientific paper deep dives”)
1. **Discovery-first** (see rule above). Produce at least a Survey (ideally Deep) Athena package on the teaching/studying practices of the domain and use it as the design brief.
2. Create `references/<domain>-guides.md` with the domain-specific requirements, source types, digest adaptations, and deliverable emphases that emerged from the discovery.
3. Add a short “Adaptive Applications” bullet or subsection in SKILL.md that points to the new reference and states when to load it.
4. Update directory-layout.md and digest-template.md only if the new domain requires structural changes that are not already covered.
5. Keep the shared research spine (syllabi/provenance, ranked sources, themes with citations, further reading) intact; the adaptive file should only supply the domain-specific overlays.

### Changing the shared spine
Any change that affects all modes (new phase, new required file, change to citation practice, anti-bias rules, etc.) goes in SKILL.md. Then check every mode file and the place-guides file for consistency and update deltas if needed.

### Versioning
- Bump the **Process version** line in SKILL.md on every meaningful change to behavior.
- Record the change in CHANGELOG.md with enough detail that a future maintainer understands *why*.
- Prefer small, focused process-version bumps over large rewrites.

## Anti-patterns to avoid
- Putting mode-specific instructions back into the main SKILL.md “just in case.”
- Copying large blocks of the shared workflow into mode files.
- Letting the Changelog live inside SKILL.md (it costs tokens on every load and is irrelevant to execution).
- Nested reference chains that require the agent to load A to discover it must load B.
- Growing SKILL.md past ~400–500 lines without extracting.

## Package layout (repo)

Recommended top-level package structure (GitHub root):

```
athena/                     # the installable skill
├── SKILL.md
├── CHANGELOG.md            # or move to repo root
├── DEVELOPMENT.md          # this file
└── references/
    ├── mode-survey.md
    ├── mode-standard.md
    ├── mode-deep.md
    ├── place-guides.md
    ├── digest-template.md
    └── directory-layout.md
README.md                   # human-facing overview, install, how to try
INSTALL.md                  # if needed
```

The skill directory itself can be copied or pointed at for installation. Keep the skill directory self-contained so “install this folder” works.

## Why this structure exists
The original monolithic SKILL.md mixed shared rules, mode deltas, place-specific rules, and history. That made the loaded context larger than necessary and made future expansion harder (every new feature risked polluting the common path). Treating modes and adaptive applications as loadable modules keeps the common path stable and the specializations explicit.
