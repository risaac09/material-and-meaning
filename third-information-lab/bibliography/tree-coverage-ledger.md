# Material and Meaning: tree-wide source-coverage ledger

Audit date: 2026-06-25. This ledger answers one question honestly: is the whole Material and Meaning tree, folders and subfolders, in a verified bibliography. The short answer is below, then the per-surface map.

## Verdict

No -- the tree is not yet a single fully-verified bibliography, but it is close and the remaining gaps are honestly bounded: the four claim-bearing prose surfaces (TIL thesis 158, M&M literature 91, the published position-paper 31, and now the two empirical pilots' data manifests plus the funder facts and embodied-science records) all resolve to real, correctly-named sources with no fabricated citations, DOIs, or URLs found anywhere. What is NOT in the verified bibliography is the org/dossiers layer (the institute's own internal source material, un-audited), a handful of self-sourced Templeton/NIMHD dollar-and-count figures that block automated fetchers, and a labeled residual literature queue (Li 2016, Powell 2003, Cohen 2016, Norris-Inglehart, the PLOS ONE 2025 ABM) -- all of which are explicitly flagged in-file as to-verify, and the esoterica/foundation-voice claims are deliberately register-labeled rather than graded, so nothing un-verified is posing as fact.

## Gap-closing update (2026-06-26)

Four named gaps were worked. Three closed, one downgraded, with two small items still pending a human.

- **Gap 1 (org/dossiers) CLOSED.** All five collaborator dossiers verified against live sources: Christopher Seto (Purdue), Ellen Idler (Emory), Tyler VanderWeele (Harvard Human Flourishing Program), Richard Sosis (UConn), Daniel Hungerman (Notre Dame), plus the Harvard HFP, Emory RPHC, and Baylor ISR institutions. No refutations, no fabricated affiliations. Added as 8 `mm-org` records.
- **Gap 2 (funder figures) CLOSED.** The TWCF planning-grant ceiling (about $100,000, the LLPW RFP) is verified on the funder's page; NIMHD's 675 social-determinants projects is verified against a peer-reviewed NIMHD-authored paper (Ogletree et al. 2024, AJPM). The Templeton "$450,000 to $730,000 average grant" is **refuted**: no Templeton primary page states it, and authoritative reporting puts the median near $202K to $217K and the mean near $311K. `knowledge-map/03-funders.md` line 24 should drop the $450K-$730K range and cite the median and mean instead.
- **Gap 3 (literature queue) DOWNGRADED, 5 of 6 verified.** Li et al. 2016 (JAMA Internal Medicine), Powell et al. 2003 (American Psychologist), Norris and Inglehart 2004 (Sacred and Secular), Puga-Gonzalez et al. 2025 (PLOS ONE agent-based model), and the Whitehouse et al. 2021 retraction are all verified with DOIs and added. The sixth, "Cohen et al. 2016," could not be uniquely identified and stays an open stub for a human to disambiguate.
- **Gap 4 (Chen 2020) CLOSED.** The general HR 0.32 is corrected to the sex-specific pair from the primary source (JAMA Psychiatry 2020;77(7):737-745): women HR 0.32 (95% CI 0.16-0.62), men HR 0.67 (95% CI 0.48-0.94), cohorts 66,492 women plus 43,141 men. The 0.32 was the women-only figure.

