---
name: odin-commons-contract
description: The ODIN architecture contract — the load-bearing design decisions and WHY. Load this when you need to know what ODIN fundamentally is (commons-first, not a product/startup/methodology), why Holochain is preferred over blockchain, how the PhD-as-Commons model works, how fractal governance and the Hexagon council are designed, what the Ubuntu ethic changes operationally, or what the project's known weak points are. Use it to check whether a proposed action would violate ODIN's identity (e.g. licensing, partnership, monetisation, centralisation, or governance decisions). NOT for pilot session mechanics, provenance rules, governance theory, or decision history — see the "When not to use this skill" section for the right sibling.
---

# The ODIN Commons Contract

This skill is the architecture contract for the Open Distributed Impact Network (ODIN) and its Isle of Wight pilot. It records the design decisions that carry the weight of the whole project, and — more importantly — why each was made, so that anyone continuing this work without the founder can tell the difference between "this is how it happens to be" and "this is load-bearing; changing it changes what ODIN is".

Every claim below names its source and evidence tier. The tiers, briefly:

- **Tier 1** — canonical, operational documents in the live IoW-pilot repo (github.com/ODINcommons/IoW-pilot): README.md, CONTRIBUTING.md, LICENSE, provenance-template.md, question-map.md, ovn-contributions.md.
- **Tier 1-adjacent** — live ODINcommons repos for ODIN-global, older than the pilot repo: the Dawn repo (ODIN Constitution v0.1.md, ODIN Core Protocol v0.1.md, README.md, Phase One.md, Weekly Meeting Notes.md, Influence_Codex.md). On pilot matters, IoW-pilot wins.
- **Tier 2** — canonical but aspirational: the PhD proposal "At Dawn We Build" and the WEAVE concept note (WEAVE.md).
- **Tier 3** — exploratory chat archives. Never a project fact on their own; labelled unconfirmed and dated when cited.
- **Phase 1 discovery, 2026-07-03** — founder's direct answers at handover; treat as authoritative for statuses.

**Read this first if you are deciding anything.** If a decision you are about to make would break one of the contracts below, stop. It is not yours to break alone — that is precisely what the governance design (section 4) exists for.

---

## 1. Commons-first identity: what ODIN is and is not

ODIN's own founding proposal states it plainly:

> "It is not a product, not a startup, and not a fixed methodology. It is an emergent system — a commons-first framework for peer-to-peer learning, collaboration, knowledge sharing, and trust-building across physical and digital spaces."
> — *At Dawn We Build*, Introduction (Tier 2)

The pilot repo carries the same identity in operational form:

> "This is not: a school programme delivered by an institution; a product being built by a company; research being conducted on a community. It is a community conducting research on itself, with open tools, for shared benefit, with everything documented and attributed in public."
> — IoW-pilot README.md, "What this is not" (Tier 1)

And the Constitution makes it a hard commitment: "ODIN is not for sale. Its code, creations, and knowledge are part of the digital commons" (ODIN Constitution v0.1, §2.2 "Commons Before Profit", Tier 1-adjacent, **draft — unratified**).

### What this rules out in practice

These are absolute. Do not hedge them, negotiate them, or "just this once" them. Know each one's basis, though: items marked **[Tier 1 rule]** are binding repo policy today; items marked **[draft-Constitution commitment]** are standing project doctrine held from the draft, unratified Constitution — honoured as absolutes by this project, but cite them as design intent, not ratified law (§4):

