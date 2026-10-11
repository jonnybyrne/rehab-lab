# gait-cycle — chart data

Data behind Essay 07, "Walking is controlled falling."

## Source

Normative teaching values in the Perry / Rancho Los Amigos gait-analysis
tradition, as presented in the essay. Joint angles approximate ±5°.
Extracted October 2026 from the essay's embedded key values (no external
retrieval; these are teaching values, not one person's recording).

## Files

- `joint-angles.csv` — the eight key values the curves interpolate between:
  `pct` (percent of gait cycle), `hip_deg`, `knee_deg`, `ankle_deg`.
- `phases.csv` — the eight Perry phases with the per-phase joint values
  shown in the scroll steps: `phase`, `pct_range`, `hip`, `knee`, `ankle`
  (values as written in the essay, e.g. `~28° flex`, `~8° PF`).

## Sign convention (joint-angles.csv)

Positive = flexion / dorsiflexion (the chart axis reads
"FLEXION / DORSIFLEXION POSITIVE"). Negative hip values are extension;
negative ankle values are plantarflexion.

## Transformations

None beyond extraction: the CSVs hold the raw key values exactly as
embedded in the essay. On the page, the joint-angle curves interpolate
linearly between the `joint-angles.csv` rows, and the walking figure,
clock, phase label, and joint readouts all read the same values.

## Gaps

- The center-of-gravity wave (~5 cm vertical, ~6 cm lateral) is drawn as a
  decorative schematic path, not plotted from data — no CSV for it.
- The stance 60% / swing 40% split, the ~10% double-support windows, and
  the ~40% single-support figure are single reference numbers stated in
  the essay text, not a dataset.
- Cadence (~101–122 steps/min) and step length (~2.5 ft) are broad
  teaching averages mentioned in the methods note; they are intentionally
  not used to score the figure.
