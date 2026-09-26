# Architecture plan

A technical plan for turning `data-sources.md` into a working, open-source
map — written before any code, so the stack is chosen for the project's
actual constraints rather than defaulting to whatever is fashionable.

## Constraints that shape every choice below

- **Zero-to-low cost.** This is a volunteer/community/school project, not a
  funded product. Recurring hosting or database costs are a liability the
  project has no budget line for.
- **Forkable.** Per the repository's own licence terms, anyone must be able
  to fork this and run it themselves. A stack that depends on a paid
  managed service (a hosted database, a paid tiling API) fails that test.
- **Low-bandwidth, school-network friendly.** Sessions run in state schools
  on shared connections. The map must work acceptably on a slow link and
  degrade gracefully offline.
- **Attribution-correct.** Per `data-sources.md`, layers carry different
  licences (OGL vs CC BY-SA vs ODbL). The architecture must keep these
  separable and render each layer's own attribution — never a single
  blanket footer that misattributes one licence's data as another's.

## Recommended stack (v1)

**Front end: [MapLibre GL JS](https://maplibre.org/)** rendering **vector
and raster tiles**, served as static files. MapLibre is a genuine
open-source fork of the last open-licensed Mapbox GL version — no API key,
no usage limits, no vendor dependency.

**Tile format: [PMTiles](https://github.com/protomaps/PMTiles)** instead of
running a tile server. PMTiles packages an entire vector or raster tileset
into a single file that can be range-requested directly from any static
file host (GitHub Pages, Netlify, S3, or the school's own web space) — no
server process, no database, no recurring compute cost. This is the single
highest-leverage decision in this plan: it means the whole "hosting" line
of the budget is zero, indefinitely, for as long as the project needs it.

**Data pipeline: Python (GDAL/OGR via `geopandas` and `rasterio`)**,
run on a schedule (or manually before each release) to:
1. Pull each source in `data-sources.md` from its landing page/API.
2. Clip to the Isle of Wight bounding box (using the ONS boundary, §H).
3. Reproject to a single consistent CRS (EPSG:4326 for web serving; keep
   OSGB36/EPSG:27700 originals where a dataset was published in it, since
   several of the government sources — LIDAR, OS — are natively OSGB36).
4. Simplify/tile with `tippecanoe` (vector) or `rio-cogeo`/`gdal2tiles`
   (raster), then package as PMTiles.
5. Write a **manifest** entry per output file recording: source dataset,
   publisher, licence, source URL, retrieval date, publisher's edition/
   version label. This is the same discipline the rest of the pilot applies
   to session provenance — a layer without a manifest entry does not ship.

Only the **clipped, Island-scale extracts** are committed or published —
not mirrors of the national raw datasets, both to respect each publisher's
own distribution terms and to keep the repository small.

**Database: none for v1.** Every layer in `data-sources.md` is either
static (survey-based) or already served live by its publisher's own API
(flood monitoring, bathing water quality) — there is no need to stand up
PostGIS to serve data that already has a perfectly good open API. Add
PostGIS (with [Martin](https://maplibre.org/martin/) as the tile server) at
the point, and only at the point, this tool needs to store something no
one else does — chiefly the community-reporting layer below.

## Community reporting layer (later milestone, see `roadmap.md`)

A moderated layer for ground-truth citizens can add themselves — "this
road floods in every high tide", "this cliff path has visibly moved" —
distinct from, and clearly labelled apart from, the official layers above.
Simplest viable version: a form that opens a GitHub issue with structured
fields (location, hazard type, description, optional photo), reviewed and
merged into a small GeoJSON file by a facilitator, same review discipline
as the rest of the repository's provenance process. Only move to a live
database/backend if that manual review step becomes the actual bottleneck.

## Attribution rendering

Each layer's config (a `layers.json` or equivalent, listing style, legend
entry, and licence) carries its own attribution string, shown in the
map's attribution control and expandable per-layer — e.g. "Contains
Environment Agency information © Environment Agency and database right"
for OGL layers, vs "CC BY-SA 4.0, ODIN Isle of Wight Pilot" for
Pooseidon/community layers. Do not collapse these into one credit line.

## Hosting

A static site (GitHub Pages from this repository, or an equivalent free
static host) is sufficient for the whole stack above — front end, tiles,
and manifest are all static files. This keeps the tool inside the same
zero-cost, fully-forkable model as the rest of the pilot.

## What this deliberately defers

- A live alerting/notification system (SMS, push) — a genuinely useful
  future capability, but a materially bigger commitment (a backend, a
  subscriber list, a duty of care around false alarms) that should be
  scoped as its own decision once the base map exists and there is a
  community to ask what they'd actually want alerted.
- Property-level risk lookup — deliberately out of scope; see `README.md`.
- Any dataset not yet catalogued in `data-sources.md` — add it there first.
