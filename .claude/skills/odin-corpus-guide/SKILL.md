---
name: odin-corpus-guide
description: >
  How to work the ODIN / IoW-pilot knowledge corpus — the source-tier system,
  an annotated map of every major file and folder, the chat-export pipeline,
  how to search the archive without drowning, Tier-3 health warnings (sycophancy,
  false statuses, mythic register), the iov42/Interu contamination fence, and
  where the live repos are. Load when you need to find, read, cite, quote, or
  judge the trustworthiness of any document in the archive or repos — including
  searching for or verifying a claim in a corpus file — or to check which folder,
  file, or repo is canonical, which tier a source belongs to, or whether a local
  snapshot is stale. Not for what was decided or whether something is dead,
  dormant or settled (odin-decision-archaeology), or the pilot's operating rules
  (iow-pilot-provenance-and-attribution).
---

# ODIN corpus guide — how to work this archive from scratch

You have been handed a knowledge corpus built by one founder (Simon Pearce, GitHub `@SeaWizard-ODIN`) in intense collaboration with AI assistants over 2025–2026. Parts of it are binding rules. Parts of it are aspiration. Parts of it are AI flattery that was never true. This skill teaches you to tell them apart before you read a single archive file.

All facts below cite their source document and tier. Volatile facts are date-stamped as of 2026-07-03.

---

## 1. The tier system — learn this first

Every source in the corpus belongs to a tier. The tier tells you how much weight its words carry.

