# Chart data — Essay 10, "The Most Expensive Steps"

Extracted from the essay's own page source (`p3-snap.html` working copy of
jonnybyrne.github.io/rehab-lab, expensive-steps view + its script block).
No values were invented, rounded, or recalculated; every number below is
byte-identical to a value already present in the file.

- Source: the essay page source itself (all figures trace to the studies
  listed in the essay's Notes and full source list).
- Date accessed / extracted: 2026-10-11.
- Transformations: mechanical extraction only — JS object literals and the
  fare-schedule HTML table were converted to CSV rows with no arithmetic.
  The fare meter's scroll mapping (1.0× at the top of the essay to 7.7× at
  the bottom) is computed in-page as 1 + 6.7 × scroll progress, not stored
  data, so it has no CSV.

## Files

- `room_dots.csv` — the 1,000-tag room: 17 walker groups, each with dot
  count, fare multiple vs the intact walker, O₂ cost (mL/kg/m), walking
  speed, daily steps, and a short source label. Sums to exactly 1,000 dots.
- `rate_cost_bars.csv` — the rate-vs-cost toggle: per condition, O₂ rate
  (percent of normal per minute) and O₂ cost (multiple of normal per meter),
  low and high of the published range.
- `fare_schedule.csv` — the fare-schedule table rows: condition, detail
  text, and the low/high fare multiples.
- `oxygen_budget_options.csv` — the daily-oxygen-budget calculator menu:
  O₂ cost per option, default steps per day, source tag, and whether the
  default step count is an estimate (true where no published step data exist).
- `feet_lists.csv` — the 1970 vs 2025 prosthetic-feet lists: name,
  description, 2025 Medicare fee-schedule price (or "price not published"),
  and added/removed/remained status.

## Caveats carried over from the essay

- The room is a modeled mix, not a census; condition shares are editorial
  estimates, and the stroke share of hemiplegic-gait walkers has no
  published headcount.
- The intact-walker baseline (~0.15 mL O₂/kg/m) is a textbook reference
  value, not a study result.
- Ranges are shown where studies disagree (transtibial 1.0–1.6× across
  four studies), never averaged.
- The hip-disarticulation figures have no entry in the essay's source
  register and are flagged for verification against the primary literature.
- The 1970 SACH price was never published; the list says "price not
  published" instead of inventing one.
