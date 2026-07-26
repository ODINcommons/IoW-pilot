---
name: iow-pilot-launch-campaign
description: >
  The executable, decision-gated campaign for getting the first SOLE sessions
  running in Isle of Wight schools, starting from absolute zero (no school
  contacted, no DBS, no consent materials, no session run). Load this skill when
  you need to know WHAT TO DO NEXT to launch the pilot: choosing and approaching
  schools, obtaining safeguarding clearance, securing consent, scheduling the
  first session, and confirming the same-day archive. Contains gate-by-gate
  checklists, expected observations, and branch decisions for common school
  responses. Do NOT use this skill for the detailed rules themselves — for
  safeguarding rules use iow-pilot-safeguarding-and-ethics; for running the
  session on the day use iow-pilot-session-operations; for SOLE method and
  question design use sole-facilitation-reference; for what you may claim
  externally use odin-external-positioning.
---

# IoW Pilot Launch Campaign

**A numbered, gated campaign from zero to the first archived SOLE session.**

This is the skill for the hardest live problem in the pilot: nothing has
happened yet, and someone — possibly you, a facilitator with no ODIN history —
has to make it happen. Every phase below is a gate. You do not pass a gate on
hope, enthusiasm, or an AI telling you it's done. You pass it when the
**expected observations** for that gate are true in the world and you can point
at the evidence.

## When to use this skill — and when not to

Use this skill when you are deciding **what to do next** to get sessions
running, or checking whether a gate has genuinely passed.

Do **not** use this skill for:

| Need | Use instead |
|---|---|
| Safeguarding rules, child ID rules, consent doctrine in depth | `iow-pilot-safeguarding-and-ethics` |
| Running the session itself (before/during/after runbooks) | `iow-pilot-session-operations` |
| SOLE method, age-band question design, seed-question logic | `sole-facilitation-reference` |
| Provenance, attribution, OVN logging mechanics | `iow-pilot-provenance-and-attribution` |
| What may be claimed to schools, funders, or the public | `odin-external-positioning` |
| Anything about building Pooseidon | `pooseidon-development-pathway` |

