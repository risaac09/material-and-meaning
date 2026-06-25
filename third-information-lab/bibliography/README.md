# Open verified bibliography

This is the Third Information Lab's open bibliography. Every empirical claim the lab ships in public writing is verified against a primary or authoritative source, graded, and published here in formats a human or another agent can fact-check and reuse.

The practice is a standing rule, not a one-time export. Lanier's data-dignity principle, that information should carry its provenance, applied to our own claims. If we make a claim, the source and its verification status are public, and you can check our work.

## What is here

- `BIBLIOGRAPHY.md`, the human-readable and agent-readable record: every claim, the figure as the source actually states it, the verdict, and a URL or DOI. Start here to fact-check.
- `position-counterpoint.csl.json`, the machine-readable bibliography in CSL-JSON, so it imports into Zotero, pandoc, or any citation tool.
- `position-counterpoint.bib`, the same records as BibTeX.
- `material-and-meaning-sources.csl.json` and `.bib`, the institute-tree dataset: the empirical pilots' data sources (CDC WONDER, Census ACS, US Religion Census, and the rest), the funder facts (Templeton, NIMHD, Players Philanthropy Fund, Russell Sage, Fetzer, Mind and Life), and the embodied-AI science claims (fascia, the enteric nervous system, the physics of the torus). 31 records, verified the same way.
- `tree-coverage-ledger.md`, the honest answer to "is the whole Material and Meaning tree in a verified bibliography." A per-subfolder map of what is verified, what is record-verified, what is register-labeled, and what is still an open gap.

Two datasets so far. `position-counterpoint` covers the public-health-AI position paper. `material-and-meaning-sources` covers the institute tree audited 2026-06-25. The coverage ledger ties them together and names what is not yet covered. More datasets are added as the lab publishes.

## Tree-wide coverage, stated honestly

The whole institute tree is not yet a single fully-verified bibliography, and the ledger says so plainly. The claim-bearing prose surfaces resolve to real sources with no fabricated citations found: the thesis corpus (158 records), the institute literature (91), the position paper (31), and now the empirical pilots, funder facts, and embodied science (31). What is not verified, and is labeled as such: the internal org and dossiers layer (un-audited), a few funder figures behind fetch-blocked official pages, a residual literature queue, and the embodied-AI esoterica, which is register-labeled (tradition and metaphysics) rather than graded as fact, by the lab's two-voice firewall. Nothing un-verified is presented as established.

## The verdict legend

- **verified**, the source states the claim and the figure matches.
- **partially-verified**, the core is right but a detail (a number, a date, an attribution, a metric) needs the qualification given in the note.
- **projection-or-forecast**, the claim is a forecast or a target, not a realized fact, and is attributed to whoever made it.
- **refuted**, the source contradicts the claim. (None in the current dataset.)
- **unverifiable**, no adequate source was found. (None in the current dataset.)

## How it was verified

Claims were checked by independent agents doing web search against primary sources (peer-reviewed papers, official filings, the company or agency itself), then a second adversarial pass re-checked the volatile financial and forecast claims. The discipline: report the figure as the source actually states it even when it differs from the claim, distinguish a fact from a forecast, and mark every gap rather than paper over it. Several figures in the draft were corrected this way, recorded in `BIBLIOGRAPHY.md` under "Corrections applied."

## How to fact-check or reuse this

- Read `BIBLIOGRAPHY.md`, follow the URL or DOI, and check the figure against the source. If you find an error, the record names exactly what was claimed and what the source said, so a correction is precise.
- Import `position-counterpoint.csl.json` or `position-counterpoint.bib` into your own tool. Records are tagged with the claim they support and their verification status.
- This bibliography is public so it can be distributed widely and checked by anyone, agent or human. Corrections are welcome.