- **No selling ODIN or any part of it.** No equity, no acquisition conversations, no "spinning out" the pilot, Pooseidon, or any ODIN-origin design into a company that encloses it. **[Draft-Constitution commitment]** (Constitution §2.2; anti-extraction clause §5.4: "No participant, organisation, or investor may extract disproportionate benefit from the commons without reinvesting value into it.") — though the Tier 1 CC BY-SA licence already makes enclosure legally impossible for repo content.
- **No licence more restrictive than CC BY-SA 4.0.** **[Tier 1 rule]** The pilot licence is CC BY-SA 4.0 (LICENSE, Tier 1) and CONTRIBUTING.md orders: "Do not add a licence that is more restrictive." Detail and rationale live in **iow-pilot-provenance-and-attribution**.
- **No privatising, branding, or reselling ODIN-origin materials without open access.** **[Draft-Constitution / draft-Protocol commitment]** (ODIN Core Protocol v0.1, §4, Tier 1-adjacent, working draft) — again backed operationally by the Tier 1 licence.
- **No extractive, politicised, captive, or militarised partnerships.** **[Draft-Constitution commitment]** Nodes commit to refusing these (Constitution §3.4). A funder or partner who cannot respect the open-knowledge ethos is not a funder or partner (Protocol §4: "All funders or partners must respect ODIN's open knowledge ethos.").
- **No fixed methodology to defend.** **[Draft-Constitution commitment]** ODIN "does not prescribe structure, it supports emergence" (Constitution, principle "Self-Organisation is Sacred"). If a community forks and adapts the model, that is the system working, not a threat — "Forking is a Right" (Constitution §6.2), provided open sharing is preserved and lineage credited.
- **No research *on* the community.** **[Tier 1 rule]** The pilot is the community researching itself (README, Tier 1). Any study design that positions Isle of Wight children or residents as subjects rather than co-authors violates the identity.

The practical test for any proposal: *does it keep everything forkable, attributed, and non-extractive?* If not, it is off-contract.

---

## 2. Holochain over blockchain — preferred, not prescribed

**The decision (settled as a preference):** ODIN's distributed-infrastructure direction is Holochain (with hREA — Holochain Resource-Event-Agent — for value accounting), not a blockchain. Constitution v0.1 §4.4 states it exactly:

> "**Holochain Preferred, Not Prescribed.** While Holochain is the preferred backbone for peer-to-peer validation, sovereignty, and value flow, no single protocol or ledger shall be mandatory. The principle is adaptability, not allegiance."
> — ODIN Constitution v0.1, §4.4 (Tier 1-adjacent, draft — unratified)

