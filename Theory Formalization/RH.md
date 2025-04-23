## Theorem 1 (SUR cost is affine)

### 1.1 Assumptions
Identical to v1:

1. **Domain** \(L:\mathbb R_{\ge0}^2\to\mathbb R_{\ge0}\).
2. **Monotone** If \((K_2,E_2)\succeq(K_1,E_1)\) then \(L_2\ge L_1\).
3. **Additive** \(L(K_1+K_2,E_1+E_2)=L_1+L_2\).
4. **Unit‑scale invariance** \(L(\alpha K,\alpha E)=\alpha L(K,E)\).

### 1.2 Derivation
Standard Cauchy → linear \(f(K)=aK\), \(g(E)=bE\) → scale fix \(a=1\).

\[
\boxed{L(K,E)=K+\lambda E,\quad \lambda=b>0.}
\]
*Note: This establishes the unique linear form for the *base* cost functional relevant for local SUR optimization.*

### 1.3 Falsifiability
Find any \(L\) obeying 1–4 that is not affine → IC invalid at base level.

---

## Theorem 2 (Only three spatial dimensions yield finite SUR cost)

*Sections identical to v1 but include one additional check:*

### 2.5 Equation‑of‑state robustness test
Replace quantum pressure by **any** term \(E_Q\propto N^\alpha / R^\beta\) with \(\alpha>1\) (extensive) and \(\beta>0\). Re‑doing the saddle‑point shows the sign of
\[
\Delta(d_s)=\beta - (d_s-2)
\]
controls divergence. Only for \(d_s=3\) can \(\Delta=0\) be satisfied without setting \(\alpha=1\) (which would violate extensivity). Thus the result survives all reasonable EOS choices.

*All other sub‑sections remain unchanged.*
*Note: This theorem relies on minimizing the base cost L=K+λE at equilibrium.*

---

## Theorem 3 (Zeta‑function is necessary and RH ↔ SUR stability - Conjectured Link)

### 3.1 Unique multiplicative norm from base SUR cost

**Goal:** show that
\[
|m| = \exp\!\bigl[\ell(m)\bigr],\quad
\ell(m)=K(m)+\lambda E(m)
\tag{3.1}
\]
is *the only* homomorphic embedding of the additive *base* SUR cost \(L = K+\lambda E\) into a multiplicative scale.

*Proof sketch*

1. **Homomorphism requirement** For concatenated words \(m_1,m_2\) we need \(|m_1m_2|=|m_1||m_2|\).
2. **Base Cost additivity** (Th. 1) gives \(\ell(m_1m_2)=\ell(m_1)+\ell(m_2)\).
3. **Cauchy again** The only real‑valued function transforming sums into products is the exponential.
4. **λ fixed** Different base λ corresponds to rescaling energy units, already fixed by unit choice in Th. 1.

Hence (3.1) is claimed as the unique multiplicative norm respecting the base SUR cost `L`.

### 3.2 Generating function
\[
\mathcal C(s)=\sum_{m\in M}|m|^{-s}
           =\prod_{a\;\text{irreducible}}(1-|a|^{-s})^{-1}.
\]
*Note: This uses the norm derived from the base cost L.*

### 3.3 Renormalisability ⇔ single‑pole β‑function (Connection requires care)

**Derivation (Conceptual link needs refinement)**

1. Renormalization Group (RG) flow is analyzed on the `(K, C₂, F_β)` state space, governed by `λ̃ = C₂ / (12F_β)`.
2. Physical renormalizability often implies the existence of a well-behaved flow with a limited number of relevant directions (couplings that grow under coarse-graining).
3. A *single* relevant coupling corresponds to the flow dynamics being dominated by one primary direction near a fixed point.
4. The analytic structure of the generating function `C(s)` (derived from the base cost L via the norm `|m|`) is proposed to reflect the structure of the underlying irreducible elements.
5. **Hypothesis:** The condition of having a single relevant coupling in the *physical RG flow* (governed by `λ̃`) translates to a condition on the *analytic structure* of the generating function `C(s)` based on the simpler norm `|m|`, specifically requiring `C(s)` to have only one simple pole in the relevant domain (`Re s > 0`). This linkage needs rigorous proof.

