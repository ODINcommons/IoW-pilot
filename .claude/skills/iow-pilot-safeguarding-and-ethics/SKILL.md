---
name: iow-pilot-safeguarding-and-ethics
description: The absolute safeguarding and ethics constraints for the ODIN Isle of Wight pilot — working with children in UK state schools. Load this BEFORE any school contact, session planning, artefact handling, photography, committing of session material, consent question, DBS question, or any situation involving a child's identity, image, voice, or work. Also load when anonymisation rules, teacher identification, disclosure handling, a conflict between attribution and anonymity, or a parent, teacher, or school question about what data is kept, published, or deleted about children arises. Contains the pre-session verification checklist and the incident procedure for identifying content pushed to the public repo. This skill outranks every other skill in the library, including attribution rules.
---

# Safeguarding and ethics — ODIN Isle of Wight pilot

This is the most safety-critical document in this library. Nothing in any other
skill, and nothing in the repository, may weaken, caveat, or route around what
is written here. **Safeguarding outranks attribution** — see
[The one place the one rule bends](#the-one-place-the-one-rule-bends).

---

## ABSOLUTE RED LINES — read this box if you read nothing else

> **If you are mid-session on a phone, this box is your whole answer.**
>
> 1. **No child's name — anywhere, ever.** Children are identified by school
>    code + year group only (e.g. `GUR-P-Y5`). In every file, forever.
> 2. **Never photograph a child.** Photograph the work, never the person.
>    No faces, no bodies, no reflections, no children in the background.
> 3. **Never commit anything that could identify a child** — names on work,
>    handwriting with names visible, identifying voice recordings, uniform
>    badges, any distinctive detail. Crop or exclude first. When in doubt,
>    leave it out.
> 4. **Never be alone with a child.** School staff must always be present.
> 5. **If a child tells you something worrying (a disclosure), or you have any
>    concern about a child's welfare: report it to the school's Designated
>    Safeguarding Lead (DSL) immediately. Do not investigate. Do not promise
>    secrecy. Do not write it into project files.**
> 6. **If attribution and anonymity ever conflict, anonymity wins.**
> 7. **As of 2026-07-03 no safeguarding infrastructure exists** — no DBS
>    (Disclosure and Barring Service criminal-record) check, no consent
>    forms, no school agreement. **No session may run until it does.** See
>    Layer 4 and the Pre-session verification checklist.

---

## How this skill is organised

Four layers, in descending order of documentary authority. **Never blur
them.** When you state a rule, know which layer it comes from — a documented
Tier 1 rule is not the same thing as sector custom, and neither is the same
thing as something that exists today.

| Layer | What it is | Authority |
|---|---|---|
| 1 | Documented rules of this pilot | Tier 1 (CONTRIBUTING.md, provenance-template.md) — absolute |
| 2 | Doctrine from the ODIN canon | Tier 2 / draft Constitution — guiding orientation, labelled as such |
| 3 | Standard UK school-sector practice | General knowledge — sensible default, must be verified with each school |
| 4 | What actually exists today | Phase 1 discovery, 2026-07-03 — currently: nothing formal |

---

## Layer 1 — Documented rules (Tier 1, absolute)

These rules are written in the repository's own canonical documents. They are
not suggestions and they have no expiry.

### Child contributor identity

- Children are identified by **school code + year group only** — e.g.
  `GUR-P-Y5`, `COW-H-Y8`. Never by name. In every file, in every commit,
  forever. (Source: CONTRIBUTING.md, "How to log an OVN contribution",
  Tier 1: "Contributor IDs for children use school code + year group only
  (no names)".)
- This applies to **every** artefact type: provenance records, field notes,
  question-map entries, OVN log rows, filenames, photograph captions, commit
  messages, issue text, pull-request descriptions — everything.
- Adult contributors use their name or GitHub handle (CONTRIBUTING.md,
  Tier 1) — but see the teacher rule below, which is stricter.

### Teacher identity

- Teachers present at sessions are recorded **anonymised or initials only**.
  (Source: provenance-template.md, "People" table, Tier 1: "Teacher present —
  anonymised or initials only".)

### The archive red lines — what may never be committed

The two rules above are the documented core. The following red lines are
**derived from them** (labelled: derivation from Tier 1, reasoned here, not
quoted from a repo document — but they follow necessarily, because each item
below would identify a child and therefore violate the Tier 1 identity rule):

Never commit, upload, share, or retain in any project store:

- [ ] A child's **name**, in any form, in any file
- [ ] A **face or photograph of a child** — including partial, background,
      or reflected appearances
- [ ] A **voice recording that could identify a child** (a child's voice is
      identifying to anyone who knows them)
- [ ] **Handwriting with a name visible** — children write their names on
      their work by habit; check every artefact
- [ ] Any detail that makes a child **re-identifiable**: a distinctive
      nickname written on work, a described disability or family circumstance,
      a uniform badge, "the girl whose dad runs the ferry"
- [ ] Anything about a **disclosure or welfare concern** (that belongs with
      the school's DSL, never in this repository)

**The small-island warning (state it whenever teaching anonymisation).** The
Isle of Wight is a small, tightly connected community. **Jigsaw
identification** — combining several individually harmless details until a
person is identifiable — is far easier here than on the mainland. "A Year 5
girl at [school] whose family keeps bees, quoted on 15 September" may be
identifiable to half the school gate. Anonymisation on the Island must
therefore be more aggressive than a generic checklist suggests: strip or
generalise contextual details in field notes, not just names. (Labelled:
reasoned application of the Tier 1 identity rule to the pilot's documented
setting — state schools on the Isle of Wight, README.md, Tier 1.)

### Artefact photography protocol

The pilot's documentation method depends on photographing children's work
(drawings, question lists, designs). The protocol:

1. **Photograph the work, never the child.** Flat on a table, top-down, no
   hands, no faces, no children in frame or background.
2. **Before committing, inspect every image at full size** for names,
   initials written by children, faces in reflections or edges, and any
   identifying detail.
3. **Crop or exclude names before committing.** If a name cannot be cleanly
   cropped out, the artefact is described in the provenance record instead of
   photographed, or re-photographed with the name masked physically (e.g.
   folded over or covered) at the time.
4. Name the file per the repository convention
   (`[SCHOOL-CODE]-[YYYY-MM-DD]-[PHASE]-[NNN]-[description].[ext]`,
   CONTRIBUTING.md, Tier 1) — the producer is credited as group + year, e.g.
   `group2`, never a name.
5. If in doubt about any image, **do not commit it**. A missing artefact is
   recoverable (describe it in the provenance record); a committed
   identification is public forever — this is a public GitHub repository
   under CC BY-SA 4.0, which grants everyone the right to copy and share.

(Steps 1 and 3 implement the Tier 1 identity rule; the workflow detail is
this skill's derivation, labelled as such. Session run-sheets live in
**iow-pilot-session-operations**.)

---

## Layer 2 — Doctrine from the ODIN canon (Tier 2 / draft Constitution — labelled)

This layer explains **why** the pilot's privacy posture is what it is. It is
guiding doctrine, not operational regulation. Sources are the ODIN
Constitution v0.1 — which is a **draft, unratified** (Dawn repo, Tier
1-adjacent) — and the practice-based PhD proposal "At Dawn We Build" (Tier 2,
aspirational, pre-dates the IoW pivot).

- **Sovereignty of the Self** (the draft's own heading reads "Sovereignity
  of the Self" [sic]). "ODIN affirms the right of all people to
  self-organise, self-identify, and self-represent. No central authority may
  claim ownership over an individual's data, identity, or contributions."
  Design orientation: "All infrastructure must support self-sovereign
  identity, agency, and informed consent." (ODIN Constitution v0.1 §2.1,
  draft, unratified.)
- **Relational privacy and consent doctrine** — unlinkability by default, a
  right to obscurity, and no assembling or inferring of a person's identity
  without their **ongoing** consent. The Phase 1 discovery brief (2026-07-03)
  records this as Constitution-draft doctrine in the form: "No agent, human
  or artificial, may assemble, share, or infer another agent's identity,
  history, or attestations without their explicit and ongoing consent."
  (Note: that sentence does not appear verbatim in the Constitution v0.1 file
  in the Dawn repo snapshot; treat it as doctrine recorded at Phase 1 and
  verify the current Constitution text before quoting it as a clause.)
- **Ethical review is community-led as well as institutional.** The PhD
  proposal commits to work "transparently documented, ethically stewarded",
  guided by "a distributed group of co-designers, peer reviewers, and
  community stakeholders", with trust mechanisms "evaluated through iterative
  feedback cycles, systems mapping, and ethical review" ("At Dawn We Build",
  Tier 2). For the pilot, read this as: the school, parents, and community
  are ethics reviewers, not just any future university board.
- **"Centre agency, not dependency."** The proposal commits to "remain
  vigilant to the risks of reproducing colonial dynamics through 'innovation'
  and ensure that digital tools are used in ways that centre agency, not
  dependency" ("At Dawn We Build", Tier 2). Applied here: children are
  contributors whose ideas are credited to their cohort, never data subjects
  to be mined; consent is a relationship, not a signature captured once.

**What this layer means in practice:** consent for a child's participation is
never treated as settled-forever. A cohort's work stays attributed to the
cohort ID precisely so that no individual child ever needs to be linked to it
— unlinkability by design is how the pilot honours both attribution and the
right to obscurity at once.

---

## Layer 3 — Standard UK school-sector practice (GENERAL KNOWLEDGE — not project documentation)

**Label discipline:** everything in this layer is standard practice in the
English state-school sector as general knowledge. **None of it is documented
in the pilot's Tier 1 files, and none of it has been agreed with any school
(no school has even been approached — Phase 1 discovery, 2026-07-03).** It is
presented as the sensible default posture. Every item must be **verified
with, and adapted to, each individual school** — schools' safeguarding
policies differ and the school's policy always governs on its own premises.

The default posture:

- **Enhanced DBS check.** An adult working regularly with children in a
  school ("regulated activity") requires an enhanced Disclosure and Barring
  Service (DBS) check with children's barred-list check. Facilitators should
  hold one before any session; an umbrella body can process it for
  individuals not employed by a school. *(Sector practice, general knowledge
  — verify the exact requirement with each school.)*
- **You work under the host school's safeguarding policy.** Visitors deliver
  activity under the school's policy, not their own. Read it before the first
  session; ask for it during setup. *(Sector practice — verify.)*
- **School staff are always present and hold the safeguarding duty.** A
  facilitator never supervises children unaccompanied. The teacher in the
  room carries the legal duty of care; the facilitator carries none of it
  away with them. **Never be alone with a child** — including corridors,
  before/after session, and one-to-one conversations out of staff sight.
  *(Sector practice — verify staffing arrangements per school.)*
- **Consent flows through the school's own parental-consent processes.** The
  pilot does not run its own consent collection past parents directly; the
  school gathers consent using its established channels and forms (adapted to
  cover the pilot's specific activities: public CC BY-SA 4.0 publication of
  anonymised artefacts is unusual and must be spelled out explicitly, not
  buried in a generic photo-consent form). A child whose consent is not in
  place still takes part in the learning — their work is simply not
  photographed or committed. *(Sector practice plus this pilot's own
  publication requirement — design with each school.)*
- **Disclosures and concerns go to the Designated Safeguarding Lead (DSL),
  immediately, and you never investigate yourself.** Every school has a DSL.
  If a child discloses harm, or you observe anything concerning: listen, do
  not promise confidentiality, do not question or probe, report to the DSL
  the same day (immediately if urgent), and follow the school's process.
  Nothing about it enters project files. Learn the DSL's name before the
  session starts — it should be on your pre-session checklist. *(Sector
  practice — the school's policy states the exact procedure; follow it.)*

---

## Layer 4 — What exists today (Phase 1 discovery, 2026-07-03)

**NOTHING formal exists.** Verbatim from the founder's Phase 1 answers
(2026-07-03, authoritative):

- **No DBS check is held** by anyone on the project.
- **No consent forms exist.**
- **No school safeguarding agreement exists** — and no school has been
  approached. Gurnard Primary (GUR-P) and Cowes High (COW-H) in
  CONTRIBUTING.md are **placeholder examples**, not partners.

Therefore: **everything in Layer 3 is TO BE BUILT before any session runs.**
No session, no visit, no classroom contact of any kind until the safeguarding
foundation is in place. This is **Gate 0** of the launch sequence — see
**iow-pilot-launch-campaign** for the executable buildout (DBS application,
school engagement, safeguarding agreement, consent design). This skill
defines what "in place" must mean; that skill sequences how to get there.

If you are a new facilitator reading this and someone has asked you to run a
session: first confirm, with the current steward, that Gate 0 has been passed
since 2026-07-03. If you cannot confirm it, the session does not happen.

---

## Pre-session verification checklist

This is the full checklist that **iow-pilot-session-operations** (before-
session runbook) and **iow-pilot-launch-campaign** (Gates 3–4) point to.
Work through it before **every** session, on or just before the day. **Every
box must tick. If any box cannot be ticked, the session does not run — no
exceptions, whatever the momentum or the school's enthusiasm.**

- [ ] **Enhanced DBS certificates physically in hand for BOTH ODIN adults**
      — the certificates themselves, with issue dates. An application in
      progress is not clearance. *(Sector practice, general knowledge — the
      school's own requirements govern and may be stricter.)*
- [ ] **Written school safeguarding agreement in place** with this school,
      including the anonymisation contract (school code + year group only;
      no names, no faces, no identifying detail — CONTRIBUTING.md, Tier 1).
- [ ] **Consent coverage confirmed** — the school's count of consented and
      non-consented children is in hand, and the **documentarian knows which
      children or groups lack consent** so their outputs are marked
      non-archivable at capture time. That knowledge stays with the school
      and in the adults' heads on the day — it is never written into project
      files.
- [ ] **The school's safeguarding policy has been read** by both ODIN adults
      — you work under it, not your own *(sector practice — verify with the
      school)*.
- [ ] **The DSL's name is known** to both adults — the Designated
      Safeguarding Lead is where every disclosure or concern goes,
      immediately.

**If a parent, teacher, or school asks what we keep:** the answer is short
and honest. We keep children's *work* (questions, drawings, designs), never
children: no names, no faces, no voices, no identifying details, ever. Work
is credited to school code + year group only (e.g. `GUR-P-Y5`) and published
openly under CC BY-SA 4.0. A child without consent takes part fully in the
session; nothing they produce enters the archive. Anything identifying is
never kept, and if one ever slipped through it would be treated as a live
incident (next section). (Tier 1: CONTRIBUTING.md, LICENSE.)

---

## Incident procedure — an identifying artefact has been pushed to the public repo

This is the procedure **iow-pilot-session-operations** routes to when
identifying content (a child's name, face, voice, or other identifying
detail) has already been committed or pushed. *(Labelled: derived practice
under the Tier 1 anonymity rule plus general git knowledge — not quoted from
a repo document. It follows necessarily: a published identification violates
the absolute Tier 1 identity rule and must be unpublished as fast and as
completely as possible.)*

**Treat this as a live safeguarding incident. Stop other work. Speed
matters** — the repo is public and every hour widens the window for forks,
clones, and caches to copy the content.

1. **Remove the file AND purge it from git history — the same day, as fast
   as humanly possible.** A follow-up commit that deletes the file is **not
   enough**: the identifying content remains in the repository's history and
   stays publicly retrievable. The history must be rewritten (e.g. with
   `git filter-repo`) and force-pushed by someone with write access to
   github.com/ODINcommons/IoW-pilot. If you lack access, contact the current
   steward immediately — this is the one situation in which you interrupt
   anyone at any hour. Consider contacting GitHub support to purge cached
   views of the removed content.
2. **Be honest about residual risk.** The repo is public under CC BY-SA 4.0:
   forks, clones, and caches made before the purge may persist and cannot be
   recalled. Never tell the school, a parent, or anyone else that the
   content is "fully gone" — say what was removed, when, and what residual
   risk remains.
3. **Notify the school's Designated Safeguarding Lead AND the current
   steward the same day.** The school decides, under its own policy, what
   the affected family is told. Do not decide that for them and do not
   contact parents directly.
4. **Record the incident honestly in the session's provenance record —
   WITHOUT reproducing the identifying detail.** State that an identifying
   artefact was pushed, when it was discovered, when it was purged, who was
   notified, and the residual-risk position. Never restate the name, image,
   or detail itself, in the record or in the commit message.
5. **Review how it happened before the next session.** Find the step that
   failed (usually the full-size image inspection in the artefact
   photography protocol, or capture-time marking of non-consented outputs),
   fix it, and note the process change in the provenance record.

---

## The one place the one rule bends

The pilot's one rule is "Everything gets attributed before it gets built"
(CONTRIBUTING.md, Tier 1). Safeguarding is the single thing that outranks it.

**If attribution and anonymity ever conflict, anonymity wins.** The
resolution is built into the Tier 1 design: children's work is attributed to
the **cohort ID** (`GUR-P-Y5`), never to the individual child. The cohort is
credited fully and forever; the child remains unlinkable. So the rule bends
without breaking — attribution survives, at cohort granularity. If a
situation arises where even cohort-level attribution would make a child
re-identifiable (a cohort of one, a uniquely attributable idea in a
small-island context), drop or coarsen the attribution and record why in the
provenance record. No skill, contributor, or future decision may reverse this
priority.

---

## When NOT to use this skill

- **Session mechanics** — run-sheets, timings, before/during/after
  checklists, room setup: use **iow-pilot-session-operations** (it must still
  comply with everything here).
- **Provenance and attribution mechanics** — the one rule, provenance-record
  timing, question-map discipline, OVN logging, licensing: use
  **iow-pilot-provenance-and-attribution**.
- This skill is the constraint layer. Everything else operates inside it.

---

## Provenance and maintenance

Sources used, by tier:

- **Tier 1:** `CONTRIBUTING.md` (child contributor IDs, one rule, filename
  convention, licence), `provenance-template.md` (teacher anonymisation,
  People table), `README.md` (pilot setting), all at
  github.com/ODINcommons/IoW-pilot.
- **Tier 1-adjacent:** ODIN Constitution v0.1 (Dawn repo) — draft,
  unratified; §2.1 quoted verbatim above.
- **Tier 2:** "At Dawn We Build" PhD proposal — aspirational, Athens-era;
  quoted phrases verbatim above.
- **Phase 1 discovery, 2026-07-03:** founder's answers — nothing formal
  exists; placeholder school codes.
- **General knowledge, labelled:** all of Layer 3 (UK school-sector
  practice). Nothing in Layer 3 is project documentation.

**This skill drifts faster than any other in the library.** Layer 4 was true
on 2026-07-03 and will (should) become false. Before EVERY school engagement:

1. **Work through the Pre-session verification checklist** (in the body,
   above) with the current steward — DBS certificates in hand, consent
   coverage (forms must explicitly cover public CC BY-SA 4.0 publication of
   anonymised artefacts), written school agreement, the school's policy,
   the DSL's name.
2. Check github.com/ODINcommons/IoW-pilot for updates to CONTRIBUTING.md and
   provenance-template.md — local snapshots may be stale. If the repo has
   grown a dedicated safeguarding document since 2026-07-03, that document
   supersedes the derivations here (the Tier 1 identity rules themselves do
   not expire).
3. Layer 3 is unverified general knowledge until a school confirms it —
   each school's own safeguarding policy replaces the generic posture the
   moment it is in hand.

The Tier 1 red lines — no names, no faces, cohort ID only, anonymity over
attribution — do not drift and are not subject to re-verification. They are
permanent.
