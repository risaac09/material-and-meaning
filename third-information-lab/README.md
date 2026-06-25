# The Third Information Lab

The AI and information division of Material & Meaning. Where the institute's empirical engine studies the material-and-meaning coupling in the world, the lab studies that coupling as it is mediated, datafied, and extracted by information systems. It runs two registers.

- **Diagnostic register.** Audit the collapse that datafied systems perform on a relational affordance, the deletion of the organism-pole. The keystone proof and the corpus live in the vault.
- **Constructive register.** Build small, governed experiments that try to hold the organism-pole instead of deleting it, and run the wager honestly. This directory is that register's build.

## What is here

- `methodology/embodied-ai/`: the embodied-AI somatic-map methodology. The master essay and research notes, the SEL governance, the testing protocol, the frozen probe sets, the system prompt hardened across versions (v1 through v6), the eval and red-team runs, and the Soma Cards. Start at `methodology/embodied-ai/README.md`.
- `embodied-service/`: the live service. A Cloudflare Worker and a static UI that run the embodied prompt as a reflection tool, with the crisis boundary enforced in code. SEL-1, experimental. Isolated from any consumer app: this is the one place with a backend and a model call.

## The other layers

This repo holds the build. The lab's other layers live where they belong:

- **Charter** (decisions, fit with the institute's C-suite): `stack-data/institutes/material-and-meaning/third-information-lab/README.md`.
- **Research and thinking** (the thesis, the keystone, the convergence map, the lab architecture): the Obsidian vault, `Second Brain/02 Research/15 Synthesis/15 Third Information Lab/`.

## Status

SEL-1, experimental, gate not cleared. The deployed prompt is v4. v5 is the lead candidate (efficacy wager 11-0-1, red team 0 blocking, formal hard gates clear, Soma Card written), still owed the human Phase A run, the live-only probes, and the four-seat sign-off. The deterministic safety floor is verified in CI (`.github/workflows/embodied-verify.yml`).

Moved here from the `alchemy` repo on 2026-06-22, where it was first built. Alchemy is a separate consumer tool, an exhibit of the constructive register, not its home. The full git history of this work through 2026-06-22 is in the alchemy repo's log.
