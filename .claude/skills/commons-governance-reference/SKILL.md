---
name: commons-governance-reference
description: Domain-theory reference for the commons-governance concepts behind ODIN and the IoW pilot — Ostrom's commons principles, open value networks (Sensorica/hREA), open value accounting, mutual credit, self-sovereign identity and the KCL-dissertation caution, copyleft mechanics (CC BY-SA vs Peer Production License), and delegative/liquid democracy and consent-based decisions. Load when a contributor or model needs to understand WHY the pilot's rules exist, what an OVN or REA is, what "share-alike" legally does, whether an identity/trust technology is safe to propose, or which governance ideas are settled versus exploratory. Do NOT load for the pilot's operational change-control rules (use iow-pilot-provenance-and-attribution), ODIN's own architecture decisions (use odin-commons-contract), or WEAVE's open research problems (use weave-research-frontier).
---

# Commons Governance Reference

This is the domain-theory pack for the ODIN Isle of Wight pilot. It explains the ideas
the project is built from — commons governance, open value networks, open value
accounting, mutual credit, self-sovereign identity, copyleft, and consent-based
decision-making — **as they apply to this project**, not as a textbook.

A mid-level contributor or a Sonnet-class model can do the pilot's day-to-day work
without this skill. Load it when you need to understand *why* a rule exists, evaluate
a proposal against the project's theory, or explain the project to an academic,
funder, or partner without overselling it.

## When NOT to use this skill

| You need... | Use instead |
|---|---|
| The pilot's actual change-control rules (provenance timing, file naming, question map, licence practice) | `iow-pilot-provenance-and-attribution` |
| ODIN's own load-bearing architecture decisions and their rationale (Holochain preference, Hexagon, PhD-as-Commons, known weak points) | `odin-commons-contract` |
| WEAVE's open research problems (AVE, RPI, governance-mode comparison, backtesting) | `weave-research-frontier` |
| The history of what was decided, when, and what died | `odin-decision-archaeology` |

## How to read this skill (tier discipline)

Every project claim below names its source and tier, per the project's evidence rules:

- **Tier 1** — the IoW-pilot repo (README.md, CONTRIBUTING.md, provenance-template.md,
  question-map.md, ovn-contributions.md, LICENSE). Canonical and operational.
- **Tier 1-adjacent** — the Dawn repo (ODIN Constitution v0.1 draft, ODIN Core Protocol
  v0.1 working draft, Influence_Codex.md). Canonical for ODIN-global but older; the
  pilot repo wins on pilot matters. The Constitution is **draft v0.1, unratified**.
- **Tier 2** — "At Dawn We Build" (the practice-based PhD proposal, drafted, never
  submitted). Canonical but aspirational.
