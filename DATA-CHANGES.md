# MapEx2 data comparison

Compared the saved March 31, 2026 snapshots with downloads completed November 5, 2026. Count changes do not prove individual additions or deletions. Older unmatched map features are preserved and can be stale or overlap.

| Dataset | March count | November count | Net change |
|---|---:|---:|---:|
| RDCK Address Points | 35,181 | 31,615 | -3,566 |
| RDCK Cadastre - Property Lines | 54,667 | 50,811 | -3,856 |
| RDKB Address Points | 12,855 | 12,881 | +26 |
| RDKB Address Table | 32,494 | 32,697 | +203 |
| RDKB Admin Boundaries | 13 | 13 | +0 |
| RDKB Assessment Table | 31,585 | 31,728 | +143 |
| RDKB Beyond RDKB | 6 | 6 | +0 |
| RDKB Community Names | 18 | 18 | +0 |
| RDKB Contours (20m) | 92,359 | 92,359 | +0 |
| RDKB Legal Table | 35,438 | 35,562 | +124 |
| RDKB Mountain Peaks | 67 | 68 | +1 |
| RDKB ParcelLink Table | 41,560 | 41,732 | +172 |
| RDKB PMBC Parcels | 33,431 | 33,480 | +49 |
| RDKB Property Search | 37,416 | 37,659 | +243 |
| RDKB Road Name Labels | 4,184 | 4,190 | +6 |
| RDKB Taxes Table | 31,585 | 31,727 | +142 |

## Feature comparison

- RDCK address points: 156 GlobalIDs only in the current feed, 3,722 only in the old feed, and 149 matched IDs with changes to address, unit, community or folio.
- RDKB address points: 28 IDs only in the current feed, 2 only in the old feed, and 77 matching IDs with selected address fields changed. Object IDs are treated as identifiers for this layer, which may not be stable forever.
- RDKB parcels: 124 GlobalIDs only in the current feed, 75 only in the old feed, and 20 matching IDs with changes to selected parcel fields.
- RDKB property-search rows: 347 parcel/address/folio combinations only in the current feed, 104 only in the old feed, and 250 matching combinations with selected fields changed.
- RDCK cadastre: 50,811 current records plus 10,832 older records with absent or unmatched PIDs. PIDs are not unique; this is a coverage-preserving merge, not a count of deleted parcels.

The other datasets were refreshed for comparison but are not all map toggles and are not shipped in the application. Live basemap and provincial parcel sources change independently; no imagery acquisition-date or feature-level change is asserted.

Raw comparison details: [feature-comparison.json](feature-comparison.json); merge details: [layer-refresh-report.json](layer-refresh-report.json).
