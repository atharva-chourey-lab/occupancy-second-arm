# Occupancy, Second Arm: On Independent Data the Brain Still Does Not Fill the Skull — and a Naive Join of the Same Data Appears to Prove That It Does

Author: Atharva Chourey
Affiliation: Atharva Chourey Lab (independent research lab)

*Manuscript — not yet peer-reviewed. Sequel arm to "The Brain Does Not Fill the Skull" (occupancy-audit), run under a pre-registration frozen before the join was built.*

## Abstract

The first occupancy audit joined brain volumes to endocranial volumes (ECV) for 42 mammal species and found median occupancy 0.919 — but the brain ruler the fossil ecosystem actually uses, Burger et al. (2019), could not be joined at all, and the one arm pairing a compilation brain ruler with measured ECV had n = 10. This second arm runs the join the first arm wanted: Burger's brain-mass canon against Dembitzer et al.'s (2022) measured (Volume-method) endocast volumes, under a pre-registration frozen before any occupancy in this arm was computed. The two datasets share 129 extant species — but 71 of them (55.0%) carry the identical number on both sides: for 54 marsupials the "ECV" is Ashwell's (2008) brain-mass number, cited by both datasets, and for 17 primates it is Isler et al.'s (2008) table carried at two print precisions. Those species sit at occupancy 1.000 by construction and cannot test anything; the pre-registration excludes them before analysis. On the remaining 58 independent species, median occupancy is 0.932 (IQR 0.882–1.006) and 65.5% of species fall outside the 90–100% band — the first arm's verdict reproduced on a second brain ruler at roughly six times the bridge arm's n. A naive join of all 129 species, by contrast, reports 70.5% of species inside the band and appears to confirm the 100% identity: the identity's apparent support in this dataset pair is manufactured by the back-filled block. The central value is ruler-dependent (Waugh paired 0.920, first-arm combined 0.919, Burger-independent 0.932, Patzke bridge ~1.0); no single occupancy constant survives. The prediction scorecard is 5 pass, 1 fail (the registered size prediction, n ≥ 60, missed at 58 — above the registered kill floor of 40, so the arm stands).

*Keywords:* endocranial volume; encephalisation quotient; occupancy; comparative neuroanatomy; data provenance; pre-registration

## 1. Why a second arm

Fossil encephalisation quotients rest on an identity: that endocranial volume equals brain volume, an occupancy of 100%. The first arm of this audit ("The Brain Does Not Fill the Skull", published as `occupancy-audit`) tested that identity in extant material and found it false — median occupancy 0.919 across a 42-species join, with 59.5% of species outside the 90–100% band and 19.0% above a physically impossible 100%.

But the first arm had two open seams. Its combined join escaped its own join-kill by two species (n = 42 against a floor of 40). And its only arm pairing a compilation brain ruler with measured ECV — Dembitzer × Patzke — had n = 10, median 1.010. The brain ruler the fossil ecosystem actually uses, Burger et al. 2019, was gated at Dryad during the first arm and could not be joined at all. Burger's data have since been obtained locally (for the Photocopy Chain project), so the join the first arm wanted is now runnable.

The Pair Hunter campaign (PAIR-1) found and sample-verified this pair from the raw files and named it as its mint candidate — and its verification surfaced a structural defect that this arm's pre-registration exists to neutralise before any number is computed: a majority of the species the two datasets share carry the same number on both sides (§3).

The audit question is unchanged from the first arm: in living mammals, what fraction of the cranial cavity does the brain occupy, and is the 100% identity (or the 90–100% folk band) defensible? The background is settled and is not this arm's claim: Waugh & Thewissen (2021) established that occupancy varies across mammals (~33–98% on directly measured pairs) and is not 100%; their paired table anchors both arms. This arm's claims are the independent-subset statistic on the Burger ruler and the identical-value block documented in §3 — a circularity inside the join itself, for which no prior exists.

## 2. Datasets and measure

**Brain ruler:** Burger et al. 2019 mammal brain-mass canon — 1,552 species with mean brain mass. **Skull ruler:** Dembitzer et al. 2022 supplementary table, restricted to Method = "Volume" rows (measured endocast volumes): 218 rows, 192 unique species, 142 of them extant. Dembitzer's 149 Method = "Mass" species are excluded entirely, as in the first arm: their published ECVs are back-calculated from brain mass (ECV = brain × ~1.108), an assumed ~90.2% occupancy wearing a lab coat.

**Anchors (comparison only):** the Waugh & Thewissen 2021 paired table (n = 26, median occupancy 0.920) and the audited Patzke clean table (357 species), used in sensitivity S3.

