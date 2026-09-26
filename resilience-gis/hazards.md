# Isle of Wight hazard inventory

A working list of the physical hazards this tool needs to represent, why each
one matters specifically on the Isle of Wight (not generically for "an
island"), and the primary evidence base for it. Each entry links forward to
the relevant rows in `data-sources.md`.

This is a living document, in the same spirit as `question-map.md`: add to
it as evidence emerges; do not delete a hazard because it hasn't happened
recently.

---

## 1. Coastal erosion and cliff retreat

The Island has 168 km of coastline and a genuinely mixed geology: soft,
fast-eroding cliffs (Bembridge, Shanklin, Luccombe, Colwell) alongside the
hard chalk of the Needles and Culver Down. Erosion rates and management
policy differ frontage by frontage — this is exactly what the Shoreline
Management Plan (SMP2) and the National Coastal Erosion Risk Map (NCERM)
model. See `data-sources.md` §C.

## 2. Ground instability and landslip

The Ventnor Undercliff is the largest urban landslide complex in the UK,
built on ground that has moved continuously since a post-glacial sea-level
rise roughly 10,000 years ago; Blackgang and Luccombe carry similar risk.
This is a genuinely distinctive Island hazard — the British Geological
Survey ran a dedicated multidisciplinary Isle of Wight landslide survey
(2007–2010) because of it. See `data-sources.md` §D.

## 3. Fluvial and surface water flooding

The Medina and the Eastern and Western Yar are the Island's main
catchments; Newport town centre sits at their confluence and floods.
Surface water flooding (rainfall overwhelming drainage, independent of any
river) is modelled separately by the Environment Agency and is often the
more locally damaging risk in the built-up northern towns. See
`data-sources.md` §B.

## 4. Coastal and tidal flooding, storm surge

Low-lying settlements — Ryde, Bembridge Harbour, Yarmouth, Newtown Creek —
are exposed to surge combined with high spring tides, the same mechanism
behind the East Coast's historic surge events. Climate change is projected
to raise both the frequency and the height of surge events this century.
See `data-sources.md` §B, §F.

## 5. Sewage and wastewater pollution

Southern Water operates roughly 103 storm overflows on the Island, spilling
on the order of 2,400 times a year; several catchments are flagged as
likely to reach "very significant" spill risk without further action. This
is the hazard **Pooseidon already exists to address** — this tool's role is
to put the same Event Duration Monitoring (EDM) data, and Environment
Agency bathing water quality data, on the map as a persistent evidence
layer rather than a one-off design prompt. See `data-sources.md` §E.

## 6. Drought and water-resource stress

The Island's public water supply depends on a limited local resource plus
an undersea main from the mainland — a genuine single point of failure.
Drought stress reduces river flows (worsening §5's dilution of discharges)
and tightens abstraction. See `data-sources.md` §F, §I.

## 7. Heatwave and public-health risk

An older-than-average population and a housing stock not built for heat
raise the health burden of heatwaves; UK Health Security Agency heat-health
alerting applies Island-wide. Lower priority for a first map release than
§1–§5, but worth a placeholder layer once UKHSA/ONS data is integrated. See
`data-sources.md` §H.

## 8. Wildfire

Heath and downland (Headon Warren, Brading Down, Parkhurst Forest margins)
carry dry-season fire risk, sharpened by hotter, drier summers under UKCP18
projections. A secondary hazard for v1; revisit once vegetation/fuel-load
data sources are identified.

## 9. Marine and lifeline infrastructure risk

The Island's ferry links and the Solent shipping lanes are the hazard
multiplier underneath every other risk: severe weather that closes the
ferries at the same time as a surge or a power outage turns a local event
into an isolation event. This is a compound-risk framing, not a single
dataset — see §10.

## 10. Compound and cascading risk

The hazard that matters most for genuine resilience planning is rarely a
single event: a spring tide plus a storm surge plus heavy rainfall plus a
ferry suspension plus a power outage is a materially different problem than
any one of those alone. Once the individual layers above exist, this tool
should support overlaying them — that is the actual point of putting them
on one map rather than five separate agency websites.

---

**Sources for the framing above**: Isle of Wight Council geotechnical case
studies and Shoreline Management Plan (see `data-sources.md` §C, §D);
Southern Water's Isle of Wight River Basin Catchment plan and Clean Rivers
and Seas Plan (§E); Hampshire & Isle of Wight Local Resilience Forum
Community Risk Register (§I). Treat this section as a summary for
orientation, not a citation of record — always check the primary source in
`data-sources.md` before using a figure in a design or a publication.