**Definitions (first use):** a **SOLE** is a Self-Organised Learning Environment
(Sugata Mitra's method): children in small self-chosen groups investigate a big
open question with internet access and no teaching. **DBS** is the UK
Disclosure and Barring Service criminal-record check; the **enhanced** DBS is
the level normally required for adults working with children. **Provenance
record** means a completed `provenance.md` per the repo's
`provenance-template.md` (Tier 1). **OVN** is Open Value Network — the
contribution log in `ovn-contributions.md` (Tier 1).

---

## Starting state — as of 2026-07-03, stated bluntly

Every item below is from the founder's Phase 1 answers (cite as "Phase 1
discovery, 2026-07-03") or Tier 1 repo documents. Do not assume any of it has
improved without re-verifying (see Provenance and maintenance, at the end).

- **No school has been contacted.** Gurnard Primary (GUR-P) and Cowes High
  (COW-H) appear in CONTRIBUTING.md's naming examples as **placeholder codes
  only** — no real school has been approached. Real prospects must be chosen
  afresh. (Phase 1 discovery, 2026-07-03.)
- **No safeguarding infrastructure exists.** No DBS check held, no consent
  forms, no school safeguarding agreement. All must be built before any
  session. (Phase 1 discovery, 2026-07-03.)
- **No session has run.** README status: "First sessions planned for 2026"
  (Tier 1). The `sessions/` folder does not yet exist in the repo. The
  question map's only entries are three pre-session seed questions
  (question-map.md, Tier 1).
- **The repo and templates are ready.** README, CONTRIBUTING.md,
  provenance-template.md, question-map.md, ovn-contributions.md, and the
  CC BY-SA 4.0 licence are all in place and in sync with
  github.com/ODINcommons/IoW-pilot (verified 2026-07-03).
- **Facilitator capacity is a real constraint.** The founder's own capacity is
  a named blocker (Phase 1 discovery, 2026-07-03). This campaign is therefore
  designed so that **every gate decomposes into tasks completable in
  30–90 minute time-boxes**. Never plan a step that needs a free week; plan
  steps that fit an evening.

**The whole campaign in one sentence:** build the safeguarding foundation
(Gate 0), get one real school to say yes (Gate 1), clear and consent through
that school's own processes (Gate 2), design the session (Gate 3), run it
(Gate 4), archive it the same day (Gate 5).

Gates 0 and 1 can run **in parallel** — DBS processing takes weeks, so start
it while doing school outreach. Gates 2 onwards are strictly sequential.

---

## Gate 0 — Safeguarding foundation

**Objective:** the minimum safeguarding kit exists before any child is in the
room. Safeguarding outranks everything, including attribution
(cross-ref `iow-pilot-safeguarding-and-ethics` for the full four-layer picture:
documented Tier-1 rules, PhD-proposal doctrine, sector practice to verify, and
what remains to be built).

### Tasks (each a 30–90 minute time-box)

- [ ] **0.1 — Start the enhanced DBS application.** An enhanced DBS check is
  **standard UK sector practice for adults working with children — stated here
  as general knowledge, to be verified with the school** (labelled per the
  Phase 1 safeguarding ground rules). An individual cannot usually apply for
  an enhanced check directly; it is requested by an employer or an **umbrella
  body** (a registered organisation that processes checks for smaller groups —
  again, sector practice to verify). See the branch below.
- [ ] **0.2 — Draft the parent/guardian consent letter.** One page. It must
  say, in plain words: what a SOLE session is; that the session is run under
  the school's own safeguarding policy with school staff present; that no
  child's name, face, or identifying detail will ever appear in the public
  archive (children are identified as school code + year group only, e.g.
  `GUR-P-Y5` — CONTRIBUTING.md, Tier 1); that children's questions and drawings
  may be published anonymously under CC BY-SA 4.0 (LICENSE, Tier 1); and that
  a child without consent still takes part in the session as normal but
  nothing they produce enters the archive.
- [ ] **0.3 — Draft the school-facing safeguarding statement.** One page,
  head-teacher audience. It commits ODIN to: working entirely under the host
  school's safeguarding policy; school staff always present and holding
  safeguarding duty (sector practice, to verify with the school); enhanced DBS
  for every ODIN adult; the anonymisation contract (school code + year group
  only; no names, no faces, no identifying detail in the archive — 
  CONTRIBUTING.md and provenance-template.md, Tier 1, which requires teachers
  "anonymised or initials only").
- [ ] **0.4 — Decide the two-adult staffing model.** The provenance template
  (Tier 1) requires both a **Facilitator** and a **Co-facilitator /
  documentarian**, and CONTRIBUTING.md (Tier 1) requires field notes from two
  authors, committed before they compare. So the staffing minimum is: two
  DBS-checked ODIN adults **plus** school staff present. Name the second
  adult now, or name recruiting one as the blocking task. Never plan a
  one-adult session — it fails both the documentation rules and ordinary
  safeguarding prudence.

### Expected observations — Gate 0 passes when ALL are true

| # | Observation | Evidence |
|---|---|---|
| 0-A | Enhanced DBS certificate physically in hand for the facilitator; second adult's certificate in hand, or their application demonstrably in progress — **provisional pass for planning sequencing only.** An in-progress application is never clearance: **no session is signed off (Gate 3) or delivered (Gate 4) until enhanced DBS certificates are physically in hand for BOTH ODIN adults. This is absolute.** | The certificates themselves, with issue dates |
| 0-B | Consent letter drafted | The document exists (draft status is fine until Gate 2 tailors it to the school) |
| 0-C | School-facing safeguarding statement drafted | The document exists |
| 0-D | Two-adult model decided; second adult named or recruitment named as the blocker | A written note of who, or of the gap |

### Branches

- **DBS routing unclear (no employer, no obvious umbrella body):** do not
  stall. Move Gate 1 forward and **ask the first interested school** whether
  they will process the DBS check themselves or can recommend the umbrella
  body they use. Schools handle this routinely (sector practice, to verify).
  This is a legitimate reason for Gate 0-A to complete *after* Gate 1 opens —
  but never after Gate 2 closes.
- **DBS delayed but a school is ready:** the session date waits. No session
  before Gate 0 passes. No exceptions (see Fenced wrong paths).

---

## Gate 1 — School engagement from zero

**Objective:** one real Isle of Wight state school, one named contact, one
meeting.

Remember: **GUR-P and COW-H are placeholders** (Phase 1 discovery,
2026-07-03). Choosing real schools is a fresh decision. When a real school
signs up, add its real code to the CONTRIBUTING.md school-code table via
normal contribution process — do not reuse a placeholder code for a different
real school.

### Tasks (each a 30–90 minute time-box)

- [ ] **1.1 — Build the shortlist.** 5–8 Isle of Wight **state** primaries and
  secondaries (the pilot is explicitly for state schools "underserved by
  conventional innovation programmes" — README, Tier 1). For each: school
  name, head/deputy head name, contact email/phone, age range, any warm
  connection (parent, governor, community link — warm beats cold). Public
  sources: school websites, the local authority's school directory.
- [ ] **1.2 — Write the one-page school offer.** It must contain, honestly:
  - **What this is** — one plain sentence stating the pilot's identity, up
    front: "a community conducting research on itself, with open tools, for
    shared benefit, with everything documented and attributed in public"
    (README, Tier 1). The school and its pupils are **credited
    co-researchers** whose questions and designs enter a public commons under
    their cohort ID — not recipients of a programme delivered by an
    institution, and never subjects of research conducted *on* them (README
    "This is not", Tier 1). The co-research identity belongs in the offer,
    not discovered later.
  - **What a SOLE session is** — one paragraph, plain language
    (cross-ref `sole-facilitation-reference`).
  - **What the school gets** — a free, safeguarding-compliant enrichment
    session; a public, attributed record of their pupils' thinking; the
    growing question map as a shareable artefact evidencing their pupils'
    cross-curricular curiosity (question-map.md, Tier 1); connection to a
    documented commons project on a real local issue (coastal water quality —
    README, Tier 1).
  - **What ODIN never does** — no assessment data, no predetermined curriculum
    outcomes, no cost to the school. "No curriculum,no sssessment, no
    predetermined answers" [sic — the README's own typos; quote verbatim if
    quoting] is the pilot's own definition (README Phase 1
    description, Tier 1). Putting the red lines *in the offer* prevents the
    awkward conversation later.
  - **Status stated honestly**: "first sessions planned for 2026" — the
    Tier-1 claim. Nothing stronger (cross-ref `odin-external-positioning`).
