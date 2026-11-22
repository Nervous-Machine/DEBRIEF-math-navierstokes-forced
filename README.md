# DEBRIEF-math-navierstokes-forced

A DEBRIEF mission record (protocol https://github.com/Nervous-Machine/DEBRIEF) for **The claimed finite-time blow-up of the three-dimensional Navier–Stokes equations with a smooth force, announced by OpenAI on 8 September 2026 with a Lean development**.

<!-- standing:begin -->
**Standing, 22 Nov 2026.** Stage: Registered. Needs next: The Lean development has not been built or kernel-checked by anyone outside the claimant ([what would close it](ASKS.md)).

| certified | accepted | refuted | open gaps | cycles filed | last cycle |
|---|---|---|---|---|---|
| 0 | 0 | 0 | 4 | 0 | 22 Nov 2026 |

| | |
|---|---|
| checked by machine | nobody yet; reported elsewhere, not filed here: [Deep Bhattacharjee (Zenodo 10.5281/zenodo.23286556)](https://zenodo.org/records/23286556) |
| read by a person | nobody yet; no reading guide yet |
| elsewhere | [Clay Mathematics Institute](https://www.claymath.org/millennium/navier-stokes-equation/): Active · [DeepMind formal-conjectures, NavierStokes.lean](https://raw.githubusercontent.com/google-deepmind/formal-conjectures/main/FormalConjectures/Millennium/NavierStokes.lean): research solved |
| related | [Navier–Stokes blow-up, unforced (Alpöge and Buckmaster)](https://github.com/Nervous-Machine/DEBRIEF-math-navierstokes): the forced case; the force is what the other claim removes; same problem page · same claimant: [Prime gaps ≤ 186 (OpenAI)](https://github.com/Nervous-Machine/DEBRIEF-math-primegaps) |
| tooling | GPT-6 Astra, OpenAI Codex (agent) · tier: internal · "developed over the weekend" before the announcement, per OpenAI's press briefing as reported (stated in the repository's formalization.yaml: GPT-6 Astra agents in the Codex framework; the claimant is the model's maker) |

Rendered from `ledger/` at regeneration; the full record is `SCORECARD.md`, what is owed is `ASKS.md`. Standing words: nothing has standing yet.
<!-- standing:end -->

This claim is on the public claims board, https://math-board.nervousmachine.com, which shows its stage, who has contributed, and what it needs next.

## The problem

Do smooth solutions of the three-dimensional incompressible Navier–Stokes equations, started from smooth data, stay smooth for all time, or can the velocity become unbounded in finite time? Fefferman's formulation accepts either answer: a proof of existence and smoothness, with no force on space (A) or on the torus (B), or a proof of breakdown, which may use a smooth force, on space (C) or on the torus (D). This claim is (C) and (D) with a force. A third-party Lean formalization of all four alternatives exists in DeepMind's formal-conjectures, and the development's Comparator files take their reference statements from it.

Source: https://www.claymath.org/millennium/navier-stokes-equation/ (posed: one of the seven Clay Millennium Prize Problems (2000), formulated by Charles Fefferman as four alternatives: existence and smoothness on space (A) and on the torus (B), or breakdown on space (C) and on the torus (D)).

A third-party formalization of the problem statement exists: `FormalConjectures/Millennium/NavierStokes.lean` in github.com/google-deepmind/formal-conjectures at commit `2207c54d0dbe960de591d280f997b195bf3f6e28` (blob `c21ccbfb73a85a930970d3b93ad23bd4c97d082a`). It is the natural reference for whether a claimant's Lean theorem states this problem.

## The claim

**OpenAI**, using GPT-6 Astra agents in the Codex framework, as listed in the repository's formalization.yaml; the paper's author line reads OpenAI, submitted 2026-09-08 at https://openai.com/index/navier-stokes-solution/.

The paper's main result says that for every positive viscosity there are a smooth force with compact support in space and time, a compact set, and smooth velocity and pressure fields on space, starting from zero velocity, supported in that set, with bounded kinetic energy, whose velocity becomes unbounded as time approaches one; and so no smooth solution with that force and datum exists for all time with bounded energy. Compact support carries the construction to the torus. The paper names these as alternatives (C) and (D) of Fefferman's formulation. A companion paper claims unforced blow-up for the Euler equations. The repository's metadata file records four main results with zero sorry and the three standard axioms, lists GPT-6 Astra in the Codex framework as the method, and records the review status as self-assessed. The press reported experts who regard the force as a loophole in the problem's wording and others who called the result a surprise if it holds. Buckmaster's statement of 7 September alleges that OpenAI adopted his and Alpöge's method after learning of their progress, which OpenAI denies; the statement says the pair's own forced results were checked in Lean on 22 August.

Artifacts, pinned:

- a PDF write-up: https://cdn.openai.com/pdf/32d9f210-8b73-45e0-91bc-82a30aef8a9a/navier-stokes.pdf (sha256 0e779481c4da40bd28d1e642e1d8ca57447d129610df28dfa5a11e9af8ae228f, 2959204 bytes, fetched 2026-11-22)
- a public repository: github.com/openai/NavierStokesAndEuler at commit f9e8bc5b38b6e212696e8a30e3e91517af887bbd (2026-09-10); licence Apache-2.0; 816 Lean files; has a lakefile

Status on the problem page as of 2026-11-22: announced on OpenAI's blog with the paper on OpenAI's servers; no preprint server, no journal, no referee report; the Clay page lists the problem as Active.

## What is owed

Each open gap is in `ASKS.md` with what closes it and who could act. In order:

1. **The Lean development has not been built or kernel-checked by anyone outside the claimant** (EG1): A rerun of the Lean build on an independent machine, written down first.
2. **Do the formal statements say what the problem asks?** (EG2): A reading of the formal statement against the problem as posed, by someone who did not write it.
3. **No independent mathematician has reported reading the proof, and there is no referee report** (EG3): Someone in the field reads it and says, under their name, what holds and what does not.
4. **A preprint reports that the Lean statements and the written proof differ in at least one lemma** (EG4): A reading of the preprint's listed mismatches against the Lean development, signed or refused one by one.

## Contributing

- **Rerun** (if there is a Lean development): copy `prereg_rerun.yaml`, fill in your predictions, register it with `tools/prereg.py register` from the protocol repository and commit it *before* running anything. Run. Report with the **Rerun report** issue form; it becomes a `rerun` cycle under your name.
- **Read**: a trace (reading guide) does not exist yet. Writing one is itself a `trace` cycle. Once it exists, the **Semantic read** form takes signatures and refusals.
- **Anything else**: open a plain issue.

Rules and templates: https://github.com/Nervous-Machine/DEBRIEF/blob/main/CONTRIBUTING.md. Every contribution is one dated cycle under your own name and goes into `CITATION.cff` and the next release.

## Layout

```
ledger/navierstokes-forced.json   the ledger (protocol 0.1.0)
claim.yaml            the pinned claim this record was opened from
SCORECARD.md / ASKS.md  generated from the ledger
prereg_rerun.yaml     a pre-registration template for the first rerun (unregistered)
cycles/               contributed cycles, one file each
```

## Words

This record never calls the claim proved, verified or a theorem. It records what was claimed, what was checked by whom under what rule, and what is still open. Nothing here has standing until a cycle gives it one.
