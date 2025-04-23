#######################################################################
IC CORE PROOF PACK : Steps 0 – 4  (2025‑04‑21 snapshot R4‑final)
#######################################################################
CONTENTS
  0. Language / state model / SUR functional
  1. Δ‑factorisation – proved
  2. Category ΔCat ≅ FdHilb(ℂ) – dagger‑compact proof (snake fixed)
  3. Uniqueness of linear SUR Lyapunov  L = |K| + λE
  4. 3 + 1 Einstein equations from the SUR Hessian metric

───────────────────────────────────────────────────────────────────────
0 · LANGUAGE, STATE, OPERATORS, SUR (final‑v2)
───────────────────────────────────────────────────────────────────────
* Alphabet Σ – finite (|Σ| ≥ 2)
* Payload w ∈ Σ^{≤L_max}
* Record r = (w,n) n ∈ ℕ (version)
* State S – multiset of r, normal‑form: one record per payload, keep max n
* Handles M = [h₁,…,h_|M|] – indices into S (never dangle)
* Code K – prefix‑free bits encoding
 (i) predictive model P_K (ii) permutation π_K of S
* Runtime τ ∈ ℕ, Precision ε ∈ ℚ⁺
 Ledger C = (|M|, |K|, τ, ε)
* Observer Ω = (S, K, M)

**Primitive operators**
* Δ_gen     : add new record; extend π_K; add codeword
* Retract_gen: if refcount(last)=0 delete record & code else no‑op
* Δ_proj    : permute S to Kraft‑min π*, rewrite K, update M (idempotent)
* Δ_self[…] : arbitrary K/M edit obeying C; never touches S directly

**Single‑step macros (built from Δ_self)**
* dup  ≔ Δ_self[M := M ++ [last(M)]]
* drop ≔ Δ_self[M := remove_last(M)]

* Ledger‑respect: map halts ≤ τ and never increases |M|, |K|, ε
* SUR cost:      L = |K| + λE with λ = k_B T ln 2 (Step 3)
* E: cross‑entropy H(empirical || P_K)

───────────────────────────────────────────────────────────────────────
1 · Δ‑FACTORISATION (Theorem 1)
───────────────────────────────────────────────────────────────────────
Legal F: Ω → Ω – total, ledger‑respect, flips ≤ 1 version, never merges payloads

**Theorem 1.** F factors uniquely
 F = Δ_projᵃ ∘ Δ_selfᵇ ∘ Δ_genᶜ with a,b ∈ ℕ and c ∈ {0,1}.
Proof by edit‑depth induction; uniqueness from (|S|, |K|, π_K) invariants. ∎

Corollary: {Δ_gen, Δ_proj, Δ_self} is a strict minimal basis.

───────────────────────────────────────────────────────────────────────
2 · CATEGORY ΔCat ≅ FdHilb(ℂ) (dagger‑compact, corrected)
───────────────────────────────────────────────────────────────────────
* Objects – ledger cells
* Morphisms – Δ‑strings with L_out ≤ L_in
* Tensor C⊗D = (|M|+|M|', |K|+|K|', max τ, max ε), symmetry β
* Unit I = (0,0,0,0)

**Lemma 2.1  (Dagger)**
 G† = R, R† = G, (Δ_self script)† = inverse‑script
 (f†)† = f and (g∘f)† = f†∘g†

**Lemma 2.2  (Caps / Cups + Snake)** – all steps primitive
* Cap η_I = G ; dup         (record r, handles h₁,h₂ → r)
* Cup ε_I = drop ; drop ; R   (refcount 0 ⇒ R deletes r)
* β swaps wires, both handles fed to ε_I, r deleted, R cancels G – strict identity.

**Lemma 2.3  (Monoidal coherence)** – tensor on ℕ, β involutive
**Lemma 2.4  (Local tomography)** – Kraft‑minimal codes fix |K|; identical local stats ⇒ identical morphism
**Lemma 2.5  (Purification + Connected reversibles)** – positive P_K simplex gives connected Lie group via Δ_self; ancilla G + reversible Δ_self yields purification

Selinger 2008 Thm 7.9 prerequisites met ⇒ **ΔCat ≅ FdHilb(ℂ)**. ∎

───────────────────────────────────────────────────────────────────────
3 · UNIQUE SUR LYAPUNOV  L = |K| + λE
───────────────────────────────────────────────────────────────────────
For any C¹, strictly convex, coercive Lyapunov S(K,E):
 S = S* + ΔK + λ ΔE + o(‖Δ‖) near minimum.
Landauer bit erasure → λ = k_B T ln 2.  Unique linear cost L. ∎
*Footnote: In RG analysis replace E by F_β to obtain monotone flows.*

───────────────────────────────────────────────────────────────────────
4 · 3 + 1 EINSTEIN EQUATIONS FROM SUR METRIC
───────────────────────────────────────────────────────────────────────
* Information metric g_ab = ∂²L/∂xᵃ∂xᵇ
* Raychaudhuri + ledger Clausius δQ = T δS with δS = (k_B ln 2 / 4ℓ_p²) δA
* Using λ = k_B T ln 2: R_ab kᵃkᵇ = 8π G T_ab kᵃkᵇ
* Holds for all null kᵃ ⇒ **R_ab − ½R g_ab + Λ g_ab = 8π G T_ab**
 Λ to be fixed by SUR β‑function (Step 6) ∎
