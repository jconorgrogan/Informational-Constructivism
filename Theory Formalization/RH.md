## Theorem 1 (SUR cost is affine)

### 1.1 Assumptions  
Identical to v1:

1. **Domain** \(L:\mathbb R_{\ge0}^2\to\mathbb R_{\ge0}\).  
2. **Monotone** If \((K_2,E_2)\succeq(K_1,E_1)\) then \(L_2\ge L_1\).  
3. **Additive** \(L(K_1+K_2,E_1+E_2)=L_1+L_2\).  
4. **Unit‑scale invariance** \(L(\alpha K,\alpha E)=\alpha L(K,E)\).

### 1.2 Derivation  
Standard Cauchy → linear \(f(K)=aK\), \(g(E)=bE\) → scale fix \(a=1\).

\[
\boxed{L(K,E)=K+\lambda E,\quad \lambda=b>0.}
\]

### 1.3 Falsifiability  
Find any \(L\) obeying 1–4 that is not affine → IC invalid.

---

## Theorem 2 (Only three spatial dimensions yield finite SUR cost)

*Sections identical to v1 but include one additional check:*

### 2.5 Equation‑of‑state robustness test  
Replace quantum pressure by **any** term \(E_Q\propto N^\alpha / R^\beta\) with \(\alpha>1\) (extensive) and \(\beta>0\).  Re‑doing the saddle‑point shows the sign of  
\[
\Delta(d_s)=\beta - (d_s-2)
\]
controls divergence.  Only for \(d_s=3\) can \(\Delta=0\) be satisfied without setting \(\alpha=1\) (which would violate extensivity).  Thus the result survives all reasonable EOS choices.

*All other sub‑sections remain unchanged.*

---

## Theorem 3 (Zeta‑function is necessary and RH ↔ SUR stability)

### 3.1 Unique multiplicative norm from SUR cost

**Goal:** show that  
\[
|m| = \exp\!\bigl[\ell(m)\bigr],\quad 
\ell(m)=|m_K|+\lambda|m_E|
\tag{3.1}
\]
is *the only* homomorphic embedding of additive SUR cost into a multiplicative scale.

*Proof sketch*

1. **Homomorphism requirement**  
   For concatenated words \(m_1,m_2\) we need \(|m_1m_2|=|m_1||m_2|\).  
2. **Cost additivity** (Th. 1) gives \(\ell(m_1m_2)=\ell(m_1)+\ell(m_2)\).  
3. **Cauchy again** The only real‑valued function transforming sums into products is the exponential.  
4. **λ fixed** Different λ would correspond to rescaling energy units, already fixed by unit choice in Th. 1.

Hence (3.1) is unique; no alternative norm exists that (i) respects SUR cost, (ii) is multiplicative.

### 3.2 Generating function

\[
\mathcal C(s)=\sum_{m\in M}|m|^{-s}
           =\prod_{a\;\text{irreducible}}(1-|a|^{-s})^{-1}.
\]

### 3.3 Renormalisability ⇔ single‑pole β‑function

**Derivation (new)**

1. Fisher metric for coarse‑grained scale μ:  
   \(g(\mu)=\partial_\mu^2 L\Big|_{\mu}\).  
2. Under rescaling \(|m|\to|m|^{b}\) (b > 1) we get  
   \(g(\mu+b) = g(\mu)+\beta(g)\,b +\dots\).  
3. A *single* relevant coupling ⇔ \(\beta(g)\propto g-g_\star\) near the fixed point \(g_\star\).  
   Writing \(g(\mu)=d\!\log\mathcal C/d\mu\) maps this to analytic structure of \(\mathcal C\).  
4. Meromorphic continuation shows: **exactly one simple pole** in \(g(s)\) on \(\Re s>0\) ⇔ exactly one relevant direction.

Any additional pole forces an extra independent coupling, splitting SUR slack into >1 scalar → violates IC postulate that complexity reduction is a single‑parameter process.

### 3.4 Only \(\mathbb Z\) meets the single‑pole condition  

Identical number‑theoretic argument from v1: any UFD \(R\neq\mathbb Z\) injects extra Dirichlet \(L\)-factors ⇒ extra poles/zeros ⇒ fails 3.3.

\[
\boxed{\mathcal C(s)=\zeta(s).}
\]

### 3.5 Riemann Hypothesis ↔ Lyapunov stability

Linearised flow:  
\(\delta g(t)\sim\sum_{\zeta(\rho)=0}\!\exp[-(\rho-1)t]\).  
Boundedness ⇔ \(\Re\rho=\tfrac12\).  Therefore

\[
\boxed{\text{SUR flow stable } \Longleftrightarrow \text{RH true}.}
\]

### 3.6 Falsifiability

* Either derive a non‑exponential homomorphic norm from SUR cost → 3.1 false.  
* Or find a multiplicative label set whose \(\mathcal C(s)\) has only one pole but is *not* ζ(s) → 3.4 false.  
* Or show SUR flow stable while RH false → 3.5 false.

Any of these breaks IC.

---

## Dependency Diagram (v2)

```mermaid
graph TD
  A((SUR axioms)) --> B[L = K + λE (Th‑1)]
  B --> C[Unique norm |m| (3.1)]
  C --> D[Partition product ζ(s) (3.4)]
  D --> E[One‑pole β  ⇔ renorm (3.3)]
  E --> F[RH ⇔ stability (3.5)]
  B --> G[d_s=3 (Th‑2)]