- [ ] **1.3 — Approach schools.** Email the head or deputy head directly,
  offer attached, requesting a 20-minute conversation. Two schools per
  time-box. **Log every attempt** (date, school, person, channel, response)
  in a private working note — not in the public repo, since school
  negotiations before agreement are not commons artefacts.
- [ ] **1.4 — Follow up once** after 7–10 days per school, then branch (below).

### Expected observations — Gate 1 passes when ALL are true

| # | Observation | Evidence |
|---|---|---|
| 1-A | At least one reply from a shortlisted school | The email/call log |
| 1-B | A meeting held (or firmly scheduled) with head/deputy or their delegate | Calendar entry, meeting notes |
| 1-C | A named school contact who has agreed in principle to host a first SOLE session | Their name and role, in writing (email is fine) |

### Branches

- **School asks for curriculum alignment:** explain, warmly and without
  apology, that the method forbids predetermined outcomes — that is the point
  (README, Tier 1: no curriculum, no assessment, no predetermined answers —
  restated; the README sentence contains its own typos, see task 1.2).
  But show them the question map: a 9-year-old asking "can water get sick?" is
  simultaneously touching environmental law, microbiology, philosophy of
  rights, and political economy (question-map.md, Tier 1;
  cross-ref `sole-facilitation-reference`). **Until sessions have run, tell
  the school plainly that the map's current entries are designed seed
  questions from the project design phase — not questions children have
  asked.** The 9-year-old in that sentence is the map's own hypothetical;
  the map fills with children's verbatim questions once sessions run. Never
  present seed questions as findings (cross-ref `odin-external-positioning`).
  Offer the growing, annotated
  question map as **the artefact the school receives** — evidence of
  cross-curricular reach without a curriculum. Many schools will accept
  "enrichment" framing where "curriculum" framing fails.