The measure follows the first arm's convention exactly, so the medians are directly comparable. The universe is extant species only. The join key is the binomial, case-insensitive, with no synonym mapping and no fuzzy matching. Species-level ECV is the median of the species' Volume rows. Occupancy (primary) = (Burger brain mass ÷ 1.036 g/ml) ÷ ECV — the field's own density convention. Nothing is winsorised, trimmed, or excluded post hoc; values above 100% are reported as-is, and their frequency is a reported statistic.

## 3. The registered exclusion: the back-filled block

Pair Hunter's row-level verification found, before this project existed, that of 151 shared row-pairs, 71 carry the identical number on both sides. For those species the "ECV" is the brain-mass number photocopied into the skull column: the two rulers are one number, their occupancy is 1.000 by construction (raw units), and they cannot test anything.

The pre-registration therefore fixed the rule before analysis: a shared species is excluded from the independent arm if any of its Dembitzer Volume rows carries a volume numerically equal to its Burger mean brain mass, and every excluded species is listed in the published joined table with its reason.

One amendment was required, and it is on the record. The first implementation used exact float equality and found only 54 identical rows — it failed to replicate PAIR-1's 71. Inspection showed why: the 17 primate pairs are the same number carried at different printed precision (Burger prints *Trachypithecus phayrei* as 72.84012102 g, citing `islerPrim2008`; Dembitzer prints 72.84 ml, citing Isler et al. 2008). Amendment A1 — committed after the replication failure and before the corrected primary analysis — redefined "identical" as equality at two decimal places, Dembitzer's own printed precision, which reproduces PAIR-1's count exactly. The exact-equality run is retained as sensitivity S0. Predictions and kill criteria were not changed by the amendment.

## 4. Results

| Stage | n |
|---|---|
| Burger species with brain mass | 1,552 |
| Dembitzer Volume rows / unique species | 218 / 192 (142 extant) |
| Shared species (all extant) | **129** |
| Excluded: identical-value block | **71** |
| **Independent arm** | **58** |

On the 58 independent species, in primary units:

- **Median occupancy 0.932** (IQR 0.882–1.006; range 0.535–4.285).
- **65.5% of species fall outside the 90–100% band** — 37.9% below 90%, and **27.6% above 100%** (a ruler-mismatch diagnostic, reported as-is, nothing trimmed).
- Raw-units sensitivity (mass ÷ ECV): median 0.965, 56.9% outside.

Against the first arm: combined n = 42 median **0.919** (59.5% outside); Waugh paired anchor n = 26 median **0.920** (0% above 100%); Dembitzer × Patzke bridge n = 10 median **1.010** (60% above 100%). This arm's median sits just above the Waugh/first-arm centre and well below the bridge — but its *spread* is bridge-like, not Waugh-like: 27.6% of species with brains "larger than their skulls", against Waugh's 0%. Same-source pairs are tight; cross-compilation joins are not, whichever compilation supplies the brain.

Per-order medians (orders with ≥3 species): Carnivora 0.937 (n = 19, 84% outside the band); Primates 0.931 (n = 25, 52% outside); Diprotodontia 0.973 (n = 5); Pilosa 0.913 (n = 3); Monotremata 0.810 (n = 3); Cingulata 1.084 (n = 3, 100% outside).

Extremes, reported as-is: lowest — *Bradypus variegatus* 0.535, *Ailuropoda melanoleuca* 0.727, *Conepatus leuconotus* 0.777. Highest — *Melogale personata* **4.285** (a Burger mass of 61.4 g against a 13.83 ml ECV; the Burger value itself is implausible for a ferret-badger and looks like a Photocopy-Chain-class canon defect — flagged here, not removed), *Euphractus sexcinctus* 1.566, *Piliocolobus badius* 1.167.

Dembitzer contains no cetaceans, so this arm is silent on them; the bowhead (0.323) remains a Waugh-only datum, as registered.

## 5. Prediction scorecard

| # | Prediction | Result |
|---|---|---|
| P1 | Independent n ≥ 60 | **FAIL — n = 58.** Above the kill floor of 40, so the arm stands, but the registered size prediction missed by two species — the same two-species margin by which the first arm escaped its own join-kill, in the other direction. |
| P2 | Median in 0.90–0.97 | **PASS — 0.932.** |
| P3 | ≥50% outside 90–100% | **PASS — 65.5%.** |
| P4 | Median above 0.919 and 0.920, below 1.00 and below the bridge's 1.010 | **PASS — 0.932**, exactly the registered direction. |
| P5 | Naive join inflates the in-band fraction by ≥5 points and raises the median | **PASS, decisively — in-band 70.5% naive vs 34.5% independent (+36.1 points); median 0.965 vs 0.932.** |
| P6 | Block ≥80% Diprotodontia/Primates, Ashwell-attributable | **PASS with a refinement — 71/71 (100%) are Diprotodontia (54) or Primates (17), but there are two lineages, not one (§6).** |