*Current Status: This step links the physical RG flow concept (on `(K, C₂, F_β)`) to the analytic properties of `C(s)` (derived from `L=K+λE`). This connection is hypothesized, not proven.*

### 3.4 Only \(\mathbb Z\) meets the single‑pole condition for `C(s)`

Identical number‑theoretic argument from v1: Assuming the connection in 3.3 holds, any UFD \(R\neq\mathbb Z\) used to define `M` and `|m|` would inject extra Dirichlet \(L\)-factors into `C(s)` ⇒ extra poles/zeros ⇒ fails the hypothesized single‑pole condition linked to renormalizability.

\[
\boxed{\mathcal C(s)=\zeta(s).} \quad \text{(Conditional on 3.1, 3.3)}
\]

### 3.5 Riemann Hypothesis ↔ Lyapunov stability (Conditional Link)

**Hypothesis:** The stability of the physical SUR Renormalization flow (on the `(K, C₂, F_β)` manifold, governed by `λ̃`) is mathematically equivalent to the location of the zeros of the Zeta function `ζ(s)` (which arose from the base cost structure).

*Argument Sketch:*
Linearized physical RG flow near a fixed point:
\(\delta (\text{State})(t) \sim \sum_{\text{eigenmodes } \rho} \exp[-(\text{eigenvalue related to } \rho) t]\).
If the eigenvalues controlling stability are directly related to the Zeta zeros `ρ` (specifically, `1-ρ`), then:
Boundedness (stability) of the physical flow ⇔ Real part of eigenvalues > 0 ⇔ `Re(1-ρ) > 0` ⇔ `Re ρ < 1`. *Correction needed: Standard argument relates decay rate to distance from critical line, stability needs `Re(ρ)=1/2`.*

*Refined Argument Sketch:*
Linearized flow analysis relates stability to eigenvalues derived from the RG beta function (`β(λ̃)`). If `β(λ̃)`'s structure near the fixed point is dictated by the non-trivial zeros `ρ` of `ζ(s)`, then stability (non-divergent oscillations) requires `Re(ρ) = 1/2`.

Therefore, the proposed connection is:
\[
\boxed{\text{SUR RG flow stable } \Longleftrightarrow \text{RH true}.} \quad \text{(Conjectured Equivalence)}
\]

### 3.6 Falsifiability

*   Derive a non‑exponential homomorphic norm from base SUR cost `L` → 3.1 false.
*   Prove the connection between physical RG stability (`λ̃` flow) and the analytic structure of `C(s)` (from `L`) is invalid → 3.3 false.
*   Find a UFD whose `C(s)` has only one pole but is not ζ(s) → 3.4 false (given 3.3).
*   Show SUR RG flow is stable while RH is false, or vice-versa → 3.5 false.

Any of these breaks the proposed IC ↔ RH link.

---

## Dependency Diagram (v2 - Updated with Qualification)

```mermaid
graph TD
  A((SUR axioms)) --> B[Base L = K + λE (Th‑1)]
  B --> C{Unique norm |m|=exp(L) ? (3.1)}
  C --> D{Partition product = ζ(s) ? (3.4)}

  subgraph RG Flow Analysis
    RF1((State Space K, C₂, F_β))
    RF2((Monotonic λ̃ = C₂ / 12F_β))
    RF3((Physical RG Flow Stability))
  end

  D -- Hypothesized Link ---> RF3
  RF3 -- Conjectured Equivalence ---> F[RH ⇔ stability (3.5)]

  E((Single Pole ⇔ Renorm? (3.3))) -.-> D
  RF2 -.-> E


  B --> G[d_s=3 (Th‑2)]

  style C fill:#f9f,stroke:#333,stroke-width:2px
  style D fill:#f9f,stroke:#333,stroke-width:2px
  style E fill:#f9f,stroke:#333,stroke-width:2px
  style F fill:#f9f,stroke:#333,stroke-width:2px