- **School wants assessment or outcome data on pupils:** **decline
  gracefully. This is a red line.** The pilot performs no assessment
  (README, Tier 1) and the archive holds no per-child data of any kind —
  school code + year group only (CONTRIBUTING.md, Tier 1). Offer the question
  map and the public session record instead. If the school cannot proceed
  without assessment data, thank them and move to the next school. Do not
  invent a compromise.
- **Silence after follow-up:** move to the next school on the shortlist. Log
  the attempt and the date. Silence is data, not failure — the log of
  approaches is itself useful to the research record later. **If outreach
  data ever enters the public record, it enters as anonymised aggregates
  (counts, dates, outcomes) — never naming a school that has not signed an
  agreement.**
- **A school says yes enthusiastically but wants to start "next week":**
  wonderful — and the answer is still governed by Gates 0 and 2. Use the
  enthusiasm to accelerate DBS routing (Gate 0 branch) and consent (Gate 2),
  not to skip them.

---

## Gate 2 — Clearance and consent

**Objective:** the legal and ethical basis for the specific session at the
specific school is confirmed, through the **school's own processes**.

The operating principle (sector practice, to verify with the school; see
`iow-pilot-safeguarding-and-ethics`): ODIN works **under the host school's
safeguarding policy**, with school staff present and holding safeguarding
duty. ODIN does not run a parallel safeguarding regime; it plugs into the
school's.

### Tasks (each a 30–90 minute time-box)

- [ ] **2.1 — Safeguarding walkthrough with the school contact.** Confirm:
  who holds safeguarding duty during the session (a school staff member);
  the school's policy applies; DBS evidence they require from ODIN adults;
  their preferred consent route.
- [ ] **2.2 — Consent via school processes.** Tailor the Gate-0 consent letter
  to the school's format and send it through **their** channels (schools
  normally have established parental-consent workflows — sector practice, to
  verify). Do not collect consent forms into ODIN's possession unless the
  school asks; the school holding them is cleaner.
- [ ] **2.3 — Agree the anonymisation contract in writing.** One short
  written exchange (email suffices) confirming with the school: children are
  identified in the public archive by **school code + year group only**
  (e.g. `GUR-P-Y5`); **no names, no faces, no identifying details** ever
  appear (CONTRIBUTING.md, Tier 1); teachers are anonymised or initials only
  (provenance-template.md, Tier 1); artefacts (photos of drawings and
  question sheets, not of children) are published under CC BY-SA 4.0.
- [ ] **2.4 — Confirm consent coverage.** Get the count from the school:
  how many children in the participating class(es) have consent, how many do
  not.

### Expected observations — Gate 2 passes when ALL are true

| # | Observation | Evidence |
|---|---|---|
| 2-A | School has confirmed ODIN adults' DBS status is acceptable to them | Written confirmation from school contact |
| 2-B | Consent letters distributed and returned via school processes | School contact's confirmation + the coverage count |
| 2-C | Anonymisation contract confirmed in writing by the school | The email/exchange |
| 2-D | A named school staff member will be present and holds safeguarding duty | Written confirmation |

### Branches

- **Consent coverage is partial (some children lack consent):** this is
  normal and fine. **Children without consent still participate in the
  session as full class members — they are never excluded from the
  learning.** They are excluded only from the **archive**: no artefact they
  produced, no quote from them, enters the repo. Agree with the teacher
  beforehand how the documentarian will track which groups' outputs are
  archivable (e.g. mark non-archivable group outputs at capture time).
  Record the coverage percentage in the session's provenance context.
  Never exclude a child from learning; only from the archive.
- **School's own paperwork is slow:** the session date moves. Gate 2 must
  pass before Gate 4. No exceptions.

---

## Gate 3 — Session design

**Objective:** the specific session is fully specified before the day.

### Tasks (each a 30–90 minute time-box)

