# Constants as Ledger-Residuals  
*A Simplicity-Under-Resource account of transcendental numbers*  
**May 2025 — v1.4**

---

## Abstract  

Informational Constructivism (IC) models any finite information-processor by a **ledger**  

\[
C=(M,K,\tau,\varepsilon)
\]

recording memory, code length, run-time and numerical precision.  
Local dynamics minimise the **SUR** functional  

\[
L(K,E)=K+\lambda E,
\qquad 
\lambda = k_{\!B}T\ln 2 ,
\]

while coarse-grained (RG) dynamics minimise the monotone Lyapunov  

\[
\tilde{\lambda} \;=\; \frac{C_{2}}{12\,F_{\beta}},
\qquad 
F_{\beta}=E-\beta^{-1}K .
\]

When optimisation meets an **infinite-cost wall**—a configuration that would send one ledger column to ∞—search halts at a finite plateau and leaves a rigid, observer-independent **ledger residual**.  
IC identifies famous constants (π, e, γ, Feigenbaum δ, the inverse fine-structure constant α⁻¹, …) with such residuals.

This paper

* formalises the ledger-wall mechanism;  
* distinguishes **single-limit residuals** (π-type) from **ratio-of-limits residuals** (δ-type, including α⁻¹);  
* explains why Bailey–Borwein–Plouffe (BBP) digit extractors occur **only** when the wall has exact radix self-similarity;  
* shows that under any bounded code budget only *finitely* many residuals can be known, and under arbitrarily growing budgets the set remains *countable*;  
* supplies an **Appendix B** mapping successive conceptual gaps to their predicted constants.

---

## 1  Background & Critical Assumptions  

Classical analysis treats all real numbers alike, yet scientists repeatedly encounter a tiny elite.  
IC explains the imbalance as a **cost filter**: only constants whose *generating walls* can be encoded below an observer’s code budget ever appear.

> **Critical assumptions (to be proved or falsified)**  
> * **Universality** – the structural form of walls is universal: every sufficiently capable ledger meets the *same* wall template and converges to the same residual (up to units).  
> * **Uniqueness** – SUR has a unique optimum next to each wall.  
> * **Weight independence / canonisation** – residual values do not depend on arbitrary cost-weights (λ, μ) or those weights are themselves fixed by thermodynamics.

---

## 2  Ledger columns, SUR cost & compression walls  

### 2.1  Ledger columns  

| Symbol | Meaning |
|--------|---------|
| \(M\)  | memory cells |
| \(K\)  | code length (bits) |
| \(\tau\)| run-time steps |
| \(\varepsilon\)| numerical precision |

### 2.2  Base cost  

SUR linearity forces  

\[
L = K + \lambda E ,\qquad 
\lambda = k_{\!B}T\ln 2 .
\]

### 2.3  Stage-specific cost box  

For a focussed task the active functional may privilege additional terms  

\[
L_{\text{stage}} =  
K + \lambda E + \mu F_{\beta} + \dots ,
\qquad
F_{\beta}=E-\beta^{-1}K .
\]

### 2.4  Infinite-cost (compression) walls  

A **wall**—also called a *compression wall* or *incompressible boundary*—is the point beyond which any further attempt to reduce error or randomness would drive **at least one ledger column to infinity**.  SUR therefore brakes one step before the blow-up; the numerical slack that remains is the **ledger residual** (π, e, δ, …).

**Example (π in one breath).**  
Approximating a unit circle with an \(n\)-gon gives  

\[
K(n) \;\propto\; \log n, 
\qquad 
E(n) \;\propto\; n^{-2}.
\]

Minimising  

\[
L(n)=a\log n + \lambda b n^{-2}
\]

yields a finite optimum \(n_{*}\).  Adding one more side would raise \(K\) faster than it lowers \(E\), forcing an infinite marginal cost—the **compression wall**.  
The unreduced arc-length slack at that point is the constant π.

---

## 3  Two flavours of residual  

| Flavour | Mechanism | Example constants |
|---------|-----------|-------------------|
| **Single-limit residual** | One cost trend vs. code length stalls at a wall. | π, e, γ |
| **Ratio-of-limits residual** | **Two** independent costs co-shrink; their ratio locks. | Feigenbaum δ, α; conjecturally α⁻¹ |

*Plain picture.*  
Random-ness bill \(C_{2}\) and energy bill \(F_{\beta}\) both fall under coarse-graining; their ratio  

\[
\tilde{\lambda}=C_{2}/12F_{\beta}
\]

rises then plateaus.  Multiplying by the bit-to-energy conversion \(k_{\!B}T\ln2\) yields a dimensionless coupling—IC’s prediction for \(1/\alpha\).

---

## 4  Wall archetypes & case studies  

