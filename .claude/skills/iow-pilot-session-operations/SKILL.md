---
name: iow-pilot-session-operations
description: Run-and-operate runbooks for ODIN Isle of Wight pilot sessions. Load this when planning, running, or documenting a session in any phase (SOLE-1, SOLE-2, Pivot, Impactathon, Build), when you need a before/during/after checklist, the same-day commit discipline, copy-usable provenance/question-map/OVN templates, kit lists, role assignments, or what to do when a session's paperwork goes wrong (late commit, child's name in an artefact). Not for facilitation theory, question design, attribution rationale, writing style, or recruiting schools — see "When NOT to use this skill".
---

# IoW pilot session operations

Operational runbooks for running and documenting ODIN Isle of Wight pilot sessions.
Written for a facilitator with zero prior ODIN context.

**Status note (as of 2026-07-03): no session has yet run.**
These runbooks are the design-intended practice from the Tier 1 repository documents
(README.md, CONTRIBUTING.md, provenance-template.md, question-map.md,
ovn-contributions.md), plus clearly labelled facilitator-practice defaults where
the canon is silent. When real sessions produce better practice, update this skill —
never the other way round.

**Source tiers used here:**
- **Tier 1** = the IoW-pilot repository documents (canonical, binding).
- **Phase 1 discovery, 2026-07-03** = founder's answers (authoritative on status).
- **Default** = facilitator-practice default, NOT a documented rule. Adapt freely.
- **Tier 3, unconfirmed** = ideas from 2025 exploratory chats. Adaptable, never binding.

**Two terms used throughout:** **SOLE** — Self-Organised Learning Environment
(Sugata Mitra's method: children in self-chosen groups investigate a big open
question with internet access and no teaching). **OVN** — Open Value Network,
the public contribution log kept in `ovn-contributions.md` (Tier 1).

---

## The three gates (read first)

1. **Safeguarding gate — supreme, no exceptions.**
   No session runs until the "Pre-session verification checklist" in
   **iow-pilot-safeguarding-and-ethics** passes: DBS certificates in hand for
   both adults, consent coverage, school agreement, policy read, DSL known.
   As of 2026-07-03 nothing formal exists yet (Phase 1 discovery, 2026-07-03).
   Safeguarding outranks everything in this skill, including attribution.

2. **The one rule: "Everything gets attributed before it gets built."**
   (CONTRIBUTING.md, Tier 1.) No build work starts on any session artefact
   until that session's provenance record is complete, public, and current.

3. **The same-day rule.**
   `provenance.md` is committed **the same day as the session**.
   Field notes are committed **before the two authors compare notes**.
   (CONTRIBUTING.md, Tier 1.)

---

## Phase map

The README (Tier 1) defines a 4-phase pilot sequence. The phase *codes*
(CONTRIBUTING.md, Tier 1) split Phase 1 into two sessions:

| README phase | Session code(s) | What it is (README, Tier 1) |
|---|---|---|
| Phase 1: SOLE sessions | `SOLE-1`, `SOLE-2` | Self-organised learning across age bands 5–7, 7–11, 11–14, 14–16. Opening question: water. No curriculum, no assessment, no predetermined answers. |
| Phase 2: Pivot | `Pivot` | Groups return to a shared Question Map assembled from Phase 1. New question: what are the water-related problems we face here, and what could we do about them? |
| Phase 3: Impactathon | `Impactathon` | Mixed-age, mixed-school teams design real responses to real problems. Designs documented, published, and attributed the same day. |
| Phase 4: Prototype | `Build` | Most viable design moves to build, with local industry, hackspaces, open hardware networks. All build files committed under CC BY-SA 4.0. |

SOLE theory and question design live in **sole-facilitation-reference**.

---

## Universal session shape (all phases)

The provenance template (Tier 1) structures every session in three phases and
gives "e.g. 90 minutes" as its duration example. That is the only duration
guidance in canon.

**Default (facilitator practice, not a rule): 90 minutes total —**
- Early phase: first 15 minutes — pose the question, groups self-organise.
- Middle phase: 15–60 minutes — self-organised inquiry. Facilitator stays out.
- Closing: final 15–20 minutes — groups share back; documentarian captures.

These three phase headings come straight from the template's "What happened"
section (provenance-template.md, Tier 1) — your field notes must fill them,
so run the session in that shape.