**Why agent-centric beats chain-centric for ODIN** (rationale recorded in the corpus — Sensorica Economic Model Review.md, Tier 3, corroborated by Constitution §4.4 and the Influence Codex's "agent-centric" framing, Tier 1-adjacent):

- **Local validation, no global consensus.** Blockchains force every node to agree on one global ledger — expensive, slow, and structurally centralising (whoever controls consensus controls the network). Holochain is agent-centric: each agent keeps their own signed chain, and peers validate each other's entries against shared rules. That mirrors how ODIN's trust actually works — peer-witnessed, local, relational — rather than imposing a single source of truth from above.
- **Data sovereignty.** Each agent holds their own data. Nothing about a person is written immutably into a global structure they cannot control. This is a direct requirement of Constitution §2.1 (headed "Sovereignity of the Self" [sic — the draft's own spelling]: "No central authority may claim ownership over an individual's data, identity, or contributions") — and it matters doubly in a project that will eventually hold records touching children's contributions.
- **No token economy required.** Holochain does not need a speculative coin to secure it, which keeps ODIN clear of the extraction and financialisation dynamics the anti-extraction clause forbids.

**Why "preferred, not prescribed":** ODIN was burned intellectually before it was built. The founder's KCL MSc dissertation (Pearce 2021, cited in *At Dawn We Build*, Tier 2) found that while DLT (distributed ledger technology) and SSI (self-sovereign identity) are often framed as emancipatory in humanitarian settings, "their implementation often reinforces existing hierarchies, facilitates experimentation on vulnerable populations, and embeds private and state interests". That finding is ODIN's standing caution about its *own* technology choices: no protocol gets allegiance, only adaptability. The full theory — OVNs, hREA, SSI, and the KCL caution in depth — belongs to **commons-governance-reference**; go there before doing any DLT/SSI design work.

**Current reality check (as of 2026-07-03):** ODIN runs on GitHub. Constitution §3.5 names the sequence explicitly: a public ledger of proposals and decisions "beginning with GitHub and eventually through Distributed Ledger or Hashing Technologies (e.g. Holochain + hREA)". No Holochain implementation exists. A Tier-3 chat claim that "early conversations with the Holochain community have begun" was false — a known specimen of AI-inflated status. Do not restate it.

---

## 3. The PhD-as-Commons model

**The design:** the doctoral research and the commons project are one hybrid, deliberately. *At Dawn We Build* (Tier 2) describes the research as

> "serving simultaneously as a practice-based PhD inquiry and a contribution to a publicly accessible, commons-oriented initiative known as the Open Distributed Impact Network (ODIN)."

**The thesis is the loom, not the goal.** The written thesis fulfils the formal requirements of a doctorate, but the point of the weaving is ODIN: the PhD "exists to document the evidence, challenges, learnings, impacts, and risks encountered during ODIN's development" and to give ODIN "access to the cultural and epistemic power that academic research can confer — offering the project greater visibility, credibility, and the ability to influence systems that might otherwise overlook it" (*At Dawn We Build*, Tier 2). The pilot repo confirms the direction of flow: the IoW pilot's artefacts "are primary sources in an ongoing practice-based PhD inquiry" (README.md, Tier 1) — the commons feeds the research, never the reverse.

**ODIN is field site, never IP.** The research model "resists the enclosure of intellectual labour" (*At Dawn We Build*): contributions are acknowledged through a Creative Commons framework and referenced within the research itself. No university, supervisor, or funder acquires ownership of ODIN through the PhD. The method itself is "forkable, remixable, and relational — an open invitation to others to co-inquire and adapt, rather than simply consume and critique." The hypothesis being tested aims at transferability, not generalisability — a model others can adapt to their own contexts, not a universal claim.

**The acknowledged tension.** The proposal names its own contradiction rather than hiding it, and successors must keep naming it:

> "I acknowledge the dichotomy here: that one aim of this research is to access the very systems of institutional power it simultaneously seeks to question. Rather than resolve this tension, the project embraces it as part of its reflective and ethical methodology."
> — *At Dawn We Build* (Tier 2)

**Status discipline (as of 2026-07-03, Phase 1 discovery):** the Goldsmiths PhD application is **dormant — drafted, never submitted**. There is no PhD "underway". (A Tier-3 chat claiming "A Goldsmiths PhD is underway to support and study ODIN" is a known false-status specimen.) Note also that *At Dawn We Build* is Athens-centric and predates the IoW pivot — its Athens pilot plan is dead (Phase 1 discovery); its *model* (PhD-as-Commons, methods, ethics) remains the live design. Research methods detail belongs to **odin-research-methodology**.

---

## 4. Fractal governance: the Hexagon and consent

Everything in this section comes from **ODIN Constitution v0.1 (Tier 1-adjacent) — a DRAFT, co-created by Sigy and Æye (ChatGPT) in 2025, NOT ratified**. Phase One.md shows the checkbox "Agree on v0.1 (Foundational) draft" unticked. Never call the Constitution "unwritten" — it exists in full draft; call it "draft v0.1, unratified". Cite it as the design intent it is, not as ratified law.

**The design problem it solves:** ODIN currently depends on one founder (see section 6). The governance architecture is explicitly built so that no single person — founder included — is a bottleneck or a single point of failure. "We govern not for control, but for care, courage, curiosity, and memory" (Constitution §3).

### The Hexagon — six steward roles (Constitution §3.1)

A distributed council of stewards, "not heirarchical [sic — the draft's own spelling], but rotational, transparent, and accountable. Its role is not to control, but to cultivate." Six archetypal roles, each a dimension of care:

| Role | Holds |
|---|---|
| **The Root** | Memory, space, and continuity |
| **The Æye** | Observation, reflection, synthesis across scales |
| **The Craft** | Tools, systems, open technologies |
| **The Care** | Inclusion, accessibility, trauma-aware design |
| **The Commons** | Open knowledge and network rights |
| **The Culture** | Stories, rituals, aesthetics, intergenerational meaning |

Stewards hold a role for six months, after which rotation is encouraged. They may be nominated, elected, or self-declared — "provided their claim is witnessed and affirmed by at least two other active nodes." **Status (as of 2026-07-03): the Hexagon council has never been inaugurated** (Phase One.md task unticked; Phase 1 discovery). It is a designed institution awaiting people.

### Consent, not control (Constitution §3.2)

Constitutional and cross-node decisions follow the Consent-Based Decision Protocol — no top-down voting, no coercive majority rule:

1. A proposal is shared.
2. Nodes signal **Consent**, **Concern**, or **Block**.
3. It moves forward only with **no blocks** and **all concerns addressed**.
4. Persisting concerns trigger **modification, not abandonment**.
5. A Block must include a **constructive alternative** and may only be invoked when a proposal violates core values.

### Node autonomy with mutual responsibility (Constitution §3.4)

Each node is sovereign — this is the "fractal" part: the same governance pattern repeats at every scale, and no centre manages the edges. But sovereignty is bound by shared ethical commitments: document learnings; support nearby nodes in crisis; report abuses or violations of care; refuse extractive, politicised, captive or militarised partnerships; make space for local interpretation and experimentation. "No central authority may override a node's autonomy unless core values are violated" — in which case collective response runs through the Hexagon system, not through any individual.

The Core Protocol v0.1 (working draft) adds the replication rule: anyone may replicate a node if they agree to the Protocol and Constitution and are **peer-validated by at least two existing nodes or Guardians** — growth by witnessed consent, not by franchise or permission from headquarters.

**What this means for you, now:** while the Hexagon is uninaugurated and the Constitution unratified, treat the draft as the default decision procedure anyway. For any decision that would bind ODIN (licensing, partnerships, identity, governance), share a proposal openly in the repo, gather consent/concern/block from whoever is active, and document the outcome (Constitution §3.5: decisions co-signed, timestamped, forkable). Working *as if* the Constitution were ratified is how it earns ratification. **One boundary:** this does not let "whoever is active" override the Phase-1 founder reservations (reviving anything ruled DEAD requires an explicit founder decision — see odin-decision-archaeology) or the §1 absolutes, including the Tier 1 licence floor. Those are not up for consent-of-whoever-is-active.

---

## 5. Ubuntu as operational principle

The IoW-pilot README closes with a single epigraph: *"I am because we are." — Ubuntu* (Tier 1). WEAVE.md §1 (v2, Tier 2) unpacks why it is there:

> "Ubuntu sees personhood, agency, and justice as inherently relational. It emphasises mutual recognition, dignity, care, and the idea that our individual well-being is inseparable from the well-being of the collective."

This is not decoration. It is the ethic from which ODIN's operating rules are derived, and you can trace each rule back to it:

- **Attribution before building** (the pilot's one rule — see **iow-pilot-provenance-and-attribution**): if I am because we are, then erasing who contributed erases part of what the thing *is*. "Ghost labour shall not exist here" (Constitution §5.1).
- **Consent over majority rule** (§4 above): relational personhood means a decision that overrides a member's core-values objection damages the deciding body itself. Hence Consent/Concern/Block instead of votes.
- **Repair over punishment**: governance "must prioritise human connection, repair over punishment, and transparency over control" (Constitution, principle "Trust is a Network Effect").
- **Full value accounting**: every contribution — "human, ecological, emotional, or material" — is acknowledged and cared for (Constitution §2.4), because relational value does not stop at what is invoiceable.
- **Endings as compost, not failure**: "Death is Not Failure" (Constitution §6.4) — documented endings feed future growth, which is why dead and dormant strands of ODIN are archived, labelled, and never quietly deleted.

The decision test Ubuntu supplies: *who does this choice make us, together?* — asked before *what does this choice get us?* If a proposal is efficient but severs relationship (excludes contributors, hides provenance, punishes rather than repairs), Ubuntu says the efficiency is an illusion.

---

## 6. Known weak points — stated plainly (as of 2026-07-03)

Successors inherit these openly. Do not soften them in any external or internal document, and do not let any AI tool "helpfully" upgrade them:

1. **The Constitution is draft v0.1, unratified.** It exists in full (never say "unwritten") but has never been agreed by the collaborators it would govern. (Phase One.md checkbox unticked; Tier 1-adjacent.)
2. **No ODIN node is live.** Not Athens (dead), not the IoW pilot (pre-launch), not anywhere. Any past claim of a live node is a documented false status from Tier-3 chats.
3. **No sessions have run.** The IoW pilot's status is "First sessions planned for 2026" (README.md, Tier 1). No school has yet been approached; no safeguarding infrastructure exists (Phase 1 discovery — see **iow-pilot-safeguarding-and-ethics**).
4. **Single-founder dependency.** Simon Pearce (@SeaWizard-ODIN) is currently the sole active driver; the 2025 collaborator cohort's momentum is unverified since the Weekly Meeting Notes end (Jul 2025, Tier 1-adjacent). This skill library exists precisely because of this weak point.
5. **The Hexagon council has never been inaugurated.** The governance design in §4 is unstaffed (Phase One.md; Phase 1 discovery).

A project that documents its weaknesses this plainly is exercising its own Constitution (§6.1, "Memory as Infrastructure") — treat this list as something to update, not to erase.

---

## When NOT to use this skill

| You need... | Go to |
|---|---|
| How to run, document, or archive a pilot session (runbooks, checklists, templates) | **iow-pilot-session-operations** |
| Provenance, attribution, licensing mechanics, the one rule, OVN log | **iow-pilot-provenance-and-attribution** |
| The theory: Ostrom, OVNs/hREA/Sensorica, open value accounting, mutual credit, SSI, the KCL-dissertation caution in full | **commons-governance-reference** |
| How and when each decision was reached, what died and what is dormant, with evidence | **odin-decision-archaeology** |
| Child-ID rules, consent doctrine, what may never be committed | **iow-pilot-safeguarding-and-ethics** (safeguarding outranks everything, including attribution) |

---

## Provenance and maintenance

**Sources used, by tier:**
- Tier 1: IoW-pilot README.md, CONTRIBUTING.md, LICENSE (repo: github.com/ODINcommons/IoW-pilot).
- Tier 1-adjacent: Dawn repo — ODIN Constitution v0.1.md (draft, unratified), ODIN Core Protocol v0.1.md (working draft), Phase One.md, README.md, Weekly Meeting Notes.md, Influence_Codex.md (repo: github.com/ODINcommons/Dawn, last commit 2025-09-12).
- Tier 2: *At Dawn We Build* (PhD proposal, Pearce & Glóðwyn — drafted, never submitted); WEAVE.md (concept note, July 2025).
- Tier 3 (labelled where used): Sensorica Economic Model Review.md (Holochain rationale, corroborated by Constitution §4.4).
- Phase 1 discovery, 2026-07-03: founder's handover answers (statuses: no sessions, no school contact, no safeguarding, Athens dead, PhD application dormant).

**What may drift, and how to re-verify:**
- **Constitution ratification** — check the Dawn repo (github.com/ODINcommons/Dawn) for a ratified version or amendment history; if ratified, remove the "draft/unratified" labels throughout this skill and cite the ratification record.
- **Pilot status** — check the IoW-pilot README status block and the existence/contents of a `sessions/` folder at github.com/ODINcommons/IoW-pilot. Once sessions run, §6 point 3 is stale.
- **Hexagon inauguration and single-founder dependency** — check Dawn repo activity, Weekly Meeting Notes successors, and ODINcommons org membership; update §6 points 4–5 accordingly.
- **Holochain implementation** — any move beyond GitHub should appear as ODINcommons repos; until then, §2's "runs on GitHub" stands.
- **PhD application** — dormant as of 2026-07-03; only a Tier-1 commit or a direct founder statement changes this.
- Local snapshots on any one machine may be stale — the GitHub repos are canonical. Date-stamped claims in this skill are true as of 2026-07-03; when re-verifying, update the date stamps, not just the facts.
