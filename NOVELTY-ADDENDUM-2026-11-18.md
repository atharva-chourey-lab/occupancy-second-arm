# NOVELTY ADDENDUM — Occupancy claims vs Waugh & Thewissen (2021)

**Atharva Chourey Lab · Addendum to the Occupancy Audit (Target 2,
2026-11-17) and Occupancy Second Arm (2026-11-18) · Scrub run
2026-11-18 in response to an external reviewer's prior-art citation,
following the lab's research_novelty_scrub procedure. This addendum
corrects the novelty framing of the occupancy work. It does not change
any number in either RESULTS.md.**

## The citation, verified at source

Waugh, D.A. & Thewissen, J.G.M. (2021). "The pattern of brain-size
change in the early evolution of cetaceans." *PLoS ONE* 16(9):
e0257803. DOI 10.1371/journal.pone.0257803 · PMCID PMC8478358 ·
PMID 34582492. Received 2020-11-13, published 2021-09-28. Verified
against the full text (PMC), not a summary.

**The reviewer's citation is real, and it is not an external prior —
it is one of this project's own sources.** The first arm's cleanest
dataset (the "Waugh paired" arm, n = 26, median 0.920) is Waugh &
Thewissen's S1 Table, and the second arm was anchored to it. The
scrub below therefore grades our claims against a paper we already
cite and use — which makes the overlap worse, not better: parts of
what we presented as findings are restatements of our anchor's own
published results.

## What Waugh & Thewissen (2021) actually show

- **Sample.** A calibration set of extant placental mammals in which
  endocranial volume was *measured directly* and paired with brain
  mass: species means of 611 specimens, **26 species in 18 genera**
  (S1 Table), spanning many placental orders but assembled for a
  cetacean/artiodactyl question; plus new dissections (beluga,
  bowhead, goats, pigs; their Table 1). Fossil cetaceans and fossil
  artiodactyls are analysed with the resulting equation, but the
  occupancy distribution itself is extant-only.
- **The occupancy range, in their words** (Discussion): *"Our results
  show the brain fills (by volume) approximately 33 to 98 percent (or
  70–98 percent if the only mysticete for which there is data is
  excluded) of the cranial cavity in extant placental mammals
  (including terrestrial artiodactyls and cetaceans), with the
  percentage decreasing with increasing body size."* Within the
  body-size range of their fossil cetaceans, predicted occupancy is
  66–81%.
- **Bowhead.** Their worked example: a bowhead brain of 2,948 g
  (≈2,835 cm³ at cetacean density 1.04) against a measured ECV of
  ≈8,400 cm³ — 66% of the cavity is adnexa + CSF. Their Introduction,
  citing Thewissen et al., states the bowhead brain "only occupies
  approximately 40 percent of the cranial cavity." They explicitly
  discuss "the outlier status of the bowhead, in terms of scaling,"
  and warn that fossil-mysticete brain estimates "should be treated
  with caution." (Our 0.323 is computed from a different tabulated
  pair in their supplement — brain 2,980 g, ECV 8,900 cm³ — same
  animal population, same conclusion.)
- **The 100% assumption.** Named and rejected in their Introduction:
  some scientists "assume the brain occupies the entire cranial
  cavity… essentially equating endocranial volume with brain mass";
  the volumetric discrepancy is "quantitatively more important than
  the relatively minor adjustment for brain tissue density." Their
  remedy is an allometric PGLS equation (log₁₀ brain mass =
  0.933·log₁₀ ECV + 0.088; adj. R² = 0.991), and their Discussion
  estimates fossil artiodactyl/cetacean ECVs "would need a volumetric
  reduction of approximately 24 percent… to approximate brain volume."
- **What they do not do.** No median occupancy, no fraction-inside-a-
  band statistic, no cross-compilation join, no audit of any other
  dataset's internal derivation, and nothing about Dembitzer et al.
  (2022), which postdates them.

## Per-part grades of our claim

Our compound claim, split as registered:

**(a) "Occupancy varies and is not ~100%" — ALREADY PUBLISHED.**
Waugh & Thewissen (2021), verbatim range 33–98% (70–98% ex-mysticete),
allometric (not constant) scaling, explicit rejection of the
equate-ECV-with-brain-mass assumption, a published correction
equation and a ~24% average fossil reduction. Behind them stand
Ridgway et al. (adnexa variability in extant cetaceans) and
Boessenecker et al. (2017, adnexa correction), both cited by Waugh —
so even the "measurement error" consequence for fossil EQ was in the
literature before us. **Any presentation of the occupancy audit that
leads with "the brain does not fill the skull" as a discovery is
wrong and is corrected here: that is Waugh & Thewissen's result,
which we used as an anchor.**