- [ ] **3.1 — Choose the age band and opening question.** The pilot's age
  bands are 5–7, 7–11, 11–14, 14–16 (README, Tier 1). The designed openers in
  question-map.md (Tier 1) are: **"Could we live without water?"** (7–11) and
  **"Who owns the water?"** (14–16). **"Can water get sick?"** (5–7) is the
  **benchmark** question — it is designed to be *watched for*, not posed: if
  it emerges naturally, that confirms the method (question-map.md, Tier 1;
  cross-ref `sole-facilitation-reference` for the reasoning). Match the
  question to the year group the school offered.
- [ ] **3.2 — Log the seed-question hypothesis BEFORE the session.** If the
  session is with the 5–7 band, commit a dated note that the hypothesis
  "'Can water get sick?' will emerge naturally" is held **before** the
  session runs. The Phase-1 success bar explicitly requires the seed-question
  finding to be "logged hypothesis-before-session" (Phase 1 discovery,
  2026-07-03; cross-ref `odin-research-methodology`). A hypothesis logged
  after the fact is worthless.
- [ ] **3.3 — Assign the two adults.** Facilitator + co-facilitator/
  documentarian, **each with their enhanced DBS certificate physically in
  hand — an in-progress application is not clearance. If either certificate
  is missing, Gate 3 does not pass and no session date is confirmed. No
  exceptions.** Both briefed on the
  anonymisation contract and on the field-notes rule: **each writes their own
  field notes and commits them before the two compare** (CONTRIBUTING.md,
  Tier 1).
- [ ] **3.4 — Prepare kit and the session folder.** Per the
  `iow-pilot-session-operations` runbook: devices with internet access, large
  paper, pens, camera for artefacts-not-children, and the session folder
  pre-staged locally as `sessions/[SCHOOL-CODE]-[YYYY-MM-DD]-[PHASE]/` with a
  blank `provenance.md` copied from `provenance-template.md` (README
  structure + CONTRIBUTING.md, Tier 1). Note: the repo's file-naming format
  string and its worked examples disagree on date/phase formatting; follow
  the explicit format string `[SCHOOL-CODE]-[YYYY-MM-DD]-[PHASE]-[NNN]-[description].[ext]`
  and see `iow-pilot-documentation-standards` for the full note. Do not
  silently "fix" the repo.

### Expected observations — Gate 3 passes when ALL are true

| # | Observation | Evidence |
|---|---|---|
| 3-A | Date, year group, room, and duration confirmed with the school | Written confirmation |
| 3-B | Opening question chosen and written down verbatim | The session plan |
| 3-C | If 5–7 band: seed-question hypothesis committed, dated, before the session | The commit, with date |
| 3-D | Both adults confirmed and briefed; enhanced DBS certificates physically in hand for both | Their written confirmation + the certificates |
| 3-E | Kit list checked; session folder pre-staged with blank provenance.md | The folder exists locally |

---

## Gate 4 — Delivery

**Objective:** the session runs.

Run it per the `iow-pilot-session-operations` runbook — that skill owns the
before/during/after detail. The campaign-level rules that must hold:

- [ ] Gate 0 and Gate 2 have **passed in full**, and — as an absolute,
  admitting no provisional pass — **enhanced DBS certificates are physically
  in hand for BOTH ODIN adults**. An in-progress application is not
  clearance. Re-check on the morning of the session against the Pre-session
  verification checklist in `iow-pilot-safeguarding-and-ethics`. If either
  certificate is missing, or consent has regressed, the session does not
  run. No exceptions.
- [ ] School staff member present throughout, holding safeguarding duty.
- [ ] The opening question is posed **exactly as written** in the session
  plan — the provenance record requires "the opening question exactly as it
  was spoken to the group" (provenance-template.md, Tier 1).
- [ ] The documentarian captures artefacts (question sheets, drawings), never
  children's faces or names.
- [ ] Non-consented children participate fully; their outputs are marked
  non-archivable at capture time (Gate 2 branch).

### Expected observations — Gate 4 passes when ALL are true

| # | Observation | Evidence |
|---|---|---|
| 4-A | The session happened, with the planned adults and school staff present | Field notes (two authors) |
| 4-B | Artefacts captured and named per convention | The files |
| 4-C | No safeguarding incident; or if one occurred, it was handled under the school's policy and by the school's duty-holder | School confirmation |

