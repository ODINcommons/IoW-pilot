# Resilience GIS

### An open-source hazard and resilience mapping tool for the Isle of Wight

---

## What this is

A companion component of the ODIN Isle of Wight pilot: an open-source, forkable
GIS tool that brings together the Island's flood, coastal, ground-instability,
water-quality, and climate hazard data into one place, so that schools,
residents, and the pilot's own Impactathon teams can see the real physical
risks the Island faces — and design real responses to them.

It exists to answer, with evidence, the questions the pilot's opening theme
already asks: *what are the water-related problems we face here, and what
could we do about them?* Coastal erosion, landslip, storm surge, surface
water flooding, and sewage discharge are not abstract categories on the
Isle of Wight — they are named places, measured events, and open datasets.
This tool puts them on a map.

It is not a replacement for statutory planning tools (the Shoreline
Management Plan, the Environment Agency's Flood Map for Planning) or for the
Hampshire & Isle of Wight Local Resilience Forum's emergency-response
function. It is a public, evidence-first layer that sits alongside them:
built from the same open data, licensed so it can never be enclosed, and
designed to be understood and extended by the people who live with the risk.

---

## Structure

```
resilience-gis/
├── README.md          ← you are here
├── hazards.md          ← the Island's hazard inventory: what, where, why
├── data-sources.md      ← the open GIS/geospatial datasets this tool draws on
├── architecture.md       ← the technical plan: stack, pipeline, hosting
└── roadmap.md          ← phased delivery plan, tied to the pilot's own phases
```

No code has been written yet. This first commit is the planning and data-sourcing
phase: understanding the hazards, cataloguing the open datasets that describe
them, and deciding an architecture before building anything — the same
discipline the rest of this pilot applies to attribution: understand and
record first, build second.

---

## Scope

**In scope:** coastal erosion and cliff retreat, ground instability and
landslip, fluvial and surface water flooding, coastal/tidal flooding and
storm surge, sewage and wastewater pollution, drought and water-resource
stress, heatwave risk, wildfire risk on heath and downland, and the Island's
compound "single point of failure" risks (ferry and undersea-main
dependency).

**Out of scope, deliberately:** live emergency dispatch, individual property
risk certification, and anything that would require restricting the data or
the tool behind a licence tighter than the rest of this repository. If a
future capability needs that, it belongs in a different, separately
licensed project — not here.

---

## Licence and attribution

This tool's own code, documentation, and any community-contributed layers
are licensed **CC BY-SA 4.0**, same as the rest of the IoW pilot — see the
repository [`LICENSE`](../LICENSE).

The underlying government and public-body datasets it draws on (Environment
Agency, Ordnance Survey, British Geological Survey, ONS, Natural England,
Met Office) are separately licensed, almost all under the **Open Government
Licence (OGL)** or a compatible open licence. `data-sources.md` records the
licence for every dataset individually, and the architecture in
`architecture.md` keeps per-layer attribution visible on the map itself —
this project must never present Crown-copyright/OGL data as if it were
CC BY-SA, or vice versa. See `data-sources.md` for the detail.

---

## Relationship to the rest of the pilot

- Shares the Island's water theme with **Pooseidon** (see the main
  `README.md`); once Pooseidon buoys are deployed, their live telemetry is
  intended to become a layer on this map (see `roadmap.md`, Milestone 3).
- Intended as shared evidence for **Phase 2 (Pivot)** and **Phase 3
  (Impactathon)** sessions, so teams designing responses to real local
  problems can ground their designs in real hazard data rather than
  starting from nothing.
- Follows the same OVN contribution logging as every other artefact in this
  repository — see `ovn-contributions.md`.

---

**Status**: Planning and data-sourcing phase.
**Licence**: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) (this project's own work); see `data-sources.md` for third-party dataset licences.
**Part of**: [ODIN Isle of Wight Pilot](../README.md)