Still pending a human: the unidentifiable "Cohen 2016" reference, the `03-funders.md` Templeton line edit, the TWCF roughly $40M Grand Challenges figure (not re-verified this pass), and the Norris and Inglehart edition (2004 first versus 2011 second). The master `sources.json` records for all of the above are computed and staged (the institute's stack-data repo had active uncommitted work from another session, so the master update was not force-committed there; it applies cleanly to origin/main as an add).

## Status legend

- **verified-bibliography**: published open, fact-checkable bibliography (this folder).
- **record-verified-master**: every source confirmed (author/title/year/DOI) in the master `sources.json`. A weaker guarantee than a fresh claim-level fact-check.
- **data-manifest**: official public datasets, each resolving to the correct named source.
- **register-labeled**: claims tagged by register (science / tradition / metaphysics); only the science is verified, the rest deliberately labeled, not graded.
- **unsourced**: not yet audited and not in any bibliography.
- **code-or-experiment**: build artifacts, no claim-bearing prose.

## Per-surface coverage

| Surface | Status | Note |
|---|---|---|
| `stack-data/institutes/material-and-meaning/third-information-lab/ (thesis corpus` | record-verified-master | 158 records, all already verified into master sources.json per the standing audit. This is the TIL thesis corpus. Two-voice firewall holds: empirical assertions are bound to verifi |
| `stack-data/institutes/material-and-meaning/ institute literature (carried in kno` | record-verified-master | 91 institute-literature records, all already verified into master sources.json. Accounted for; not re-verified this pass. |
| `material-and-meaning/third-information-lab/bibliography/ (position-counterpoint:` | verified-bibliography | The position paper, already PUBLISHED as an open fact-checkable bibliography. 31 records, 30 verified, 1 self-reported resume line correctly labeled. This is the model the rest of  |
| `stack-data/institutes/material-and-meaning/papers/pilot-01-rent-ecology-despair/` | data-manifest | All 11+ data sources resolve to correct official public datasets at the exact identity named (CDC WONDER MCD, ACS B25070 + covariate tables, ARDA RCMSCY10, Vera, BLS QCEW, NCHS Urb |
| `stack-data/institutes/material-and-meaning/papers/gap3-belief-estimation/ (SPEC,` | data-manifest | All sources resolve correctly (Pew RLS 2014, GSS cumulative, ACS PUMS, MCDC Geocorr, MRP method literature). MRP described accurately with honest limits. Smoke test ran on syntheti |
| `stack-data/institutes/material-and-meaning/papers/*/pipeline/ (README, RUNBOOK, ` | code-or-experiment | Build/run scaffolding and a Python virtualenv. The .venv LICENSE.md files (idna, numpy, scipy) are third-party package licenses, NOT institute claims; ignore for bibliography purpo |
| `stack-data/institutes/material-and-meaning/fundraising/ (templeton-funding-inqui` | record-verified-master | Outward-facing funder facts verified against live sources: Templeton July 15 2026 OFI / Dec 4 2026 full proposal, $150k/18mo ask (internally consistent, inquiry-stage), NIMHD 2023  |
| `stack-data/institutes/material-and-meaning/knowledge-map/ (01-literature, 03-fun` | register-labeled | Adversarial internal landscape analysis carrying its own per-claim confidence ratings. Anchor/omission claims verified (Seto, Whitehouse retraction, Healthy People 2030 five-domain |
| `stack-data/institutes/material-and-meaning/org/ + org/dossiers/ (C-SUITE, brand-` | unsourced | NOT audited this pass and NOT in the verified bibliography. The dossiers (funder-deadline-verification-2026-06-15, collaborator-01..05) are the institute's OWN internal source mate |
| `stack-data/institutes/material-and-meaning/engine/ (ARCHITECTURE, README, journa` | code-or-experiment | The research engine: egress/grade/provenance Python plus architecture docs and a study registry. Tooling that enforces the no-fabrication discipline; not itself a claim-bearing sur |
| `stack-data/institutes/material-and-meaning/design/ (DESIGN-PROMPTS, GENERATED-CA` | code-or-experiment | Brand/design prompt material and the static site shell. No empirical claims requiring sources; presentation layer. |
| `material-and-meaning/third-information-lab/methodology/embodied-ai/ (README, PRO` | register-labeled | 6 embodied-AI notes audited. The notes self-tag three registers cleanly: ESTABLISHED SCIENCE (fascia/Schleip, ENS/Gershon, holobiont, torus physics, AI-governance frameworks) all v |
| `material-and-meaning/third-information-lab/embodied-service/ (worker, ui, verify` | code-or-experiment | Build artifact for the embodied register (the constructive lane). Code, not a claim-bearing prose surface. |

## Register-labeled (NOT verified, by design)

These are foundation-voice or contemplative-tradition claims, labeled rather than fact-checked, per the lab's two-voice firewall. Nothing here is presented as established fact.

- Note 01 (embodied-ai): Anatomy Trains myofascial-meridian map (Myers) + fascial-line-vector AI idea -- contemplative-tradition / structural-bodywork lineage, tagged correctly, not verified.
- Note 02 (embodied-ai): seven chakras + endocrine correspondences; nadis (the 64,000 count flagged against 72,000/350,000 variants); five prana vayus; 107 Sushruta marma points; 600 BCE traditional dating -- contemplative-tradition, labeled-not-verified.
- Note 02 (embodied-ai): subtle-body systems reimagined as nested AI coordinate layers -- personal-metaphysics, self-flagged as invention.
- Note 03 (embodied-ai): a ganglia-layer AI inferring autonomic state from text -- personal-metaphysics, self-flagged speculation.
- Note 04 (embodied-ai): design hypotheses (medium as message, viability-stake, holobiont architecture) -- personal-metaphysics, self-flagged speculation.
- Note 05 (embodied-ai) ISAAC FRAME: involution/evolution as one source-consciousness moving through the torus; the torus as the single geometry unifying the three body maps -- personal cosmology / foundation voice, never to be graded as science.
- Note 05 (embodied-ai): body toroidal-field claims + HeartMath coherence claims (HeartMath flagged contested); involution/evolution lineage (Plotinus, Blavatsky, Aurobindo, Wilber) -- esoteric/philosophical tradition, real field-fact separated from contested coherence claims.
- M&M fundraising/foundation voice: meaning-making and material conditions as a coupled dynamical system, meaning as a determinant of survival, read through cultural-evolution/game-theory models of religion as cooperation -- personal-metaphysics / institute theoretical lens framed as hypothesis-to-test, correctly passed through the two-voice firewall.

## Open gaps (honestly named)

- org/ and org/dossiers/ (16 files: C-SUITE, brand-architecture, the CFO/CLO/COO/CSO briefings, collaborator-01..05, institutions, and the funder-deadline-verification-2026-06-15 dossier) were NOT audited and are NOT in the verified bibliography. These dossiers are the institute's OWN source material that several outward-facing figures rest on.
- Three Templeton/NIMHD figures remain UNVERIFIABLE because official pages return HTTP 403 to automated fetchers and they rest on the un-opened internal dossier: Templeton ~$450k-$730k average grant and the $234,800 renewal/follow-up ceiling, and NIMHD's '675 social-determinants projects' / '977 terminated awards (~$1.7B)' / FY2027-elimination counts. Re-verify against the live application page and NIH RePORTER / primary budget documents before any figure goes external. NOT a blocker for the July 15 deadline, which is independently confirmed.
- knowledge-map residual verification queue, labeled-not-verified and NOT yet in master: Li/Stampfer/Williams/VanderWeele 2016 (JAMA Intern Med, ~33% mortality reduction), Powell/Shahabi/Thoresen 2003 (Am Psychol, ~25%), Cohen/Bavishi/Rozanski 2016 (Psychosom Med meta-analysis, RR ~0.83), Norris-Inglehart existential-security + Hollinger-Muckenhuber 2019 (Int Sociology 34(1):19-37), and the 2025 PLOS ONE existential-security agent-based model (DOI 10.1371/journal.pone.0327674). The last two are grader-facing (Templeton abstract + Gaps 2/7) and should be confirmed before submission; PLOS ONE is open-access, a cheap check.
- Chen 2020 carries a live NUANCE, not a gap: the HR ~0.32 presented generally is the women-only estimate (men ~0.67). Separate the sex-specific HRs or label 0.32 as the women's estimate before it enters any proposal or paper.
- Two staleness items to update (harmless to current windows): Vera jail series now runs past 2018 to 2026 v3.1 (DATA-SOURCES sec 4); and Giles-Hungerman-Oostrom has since published (Nov 2025) and now instantiates the institute's own thesis -- promote it from a reserved future-design footnote to an engaged anchor/competitor.
- pilot-01 paper.md and gap3 results carry NO computed estimates -- every value is a marked placeholder because network egress to api.census.gov / wonder.cdc.gov / thearda.com was blocked in the build session. This is correct discipline, not a defect, but the pilots have not been run end-to-end, so the empirical findings themselves remain un-generated (and therefore trivially un-verified).

## New verified records this pass

31 records added to the master bibliography and exported here as `material-and-meaning-sources.csl.json` and `.bib`. Covers the two empirical pilots' data sources, the funder facts, and the embodied-AI science claims.

