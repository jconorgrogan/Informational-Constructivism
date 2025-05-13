
**Assumptions**

1. **Domain**  \(L:\,\mathbb R_{\ge 0}^{\,2}\to\mathbb R_{\ge 0}\) with arguments \(K\) (code length) and \(E\) (energy).  
2. **Monotonicity**  If \(K_2 \ge K_1\) and \(E_2 \ge E_1\) then \(L(K_2,E_2) \ge L(K_1,E_1)\).  
3. **Additivity for independent subsystems**  
   \(L(K_1+K_2,\;E_1+E_2)=L(K_1,E_1)+L(K_2,E_2)\) for all \((K_i,E_i)\).  
4. **Scale‑invariance of units**  For every \(\alpha>0\),  
   \(L(\alpha K,\alpha E)=\alpha\,L(K,E)\).

**Goal:** show \(L(K,E)=aK+bE\) with constants \(a,b>0\).

---

#### Step 1  Separate \(K\) and \(E\)

Define  
\(f(K)=L(K,0),\qquad g(E)=L(0,E).\)

Using additivity with \((K,0)\) and \((0,E)\),

\(L(K,E)=L(K,0)+L(0,E)=f(K)+g(E). \tag{1}\)

---

#### Step 2  Additivity forces linear Cauchy functions

From assumption 3 with energy fixed to zero:

\(f(K+K')=f(K)+f(K'). \tag{2}\)

Likewise with code length fixed to zero:

\(g(E+E')=g(E)+g(E'). \tag{3}\)

Monotone solutions of the one‑variable Cauchy equation are linear, so

\(f(K)=aK,\qquad g(E)=bE,\qquad a,b\ge 0. \tag{4}\)

---

#### Step 3  Assemble the general form

Insert (4) into (1):

\(L(K,E)=aK+bE. \tag{5}\)

---

#### Step 4  Use scale‑invariance to relate coefficients

Assumption 4 gives

\(L(\alpha K,\alpha E)=\alpha L(K,E)\).

With (5) this holds for all \(\alpha\); choose units so \(a=1\), yielding

\[
\boxed{\,L(K,E)=K+\lambda E,\qquad \lambda=b/a>0\,}. \tag{6}
\]

---

**Result**

Under monotonicity, subsystem additivity, and unit scale‑invariance, the SUR cost functional is necessarily affine linear in \(K\) and \(E\).