**Two people, always (default, grounded in Tier 1 structure):**
- **Facilitator** — poses the question, holds the room, does NOT answer questions.
- **Co-facilitator / documentarian** — captures everything (see During, below).

Two people because the session folder requires `field-notes-facilitator.md`
AND `field-notes-cofacilitator.md` (README structure, Tier 1), and the two must
be independently authored — committed before comparing, never merged
(CONTRIBUTING.md, Tier 1). One person cannot produce two independent accounts.

---

## BEFORE the session — checklist

Work through in order. **Item 1 is a hard gate.**

- [ ] **1. Safeguarding gate passes.** Verified with the school:
      consent state confirmed, DBS certificates in hand for both adults,
      school safeguarding agreement live, school staff present throughout.
      Full checklist: the "Pre-session verification checklist" in
      **iow-pilot-safeguarding-and-ethics**. **If this fails, stop. No session.**
- [ ] **2. Roles assigned.** One facilitator, one co-facilitator/documentarian.
      Confirm both understand: facilitator never answers content questions;
      documentarian captures verbatim; field notes stay independent.
- [ ] **3. Opening question chosen** for the age band.
      Question design and age-band logic: **sole-facilitation-reference**.
      The designed openers on record (question-map.md, Tier 1):
      - 7–11: "Could we live without water?"
      - 14–16: "Who owns the water?"
      - 5–7 benchmark (anticipated emergent, not an opener): "Can water get sick?"
- [ ] **4. Hypothesis logged before the session** if you expect a designed seed
      question to emerge naturally — write the expectation down (commit or
      timestamp it) BEFORE the session, or the finding doesn't count
      (Phase 1 discovery success bar, 2026-07-03; method detail in
      **odin-research-methodology**).
- [ ] **5. Session folder pre-created** from the template (see next section).
- [ ] **6. Kit packed** (see kit list below).
- [ ] **7. Practicalities confirmed with school:** room (classroom / hall /
      outdoor — the template asks for location), start time, group size,
      year group(s), which teacher will be present.

### Pre-create the session folder — locally only

