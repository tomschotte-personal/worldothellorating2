# World Othello Rating — Shift-1800 (experimental)

Experimental rating scale where `INITIAL_RATING = PRIOR_RATING = 1800` (vs the
official 1500). Identical algorithm to the main published rating, only the
two anchor constants differ.

**Why:** Aligns the rating scale with the historical WOF intuition that world
champions sit at 2400+. With this anchor, the top ~15 active players cross
2400 cleanly and the K=10 sticky floor at 2400 engages as designed in FIDE.

**Effect on ratings:** every player is shifted +300 from the official scale.
Relative ordering is preserved exactly — this is a calibration shift, not a
ranking change.

| Official top | Shift-1800 top |
|---|---|
| Takahashi 2333 | Takahashi 2575 |
| Suekuni 2266 | Suekuni 2533 |
| Kurita 2254 | Kurita 2526 |
| Takanashi 2251 | Takanashi 2540 |
| Fukuchi 2239 | Fukuchi 2480 |

**To convert:** subtract 300 to get the official-scale equivalent.

Main published rating: <https://tomschotte-personal.github.io/worldothellorating/>