- **Tier 3** — exploratory ChatGPT chat exports from 2025 (`Archive\RAW\`). Ideas, not
  facts. Anything cited only from Tier 3 is labelled **unconfirmed** with its date.

Statements about the general literature (Ostrom, REA accounting, copyleft law, mutual
credit, sociocracy) are labelled **general knowledge** — established outside the
project, summarised here for convenience.

Statuses are date-stamped **as of 2026-07-03**. As of that date: no pilot sessions
have run, no ODIN node is live, and the pilot repo contains exactly two OVN log
entries, both by the founder (Phase 1 discovery, 2026-07-03; ovn-contributions.md,
Tier 1).

---

## 1. Ostrom's commons principles

**General knowledge.** Elinor Ostrom's *Governing the Commons* (1990) studied how
real communities govern shared resources without privatisation or state control. From
long-lived cases she derived eight "design principles" found in successful commons:

1. **Clearly defined boundaries** — who is a member, and what the resource is.
2. **Congruence between rules and local conditions** — rules fit the actual place,
   and what people put in relates to what they take out.
3. **Collective-choice arrangements** — those affected by the rules can participate
   in changing them.
4. **Monitoring** — resource use and rule compliance are actively watched, by
   monitors accountable to the community.
5. **Graduated sanctions** — rule-breakers face escalating consequences, starting
   gentle, applied by the community.
6. **Conflict-resolution mechanisms** — cheap, rapid, local ways to resolve disputes.
7. **Minimal recognition of rights to organise** — outside authorities do not
   undermine the community's right to make its own rules.
8. **Nested enterprises** — for larger systems, governance is layered: local units
   inside wider coordinating structures.

Ostrom is cited directly in both "At Dawn We Build" (Tier 2, reference list) and
WEAVE.md (Tier 2, reference list). The pilot's design is a deliberate, if partial,
Ostrom implementation. Here is the honest scorecard, as of 2026-07-03:

| Principle | Status in the IoW pilot | Evidence |
|---|---|---|
| 1. Boundaries | **Operationalised.** The repo *is* the resource boundary; the attribution chain defines membership. Contributor IDs (adults: name/handle; children: school code + year group) define who is inside the commons; CC BY-SA defines the terms of entry and exit. | CONTRIBUTING.md, Tier 1 |
| 2. Congruence | **Designed, untested.** Rules are written for this exact context (child contributors, school sessions, same-day provenance) — but no session has run, so fit with local conditions is unverified. | CONTRIBUTING.md, Tier 1; Phase 1 discovery, 2026-07-03 |
| 3. Collective choice | **Open.** Anyone may fork or PR the rules (CONTRIBUTING.md invites it), and the ODIN Constitution drafts a consent protocol (§3.2) — but the Constitution is unratified and, in practice, one founder holds change control. This is a known weak point, owned by `odin-commons-contract`. | CONTRIBUTING.md, Tier 1; Constitution v0.1 draft, Tier 1-adjacent |
| 4. Monitoring | **Operationalised.** Public provenance is the monitoring mechanism: same-day provenance commits, field notes committed before comparison, a public OVN log, and a git history anyone can audit. Monitoring is done by the commons itself, at zero marginal cost. | CONTRIBUTING.md, provenance-template.md, ovn-contributions.md, Tier 1 |
| 5. Graduated sanctions | **ABSENT — an honest gap.** The pilot has a "what not to do" list but no sanction ladder: nothing says what happens the first, second, or third time someone commits an unprovenance'd file or starts a build early. The Constitution's orientation is "repair over punishment" (Principles, "Trust is a Network Effect", draft) and the Protocol drafts a mediated resolution process (§7, working draft), but neither is ratified, and neither is graduated. Anyone designing enforcement should read Ostrom's principle 5 first: start gentle, escalate slowly, keep it communal. Do not import platform-style bans. | CONTRIBUTING.md, Tier 1; Constitution v0.1 draft and Core Protocol v0.1 working draft, Tier 1-adjacent |
| 6. Conflict resolution | **Draft only.** Protocol §7 (working draft) names an "open forum or Guardian channel" and bi-annual protocol review — but no Guardians exist and the Hex Council has never been inaugurated. Nothing operational. | Core Protocol v0.1 working draft, Tier 1-adjacent; Phase 1 discovery, 2026-07-03 |
| 7. Right to organise | **Partly in place.** Internally, forking is declared a right and CC BY-SA makes it legally real. Externally — recognition by schools, the local authority, and funders — entirely untested; no school has even been contacted. | Constitution §6.2 (draft), Tier 1-adjacent; LICENSE, Tier 1; Phase 1 discovery, 2026-07-03 |
| 8. Nested enterprises | **Aspirational.** The node/network architecture (autonomous nodes, peer validation by ≥2 nodes, Hexagon coordination) is exactly a nested design — on paper. One node exists (this pilot) and it has not run a session. | Core Protocol v0.1 working draft, Constitution v0.1 draft, Tier 1-adjacent |

**Practical use:** when someone proposes a new rule or tool for the pilot, check it
against this table. Proposals that strengthen principles 5 and 6 (sanctions, conflict
resolution) fill real gaps. Proposals that weaken 1 or 4 (blur the boundary, make
monitoring private) should be blocked — they attack the parts that already work.

---

## 2. Open value networks (OVNs)

**Definition.** An open value network is a peer production structure in which value is
co-created by fluid contributors rather than employees, and every contribution is
transparently logged so that recognition (and any eventual reward) can flow back to
contributors in proportion to what they actually did. Contributions are not confined
to job titles; they are recorded events on an open ledger. (General knowledge;
the project's own gloss is in Influence_Codex.md Part IV §11, Tier 1-adjacent:
"Contribute what you can. Receive what you need. Coordinate through trust.")

**Lineage.** The OVN model was pioneered by **Sensorica**, a Montréal open hardware
network, from 2011 onward, and its accounting layer evolved into the **Valueflows**
vocabulary and **hREA** (the Holochain implementation of Resource-Event-Agent
accounting). ODIN's corpus contains a long review of Sensorica's economic model
(*Sensorica Economic Model Review.md*, Tier 3, 2025) covering their design→validation→
certification NFT pipeline and hREA integration. **Treat Sensorica's model as a design
template only. No partnership, contact, or collaboration with Sensorica exists — the
review is an unconfirmed Tier-3 study document, and nothing in Tier 1 or the Phase 1
answers establishes any relationship.**

**The Resource-Event-Agent (REA) model in one paragraph.** (General knowledge — REA
originates in accounting research, McCarthy 1982, and underpins Valueflows/hREA.)
REA replaces double-entry bookkeeping with three primitives: **Agents** (people,
groups) perform **Events** (create, transfer, use, consume) that affect **Resources**
(designs, documents, materials, time). An economy is then just the graph of who did
what to what, when. Because every event names its agent, attribution is not an
add-on — it is the data model. This is why ODIN's corpus keeps returning to hREA: an
agent-centric ledger of events is structurally identical to an attribution chain.

**How the pilot applies this.** The pilot's `ovn-contributions.md` (Tier 1) is a
**minimal OVN ledger** — deliberately minimal. Each row is an REA event:

| REA primitive | ovn-contributions.md column |
|---|---|
| Agent | Contributor ID |
| Event (type + time) | Type + Date |
| Resource / context | Session ref + Description |

No tokens, no smart contracts, no software — a markdown table in a public git repo.
That is the point: the pilot tests whether the *discipline* of open value accounting
works with children's contributions in schools, before any technology is layered on.
The repo describes the log as "the backbone of attribution... updated after every
session and before any external partner joins a build phase" (ovn-contributions.md,
Tier 1). As of 2026-07-03 it holds two entries, both dated 2025-03-30, both by the
founder (SeaWizard-ODIN).

---

## 3. Open value accounting

**Definition.** Open value accounting is the practice side of an OVN: recording all
contributions — including kinds a payroll would never see — in a transparent,
public, pluralistic ledger, so value is *recognised* even where it is not *paid*.
The ODIN Constitution commits to it directly: "All projects and nodes shall strive to
account for inputs and outputs in transparent, pluralistic ways, including
non-monetary forms of value such as time, trust, and care" (§5.2, draft v0.1,
unratified, Tier 1-adjacent) and "Ghost labour shall not exist here" (§5.1, same).

**Value recognition without wages.** Nobody in the pilot is paid from the ledger, and
the ledger creates no financial claim. What it creates is a permanent, public,
licence-protected record that a specific agent made a specific contribution on a
specific date — and CC BY-SA then drags that attribution through every fork and
derivative ("All contributors retain attribution through every fork and derivative",
ovn-contributions.md, Tier 1). If value is ever monetised downstream (a Pooseidon
build, a commercial partner), the ledger is the evidence base for who is owed
recognition. Recognition-first, reward-maybe-later is the standard OVN posture
(general knowledge), and it is the pilot's explicit design.

**The six contribution types** (ovn-contributions.md, Tier 1) map the whole value
chain of a session-to-build pipeline, not just "work product":

| Type | Covers | Open-value point |
|---|---|---|
| `conceptual` | ideas, questions, framings, hypotheses | A child's question is a logged economic event — the pilot's core wager |
| `design` | drawings, annotated sketches, system designs, proposals | The bridge from session artefact to buildable thing |
| `fabrication` | physical building, prototyping, manufacturing | Where external partners (hackspaces) typically enter |
| `deployment` | installing, operating, maintaining in the field | Ongoing labour that conventional credit systems forget |
| `documentation` | field notes, provenance records, write-ups, photography | Meta-labour: the accounting is itself accounted for |
| `facilitation` | session design, delivery, community coordination | Care/coordination labour — the classically invisible kind |

Note that `documentation` and `facilitation` being first-class types is Constitution
§5.1/§5.2 (draft) made operational: the categories exist precisely to catch labour
that wage accounting renders invisible.

---

## 4. Mutual credit

**Definition (general knowledge).** Mutual credit is a currency design in which money
is created at the moment of trade between members rather than issued by a bank: when
A does something for B, A's balance goes up and B's goes down by the same amount, so
all balances sum to zero and the "money" is simply a record of who has given more
than they have received. LETS schemes and business barter rings are the classic
implementations; Holochain's ancestry (MetaCurrency, and currency designer Art Brock)
is steeped in it.

**Status in ODIN: concept stage only. Nothing is built.** The idea appears in:

- "At Dawn We Build" (Tier 2) as a *research question*, not a plan: "How do concepts
  like self-sovereign identity, open value accounting, and mutual credit need to be
  adapted when the goal is not scale or efficiency — but care, impact, and meaning?"
- Tier-3 chats (2025, unconfirmed) that sketch a "mutual credit ledger prototype"
  among possible ODIN tools, and outreach drafts to Art Brock referencing currency
  design (*Networking and Currency Design.md*, Tier 3, 2025 — the outreach was never
  confirmed as sent or answered; no advisory relationship exists, Phase 1 discovery,
  2026-07-03).

There is no mutual credit system in the pilot repo, no design document, no prototype.
If you are asked about "ODIN's currency", the correct answer is: **there isn't one;
mutual credit is a labelled, unbuilt concept**, and the Tier-2 research question —
adapting it for care rather than scale — is the required starting point for anyone
who ever picks it up.

---

## 5. Self-sovereign identity (SSI) — and the standing caution

**Definition (general knowledge).** Self-sovereign identity is a model of digital
identity in which the individual — not a platform, state, or corporation — holds and
controls their identifiers, credentials, and the choice of what to disclose to whom.
It is usually implemented with decentralised identifiers and verifiable credentials,
often on distributed ledger technology (DLT).

**ODIN's design orientation.** The Constitution makes SSI a stated direction:
"No central authority may claim ownership over an individual's data, identity, or
contributions... All infrastructure must support **self-sovereign identity**, agency,
and informed consent" (§2.1, draft v0.1, unratified, Tier 1-adjacent). The
Influence_Codex (Part IV §12, Tier 1-adjacent) carries the same commitment: "ODIN's
network doesn't track users. It recognises agents."

**The standing caution — THE critical lens for all identity/trust tech in ODIN.**
The founder's KCL MSc dissertation (Pearce 2021, *Self-Sovereign Identity and
Distributed Ledger Technology in Humanitarian Identity Management: A Thematic
Analysis of the Literature*, King's College London — cited and summarised in
"At Dawn We Build", Tier 2) examined DLT/SSI deployments in refugee and humanitarian
contexts and found that while these technologies are framed as emancipatory, their
implementation often "**reinforces existing hierarchies, facilitates experimentation
on vulnerable populations, and embeds private and state interests**" within systems
of aid and identification — surveillance, securitisation, and extraction wearing the
costume of empowerment.

This is not background reading. It is the project's own founding critique, and it
binds every future proposal:

- **Any** identity, credentialing, reputation, or trust technology proposed for ODIN
  or the pilot must be assessed against the dissertation's finding: does this system
  actually shift power to its subjects, or does it create new surveillance and
  extraction surfaces while claiming to dissolve hierarchy?
- The bar is **highest for anything touching children**. The pilot's participants are
  children in state schools — a vulnerable population by definition. The dissertation
  finding says vulnerable populations are precisely where "emancipatory" identity
  tech does its worst harm. Safeguarding rules outrank everything, including
  attribution (see `iow-pilot-safeguarding-and-ethics`).
- Note what the pilot actually does today: **data minimisation, not identity
  technology**. Children are identified only as school code + year group (e.g.
  `GUR-P-Y5`) — never names (CONTRIBUTING.md, Tier 1). No SSI system exists or is
  planned for the pilot. The low-tech answer is the current answer; anyone proposing
  to "upgrade" it carries the burden of proof under the KCL lens.
- The project's recorded consent doctrine points the same way: "No agent, human
  or artificial, may assemble, share, or infer another agent's identity, history,
  or attestations without their explicit and ongoing consent" — **Tier-3 draft
  language** (*Research Proposal Creation.md*, 2025, unconfirmed), recorded as
  doctrine in the Phase 1 discovery brief (2026-07-03). The sentence does **not**
  appear verbatim in the Constitution v0.1 file in the Dawn repo snapshot —
  verify the current Constitution text before quoting it as a clause
  (`iow-pilot-safeguarding-and-ethics` handles it the same way).

If you remember one thing from this section: **ODIN is SSI-sympathetic in principle
and SSI-sceptical in deployment, on the strength of its founder's own research.**
"Holochain Preferred, Not Prescribed" (Constitution §4.4, draft) carries the same
posture on the ledger side — see `odin-commons-contract` for that rationale.

---

## 6. Copyleft mechanics

**The pilot's licence is CC BY-SA 4.0** (Creative Commons Attribution-ShareAlike 4.0
International — LICENSE, Tier 1). This is settled, Tier-1 fact.

**How share-alike actually propagates (general knowledge, applied).** BY-SA is a
copyleft licence. Mechanically:

1. Anyone may use, share, and adapt the material — including commercially.
2. Every use must credit the original creators. In this repo, credit is carried by
   the provenance records, the OVN log, and the file names themselves ("The name is
   the attribution", CONTRIBUTING.md, Tier 1).
3. Any *adaptation* (derivative) must be released under the same licence (or one
   Creative Commons designates as compatible). This is the "viral" step: a hackspace
   that turns a child's buoy sketch into a CAD file must license the CAD file BY-SA;
   a company that turns the CAD file into a product manual must license the manual
   BY-SA. Attribution and openness propagate through the whole derivative chain,
   automatically, without anyone policing it — the licence does the enforcement.
4. **No added restrictions.** You may not apply legal terms or technological measures
   (DRM, restrictive terms of use) that legally prevent others from doing anything
   the licence permits. This is why CONTRIBUTING.md (Tier 1) commands: "Do not add a
   licence that is more restrictive than CC BY-SA 4.0." It is not a preference; a
   more restrictive downstream licence is *invalid* over BY-SA material, and adding
   one breaks the promise made to the children who contributed first. CONTRIBUTING.md
   calls this "the copyleft of the commons. It protects everyone who contributed,
   especially those who contributed first."

**Contrast 1 — the Peer Production License (PPL).** The ODIN Core Protocol v0.1
(**working draft**, Tier 1-adjacent, §4) lists "Optional Peer Production License for
commercial limitation" alongside CC BY-SA. The PPL (general knowledge: Kleiner's
"copyfarleft" licence) allows free use by commons-based collectives and cooperatives
but restricts commercial exploitation by conventional capitalist firms unless they
reciprocate. Two things to hold clearly:

- It is **draft ODIN-global language**, not pilot policy. The pilot repo licenses
  everything BY-SA, full stop.
- A PPL is *more restrictive* than BY-SA (it limits commercial use by class of
  actor). It therefore **cannot be applied to pilot content** without violating the
  Tier-1 "no more restrictive licence" rule. If ODIN-global ever adopts an optional
  PPL for other materials, that is a decision for the (unratified) consent process —
  and it still could not retroactively touch anything already released BY-SA.

**Contrast 2 — the "ODIN General Commons License v1.0": dead. Never use it.** A
bespoke licence by this name was drafted in a Tier-3 chat (*Global Democracy Paddle
Play Test.md*, 2025, unconfirmed). It was **superseded by CC BY-SA 4.0** in Tier 1
(LICENSE) and must never be presented as live, proposed, or available. Custom
licences fragment the commons and are legally untested; the project chose a
standard, court-tested licence instead. If you find the OGCL referenced anywhere,
treat it as decision archaeology (see `odin-decision-archaeology`), not an option.

---

## 7. Delegative/liquid democracy and consent-based decision-making

**Delegative (liquid) democracy — definition (general knowledge).** A governance
model blending direct and representative democracy: every member may vote directly
on any issue, or delegate their vote to someone they trust — per topic if desired —
and may revoke or reassign that delegation at any time. "Liquid" because voting
power flows and re-pools continuously rather than being locked in for an electoral
term.

**Consent-based decision-making — definition (general knowledge).** From the
sociocracy tradition: a proposal passes not when everyone enthusiastically agrees
(consensus) but when **no one has a reasoned, paramount objection**. Objections are
treated as information that improves the proposal, not as vetoes to be defeated.

**Where ODIN actually uses these.** One place, and it is a draft: the Constitution's
**Consent-Based Decision Protocol** (§3.2, draft v0.1, unratified, Tier 1-adjacent) —
a textbook consent process (proposals meet Consent/Concern/Block signals) with one
ODIN-specific tightening: a Block must include a constructive alternative. The full
five-step protocol and its Hexagon context live in `odin-commons-contract` — do not
restate it from memory; read it there.

Remember its status honestly: the Constitution is draft v0.1,
unratified — never call it "unwritten", never call it ratified. No Hexagon council
has been inaugurated, and no record exists of any decision ever run through this
protocol (inference from Phase One.md — the Hexagon was never inaugurated — and
Phase 1 discovery, 2026-07-03). The pilot repo itself has **no** formal
decision protocol; in practice the founder holds change control.

**Tier-3 liquid-democracy designs — exploratory only.** A 2025 chat (*Delegative
Democracy Explained.md*, Tier 3, unconfirmed) sketches mechanisms for a future ODIN
governance layer: reputation-based and topic-scoped delegation, delegation decay and
instant revocability, quadratic/weighted voting, challenge quorums with rotating
citizen juries, contribution-weighted influence, and SSI-backed
one-person-one-vote. None of this is designed, decided, or built. Treat it as an
idea inventory for future work — and note that the SSI-backed voting idea must clear
the KCL-dissertation lens (section 5) before it goes anywhere. WEAVE's concept note
also cites "recent work on liquid democracy, trust metrics, and decentralised
coordination systems" among its references (WEAVE.md, Tier 2) — evaluating such
mechanisms experimentally is WEAVE's research territory, not the pilot's operations:
see `weave-research-frontier` for the research angle.

**Practical use:** if a contributor proposes "let's vote on it", the ODIN-native
answer is the consent pattern (Consent/Concern/Block) — clearly labelled as drawn
from a draft, unratified Constitution — not majority voting and not any Tier-3
liquid-democracy machinery.

---

## Provenance and maintenance

Written 2026-07-03 from the Phase 1 discovery brief and the sources below. Volatile
facts are date-stamped in the text; here is what may drift and how to re-verify:

**Sources used (cite these, in this priority order):**
- Tier 1: `README.md`, `CONTRIBUTING.md`, `ovn-contributions.md`,
  `provenance-template.md`, `LICENSE` in the IoW-pilot repo —
  canonical copy at github.com/ODINcommons/IoW-pilot (**local snapshots may be
  stale; check the GitHub repo first**).
- Tier 1-adjacent: `ODIN Constitution v0.1.md`, `ODIN Core Protocol v0.1.md`,
  `Influence_Codex.md` (Dawn repo, ODINcommons org; last commit 2025-09-12 as of
  writing).
- Tier 2: *At Dawn We Build* (PhD proposal, drafted, never submitted); `WEAVE.md`
  (concept note, July 2025).
- Tier 3 (all unconfirmed, 2025): *Sensorica Economic Model Review.md*, *Delegative
  Democracy Explained.md*, *Networking and Currency Design.md*, *Global Democracy
  Paddle Play Test.md* (in the ODIN archive, `Archive\RAW\` and `GlobalPong\`; see
  `odin-corpus-guide` for where the corpus lives and how to search it safely).
- General knowledge, labelled where used: Ostrom (1990) *Governing the Commons*;
  REA accounting (McCarthy 1982) / Valueflows / hREA; mutual credit and LETS;
  CC BY-SA 4.0 legal code (creativecommons.org/licenses/by-sa/4.0/); the Peer
  Production License; sociocracy/consent process; liquid democracy literature.

**What may drift, and how to re-check:**
- **Constitution ratification.** This skill says draft v0.1, unratified. If the Dawn
  repo (or a successor) shows a ratified version, sections 1 (principle 3), 5 and 7
  need rewriting. Check the Dawn repo's commit history.
- **OVN log contents.** "Two entries, both by the founder" will be false the moment
  sessions run. Re-read `ovn-contributions.md` before quoting counts.
- **Graduated sanctions and conflict resolution (the honest gaps).** If CONTRIBUTING.md
  or a new Tier-1 document adds an enforcement or dispute process, update the Ostrom
  scorecard (section 1).
- **Sensorica.** This skill states no partnership exists. If a real relationship
  forms, it will appear in Tier 1 (OVN log / README) or Phase-1-style founder
  answers — never trust a Tier-3 or AI-generated claim of partnership.
- **Licensing.** CC BY-SA 4.0 is settled Tier 1. Any change would appear in LICENSE
  in the pilot repo. The PPL remains draft-optional at ODIN-global level; the OGCL
  remains dead regardless.
- **Mutual credit / SSI builds.** Both are marked unbuilt. Before repeating that,
  check the pilot repo and ODINcommons org for new repos or design docs.

Maintenance rule inherited from the discovery brief: **no status claim (sessions run,
partnerships live, systems built) may be stated from Tier-3 or AI-generated sources.**
If Tier 1 or a founder answer does not confirm it, it has not happened.

*This skill is part of the ODIN commons and is licensed CC BY-SA 4.0, like everything
else here. Fork it, adapt it — just carry the attribution.*