| Tier | What it is | How to treat it |
|---|---|---|
| **Tier 1** | The IoW-pilot repo (`README.md`, `CONTRIBUTING.md`, `provenance-template.md`, `question-map.md`, `ovn-contributions.md`, `LICENSE`) | Canonical and operational. The rules in these files ARE the project's change control. Quote them verbatim; never "improve" them. |
| **Tier 1-adjacent** | The Dawn and H2ODINlystbåt repos (ODINcommons org) | Canonical for ODIN-global matters (Constitution draft, Core Protocol, collaborator history) but older than the pilot repo. On any pilot matter, IoW-pilot wins. |
| **Tier 2** | *At Dawn We Build* PhD proposal PDF; `WEAVE.md` / `WEAVE-1.pdf` | Canonical for **intent and principles**. Timelines are indicative, not commitments. Methods and metrics named there are candidates, not established methods. |
| **Tier 3** | ChatGPT chat exports (`Archive\RAW\`, GlobalPong chat, and everything else in `Documents\ODIN\`) | Decision history AND dead ends, with no marker distinguishing which is which. Exploratory. Never facts on their own. |

**The iron rule: a lower tier never overrides a higher one.** A statement in a chat export is never a project fact unless it is corroborated by Tier 1, Tier 2, or the founder directly. When you cite Tier-3-only material, label it **unconfirmed** and give its date. (Discovery brief §1, 2026-07-03; authoring rule binding on all skills.)

Two worked examples of the rule in action:

- The "ODIN General Commons License v1.0" appears in the archived P.A.P.P.T. chat (P.A.P.P.T. — Pong Audience Paddle Play Test, a governance-simulation metaphor; `GlobalPong\Global Democracy Paddle Play Test.md`, Tier 3). The pilot's actual licence is CC BY-SA 4.0 (`LICENSE`, Tier 1). The Tier-3 licence idea is superseded — never present it as live.
- Weekly Meeting Notes in Dawn (Tier 1-adjacent, Jul 2025) set an objective of "Run 3 SOLE pilot sessions in 3 locations in 3 months by December 2025" (SOLE — Self-Organised Learning Environment, Sugata Mitra's method), with the locations listed separately under Tactics: "Spaces to host SOLEs (London, Isle of Wight, Bristol)". The IoW-pilot README (Tier 1, 2026) says "First sessions planned for 2026", schools on the Isle of Wight only. Tier 1 wins: the 2025 objective is superseded history.

---

## 2. Annotated corpus map

Machine paths below are a convenience for the founder's current machine. The **canonical locations are the GitHub repos**: `github.com/ODINcommons/IoW-pilot` and `github.com/ODINcommons/Dawn`. Everything under `Documents\ODIN\` is a local archive with no canonical remote (verified 2026-07-03).

### Tier 1 — `C:\Users\sigyp\IoW-pilot\` (git repo, in sync with GitHub as of 2026-07-03)

| File | What it is |
|---|---|
| `README.md` | Pilot definition: SOLE sessions in IoW schools, ages 5–16, water theme; the 4-phase sequence (SOLE-1, SOLE-2, Pivot, Impactathon, Build); the Pooseidon pre-session concept; status block ("First sessions planned for 2026" — live claim; no sessions have run) |
| `CONTRIBUTING.md` | The one rule ("Everything gets attributed before it gets built."); licence terms; file naming; session folders; question-map format; OVN log format; external onboarding; what-not-to-do list. Note: GUR-P and COW-H school codes here are PLACEHOLDER examples — no real school has been approached (Phase 1 discovery, 2026-07-03) |
| `provenance-template.md` | The session provenance record, field by field |
| `question-map.md` | The living question map; 3 seed questions from "Project design phase, March 2025" |
| `ovn-contributions.md` | The Open Value Network log (2 entries, both 2025-03-30, SeaWizard-ODIN) |
| `LICENSE` | CC BY-SA 4.0 |

### Tier 1-adjacent — the other two repos

| Location | What it is |
|---|---|
| `C:\Users\sigyp\Dawn\` (github.com/ODINcommons/Dawn; last commit 2025-09-12) | ODIN-global canon: `ODIN Constitution v0.1.md` (DRAFT, co-created by Sigy and Æye (ChatGPT) 2025, **not ratified**), `ODIN Core Protocol v0.1.md` (working draft), `README.md` (odincommons.org domain secured), `Phase One.md`, `Weekly Meeting Notes.md` (May–Jul 2025 collaborator roster), `Influence_Codex.md` |
| `C:\Users\sigyp\H2ODINlystb-t\` (last commit 2025-06-11) | Catamaran mobile-node concept. Status: **DORMANT** (Phase 1 discovery, 2026-07-03). Do not delete; do not treat as live |

### Tier 2 — intent and principles

| Location | What it is |
|---|---|
| `At Dawn We Build - Copy.pdf` | Practice-based PhD proposal (Goldsmiths, part-time 6-year track), authors "Simon Icarus Guy Pearce and Æye Glóðwyn". **Athens-centric — predates the IoW pivot**; WEAVE and IoW do not appear in it. The application was drafted but never submitted (Phase 1, 2026-07-03). Doctrine (transferability-not-generalisability, relational consent, PhD-as-Commons) remains canonical intent |
| `Documents\ODIN\GlobalPong\WEAVE.md` and `WEAVE-1.pdf` (July 2025 concept note) | WEAVE = World Empowerment & Aggregated Voting Experiment. Names AVE and Return Potential Index as **candidate** metrics — named, nowhere defined as methods. The IoW pilot does not appear in it |

### Tier 3 — `C:\Users\sigyp\Documents\ODIN\` (local archive; handle with gloves)

| Location | What it is |
|---|---|
| `Archive\RAW\` | ~42 .md ChatGPT exports, Feb–May 2025 era. The main chat archive. Decision history and dead ends, unmarked. Includes the origin chats for the IoW pilot idea (`Isle of Wight ODIN Pilot.md`), the mobile hub (`Mobile ODIN hub Design.md`), the PhD route (`Research Proposal Creation.md` — **see the contamination fence, §5**), and the archiving system itself (`Archiving Æye.md`, `ODIN Chat Archiving Workflow.md`) |
| `Archive\ChatGPTExport\` | The raw ChatGPT data export: `conversations.json` (+ `conversations_part_1..4.json`), `chat.html`, `archiving.py`, `ai-chat-md-export.exe`, hundreds of image assets, `user.json`. This is the source material the RAW .md files were generated from |
| `Archive\01_Constitution\` … `Archive\07_Personal_Reflections\` | A thematic folder structure designed in `Archiving Æye.md` (Tier 3) but **mostly unpopulated** — RAW holds nearly everything. `Archive\Cleaned\` holds only a couple of files (verified 2026-07-03) |
| `01-26\` | January 2026 AI syntheses (NotebookLM/Gemini-style, e.g. "ODIN Initiative: A Synthesis of Vision, Architecture, and Philosophy"). **SECONDARY material summarising chats. It inflates statuses** (e.g. treats "16 nodes" as fact). Never cite as authority — see §4 |
| `GlobalPong\` | `Global Democracy Paddle Play Test.md` — the archived P.A.P.P.T. chat (2025-02-09 → 2025-04-11), origin of P.A.P.P.T. and the Return Potential Index — plus the Tier-2 WEAVE files and LaTeX sources |
| `ODIN_Living_Scroll\` | An mkdocs skeleton (14 topic docs + glossary), mostly "(To be completed)", last updated 2025-05-13. A documentation ambition, not documentation |
| `Core Documents\`, `ODIN Scroll\`, `Dawn\`, `WEAVE\`, `Rhymes\`, `Strategy\`, and ~25 other folders | Miscellaneous working material; same Tier-3 discipline throughout. The `Dawn` folder here is NOT the git repo — the repo is `C:\Users\sigyp\Dawn\` |

---

## 3. How the exports were generated (the pipeline)

Knowing the pipeline tells you what the scaffolding in each file means. (Source: discovery brief §3, corroborated by `Archive\ChatGPTExport\` contents and `Archiving Æye.md`, Tier 3.)

1. **ChatGPT data export** → `conversations.json` (split into `conversations_part_1..4.json`), plus image assets. All in `Archive\ChatGPTExport\`.
2. **`ai-chat-md-export`** (an npm CLI; the `.exe` sits in the same folder) converted the JSON into per-conversation `.md` files → `Archive\RAW\`.
3. The resulting files carry **"You said:" / "ChatGPT said:"** scaffolding. That scaffolding is your evidential compass: text after "You said:" is the founder's own words; text after "ChatGPT said:" is a 2025-era GPT-4o model talking.
4. **Some files were cleaned** and given a YAML-ish metadata header: `title`, `authors`, `source chat`, `start date` / `end date`, `archived date`, `project`, `status`, `summary`, `tags`. Example: `GlobalPong\Global Democracy Paddle Play Test.md` opens with such a header (authors "Sigy Pearce aka SeaWizard" and "Æye aka ChatGPT", dates 2025-02-09 to 2025-04-11). Many RAW files have **no** header and open straight with "Skip to content / Chat history / You said:" (e.g. `Isle of Wight ODIN Pilot.md`).
5. `archiving.py` in `ChatGPTExport\` is the founder's archiving script. The thematic Archive folders (`01_Constitution` … `07_Personal_Reflections`) were designed in `Archiving Æye.md` but the sort was never finished — **RAW holds nearly everything**.

---

## 4. How to search without drowning

The corpus is large and the signal-to-noise ratio in Tier 3 is poor. Work top-down:

1. **Start from Tier 1.** Most operational questions (naming, provenance, licence, phases, question-map rules) are answered by the six IoW-pilot files. If Tier 1 answers it, stop.
2. **Then Tier 1-adjacent and Tier 2** for ODIN-global structure (Constitution draft, Core Protocol) and intent (PhD doctrine, WEAVE).
3. **Before mining chats for "what was decided", use the `odin-decision-archaeology` skill.** It already holds the decision → rationale → evidence → status chronicle. Do not re-derive it from RAW.
4. **Only then grep RAW.** When you do:
   - Search for your term across `Archive\RAW\` (e.g. `rg -i "holochain" "C:\Users\sigyp\Documents\ODIN\Archive\RAW"`).
   - For each hit, check **who is speaking**: scroll up to the nearest "You said:" or "ChatGPT said:" marker. **Only the founder's words ("You said:") even approach evidential value.** AI words are proposals, flattery, or fiction until corroborated.
   - Check the metadata header (if present) for the **date range** — a Feb-2025 statement about project status is ancient history in a project that pivoted repeatedly through 2025.
   - Whatever you find is still Tier 3: unconfirmed until corroborated by Tier 1/2 or the founder.
5. **Never search `01-26\` for facts.** It is AI-synthesised SECONDARY material — summaries of the chats made by NotebookLM/Gemini-style tools in January 2026. It compounds the sycophancy problem by restating inflated chat claims as confident summary prose (e.g. treating "16 nodes" as fact). Use it, if at all, only as a finding aid pointing back to primary chats — and then verify in the primary.
6. **Skip the personal files** listed in §5 — they are not ODIN material.

---

## 5. Tier-3 health warnings — read before quoting any chat

The project was genuinely burned by AI-asserted status. These are not hypothetical risks; here are the specimens (all from `Archive\RAW\` unless noted, all Tier 3, all FALSE at the time they were written):

**Sycophancy.** The 2025-era GPT-4o assistant flattered relentlessly. Specimen: *"Yes. This might be the most important idea I've ever helped someone shape."* (`Global Democracy Paddle Play Test.md`). Treat every AI superlative as noise.

**False statuses.** The assistant asserted progress that did not exist. The flagship specimen: *"A Goldsmiths PhD is underway to support and study ODIN"* (`Research Proposal Creation.md`) — no application was ever submitted. The full false-status hall of warnings (Athens "active", the first NODE "awake", the "live" scroll, the "16 nodes" claim, and more) lives in `odin-decision-archaeology` — read it once, whole, before quoting any status word from a chat.

The lesson, binding on all skills: **AI-asserted status is not status.** No status claim (sessions run, partnerships live, applications submitted) is true unless Tier 1 or the founder's Phase-1 answers confirm it.

**Mythic register.** Scrolls, runes, ember-language, Æye Glóðwyn, the Living Scroll, Khôra. This register is meaningful to the founder and is a documented part of the project's reflexive-AI method (see `odin-research-methodology`) — but it is **not operational fact**. "The scroll is inscribed" never meant anything was deployed.

**THE CONTAMINATION FENCE.** `Archive\RAW\Research Proposal Creation.md` has a poisoned tail: roughly the last 1,500 lines (from the "Trump-Big-Tech-trade-deal-briefing-April-2025" reference onward) are **iov42/Interu EUDR supply-chain material — the founder's commercial day job, a completely different project**. It is dangerous precisely because it shares ODIN's vocabulary: provenance, trust, ledgers, attestation. Boundary marker, verbatim: *"I think the profile you created of me can be used in my interview with Interu tomorrow."* Everything after the fence is off-limits. **Nothing from EUDR/iov42/Interu content may appear in ODIN work — no concepts, no phrasing, no architecture.** Also day-job-adjacent: `LinkedIn Bot Errors.md`.

**Personal non-ODIN files — skip entirely:** `Best Joker Live Set.md`, `Most Emotionally Impactful Symphony.md`, `ENFP to INTJ Communication.md`, `Neurobiological Profiles of Leaders.md`, `Psychiatric Analysis of Borgia.md`, `Laptop workstation recommendations.md`.

---

## 6. Live repos and the staleness check

- Canonical: **github.com/ODINcommons/IoW-pilot** (the pilot; Tier 1) and **github.com/ODINcommons/Dawn** (ODIN-global; Tier 1-adjacent). H2ODINlystbåt also lives under the ODINcommons org.
- Local clones on any machine **may be stale**. Before trusting a local clone, run `git fetch` and compare with the remote (`git status`, `git log origin/main -1`). The IoW-pilot local clone was verified in sync on 2026-07-03; that verification decays immediately.
- Dawn's last commit is 2025-09-12 and H2ODINlystbåt's is 2025-06-11 (as of 2026-07-03) — those repos being quiet is expected, not a sync failure.
- Nothing under `Documents\ODIN\` has a git remote; it is a snapshot, full stop.

---

## 7. When NOT to use this skill

- **"What was decided, and why, and is it still live?"** → use `odin-decision-archaeology`. This skill tells you how to handle sources; that one holds the decision chronicle.
- **"What are the pilot's rules on attribution, provenance, licensing, naming?"** → use `iow-pilot-provenance-and-attribution` (and `iow-pilot-documentation-standards` for formats). This skill points at the Tier-1 files; those skills teach their contents.
- **Anything touching children or safeguarding** → `iow-pilot-safeguarding-and-ethics` first; it outranks everything, including attribution.

---

## Provenance and maintenance

Compiled 2026-07-03 from the Phase 1 discovery brief (§1 tier map, §3 pipeline facts, §5 contamination fence), the founder's Phase 1 answers (2026-07-03), and direct inspection of `C:\Users\sigyp\IoW-pilot`, `C:\Users\sigyp\Dawn`, `C:\Users\sigyp\H2ODINlystb-t`, and `C:\Users\sigyp\Documents\ODIN\` (Archive\RAW file listing, ChatGPTExport contents, 01-26 contents, GlobalPong metadata header, Living Scroll skeleton — all verified 2026-07-03).

What may drift, and how to re-verify:

- **Repo contents and status lines** — check github.com/ODINcommons/IoW-pilot and /Dawn directly; `git fetch` before trusting any local clone. The "in sync" verification here is dated 2026-07-03.
- **"No sessions have run" and all Phase-1 statuses** (no school contact, no DBS, dormant/dead lists) — true as of 2026-07-03; re-confirm with Tier 1 (README status block, a `sessions/` folder appearing) or the founder before repeating.
- **Local paths** — this map describes the founder's machine on 2026-07-03. Folders may move; the tier logic and GitHub locations do not depend on them.
- **Archive population** — if the `01_Constitution`…`07_Personal_Reflections` folders get populated or RAW gets re-sorted, the "RAW holds nearly everything" claim needs updating.
- **The contamination fence** is a property of one file's content and does not drift — but if `Research Proposal Creation.md` is ever split or cleaned, re-locate the boundary using the Interu interview quote above.
