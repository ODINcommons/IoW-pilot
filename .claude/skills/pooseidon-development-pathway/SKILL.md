---
name: pooseidon-development-pathway
description: >-
  Guides the journey from children's impactathon designs to a working
  citizen water-quality monitoring prototype (working name "Pooseidon") in
  the ODIN Isle of Wight pilot. Load this when: an impactathon has produced
  designs and someone asks "what happens next"; a hackspace, makerspace,
  industry partner, or open-hardware group wants to join the build phase;
  someone asks what Pooseidon is or whether it can be built yet; questions
  arise about water-quality sensing, buoys, sewage-discharge detection, or
  alerting water companies; or build files, hardware licensing, or open-data
  questions for the prototype come up. Do NOT load for getting sessions
  running (iow-pilot-launch-campaign), running an impactathon
  (iow-pilot-session-operations), or licence/attribution mechanics
  (iow-pilot-provenance-and-attribution).
---

# Pooseidon development pathway

From impactathon designs to a working citizen water-quality monitoring prototype — with the attribution chain intact at every step.

## Read this first: what Pooseidon is, and is not

**Pooseidon is a pre-session concept sketched by the founder.** The README (Tier 1) describes it as the "first project idea": "a citizen-deployed water quality monitoring network for Isle of Wight coastal waters" whose "buoys detect pollution signatures in real time and automatically alert water companies, local MPs, and the public when unsafe thresholds are crossed."

**As of 2026-07-03, no session has run** (README status line, Tier 1; Phase 1 discovery, 2026-07-03). There are no children's designs yet. There is nothing to build yet.

**When children's impactathon designs exist, they take precedence over the founder's sketch.** The build phase builds what the children designed, attributed to them. The name "Pooseidon", the buoy form factor, and the alerting concept are all subject to replacement by what actually emerges from the impactathon. If the children design a shoreline sensor post, a drone, or something nobody predicted, that is the project. Treat the README sketch as a seed, not a specification.

This matters because the whole pilot exists to test whether "a peer network of curious people, including children, [can] prototype impactful solutions to real local problems faster and more honestly than industry" (README, Tier 1). Building the founder's sketch instead of the children's design would break the experiment.

**Jargon defined once:**
- **Impactathon**: the pilot's Phase 3 — a mixed-age, mixed-school design event where teams "design real responses to real problems"; designs are documented, published, and attributed the same day (README, Tier 1).
- **Provenance record**: the per-session `provenance.md`, completed from `provenance-template.md`, logging who contributed what (Tier 1).
- **OVN log**: the Open Value Network contribution log, `ovn-contributions.md`, one row per contribution (Tier 1). An Open Value Network is a way of recording every contribution to a shared project so value and credit are traceable.
- **CC BY-SA 4.0**: Creative Commons Attribution-ShareAlike 4.0 International — the repository's licence (LICENSE, Tier 1).

---

## The provenance gate (non-negotiable)

CONTRIBUTING.md (Tier 1) is explicit: **"Do not begin a build phase before the relevant provenance records are complete."** And: "Before any external contributor — individual, organisation, or institution — begins building on that work, the provenance record must be complete, public, and current."

Before ANY external partner builds anything based on session outputs, verify all of the following for every session the build draws on:

- [ ] `provenance.md` exists in the session folder and is committed (it should have been committed the same day as the session — CONTRIBUTING.md, Tier 1)
- [ ] All artefacts the build is based on are named per the file naming convention and logged (see iow-pilot-documentation-standards for the convention and a known formatting ambiguity in it)
- [ ] OVN log entries exist in `ovn-contributions.md` for the contributing cohorts (child contributors identified by school code + year group only, e.g. `GUR-P-Y5` — never names)
- [ ] The records are **public** — pushed to github.com/ODINcommons/IoW-pilot, not sitting in a local clone
- [ ] The records are **current** — they reflect the actual sessions and artefacts, not placeholders

**If any item is incomplete: complete it first, build second. No exceptions.** CONTRIBUTING.md: "If a session's provenance record is incomplete, complete it first." This is the pilot's one rule in action: "Everything gets attributed before it gets built."

