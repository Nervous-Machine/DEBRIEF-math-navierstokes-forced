# Asks — The claimed finite-time blow-up of the three-dimensional Navier–Stokes equations with a smooth force, announced by OpenAI on 8 September 2026 with a Lean development

Each open gap below is a place a contribution can land. A contribution is one cycle in this repository's ledger, under your name. How to contribute, and the templates: https://github.com/Nervous-Machine/DEBRIEF/blob/main/CONTRIBUTING.md

## 1. The Lean development has not been built or kernel-checked by anyone outside the claimant (ledger id EG1)

The claimant reports a Lean development that compiles with standard axioms only. Nobody outside the claimant has reported building it.

Status: proposed.

- **a pre-registered rerun: fetch at the pinned commit, build, confirm no sorry or admit, print the axioms** — contribution kind: rerun; who could act: anyone with a machine and a few hours.

Signal expected: a rerun cycle reporting build exit status, the sorry/admit scan and the axiom list for the main theorem. Resolution by: none registered.

## 2. Do the formal statements say what the problem asks? (ledger id EG2)

A Lean check establishes that the formal statement follows from its hypotheses. Whether that formal statement is the problem as posed is a separate question that a person has to answer. A third-party formalization of the problem statement exists, so part of this can be compared by machine.

Status: proposed.

- **a machine comparison of the claimant's main theorem with the third-party formal statement navier_stokes_breakdown_R3 in google-deepmind/formal-conjectures, then a human read of any difference** — contribution kind: trace (a reading guide); who could act: anyone who can read Lean; the two statements are public.
- **two independent mathematicians read the formal statement against the problem as posed and sign, or refuse** — contribution kind: read; who could act: a mathematician in the problem's area, about an hour with a reading guide.

Signal expected: a trace cycle and two signed read cycles, or a refusal naming the difference. Resolution by: none registered.

## 3. No independent mathematician has reported reading the proof, and there is no referee report (ledger id EG3)

The claim was announced on OpenAI's blog and at a press briefing, with the paper on OpenAI's own servers and the Lean development on GitHub. No independent reading, referee report or journal submission is on the public record.

Status: proposed.

- **a read cycle by a mathematician in the area who is not an author, signing or refusing each main step** — contribution kind: read; who could act: a mathematician in the problem's area.
- **a referee report or journal acceptance, recorded by date** — contribution kind: data; who could act: a journal; the record notes the date when it happens.

Signal expected: a signed or refused read cycle; a dated referee report. Resolution by: none registered.

## 4. A preprint reports that the Lean statements and the written proof differ in at least one lemma (ledger id EG4)

Bastounis, Circelli and Hansen report that the Lean estimate standing in for the paper's Lemma 8.6 bounds the inverse with one more derivative than the paper's inequality, and that similar mismatches occur elsewhere, so a clean Lean check does not by itself confirm the written proof. They make no claim that the result fails. Whether the formal development carries the paper's argument, or a different one that reaches the same statement, is a reading.

Status: proposed.

- **an analyst reads Lemma 8.6 and the other mismatches the preprint lists against the Lean files and signs or refuses that each is immaterial to the formal result** — contribution kind: read; who could act: an analyst who reads Lean, a few hours with the preprint's list.

Signal expected: a read cycle listing each mismatch as immaterial, material or unresolved. Resolution by: none registered.
