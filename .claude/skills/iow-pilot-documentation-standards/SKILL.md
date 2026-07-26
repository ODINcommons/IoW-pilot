---
name: iow-pilot-documentation-standards
description: >
  Formats, voice, and house style for writing ODIN Isle of Wight pilot
  documentation. Load this when completing or checking a session provenance
  record (provenance.md), writing facilitator or co-facilitator field notes,
  adding an entry to question-map.md, logging a row in ovn-contributions.md,
  naming a session file or folder, or drafting any repo document that must
  match the pilot's house style (British English, licence footer, heading
  style). Covers every field of provenance-template.md with a worked example,
  the field-note voice, the exact question-map and OVN table formats,
  contributor-ID conventions, and the known naming-format inconsistency.
  Does NOT cover why attribution works this way (use
  iow-pilot-provenance-and-attribution), child-safety rules in depth (use
  iow-pilot-safeguarding-and-ethics), or how to run a session (use
  iow-pilot-session-operations).
---

# IoW pilot documentation standards

How to write pilot documentation correctly: the provenance record field by field, the field-note voice, the question-map entry format, the OVN log format (OVN — Open Value Network, the public contribution log kept in `ovn-contributions.md`), file and folder naming, and the repo's house style. (One more term used throughout: SOLE — Self-Organised Learning Environment, Sugata Mitra's method and the pilot's session format.)

This skill owns **formats and voice**. The *rules* behind them — why provenance must be same-day, why field notes are committed before comparing, why the licence is CC BY-SA 4.0 — belong to **iow-pilot-provenance-and-attribution**. Where a rule is restated here, it is restated only so a format instruction makes sense on its own.

**Source discipline.** Every claim below names its source. Tier 1 = the canonical repo documents (`provenance-template.md`, `CONTRIBUTING.md`, `question-map.md`, `ovn-contributions.md`, `README.md` in the IoW-pilot repo). "Phase 1 discovery, 2026-07-03" = the founder's answers recorded at project handover. Where a Tier 1 document conflicts with this skill, the Tier 1 document wins — re-read it.

---

## When NOT to use this skill

| You want | Use instead |
|---|---|
| To understand *why* attribution, provenance timing, or the licence work the way they do; the one rule; external onboarding | **iow-pilot-provenance-and-attribution** |
| Child identity rules in depth; what may never be committed; consent | **iow-pilot-safeguarding-and-ethics** |
| To plan or run a session; before/during/after checklists | **iow-pilot-session-operations** |
| SOLE method and question design | **sole-facilitation-reference** |

---

## The provenance record, field by field

Source: `provenance-template.md` (Tier 1) throughout this section.

Three rules from the template's own header govern everything below (Tier 1, verbatim):

> Copy this file into the relevant session folder and complete every field.
> Do not leave fields blank — write "unknown" or "not recorded" if necessary.
> This record is the intellectual birth certificate of every artefact in this folder.

And from `CONTRIBUTING.md` (Tier 1): "The `provenance.md` must be committed **the same day as the session**." The template footer repeats it: *"Completed on: [date — same day as session where possible]"*.

Copy `provenance-template.md` into the session folder as `provenance.md`. Never edit the template itself.

### Session identity