Create the folder **locally, before the day — do not commit or push any of it
until the after-session checklist**. Committing before the session would put
files without provenance into the public repo ("Do not commit files without
provenance tags" — CONTRIBUTING.md what-not-to-do, Tier 1), publicly assert a
session that has not happened, and announce in advance that a named school's
year group will be in a session on a named date. The commit happens same-day
**after** the session, never before.

The local folder shape:

```
sessions/
└── [SCHOOL-CODE]-[YYYY-MM-DD]-[PHASE]/
    ├── provenance.md              ← copied from provenance-template.md, blank
    ├── field-notes-facilitator.md ← empty stub
    ├── field-notes-cofacilitator.md ← empty stub
    └── artefacts/                 ← empty
```

(README structure + CONTRIBUTING.md session-folder example, Tier 1.
The `sessions/` folder does not exist in the repo yet as of 2026-07-03 —
the first session creates it.)

**School codes** (CONTRIBUTING.md, Tier 1): `GUR-P` (Gurnard Primary),
`COW-H` (Cowes High), "(add as needed)".
**Caution:** as of 2026-07-03 these are PLACEHOLDER examples — no real school
has been approached (Phase 1 discovery, 2026-07-03). Add your real school's
code to the CONTRIBUTING.md table when one signs up.

### File naming — one-line reminder

Format (CONTRIBUTING.md, Tier 1):

```
[SCHOOL-CODE]-[YYYY-MM-DD]-[PHASE]-[NNN]-[description].[ext]
```

Phase codes: `SOLE-1` / `SOLE-2` / `Pivot` / `Impactathon` / `Build`.
**Follow the explicit format string, not CONTRIBUTING.md's worked examples**
(the two disagree — full note on the inconsistency:
**iow-pilot-documentation-standards**). Never rename existing repo files
(CONTRIBUTING.md what-not-to-do, Tier 1).

### Kit list

**Default (facilitator practice). Tier-3 items marked — unconfirmed 2025 chat
ideas, adapt to what the school has.**

- [ ] Internet-connected devices, ~1 per group of 4–5 — tablets or school
      laptops *(Tier 3, unconfirmed, 2025 chats; SOLE method needs group
      internet access)*
- [ ] Large paper / flipchart pads, 2+ sheets per group *(Tier 3, unconfirmed)*
- [ ] Marker pens / sharpies, mixed colours *(Tier 3, unconfirmed)*
- [ ] Camera or phone for artefact capture (documentarian's — check the
      school's photography policy first; see **iow-pilot-safeguarding-and-ethics**)
- [ ] Notebook or laptop for the documentarian's verbatim question log with times
- [ ] A visible clock or timer
- [ ] Printed copy of the opening question (optional, default)
- [ ] Printed blank provenance record as a capture aid (optional, default)

---

## DURING the session — capture protocol

### Facilitator
- Pose the opening question exactly as planned. The provenance record asks for
  it "exactly as it was spoken to the group" (provenance-template.md, Tier 1) —
  so speak it deliberately and note any deviation.
- Then get out of the way. Groups self-organise. **Do not answer questions.**
  No curriculum, no assessment, no predetermined answers (README, Tier 1).
  How to deflect gracefully: **sole-facilitation-reference**.
- Watch for: how groups form, unexpected directions, moments of difficulty,
  surprises — the template's "What happened" section asks for exactly these
  (provenance-template.md, Tier 1).

### Co-facilitator / documentarian
Capture, in real time:

1. **Questions verbatim** — every significant question participants produce,
   word for word, tagged with **group** (e.g. Group 2, Y5) and **approximate
   time** it emerged. This feeds the template's emergent-questions table
   directly (provenance-template.md, Tier 1). Verbatim means verbatim —
   the question map "does not improve questions into more sensible versions"
   (question-map.md, Tier 1).
2. **Artefacts** — photograph or collect everything groups produce
   (drawings, notes, flipchart sheets). Note which group/year made each one.
   **Check nothing identifying is in frame — no faces, no names**
   (safeguarding, Tier 1 child-ID rule; see failure branch below).
3. **What actually happened** — running notes in the three template phases:
   early (first 15 min), middle (15–60 min), closing (final 15–20 min).
   Honest, colleague-voice, not polished (provenance-template.md, Tier 1).

**Default:** timestamp your notes as you go — approximate times are a required
column and memory reconstructs badly.

Both adults keep their own notes. **Do not compare or co-write during the
session** — independence is the point (CONTRIBUTING.md, Tier 1).

---

## AFTER the session — the same-day discipline

Same day. Not "soon". Same day (CONTRIBUTING.md, Tier 1).

### End-of-day checklist (copy-usable)

- [ ] **1. Both authors write up field notes separately** —
      `field-notes-facilitator.md` and `field-notes-cofacilitator.md`.
- [ ] **2. Both field notes committed BEFORE the authors compare notes.**
      Never merge the two into one document (CONTRIBUTING.md, Tier 1).
- [ ] **3. Artefacts screened for safeguarding** — no names, faces, or
      identifying details. Crop or exclude before anything is committed
      (see failure branch below).
- [ ] **4. Artefacts named** per the format string, numbered `-001-` upward,
      placed in `artefacts/`.
- [ ] **5. `provenance.md` completed** — every field. Write "unknown" or
      "not recorded" rather than leaving blanks (provenance-template.md, Tier 1).
      Teacher: anonymised or initials only.
- [ ] **6. New questions added to `question-map.md`** in its exact format
      (below). Add within the "## Questions" section, below existing session
      entries — the seed-questions section stays untouched at the bottom.
      Never edit or rephrase existing questions (CONTRIBUTING.md, Tier 1).
- [ ] **7. OVN rows added to `ovn-contributions.md`** — at minimum:
      children (conceptual), facilitator (facilitation),
      documentarian (documentation). The provenance record's own OVN section
      lists what to carry over (provenance-template.md, Tier 1).
- [ ] **8. Everything committed and pushed** to
      github.com/ODINcommons/IoW-pilot, same day.
- [ ] **9. Only now:** the two authors may compare notes.
- [ ] **10. If a pre-logged hypothesis existed** (seed question), record
      whether it emerged — in provenance notes and question-map Notes.

### Contributor IDs (Tier 1, CONTRIBUTING.md — absolute)
- Children: school code + year group ONLY. `GUR-P-Y5`, `COW-H-Y8`. **Never names.**
- Adults: name or GitHub handle.

---

## Copy-usable templates

### 1. Provenance record

**Copy `provenance-template.md` from the repo root** into the session folder
as `provenance.md` — never retype it, and never add, remove, or rename fields
(provenance-template.md, Tier 1). The template is Tier 1 and may change;
always copy from the repo at HEAD, not from a reproduction (local snapshots
go stale). Field-by-field guidance: **iow-pilot-documentation-standards**.

Its sections, in order, so you know what the day must produce:

1. **Session identity** — school code, school type, date, phase, year
   group(s), participants, duration, general location
2. **People** — facilitator; co-facilitator/documentarian; teacher
   (anonymised or initials only); other adults
3. **The question posed** — exactly as it was spoken to the group
4. **What happened** — early / middle / closing phases, colleague voice
5. **Questions that emerged** — verbatim | group | approx. time
6. **Artefacts produced** — standard filename format
7. **Licence declaration** — CC BY-SA 4.0, attribution, link back
8. **OVN contribution entries** — to carry over to `ovn-contributions.md`

One wrinkle: the template's OVN section lists four contribution types, the
OVN log defines six — full note in **iow-pilot-documentation-standards**.

### 2. Question-map entry format (CONTRIBUTING.md, Tier 1 — exact)

```markdown
## [Question verbatim]
- **Source**: [SCHOOL-CODE], [YEAR-GROUP], [DATE], [PHASE]
- **Disciplines**: [list: e.g. environmental law, microbiology, economics]
- **Related questions**: [link to others in the map if relevant]
- **Notes**: [optional — any context about how it emerged]
```

**Worked micro-example** (illustrative — placeholder school code and date;
no session has run as of 2026-07-03):

```markdown
## Why does the sea smell worse after it rains?
- **Source**: GUR-P, Y5, 2026-09-15, SOLE-1
- **Disciplines**: Chemistry, marine biology, sewage infrastructure, public health
- **Related questions**: Can water get sick?
- **Notes**: Emerged from Group 3 around 40 minutes in, after finding a news
  article about storm overflow discharges. Recorded verbatim.
```

Disciplinary annotation logic: **sole-facilitation-reference**.
Add within the "## Questions" section, below existing session entries (the
seed-questions section stays untouched at the bottom). Never touch existing
entries (CONTRIBUTING.md, Tier 1).

### 3. OVN row format (CONTRIBUTING.md, Tier 1 — exact)

```
| [date] | [contributor ID] | [type] | [session ref] | [description] |
```

Types: `conceptual` / `design` / `fabrication` / `deployment` /
`documentation` / `facilitation` (ovn-contributions.md, Tier 1).

**Worked micro-example** (illustrative — placeholder code and date):

```
| 2026-09-15 | GUR-P-Y5 | conceptual | GUR-P-2026-09-15-SOLE-1 | Questions and ideas generated in session, incl. "Why does the sea smell worse after it rains?" |
| 2026-09-15 | SeaWizard-ODIN | facilitation | GUR-P-2026-09-15-SOLE-1 | Session design and delivery |
| 2026-09-15 | [co-fac name/handle] | documentation | GUR-P-2026-09-15-SOLE-1 | Artefact capture, field notes, provenance record |
```

---

## Per-phase runbooks

Everything in "Universal session shape", BEFORE, DURING, and AFTER applies to
every phase. Below are the phase-specific deltas.

### SOLE-1 (Phase 1, first session)

**Canon (README + question-map.md, Tier 1):** self-organised learning, opening
question on water, no curriculum, no assessment, no predetermined answers.
Age bands 5–7, 7–11, 11–14, 14–16.

- Opening question per age band (see BEFORE, item 3;
  design logic in **sole-facilitation-reference**).
- **Default flow (90 min):** pose question (5 min) → groups self-form,
  4–5 per group around one device (10 min) → inquiry (45 min) →
  share-back, each group presents what they found and what they now want
  to know (20–25 min) → close.
- 5–7 band: watch for the benchmark. If "Can water get sick?" (or close kin)
  emerges naturally, that is the seed-question finding — but only if the
  hypothesis was logged before the session (see BEFORE, item 4).
- Documentarian priority: the emergent-questions table. SOLE-1's questions
  seed the whole Question Map and therefore Phase 2.

### SOLE-2 (Phase 1, second session)

**Canon:** CONTRIBUTING.md (Tier 1) defines the `SOLE-2` code; the README
folds it into Phase 1. No further canonical specification exists.

- **Default:** same group, same shape as SOLE-1. Open either with a deeper
  water question or with a question the group itself produced in SOLE-1
  (read it back verbatim from the Question Map — their words, attributed).
- Purpose (default): depth and continuity — groups pick up their own threads.
- New session folder, new provenance record, new commits. Every session
  stands alone in the archive.

### Pivot (Phase 2)

**Canon (README, Tier 1):** "Groups return to a shared Question Map assembled
from Phase 1. A new question emerges from what they found: what are the
water-related problems we face here, and what could we do about them?"

- **Before (extra):** print or display the Question Map — the actual
  `question-map.md`, questions verbatim, attributions visible. Children
  should see their own questions with their group's mark on them.
- **Default flow:** walk the map together (15 min) → groups cluster
  problems: which of these are OUR problems, here, on the island? (30 min) →
  "what could we do about them?" — capture proposed responses as artefacts
  (30 min) → share-back (15 min).
- Documentarian: proposed problem/response framings are conceptual
  contributions — capture verbatim, attribute by group, log in OVN.
- The Pivot output is the raw material for Impactathon team formation.

### Impactathon (Phase 3)

**Canon (README, Tier 1):** "Mixed-age, mixed-school teams design real
responses to real problems. Designs are documented, published, and attributed
**the same day**."

An impactathon is a mixed-age, mixed-school design event — defined only in
the README (Tier 1).

- **Before (extra):**
  - Multi-school consent and safeguarding: EVERY participating school's
    gate must pass (**iow-pilot-safeguarding-and-ethics**). Mixed-school
    means multiple consent chains.
  - Session ref: the repo's own example uses a cross-school code —
    `IOW-IMPACT-20251115-Impactathon-007-...` (CONTRIBUTING.md, Tier 1).
    Default: use `IOW-IMPACT` as the school-code slot for mixed-school
    events, folder `IOW-IMPACT-[YYYY-MM-DD]-Impactathon`.
  - **Default:** likely longer than 90 minutes — a half-day or full day.
    No canonical duration exists; agree it with the schools.
    Scale documentarians accordingly (default: one per 3–4 teams).
- **During:** design work. Every design artefact photographed/collected with
  its team's composition noted (which schools, which year groups) — the
  producer column and OVN attribution need it. Contribution types shift
  toward `design`.
- **After:** the same-day rule is explicit and doubled here — README says
  designs are "documented, published, and attributed the same day".
  Publish means committed and pushed, publicly, that day.
- Pooseidon note: the buoy network is the founder's PRE-SESSION concept
  (README, Tier 1; status per Phase 1 discovery, 2026-07-03). Do not steer
  teams toward it. If children design something like it — or unlike it —
  **children's designs take precedence**. Rationale:
  **iow-pilot-provenance-and-attribution**; build pathway:
  **pooseidon-development-pathway**.

### Build (Phase 4)

**Canon (README, Tier 1):** "The most viable design moves into a build phase,
in partnership with local industry, hackspaces, and open hardware networks.
All build files are committed here under CC BY-SA 4.0."

Build is a phase of work, not a single 90-minute session. What this skill
covers: the operational gates and logging. What it doesn't: partner
onboarding detail (**pooseidon-development-pathway**), attribution rationale
(**iow-pilot-provenance-and-attribution**).

- **Gate (hard, Tier 1):** "Do not begin a build phase before the relevant
  provenance records are complete" (CONTRIBUTING.md what-not-to-do list).
  Verify every source session's `provenance.md` is complete, public, current.
  If incomplete: complete it first — that is the documented remedy
  (CONTRIBUTING.md, Tier 1).
- External partners join via the documented route (CONTRIBUTING.md, Tier 1):
  read README → read the relevant provenance records → confirm in writing
  (GitHub issue suffices) acceptance of CC BY-SA 4.0 and the attribution
  chain → pull request including their own OVN log entry.
- Build files: named per the format string, phase code `Build`, committed
  under CC BY-SA 4.0. Never a more restrictive licence (CONTRIBUTING.md, Tier 1).
- OVN types now in play: `fabrication`, `deployment` — plus `design` and
  `documentation`. Log every contribution.
- **Default:** for build "sessions" with children present, the full
  before/during/after discipline above applies unchanged, including
  safeguarding and same-day provenance.

---

## Failure branches

### You cannot commit same day

(No internet at the venue, repo access failure, emergency.)

1. Write everything anyway, locally, same day — field notes, completed
   provenance record, named artefacts. The writing discipline is same-day
   even when the commit physically cannot be.
2. Do NOT compare field notes until both are committed. The
   before-comparing rule (CONTRIBUTING.md, Tier 1) still holds — the delay
   does not license an early comparison.
3. Commit at the first opportunity.
4. Record the delay honestly in `provenance.md` — e.g. in the completion
   footer: "Completed on: 2026-09-15 (session day); committed 2026-09-17 —
   no repo access at venue." Never backdate, never pretend.
   Honest records beat tidy ones — the template demands "not recorded"
   over blank fields for the same reason (provenance-template.md, Tier 1).

### A child's name (or face, or identifying detail) appears in an artefact

**Safeguarding outranks completeness. Always.** (Discovery brief §4;
child-ID rule in CONTRIBUTING.md, Tier 1.)

1. Do not commit it as-is. Ever.
2. Crop or edit the copy so the identifying detail is gone, OR exclude the
   artefact entirely if it cannot be cleaned.
3. In the provenance artefact table, log honestly: e.g.
   "GUR-P-2026-09-15-SOLE-1-004: cropped before commit to remove a
   pupil's name" or "one artefact excluded — identifying content".
4. If an identifying artefact was already pushed: treat as a live
   safeguarding incident — follow the "Incident procedure — an identifying
   artefact has been pushed to the public repo" in
   **iow-pilot-safeguarding-and-ethics** immediately (same-day purge from
   git history, DSL and steward notification, honest record). Do not
   quietly fix and move on.
5. Attribution survives: the group + year group ID (`GUR-P-Y5`) carries the
   credit. Names were never the attribution mechanism for children.

---

## When NOT to use this skill

| You need | Go to |
|---|---|
| SOLE facilitation theory, age-band question design, seed-question benchmark logic, disciplinary annotations | **sole-facilitation-reference** |
| Why attribution works this way, the one rule's rationale, licence reasoning, external onboarding detail | **iow-pilot-provenance-and-attribution** |
| Consent, DBS, child-ID rules, what may never be committed, incident handling | **iow-pilot-safeguarding-and-ethics** |
| Writing voice, template field-by-field guidance, house style, naming-format detail | **iow-pilot-documentation-standards** |
| Getting schools to yes — recruitment, gates, campaign sequence | **iow-pilot-launch-campaign** |
| Pooseidon build pathway, partner onboarding, sensing domain | **pooseidon-development-pathway** |
| Hypothesis-before-session methodology, artefacts as primary sources | **odin-research-methodology** |

---

## Provenance and maintenance

**Sources for this skill:**
- Tier 1: `README.md` (phase sequence, session-folder structure, Pooseidon,
  status line), `CONTRIBUTING.md` (one rule, naming format + phase codes,
  same-day and before-comparing rules, question-map format, OVN format,
  contributor IDs, external onboarding, what-not-to-do list),
  `provenance-template.md` (all fields, session phases, duration example),
  `question-map.md` (seed questions, non-curation), `ovn-contributions.md`
  (six contribution types, row format) — all at github.com/ODINcommons/IoW-pilot.
- Phase 1 discovery, 2026-07-03: no sessions run; no safeguarding formalised;
  GUR-P/COW-H are placeholders; seed-question hypothesis-before-session
  success criterion.
- Facilitator-practice defaults and Tier-3 kit ideas (2025 chats,
  unconfirmed) are labelled inline and carry no authority.

**What may drift — re-verify before relying on this skill:**
- **"No session has run" (as of 2026-07-03).** Check for a `sessions/` folder
  at github.com/ODINcommons/IoW-pilot — its existence means sessions have
  started and real practice may have superseded these defaults.
- **School codes.** The CONTRIBUTING.md table may hold real schools by now.
- **The naming-format inconsistency.** May be resolved in a later
  CONTRIBUTING.md — re-read it and follow whatever the current format string says.
- **Safeguarding status.** Was "nothing formal" at Phase 1 discovery;
  will change — **iow-pilot-safeguarding-and-ethics** owns the current state.
- **Session duration and kit defaults.** Replace with observed practice after
  the first real sessions; update this skill when you do.
- Local snapshots may be stale — the GitHub repo is canonical.

*This skill is licensed under CC BY-SA 4.0, like everything else here.
Fork it, adapt it, carry the attribution.*
