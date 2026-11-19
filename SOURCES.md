# Sources Map — Occupancy, Second Arm (Burger × Dembitzer, independent subset)

Author: Atharva Chourey
Affiliation: Atharva Chourey Lab (independent research lab)

*Manuscript — not yet peer-reviewed.*

This file maps every key number, verdict and reference in `paper.md` to the source file it was taken from. Nothing in the paper was taken from a source outside this list.

## Primary sources

- `~/workspace/occupancy-second-arm/RESULTS.md` — the run record: verdict, join table, headline distribution, per-order medians, extremes, the P1–P6 scorecard, the back-filled block audit, sensitivities S0–S3, and the strengthens/complicates assessment the paper's §8 follows.
- `~/workspace/occupancy-second-arm/PREREGISTRATION.md` — frozen 2026-11-18 (commit `0353845`) before the full join was built or any occupancy in this arm was computed; Amendment A1 (commit `1b6d84e`) redefined the identical-value exclusion at two-decimal equality after the first run failed to replicate PAIR-1's block count, and before the corrected primary analysis. Predictions and kill criteria were not changed by the amendment.
- `~/workspace/occupancy-second-arm/outputs/summary.json` — machine summary of both joins; every headline number in the paper was checked against it during the publication build.
- `~/workspace/occupancy-second-arm/outputs/joined_independent.csv` — the joined table: all 129 shared species, excluded species flagged with reasons.
- `~/workspace/occupancy-second-arm/scripts/run_second_arm.py` — the build/analysis script.
- `~/workspace/research-tools/campaigns/CAMPAIGN-PAIR-1-RESULTS.md` — Pair Hunter PAIR-1: the pair's discovery and row-level sample verification (151 shared rows, 71 identical, ~80 remaining, median ≈ 0.971, 55% outside), which this arm's sensitivity S2 replicates exactly.
- First arm: `~/workspace/brain-scan-comparison/projects/occupancy-audit/` (PREREGISTRATION.md as amended, RESULTS.md, outputs) — published as the `occupancy-audit` manuscript repo.

## Underlying datasets (as cited in the sources above)

- Burger et al. 2019 mammal brain-mass canon, local file `~/workspace/brain-scan-comparison/projects/photocopy-chain/data/burger_data.csv` (1,552 species with mean brain mass).
- Dembitzer et al. 2022 supplementary table MOESM1, local file `~/workspace/brain-scan-comparison/projects/occupancy-audit/data/dembitzer_supp/41598_2022_7327_MOESM1_ESM.csv`, restricted to Method = "Volume" rows (218 rows / 192 unique species; the 149 Method = "Mass" species excluded as back-calculated, ECV = brain × ~1.108, per the first arm).
- Waugh & Thewissen 2021 paired table (anchor, n = 26) and the audited Patzke clean table (357 species), as joined in the first arm.

## Key numbers and their sources

| Claim in paper | Value | Source |
|---|---|---|
| Shared species (extant) | 129 | RESULTS.md, The join; summary.json `shared_species_all` |
| Excluded identical-value block | 71 species (55.0% of shared) | RESULTS.md §3/§6; summary.json `excluded_species` |
| Independent arm | n = 58 | RESULTS.md; summary.json `independent_n` |
| Median occupancy (independent, primary units) | 0.932 (IQR 0.882–1.006; range 0.535–4.285) | RESULTS.md, Headline distribution; summary.json `independent_primary` (0.9316) |
| Outside 90–100% (independent) | 65.5% (37.9% below, 27.6% above 100%) | RESULTS.md; summary.json `independent_primary` (0.6552) |
| Naive join | median 0.965; 70.5% inside the band | RESULTS.md §6; summary.json `naive_extant_primary` (in-band 0.7054) |
| Marsupial block | 54 species, Ashwell (2008) on both sides, exact equality | RESULTS.md §6 |
| Primate block | 17 species, Isler et al. (2008) on both sides, equality at 2 dp | RESULTS.md §6; PREREGISTRATION Amendment A1 |
| Scorecard | P1 FAIL (n = 58 < 60); P2–P4 PASS; P5 PASS (+36.1 pts in-band inflation); P6 PASS with refinement; K1/K2/F1 not fired | RESULTS.md, Prediction scorecard |
| First-arm comparators | combined n = 42 median 0.919; Waugh n = 26 median 0.920; bridge n = 10 median 1.010 | RESULTS.md; first-arm RESULTS.md |
| S2 replication | 151 rows, 71 identical, 80 remaining, median 0.970, 55.0% outside | RESULTS.md, Sensitivities |
| S3 Patzke swap | n = 10, median 0.999 | RESULTS.md, Sensitivities |