| Field | What goes in it | Common mistakes |
|---|---|---|
| School code | The code from the school-codes table in `CONTRIBUTING.md` (e.g. GUR-P, COW-H). If the school is new, add it to that table first. | Inventing an ad-hoc code without registering it; using the school's full name. |
| School type | "State primary" or "State secondary" (the template offers exactly these two). | Writing the school's name or Ofsted category. |
| Date | The session date, `YYYY-MM-DD`. | Using the write-up date instead of the session date; UK-style `DD/MM/YYYY`. |
| Phase | One of `SOLE-1 / SOLE-2 / Pivot / Impactathon / Build` — exactly as listed. | Free-text like "first session"; `SOLE1` without the hyphen (see the naming section below). |
| Year group(s) | e.g. `Y5`, `Y8`, `mixed`. | Ages instead of year groups; listing a class name that could identify children. |
| Number of participants | A count. If you did not count, write "not recorded" — never guess a precise number. | Leaving it blank; inventing precision ("23" when you mean "about 25"). |
| Session duration | e.g. "90 minutes". Actual, not planned. | Recording the timetabled slot rather than what happened. |
| Location (general) | General only: "classroom, hall, outdoor" (template's own examples). | Room numbers or anything that pinpoints a specific class. |

### People

| Field | What goes in it | Common mistakes |
|---|---|---|
| Facilitator | Name or GitHub handle (adults use real identifiers — `CONTRIBUTING.md`). | Anonymising the facilitator — adults are attributable by name. |
| Co-facilitator / documentarian | Same. If solo, write "none" — not blank. But a solo session should not have happened (never plan a one-adult session — **iow-pilot-session-operations**); record "none" honestly and flag it in What happened. | Leaving blank. |
| Teacher present | **"anonymised or initials only"** (template, verbatim). Initials at most. | Writing the teacher's full name. This is the one *adult* field the template restricts. |
| Other adults | Role descriptions ("TA", "parent volunteer") or initials. If none, write "none". | Blank; full names of school staff. |

Children never appear in the People table or anywhere else by name. School code + year group is the only child identifier permitted anywhere in the repo (`CONTRIBUTING.md`, Tier 1). Full rules: **iow-pilot-safeguarding-and-ethics**.

### The question posed

Template instruction (Tier 1, verbatim): "Write the opening question exactly as it was spoken to the group."

*As spoken*, not as designed. If you planned "Who owns the water?" but actually said "So — who do you think owns the water?", record the latter. Common mistake: pasting the planned question from your session plan. The gap between planned and spoken wording is itself data.

### What happened

The field-note summary — early / middle / closing structure. Voice rules are in the next section. Common mistakes: writing it as a polished report; skipping the difficulties; leaving a phase heading empty (write "not recorded" under it instead).

The template's own sub-structure (Tier 1): **Early phase (first 15 minutes)**, **Middle phase (15–60 minutes)**, **Closing (final 15–20 minutes)**. Keep these headings even if your session ran to different timings — note the actual timings in the text.

### Questions that emerged

Template instruction (Tier 1): "List every significant question produced by participants, verbatim where possible. Tag each with the group that produced it (e.g. Group 2, Y5) and the approximate time it emerged."

Three-column table: `Question (verbatim) | Group | Approx. time`. Common mistakes: tidying children's grammar (verbatim means verbatim — "why does the sea smells funny" stays as asked); recording only the "good" questions (the map is a record, not a curation — `question-map.md`, Tier 1); tagging with a child's name instead of group + year.

Every question logged here should then be added to `question-map.md` in the format given below.

### Artefacts produced

List every file committed to the session's `artefacts/` folder, using the standard filename format (reproduced in the naming section below). Three columns: `Filename | Type | Producer (group/year)`. Common mistakes: committing artefacts that are not listed here; listing a producer by name — it is group/year only; photographing anything with a child's face or name visible (safeguarding — see **iow-pilot-safeguarding-and-ethics**).

### Licence declaration

Pre-written in the template; you complete the placeholders only: `[SCHOOL-CODE]`, `[DATE]`, `[FACILITATOR NAME]`. Do not reword the declaration, weaken it, or substitute a different licence — "Do not add a licence that is more restrictive than CC BY-SA 4.0" (`CONTRIBUTING.md`, Tier 1). Why CC BY-SA 4.0: **iow-pilot-provenance-and-attribution**.

### OVN contribution entries

List the session's contributions to be copied into `ovn-contributions.md`. Note a Tier 1 internal wrinkle: the template's OVN section lists four types (`conceptual / design / documentation / facilitation`) while `ovn-contributions.md` and `CONTRIBUTING.md` define **six** (adding `fabrication` and `deployment`). The six-type list in the log itself is the full set; the template shows the four that typically arise in a session. Use any of the six where accurate; do not invent a seventh.

### Footer

*Completed by* (your name), *Completed on* (the date — same day as the session where possible), *Committed to* (the repo URL, already filled). Common mistake: back-dating. If the record was genuinely completed the day after, say so — an honest date is worth more than a tidy one.

### Worked example (invented — every detail below is fictional)

> **Note:** `GUR-P` appears in Tier 1 as an example code, but as of 2026-07-03 no real school has been approached — GUR-P and COW-H are placeholders (Phase 1 discovery, 2026-07-03). Everything in this example, including the date, is invented for illustration. Never copy invented details into a real record, and never include any real child detail.

```markdown
## Session identity

| Field | Value |
|---|---|
| School code | GUR-P |
| School type | State primary |
| Date | 2026-09-14 |
| Phase | SOLE-1 |
| Year group(s) | Y5 |
| Number of participants | 27 |
| Session duration | 85 minutes |
| Location (general) | school hall |

## People

| Role | Name or identifier |
|---|---|
| Facilitator | Simon Pearce (@SeaWizard-ODIN) |
| Co-facilitator / documentarian | A. Facilitator (@example-handle) |
| Teacher present | J.B. |
| Other adults | one TA |

## The question posed

> Could we live without water?

## Questions that emerged

| Question (verbatim) | Group | Approx. time |
|---|---|---|
| do fish drink | Group 1, Y5 | 20 min |
| why does the sea smells funny at gurnard | Group 3, Y5 | 40 min |

## Artefacts produced

| Filename | Type | Producer (group/year) |
|---|---|---|
| GUR-P-2026-09-14-SOLE-1-001-water-mindmap-group1.jpg | photo of poster | Group 1, Y5 |

## OVN contribution entries

| Contributor ID | Type | Description |
|---|---|---|
| GUR-P-Y5 | conceptual | Questions and ideas generated in session |
| SeaWizard-ODIN | facilitation | Session design and delivery |
| @example-handle | documentation | Artefact capture and field notes |

*Completed by: Simon Pearce*
*Completed on: 2026-09-14*
*Committed to: https://github.com/ODINcommons/IoW-pilot*
```

---

## Field-note voice

Source: the "What happened" instruction in `provenance-template.md` (Tier 1, verbatim):

> A brief, honest account of the session. Include: how groups self-organised, unexpected directions taken, moments of difficulty, and anything that surprised you. This is a field note summary, not a polished report. Write it like you're telling a colleague what happened.

The same voice applies to the standalone `field-notes-facilitator.md` and `field-notes-cofacilitator.md` files in each session folder (`CONTRIBUTING.md` folder structure, Tier 1). Field notes are committed **before the two authors compare notes**, and are never merged into one document (`CONTRIBUTING.md`, Tier 1 — rationale in **iow-pilot-provenance-and-attribution**).

Rules of the voice:

- **First person.** You were there; write as yourself.
- **Honest account, not polished report.** Include what went wrong and what surprised you. A field note with no difficulty in it reads as unreliable.
- **Specifics over generalities.** "Group 3 spent ten minutes arguing about whether the sea counts as water" beats "engagement was high".
- **Early / middle / closing structure** — the template's three phase headings.
- Plain sentences. No education-sector jargon, no grant-report tone.

### Good vs bad (both invented — no real details)

**Bad** (polished-report voice — do not write this):

> The session was highly successful. Pupils engaged enthusiastically with the stimulus question and demonstrated excellent collaborative learning behaviours. All learning objectives were met and outcomes exceeded expectations.

**Good** (field-note voice — write this):

> The first ten minutes were chaos and I nearly intervened — two groups just stared at the screen. Group 3 argued about whether the sea "counts" as water, which I hadn't expected, and it turned into the most interesting thread of the session. One group copied a Wikipedia paragraph verbatim onto their poster; I let it stand. What surprised me most: nobody asked me anything after minute twenty.

The bad version could describe any session anywhere; the good version could only describe this one. That is the test.

---

## Question-map entry format

Source: `CONTRIBUTING.md` "How to add to the question map" (Tier 1). The exact format, verbatim:

```markdown
## [Question verbatim]
- **Source**: [SCHOOL-CODE], [YEAR-GROUP], [DATE], [PHASE]
- **Disciplines**: [list: e.g. environmental law, microbiology, economics]
- **Related questions**: [link to others in the map if relevant]
- **Notes**: [optional — any context about how it emerged]
```

Hard rules (Tier 1, verbatim from `CONTRIBUTING.md`): "Do not edit or rephrase existing questions. Add new ones below existing entries. The map is a record, not a curated document." And from `question-map.md` itself: "This document does not curate. It does not edit. It does not improve questions into more sensible versions."

That means: a misspelt, ungrammatical, or "wrong" question is recorded exactly as asked. The child's wording is the primary source; your annotations are secondary (`question-map.md`, Tier 1).

**Disciplines annotation style** — follow the seed-question entries in `question-map.md` (Tier 1). They list 4–6 fields, comma-separated, mixing conventional subjects with wider framings, e.g. for "Who owns the water?": *"Property law, commons theory, political philosophy, environmental economics, indigenous rights, UK water privatisation history"*. Cast wide; the map exists to show that curiosity crosses curriculum boundaries (`question-map.md`, "How to read this map"). Guidance on choosing annotations: **sole-facilitation-reference**.

The three seed questions ("Can water get sick?", "Who owns the water?", "Could we live without water?") are tagged "Project design phase, March 2025" — they came from designing the pilot, not from children. Session questions go in the "Questions" section above the seed questions, with a real source line.

---

## OVN log format

Source: `ovn-contributions.md` and `CONTRIBUTING.md` (both Tier 1).

Add one row per contribution to the table in `ovn-contributions.md`:

```
| [date] | [contributor ID] | [type] | [session ref] | [description] |
```

**The six contribution types** (definitions verbatim from `ovn-contributions.md`, Tier 1):

| Type | Definition |
|---|---|
| `conceptual` | ideas, questions, framings, hypotheses |
| `design` | drawings, annotated sketches, system designs, proposals |
| `fabrication` | physical building, prototyping, manufacturing |
| `deployment` | installing, operating, maintaining in the field |
| `documentation` | field notes, provenance records, write-ups, photography |
| `facilitation` | session design, delivery, community coordination |

**Contributor IDs** (`CONTRIBUTING.md`, Tier 1):

- Children: **school code + year group only, no names** — `GUR-P-Y5`, `COW-H-Y8`. This is a safeguarding rule as much as a format rule; full rationale and limits in **iow-pilot-safeguarding-and-ethics**.
- Adults: name or GitHub handle (e.g. `SeaWizard-ODIN`).

**Session ref**: the session folder name (e.g. `GUR-P-2026-09-14-SOLE-1`); the two existing entries use `project-init` for pre-session work — follow that precedent for non-session contributions.

The log "must be updated after every session and before any external partner joins a build phase" (`ovn-contributions.md`, Tier 1). Timing and enforcement: **iow-pilot-provenance-and-attribution**.

---

## File and folder naming

Source: `CONTRIBUTING.md` (Tier 1). The format string, verbatim:

```
[SCHOOL-CODE]-[YYYY-MM-DD]-[PHASE]-[NNN]-[description].[ext]
```

The examples given in `CONTRIBUTING.md`, verbatim:

```
GUR-P-20250915-SOLE1-001-water-questions-group2.jpg
GUR-P-20250915-SOLE1-002-buoy-drawing-annotated.jpg
COW-H-20251003-Pivot-001-field-notes-facilitator.md
IOW-IMPACT-20251115-Impactathon-007-pooseidon-alert-system-design.jpg
```

Session folders (`CONTRIBUTING.md` and `README.md`, Tier 1): one folder per session under `sessions/`, named `[SCHOOL-CODE]-[YYYY-MM-DD]-[PHASE]` — the worked example is `GUR-P-2025-09-15-SOLE-1`. Each contains `provenance.md`, `field-notes-facilitator.md`, `field-notes-cofacilitator.md`, and `artefacts/`.

Phase codes (`CONTRIBUTING.md` phase table, Tier 1): `SOLE-1`, `SOLE-2`, `Pivot`, `Impactathon`, `Build`.

### Known internal inconsistency — read before naming anything

Tier 1 disagrees with itself (documented in the Phase 1 discovery brief, 2026-07-03, and visible above):

1. **Dates**: the format string says `YYYY-MM-DD` (hyphenated), but the filename examples use compact dates (`20250915`). The session-folder example uses hyphenated dates (`GUR-P-2025-09-15-SOLE-1`).
2. **Phase codes**: the phase table says `SOLE-1`, but the filename examples use `SOLE1`.

**Recommended resolution: follow the explicit format strings, not the examples.** That means:

- Folders: `[SCHOOL-CODE]-[YYYY-MM-DD]-[PHASE]` → `GUR-P-2026-09-14-SOLE-1`
- Files: `[SCHOOL-CODE]-[YYYY-MM-DD]-[PHASE]-[NNN]-[description].[ext]` → `GUR-P-2026-09-14-SOLE-1-001-water-mindmap-group1.jpg`
- Phase codes as the phase table gives them: `SOLE-1`, not `SOLE1`.

Two absolute limits on "fixing" this:

- **Never rename existing artefacts** to make old names consistent — "Do not rename or reformat existing artefacts" (`CONTRIBUTING.md`, Tier 1, "What not to do"). A file's name is its attribution; renaming breaks the chain.
- **Do not silently edit `CONTRIBUTING.md`** to resolve the inconsistency. Fixing the source document is a change to Tier 1 and needs the founder's or maintainers' decision, made in the open (a GitHub issue or PR on github.com/ODINcommons/IoW-pilot).

Other naming details: `NNN` is a zero-padded three-digit sequence number per session (the examples run `001`, `002`, `007`); descriptions are lowercase, hyphen-separated, short, and specific; group identifiers in descriptions use group number (`group2`), never a child's name. "A correctly named file is self-describing. Its provenance travels with it when it is shared, forked, posted, or emailed. The name is the attribution." (`CONTRIBUTING.md`, Tier 1.)

---

## House style

Derived from the Tier 1 corpus itself — match what is already there.

- **British English throughout.** Licence (noun), artefact, organised, colour, programme. The repo consistently uses these spellings (`CONTRIBUTING.md`, `README.md`, Tier 1).
- **Voice: plain, warm, direct.** Short declarative sentences. Second person is fine ("Read this before you commit anything. It is short." — `CONTRIBUTING.md`). Warmth is explicit where it matters: "You are welcome here. The only condition is that you bring the attribution chain with you." (`CONTRIBUTING.md`, Tier 1.)
- **Unhedged where rules are absolute.** Rules are bold, imperative, unqualified: "**Everything gets attributed before it gets built.**"; "Do not leave fields blank". Do not soften absolute rules with "please try to" or "where convenient". Hedge only where the thing is genuinely open — e.g. session-duration defaults, where the template offers only "e.g. 90 minutes". (The template footer's "same day *where possible*" is not a model hedge: CONTRIBUTING.md's rule is absolute — "must be committed **the same day as the session**" — and the footer wording covers physical impossibility only, with the late-commit honesty rules in **iow-pilot-session-operations** applying.)
- **Short sections separated by horizontal rules** (`---`). Every Tier 1 document does this. One idea per section.
- **Sentence-case headings.** "The one rule that matters most", "How to add to the question map", "What this is not" — not Title Case.
- **Tables and fenced code blocks** for anything structured: codes, formats, examples.
- **The licence footer pattern.** Tier 1 documents end with an italicised CC BY-SA 4.0 footer that names the licence and invites forking while requiring attribution. Verbatim specimens:
  - `CONTRIBUTING.md`: *"This document is itself licensed under CC BY-SA 4.0. Fork it, adapt it, use it for your own commons project. Just carry the attribution."*
  - `question-map.md`: *"This document is licensed under CC BY-SA 4.0. Fork it. Annotate it. Translate it. Carry the attribution."*

  New repo documents should carry a footer in this pattern.

### Date-stamping volatile claims

Any claim that can go stale — statuses, plans, timelines, "current" anything — must carry a date: "as of 2026-07-03, …". This is a learned lesson, not a nicety: the corpus already contained a dead timeline presented as live. `CONTRIBUTING.md`'s examples carry 2025 dates and `ovn-contributions.md`'s entries are dated 2025-03-30, while `README.md`'s status line reads "First sessions planned for 2026" — the 2025 dates are illustrative leftovers, not a live timeline (Tier 1 documents compared; git history "Change launch year in project status"; Phase 1 discovery, 2026-07-03). A reader with no context cannot tell a stale claim from a live one unless you stamp it. When you write anything of the form "X is planned", "X is underway", "the current status is X" — date it, and only assert it if Tier 1 or a Phase 1 answer confirms it.

---

## Provenance and maintenance

- **Written**: 2026-07-03, from the Tier 1 documents of the IoW-pilot repo (`provenance-template.md`, `CONTRIBUTING.md`, `question-map.md`, `ovn-contributions.md`, `README.md`, all quoted at that date's state) and the Phase 1 discovery brief (founder's answers, 2026-07-03).
- **What may drift**:
  - `CONTRIBUTING.md` may be amended to resolve the naming inconsistency documented above — if it has been, the amended format string wins and the inconsistency note here is historical.
  - The school-codes table (GUR-P, COW-H are placeholders as of 2026-07-03; real schools will add real codes).
  - `provenance-template.md` fields may be added or reworded; the field-by-field guide above describes the template as of 2026-07-03 — always complete the *current* template, not this skill's memory of it.
  - The OVN contribution-type list (four in the template vs six in the log, as of 2026-07-03) may be harmonised.
  - The `sessions/` folder does not exist yet as of 2026-07-03; once real sessions exist, their records become additional format precedents.
- **How to re-verify**: read the six Tier 1 files in the repo root (README.md, CONTRIBUTING.md, provenance-template.md, question-map.md, ovn-contributions.md, LICENSE) and compare against this skill; check github.com/ODINcommons/IoW-pilot for the canonical current versions — local snapshots may be stale. Where this skill and the current Tier 1 documents disagree, Tier 1 wins; update this skill.

---

*This document is licensed under CC BY-SA 4.0.*
*Fork it, adapt it, use it for your own commons project.*
*Just carry the attribution.*
