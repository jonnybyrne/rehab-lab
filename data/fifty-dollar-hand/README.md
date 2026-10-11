# Chart data — Essay 06 · "Why does a humid 75°F morning feel so bad?"

Every value in these CSVs was extracted from the essay's own page source (October 2026 build). Nothing was invented; computed columns reuse the essay's stated method.

## Files

- `miami-dew-point-normals.csv` — NOAA 1991–2020 U.S. Climate Normals, Miami International Airport: mean dew point for June–September (72.0, 73.0, 73.8, 73.2°F). The other eight months were intentionally left unquantified in the essay.
- `che-muhamed-2016-conditions.csv` — the five treadmill atmospheres from Che Muhamed et al., *Temperature*, 2016 (DOI 10.1080/23328940.2016.1182669): relative-humidity conditions at 31°C, with time-to-exhaustion significance versus the 23% RH reference (P=0.045 at 61%, P=0.005 at 71%; no reported significance at 43% or 52%; whole-body sweat loss P=0.183).
- `ely-2008-wbgt-slowdown.csv` — Ely et al., *Medicine & Science in Sports & Exercise*, 2008 (DOI 10.1249/mss.0b013e31802d3aba): top-men's marathon slowdown versus course-record pace across four WBGT quartiles (1.7%, 2.5%, 3.3%, 4.5%).
- `day-a-day-b-comparison.csv` — the essay's worked comparison: Day A (75°F, 90% RH, 72°F dew point) vs Day B (95°F, 40% RH, 67°F dew point, ≈99°F heat index).
- `comfort-bands.csv` — the runner's dew-point comfort bands (≤54 through ≥75°F) as shown in the essay's band table.
- `hadley-pace-bands.csv` — coach Mark Hadley's 2013 temperature-plus-dew-point pace-adjustment bands (0.5% at 101–110 through 10% at 171–180; 0% at ≤100; outside the table above 180).
- `acsm-event-alert-flags.csv` — the classic 2007 ACSM Event Alert System WBGT thresholds (white <50 through black >82°F).

## Sources & dates accessed

- NOAA 1991–2020 Climate Normals; NWS Miami summer-season climatology — read October 2026.
- Che Muhamed et al. 2016 and Ely et al. 2008 via their published records — read October 2026.
- Comfort chart: letsrun.com forum thread 3139849 (~1995), cross-checked against NOAA/NWS conventions.
- Hadley 2013 pace bands; 2026 preprint describing them as "not peer-reviewed physiology."
- ACSM 2007 Event Alert System; ACSM 2023 exertional-heat-illness consensus (current clinical reference).

## Transformations

- Dew points (`dew_point_f`, `dew_point_f_computed`) were computed from air temperature and relative humidity with the Magnus–Tetens approximation (b=17.625, c=243.04°C), matching the essay.
- Day B heat index (≈99°F) uses the NWS Rothfusz regression, shown only at ≥80°F air temperature; Day A's cell is blank because the regression is not valid below 80°F.
- Lab bar heights in the essay are categorical emphasis, not unreported time-to-exhaustion values — no TTE magnitudes are stored here.
- The pace rule and comfort chart are coaching heuristics, not peer-reviewed physiology; the CSVs record the bands as published, not as prescriptions.
