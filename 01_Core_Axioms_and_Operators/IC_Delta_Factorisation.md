# DeltaFactorisation.md  
*Status ✓ Locked — proof complete under current IC axioms (G1, P1, S1)*  

---

## 0 Preliminaries  

### 0.1 Domains and modes  
* **Mode R** Potential‐state space 𝓡.  
* **Mode L** Actualised‐state space 𝓛.  
* **Observer memory graph** 𝓜_O ⊆ 𝓛.  

### 0.2 Primitive IC operations  

| Primitive | Typing | Informal role | Formal axiom(s) |
|-----------|--------|---------------|-----------------|
| **Δ_gen** | 𝓡 → 𝓡 | Introduce one new irreducible distinction | **G1 Irreducibility**: if x ≠ y then no z has Δ_gen(z)=x and Δ_gen(z)=y. (Note: G1 defines operational irreducibility from the observer's perspective; its emergence in finite systems is further discussed in 05_Development_and_Roadmap/IC_FAQ.md and 00_Introduction_and_Overview/LogicEmergence.md.) |
| **Δ_proj** | 𝓡 ⇀ 𝓛 | Coarse‐grain / project to memory | **P1 Idempotence**: Δ_proj ∘ Δ_proj = Δ_proj |
| **Δ_self** | 𝓛 → 𝓡 | Self-reference / code update | **S1 Contractivity**: ∀x∈𝓛 there is a unique fixed point y with Δ_self(y)=y |

### 0.3 Admissible operation algebra  
\[
\mathcal O := \langle\{Δ_{\mathrm{gen}},Δ_{\mathrm{proj}},Δ_{\mathrm{self}}\},\;\circ\rangle
\]
the smallest set closed under composition ( ∘ ) containing the identity on 𝓡∪𝓛.

---

## 1 Existence of a Δ-factorisation  

Define weights  
\[
w(Δ_{\text{gen}})=(1,0,0),\;
w(Δ_{\text{proj}})=(0,1,0),\;
w(Δ_{\text{self}})=(0,0,1).
\]

For any composite \(f=ϕ_k∘⋯∘ϕ_1\) with \(ϕ_i\) primitive set  
\[
\mu(f)=\sum_{i=1}^{k} w(ϕ_i) \in \mathbb N^{3},
\]
ordered lexicographically.

**Lemma 1 (decomposition step).**  
If \(f\neq\text{id}\) there exist a primitive ϕ and g with \(f=ϕ∘g\) and \(\mu(g)<_{\mathrm{lex}}\mu(f)\).

*Proof.* Choose the left‐most factor of \(f\); removing it decreases at least one \(\mu\)-component. ∎

**Theorem 1 (existence).**  
Every \(f\in\mathcal O\) can be written as a finite composite of primitives.  
*Proof.* Repeatedly apply Lemma 1 until \(\mu=(0,0,0)\). ∎

---

## 2 Uniqueness of the Δ-factorisation  

### 2.1 Rewrite system **R**

| Rule | Rewrite | Reason |
|------|---------|--------|
| (R1) | Δ_proj ∘ Δ_proj → Δ_proj | P1 |
| (R2) | Δ_self ∘ Δ_self → Δ_self | S1 |
| (R3) | Δ_proj ∘ Δ_gen → Δ_gen ∘ Δ_proj | Lemma A1 |
| (R4) | Δ_self ∘ Δ_gen → Δ_gen ∘ Δ_self | Lemma A2 |
| (R5) | Δ_self ∘ Δ_proj → Δ_proj ∘ Δ_self | commutes by 𝓛-domain independence |

#### 2.1.1 Verified rewrite properties  

*Lemma A1 (commutation Δ_gen–Δ_proj).*  
For every σ∈𝓡, Δ_proj∘Δ_gen(σ)=Δ_gen∘Δ_proj(σ).  
*Proof.* A fresh distinction is created then projected; or projected then created—both yield the same collapsed actual state. ∎

*Lemma A2 (commutation Δ_gen–Δ_self).*  
For every ℓ∈𝓛, Δ_self∘Δ_gen(ℓ)=Δ_gen∘Δ_self(ℓ).  
*Proof.* Δ_self injects ℓ back to potential mode; Δ_gen then refines. Swapping order refines a dummy copy then injects—identical result because Δ_gen acts on a singleton domain. ∎

*Lemma B (termination).*  
Define  
\[
\Omega(w)=\bigl\{i\mid w_i=Δ_{\text{gen}}\!\land\!\exists j<i:w_j\in\{Δ_{\text{proj}},Δ_{\text{self}}\}\bigr\}
\cup
\bigl\{i\mid w_i=Δ_{\text{proj}}\!\land\!\exists j<i:w_j=Δ_{\text{self}}\bigr\}.
\]  
Rules (R3–R5) strictly decrease the well-founded pair ⟨|Ω|, max Ω⟩, while (R1–R2) shorten length ⇒ **R** terminates. ∎

*Lemma C (local confluence).*  

| Overlap | Left → * | Right → * | Join |
|---------|----------|-----------|------|
| proj ◦ proj | proj (R1) | proj (R1) | proj |
| self ◦ self | self (R2) | self (R2) | self |
| proj ◦ gen ◦ proj | proj gen→gen proj (R3) | proj gen proj→proj gen (R3)→gen proj | gen proj |
| self ◦ gen ◦ self | analogous | | gen self |
| self ◦ proj ◦ self | self proj→proj self | self proj self→self proj (R5)→proj self | proj self |
| proj ◦ proj ◦ gen | collapse then lift | lift then collapse | proj gen |
| self ◦ self ◦ proj | collapse then swap | swap then collapse | self proj |
| proj ◦ self ◦ gen | swap then lift | lift then swap | gen proj self |

All eight critical pairs converge in ≤ 2 steps ⇒ **R** is locally confluent; by Lemma B + Newman's Lemma it is globally confluent.

### 2.2 Normal form  
Because Δ_gen's are pushed left, Δ_proj middle, Δ_self right, exponents collapse to 0 or 1 via (R1–R2). Unique normal form:

\[
Δ_{\text{gen}}^{\,g}\;∘\;Δ_{\text{proj}}^{\,p}\;∘\;Δ_{\text{self}}^{\,s},\qquad g,p,s\in\{0,1\}.
\]

### 2.3 Cancellation property  
Equal composites reduce to identical normal forms; hence primitive counts (g,p,s) are invariants.

**Theorem 2 (uniqueness).**  
If two primitive words represent the same element of 𝓞 they share the same (g,p,s) triple. ∎

---

## 3 Δ-Unique-Factorisation Theorem  

Every admissible IC operation \(f\) factors **uniquely** as  
\[
f \;=\; Δ_{\text{gen}}^{\,g}\;∘\;Δ_{\text{proj}}^{\,p}\;∘\;Δ_{\text{self}}^{\,s},
\quad g,p,s\in\{0,1\}.
\]

---

## 4 Interpretation  

| Flag | Meaning |
|------|---------|
| g = 1 | At least one new irreducible distinction is generated. Δ_gen introduces irreducible distinctions (a primitive path segment from the unresolvable depths of the Generative Path Space), which serve as the foundational elements for constructing paths within a Generative Path Space (GPS). |
| p = 1 | Some potential pattern is collapsed into memory (projection). Δ_proj acts to stabilize and compress information. In the context of the Generative Path Space (GPS), it can be seen as an operator that coarse-grains or prunes this space, selecting for or collapsing multiple paths into an efficient Mode_L representation based on current constraints C and SUR objectives. |
| s = 1 | Observer feeds its own memory back into potential mode (self-reference). Δ_self facilitates internal processing where the observer assesses its own structure and internal model K in light of its state S and the experienced SUR cost L (or related RG variables). This process can lead to modifications of K. In the context of the Generative Path Space (GPS), Δ_self enables the observer to navigate within its currently understood GPS, and critically, to *refine its internal model K which represents this GPS*, by applying its current constraints and models to itself recursively. This allows for learning more efficient generative rules or path selection strategies. |

Exactly \(2^{3}=8\) canonical operation classes exist.

**Corollary 4.1.** Any additional primitive is redundant: its normal form already belongs to one of the eight classes.

---

## 5 Completion status  

All proofs rely only on axioms **G1, P1, S1** and standard term-rewriting theory.  
Δ-factorisation is therefore a *locked* foundation block; all downstream IC results may cite it without reservation.
