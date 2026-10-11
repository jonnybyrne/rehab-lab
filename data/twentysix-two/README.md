# Data: Essay 09 · 26.2 — "What happens to your body at every hour of a marathon?"

Values transcribed from the essay text in `/tmp/p3-snap.html` (Essay 09 build,
October 2026). **Nothing was recomputed and no data points were invented.**
Where the essay shows a derivation (e.g. 5 mmol/kg/km × 42.2 km ≈ 210 mmol/kg),
the CSV records the same arithmetic the essay shows.

## Files

- `clock_stops.csv` — the 7 race-clock stops plus the +24 h coda: clock time,
  distance, beat title, which runner(s), and the key claim at each stop.
- `fueling_bands.csv` — the carbohydrate-intake guideline bands behind the
  "What if you fueled differently?" slider (30 / 60 / 90 g/h).
- `fueling_mechanism.csv` — the Tsintzas et al. 1996 mechanism shown beside the
  slider: 25% type-I fiber glycogen sparing; exhaustion 104 → 132 min.
- `glycogen_arithmetic.csv` — the Sherman glycogen math behind the wall claim.
- `sweat_drift.csv` — sweat rates, body-mass loss, the 42.5% sweat-loss
  underestimate, and cardiovascular-drift figures.
- `wall_rates.csv` — self-reported vs pacing-defined wall rates (Buman 2008,
  Smyth 2021, Berlin 1999–2025, Boston 2015–17).
- `hyponatremia.csv` — Almond et al. NEJM 2005 Boston figures.
- `ck_enzymes.csv` — post-marathon creatine kinase figures (JAMA 1979/1981).
- `core_temperature.csv` — core-temperature plateau and the hot half-marathon
  outlier group.

## Sources

Every value traces to a source named in the essay's numbered footnotes
(notes 1–19) and the full source list in the essay's "How this was built"
section. Key primary sources: Sherman et al. (Int J Sports Med, glycogen
utilization); Bergström et al. 1967 (glycogen stores); Wingo, Ganio & Cureton
2012 (cardiovascular drift); Stone et al. 2025 (drift magnitude); Lara et al.
(sweat rate); Almond et al. NEJM 2005 (hyponatremia); Tsintzas et al. 1996
(carbohydrate mechanism); Jeukendrup 2012 / ACSM (fueling guidelines); Smyth
2021 and Buman et al. 2008 (wall rates); PLoS One 2025 (Boston pacing).

## Dates and transformations

- **Source reading:** October 2026 (per the essay's methods note).
- **Extraction:** October 11, 2026, transcribed from the essay build.
- **Transformations:** none beyond transcription. Ranges and tildes are kept
  exactly as written in the essay ("~", "–", "≈"). Unicode minus signs are
  preserved.

## Caveats (from the essay)

- Priya, Marcus, and Louise are **illustrative composites** — made-up names
  and ages over real published numbers.
- Cardiovascular-drift and hypohydration heart-rate figures are **lab data**
  (cycling), not marathon-race measurements.
- The Berlin 1999–2025 wall figures are as reported in news coverage; the
  original was not checked.
