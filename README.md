# MapEx2

Separate vanilla JavaScript MapEx copy. Serve this directory over HTTP, for example `python -m http.server 8000`, then open `http://localhost:8000/`. The original MapEx repository is unchanged.

The map includes current regional snapshots downloaded on 2026-11-05 plus older features retained where they could not be matched. Layer status in the map reports how many older features are included. Those features can be stale. Where parcel IDs are missing or ambiguous, retaining older boundaries may create overlaps. The map is informational and does not establish current legal boundaries.

`layer-refresh-report.json` documents the merge counts and matching fields; `feature-comparison.json` contains the comparison. Object IDs on the RDKB property-search service changed between snapshots, so properties are matched using parcel GUID, address ID and folio. Imagery and BC provincial parcel layers use live services; RDCK imagery is optional. Address coordinates use saved regional data, with BC Geocoder offered only as an explicitly approximate fallback.

Contains information licensed under the Open Government Licence – Regional District of Kootenay Boundary; see [RDKB licence](RDKB-open-data-license.pdf). RDCK data is attributed to the Regional District of Central Kootenay. Public redistribution terms for every cached layer have not been independently verified; this repository is private.
