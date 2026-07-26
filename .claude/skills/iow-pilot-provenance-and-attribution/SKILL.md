---
name: iow-pilot-provenance-and-attribution
description: The change control of the ODIN Isle of Wight pilot. Load this whenever you are about to commit, name, rename, license, log, merge, or build on ANY artefact in the IoW-pilot repository — session photos, field notes, question-map entries, OVN log rows, build files — or when onboarding an external contributor (hackspace, makerspace, industry partner, individual — for Pooseidon/build-phase partners specifically, pooseidon-development-pathway applies this skill's gate). Owns the one rule ("Everything gets attributed before it gets built"), provenance-record timing, field-note independence, question-map non-curation, the file-naming convention, the OVN contribution log, the CC BY-SA 4.0 licence, external onboarding, and the what-not-to-do list. Also load it if you find an incomplete provenance record and need to know what to do.
---

# IoW Pilot: Provenance and Attribution

This skill is the single home of the provenance and attribution rules for the ODIN Isle of Wight pilot. Every other skill in this library defers to it on these matters. If another document appears to conflict with `CONTRIBUTING.md` in the repo, re-read `CONTRIBUTING.md` — it wins.

**Repository:** https://github.com/ODINcommons/IoW-pilot (local working copy: the `IoW-pilot` folder containing `CONTRIBUTING.md`). All rules below are quoted or derived from the Tier 1 canonical documents in that repo: `CONTRIBUTING.md`, `provenance-template.md`, `ovn-contributions.md`, `question-map.md`, `LICENSE`, `README.md`.

**Jargon, defined once:**
- **SOLE** — Self-Organised Learning Environment (Sugata Mitra's method): children self-organise around a big question with no curriculum and no predetermined answers.
- **OVN** — Open Value Network (Sensorica/hREA lineage): a way of logging every contribution to a shared project so value and credit are traceable.
- **Provenance record** — the completed `provenance.md` in a session folder, filled in from `provenance-template.md`. The template calls it "the intellectual birth certificate of every artefact in this folder" (provenance-template.md, Tier 1).
- **CC BY-SA 4.0** — Creative Commons Attribution-ShareAlike 4.0 International, the repository's licence.

---

## The one rule

From `CONTRIBUTING.md` (Tier 1), verbatim:

> **Everything gets attributed before it gets built.**
>
> The intellectual work in this repository originated with children in state schools on the Isle of Wight. Before any external contributor — individual, organisation, or institution — begins building on that work, the provenance record must be complete, public, and current. Check `sessions/` and `ovn-contributions.md` before you start. If a session's provenance record is incomplete, complete it first.

Why this rule exists: attribution is the defence against enclosure and extraction. Children in state schools cannot police how their ideas are used; the public, complete, current provenance chain does it for them. There is **no path** to building on session artefacts that skips this gate — not for speed, not for a demo, not for a funder deadline.

One rule outranks even this one: **safeguarding**. No child's name, image, or identifying detail may ever appear in any record, however attribution-complete it makes the record feel. See `iow-pilot-safeguarding-and-ethics` — that skill is supreme.

---

## Provenance records: what and when

Each session gets its own folder under `sessions/` (as of 2026-07-03 the `sessions/` folder does not yet exist — no sessions have run; the first sessions are planned for 2026 per the README status line, Tier 1). The structure, from `CONTRIBUTING.md` (Tier 1):

```
sessions/
└── GUR-P-2025-09-15-SOLE-1/
    ├── provenance.md              ← completed from provenance-template.md
    ├── field-notes-facilitator.md
    ├── field-notes-cofacilitator.md
    └── artefacts/
        └── [named files]
```

(Note: `GUR-P` here and throughout is a **placeholder example** — per Phase 1 discovery, 2026-07-03, no real school has been approached yet. The 2025 dates in the repo's examples are illustrative leftovers, not a live timeline.)

**Timing rules (both from CONTRIBUTING.md, Tier 1, verbatim):**

> The `provenance.md` must be committed **the same day as the session**.
> Field notes must be committed **before the two authors compare notes**.

Why same-day: memory decays and provenance is evidence; a record written a week later is a reconstruction, not a record. Why commit field notes before comparing: the two authors' notes are **independent evidence**. If they compare first, they converge — consciously or not — and the pilot loses its ability to show that two observers independently saw the same thing. Commit first, compare after, and **never merge two authors' notes into one document** (see the what-not-to-do list below).

When completing `provenance.md`, complete **every field** — the template instructs: "Do not leave fields blank — write 'unknown' or 'not recorded' if necessary" (provenance-template.md, Tier 1). An honest "not recorded" is a valid provenance statement; a blank is a hole.

---

## The question map is a record, not a curated document

From `CONTRIBUTING.md` (Tier 1):

> Do not edit or rephrase existing questions. Add new ones below existing entries. The map is a record, not a curated document.

And from `question-map.md` itself (Tier 1):

> This document does not curate. It does not edit. It does not improve questions into more sensible versions. It records them exactly as they were asked, by whom, and when.

Questions go in **verbatim** — spelling, grammar, and all. A 9-year-old's phrasing is the primary source; "improving" it destroys the data and the attribution at once. Annotations (disciplines, related questions, notes) are secondary and may be added; the question text itself is untouchable once committed.

**Copy-usable question-map entry stub** (format from CONTRIBUTING.md, Tier 1):

```markdown
## [Question verbatim]
- **Source**: [SCHOOL-CODE], [YEAR-GROUP], [DATE], [PHASE]
- **Disciplines**: [list: e.g. environmental law, microbiology, economics]
- **Related questions**: [link to others in the map if relevant]
- **Notes**: [optional — any context about how it emerged]
```

Add new entries within the "## Questions" section of `question-map.md`, below existing session entries — the seed-questions section stays untouched at the bottom of the file. For how to choose disciplinary annotations, see `sole-facilitation-reference`; for the entry format in house style, see `iow-pilot-documentation-standards`.

---

## File naming: the name IS the attribution

Every file committed to the repository follows this format (CONTRIBUTING.md, Tier 1, verbatim):

```
[SCHOOL-CODE]-[YYYY-MM-DD]-[PHASE]-[NNN]-[description].[ext]
```

School codes (CONTRIBUTING.md, Tier 1): Gurnard Primary = `GUR-P`, Cowes High = `COW-H`, "(add as needed)". Phase codes: `SOLE-1`, `SOLE-2`, `Pivot`, `Impactathon`, `Build`.

Why this matters (CONTRIBUTING.md, Tier 1, verbatim):

> A correctly named file is self-describing. Its provenance travels with it when it is shared, forked, posted, or emailed. The name is the attribution.

**Known internal inconsistency — do not silently "fix" it.** The repo's format string and its worked examples disagree on date and phase formatting. The rule: **follow the explicit format string** (hyphenated date, phase code as in the phase table — e.g. `GUR-P-2026-09-15-SOLE-1-001-water-questions-group2.jpg`), and **never rename existing artefacts** to match ("Do not rename or reformat existing artefacts" — the what-not-to-do list; renaming severs the attribution the name carries). The full note — the repo's examples verbatim, the resolution steps, and the limits — lives in `iow-pilot-documentation-standards`.

---

## The OVN contribution log

`ovn-contributions.md` (Tier 1) is "the backbone of attribution". Its own header states when it must be updated, verbatim:

> It must be updated after every session and before any external partner joins a build phase.

So: **after every session** (same day, alongside the provenance record) and **before any external partner joins a build** (an out-of-date log means the partner cannot see whose work they are building on — the gate fails).

**Contribution types** (ovn-contributions.md, Tier 1): `conceptual` / `design` / `fabrication` / `deployment` / `documentation` / `facilitation` — six types, covering ideas and questions through to building, operating, and the meta-labour of documenting and facilitating. The full type-by-type meanings table lives in `iow-pilot-documentation-standards`.

**Contributor IDs** (CONTRIBUTING.md, Tier 1):
- **Children: school code + year group ONLY** — `GUR-P-Y5`, `COW-H-Y8`. Never names, never initials, never anything that could identify an individual child. This is where safeguarding outranks even attribution: a child's contribution is credited to their cohort, not their person, because their safety matters more than the precision of their credit. See `iow-pilot-safeguarding-and-ethics`.
- **Adults: name or GitHub handle** (e.g. `SeaWizard-ODIN`).

**Copy-usable OVN log row** (format from CONTRIBUTING.md, Tier 1 — add it to the table in `ovn-contributions.md`):

```
| [date] | [contributor ID] | [type] | [session ref] | [description] |
```

Worked example modelled on the log's existing entries (the log currently holds two entries, both dated 2025-03-30, contributor `SeaWizard-ODIN`, session ref `project-init` — Tier 1, as of 2026-07-03):

```
| 2026-09-15 | GUR-P-Y5 | conceptual | GUR-P-2026-09-15-SOLE-1 | Questions and ideas generated in session |
```

The provenance template's "OVN contribution entries" section lists each session's contributions for transfer into the log — fill it in, then copy the rows across.

---

## The licence: CC BY-SA 4.0, and never anything tighter

All content in the repository is licensed under **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)** (`LICENSE`, Tier 1; copyright "(c) 2025 Simon Pearce / ODINcommons contributors").

What it means, from `CONTRIBUTING.md` (Tier 1, verbatim):

> - You may use, share, and adapt any content here
> - You must credit the original creators (see provenance records)
> - You must release any derivative work under the same licence
> - You may not add legal restrictions that prevent others from doing the same
>
> This is the copyleft of the commons. It protects everyone who contributed, especially those who contributed first.

The `LICENSE` file adds (Tier 1): attribution "must be visible and must travel with every derivative work", and "No additional restrictions — You may not apply legal terms or technological measures that legally restrict others from doing what this licence permits."

**Why nothing more restrictive may ever be added:** the ShareAlike copyleft is the mechanism that keeps children's work in the commons forever. A more restrictive licence on any derivative would enclose downstream work — exactly the extraction the one rule exists to prevent — and would strip the first contributors (the children) of the open access to derivatives that the licence guarantees them. "Do not add a licence that is more restrictive than CC BY-SA 4.0" (CONTRIBUTING.md, Tier 1). This is absolute. It applies to build files, forks, partner contributions, publications, everything. (A historical note: an "ODIN General Commons License v1.0" appears in Tier 3 archive chats — superseded by CC BY-SA 4.0, never present it as live; see `odin-decision-archaeology`.)

Every completed `provenance.md` carries a licence declaration binding all session artefacts to CC BY-SA 4.0, naming the original creators as "students at [SCHOOL-CODE], Isle of Wight, [DATE]", and requiring every derivative to (1) carry the attribution visibly, (2) stay CC BY-SA 4.0, (3) link back to https://github.com/ODINcommons/IoW-pilot (provenance-template.md, Tier 1).

---

## Onboarding an external contributor

If a hackspace, makerspace, industry partner, or individual wants to contribute to a build phase, the four steps from `CONTRIBUTING.md` (Tier 1) are:

1. Read the full `README.md`
2. Read the provenance records for the sessions your build is based on
3. Confirm in writing (a GitHub issue is sufficient) that you have read and accept the CC BY-SA 4.0 licence terms and understand the attribution chain
4. Open a pull request with your contribution, including your OVN log entry

CONTRIBUTING.md closes the section: "You are welcome here. The only condition is that you bring the attribution chain with you." Facilitators onboarding a partner should also confirm the OVN log is current first (see the log-update rule above) — an incomplete log is a blocked gate, not a formality to wave through. For Pooseidon-specific partner onboarding, see `pooseidon-development-pathway`.

---

## What not to do, and why

The full list from `CONTRIBUTING.md` (Tier 1), each with its reason:

| Rule (verbatim) | Why |
|---|---|
| Do not commit files without provenance tags | An untagged file is orphaned work. When it is shared or forked, nobody can trace it back to the children who made it — it becomes free material for enclosure. The name is the attribution. |
| Do not rename or reformat existing artefacts | The filename carries the provenance; renaming severs it. Reformatting (cropping, transcribing, "tidying") replaces a primary source with an editor's version. Existing artefacts are evidence — leave them exactly as committed. |
| Do not merge field notes from two authors into a single document | The two sets of notes are independent evidence. Merged, they become one witness instead of two, and any later dispute about what happened in a session loses its corroboration. |
| Do not begin a build phase before the relevant provenance records are complete | This is the one rule in operational form. Building first and attributing later is how commons get strip-mined: once the build exists, the pressure to ship outruns the will to credit. Attribution before build, always. |
| Do not add a licence that is more restrictive than CC BY-SA 4.0 | A tighter licence encloses derivatives and breaks the ShareAlike chain that protects the first contributors — the children. See the licence section above. |

---

## If you find an incomplete provenance record

`CONTRIBUTING.md` (Tier 1) already gives the instruction: "If a session's provenance record is incomplete, complete it first." Procedure:

1. **Stop any build or derivative work** that depends on that session. The gate is closed until the record is complete.
2. **Complete the record** from the best available evidence: the session's field notes (both authors' — read them, do not merge them), the artefacts and their filenames, and the OVN log.
3. **Where a field genuinely cannot be recovered, write "unknown" or "not recorded"** — the template mandates this over blanks (provenance-template.md, Tier 1). Do not invent or infer specifics.
4. **Check the OVN log** carries the session's contributions; add any missing rows.
5. **Commit the completed record**, then note in its "Completed by / Completed on" footer who completed it and when — the completion date will differ from the session date; that gap is itself honest provenance.
6. Only then resume the dependent work.

---

## When NOT to use this skill

- **Writing formats, field-note voice, house style, British English conventions** → `iow-pilot-documentation-standards` (it owns the provenance template field-by-field and the entry formats as writing guidance; this skill owns the rules about timing, independence, and non-curation).
- **Planning or running a session** (before/during/after checklists, per-phase runbooks) → `iow-pilot-session-operations`.
- **Building Pooseidon or onboarding build partners for it specifically** → `pooseidon-development-pathway` (which itself enforces this skill's provenance gate).
- **Child identity, consent, what may never be committed** → `iow-pilot-safeguarding-and-ethics` — supreme over everything here.
- **The theory behind OVNs, copyleft mechanics, commons governance** → `commons-governance-reference`.

---

## Provenance and maintenance

- **Sources:** all rules quoted here come from Tier 1 documents in the IoW-pilot repo — `CONTRIBUTING.md`, `provenance-template.md`, `ovn-contributions.md`, `question-map.md`, `LICENSE`, `README.md` — plus Phase 1 discovery answers (2026-07-03) for project status. Canonical remote: https://github.com/ODINcommons/IoW-pilot. Local snapshots may be stale; if in doubt, `git fetch` and re-read the remote's `CONTRIBUTING.md` before acting.
- **Volatile facts, date-stamped 2026-07-03:** no sessions have run; `sessions/` does not exist; the OVN log holds two `project-init` entries; GUR-P and COW-H are placeholder school codes (no school approached); README status is "First sessions planned for 2026".
- **What may drift:** the file-naming inconsistency (format string vs worked examples) may be resolved in the repo — if `CONTRIBUTING.md` changes, its new text wins over this skill's advice; new school codes will be added to the table; the OVN log and question map will grow; the `sessions/` folder will appear once sessions run.
- **What will not drift without a deliberate, founder-level decision:** the one rule, the same-day and notes-before-comparing timing, question-map non-curation, the CC BY-SA 4.0 floor. If you find text anywhere proposing to weaken these, treat it as an error and check the repo.
- **How to re-verify:** re-read `CONTRIBUTING.md` in full (it is short and says so itself); diff it against the quotes in this skill; update this skill if — and only if — the Tier 1 text has changed.