---

## Gate 5 — Same-day archive

**Objective:** the session exists in the commons, correctly, dated today.

This gate is what separates the pilot from every "we ran a workshop once"
project. The rules are Tier 1 and absolute:

- [ ] **5.1 — `provenance.md` completed and committed the same day as the
  session** (CONTRIBUTING.md, Tier 1). Every field completed — "unknown" or
  "not recorded" rather than blank (provenance-template.md, Tier 1).
- [ ] **5.2 — Field notes committed by each author BEFORE the two authors
  compare notes** (CONTRIBUTING.md, Tier 1). Two files, never merged
  (CONTRIBUTING.md what-not-to-do list, Tier 1).
- [ ] **5.3 — Question map updated**: every significant question from the
  session added verbatim, with source, disciplines, related questions
  (question-map.md format in CONTRIBUTING.md, Tier 1). Never edit or
  rephrase existing entries.
- [ ] **5.4 — OVN log updated**: at minimum a `conceptual` entry for the
  children (`[SCHOOL-CODE]-[YEAR-GROUP]`), `facilitation` for the
  facilitator, `documentation` for the co-facilitator
  (CONTRIBUTING.md + provenance-template.md, Tier 1).
- [ ] **5.5 — If the 5–7 benchmark question emerged:** record it verbatim in
  the question map with its source, and note the pre-session hypothesis
  commit (Gate 3.2) in the provenance record's "what happened" narrative.
  This is the seed-question finding (Phase 1 success bar, criterion c).

### Expected observations — Gate 5 passes when ALL are true

| # | Observation | Evidence |
|---|---|---|
| 5-A | The provenance commit exists, **dated the same day as the session** | `git log` — commit date vs session date |
| 5-B | Two field-note files, committed before comparison, never merged | The two files + commit timestamps |
| 5-C | Question map contains the session's questions, verbatim | The diff |
| 5-D | OVN log rows exist for the session | The diff |

### Branch

- **Same-day commit missed** (exhaustion, tech failure): commit at the
  earliest possible moment and record the true dates honestly in the
  provenance record — never backdate, never pretend. Then fix the process
  (e.g. block out the evening after the next session) so it does not recur.
  One late archive is a wound; a pattern of them kills the pilot's core claim.

**After Gate 5:** the loop restarts at Gate 3 (same school, next session:
SOLE-2, then Pivot) or Gate 1 (next school). The pilot's full arc is
SOLE-1 → SOLE-2 → Pivot → Impactathon → Build (README, Tier 1).

---

## Fenced wrong paths — do not go here

| Wrong path | Why it is fenced |
|---|---|
| **Reopening Athens-vs-IoW sequencing** ("should we do Athens first / as well?") | The Athens node is **DEAD** — fenced off, never resurrected without an explicit founder decision (Phase 1 discovery, 2026-07-03). The IoW schools pilot is the settled, current design (Tier 1 repo). Any document suggesting Athens is live is a stale Tier-3 artefact. |
| **Starting to build Pooseidon before sessions have produced attributed designs** | "Everything gets attributed before it gets built" (CONTRIBUTING.md, Tier 1). Pooseidon is a **pre-session concept by the founder** (README, Tier 1; Phase 1 discovery); children's designs, when they exist, take precedence. Building now would make the pilot a product pitch wearing a school visit as a costume. Cross-ref `pooseidon-development-pathway` for the provenance gate. |
| **Promising schools outcomes, curriculum coverage, or assessment data** | The method forbids it: no curriculum, no assessment, no predetermined answers (README, Tier 1 — restated; the source sentence carries its own typos, see task 1.2). A promise you cannot keep at Gate 1 becomes a betrayal at Gate 4. Offer the question map instead (Gate 1 branch). |
| **Running any session before Gate 0 AND Gate 2 have passed, with enhanced DBS certificates physically in hand for BOTH ODIN adults** | No exceptions, ever. An in-progress DBS application is not clearance. Safeguarding outranks everything, including attribution and momentum (Phase 1 safeguarding ground rules; cross-ref `iow-pilot-safeguarding-and-ethics`). An enthusiastic school is not a waiver. |
| **Letting AI-drafted outreach overclaim status** | No "pilot underway", no "sessions running", no "PhD in progress" (the Goldsmiths application was drafted, never submitted — Phase 1 discovery). This project has been burned by AI-asserted status before ("A Goldsmiths PhD is underway…", "The Athens Node is active" — both false, Tier-3 specimens). Every outward claim passes through the claimability gates in `odin-external-positioning`. The honest claim as of 2026-07-03 is: "first sessions planned for 2026" (README, Tier 1). |

