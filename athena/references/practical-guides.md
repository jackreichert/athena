# Practical Guides / Hands-on Course Supplements (Athena Adaptive Application)

Load this file when the user asks for a **practical, hands-on, workbook, lab, studio, practicum, implementation, or job-aid companion** to a course (including an existing Athena study package), or when the topic is itself a practicum / studio / laboratory / skills course. Orthogonal to package shape (Survey / Standard / Deep). May be combined with other adaptive applications (a science-paper package may also grow a practical companion).

This overlay is grounded in the Discovery-first Deep package on the pedagogy of practical guides (cognitive apprenticeship; 4C/ID / Ten Steps; worked examples and fading; Schön’s reflective practicum; Understanding by Design / constructive alignment; deliberate practice; laboratory genre critique; checklists as performance support). Do not invent a pile of “exercises” that ignore that brief.

## Core orientation

A practical companion is a **supplement that makes the reader do the work the course claims to teach**. It is not a friendlier restatement of the digests, not a quiz bank, and not a substitute for the primary encounter.

The written unit is a **task sequence with a declared guidance state**, not a chapter of activities. Alignment is non-negotiable: each task must be a performance the parent course’s outcomes already named (or that this package’s own outcomes name, if the practical layer *is* the course).

Goals of the companion:
- Make expert thinking visible at least once before independent performance is demanded
- Move guidance (modeled → faded / completion → independent → exploratory-with-scaffolds) rather than parking on a recipe or on unguided search
- Specify feedback and acceptable evidence for the performance, not for having filled blanks
- Label job aids as job aids (they assume competence) and lessons as lessons
- Name how the sequence can fail (cookbook compliance, inert knowledge, unguided flop, expertise reversal, activity-for-its-own-sake)

Digests still do not replace reading. Practical tasks do not replace digests.

## When to load — and when not to

**Load** when the user says practical guide, hands-on supplement, workbook, lab manual, studio brief, practicum, implementation companion, “exercises for this course,” job aid, checklist companion, or when the topic is already a lab / studio / practicum / skills course.

**Do not auto-add** a practical layer to every Athena run. A Plato or Kant package does not grow a workbook unless asked. Auto-adding exercises is the activity-oriented failure this overlay exists to prevent.

Science-paper and legal-case overlays already contain proto-tasks (annotate the figure; write the next experiment; hypotheticals). When those overlays are loaded *and* the user also asked for a practical companion, promote those hooks into the `practical/` directory instead of inventing a second, disconnected exercise list.

## Design unit

Default unit: a **task that could count as evidence** of a stated outcome, written at a declared guidance state.

Alternate unit when the work is professional artistry rather than a well-structured problem: a **studio brief + critique protocol** (Schön), not a faded algebra example.

Alternate unit when the user already has the skill and the risk is omission under complexity: a **job aid / checklist** (Gawande). Do not grade a job aid as a lesson.

Lab exercises and faded-example items are specializations of the task unit. Part-task drills are allowed only for routines that must automate (4C/ID component 4) and must not become the spine.

### Guidance states (declare on every task)

- **Modeled** — worked example or demonstration that makes control decisions / framing visible
- **Completion / faded** — part of the solution or brief is given; the learner finishes; successive tasks withhold more
- **Independent** — the learner performs the whole task
- **Exploratory** — only with specified scaffolds (problem structure, tools, constraints). “Figure it out” with no scaffolds is not a legal state for novices

A one-page worksheet cannot fade. Fading requires a series, or explicit parallel tracks (novice sequence / independent studio brief) when the audience is mixed.

Productive-failure designs (struggle *then* canonical instruction) are allowed only when the consolidation phase is actually written. Struggle without the second phase is a failure mode, not a method.

## Required files

Create `practical/` only when this overlay is in scope. Do not leave it empty.

```
practical/
├── README.md              # How to use the companion; relationship to the parent package
├── 00-outcomes.md         # Performances the tasks train; map to parent-course outcomes
├── 01-sequence.md         # Task index with guidance state + outcome link for each item
└── tasks/
    ├── 01-short-slug.md
    └── ...
```

Deep companions also include `practical/instructor-notes.md` (how to run a critique, what to watch on the first attempt, common misfires).

Optional: `practical/job-aids/` for true checklists, kept separate from lesson-tasks.

## Required sections on every task file

1. **Performance** — what the learner will *do*, in the language of the outcome
2. **Guidance state** — one of the four above, with a one-line reason
3. **Genre label** — faded-example item / inquiry or verification lab / studio brief / practicum artifact / job aid / simulation protocol / other named genre
4. **Links back** — parent digest(s) and theme(s), or named sources if the parent is Survey
5. **Modeled example or pointer** — on this page or an earlier page in the sequence. Independent and exploratory tasks must point to the prior model unless a documented productive-failure design is in play
6. **What good looks like** — criterion or critique foci, not a secret key that replaces judgment in swampy work
7. **Feedback** — who inspects (self / peer / coach / answer-comparison), what they inspect, when
8. **Failure-mode note** — the one or two ways *this* task most easily collapses
9. **Job-aid vs. lesson** — explicit if the page could be mistaken for the other

Supportive information (why the domain is organized this way) stays in digests and themes. Just-in-time procedure may live on the task page. Do not mix a lecture and a recipe into one unlabeled blob.

## Phase adaptations

### Phase 0
Declare that a practical companion is in scope. Add learning outcomes that are *performances*. Load this file in addition to the mode file. If the request is “only the practical companion” to an already-built study package, still write a short `00-scope.md` note that names the parent package and the performances.

### Phase 1
Keep the shared source spine for the study layer. For the practical layer, also collect exemplars of the *genre* (a strong lab manual page, a studio brief, a faded-example sequence, a checklist) when they help the designer. Do not replace primary sources with how-to blogs.

### Phase 2
Digests follow the ordinary template (and any other loaded overlay). Do not turn digests into worksheets. The practical layer is a separate directory.

### Phase 3
At least one theme should address how the course’s work is actually *done* (method, studio culture, lab genre, briefing practice). Place and science-paper overlays already require a Navigating / next-experiment theme; keep those and link them from `practical/01-sequence.md`.

### Phase 4
Assemble `practical/` as specified. Parent `README.md` must point to it and say how study and practice are sequenced (usually: encounter source → digest check → task, or task-as-prep when the design is productive-failure or a pre-reading lab).

### Phase 5 (additional audit when this overlay is loaded)
After the shared integrity audit, verify:
- `practical/` exists and is non-empty
- `practical/README.md`, `00-outcomes.md`, `01-sequence.md` are complete, not stubs
- every task listed in `01-sequence.md` has a complete file under `practical/tasks/` with the required sections
- every task maps to a stated outcome
- at least one modeled task exists before the first independent task, unless a productive-failure design is documented in `00-outcomes.md`
- no task is only “reread the digest and write a paragraph”
- empty `practical/` fails the audit the same way a missing digest file does

If any check fails, return to Phase 4 (or 0 if outcomes were never performances) and repair.

## What this overlay refuses

- Activity-for-its-own-sake (hands-on as a goal rather than as evidence of a result)
- Cookbook pages sold as inquiry
- Reflection journals that stand in for critique or for self-explanation of a worked step
- Checklists assigned to novices as if they were worked examples
- Measuring compliance with the worksheet instead of the performance
- A single `exercises.md` dump

## Relationship to the shared spine

All standard Athena rules remain in force. This file supplies only the practical-companion overlay. Survey + practical is allowed (practice a first authentic move that points at named sources). Standard/Deep + practical is the intended full form.