Do not accept "we'll backfill the provenance after the prototype works" from anyone, however well-meaning. The attribution chain is the product as much as the hardware is.

---

## Onboarding a build partner

Per CONTRIBUTING.md (Tier 1), the build phase is open to hackspaces, makerspaces, industry partners, open-hardware networks, and individuals. Phase 4 of the pilot: "The most viable design moves into a build phase, in partnership with local industry, hackspaces, and open hardware networks" (README, Tier 1).

Every external contributor follows these four steps (CONTRIBUTING.md, verbatim in substance):

1. **Read the full `README.md`** — so they understand what the pilot is (a community conducting research on itself) and what it is not (a product being built by a company).
2. **Read the provenance records for the sessions their build is based on** — they must know whose work they are building on.
3. **Confirm in writing that they have read and accept the CC BY-SA 4.0 licence terms and understand the attribution chain.** A GitHub issue on ODINcommons/IoW-pilot is sufficient. Do not let a partner start work on a handshake — the written confirmation is the record.
4. **Open a pull request with their contribution, including their OVN log entry** (contribution types: `conceptual` / `design` / `fabrication` / `deployment` / `documentation` / `facilitation`).

The spirit, verbatim from CONTRIBUTING.md: **"You are welcome here. The only condition is that you bring the attribution chain with you."**

**Note on partners, as of 2026-07-03:** no build partners exist. No hackspace, industry, or open-hardware relationship has been established (no such relationship appears in any Tier 1 source, and no session has run to build from). Anything in older ODIN chat archives implying live partnerships is unconfirmed Tier 3 material — do not repeat it as fact.

---

## Water-quality sensing: domain background for contributors

**Everything in this section is general knowledge, labelled as such — background to help a zero-context contributor think clearly, NOT project fact, NOT a design decision.** The children's designs and the partners' engineering judgement decide what is actually built.

### What citizen sensors can plausibly measure (general knowledge)

Low-cost, real-time, in-water sensors can realistically measure **proxies** for pollution, not sewage itself:

| Parameter | What it proxies | Citizen-sensor feasibility (general knowledge) |
|---|---|---|
| Turbidity | Suspended solids; storm/sewage discharge plumes | Feasible cheaply (optical sensors); noisy, affected by weather and sediment |
| Temperature | Discharge events, thermal anomalies | Trivially cheap and reliable |
| Electrical conductivity | Dissolved ions; freshwater/effluent intrusion in seawater | Cheap; interpretation in coastal water is harder than in rivers |
| Dissolved oxygen | Organic pollution load (sewage consumes oxygen as it decomposes) | Mid-cost; sensors drift and need maintenance/calibration |
| pH | General chemical disturbance | Cheap; drifts, needs recalibration |
| Ammonia/nitrate | Sewage and agricultural runoff | Harder and costlier at citizen grade; ion-selective electrodes drift badly |