**(b) "Bowhead specifically low" — ALREADY PUBLISHED.**
It is Waugh & Thewissen's own extreme example and their own word
("outlier") before it was ours; the underlying datum is theirs
(Thewissen et al.'s bowhead measurements). Our residual contribution
is narrow and negative: on the only paired data, the bowhead does
*not* generalise to Cetacea (beluga 0.792, dolphin 0.937 — also
computed from Waugh's table). That is a correct caution, not a
finding. Grade forced by Waugh & Thewissen (2021).

**(c) Cross-dataset median 0.919 / band statistics (n = 42; second
arm n = 58, median 0.932, 65.5% outside) — NARROWED BUT OPEN.**
The narrowing is severe and must be stated: our combined n = 42
median (0.919) is majority-Waugh (26 of 42 species are Waugh's own
S1 species, whose recomputed range in our hands is 0.323–0.976 —
i.e. their published 33–98% restated), and the Waugh-arm median
0.920 is a re-summary of their distribution in a statistic (median /
band fraction) they did not report, not new evidence. What Waugh
does not contain, and a widened search (2026-11-18; terms for
cross-mammal occupancy medians/band fractions) found no other prior
for: (i) the *cross-compilation* joins (Dembitzer × Patzke bridge,
Sakai × Patzke, Brain Catalogue MRI arm) and their diagnostic —
19–60% of species with physically impossible occupancy >100%,
i.e. ruler disagreement larger than the occupancy shortfall itself,
where Waugh's directly-measured set is clean by construction
(R² = 0.991, nothing above 100%); (ii) per-order band statistics
outside Cetartiodactyla (Carnivora, Primates, Perissodactyla arms);
(iii) the second arm's independent-subset statistic on the Burger
ruler (n = 58, median 0.932). Surviving seam for (c): *a
cross-compilation occupancy distribution whose headline is ruler
disagreement (>100% occupancies), not the occupancy level.* The
level was published in 2021; the disagreement across compilations
was not.

**(d) The circularity findings — OPEN (no prior found).**
(i) Dembitzer et al. (2022, *Sci Rep* 12:3453) back-calculation:
their supplement's brain-mass and endocast records are disjoint
species sets; for the 149 brain-mass species the published
"Endocast Volume" equals brain volume × 1.108 (median; IQR
1.085–1.125) — an assumed ~90.2% occupancy encoded in the largest
modern ECV dataset. Dembitzer's main text states only that endocast
volumes were "recorded… from the literature and directly from skull
digital models"; no conversion is stated there. (ii) The second
arm's photocopy block: 71 of 129 Burger × Dembitzer shared species
carry the identical number on both sides (54 Ashwell marsupials,
exact; 17 Isler primates, equal at print precision), so a naive join
reports 70.5% of species inside the 90–100% band and appears to
confirm the identity the block manufactures. Two widened searches
(2026-11-18) found **no published critique, correction or audit of
either derivation** — the only hits are the source papers
themselves. Caveat recorded honestly: a search returning nothing is
weak evidence; the grade is "open, no prior found," and the ×1.108
pattern is detectable by a careful reader of Dembitzer's supplement
(the records are kept in separate files) — our claim is the
*measurement and its consequence*, not that the data were hidden.

## Corrected one-sentence claim

> Waugh & Thewissen (2021) established that mammalian brain
> occupancy varies (~33–98%) and is not 100%; what this lab adds is
> (1) a cross-compilation audit showing the field's brain and skull
> rulers disagree by more than that shortfall (up to 60% of joined
> species above a physically impossible 100% occupancy), and (2) the
> first measurement of two circularities that manufacture apparent
> support for the folk occupancy band — Dembitzer et al.'s ×1.108
> back-calculation for 149 species and the 71-species
> identical-value block (55% of the Burger × Dembitzer join).

## Verdict on the reviewer's framing

**Fair — in substance, and if anything understated.** The reviewer
said occupancy variation (33–98%), the error in assuming complete
occupancy, and bowhead-low were already established, and that only
the circularity analysis survives. All three "already established"
items are verbatim in Waugh & Thewissen (2021) — including the exact
33–98% range and the word "outlier" for the bowhead. The reviewer
did not add that the establishing paper is *our own anchor source*,
so our Waugh-arm "cleanest result" (median 0.920) is a re-summary
of their published distribution. The one place the reviewer's
summary is incomplete: the cross-compilation ruler-disagreement
result (>100% occupancies; part (c)(i)) is also not in Waugh and
survives alongside the circularity — it, not the occupancy level,
is the audit's defensible headline. Presentations of this work
should lead with ruler disagreement + circularity and cite Waugh &
Thewissen (2021) as the source of the occupancy-variation result
itself.

*Scrub sources: Waugh & Thewissen 2021 full text (PMC8478358);
Dembitzer et al. 2022 full text (PMC8971383); project RESULTS.md
(first arm) and RESULTS.md (second arm) for our numbers; widened
searches logged 2026-11-18 (occupancy-median/band terms;
Dembitzer-derivation/audit terms — no closer prior returned for
(c)(i–iii) or (d)).*
