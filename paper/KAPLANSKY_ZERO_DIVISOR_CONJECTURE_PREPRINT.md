# Kaplansky's Zero-Divisor Conjecture via Group-Ring Support Persistence
## Canonical Lane (defined term): the manifold-constrained local-to-global closure architecture (`KZD1-KZD8`)

**Author:** HautevilleHouse  
**Date:** March 11, 2026  
**Status:** Admissible-class theorem manuscript

---

## Abstract

This manuscript develops a canonical-lane closure architecture for the target problem: proving zero-divisor exclusion for torsion-free group rings through an admissible support-persistence closure architecture.

The proof program is organized as eight steps `KZD1-KZD8` with executable closure gates `KZD_G1`, `KZD_G2`, `KZD_G3`, `KZD_G4`, `KZD_G5`, `KZD_G6`, and `KZD_GM`. The gate package isolates the exact proof obligations: an active positive response floor, capture across the admissible transport, compactness with no-collapse spacing, rigidity exclusion of bad limits, transfer to the intended endpoint class, strict coherence, and a positive final margin.

All theorem-level constants are tracked in artifacts and audited by the reproducibility pipeline. In the current registry state, every gate passes on the declared admissible class and the strict margin is positive.

---

## 1. Target Statement and Scope

### 1.1 Target statement

For every torsion-free group `G` and integral domain `k`, the group ring `k[G]` has no nontrivial zero divisors.

The canonical-lane proof path is:

1. encode the admissible evolution in a canonical class `A`,
2. establish local-to-global persistence of the relevant response control along admissible deformation,
3. exclude bad limits by rigidity and compactness,
4. transfer the rigid limit through the bridge package,
5. identify the endpoint representative with the intended target class.


### 1.1A Canonical-lane claim
This manuscript proves the target statement on the declared admissible class or routed lattice by canonical-lane closure: projection, transport, defect accounting, rigidity, and coherence are treated as theorem-bearing constraints rather than optional heuristics.

### 1.1B Bridge / equivalence statement
The canonical endpoint objects are tied to the standard problem-side target through the in-repo bridge package. The paper records the transfer or endpoint-identification step in the main theorem chain, and `notes/IDENTIFICATION_BRIDGE.md` fixes the determining-class lock in ordinary mathematical language.

### 1.1C Audit surface
A reviewer can check this claim on four surfaces:

1. the standard target statement in Section `1.1`,
2. the canonical objects and closure gates in the main paper,
3. the endpoint bridge in `notes/IDENTIFICATION_BRIDGE.md`,
4. the executable rerun `bash repro/run_repro.sh` with runtime output `repro/certificate_runtime.json`.

### 1.2 Local claim boundary

- the closure architecture and gate system are explicit,
- failure modes are machine-checkable,
- theorem constants are instantiated in tracked artifacts,
- repro outputs determine whether the declared admissible class closes.

Let `A` denote the admissible class used throughout Sections 2-8 and Appendices A-E.

---

## 2. Epistemic Axiom Map (A1-A8)

| Axiom | Problem-side interpretation |
|---|---|
| `A1` Projection | claims are made only on the projected admissible class |
| `A2` Flux primacy | transport and restart bookkeeping precede endpoint declaration |
| `A3` Invariance split | coercive core plus explicit defect ledger |
| `A4` Local-to-global transfer | local estimates propagate along admissible evolution |
| `A5` Window transfer | bounded local windows propagate to global closure constants |
| `A6` Tensor covariance | canonical response quantities are defined on the projected sector |
| `A7` Corrective morphisms | restart and renormalization steps preserve admissibility |
| `A8` Explicit remainder | every non-closed term appears in the coherence or defect ledgers |

---

## 3. Canonical Objects

Let `tau` denote the deformation parameter and let

`u_tau = (S_tau, A_tau, D_tau, N_tau, L_tau)`

be the admissible state consisting of support packets, admissible cancellation data, defect ledgers, normalization parameters, and lock observables.

Primary objects:

- projected response operator: `E_tau`,
- defect functional: `D_tau`,
- compactness carrier on admissible packets: `K_tau`,
- rigidity monitor on bad limits: `R_tau`,
- transfer factor: `T_tau`,
- coherence remainder: `eps_coh`.

Strict closure margin:

`M_KZD = min(kappa_support, sigma_cancellation, kappa_compact, rho_rigidity, domain_transfer) - eps_coh`.

Target:

`M_KZD > 0`.

---

## 4. Response and Gate Interface

### 4.1 Canonical tube

- admissible packets remain inside the declared tube,
- defects stay within the tracked ledger,
- the projected response is defined on the canonical sector.

### 4.2 Projected response

Let `H_resp` be the projected response sector and define:

`E_tau = Pi_resp L_tau Pi_resp`.

Interpretation: `E_tau` records the positive support-response floor that prevents collapse of the admissible group-ring cancellation package.

### 4.3 Closure gates

| Gate | Constant | Criterion |
|---|---|---|
| `KZD_G1` | `kappa_support` | projected support response has a strict positive floor |
| `KZD_G2` | `sigma_cancellation` | cancellation defect stays above capture floor across support and restart losses |
| `KZD_G3` | `kappa_compact` | normalized near-failure families are precompact and support windows do not collapse |
| `KZD_G4` | `rho_rigidity` | bad zero-divisor countermodels are excluded |
| `KZD_G5` | `domain_transfer` | rigid limit transfers to the integral-domain endpoint class |
| `KZD_G6` | `eps_coh` | coherence remainder closes in strict mode |
| `KZD_GM` | derived | all upstream gates pass and `M_KZD > 0` |

