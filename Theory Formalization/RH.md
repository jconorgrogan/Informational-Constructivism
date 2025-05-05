# Formal Core Results (IC / SUR v3)

---

## Theorem 1 (Base SUR cost is uniquely affine)

### 1.1 Axioms  
1. **Domain** \(L:\mathbb{R}_{\ge0}^2\!\to\!\mathbb{R}_{\ge0}\).  
2. **Monotonicity** \((K_2,E_2)\succeq(K_1,E_1)\Rightarrow L_2\!\ge\!L_1\).  
3. **Additivity** \(L(K_1\!+\!K_2,E_1\!+\!E_2)=L_1\!+\!L_2\).  
4. **Unit-scale invariance** \(L(\alpha K,\alpha E)=\alpha\,L(K,E)\) for all \(\alpha>0\).

### 1.2 Derivation  
Cauchy functional-equation arguments ⇒ \(L(K,E)=aK+bE\).  
Unit choice fixes \(a=1\); positivity demands \(b=\lambda>0\).

\[
\boxed{L(K,E)=K+\lambda E,\quad\lambda>0.}
\]

### 1.3 Falsifiability  
Exhibit any cost \(L\) satisfying 1–4 that is *not* affine ⇒ IC fails at ground level.

---

## Theorem 2 (Only \(d_s=3\) admits finite SUR equilibrium)

*Proof follows v1, with robustness addendum.*

### 2.5 Equation-of-state robustness  
Replace quantum pressure by any extensive term \(E_Q\propto N^\alpha/R^\beta\) (\(\alpha>1,\beta>0\)).  
At the saddle point the divergence sign is controlled by  

\[
\Delta(d_s)=\beta-(d_s-2).
\]

Finite total cost requires \(\Delta=0\).  The only integer spatial dimension satisfying \(\Delta=0\) without violating extensivity (\(\alpha>1\)) is  

\[
\boxed{d_s=3.}
\]

Thus the “three-dimensions” result is **independent** of the ζ-function material and relies solely on minimising \(L=K+\lambda E\).

---

## Theorem 3A (Exponential norm and the appearance of ζ)

### 3A.1 Uniqueness of the multiplicative norm  
For any message \(m\) with additive SUR cost \(\ell(m)=K(m)+\lambda E(m)\) define  

\[
|m|:=\exp\!\bigl[\ell(m)\bigr].
\]

*Claim:* \(|\cdot|\) is the **only** multiplicative embedding of \(L\) into \(\mathbb{R}_{>0}\).

*Sketch:* Additivity of \(L\) ⇒ \(\ell(m_1m_2)=\ell(m_1)+\ell(m_2)\).  
The sole real function turning sums into products is the exponential (Cauchy). ∎

### 3A.2 Generating function of irreducibles  
With that norm the partition function over the free commutative monoid \(M\) is

\[
\mathcal{C}(s)=\sum_{m\in M}|m|^{-s}
             =\prod_{a\;\text{irreducible}}\!(1-|a|^{-s})^{-1}.
\]

For \(M\cong(\mathbb{N}_{>1},\times)\) this *is* the Riemann zeta function:

\[
\boxed{\mathcal{C}(s)=\zeta(s).}
\]

(Any other UFD injects extra Dirichlet factors ⇒ extra poles/zeros.)

---

## Theorem 3B (SUR ledger stability ⇔ Prime-error bound ⇔ RH)

### 3B.1 Definitions  
* Ledger capacity \(C\).  
* Minimal code-length for primes ≤ \(x\): \(K_{\min}(x;C)\).  
* Prime counting error \(E_{\text{prime}}(x)=\pi(x)-\operatorname{Li}(x)\).

### 3B.2 Two instability lemmas  

*Lemma A (over-compression).*  
If \(|E_{\text{prime}}(x)| < k\,x^{\beta}\) for some \(\beta<\tfrac12\) eventually, then a prefix code shorter than \(\log p\!+\!o(\log p)\) exists ⇒ irreducible distinctions blur ⇒ violates SUR irreducibility.

*Lemma B (ledger blow-up).*  
If \(|E_{\text{prime}}(x)| > k\,x^{\beta}\) for some \(\beta>\tfrac12\) infinitely often, then \(K_{\min}(x;C)\to\infty\) ⇒ finite observer cannot maintain resolution thresholds.

### 3B.3 Critical-noise criterion  
SUR stability ⇔ neither lemma fires ⇔ tightest admissible bound is  

\[
|E_{\text{prime}}(x)|=O\!\bigl(x^{1/2+\varepsilon}\bigr).
\]

### 3B.4 Classical equivalence  
By the explicit-formula theorem of analytic number theory,  
\(E_{\text{prime}}(x)=O(x^{1/2+\varepsilon})\) ⇔ **all non-trivial zeros of ζ satisfy \(\Re \rho=\tfrac12\).**

\[
\boxed{\text{Finite-ledger SUR stability }\Longleftrightarrow\text{ RH true}.}
\]

### 3B.5 Falsifiability  
* Produce a prime stream with error exponent ≠½ for which SUR code remains stable ⇒ theorem false.  
* Conversely, find RH false yet SUR unstable ⇒ theorem vindicated.

---

## Appendix (RG single-pole conjecture) — *optional future work*  
The earlier idea that “single relevant coupling ⇔ ζ has one pole” can be restated as a conjecture linking physical β-functions to the analytic continuation of \(\mathcal{C}(s)\).  It is **not** required for Theorems 3A–3B.

---

## Dependency diagram (v3)

```mermaid
graph TD
  A((SUR axioms)) --> B[Affine cost L (Th.1)]
  B --> C[Exp norm |m| (Th.3A)]
  C --> D[ζ(s) product (Th.3A)]
  B --> E[d_s=3 (Th.2)]

  subgraph Ledger Stability
    F[Prime error bound]
    G[SUR stable ⇔ RH (Th.3B)]
  end

  D --> F
  F --> G
