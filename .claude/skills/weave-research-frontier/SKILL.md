---
name: weave-research-frontier
description: Open research problems where the WEAVE programme (World Empowerment & Aggregated Voting Experiment) could advance the state of the art. Load this when working on WEAVE metrics (AVE, Return Potential Index / RPI), the P.A.P.P.T. governance simulation, backtesting against historical decisions, governance-mode comparison, or connecting IoW pilot session data to WEAVE research. Also load when asked "what is WEAVE", "what is RPI", "what research could this project produce", or when scoping a paper, PhD chapter, funding bid, or prototype connected to collective-decision metrics or governance simulation.
---

# WEAVE research frontier

Open problems where this project could genuinely advance the state of the art — and exactly where each one stands, so you never claim more than exists.

**Who this is for:** a contributor or AI maintainer with zero prior context who needs to pick up a WEAVE research thread, scope it honestly, and take the first concrete steps using only this corpus.

## Ground truth first — read before doing anything

As of **2026-07-03**:

- **WEAVE is a concept note.** The canonical text is `WEAVE.md` (and WEAVE-1.pdf, July 2025) in the ODIN corpus (`Documents\ODIN\GlobalPong\`) — Tier 2: canonical but aspirational. No simulation exists. No code exists. No metric is defined.
- **P.A.P.P.T.** (Pong Audience Paddle Play Test) is listed in WEAVE.md §9 as a "simulation metaphor" (Tier 2). Its only substantive treatment is an archived ChatGPT conversation, `Global Democracy Paddle Play Test.md` (Tier 3 — exploratory chat, 2025-02-09 to 2025-04-11). Everything sourced from that chat is **unconfirmed and exploratory**, not project fact.
- **The IoW pilot has not yet produced data.** README.md status (Tier 1): "First sessions planned for 2026". No sessions have run (Phase 1 discovery, 2026-07-03). The `sessions/` folder does not exist yet.
- **Every milestone in this skill is unstarted.** That is the point: this is a frontier map, not a progress report.

Definitions used throughout (each defined once here):

- **WEAVE** — World Empowerment & Aggregated Voting Experiment: "a simulation framework for prototyping and stress-testing collective intelligence systems at planetary scale" (WEAVE.md §1 v2, Tier 2).
- **ODIN** — Open Distributed Impact Network, the "applied deployment context" for WEAVE (WEAVE.md §4, Tier 2).
- **P.A.P.P.T.** — Pong Audience Paddle Play Test: governance-simulation metaphor where the ball is a shared global challenge and the paddle is collective governance.
- **AVE** — Average Variance Extracted: named as a candidate metric in WEAVE.md; undefined as a WEAVE method (see Problem 1).
- **RPI** — Return Potential Index: coined in the P.A.P.P.T. chat; undefined as a method (see Problem 1).
- **SOLE** — Self-Organised Learning Environment (Sugata Mitra's method), the session format of the IoW pilot (README.md, Tier 1).
- **Tier discipline** — every claim below names its source document and tier. Tier 1 = canonical repo documents; Tier 2 = canonical but aspirational concept documents; Tier 3 = exploratory chat exports, never project fact unless corroborated.

## WEAVE's research questions, verbatim

From WEAVE.md §2 (Tier 2) — quote these exactly when citing WEAVE's aims; do not paraphrase them into stronger claims:

> - Can distributed, trust-sensitive democratic systems exhibit greater adaptability, foresight, and responsiveness than nation-state models under crisis scenarios?
> - How can aggregated input from global participants be evaluated for signal strength, coherence, and long-term impact?
> - Can a simulation-based methodology (using game metaphors like Pong) reveal patterns of emergent collective intelligence?
> - What metrics (e.g. Average Variance Extracted, Return Potential Index) are most useful in evaluating collective decision performance?
> - How might this system integrate with, and inform, real-world governance frameworks such as ODIN (Open Distributed Impact Network)?

Note the phrasing of the fourth question: the metrics are **candidates inside an open question**, not methods the project possesses.

---

## Problem 1 — Defining and validating AVE and the Return Potential Index

**Status: open. Neither metric is defined anywhere in the corpus. Defining them is the work.**

### Why current approaches fall short

Collective-intelligence research has plenty of outcome measures (task accuracy, prediction-market calibration, the "c factor" of group performance) but no accepted composite metric for the *quality of a governance decision* that is independent of whether the outcome happened to go well. Outcome-only scoring rewards luck and punishes principled decisions that met bad fortune; process-only scoring can bless well-run deliberations that produced disasters. A defensible metric that combines both, and can be computed on real deliberation records, does not exist off the shelf.

**An honesty note on AVE, stated plainly.** "Average Variance Extracted" has an established meaning in structural-equation modelling: it is a convergent-validity statistic (the average proportion of variance in a set of indicators explained by their latent construct — general knowledge, labelled as such). WEAVE.md names AVE in a research question and in Objectives ("Develop and test new evaluation metrics for collective judgement (e.g., AVE, meta-feedback loops)" — Tier 2) but never says whether it intends the SEM statistic, a repurposing of it, or a new collective-decision metric that happens to share the acronym. **That ambiguity is itself undetermined. The first step is to decide and document which is meant.** Do not resolve it silently in either direction.

**RPI's full provenance.** RPI appears nowhere in Tier 1 or Tier 2 as a method. Its only trace is the P.A.P.P.T. chat (Tier 3, unconfirmed, Feb–Apr 2025), where it is proposed as the "Principled Metrics" layer of a three-layer evaluation — scoring decisions on meta-values independent of outcomes:

> "Inclusion (Did all voices get heard?) … Transparency (Were assumptions clear?) … Foresight (Did it consider long-term impacts?) … Cohesion (Did it reduce fragmentation and fear?) … We might call these the Return Potential Index (RPI) — a kind of metapaddle performance score." (Global Democracy Paddle Play Test.md, Tier 3, unconfirmed)

That is the entire published definition. Four named meta-values, no operationalisation, no scale, no aggregation rule, no validity evidence.

### ODIN/IoW's specific asset

The IoW pilot is designed to produce exactly the data such a metric needs for a first pilot computation: same-day, verbatim, attributed, timestamped records of self-organised group deliberation (question-map.md and provenance-template.md, Tier 1). Almost no metric-development effort in this space has honest, provenance-complete deliberation records to compute against; this project will, if the pilot runs (see Problem 5).

### First three steps in this corpus

1. **Write a decision memo on AVE's intended meaning.** One page: the SEM definition (labelled general knowledge), the WEAVE.md quotes, the options (adopt / adapt / rename), and a recommendation. This is a documentation task, not a maths task — it belongs in the corpus so the ambiguity is never re-litigated.
2. **Draft an operational definition of RPI** from the Tier 3 sketch: for each of inclusion, transparency, foresight, cohesion, specify what observable in a deliberation record counts as evidence, how it is scored, and how the four combine. Label the whole draft as building on an unconfirmed Tier 3 idea (Feb–Apr 2025) until the founder confirms the lineage.
3. **Specify the validity argument in advance**: what would convince a sceptical reviewer that RPI measures decision quality rather than, say, group verbosity? Name at least one convergent check and one discriminant check before touching data (hypothesis-before-session discipline — see odin-research-methodology).

### You have a result when…

…there exists a written operational definition of at least one metric, **plus** a pilot computation of it on real deliberation data (IoW session records or another documented deliberation corpus), **plus** a written validity argument that a third party could attack. Falsifiable failure mode: if two independent coders applying the definition to the same session record cannot agree within a stated tolerance, the definition has failed and must be revised — record that too.

---

## Problem 2 — P.A.P.P.T. mechanics: from metaphor to playable system

**Status: open. The metaphor exists; the mechanics do not.**

### Why current approaches fall short

Governance games and civic simulations exist (labelled general knowledge: serious-games work, Metagov's modular governance experiments, quadratic-voting trials), but there is no minimal, open, reproducible testbed in which *the same crisis scenario* is played under *different governance modes* with all aggregation rules published. Most demos hard-code one voting mechanism; comparisons across mechanisms are done on paper, not in a shared executable environment.

### What exists in the corpus

The metaphor, from the P.A.P.P.T. chat (Tier 3, unconfirmed, Feb–Apr 2025): "The ball = a shared global challenge… The paddle = collective governance… The paddle movement = collective decisions", with governance models as game modes. The chat sketches candidate aggregation modes ("Majority vote (slow parliamentary model), Leader control (autocracy), Delegative vote (liquid democracy), Direct live input averaging (hive democracy)"), candidate metrics (paddle responsiveness, ball returns, adaptation under stress), simulated events (multi-ball = compound crises), a proposed tech stack, and a "chaos-linked scenario engine" where scenarios feed each other. **All of it is a single AI-assisted brainstorm. Input aggregation, trust weighting, scoring, and the scenario engine are unspecified beyond that chat.** WEAVE.md (Tier 2) canonises only the label: "P.A.P.P.T. – Pong Audience Paddle Play Test (simulation metaphor)" (§9).

### ODIN/IoW's specific asset

A design lineage that already commits to openness: WEAVE.md proposes building on open platforms (§5), the pilot licence is CC BY-SA 4.0 (LICENSE, Tier 1), and the one rule — "Everything gets attributed before it gets built." (CONTRIBUTING.md, Tier 1) — means a P.A.P.P.T. prototype would carry its full design provenance, which is precisely what reproducible mechanism comparison requires.

### First three steps in this corpus

1. **Specify one minimal playable volley** on paper: one scenario, one ball trajectory, one decision window, exact input format (e.g. a slider position per participant per tick). Resist the chaos engine, AI agents, and trust weighting entirely at this stage — the Tier 3 chat's expansiveness is the anti-pattern.
2. **Choose and write down one aggregation rule per governance mode** for that volley (e.g. periodic majority vote with a lag for "parliamentary"; single controller for "autocratic"; continuous mean of live inputs for "swarm"). Cite the Tier 3 sketch as inspiration, not specification.
3. **Define win/learn conditions**: what counts as returning the ball, and — more importantly — what is logged per volley so that a failed return still produces analysable data.

### You have a result when…

…a runnable prototype exists in which **two governance modes produce measurably different paddle behaviour on the same scenario**, with the difference visible in logged data, not just on screen. Falsifiable failure mode: if the modes' behaviour is statistically indistinguishable on the chosen scenario, the scenario or the modes are badly specified — that is itself a publishable negative result if documented.

---

## Problem 3 — Backtesting against historical nation-state decisions

**Status: open. Named in WEAVE.md; the methodology needs to be designed.**

### Why current approaches fall short

Counterfactual evaluation of governance is methodologically treacherous. You cannot observe the timeline where a different decision was taken; naive backtesting produces hindsight-flattered results ("the crowd would obviously have locked down earlier"). Existing comparative-politics work compares real polities to each other, not real polities to simulated participatory alternatives. There is no accepted protocol for scoring a simulated collective decision against a historical one honestly.

### What exists in the corpus

WEAVE.md Objectives (Tier 2): "Compare participatory outcomes to historical nation-state decisions across a set of backtested global scenarios." The P.A.P.P.T. chat (Tier 3, unconfirmed, Feb–Apr 2025) sketches a three-layer evaluation: **retrospective benchmarking** (compare to actual historical outcomes), **simulated predictive modelling** ("Score not based on certainty, but on probability-weighted future impacts"), and **principled metrics** (the RPI layer, Problem 1). Crucially, the chat itself flags the core honesty problem — "we can't know with certainty where the ball will hit until it's hit" — and the founder's own question in that chat ("how do you know if it would have created positive impacts") is the right one. The three-layer structure is a reasonable starting sketch, but it is Tier 3: treat it as a hypothesis about method, not a method.

### ODIN/IoW's specific asset

A documentation culture built for exactly this discipline: hypothesis-before-session logging and artefacts-as-primary-sources (see odin-research-methodology) mean predictions can be committed *before* outcomes are scored — the single strongest defence against hindsight bias, and one most simulation projects lack because they have no provenance infrastructure.

### First three steps in this corpus

1. **Write scenario selection criteria** before choosing any scenario: what makes a historical decision backtestable (documented decision point, documented information available *at the time*, measurable outcomes, plausible decision alternatives that were actually on the table)?
2. **Write the counterfactual honesty policy**: state explicitly that alternate timelines are unknowable; commit to probability-weighted claims with stated uncertainty, never point claims ("the participatory mode would have saved X lives" is banned phrasing — cross-ref odin-external-positioning).
3. **Pre-register one worked case**: pick one historical decision, log the evaluation protocol and predictions in the corpus *before* running any comparison, then run it.

### You have a result when…

…a documented backtesting protocol exists **plus** one worked historical case with stated uncertainty bounds, committed in pre-registered order (protocol first, results second, timestamps proving it). Falsifiable failure mode: if the worked case's conclusion flips under reasonable perturbation of the counterfactual assumptions, the protocol must say so in the write-up — a result whose sign depends on unstated assumptions is not a result.

---

## Problem 4 — Governance-mode comparison: operationalising "outperform"

**Status: open. The modes are named; the comparison criteria are not.**

### Why current approaches fall short

WEAVE's headline question — can distributed systems "outperform traditional governance models" (WEAVE.md §1, Tier 2) — is unanswerable as stated, because "outperform" bundles incommensurable goods: decision **speed**, **legitimacy** (who consented?), **foresight** (long-horizon quality), and **equity** (who bore the costs?). A mode can win on speed and lose on legitimacy (the chat's own observation that autocracies are swift but sacrifice "transparency, equity, and long-term resilience" is in WEAVE.md §1 v2, Tier 2). Comparative governance literature discusses these trade-offs qualitatively; a fixed, pre-registered, multi-criteria comparison on a shared scenario set has not been done because no shared executable scenario set exists (Problem 2 is the prerequisite).

### What exists in the corpus

WEAVE.md §5 Methodology (Tier 2): "Run parallel simulations with different governance modes: parliamentary, autocratic, decentralised swarm, etc." The P.A.P.P.T. chat (Tier 3, unconfirmed, Feb–Apr 2025) adds liquid/delegative modes: "Hive Democracy (Weighted / Delegated) — Influence is distributed dynamically based on trust, accuracy, or expertise (like Liquid Democracy)" and "Delegative vote (liquid democracy)" as an aggregation option.

### ODIN/IoW's specific asset

The RPI sketch (Problem 1) is, in embryo, a multi-criteria answer to exactly this operationalisation problem — inclusion, transparency, foresight, cohesion are candidate axes for "outperform". Defining the metric and defining the comparison are the same research programme approached from two ends; few projects have both halves under one roof.

### First three steps in this corpus

1. **Write the operationalisation memo**: for each of speed, legitimacy, foresight, equity (and any RPI axes adopted), one measurable proxy computable from P.A.P.P.T. volley logs. State explicitly that no single winner is expected — the deliverable is a trade-off frontier, not a champion.
2. **Fix the scenario set and mode definitions** (from Problems 2's prototype) and freeze them in a pre-registration document committed to the corpus before any comparison run.
3. **Decide the human-participation boundary**: which comparisons run with simulated agents only, and which require human participants (triggering ethics work — safeguarding and consent obligations outrank research; cross-ref iow-pilot-safeguarding-and-ethics before any human trial).

### You have a result when…

…a pre-registered comparison of at least two governance modes on a fixed scenario set has been executed, with all criteria, scenarios, and analysis choices committed before the runs, and results reported on every pre-registered criterion including the unflattering ones. Falsifiable failure mode: if results are reported on criteria chosen after seeing the data, the comparison is void — rerun under a new pre-registration.

---

## Problem 5 — IoW pilot data as WEAVE's first real-world trust-and-deliberation dataset

**Status: open. The pilot has not run; no data exists (Phase 1 discovery, 2026-07-03). This is the nearest-term problem and the only one with a live operational pathway.**

### Why current approaches fall short

WEAVE.md §5 (Tier 2) calls for piloting "small-scale tests with human users to model deliberation, feedback loops, and trust dynamics" — but WEAVE has no data-collection apparatus at all, and most collective-intelligence datasets are lab tasks or platform scrapes: short, decontextualised, consent-ambiguous, and stripped of provenance. Records of *self-organised* group deliberation with full same-day provenance are vanishingly rare.

### ODIN/IoW's specific asset

The IoW pilot's Tier 1 documentation machinery produces, by design, same-day, verbatim, attributed, timestamped records of self-organised group deliberation: the living question map ("It records them exactly as they were asked, by whom, and when" — question-map.md, Tier 1) plus per-session provenance records (provenance-template.md, Tier 1), under CC BY-SA 4.0. That is exactly the kind of data WEAVE lacks. This connection is not incidental: Phase 1 discovery (2026-07-03) names "IoW pilot data becoming WEAVE's first real-world trust/deliberation dataset or a defined+piloted metric (RPI/AVE)" as one of the four success criteria for the whole pilot. README.md (Tier 1) confirms the direction: pilot artefacts "are primary sources in an ongoing practice-based PhD inquiry" — but note the enrolment caveat: the PhD route is chosen and the application is dormant (proposal drafted, never submitted, Phase 1 discovery, 2026-07-03), so "ongoing... PhD inquiry" overstates the README's own status; never repeat it uncorrected (see odin-external-positioning).

**An honesty note on the bridge, stated plainly.** Children's classroom deliberation is not a global governance simulation. What transfers from a Year 5 SOLE on "who owns the water?" to trust-weighted planetary decision systems must itself be argued, case by case — the project's methodological commitment is **transferability, not generalisability** (At Dawn We Build, Tier 2; see odin-research-methodology). Any WEAVE analysis of IoW data must open with its transferability argument, not assume one.

### First three steps in this corpus

1. **Define what a "deliberation event" is in session data.** Write a codebook entry: is it a question being asked, a group converging on a sub-question, a disagreement being resolved? It must be identifiable from question-map entries and field notes without inference beyond the record.
2. **Specify an anonymisation-preserving dataset schema.** Contributor identifiers are school code + year group only (e.g. `GUR-P-Y5`), never names (CONTRIBUTING.md, Tier 1). Safeguarding outranks research — if a research need conflicts with the child-ID rules, the research need loses (cross-ref iow-pilot-safeguarding-and-ethics; note the school codes in CONTRIBUTING.md are placeholder examples — Phase 1 discovery, 2026-07-03).
3. **Log the research intention before the sessions.** Commit a hypothesis-before-session record stating what the WEAVE analysis will look for (e.g. which RPI axes are observable in SOLE deliberation) *before* the first session runs (discipline owned by odin-research-methodology). Retrofitted hypotheses are the failure mode this corpus was built to prevent.

### You have a result when…

…a first dataset release exists (schema-conformant, safeguarding-clean, CC BY-SA 4.0) **plus** one completed WEAVE-relevant analysis of it (e.g. a pilot RPI computation per Problem 1, or a documented deliberation-event catalogue) **plus** a written transferability argument for that analysis. Falsifiable failure mode: if the pre-logged hypothesis finds nothing, publish that — an honest null on real data is still WEAVE's first empirical result.

---

## Landscape note — where this sits (general knowledge, labelled as such)

Everything in this section is general knowledge as of the author's training, not corpus fact; verify before citing externally (cross-ref odin-external-positioning before making any comparative claim in public).

- **Metagov and RadicalxChange** (both named in WEAVE.md §9, Tier 2) run governance toolkits and democratic-mechanism experiments (modular governance, quadratic funding/voting). They study *mechanisms*; WEAVE's distinctive ambition is a *comparative simulation testbed* across mechanism families with published metrics. That comparative-testbed slot appears genuinely open.
- **Liquid democracy literature** has formal results (delegation cycles, concentration of power in super-voters) and small platform trials. The P.A.P.P.T. chat's delegative mode (Tier 3) would be a late entrant to a studied field — the open part is not liquid democracy itself but head-to-head simulation against other modes on shared scenarios.
- **Collective intelligence research** — Pentland's *Social Physics* and Helbing's globally-networked-risks work are cited in WEAVE.md §8 (Tier 2) — established that interaction patterns predict group performance and that networked risks cascade. Largely already studied: crowd accuracy on estimation tasks, prediction markets. Genuinely open: composite decision-quality metrics computable on real deliberation records (Problem 1), honest counterfactual backtesting protocols (Problem 3), and provenance-complete deliberation datasets from self-organised groups (Problem 5).
- **What this project should never claim**: that hive/swarm democracy is proven superior (WEAVE's own research questions are questions), that RPI exists as a method, or that any simulation has run. All external claims route through odin-external-positioning.

## When NOT to use this skill

| If you need… | Use instead |
|---|---|
| Rules for hypothesis logging, reflexive AI dialogue norms, artefacts-as-primary-sources, transferability doctrine | **odin-research-methodology** |
| What may be claimed publicly, to schools, funders, or supervisors | **odin-external-positioning** |
| Ostrom, OVNs, mutual credit, SSI, copyleft — governance and commons theory | **commons-governance-reference** |
| Running or documenting an actual IoW session | **iow-pilot-session-operations** and **iow-pilot-documentation-standards** |
| Child data rules, consent, DBS, safeguarding buildout | **iow-pilot-safeguarding-and-ethics** (supreme — outranks everything here) |
| Why the metrics/decisions history looks the way it does | **odin-decision-archaeology** |

## Provenance and maintenance

**Sources used, by tier:**

- Tier 1: `README.md`, `CONTRIBUTING.md`, `question-map.md`, `provenance-template.md`, `LICENSE` (IoW-pilot repo — canonical copy at github.com/ODINcommons/IoW-pilot; local snapshots may be stale).
- Tier 2: `WEAVE.md` / WEAVE-1.pdf (July 2025 concept note, ODIN corpus `Documents\ODIN\GlobalPong\`); "At Dawn We Build" PhD proposal (transferability doctrine).
- Tier 3 (unconfirmed, exploratory): `Global Democracy Paddle Play Test.md` (archived ChatGPT conversation, 2025-02-09 to 2025-04-11, ODIN corpus) — sole source for RPI's coinage, the three-layer evaluation sketch, P.A.P.P.T. mechanics ideas, and liquid/delegative modes. Nothing from it is project fact. It also contains an "ODIN General Commons License v1.0" — superseded by CC BY-SA 4.0 (Tier 1); never present it as live. It is also the register specimen for AI sycophancy ("Yes. This might be the most important idea I've ever helped someone shape.") — treat its enthusiasm as noise, not evidence.
- Phase 1 discovery answers, 2026-07-03 (founder): pilot success criteria including the WEAVE-dataset criterion; no sessions run; school codes are placeholders.
- General knowledge, labelled inline: the SEM meaning of Average Variance Extracted; the landscape note.

**What may drift, and how to re-verify:**

- *"No sessions have run; no data exists"* — dated 2026-07-03. Re-verify by checking for a `sessions/` folder and question-map entries at github.com/ODINcommons/IoW-pilot before repeating the claim.
- *"No metric is defined; no simulation exists"* — dated 2026-07-03. Re-verify by searching the IoW-pilot and ODINcommons repos for RPI/AVE definition documents or P.A.P.P.T. code before repeating.
- *WEAVE's status as concept note* — a submitted proposal, funded project, or published paper would change this; only Tier 1 documents or founder confirmation can upgrade it.
- *The landscape note* — external fields move; re-check Metagov, RadicalxChange, and liquid-democracy literature before any external comparative claim.
- If any milestone above is achieved, update this skill's status lines and record the achievement's provenance in the corpus first — attribution before building applies to research results too (CONTRIBUTING.md, Tier 1).

*Written 2026-07-03. British English. Licence of the pilot corpus: CC BY-SA 4.0.*