Kill/fallback criteria: K1 (thin arm, n < 40) did not fire; K2 (identity survives) did not fire; F1 (median ≥ 1.00) did not fire.

## 6. The back-filled block audit

The block is a finding in its own right, and it was half the registered deliverable.

- **71 species = 55.0% of all shared species.** Any Burger × Dembitzer join that does not exclude them is majority-photocopy on its shared set.
- **Marsupial block (54 species, all Diprotodontia):** exact numerical equality as printed. Dembitzer's "measured endocast volume" for these species *is* Ashwell's (2008) brain-mass number, and Burger's mass for the same species cites the same Ashwell source — Ashwell on both sides, 54/54. One measurement, two columns, two datasets.
- **Primate block (17 species):** equality at two decimal places — Dembitzer's printed precision. Dembitzer's ECVs are Isler et al. 2008 endocranial volumes; Burger's masses for these species derive from the same Isler table (Burger value = Isler ECV carried at full precision). The numbers agree because they are the same numbers, converted by nobody. Isler is Burger's sole reference for 17/17.
- **What it does to a naive join:** the block's species sit at raw occupancy 1.000 (0.965 in primary units) — dead centre of the folk band. Naive join: median 0.965, **70.5% inside 90–100%** — a result that reads as "the identity roughly holds, folk band confirmed". Independent join: median 0.932, **34.5% inside**. The block does not nudge the answer; it reverses the headline.
- **Definition sensitivity:** S1 (exclude only species whose median ECV equals the mass at 2 dp) excludes 68 and keeps 61 (median 0.937, 62.3% outside); the three differing species each carry one identical row and one genuine row. The verdict is insensitive to which registered definition is used. The demoted exact-equality arm S0 (excluding only the 54 marsupials) gives median 0.965 with 50.7% outside — visibly pulled toward the identity by the primate block it fails to exclude.

## 7. Sensitivities

- **S2 (PAIR-1 replication, row-level, all species, raw units):** 151 shared rows, 71 identical, 80 remaining — median **0.970**, **55.0% outside** — reproduces PAIR-1's recorded sample (0.971 / 55%) in full. The record and this run are the same computation.
- **S3 (Patzke swap on the independent set):** n = 10, median **0.999**, 50% above 100% — the first arm's bridge arm (n = 10, 1.010) reproduced almost exactly on the same species set. The histology-lineage brain ruler reads ~7 points higher against Dembitzer ECV than Burger does on the same species, confirming the bridge was a ruler effect, not a join accident.

## 8. What this does to the published occupancy-audit claim

**Strengthens:** the core claim — *the brain does not fill the skull; no single occupancy constant survives* — now holds on the Burger ruler as well as the Patzke and Waugh rulers, at n = 58 independent species, with the pre-registered exclusion doing the work the first arm could not do (Burger was gated then). The "ruler chaos" half of the first arm's headline is also strengthened: this arm's spread (27.6% above 100%) resembles the bridge, not the clean Waugh pairs.

**Complicates:** (1) The central value is ruler-dependent in a narrower band than the first arm suggested — Waugh 0.920, combined 0.919, Burger-independent 0.932, Patzke-bridge ~1.0. "≈0.92" is a Burger/Waugh statement, not a constant of nature. (2) The published audit's own framing missed that the largest ECV dataset's *Volume* rows are themselves partly back-filled from brain masses, for the two orders where a single source (Ashwell; Isler) supplied both literatures — the Mass-method circularity the first arm caught (149 species, ×1.108) has a quieter Volume-method sibling (71 species, ×1.000). (3) Any future Burger × Dembitzer join published without an identical-value exclusion should be read as measuring the block, not occupancy.

**Licensed statement:** "On the 58 mammal species where Burger's brain masses and Dembitzer's measured endocast volumes are genuinely independent numbers, median occupancy is 0.932 and two-thirds of species fall outside 90–100%. A further 71 shared species — 55% of the join — carry the same number on both sides and cannot test occupancy at all."

## 9. Known limitations

Neither ruler is measured on the same individuals; occupancy here is a species-level ratio of two compilations. Burger is itself a compilation with documented photocopy-chain defects; a Burger-specific error enters this arm one-for-one — the Patzke swap (S3) and the Waugh anchor bound, but do not remove, that risk (the *Melogale* extreme in §4 is a visible instance). Dembitzer's species-level ECVs average different specimen sets per species; duplicate Volume rows are collapsed by the registered median rule, which is a choice, declared in the pre-registration.

## Sources

Every number in this paper is traced in [SOURCES.md](SOURCES.md) to the run record (`RESULTS.md`), the frozen pre-registration and its Amendment A1, the machine summary (`outputs/summary.json`), and the published joined table (`outputs/joined_independent.csv`) of the second-arm project.
