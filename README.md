# Nested Congruence Constraints on Collatz Synchronization

**Paper H — Jump Heights, Odd-Core Transport, and the Consecutive Cascade Conflict**

Establishes the algebraic mechanism governing synchronization jump heights in Collatz dynamics. At renewal events, the next jump height is exactly determined by the residue of the odd core, and consecutive jumps of the same height are proved impossible.

> This repository does not claim a proof of the Collatz conjecture.

---

## Overview

Building on the odd-core decomposition nₜ = 1 + 2^{aₜ} qₜ, this paper proves that at renewal events (aₜ = 1), the next jump height is given by aₜ₊₁ = v₂(3qₜ + 1), and height K is achieved if and only if qₜ ≡ r_K (mod 2^K). The target residue class has density 2^{-K} — exponentially thin.

The central results are:

- **Theorem JE** (Jump-Explosion Link): Jump height formula is exact; achieving height K requires qₜ in a residue class of density 2^{-K}
- **Theorem CC** (Consecutive Cascade Conflict): Two consecutive jumps of the same height K ≥ 4 are impossible
- **Nested congruence chain**: ord_{2^K}(3) = 2^{K-2} and the cascade length L = ⌊(K−2)/2⌋ satisfies 3^L ≢ 1 (mod 2^K)

---

## Main Results

### Proved (Rigorous)

| Result | Method | Status |
|--------|--------|--------|
| Theorem JE: exact jump height formula | 2-adic valuation | ✓ proved |
| Theorem JE: height K requires qₜ ≡ r_K (mod 2^K), density 2^{-K} | Congruence | ✓ proved |
| Theorem CC: consecutive same-height jumps impossible (K ≥ 4) | Order of 3 mod 2^K | ✓ proved |
| ord_{2^K}(3) = 2^{K-2} | Group theory | ✓ proved |

---

## Structure

```
§1   Introduction and structure
§2   Theorem JE: jump formula          ✓
§3   Theorem CC: consecutive conflict   ✓
§4   The nested congruence chain        ✓
§5   The core open problem
§6   Summary
```

---

## Open Problems

- Can jumps of strictly increasing heights K₁ < K₂ < K₃ < ··· → ∞ be simultaneously achieved by a single orbit, given that each cascade multiplies q by 3^{⌊Kᵢ/2⌋}?

---

## Repository Structure

```
collatz-congruence-synchronization/
├── README.md
├── paper/
│   └── paper_h_nested_congruence_constraints.pdf
└── LICENSE
```

---

## Related Work

This paper is part of a series on Collatz dynamics:

- [collatz-act1](https://github.com/KAMANOI/collatz-act1) — Foundational paper: prime survival dynamics and Chen-type theorem (v11)
- [collatz-renewal-structure](https://github.com/KAMANOI/collatz-renewal-structure) — Paper A: exact operator structure and finite information memory
- [collatz-finite-mixing-geometry](https://github.com/KAMANOI/collatz-finite-mixing-geometry) — Paper B: finite-level mixing geometry
- [collatz-spectral-amplification](https://github.com/KAMANOI/collatz-spectral-amplification) — Paper C: spectral amplification
- [collatz-scale-coherence](https://github.com/KAMANOI/collatz-scale-coherence) — Paper D: scale-coherence rigidity
- [collatz-valuation-renewal](https://github.com/KAMANOI/collatz-valuation-renewal) — Valuation renewal, finite residue connectivity, and orbitwise gap
- [collatz-residual-core](https://github.com/KAMANOI/collatz-residual-core) — The residual core: structural decomposition
- [collatz-congruence-synchronization](https://github.com/KAMANOI/collatz-congruence-synchronization) — Paper H: nested congruence constraints on synchronization
- [collatz-record-renewal](https://github.com/KAMANOI/collatz-record-renewal) — Paper N: record renewal compatibility
- [collatz-hensel-escape](https://github.com/KAMANOI/collatz-hensel-escape) — Paper O: Hensel memory and 2-adic escape target
- [collatz-hensel-scarcity](https://github.com/KAMANOI/collatz-hensel-scarcity) — Paper T: Hensel conditional scarcity and telescoping contradiction
- [collatz-prefix-counting](https://github.com/KAMANOI/collatz-prefix-counting) — Paper V: direct prefix counting and synchronization collapse
- [collatz-first-passage](https://github.com/KAMANOI/collatz-first-passage) — Paper W: first-passage obstruction (closes series A–V)
- [collatz-series-summary](https://github.com/KAMANOI/collatz-series-summary) — Series summary: research program on Collatz synchronization dynamics
- [collatz-prime-survival](https://github.com/KAMANOI/collatz-prime-survival) — Paper X v20: prime survival in affine Collatz dynamics

---

## Author

Hiroki Kamanoi
hirokikamanoi@gmail.com
2026
