# EG4 Public Note (Rigidity and Endpoint Transfer)

Mature wording: `bad-limit exclusion / endpoint transfer`.

In-paper anchor: `paper/KAPLANSKY_ZERO_DIVISOR_CONJECTURE_PREPRINT.md` (`KZD_G4`, `KZD_G5`).

## Goal
Separate the rigidity job from the endpoint-transfer job for `proving zero-divisor exclusion for torsion-free group rings through an admissible support-persistence closure architecture`.
The older wording `rigidity and endpoint-transfer` corresponds to bad-limit exclusion plus the bridge into the intended endpoint object.

## Objects

- bad-limit class: candidates extracted by the compactness gate but incompatible with closure.
- rigidity floor: `rho_rigidity`.
- endpoint-transfer lock: `domain_transfer`.
- coherence interface: `eps_coh` remains available to the bridge and final margin.

## Closure Criterion

`KZD_G4` closes when `rho_rigidity` excludes bad endpoint alternatives: bad zero-divisor countermodels are excluded.
`KZD_G5` closes when `domain_transfer` transfers the surviving endpoint to the intended target class: rigid limit transfers to the integral-domain endpoint class.
Together they feed the strict margin `M_KZD`.

## Lemma Chain and Proof Payload

### Lemma EG4.1 (bad-limit exclusion)
Every extracted bad limit contradicts a declared rigidity constraint or leaves the admissible class.

Payload: check `rho_rigidity` in the registry and certificate surfaces.

### Lemma EG4.2 (endpoint transfer)
The surviving rigid representative is locked to the standard problem-side endpoint by `domain_transfer`.

Payload: read this note together with `notes/IDENTIFICATION_BRIDGE.md`.

### Theorem EG4.3 (rigidity/transfer gate closure)
If bad limits are excluded and the endpoint lock is active, then `KZD_G4` and `KZD_G5` deliver the boundary object needed by the final margin.

## Current Instantiation

- rigidity gate: `KZD_G4`
- rigidity artifact key: `rho_rigidity`
- transfer gate: `KZD_G5`
- transfer artifact key: `domain_transfer`
- mature equivalent: `bad-limit exclusion / endpoint identification`
- audit surface: `notes/IDENTIFICATION_BRIDGE.md` and `repro/certificate_runtime.json`
