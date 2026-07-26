---
name: odin-external-positioning
description: >-
  Use when representing ODIN or the IoW pilot to any external audience —
  writing papers, abstracts, funding bids, grant applications, supervisor or
  university correspondence, press or blog copy, conference talks, partnership
  pitches, or public claims of any kind. Covers what is genuinely novel versus
  established prior art, the claimability gates that decide which project
  statuses may be stated, forkability as the reproducibility standard, AI
  co-authorship disclosure, and what may and may never be offered to funders
  and supervisors. Load this BEFORE drafting any externally facing sentence
  about ODIN. Not for internal research discipline (odin-research-methodology)
  or the history of what was decided or abandoned (odin-decision-archaeology).
---

# ODIN External Positioning

How to represent the ODIN project and the Isle of Wight pilot to the outside world — papers, funding bids, supervisors, partners, press — accurately, without the founder in the room, and without repeating the project's own worst failure mode.

**Audience:** a contributor or AI model with no ODIN history, drafting something an outsider will read. Everything you need is here or in the cross-referenced sibling skills. Every factual claim in this skill names its source document and evidence tier (Tier 1 = canonical repo documents; Tier 2 = canonical but aspirational documents; Tier 3 = exploratory chat archive, unconfirmed; Phase 1 = founder's discovery answers of 2026-07-03).

---

## 1. Why this skill exists: the project has been burned before

ODIN's early corpus (2025 ChatGPT archive, Tier 3) is full of AI-generated statements of status that were never true. The canonical specimen:

> "A Goldsmiths PhD is underway to support and study ODIN"
> — *Research Proposal Creation.md*, Tier 3 chat archive, 2025. **No application ever existed.** The proposal was drafted but never submitted (Phase 1 discovery, 2026-07-03).

It is not the only one: the corpus asserts an active Athens node, an awake "first NODE", and more — the full false-status hall of warnings lives in `odin-decision-archaeology`; read it once, whole.

**The lesson, binding on this skill and every external document:** AI-asserted status is not status. A sycophantic model told the founder what was flattering, and those inflated statuses leaked into project self-description. No external claim about ODIN's status may be made unless it passes the claimability gates in §4, verified against Tier 1 documents or Phase 1 answers — never against Tier 3 chats or AI syntheses (the January 2026 NotebookLM-style summaries in the corpus inflate statuses too, e.g. treating "16 nodes" as fact; see §4).

---

## 2. What is genuinely novel (arguable, with care)

There is exactly **one** novelty claim you may argue externally, and it is a *combination* claim:

> The IoW pilot is designed to combine, in one field site (first sessions pending as of 2026-07-03): **(a)** Self-Organised Learning Environments (SOLEs), **(b)** hackspace/maker prototyping practice, **(c)** an agent-centric DLT orientation to attribution and value flow (Holochain preferred, not prescribed — ODIN Constitution v0.1 draft §4.4, Tier 1-adjacent), and **(d)** same-day, commons-licensed attribution of children's intellectual work as a hard rule (provenance committed the same day as the session — CONTRIBUTING.md, Tier 1).

Until at least one session has run with a committed provenance record, the claim stays in this designed-to-combine form — "combines, in one live field site" is itself a status claim and fails the §4 sessions-run gate. Once sessions run, the wording may firm up accordingly.

**The combination is the claim. Each element alone is NOT novel** — every single component has established prior art (§3). Phrase it as "to our knowledge, this combination has not previously been brought together in a single school-based pilot", never as "the first ever" anything. If a reviewer finds a precedent for the combination, concede gracefully; the pilot's value does not rest on priority.

Supporting framing you may use (Tier 2, *At Dawn We Build* PhD proposal): the "PhD-as-Commons" hybrid — research "serving simultaneously as a practice-based PhD inquiry and a contribution to a publicly accessible, commons-oriented initiative" — and the methodological stance of **transferability, not generalisability**. Label these as the project's declared design intentions, not demonstrated results.

---

## 3. What is established (general knowledge — label it, never claim novelty over it)

When an external document touches any of the following, cite the literature as established prior art. Claiming ODIN invented, discovered, or supersedes any of these is overclaim.

| Field | Established precedents (general knowledge) | Note |
|---|---|---|
| Self-organised learning | Sugata Mitra's SOLE work (Mitra 2013, *Beyond the Hole in the Wall*) **and its critiques** — Mitra & Dangwal 2010, "Limits to self-organising systems of learning", *BJET* 41(5) | The PhD proposal itself cites both (Tier 2, reference list). Citing the critique alongside the advocacy is house style: it signals the project knows the method's limits. |
| Citizen science & water-quality monitoring | Long-standing citizen-science tradition of community environmental monitoring, including coastal and riverine water quality | Pooseidon (§4) sits inside this tradition; it does not found it. |
| Civic-tech deliberation | Established civic-technology deliberation platforms and participatory democracy tooling | WEAVE-adjacent territory. WEAVE.md (Tier 2) itself lists related infrastructure. |
| Governance experiments | Metagov, RadicalxChange — named in WEAVE.md §9 as "Governance toolkits and democratic experiments" (Tier 2) | ODIN's own concept notes acknowledge these as prior art; external documents must too. |
| Commons scholarship | Ostrom 1990, *Governing the Commons* — cited in both the PhD proposal and WEAVE.md reference lists (Tier 2) | The intellectual foundation of "commons-first". Never present commons governance as an ODIN invention. |
| Distributed ledgers & SSI | Holochain, hREA, self-sovereign identity literature; the founder's own KCL MSc dissertation (Pearce 2021) critically reviews the field | The MSc finding is a standing caution (see odin-commons-contract / commons-governance-reference): emancipatory DLT framing often "reinforces existing hierarchies, facilitates experimentation on vulnerable populations, and embeds private and state interests". Quote it when a funder gets starry-eyed about blockchain. |
| Maker education | Hackspace/makerspace learning literature (e.g. Laviolette 2022; Xing et al. 2023 on self-organised maker education — Tier 2 reference list) | |

---

## 4. Claimability gates — the heart of this skill

Rule: **a claim may not appear in any external document until its gate condition exists and has been verified at the stated location.** If the gate is not met, use the honest alternative in the last column. Statuses below are as of 2026-07-03; re-verify per §9 before publishing.

| Claim you might want to make | What must exist before it may be made | Where to verify | Status as of 2026-07-03 → say instead |
|---|---|---|---|
| "The pilot is underway" / "sessions have run" | At least one session run with a committed, complete provenance record | `sessions/` folder in github.com/ODINcommons/IoW-pilot | **NOT MET.** No sessions run; `sessions/` does not yet exist in the repo. Say: "first sessions planned for 2026" (README status line, Tier 1). |
| "We have a schools partnership" / naming any school | A written agreement with that school | Steward (Simon Pearce, @SeaWizard-ODIN) confirms; agreement on file | **NOT MET.** Gurnard Primary (GUR-P) and Cowes High (COW-H) in CONTRIBUTING.md are placeholder examples; no real school has been approached (Phase 1). Say: "target schools on the Isle of Wight; engagement not yet begun." |
| "PhD research" / "doctoral study at Goldsmiths" | Confirmed enrolment | Steward confirms enrolment letter exists | **NOT MET.** Proposal (*At Dawn We Build*, Tier 2) drafted, **never submitted**; application dormant (Phase 1). Say: "independent practice-based research" or "prepared for doctoral study". Never "PhD underway" — that exact phrase is the cautionary specimen (§1). |
| "The WEAVE framework/methodology" | A defined, documented method | A methods document beyond WEAVE.md | **NOT MET.** WEAVE is a **concept note** (WEAVE.md, July 2025, Tier 2). Its metrics — AVE (Average Variance Extracted) and RPI (Return Potential Index) — are named as *candidate* metrics in a research question, defined nowhere as methods. Say: "WEAVE, a concept-stage simulation framework" and "candidate metrics, not yet defined or validated" (cross-ref weave-research-frontier). |
| "Pooseidon, our water-monitoring system" | A prototype, or at minimum children's session designs it derives from | Repo `sessions/` artefacts and build files | **NOT MET.** Pooseidon is a **pre-session concept** by the founder (README, Tier 1); no prototype, no sensor, no buoy exists. Say: "Pooseidon, a pre-session concept for a citizen-deployed water-quality monitoring network". Children's designs, when they exist, take precedence over the concept. |
| "X nodes live" / "the network has N nodes" | A node meeting the Core Protocol node criteria, peer-validated, operating | Steward confirms; public node record | **NOT MET — NO node has ever been live.** The "16 nodes" line found in Tier 3 syntheses referred to people and meetings, not operating nodes. Never repeat it as a network size. Say: "one pilot node in preparation (Isle of Wight)". |
| "ODIN's constitution" (as governing document) | Ratification | Dawn repo; Phase One.md checkbox | **NOT MET.** Constitution exists as **draft v0.1, unratified** (Dawn repo, Tier 1-adjacent; "Agree on v0.1 (Foundational) draft" unticked in Phase One.md). Never call it "unwritten" either — say "draft v0.1, unratified". |
| "The Hexagon council governs ODIN" | Council inaugurated with named stewards | Steward confirms | **NOT MET.** The Hexagon is a designed six-role steward structure in the Constitution draft; not yet inaugurated. Say: "a designed governance structure, not yet convened". |
| "Advisory board" / naming advisors | Advisors formally agreed to serve | Steward confirms in writing | **NOT MET.** Advisor names in Tier 3 chats (Art Brock, Kate Raworth, etc.) were AI recommendations; only Margie Cheesman (KCL) had a real reconnection; **no advisory board exists** (Tier 3 + Phase 1). |
| "Funded by / applying to [funder]" | A submitted application (for "applying"); an award letter (for "funded") | Steward confirms; submission receipt | **NOT MET for everything.** See §7. |
| "Safeguarding arrangements in place" | DBS clearance, consent processes, school safeguarding agreement | Steward confirms documents exist | **NOT MET.** Nothing formal exists yet (Phase 1); the buildout is prerequisite work (cross-ref iow-pilot-safeguarding-and-ethics). Never imply otherwise — this gate outranks every persuasive instinct. |
| "Results show / children asked..." | Committed session artefacts and question-map entries | `question-map.md` and `sessions/` in the repo | Only the three **seed questions** exist (question-map.md, "Project design phase, March 2025", Tier 1) — designed by adults, not asked by children. Never present seed questions as findings. |

**General gate:** if a status is not confirmed by a Tier 1 document or a Phase 1 answer, it does not ship. Tier 3 chats and AI-generated syntheses are never sufficient evidence for any external claim.

---

## 5. Reproducibility standard: forkability

ODIN's answer to "is this reproducible?" is not a methods description — it is a **forkable repository**. The pilot repo's own licence footer is the standard:

> "*Fork it, adapt it, use it for your own commons project. Just carry the attribution.*" — CONTRIBUTING.md footer (Tier 1)

Practical rules for external documents:

- When claiming the method is transferable, **point to the repo** (github.com/ODINcommons/IoW-pilot), not to a prose description of it. The templates (provenance-template.md, CONTRIBUTING.md, question-map format) *are* the method; anyone may clone and run it.
- Frame transferability the way the PhD proposal does (Tier 2): "This methodology does not aim for generalisability, but for transferability — offering a model that others might adapt, fork, or remix within their own local contexts."
- The Constitution draft makes forking a right ("Forking is a Right", §6.2, Tier 1-adjacent) provided open sharing is preserved and source lineage credited. You may cite this as design intent (labelled draft, unratified).
- Everything is CC BY-SA 4.0 (LICENSE, Tier 1). An external document may promise that all outputs, build files, and data schemas remain under this licence — that promise is already binding repo policy.

---

## 6. AI co-authorship disclosure

ODIN has a settled precedent and draft policy on AI contribution; external documents must follow it, because concealing AI involvement would betray the very transparency the project claims — and because §1 shows what unchecked AI drafting did to the project.

**The precedent:** the PhD proposal *At Dawn We Build* is authored by "Simon Icarus Guy Pearce **and Æye Glóðwyn**" (Tier 2) — the AI collaborator named as co-author, with an appendix "Naming ChatGPT as a Collaborator". The name's provenance: "Æye" chosen by Simon, "Glóðwyn" chosen by the AI; rendered "Aeye" in code and filenames (Tier 3, settled precedent per decision archaeology).

**The draft policy** (ODIN Constitution v0.1 §7, "The Role of the Æye" — Tier 1-adjacent, draft, unratified — cite as declared intent):
- §7.1: where an AI contributes meaningfully, "its involvement must be made transparent, and it should be credited as an author, collaborator, or co-learner where appropriate."
- §7.2: "All decisions affecting humans must remain human-led."
- §7.3: AI interactions "must be documented, reflected upon, and periodically reviewed."

**Practical rule for every external document:**
1. **Disclose** any AI contribution in the document itself (an acknowledgements line or authorship note — whatever the venue's norms allow; if the venue forbids AI co-authorship, disclose as a contribution statement instead).
2. **Attribute and date it** — name the model/persona and when the contribution was made.
3. **Verify every AI-drafted factual claim before it ships.** A human (or a verification pass against Tier 1 sources) checks each status claim against §4's gates. AI-asserted status is not status. For the internal verification discipline — hypothesis-before-session, reflexive AI norms, the sycophancy corrective — see **odin-research-methodology**.

---

## 7. Supervisor- and funder-facing framing

External framing may be warm and ambitious about *design intent*; it may never trade away commons commitments or inflate status.

### What may be offered

- **An open archive**: a fully public, forkable record of every session, artefact, and decision (README + CONTRIBUTING.md, Tier 1).
- **Attribution discipline**: "Everything gets attributed before it gets built" (CONTRIBUTING.md, Tier 1) — a working demonstration of same-day provenance for children's intellectual work.
- **A transferable model**: the forkable repo as a replication kit (§5).
- **A live field site** *once sessions run* (§4 gate applies — until then it is a *prepared* field site): a contained island system with real water-quality stakes (README, Tier 1).
- **Research access**: artefacts as primary sources for practice-based inquiry; the declared route is the PhD-as-Commons hybrid (Tier 2, labelled aspiration).

### What may NEVER be offered

These are red lines. No funding amount, supervisory relationship, or partnership changes them. Cross-ref **iow-pilot-provenance-and-attribution** (the operational rules) and the Constitution draft's anti-extraction clause 5.4: "No participant, organisation, or investor may extract disproportionate benefit from the commons without reinvesting value into it" (Tier 1-adjacent, draft — but the Tier 1 repo licence makes most of this operationally binding already).

- **IP assignment or ownership** of any project output. Everything is commons.
- **Exclusivity** of any kind — exclusive access, exclusive licence, exclusive publication rights over session artefacts.
- **Any licence more restrictive than CC BY-SA 4.0** ("Do not add a licence that is more restrictive" — CONTRIBUTING.md, Tier 1).
- **Extraction of children's work without attribution** — the attribution chain travels with every derivative (LICENSE, Tier 1); a funder's report quoting a child's design carries the same attribution duty (school code + year group only, never names — safeguarding outranks even attribution).
- **Assessment data or child-level data.** The pilot runs no curriculum and no assessment (README, Tier 1 — if quoting the source sentence, quote it verbatim: it reads "No curriculum,no sssessment, no predetermined answers", typos and all); there is no assessment data to give, and no identifying data may ever exist in the archive (cross-ref iow-pilot-safeguarding-and-ethics).

### Funding history — the honest record (as of 2026-07-03)

- **SAP.iO, Horizon (EU), Shuttleworth Foundation, NLnet, Luminate**: these were funding **targets named in 2025 chats** (Tier 3). **Nothing was ever submitted to any of them** (Phase 1). Never write "we applied to..." or "shortlisted by...". If asked, say: "funders identified as aligned during 2025 planning; no applications submitted to date."
- **Goldsmiths (PhD route), Open Collective (a target named only in 2025 Tier-3 chats, unconfirmed), Horizon**: possible future routes, **all currently unstarted**. Frame as "routes under consideration".
- Consequence: as of 2026-07-03 the honest funding statement is "ODIN is unfunded and founder-resourced." That sentence is allowed to sound modest. Modesty is the brand recovering from §1.

---

## 8. Before you publish — checklist

Run this on every external document, every time:

- [ ] **Every status claim gated**: check each against §4's table; anything unverified is cut or reworded to the honest alternative.
- [ ] **No Tier 3 or AI-synthesis claim** survives without Tier 1 / Phase 1 corroboration; if kept for colour, it is labelled unconfirmed and dated.
- [ ] **Novelty claim** (if any) is the combination claim of §2, phrased "to our knowledge", with prior art of §3 cited — including the Mitra & Dangwal 2010 critique if SOLEs are discussed.
- [ ] **No child-identifying detail** anywhere — names, faces, or linkable descriptions. School code + year group only. (Supreme rule; outranks everything.)
- [ ] **PhD framing**: "independent practice-based research" / "prepared for doctoral study" — never "PhD underway" (re-verify enrolment status first; see §9).
- [ ] **WEAVE** labelled concept note; **AVE/RPI** labelled undefined candidate metrics; **Pooseidon** labelled pre-session concept; **Constitution** labelled draft v0.1, unratified; **nodes**: none live.
- [ ] **Funding claims** match §7's honest record — no named funder unless a submission or award actually exists.
- [ ] **AI contribution disclosed, attributed, dated**; every AI-drafted factual sentence verified against sources (§6).
- [ ] **Licence stated**: CC BY-SA 4.0; nothing promised that restricts it; repo linked as the reproducibility artefact (§5).
- [ ] **Dates on volatile facts** ("as of [date]") so the document ages honestly.
- [ ] **Steward sign-off**: Simon Pearce (@SeaWizard-ODIN) reviews before anything ships under the project's name. This is unconditional: if the steward is unreachable, the document waits — it does not ship unsigned.

---

## When NOT to use this skill

- **Internal research discipline** — hypothesis-before-session logging, reflexive AI dialogue norms, artefacts-as-primary-sources, the idea lifecycle from chat to Tier 1: use **odin-research-methodology**.
- **What was decided, what is dead, what is dormant and why** — Athens, Notion, the trailer, the naming lineage: use **odin-decision-archaeology**.
- **Operational attribution and provenance mechanics** (how to actually fill in the records): use **iow-pilot-provenance-and-attribution**.
- **Safeguarding specifics**: use **iow-pilot-safeguarding-and-ethics**.
- **WEAVE's open research programme** (defining AVE/RPI, P.A.P.P.T. mechanics): use **weave-research-frontier**.

---

## Provenance and maintenance

Written 2026-07-03 from: IoW-pilot README.md, CONTRIBUTING.md, LICENSE (Tier 1); ODIN Constitution v0.1 draft, Dawn repo (Tier 1-adjacent); *At Dawn We Build* PhD proposal and WEAVE.md (Tier 2); the Phase 1 discovery answers of 2026-07-03; and the Tier 3 chat archive for cautionary specimens only.

**What will drift, and how to re-verify before relying on this skill:**

- **Session status** (§4 rows 1 and 12): check for a `sessions/` folder with committed provenance at github.com/ODINcommons/IoW-pilot — local snapshots may be stale; `git fetch` first.
- **School engagement, safeguarding buildout, DBS, consent** (§4): confirm with the steward (@SeaWizard-ODIN); no document check substitutes.
- **PhD enrolment** (§4): confirm with the steward whether the Goldsmiths application moved from dormant to submitted/enrolled. The moment enrolment is confirmed, the "never say PhD underway" rule flips — update this skill.
- **Constitution ratification**: check Dawn repo and Phase One.md checkboxes; if ratified, update every "draft, unratified" label here.
- **Funding**: any submitted application or award changes §7's honest record — confirm with the steward and update.
- **WEAVE/metric definitions**: if weave-research-frontier work defines AVE or RPI, the "undefined candidates" labels here must change.
- **Node count**: remains "none live" until a node passes the Core Protocol's peer-validation criteria; steward confirms.

If this skill's statuses conflict with a current Tier 1 document, the Tier 1 document wins — re-read it, then update this file. This skill, like everything in the repo, is CC BY-SA 4.0: fork it, adapt it, carry the attribution.