**Be honest about the hard part:** the thing people most want to know — *is there faecal bacteria (E. coli, intestinal enterococci) in the water right now?* — **cannot currently be measured cheaply in real time.** Bacterial counts need lab culture methods (typically 18–48 hours) or expensive molecular/fluorometric field instruments. Cheap real-time sewage detection is a genuinely unsolved problem; a citizen network detects *correlates and events* (turbidity spike + conductivity change + rainfall = probable discharge), not certified contamination readings. Any contributor or partner who claims otherwise should be pressed on it. (All of this paragraph: general knowledge, as of the authoring model's early-2026 knowledge; verify current sensor state of the art before build decisions.)

Other practical realities of coastal deployment (general knowledge): biofouling degrades sensors within weeks without antifouling measures and maintenance visits; moorings and buoys in navigable coastal waters raise marine-licensing and navigation-marking questions (in England, the Marine Management Organisation and Trinity House are the usual bodies — verify); salt water destroys cheap electronics without proper enclosures; power and data backhaul (LoRaWAN, GSM, satellite) constrain what "real time" means.

### The Isle of Wight context (Tier 1)

The README (Tier 1) states the island's "coastline l faces ongoing sewage discharge from water companies" [sic — the source sentence contains a stray "l"; quote it verbatim] and its communities have "maritime,composite,and engineering heritage that makes peer prototyping plausible" [sic — missing spaces in the source]. That heritage is exactly why a local build phase is credible: boatbuilders, composite fabricators, and marine engineers are the natural partner pool.

### Citizen-science landscape to learn from (general knowledge — landscape, NOT partnerships)

These are precedents a contributor should study; **none of them is a partner of this pilot**, and none appears in any Tier 1 source:

- **Surfers Against Sewage** — UK charity running water-quality reporting and a real-time sewage-discharge alert service built partly on water-company event-duration monitoring data. Closest existing model for the alerting concept.
- **River citizen-science kits and groups** — e.g. the Riverfly Partnership's invertebrate monitoring, WaterRangers-style test kits, and UK river trusts' volunteer sampling programmes. Useful for protocols, data-quality practice, and volunteer training models.
- **Water-company event-duration monitoring (EDM) data and Environment Agency bathing-water classifications** — the existing official data streams any citizen network would be compared against and could calibrate against.

(All general knowledge; verify current status of each before citing to partners.)

### The alerting concept: open questions, not solved problems

The README (Tier 1) sketch has buoys "automatically alert water companies, local MPs, and the public when unsafe thresholds are crossed". Treat everything about that sentence as **open design and governance work**, to be resolved during the build phase — none of it is decided:

- **Data-quality claims.** What may the network honestly claim? Uncalibrated citizen sensors cannot declare water "unsafe" in a regulatory sense; they can flag anomalies. Who sets thresholds, and against what baseline? (General knowledge: Environment Agency bathing-water and EDM data are the obvious public baselines to calibrate and compare against.)
- **Defamation and accuracy care.** Automatically telling the public that a named water company is polluting is a factual accusation. If a sensor artefact triggers a false alert, that carries legal and credibility risk. The alert wording, evidence threshold, and review step before publication all need designing. This is an open issue to resolve with partners (and, if warranted, legal advice) — not a reason to abandon the concept, but not a detail to hand-wave either.
- **Regulatory position.** Whether and how citizen data can be submitted to, or challenge, official monitoring is an open question. (General knowledge: the Environment Agency has run citizen-science engagement schemes; their current form should be checked at build time.)
- **Alert recipients.** "Water companies, local MPs, and the public" is the founder's sketch. The children's design and the partners decide the real recipient list and mechanism.

Log these as questions in `question-map.md` when they arise in sessions — several are exactly the kind of question a 14–16 cohort may reach on its own.

---

## Open by default: data and licensing for the build

- **All data is open by default. All designs are commons-licensed from day one.** (README, Tier 1 — verbatim in substance.) There is no "we'll open it after the pilot" path.
- **All build files are committed to this repository** under the file naming convention with phase code `Build` (CONTRIBUTING.md phase table, Tier 1), inside the relevant session-lineage structure. Phase 4: "All build files are committed here under CC BY-SA 4.0" (README, Tier 1).
- **Licence: CC BY-SA 4.0** (LICENSE, Tier 1). Derivatives must carry the same licence; "Do not add a licence that is more restrictive than CC BY-SA 4.0" (CONTRIBUTING.md, Tier 1).
- **Hardware licensing nuance, stated honestly (general knowledge):** CC BY-SA 4.0 is a copyright licence; copyright covers design files, schematics, documentation, and code, but gives weak protection over the *manufactured hardware itself* — a physical circuit or hull shape is largely outside copyright's reach. Open-hardware-specific licences (e.g. CERN-OHL variants, TAPR OHL) exist to address this and the gap may be raised — but only inside hard guard rails: **(a)** any OHL discussion can only ever be about an **additional, parallel licence on new build files** — never a replacement, restriction, or exclusivity of any kind; **(b)** build files derived from children's session artefacts are **derivatives already bound to CC BY-SA 4.0 by ShareAlike** — no future decision, Tier 1 change, or partner agreement can restrict them; **(c)** nothing more restrictive than CC BY-SA 4.0 may ever be applied to repository content ("Do not add a licence that is more restrictive" — CONTRIBUTING.md, Tier 1; README Phase 4 is categorical: "All build files are committed here under CC BY-SA 4.0"); and **(d)** adopting any additional licence would be a Tier-1 change proposed in the open (GitHub issue/PR, steward review), **never negotiated bilaterally with a partner** (see odin-external-positioning's never-offer list). For the full licence rationale and attribution mechanics, defer to **iow-pilot-provenance-and-attribution** — that skill owns licensing; this one only flags the hardware nuance.
- Every build contribution gets an OVN log entry (`fabrication`, `design`, `deployment`, etc.), and the children's design contributions remain in the chain: a Pooseidon-descendant prototype's provenance runs child cohort → impactathon artefact → build files, unbroken.

---

## Build-phase sequence at a glance

1. **Impactathon completes** (see iow-pilot-session-operations) — designs documented, published, attributed same day.
2. **Provenance gate check** (this skill, above) — all records complete, public, current. If not: stop, complete, then proceed.
3. **Select the most viable design** — README Phase 4 says "the most viable design moves into a build phase". *How* viability is judged, and by whom (children? facilitators? partners jointly?), is not defined in any Tier 1 source — it is an open decision. Record whatever process is used, transparently, in the repo.
4. **Onboard partners** — the four steps above, written licence confirmation before work starts.
5. **Build in the open** — files committed under the naming convention, phase code `Build`, CC BY-SA 4.0, OVN entries per contribution.
6. **Resolve alerting/data-quality open questions** before any public alerting goes live.
7. **Deploy, maintain, publish data openly** — and log deployment and maintenance as OVN contributions too.

---

## When NOT to use this skill

- **Getting sessions running at all** (safeguarding, school contact, first SOLE) → **iow-pilot-launch-campaign**. As of 2026-07-03 that is where the project actually is; this skill describes a later stage.
- **Running the impactathon itself** (formats, checklists, same-day documentation) → **iow-pilot-session-operations**.
- **Licence, attribution, provenance-record, OVN-log mechanics in detail** → **iow-pilot-provenance-and-attribution** (it owns the one rule; this skill only applies it to the build phase).
- **Documentation formats and the naming convention's fine print** → **iow-pilot-documentation-standards**.

---

## Provenance and maintenance

- **Sources used:** `README.md` (Tier 1 — Pooseidon concept, Phase 4, IoW sewage context, open-by-default, status line), `CONTRIBUTING.md` (Tier 1 — provenance gate, external onboarding steps, licence rules, what-not-to-do), `LICENSE` (Tier 1 — CC BY-SA 4.0), Phase 1 discovery answers from the founder (2026-07-03 — no sessions run, no partners exist). Water-sensing, citizen-science-landscape, marine-deployment, and hardware-licensing material is **general knowledge as of early 2026**, explicitly not project fact.
- **What may drift, and how to re-verify:**
  - *Whether sessions have run and designs exist* — check `sessions/` at github.com/ODINcommons/IoW-pilot (the folder does not exist as of 2026-07-03). The moment real impactathon designs land, the "pre-session concept" framing at the top of this skill must be updated to point at the actual designs, and this skill re-centred on them.
  - *Whether build partners exist* — check GitHub issues on the repo for written licence confirmations, and `ovn-contributions.md` for partner entries.
  - *Sensor state of the art and citizen-science landscape* — the general-knowledge sections here age fast; re-verify (web search: current low-cost sensor capability, Surfers Against Sewage service status, Environment Agency citizen-science schemes) before advising a real build.
  - *Licensing decisions* — if an open-hardware licence discussion concludes, it must land in Tier 1 (LICENSE or CONTRIBUTING.md) before this skill treats it as settled.
  - Local snapshots may be stale — the GitHub repo is canonical.
- **This skill states no session, partnership, or build as having happened.** If you find text here that does, it has drifted; correct it against Tier 1.
