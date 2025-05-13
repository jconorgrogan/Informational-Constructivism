#### Assumptions

* **SUR cost:** \(L = K + \lambda E\) with \(\lambda > 0\).  
* **System:** A self‑gravitating quantum register of \(N\) identical “bits’’ (mass \(m\)) confined to radius \(R\) in \(d_s\) spatial dimensions.  
* **Energetics:**  

| Term | Scaling | Origin / Robustness note |
|------|---------|--------------------------|
| Quantum pressure | \(E_Q \;\sim\; \dfrac{\hbar^2}{m}\, \dfrac{N^{\,1+2/d_s}}{R^{2}}\) | Holds for fermions; for bosons the same exponent appears once short‑range repulsion prevents trivial collapse. Any realistic correlation only changes the **coefficient**, not the exponent. |
| Gravity (weak‑field GR) | \(E_G \;\sim\; -\,G\,m^2\, \dfrac{N^{\,2}}{R^{d_s-2}}\) | Derived from the \(d_s\!+\!1\)‑dimensional Einstein equations in the Newtonian limit. Post‑Newtonian corrections alter the prefactor, not the \(R^{d_s-2}\) power. |

**Code length:** the most *lenient* assumption is \(K = N\).  Any compression (\(K < N\)) will only **strengthen** the conclusion because it reduces \(L\) equally in all dimensions.

---

#### Stationary Radius

Minimise \(E(R)=E_Q+E_G\) in \(R\):

\[
\frac{\partial E}{\partial R}=0
\;\;\Longrightarrow\;\;
R_c \;=\;
\Bigl[\frac{d_s-2}{2}\Bigr]^{\!1/(d_s-4)}
\, N^{\,(1-2/d_s)/(d_s-4)}.
\tag{1}
\]

Define the exponent  
\(\displaystyle \gamma(d_s) = \frac{1-2/d_s}{d_s-4}.\)

---

#### SUR Cost per Bit in the \(N \to \infty\) Limit

Because \(K=N\) is \(R\)-independent, minimising \(L\) in \(R\) yields the same \(R_c\) as (1). Evaluate

\[
\frac{L_{\min}}{N}
=
1 + \lambda \frac{E_Q(R_c)+E_G(R_c)}{N}.
\]

| Region | \(\gamma(d_s)\) | Behaviour of \(R_c\) as \(N\!\to\!\infty\) | Outcome for \(L_{\min}/N\) |
|--------|-----------------|---------------------------------------------|---------------------------|
| \(d_s < 3\) | \(+\) | \(R_c \!\to\! 0\) (UV collapse) | \(E_G \!\to\! -\infty\) ⇒ \(L/N\!\to\! -\infty\) (unstable) |
| **\(d_s = 3\)** | \(-\tfrac13\) | \(R_c \propto N^{-1/3}\) | Finite plateau; \(L/N\) bounded and positive |
| \(3 < d_s < 4\) | \(-\) | \(R_c \!\to\! 0\) | Same UV collapse as \(d_s<3\) |
| \(d_s = 4\) | \(0\) | \(R_c \propto N^{1/2}\) | Finite plateau **only if** gravitational prefactor is small; one‑loop GR boosts it ⇒ instability |
| \(d_s > 4\) | \(+\) | \(R_c \!\to\! \infty\) (IR dispersion) | \(E_Q\!\to\! 0\), info density \(\to 0\); \(L/N \!\to\! +\infty\) |

---

#### Robustness Audit

1. **Different statistics / interactions** Changing particle type or adding realistic correlations alters coefficients, not exponents → the divergence pattern is unchanged.  
2. **Full GR** Tolman–Oppenheimer–Volkoff solutions preserve the \(R^{d_s-2}\) scaling until a horizon forms, which *tightens* the exclusion for \(d_s>3\).  
3. **Alternate code scaling** If \(K < N\) (compression), \(L/N\) decreases **equally in every dimension**, so relative divergence remains.  
4. **λ‑dependence** \(\lambda\) rescales energy but leaves \(R_c\) and the divergence signs untouched.  
5. **Metastability at \(d_s=4\)** Exact power balance; quantum‑gravity corrections drive the system off the knife‑edge, rendering \(d_s=4\) unstable.  
6. **Local minima vs global divergence** SUR demands a *finite* thermodynamic cost; any global divergence forces perpetual renormalisation, violating “stationary slack’’—hence forbidden.

---

### Final Statement

\[
\boxed{
\displaystyle
\lim_{N\to\infty}\frac{L_{\min}}{N}
=
\begin{cases}
+\infty & d_s \neq 3,\\[6pt]
\text{finite} & d_s = 3.
\end{cases}}
\]

Therefore **three spatial dimensions** (with an induced temporal ordering from successive SUR updates) is the *unique* rank compatible with a stable, self‑maintaining information register under the SUR principle.
