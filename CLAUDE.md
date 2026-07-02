# CLAUDE.md

## What this repo is
Two public surfaces in one repo: the Material and Meaning public health research institute's static site (root `index.html`, GitHub Pages), and the Third Information Lab's constructive build under `third-information-lab/` (the embodied-AI somatic-map methodology, its governance and eval runs, and the Cloudflare Worker reflection service). The full map is `docs/PRODUCT.md`.

## The one guardrail
Phase A privacy: reflections, scoresheets, keys, and generated outputs are vault-private and gitignored. Isaac's real Lived Record entries never land in this repo. Check `.gitignore` before adding anything under `third-information-lab/methodology/embodied-ai/`.

## Session rules
- Site copy makes empirical claims (published papers, open data). Before touching section 03 or 04 of `index.html`, check the claim against what the repo and the bibliography exports actually contain; the current mismatches are listed in `docs/PRODUCT.md` under Known drift.
- `embodied-verify.yml` gates the Worker: verify runs on push and PR touching `embodied-service/`, deploy is workflow_dispatch only. Secrets by name: `CLOUDFLARE_API_TOKEN`, `ANTHROPIC_API_KEY`.
- Bibliography exports regenerate from `../stack-data/data/sources.json`; do not hand-edit the `.csl.json` or `.bib` files.

## Routing
- Tier: none, a public institute surface outside the personal stack. The spine is stack-data, Tier 1, the operational source of truth, a sibling clone (`../stack-data`).
- No phase-zero kit is deployed here; install from `../rubinstein-productions-toolkit/phase-zero/install.sh` if wanted.
- Route research, citation, and lineage tasks to stack-data and its `research-bibliographer` agent; the non-fabrication discipline (a named gap beats a fabricated link) is the institute's own standard.
