# Data: The Pickleball Fracture Curve

Chart data used in the essay, extracted from the values in the published page.
No new data collected; see essay footnotes for full citations.

## Files
- `participation.csv` — SFIA U.S. pickleball player estimates, 2019–2024 (millions).
- `ed_endpoints.csv` — NEISS nationally estimated pickleball ED visits for the two
  verified Cheng endpoints (2020, 2022) with the essay's derived per-1,000-player rates.
- `age_anchors.csv` — published age anchors for ED injuries (Cheng et al. 2024).
  Only the 60–79 combined share (73%) and mean age are published; other bins are
  shown pale in the chart with no values.
- `mechanism.csv` — falls and wrist-injury shares (Yu et al. 2025; Weiss et al. 2021).

## Sources and access
- Cheng R, et al. 2024 (NEISS analysis, via PubMed Central). DOI 10.1016/j.asmr.2024.101067.
- Yu J, et al. 2025. DOI 10.1177/23259671241305364.
- Weiss H, et al. 2021. DOI 10.1186/s40621-021-00327-9.
- SFIA 2025 Topline Participation Report.
- Data extracted from the essay file on 2026-10-11.

## Transformations
- Per-1,000-player rates are the essay's own arithmetic (ED visits ÷ SFIA players),
  not published incidence rates.
- The 2020 dip (−14%) is shown as reported; the essay labels it a pandemic
  closure artifact, not a modeled safety improvement.