---

## Success — measured, never vibes

The Year-1 success bar, verbatim in substance from Phase 1 discovery
(2026-07-03), requires **all four**: (a) sessions run in ≥1 IoW school with
same-day provenance and a growing question map; (b) the full Phase 1→3 arc to
an impactathon with attributed designs; (c) the seed-question finding, logged
hypothesis-before-session; (d) the pilot's data becoming WEAVE's first
real-world trust/deliberation dataset, or a defined and piloted metric
(RPI/AVE — both currently **candidates**, undefined as methods; cross-ref
`weave-research-frontier`).

Track these numbers. Each has an unambiguous source of truth:

| Metric | How measured | Source of truth |
|---|---|---|
| Sessions run | Count of session folders in `sessions/` | The repo |
| Same-day provenance rate | For each session: provenance.md commit date == session date? Report as n-of-m | `git log` |
| Questions in the map | Count of question entries added from sessions (seed questions excluded) | `question-map.md` diff history |
| Consent coverage | Consented children ÷ participating children, per session, as % | School's count, recorded per session |
| Schools engaged | Approached / replied / met / hosting — four counts | The outreach log |
| Seed-question finding | Hypothesis commit date < session date, AND the question appears verbatim in the map | Both commits |
| Phase arc progress | Furthest phase reached: SOLE-1 → SOLE-2 → Pivot → Impactathon → Build | Session folders' phase codes |

If a report about the pilot contains no numbers from this table, it is vibes.
Rewrite it.

---

## Provenance and maintenance

**This skill has the shortest shelf life in the library.** It describes a
starting state ("nothing has happened") that the campaign itself exists to
destroy. **Update this skill after every gate passes** — rewrite the starting
state, mark the gate passed with its evidence and date, and prune branches
that are no longer reachable.

Sources used, by tier:

- **Tier 1** (canonical, in this repo — wins over everything here):
  `README.md` (pilot definition, phases, age bands, no-assessment rule,
  Pooseidon concept, status line), `CONTRIBUTING.md` (the one rule, naming,
  session folders, same-day provenance, field-notes rule, question-map
  format, OVN log, what-not-to-do), `provenance-template.md` (roles, teacher
  anonymisation, verbatim opening question), `question-map.md` (seed
  questions and their design logic), `LICENSE` (CC BY-SA 4.0).
- **Phase 1 discovery, 2026-07-03** (founder's answers — authoritative):
  no school contacted; GUR-P/COW-H are placeholders; no DBS/consent/agreement
  exists; founder capacity constrained; Athens DEAD; success bar (a)–(d).
- **Sector practice, labelled as such throughout** (general UK schools
  knowledge — **must be verified with each school**): enhanced DBS via
  employer or umbrella body; working under the host school's safeguarding
  policy with school staff present and holding safeguarding duty; consent via
  the school's own processes.

What may drift, and how to re-verify:

| Volatile fact | Re-verify by |
|---|---|
| "No school contacted / no session run" | Check `sessions/` and the outreach log; check github.com/ODINcommons/IoW-pilot — local snapshots may be stale |
| DBS/consent status | Ask the facilitator; check for the documents themselves, not assertions about them |
| School codes table | Read CONTRIBUTING.md at HEAD — real codes should replace placeholder-only status once a school signs |
| README status line ("First sessions planned for 2026") | Read README.md at HEAD; after Gate 5, it should change — if it hasn't, flag it |
| Sector-practice claims | Confirm with the partner school's office; their answer beats this skill |

*This skill is part of the ODIN IoW pilot commons, licensed CC BY-SA 4.0.
Fork it, adapt it, carry the attribution.*
