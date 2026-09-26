# GIS / geospatial data sources

Every dataset below is public and (unless noted) free to use with
attribution. Licence terms are recorded per dataset because they are not
uniform — most government data is **Open Government Licence (OGL)**, but a
few community-aggregated sources are not government data at all and carry
their own terms. Do not blend attribution strings across licences; the
architecture in `architecture.md` renders each layer's own attribution.

Each row's "Access" column notes the most durable retrieval method — a
downloadable extract, a WMS/WFS map service, or a REST/JSON API — since
government portals do periodically reorganise their URLs. Where a dataset
is versioned annually or per-survey, that's noted so the ingest pipeline
(see `architecture.md`) knows to check for a newer edition rather than
hard-coding one.

---

## A. Terrain and base mapping

| Dataset | Publisher | Access | Licence | Notes |
|---|---|---|---|---|
| OS Terrain 50 (contours, spot heights) | Ordnance Survey | [Download — OS Data Hub](https://osdatahub.os.uk/downloads/open) | OGL / OS OpenData | GB-wide open elevation data; coarse but zero-friction base layer. |
| OS Open Rivers | Ordnance Survey | [Download — OS Data Hub](https://osdatahub.os.uk/downloads/open/OpenRivers) | OGL / OS OpenData | Connected river/stream network — needed to relate flood layers to named watercourses (Medina, Eastern/Western Yar). |
| OS Open Greenspace | Ordnance Survey | [Download — OS Data Hub](https://osdatahub.os.uk/downloads/open/OpenGreenspace) | OGL / OS OpenData | Public greenspace polygons — useful for evacuation/shelter-space context. |
| LIDAR Composite DTM, 1 m (and 25 cm where flown) | Environment Agency | [environment.data.gov.uk dataset](https://environment.data.gov.uk/dataset/ce8fe7e7-bed0-4889-8825-19b042e128d2) | OGL | High-resolution bare-earth terrain — the base for any real flood-depth or landslide-runout modelling on the Island. No access restriction. |

## B. Flood risk (fluvial, tidal, surface water)

| Dataset | Publisher | Access | Licence | Notes |
|---|---|---|---|---|
| Real-time flood monitoring (warnings, alerts, gauge levels) | Environment Agency | [flood-monitoring API](https://environment.data.gov.uk/flood-monitoring/doc/reference) | OGL, no registration | 15-minute refresh; the only genuinely "live" layer in this list before Pooseidon deploys. |
| Recorded Flood Outlines (historic events) | Environment Agency | [Defra Data Services Platform](https://environment.data.gov.uk/) | OGL | Ground-truths modelled risk against what has actually flooded. |
| Flood Map for Planning — Rivers and Sea flood risk extents (Zones 2/3) | Environment Agency | [Download by area](https://environment.data.gov.uk/) | OGL | Statutory planning layer; clip to Island bounding box. |
| Risk of Flooding from Surface Water (RoFSW) — extents, depth, hazard | Environment Agency | [Dataset](https://environment.data.gov.uk/dataset/b5aaa28d-6eb9-460e-8d6f-43caa71fbe0e) · [Download service](https://environment.data.gov.uk/DefraDataDownload/?Mode=rofsw) | OGL | Models rainfall overwhelming drainage independent of rivers — the dominant risk in Newport and other built-up areas. |
| RoFSW — climate change scenarios | Environment Agency | [Dataset](https://environment.data.gov.uk/dataset/e5b38de2-99b3-44ee-b10c-b244926878ef) | OGL | Forward-looking version of the above; pairs with UKCP18 (§F). |

## C. Coastal erosion and shoreline management

| Dataset | Publisher | Access | Licence | Notes |
|---|---|---|---|---|
| National Coastal Erosion Risk Mapping (NCERM), national dataset | Environment Agency | [Dataset](https://environment.data.gov.uk/dataset/9fede91f-5acd-4fd2-9bd8-98153fa3c2ff) | OGL | Erosion-risk extents to 2055 and 2105, under "with defences" and "no active intervention" scenarios, using UKCP18 sea-level scenarios. Released Jan 2025 — check for newer editions. |
| Isle of Wight Shoreline Management Plan 2 (SMP2), incl. Appendix C (shoreline dynamics/climate change) and Appendix F (future shoreline scenarios) | Isle of Wight Council / Environment Agency | [Plans and strategies](https://www.iow.gov.uk/environment-and-planning/coastal-management/shoreline-management-plan-strategies-and-schemes/plans-and-strategies/) · [SMP documents mirror](https://environment.data.gov.uk/shoreline-planning/documents/SMP14/) | Public document (Crown/Council copyright); geospatial policy units digitisable from the maps | The Island's own 100-year coastal policy document — every erosion/flood layer above should be read against this. Adopted 2011; assesses coastal flood, erosion, and landslide risk together. |
| Regional Coastal Monitoring Programme surveys (topographic, bathymetric, aerial) | Channel Coastal Observatory (National Network of Regional Coastal Monitoring Programmes) | [coastalmonitoring.org](https://coastalmonitoring.org) | Free, attribution required | Includes a 2011 100%-coverage nearshore swath bathymetry survey of the Island's north and south coasts. Best source for measured (not modelled) shoreline change. |
| SCOPAC sediment transport studies (NW/NE/SW+SE Isle of Wight) | SCOPAC (Standing Conference on Problems Associated with the Coastline) | [scopac.org.uk](https://scopac.org.uk/sts/) | Public reports | Literature/process context behind the erosion numbers; not a GIS layer itself but needed to interpret one. |

## D. Ground instability and landslip

| Dataset | Publisher | Access | Licence | Notes |
|---|---|---|---|---|
| BGS GeoSure — landslides (slope instability) | British Geological Survey | [Dataset page](https://www.bgs.ac.uk/datasets/bgs-geosure-landslides/) | OGL, free | GB-wide susceptibility layer; the Island's Undercliff shows as the most severe class nationally. |
| BGS National Landslide Database | British Geological Survey | [Dataset page](https://www.bgs.ac.uk/datasets/national-landslide-database/) | OGL; some records need direct request to BGS | Point/event-level landslide records; over 17,000 GB-wide, continually updated. |
| Isle of Wight Council geotechnical case studies (Ventnor Undercliff, Bonchurch, etc.) | Isle of Wight Council | [Ventnor Undercliff case study (PDF)](https://www.iow.gov.uk/media/3515/Geotechnical-case-study-1-Ventnor-Undercliff-Landslide-Complex/pdf/Geotechnical_case_study_1_Ventnor_Undercliff_Landslide_Complex.pdf) | Public document | Island-specific ground-truth on movement rates (5–10 mm/yr on the main Undercliff shear surface) and affected zones. |

## E. Water quality and sewage discharge

*(Directly shared with Pooseidon — see `README.md`.)*

| Dataset | Publisher | Access | Licence | Notes |
|---|---|---|---|---|
| Bathing Water Quality (14 designated Island sites: Bembridge, Colwell Bay, Compton, Cowes, Gurnard, Ryde, Sandown, Seagrove, Shanklin, St Helens, Totland Bay, Ventnor, Whitecliff Bay, Yaverland) | Environment Agency | [API](https://environment.data.gov.uk/bwq/) · [API reference](https://environment.data.gov.uk/bwq/doc/api-reference-v0.6.html) | OGL, linked open data | Seasonal (May–Sept) sampling plus daily pollution-risk forecasts at some sites. |
| Event Duration Monitoring (EDM) — storm overflow spill data | Environment Agency (published), Southern Water (operator) | [Flow and Spill Reporting](https://www.southernwater.co.uk/about-us/environmental-performance/healthy-rivers-and-seas/flow-and-spill-reporting/) | OGL (EA published data) | Records start/stop of each overflow discharge, not volume. ~103 Island overflows. |
| Isle of Wight River Basin Catchment / Clean Rivers and Seas Plan | Southern Water | [Catchment page](https://www.southernwater.co.uk/about-us/our-plans/drainage-and-wastewater-management-plans/isle-of-wight-catchment/) · [Clean Rivers and Seas Plan](https://www.southernwater.co.uk/about-us/our-plans/clean-rivers-and-seas-plan/) | Public document | Company's own investment/priority plan per catchment — useful for identifying which overflows are flagged highest-risk. |
| Community EDM aggregators (secondary — verify against primary EA/company data before relying on them) | e.g. WaterWatch, Rivers and Seas Watch, Island Rivers | [water-watch.co.uk](https://water-watch.co.uk/company/southern) · [islandrivers.org.uk](https://islandrivers.org.uk/sewage-discharges-to-rivers-and-the-sea/) | Varies — check each site | Useful for a friendlier public-facing view of the same EDM data; not a substitute for citing the primary Environment Agency/Southern Water source. |

## F. Climate projections

| Dataset | Publisher | Access | Licence | Notes |
|---|---|---|---|---|
| UKCP18 Local projections (2.2 km, RCP8.5, 1980–2080) | Met Office | [CEDA Archive](https://catalogue.ceda.ac.uk/uuid/e7b0165f3b57409998ca2632dad7a1a3/) · [Met Office climate data portal](https://climate-themetoffice.hub.arcgis.com/) · [Guidance](https://www.metoffice.gov.uk/research/approach/collaboration/ukcp/guidance-reports) | OGL | The projection basis behind NCERM's climate scenarios (§C) and RoFSW's climate-change layer (§B). Requires a free CEDA account for the archive route. |

## G. Natural environment and designations

| Dataset | Publisher | Access | Licence | Notes |
|---|---|---|---|---|
| MAGIC map (400+ layers: SSSI, SPA, Ramsar, AONB/National Landscape boundaries, flood risk overlays) | Defra / multi-agency | [magic.defra.gov.uk](https://magic.defra.gov.uk/MagicMap.aspx) | OGL | The single broadest viewer; useful for cross-checking hazard layers against protected-area boundaries (much of the Island's coast is AONB/National Landscape, which constrains defence options — see SMP2). |
| Sites of Special Scientific Interest (England) | Natural England | [Open Data Geoportal](https://naturalengland-defra.opendata.arcgis.com/datasets/Defra::sites-of-special-scientific-interest-england/about) | OGL | Direct download/API rather than the MAGIC viewer, for pipeline use. |

## H. Administrative and socio-demographic context

| Dataset | Publisher | Access | Licence | Notes |
|---|---|---|---|---|
| Digital boundaries (LSOA, ward, parish, Isle of Wight unitary authority boundary) | ONS | [Open Geography Portal](https://geoportal.statistics.gov.uk/) | OGL | Needed to join any hazard layer to population/deprivation context, and to clip national datasets to "Isle of Wight" cleanly. |
| English Indices of Deprivation (IMD), LSOA level | MHCLG / ONS | [gov.uk statistics release](https://www.gov.uk/government/statistics/english-indices-of-deprivation-2025) · lookups via [Open Geography Portal](https://geoportal.statistics.gov.uk/) | OGL | For vulnerability-weighted risk views — a flood or heat hazard matters more where people have fewer resources to recover. Use with care and say so on the map: deprivation data describes structural disadvantage, not individual capacity. |
| Census 2021 population counts | ONS | [ONS website](https://www.ons.gov.uk/) | OGL | Denominator for any exposure estimate (e.g. "X residents within the surface-water flood extent"). |

## I. Emergency-planning and community-risk context

| Dataset | Publisher | Access | Licence | Notes |
|---|---|---|---|---|
| Hampshire & Isle of Wight Community Risk Register | Hampshire & Isle of Wight Local Resilience Forum | [hiowprepared.org.uk](https://hiowprepared.org.uk/home/local-risks/) | Public document | The statutory risk-assessment framing (natural events, disease, major accidents, malicious attacks) this tool's hazard layers should be legible against. Updated annually. |
| Isle of Wight Council Community Risk Register page | Isle of Wight Council | [iow.gov.uk](https://www.iow.gov.uk/keep-the-island-safe/emergency-management/community-risk-register) | Public document | Island-specific entry point into the same LRF framework. |

## J. Community and crowd-sourced layers

| Dataset | Publisher | Access | Licence | Notes |
|---|---|---|---|---|
| OpenStreetMap (roads, critical infrastructure points, ferry terminals, harbours) | OSM contributors | Overpass API, or a Geofabrik regional extract | ODbL (share-alike, compatible in spirit with CC BY-SA but check compatibility case-by-case before merging into a CC BY-SA layer) | Best source for "what's actually there" — evacuation routes, shelter-candidate buildings — where no government layer exists. |
| Pooseidon buoy telemetry (once deployed) | This pilot | n/a yet — see `roadmap.md` Milestone 3 | CC BY-SA 4.0 (this project's own data) | The pilot's own citizen-deployed sensor network; will become this map's first genuinely live, locally-owned layer. |

---

## Access notes for the ingest pipeline

- Prefer a durable **dataset landing page** URL (as above) over a raw file
  link — direct file links on `environment.data.gov.uk` and
  `data.gov.uk` are periodically re-issued per survey year.
- Where a dataset has an interactive **download-by-area** tool (Flood Map
  for Planning, RoFSW), use it to fetch only the Isle of Wight bounding box
  rather than a national extract.
- Record, for every file the pipeline pulls: source URL, licence,
  retrieval date, and publisher's version/edition label. See
  `architecture.md` for the manifest format — this mirrors the same
  provenance discipline the rest of the repository applies to session
  artefacts.
