# Roadmap

Phased delivery, tied to the pilot's own phase structure (see the main
`README.md`) rather than a generic sprint plan — this tool exists to serve
the pilot's sessions, not the other way round.

## Milestone 0 — Planning and data-sourcing (this commit)

- Hazard inventory (`hazards.md`)
- Open GIS/geospatial data-source catalogue (`data-sources.md`)
- Technical architecture plan (`architecture.md`)

Nothing built yet. This milestone exists so that Milestone 1 starts from a
reasoned plan, not from whichever dataset is easiest to find first.

## Milestone 1 — First data package

- Stand up the Python ingest pipeline described in `architecture.md`.
- Pull and clip to the Isle of Wight bounding box: OS Terrain 50, EA LIDAR
  Composite DTM, EA Recorded Flood Outlines, RoFSW extents, NCERM, BGS
  GeoSure landslides, MAGIC/Natural England designations, ONS boundaries,
  bathing water quality sites.
- Produce the provenance manifest for every extract.
- **Exit condition**: every layer in `data-sources.md` groups A–D, G, H has
  a clipped extract and a manifest entry.

## Milestone 2 — v1 static viewer

- MapLibre + PMTiles front end, deployed to a static host.
- Base layers with legend and per-layer attribution rendering correctly
  (see `architecture.md`, "Attribution rendering").
- No live data yet beyond what the Environment Agency's own APIs already
  provide (flood monitoring, bathing water quality can be fetched
  client-side rather than baked into tiles).
- **Exit condition**: a working public URL, forkable, that a facilitator
  can open in a school and use to show real Island hazard data.

## Milestone 3 — Live and community layers

- Wire in Southern Water/EA Event Duration Monitoring data as a refreshed
  layer.
- Add the Pooseidon buoy telemetry layer once buoys are physically
  deployed (see main `README.md`, "First project idea: Pooseidon") — this
  is the point where the tool starts carrying the pilot's own
  citizen-generated data, not just government data.
- Add the moderated community-reporting layer (`architecture.md`).

## Milestone 4 — Feed into sessions

- Use the v1/v2 map as shared evidence in Phase 2 (Pivot) sessions, where
  groups return to the Question Map and ask what could be done about the
  water-related problems they found.
- Use it in Phase 3 (Impactathons) as a grounding reference for teams
  designing real responses — so a design like Pooseidon's alert system can
  be checked against where the actual highest-risk overflows and
  bathing-water sites are, rather than designed in the abstract.
- Log every question this raises in `question-map.md` and every
  contribution in `ovn-contributions.md`, as normal.

## Governance and attribution across all milestones

- This tool's own outputs stay CC BY-SA 4.0, same as the rest of the
  pilot. Never add a tighter licence to any layer, script, or derivative —
  see `CONTRIBUTING.md`.
- Third-party datasets keep their own licence, attributed per layer — see
  `data-sources.md` and `architecture.md`.
- Every milestone's work gets an OVN log entry per the usual process
  (`ovn-contributions.md`).
