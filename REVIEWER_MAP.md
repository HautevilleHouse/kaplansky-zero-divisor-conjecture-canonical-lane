# Reviewer Map

    ## Claim Scope

    - Canonical-lane claim: inside the `manifold_constrained` lane, if the theorem chain in this repository holds and the guard certificate passes, the repository-level closure claim is satisfied.
    - Standard target claim: carried by the in-repo bridge theorems tying the lane to the target statement.

    ## Theorem Dependency Chain

    1. `EG1`: coercive response and active control floor.
    2. `EG2`: capture and admissible continuation.
    3. `EG3`: compactness and no-collapse spacing.
    4. `EG4`: rigidity and transfer.
    5. Identification bridge: strict coherence on the determining class.
    6. Scalar closure: `KZD_G1, KZD_G2, KZD_G3, KZD_G4, KZD_G5, KZD_G6, KZD_GM` all `PASS`.

    Primary files:

    - `paper/KAPLANSKY_ZERO_DIVISOR_CONJECTURE_PREPRINT.md`
    - `notes/EG1_public.md`
    - `notes/EG2_public.md`
    - `notes/EG3_public.md`
    - `notes/EG4_public.md`
    - `notes/IDENTIFICATION_BRIDGE.md`

    ## Closure Gates

    | Gate | Constant | Description |
    |------|----------|-------------|
    | `KZD_G1` | `kappa_support` | projected support response has a strict positive floor |
| `KZD_G2` | `sigma_cancellation` | cancellation defect stays above capture floor across support and restart losses |
| `KZD_G3` | `kappa_compact` | normalized near-failure families are precompact and support windows do not collapse |
| `KZD_G4` | `rho_rigidity` | bad zero-divisor countermodels are excluded |
| `KZD_G5` | `domain_transfer` | rigid limit transfers to the integral-domain endpoint class |
| `KZD_G6` | `eps_coh` | strict coherence / identification closure |
| `KZD_GM` | derived | final strict margin |

    ## Falsification Conditions

    - `repro/certificate_runtime.json` has any non-`PASS` gate.
    - `lane.active_lane != "manifold_constrained"`.
    - `all_pass != true`.
    - Any manifest hash mismatch under `repro/repro_manifest.json`.
    - A verified counterexample to any EG theorem statement used in the paper.