| Archetype | Diverging columns | Symmetry | Typical residual |
|-----------|-------------------|----------|------------------|
| **Curvature** (polygon → circle) | \(K↑,E↓\) | radix-4 | π, ζ(2) |
| **Discrete ↔ continuous** | \(\tau↑\) | log drift | e, γ, ζ(3) |
| **Modular / elliptic** | \(\varepsilon↓\) | modular | Catalan G |
| **RG fixed point** | \(\tau↑,\varepsilon↓\) | log-2 | δ, α, α⁻¹ (?) |
| **Statistical** | \(K↑\) | ergodic | Khinchin K₀ |
| **Constructed extreme** | \(K→∞\) | — | Liouville, Ω |

### 4.1  Selected examples  

*π* Regular \(n\)-gon wall (§2.4).  Exact 4-fold scaling ⇒ BBP series in base 16.

*e* \((1+1/n)^n\) wall.  Broken scaling ⇒ no BBP.

*Fine-structure constant* Flow of \(C_{2},F_{\beta}\) for EM vacuum plateaus; Landauer-scaled ratio matches 137.036.

---

## 5  Digit extraction & radix symmetry  

> **Conjecture 2 (BBP criterion).**  
> If a wall has exact radix-\(b\) self-similarity  
> \(\nabla L(Sx)=b^{-d}\nabla L(x)\) with \(S:x\mapsto b\,x\),  
> its residual admits a finite polylog / BBP series in base \(b\).

Verified for π, ζ(2) in base 16.  No such symmetry for γ ⇒ no BBP expected.

---

## 6  Curvature, Hessians & structure constants  

Residual values such as π, ζ(2k) appear in the Hessian of the cost landscape,  
\(g_{ij}=\partial_{i}\partial_{j}L\), acting as **structure constants** of the emergent information-metric.  Under RG flow they surface as universal fixed-point data.

---

## 7  How many constants fit any ledger?  

Walls describable with ≤ \(K_{\max}\) bits are ≤ \(2^{K_{\max}}\).  
Each wall yields finitely many residuals; therefore an observer with code budget \(K_{\max}\) can encounter *only finitely many* constants.  Allowing \(K_{\max}\to\infty\) gives a *countable* union, whereas the mathematical continuum is uncountable.

---

## 8  Future work  

1. **Universality proof** – residual independence from ledger budget above threshold.  
2. **Uniqueness proof** – convexity or dynamical argument for single optimum.  
3. **Weight analysis** – derive λ, μ canonically.  
4. **Explicit RG test of α⁻¹** – lattice-QED or functional RG for \(C_{2},F_{\beta}\) flow.  
5. **BBP criterion** – prove Conjecture 2 or find counter-example.  
6. **Modular walls** – classify elliptic constants; predict BBP status.  
7. **Hierarchy simulations** – verify Appendix B table in toy models.  
8. **Constant-free derivations** – show π emerges without prior π in the ledger.  
9. **Signed residuals** – interpret negative ζ(½) within optimal-structure parameters.

---

## Appendix A – Proof sketch: SUR linearity  

SUR linearity follows from monotonicity, subsystem additivity and unit-scale invariance; see formal Metamath file *sur.mm*.

---

## Appendix B – Hierarchy of minimal extensions  

| Stage | Task variable | Dominant cost term(s) | Wall / gap | Predicted residual | Status |
|-------|---------------|-----------------------|------------|--------------------|--------|
| 0 → 1 | Presence bit \(b\) | \(K\) | Distinct vs. indistinct | – | ✓ |
| 1 → 2 | Count \(N\) | \(E\) | Unbounded enumeration | – (Hₙ gap) | ✓ |
| 2 → 3 | Smoothing δ | \(F_{\beta}\) | Hₙ vs. ln n | γ | PTM |
| 3 → 4 | Rule \(R\) | \(K+\lambda E\) | Off-integer Γ | (π via reflection) | C |
| 4 → 5 | Truncation \(N\) | \(τ\) | Infinite series | e | C |
| ⋯ | ⋯ | ⋯ | ⋯ | ⋯ | ⋯ |
| “Angle” ϕ | \(K+\mu F_{\beta}\) | Perfect alignment | ζ(½) | C |

Symbols: ✓ proved PTM = toy-model proof C = conjecture.

---

## References  

Bailey, D. H.; Borwein, P.; Plouffe, S. (1997) “On the rapid computation of various polylogarithmic constants.”  
Borwein, J.; Bradley, D.; Gallimore, M. (2004) “A BBP-type formula for ζ(2).”  
Feigenbaum, M. J. (1978) “Quantitative universality for a class of nonlinear transformations.”  
Khinchin, A. (1935) *Continued Fractions.*  
Selinger, P. (2010) “A survey of graphical languages for monoidal categories.”  
IC technical notes: *ISG.md*, *sur.mm*, *deltafactorisation.mm*.