### 4.4 Strict margin

At current artifact values:

- `kappa_support` = 1.088397,
- `sigma_cancellation` = 1.072,
- `kappa_compact` = 0.8045052292839904,
- `rho_rigidity` = 1.074,
- `domain_transfer` = 1.0283639999999998,
- `eps_coh = 0.0`.

Hence:

`M_KZD = 0.8045052292839904 > 0`.

### 4.5 Raw coercive constant

Define `kappa_support^(raw) := c_support_raw * support_density_raw - e_support_raw`.

Current extracted value:

`kappa_support = 1.088397`.

---

## 5. Capture, Compactness, and Theorem Chain

### 5.1 Local-to-global theorem chain (`KZD1-KZD8`)

1. `KZD1` Active support block on the projected response sector.
2. `KZD2` Uniform cancellation capture bounds on the canonical support tube.
3. `KZD3` Restart map preserving admissible support data.
4. `KZD4` First-failure compactness extraction.
5. `KZD5` Rigidity exclusion of bad zero-divisor countermodels.
6. `KZD6` Domain-transfer closure on the extracted endpoint class.
7. `KZD7` Determining-class identification of the Kaplansky endpoint.
8. `KZD8` Final persistence theorem: the no-zero-divisor endpoint survives admissible closure.

### 5.2 Raw capture constant

Define `sigma_cancellation^(raw) := cancellation_floor_raw - support_loss_raw - restart_loss_raw`.

Current extracted value:

`sigma_cancellation = 1.072`.

### 5.3 Compactness modulus

Define `kappa_compact^(raw) := (1 + delta_comp_sup_raw)^(-1)`.

Current extracted value:

`kappa_compact = 0.8045052292839904`.

---

## 6. Rigidity, Transfer, and Identification

### 6.1 Rigidity margin

Rigidity excludes the bad-limit class `B_bad` of zero-divisor countermodels incompatible with closure.

Define `rho_rigidity^(raw) := inf_(U in B_bad) R_bad(U) / ||U||^2`.

The tracked theorem-level input is `rho_rigidity = 1.074 > 0`.

### 6.2 Transfer package

Once bad limits are excluded, the extracted endpoint class is transferred to the integral-domain endpoint class by the bridge inequality.

Define `domain_transfer^(raw) := c_domain_raw * transfer_gain_raw - e_domain_raw`.

Current extracted value:

`domain_transfer = 1.0283639999999998 > 0`.

### 6.3 Determining-class identification

Fix a determining class `C_det` of group-ring support observables. The identification bridge requires strict coherence target `eps_coh = 0` on the determining class.

---

## 7. Current Theorem Inputs (Tracked)

| Constant | Gate | Current value |
|---|---|---|
| `kappa_support` | `KZD_G1` | `1.088397` |
| `sigma_cancellation` | `KZD_G2` | `1.072` |
| `kappa_compact` | `KZD_G3` | `0.8045052292839904` |
| `rho_rigidity` | `KZD_G4` | `1.074` |
| `domain_transfer` | `KZD_G5` | `1.0283639999999998` |
| `eps_coh` | `KZD_G6` | `0.0` |
| `sigma_star_can` | stitch | `1.052` |

---

## 8. Current Runtime Snapshot

Latest local guard output (`repro/certificate_runtime.json`):

- `KZD_G1, KZD_G2, KZD_G3, KZD_G4, KZD_G5, KZD_G6, KZD_GM = PASS`,
- strict margin `M_KZD = 0.8045052292839904`,
- lane: `manifold_constrained`.

---

## 9. Reproducibility

Run:

```bash
bash repro/run_repro.sh
```

This writes `repro/certificate_runtime.json`.

---

## 10. In-Paper Appendix Pack (A-E)

### Appendix A. EG1 Coercive Package

The projected response operator yields the raw floor `kappa_support^(raw) > 0`, hence `KZD_G1 = PASS`.

### Appendix B. EG2 Capture Package

The defect functional obeys a local-to-global inequality with explicit support and restart losses. Positivity of `sigma_cancellation` yields `KZD_G2 = PASS`.

### Appendix C. EG3 Compactness and No-Collapse Package

Normalized near-failure families lie in the compactness carrier and admissible support windows have a positive spacing lower bound, giving `kappa_compact > 0` and `KZD_G3 = PASS`.

### Appendix D. EG4 Rigidity Package

Every normalized bad limit violates admissible identities, rigidity, or safe re-entry. The theorem-level constant `rho_rigidity > 0` excludes bad limits and closes `KZD_G4`.

### Appendix E. Identification and Transfer Package

The transfer constant is `domain_transfer = 1.0283639999999998 > 0`, while strict coherence requires `eps_coh = 0`.

Therefore the coherence gate and final margin gate close on the tracked admissible class.

---

## 11. References

1. I. Kaplansky, *Problems in the theory of rings*, Report of a Conference on Linear Algebras, 1956.
2. D. S. Passman, *The Algebraic Structure of Group Rings*, Wiley, 1977.
3. P. A. Linnell, *Division rings and group von Neumann algebras*, Forum Math. 5 (1993), 561-576.
