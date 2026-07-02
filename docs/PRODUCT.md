# material-and-meaning

Public repo carrying two surfaces. The first is the website of Material & Meaning, a public health research institute studying how material conditions (rent, wages, incarceration, psychiatric holds) and meaning-making couple to shape health, aimed at population-health researchers and funders. The second is the constructive-register build of the Third Information Lab, the institute's AI and information division: the embodied-AI somatic-map methodology, a live Cloudflare Worker reflection service, and an open verified bibliography, all under `third-information-lab/`. The repo carries no tier in the estate hierarchy; it is a public institute surface. The spine is stack-data, Tier 1, the operational source of truth, a sibling clone (`../stack-data`). The lab's charter lives at `stack-data/institutes/material-and-meaning/third-information-lab/`, its thesis in the vault.

## What it is (technical)

Two halves that share nothing but the repo.

- **Institute site**: `index.html` plus `style.css`, static, no build step, GitHub Pages from the repository root. Live at https://risaac09.github.io/material-and-meaning/. The root `README.md` covers this half only.
- **Lab build** (`third-information-lab/`): three trees. `methodology/embodied-ai/` holds the essay, governance, testing protocol, probes, prompts v1 through v6, and the run records; start at its README for the read-order map. `embodied-service/` is the estate's one backend with a model call: a static `ui/` and a Worker (`worker/src/`, router, prompt, guards, gate, LLM call) with a deterministic verify harness under `verify/`. Architecture, defense-in-depth layers, and privacy posture: `third-information-lab/embodied-service/README.md`. Config-as-doc for `ALLOWED_ORIGIN`, `DAILY_TOKEN_CAP`, and the Durable Object bindings: `worker/wrangler.toml`. The soma state object and coordinate design: `methodology/embodied-ai/build-sketch.md`. `bibliography/` holds the verified claim datasets (`.csl.json` and `.bib` exports) and the ledger.
- `.gitignore` encodes the Phase A privacy patterns: reflections, scoresheets, keys, and generated outputs never land in this public repo.

Gap: no root-level doc maps the repo's two halves together; the root README lists only `index.html` and `style.css` and never mentions `third-information-lab/`. The fix is a root README extension or a CLAUDE.md, decided by Isaac.

## How it runs (operational)

The site deploys itself: push to `main`, GitHub Pages serves from root. Everything else is inventoried under Workflows below. The operative runbooks already exist and this file points at them instead of restating them.

- Service dev, go-live, and verification: `third-information-lab/embodied-service/README.md`.
- Eval suite, probe freezing, red team, SEL gate checklist: `methodology/embodied-ai/testing-protocol.md`.
- Independent grader steps: `methodology/embodied-ai/frontier-lab/grader-runbook.md`.
- Bibliography verification practice: `third-information-lab/bibliography/README.md`.

Gap: no runbook describes how the bibliography exports (`position-counterpoint` and `material-and-meaning-sources` in `.csl.json` and `.bib`) regenerate from the master sources.json in stack-data; the ledger references staged records there but the round-trip is undocumented. The answer lives with the stack-data export tooling.
Gap: no documented pre-publish check ties site copy claims to the verified bibliography; the index.html drift listed below is the failure this check would have caught. The check would live beside `bibliography/README.md` once Isaac defines it.

## Why it exists (intellectual)

