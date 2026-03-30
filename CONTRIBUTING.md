# Contributing to the ODIN Isle of Wight Pilot

This document explains how to contribute to this repository — whether you are a
session facilitator, a collaborator joining a build phase, a hackspace member
picking up a design, or anyone else who wants to work with or build on what's here.

Read this before you commit anything. It is short.

---

## The one rule that matters most

**Everything gets attributed before it gets built.**

The intellectual work in this repository originated with children in state schools
on the Isle of Wight. Before any external contributor — individual, organisation,
or institution — begins building on that work, the provenance record must be
complete, public, and current. Check `sessions/` and `ovn-contributions.md` before
you start. If a session's provenance record is incomplete, complete it first.

---

## Licence

All content in this repository is licensed under
**Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**.

This means:
- You may use, share, and adapt any content here
- You must credit the original creators (see provenance records)
- You must release any derivative work under the same licence
- You may not add legal restrictions that prevent others from doing the same

This is the copyleft of the commons. It protects everyone who contributed,
especially those who contributed first.

Full licence text: https://creativecommons.org/licenses/by-sa/4.0/

---

## File naming convention

Every file committed to this repository follows this format:

```
[SCHOOL-CODE]-[YYYY-MM-DD]-[PHASE]-[NNN]-[description].[ext]
```

**Examples:**
```
GUR-P-20250915-SOLE1-001-water-questions-group2.jpg
GUR-P-20250915-SOLE1-002-buoy-drawing-annotated.jpg
COW-H-20251003-Pivot-001-field-notes-facilitator.md
IOW-IMPACT-20251115-Impactathon-007-pooseidon-alert-system-design.jpg
```

**School codes:**
| School | Code |
|---|---|
| Gurnard Primary | GUR-P |
| Cowes High | COW-H |
| (add as needed) | |

**Phase codes:**
| Phase | Code |
|---|---|
| First SOLE session | SOLE-1 |
| Second SOLE session | SOLE-2 |
| Pivot session | Pivot |
| Impactathon | Impactathon |
| Build / prototype | Build |

**Why this matters:** A correctly named file is self-describing. Its provenance
travels with it when it is shared, forked, posted, or emailed. The name is
the attribution.

---

## Session folder structure

Each session gets its own folder:

```
sessions/
└── GUR-P-2025-09-15-SOLE-1/
    ├── provenance.md              ← completed from provenance-template.md
    ├── field-notes-facilitator.md
    ├── field-notes-cofacilitator.md
    └── artefacts/
        └── [named files]
```

The `provenance.md` must be committed **the same day as the session**.
Field notes must be committed **before the two authors compare notes**.

---

## How to add to the question map

Open `question-map.md` and add any new questions from your session using
this format:

```markdown
## [Question verbatim]
- **Source**: [SCHOOL-CODE], [YEAR-GROUP], [DATE], [PHASE]
- **Disciplines**: [list: e.g. environmental law, microbiology, economics]
- **Related questions**: [link to others in the map if relevant]
- **Notes**: [optional — any context about how it emerged]
```

Do not edit or rephrase existing questions. Add new ones below existing entries.
The map is a record, not a curated document.

---

## How to log an OVN contribution

Open `ovn-contributions.md` and add a row to the table:

```
| [date] | [contributor ID] | [type] | [session ref] | [description] |
```

Contribution types: `conceptual` / `design` / `fabrication` /
`deployment` / `documentation` / `facilitation`

Contributor IDs for children use school code + year group only (no names):
`GUR-P-Y5`, `COW-H-Y8` etc.

Adult contributors use their name or GitHub handle.

---

## How to join as an external contributor

If you are a hackspace, makerspace, industry partner, or individual who wants
to contribute to a build phase:

1. Read the full `README.md`
2. Read the provenance records for the sessions your build is based on
3. Confirm in writing (a GitHub issue is sufficient) that you have read and
   accept the CC BY-SA 4.0 licence terms and understand the attribution chain
4. Open a pull request with your contribution, including your OVN log entry

You are welcome here. The only condition is that you bring the attribution
chain with you.

---

## What not to do

- Do not commit files without provenance tags
- Do not rename or reformat existing artefacts
- Do not merge field notes from two authors into a single document
- Do not begin a build phase before the relevant provenance records are complete
- Do not add a licence that is more restrictive than CC BY-SA 4.0

---

*This document is itself licensed under CC BY-SA 4.0.*
*Fork it, adapt it, use it for your own commons project.*
*Just carry the attribution.*