The institute premise, material conditions and meaning-making as coupled health determinants read through complexity theory and game theory, is stated in the root `README.md` and argued in full on `index.html` (the research question, the two poles, pilot 01's design logic). The lab's reason for being, two registers where the diagnostic audits the organism-pole deletion and the constructive builds governed experiments that try to hold it, is `third-information-lab/README.md`. The master essay with premise, wager, five maps, and honest limits is `methodology/embodied-ai/embodied-ai-somatic-map.md`, grounded by six three-register-tagged research notes under `methodology/embodied-ai/research/`. The build narrative is `frontier-lab/the-story.md`; the five learnings from the arc are in `PROPOSAL.md`. This dimension is well covered in-tree; nothing new is needed here.

## How it works (methodological)

The method is documented where it is enforced.

- **Governance**: Council of Four Directions, the Center veto (anything claiming to read, replace, or speak for the Center fails at any exposure level), and the SEL-0 to SEL-3 exposure ladder: `methodology/embodied-ai/governance.md`.
- **Testing**: eval suite with thresholds, frozen probe sets (`probes/`), red-team procedure, Soma Card requirement, gate checklist: `testing-protocol.md`. Twelve run records under `runs/` carry the evidence trail.
- **Model cards**: `SOMA-CARD.md` and `SOMA-CARD-v5.md`, including known failures and refusals.
- **The three-register rule**: established science, tradition, and speculative synthesis stay separated; tradition is never presented as physiology; esoterica is register-labeled, never graded as fact (`methodology/embodied-ai/README.md`, the method rule; `bibliography/tree-coverage-ledger.md`).
- **Non-fabrication bibliography discipline**: every public empirical claim verified against a primary source, adversarial second pass on volatile figures, verdicts and corrections published (`bibliography/README.md`, `BIBLIOGRAPHY.md`). Per-surface coverage lives in `tree-coverage-ledger.md`.
- **Friction log**: one line per catch in `friction-log.md`; a serious overstep triggers a Threshold Review.

Gap: the site's pilot 01 section describes a pre-registered design whose actual design, pre-registration, and data manifest live in private stack-data (`papers/pilot-01-rent-ecology-despair/`, per the coverage ledger); this public repo holds no public methods artifact backing the study claims the site makes. Publishing one is Isaac's call.

## How it speaks (marketing and comms)

`index.html` is the sole institute comms surface. Positioning: measure meaning the way housing gets measured; stance: we measure, we do not preach. Audience (section 04): population-health, sociology-of-religion, and economics-of-religion researchers and funders. Funnel (section 05): mailto isaac@isaacrubinstein.com. The grader-seat outreach material is `methodology/embodied-ai/frontier-lab/grader-invitation.md` and `deck.md`.

The estate voice rules govern all public copy here: no em-dashes, no rule-of-three, no throat-clearing openers, no false agency, no vague declaratives, no adverb stacking, no business jargon, no binary contrasts, varied sentence length.

Gap: those voice rules are written down only in sibling repos' CLAUDE.md files (rubinsteinproductions, saywhy-app); this repo enforces them in practice (commit 6214501 dropped em-dashes from a README) but carries no copy of them. A CLAUDE.md here would close it.

## Where it goes (strategic)

Status, from `third-information-lab/README.md`: SEL-1, experimental, gate not cleared. Deployed prompt is v4. v5 is the lead candidate (efficacy wager 11-0-1, red team 0 blocking, formal hard gates clear, Soma Card written) and still owes the human Phase A run, the live-only probes (II-1, AD-6, AD-7), and the four-seat sign-off. The approved Phase A/B plan and the honest statement of where the work stands are `methodology/embodied-ai/PROPOSAL.md`. Open gaps per surface, including pending-human items, are named in `bibliography/tree-coverage-ledger.md`. The work moved here from the alchemy repo on 2026-06-22; git history through that date stays in alchemy's log. Material & Meaning is a working name; the fiscal sponsor, Players Philanthropy Fund, is pending (root `README.md`).

Gap: this repo has no CLAUDE.md, no tier or routing statement, and is absent from the toolkit's list of ten phase-zero consuming repos; whether to deploy the phase-zero kit here is an open decision for Isaac.

## Workflows

Automated:

- **`embodied-verify.yml`, verify job**: on push or PR touching `third-information-lab/embodied-service/**` or the workflow file. Syntax-checks `worker/src/*.js` and runs `verify/verify.mjs`, the deterministic safety floor (crisis detection, input validation, soma allowlist). No secrets required.
- **`embodied-verify.yml`, deploy job**: `workflow_dispatch` only, needs the verify job green, runs `wrangler deploy` on the Worker. Skips cleanly when the `CLOUDFLARE_API_TOKEN` secret is unset. The gate ordering means the safety floor cannot be bypassed on the way to a deploy.
- **GitHub Pages**: serves the site from the repository root on push to `main`. Pages default, no Actions workflow.

Manual:

- **Local dev**: `cd third-information-lab/embodied-service/worker && npm install && npm run dev`. Mock mode, no key needed. Good looks like the UI answering against the mock.
- **Go live**: set `ALLOWED_ORIGIN` first, then `wrangler secret put ANTHROPIC_API_KEY`, then `npm run deploy` (secret named, never written down).
- **Safety verification**: `node verify/verify.mjs`, same harness CI runs. Good looks like every deterministic check passing.
- **Wager test**: `node verify/wager.mjs [reflections.txt]`, blind-labels embodied-vs-flat pairs, writes a scoresheet plus key. Placeholder inputs must be replaced with real entries for the run to count.
- **Live probes for SEL-1 sign-off**: `EMBODIED_BASE_URL=... node verify/live-probes.mjs`, records II-1 and AD-6 for the grader; AD-7 runs directly against the API.
- **Phase A wager**: `node verify/wager-phase-a.mjs` with prompt-v5.js, v5 versus flat on real entries, human-graded. Outputs are vault-private and gitignored; the guide lives in the vault under 15 Third Information Lab/phase-a/.
- **Grader ritual**: the independent grader follows `frontier-lab/grader-runbook.md`, runs the wager plus live probes, and scores blind. Seat status is tracked in `worker/src/gate.js`.
- **Friction log**: one line per catch in `methodology/embodied-ai/friction-log.md`, at the moment of the catch. A serious overstep triggers a Threshold Review.
- **Bibliography verification**: as the lab publishes, independent agents web-search every public empirical claim against primary sources, run a second adversarial pass on volatile figures, and record corrections in `BIBLIOGRAPHY.md`. Standing rule per `bibliography/README.md`.

## Known drift

Listed for Isaac to rule on. Nothing here has been changed by this doc.

1. `index.html` sections 03 and 04 claim, in the present tense, published papers, code, and cleaned data ("The paper is the artifact", "We publish the code and the cleaned data"). No paper, code, or cleaned data is published in this repo, and `tree-coverage-ledger.md` states the pilot-01 paper and gap3 results carry no computed estimates and the pilots have not run end to end. The registry note is confirmed.
2. `index.html` section 03 status line says "Pre-registered and scoped." The design and manifest exist in private stack-data, but no public registration artifact or link exists; a reader cannot verify the claim.
3. `methodology/embodied-ai/frontier-lab/README.md` points the grader at the risaac09/alchemy repo on branch claude/embodied-ai-somatic-map-vfet1g. The work moved to this repo on 2026-06-22. The onboarding doc for the one external collaborator names the wrong repo.
4. `SOMA-CARD.md` frontmatter says SEL-0 while its own body and the service README say SEL-1, experimental, gate not cleared. governance.md requires the card be updated at every level change.
5. `SOMA-CARD.md` describes the system as an embodied companion inside Alchemy reading scores Alchemy collects; the deployed surface is the isolated embodied-service UI, and `third-information-lab/README.md` calls Alchemy a separate consumer tool, not its home.
6. `embodied-service/README.md` contradicts itself on rate limiting: the defense-in-depth section describes a best-effort in-isolate per-IP limit, while the Phase A status section and `wrangler.toml` confirm the Durable Object RateLimiter replaced it. The architecture tree also omits `worker/src/limits.js`, where RateLimiter and SpendCounter live.
7. Root `README.md` lists only `index.html` and `style.css` under Files, omitting the entire `third-information-lab/` tree.
8. `tree-coverage-ledger.md` calls the position paper "already PUBLISHED as an open fact-checkable bibliography"; the bibliography is published here, but the paper itself appears nowhere in this repo and no link says where it lives.
