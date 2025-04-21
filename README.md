# Informational Constructivism

## Preamble: The Primacy of Information and Contrast

There are several rival blueprints for what the universe is and why it exists. Quantum mechanics, general relativity, and string theory each offer a different ontology, yet they converge on one premise: **information** sits at the root of every description. No matter how the theories differ, all agree that something is being distinguished from something else. This points towards information processing as a fundamental aspect of reality.

But can we go deeper? Where does information, or the capacity for distinction, come from in the first place? Why should there be *any* distinction at all, any structure, any state that differs from another? Why is there something rather than nothing? [Further discussion: https://github.com/jconorgrogan/Why-there-is-something-and-not-nothing]

Informational Constructivism (IC) proposes that the most primitive *operational* event necessary for any structure or process is **Registered Contrast**. This minimal axiom, **F0**, consists of two inseparable components:
*   **D0 (Distinction Event):** Something is distinguishable from something else (a potential difference exists).
*   **R0 (Registration):** Some subsystem registers this distinction as a state change (an echo, a memory bit flip, however minimal).

Without D0, there is no difference to register. Without R0, any potential distinction has no informational consequence, leaves no trace, and cannot participate in any causal or computational process. F0 = D0 + R0 is thus the minimal requirement for "something happening" in an informational sense.

[From a phenomenological perspective, within sufficiently complex systems like evolved observers, the ongoing processing of such fundamental registered contrasts may correspond to the basic subjective experience of **feeling** or **presence** – the raw fact that *something* is being experienced, distinct from nothingness. This provides an experiential anchor, but the operational F0=D0+R0 is the formal starting point.]

Even a single F0 event implies latent "texture". This isn't an extra assumption, but a consequence of information theory: the set of possible simpler descriptions (programs) that could account for even one registered bit (`{p: U(p)=x}`) has unbounded complexity [See **Box 0b / TODO:** Formal lemma: Kolmogorov structure function / Levin's coding theorem application]. This potential complexity exists in the universal prior, providing a reservoir that later compression stages can exploit.

From F0 alone, a surprising chain of consequences follows via information compression under resource constraints (the SUR dynamic, detailed below): Registered contrast (F0) implies limitation (T2), limitation forces compression (T3), compression yields memory, prediction, time, identity, and eventually the structured physical world we observe (T4-T24).

Alternatively, consider the negation: Everything I started from is wrong; you do not permit me any axioms, and we therefore assume F0 is false – a uniform void (S₀) with absolutely no distinction (T25). As argued formally (Box 0), the very act of representing or processing this "void" state within *any* system capable of holding state necessitates introducing a minimal contrast (via `Δ_gen`), making the void inherently unstable from an internal perspective.

Therefore, IC develops two converging paths driven by the same underlying logic of information compression (SUR):
1.  **The Generative Path:** Starting from F0, SUR builds complexity and structure, eventually leading to observers capable of experiencing F0.
2.  **The Collapse Path:** Starting from the hypothetical void (T25/S₀), the instability forces the emergence of F0, initiating the generative path.

The framework below formalizes this self-consistent loop, where the existence of contrast necessitates structure, and the attempt to enforce absolute lack of contrast ironically generates it.

## The Counterpoint: The Instability of the Void (T25 / S₀)

Let's say that you disagree with my entire premise. Consider the negation: assume F0 is false, that the most basic reality is a uniform void with no distinction. As formalized below (Box 0), the very act of encoding, describing, or proving this void within a system capable of representation introduces contrast (via the minimal distinction-creating operation, `Δ_gen`), making the void state (S₀) inherently unstable or unreachable *within* the system.

**(Box 0: Pre-distinction state and the Genesis lemma)**
> **Definition S₀**
> The pre-distinction state S₀ is the unique configuration that satisfies
> ∀x,y ∈ S₀ : x ≡ y.
> It is maximally symmetric since no internal mapping can label one part of the state apart from another.
>
> **Genesis lemma**
> Let `Δ_gen` be any operation that violates the above equivalence at a single ordered pair. Then
> `Δ_gen` (S₀) = S₁ ≠ S₀
> and S₁ necessarily has at least one two-element equivalence class.
> *Proof sketch:* If S₁ still satisfied ∀x,y ≡, the violation never occurred; hence S₁≠S₀. Uses classical logic; removing LEM makes the lemma undecidable.

## The Engine: Δ-Operators and SUR Dynamics

Structure formation from F0, or the escape from S₀, is driven by fundamental information processing operators acting under resource constraints, governed by an emergent optimization principle: **Simplicity under Resource-constraint (SUR)**.

**(Box 1: The three Δ-operators and their algebra)**
> | Operator  | Type signature        | Laws                                                                                        |
> | :-------- | :-------------------- | :------------------------------------------------------------------------------------------ |
> | `Δ_gen`   | State → State         | Not idempotent; produces first non‑trivial equivalence class from S₀.                       |
> | `Δ_proj`  | (State, Constraint) → State | Idempotent: `Δ_proj`∘`Δ_proj` = `Δ_proj`. Stabilizes contrast under C.                   |
> | `Δ_self`  | (Code, Memory) → Code   | Generates self‑reference/model updates. Has unique fixed point Y if halts (Y := fix f(f)). |
>
> **Composition rules**
> 1. `Δ_proj`∘`Δ_gen` = `Δ_proj` (projection immediately stabilises fresh contrast).
> 2. `Δ_self`∘`Δ_proj` may diverge; if convergent, returns code encoding own description.
> 3. **Factorisation Theorem (Proof Pack Step 1):** Every finite legal Δ‑sequence factors uniquely as Δ = `Δ_proj`ᵃ ∘ `Δ_self`ᵇ ∘ `Δ_gen`ᶜ (a,b∈ℕ, c∈{0,1}, uniqueness via S/K invariants). This basis is minimal and complete.

**(Refined IC Lattice: Resource Constraints)**
> Structure emerges within resource limits defined by a "ledger" C:
> *   **Memory (M):** Number of state handles/slots.
> *   **Code (K):** Length (bits) of the observer's internal model/program.
> *   **Runtime (τ):** Processing steps allowed.
> *   **Precision (ε):** Allowed numerical/representational error.
> The lattice L_{M,K,τ,ε} contains structures reachable within budget C.

**(Box 2: Constraints as a dynamical vector)**
> Let C(t) = ( M(t), K(t), τ(t), ε(t) ) be the instantaneous resource budgets. Its slow drift can be modeled by:
> ```
> dC/dt = -∇_C L + η(t)
> ⟨η_i(t)η_j(t')⟩ = 2Dδ_ijδ(t−t')
> ```
> where L = K + λE is the SUR cost (see below), and η(t) is environmental noise (diffusion D has units ensuring L/D is dimensionless time, setting T scale). This shows C co-evolves under adaptive pressure to minimize cost L.

**(Emergence of MDL/SUR)**
> MDL/SUR is not posited but emerges as the stable equilibrium of local adaptive dynamics.
> *   **Setup:** System with finite C processing distinctions (F0), attempting to model/predict (Error E) using internal Code K.
> *   **Local Dynamics:** Subsystems adopt changes only if they reduce local cost L = K + λE (where λ balances description cost K vs. prediction error E).
> *   **Convergence:** Under finite C, these local steps converge to a minimum of L (cf. Robbins-Monro, requires step sizes γ_n s.t. Σγ_n = ∞, Σγ_n² < ∞). This minimum is the **Minimum Description Length / SUR** equilibrium.
> *   **Role:** SUR becomes the operational principle driving structure formation (T3a onwards).

## The IC Ladder: Building Reality from Contrast

The following ladder formalizes the loop: F0 → T24 (Generative) and T25 → F0 (Collapse). Both paths are driven by SUR dynamics under evolving constraints C.

**(Box 3: Operational boundary between Mode_R and Mode_L)**
> *   **Mode_R (relational):** Potential distinctions addressable under current C.
> *   **Mode_L (logged):** Image of Mode_R under `Δ_proj` stored in memory M.
> *   The map `Δ_proj` : Mode_R → Mode_L is surjective and idempotent. (Related to ζ(s) symmetry in speculative extensions).

**(Box 4: Memory graph metric)**
> Memory M forms a directed labelled graph G=(V,E).
> *   V = { S_k } (stabilised Δ outputs / Mode_L states).
> *   E = { (S_i, S_j, ℓ) } (Δ operator label ℓ ∈ {`Δ_gen`,`Δ_proj`,`Δ_self`}).
> *   Metrics: d_T (time = path length), d_I (information = cumulative SUR cost L along path).

**(Box 5: Landauer link and the λ parameter)**
> Minimising L = K + λE (predictive cross-entropy E=H) subject to a thermal reservoir (Noise D in Box 2) yields:
> λ = ∂K/∂H|_{min} = k_B T ln 2.
> Thus λ equals the marginal Landauer cost for information erasure at the effective temperature T set by noise D. It's not arbitrary.

**(Box 8: Layered resolution and synthetic indistinguishability)**
> Observers resolve distinctions only up to nesting depth k of `Δ_self`. Deeper structure remains indistinguishable (projects flatly). L_k = { S | S = `Δ_proj`^≤k(X) }. Layering enables consensus (T10) among observers with different k limits interacting within L_min(k₁,k₂).

### 1. Foundational Tiers & Forward Logic Sketch (Generative Path F0 → T12+)

| Tier | Label / Lemma       | Necessary statements                        | Why it follows (Forward Sketch)                                                | Minimal new term(s)         |
| :--- | :------------------ | :------------------------------------------ | :----------------------------------------------------------------------------- | :-------------------------- |
| 0    | F0—Registered Contrast | D0: Distinction + R0: Registration occur. | Minimal operational premise. Latent K-complexity (Box 0b).                   | distinction, registration   |
| 1    | Phenomenology       | F1 Numerous contrasts, F2 Memory ref, F3 Salience. | Direct unpacking of F0's latent texture & minimal registration.              | salience                    |
| 2    | Bottleneck          | C1 Finite channel [e.g. |M|,|K| bits], C2 Incompleteness. | From finite C (Box 2). Unlimited capacity flattens salience (T1).           | capacity                    |
| 3    | Compression         | S1 Selective retention, S2 Lossy memory trace. | Forced by T2 constraints on T0/T1 data. Uses Mode_R/L boundary (Box 3).     | memory trace, Mode_R/L      |
| 3a   | SUR (Emergent)      | System dynamics converge to L=K+λE minimum. | Local cost minimization converges under finite C (Robbins-Monro conditions). | MDL balance                 |
| 4    | Pattern extraction  | P1 MDL attractor, P2 Proto-self cluster.  | SUR (T3a) prunes redundant bits. Memory Graph G forms (Box 4).              | prediction, self cluster, memory graph G, d_T, d_I |
| 4.5  | Observer (O1)       | MDL compressor (K) + self-cluster (M) + `Δ_self` loop. | Minimal D0→R0→`Δ_self` loop under SUR for recursive prediction (T4).       | observer                    |
| 5    | World partition     | E1 World = non-self, ToM lemma.             | Complement of self + cheapest agent model (SUR). Uses Layering (Box 8).       | world, other mind           |
| 6    | Process dynamics    | D1 Arrow of time, D2 Info-metric distance d_I. | Compression (K reduction) monotone (T3a)→time. Metric from SUR cost (Box 4). | time, metric d_I            |
| 6a   | Op. constraints     | R1 Reversibility, R2 Additive cost, R3 No cloning. | SUR selects optimal codes [Lemma: L rises if E grows w/o K drop]. Link Box 5. | —                           |
| 7    | Theorem MIN (QM Base) | Constraints (T6a) force complex Hilbert space H. | Via Category theory: ΔCat ≅ FdHilb(ℂ) (Proof Pack Step 2).                 | Hilbert space H             |
| 8    | Probability rule    | Gleason ⇒ Born weights uniquely minimise L.   | Cost optimization on projectors in H (dim ≥ 3) (T7).                        | Born weights                |
| 9    | Projection bound    | Channel overrun → SUR prunes branches.      | Cost-minimal state selection under T2 capacity limit.                          | projection event            |
| 10   | Consensus layer     | Shared basis = inter-subjective reality.    | Intersection of observer channels (T4.5) via SUR, uses Layering (Box 8).     | inter-subjective reality    |
| 11   | Geometric curve     | Path-dependent code reuse ⇒ curvature.      | Second derivative of L along geodesics in G (Box 4). Links to Box 6.         | curvature                   |
| 12   | Energy analogue     | λ = ∂L/∂C ≈ 1/k_B T; conserved quantity emerges. | Lagrange multiplier λ (T3a, Box 2, Box 5) behaves like inverse Temp.         | energy analogue             |

**(Box 6: Curvature algebra / EFE Derivation)**
> Let g_ab = ∂²L/∂xᵃ∂xᵇ be the metric from T11. Using Raychaudhuri equation, the IC Area Law S = A k_B / (4ℓ_p²) (derived from Proof Pack Steps 1-3), and the Ledger Clausius relation δQ=TδS linked via λ (Box 5), leads to the Einstein Field Equations (as per Proof Pack Step 4):
> R_ab - ½R g_ab + Λ g_ab = 8πG T_ab.

**(Box 7: Emergent constants from SUR plateaus)**
> The parameter λ runs with scale μ: μ dλ/dμ = β(λ). Physical constants (like α⁻¹ ≈ 137.036) emerge at stable fixed points (β≈0) where the SUR cost landscape is locally scale-invariant. Derivation requires modeling interacting channels.

### 2. Speculative Extensions (Tiers 13 – 25)

*(Status: open=⊥, partial=≈, likely=≈≈)*

| Tier | Label                    | Core claim                                              | Driver / Prerequisite                              | Status |
| :--- | :----------------------- | :------------------------------------------------------ | :------------------------------------------------- | :----- |
| 13   | Local gauge symmetry     | Redundant global phase bit → U(1) → SU(2), SU(3)        | Lemma G (unused reference bits under SUR)          | ⊥      |
| 14   | Yang–Mills cost field    | Phase-gradient cost ‖dθ‖² → YM equations via MDL        | Euler-Lagrange on T13 phase cost                   | ⊥      |
| 15   | Mode factorisation / QFT | Area-scaled channel capacity → Fock space operators     | Bit-rate ∝ Area (from SUR/Holography)              | ≈      |
| 16   | Renormalisation flow     | Coarse-grain MDL gradient ⇒ β-functions                 | SUR gradient flow across T15 scales → Box 7        | ⊥      |
| 17   | Standard-Model constants | RG plateaus (Box 7) lock parameters → α, θ_W …          | MDL saturation at SUR fixed points                  | ≈      |
| 18   | GR field equations       | ∫(Curvature + λ) extremal ⇒ G = κT                    | T11 + T12 + Area Law under SUR (Box 6 / Step 4)    | ≈      |
| 19   | Inflation & spectra      | Channel capacity burst (T2) + Curvature (T11) → spectrum| Bottleneck shock + SUR dynamics                    | ≈      |
| 20   | Planck spin-foam codes   | Max-noise SUR → fault-tolerant graph codes (spin foams)| Robust MDL under high noise                       | ≈      |
| 21   | Computat. Irreducibility | Some T4 patterns compress no further (K reaches limit) | Kolmogorov bound inherent in SUR (T3a)             | ≈≈     |
| 22   | Qualia-bias seeding      | F0 structure biases gauge minimization path selection    | Initial "Felt Contrast" graph → coupling landscape | ≈≈     |
| 23   | Nested observer hierarchy| Agents compressing agents ⇒ MDL gain / complexity layers | Basis-aligned SUR sharing (T10)                   | ≈≈     |
| 24   | Ontological closure loop | SUR-shaped physics (T18+) regenerates F0 observers       | Global SUR fixed point implies loop stability      | ≈≈     |
| 25   | No-distinction limit     | Describing S₀ (Box 0) introduces contrast (`Δ_gen`)    | Gödel-style instability in IC logic (Box 0)      | ≈≈     |

## 3. The Two Paths to Reality: A Self-Locking Loop

### 3.1 Generative Path (F0 → T24)
Registered Contrast (F0) + Salience (T1) hits Bottleneck (T2, Box 2) → Compression (T3, Box 3) via SUR (T3a) → Patterns & Memory Graph (T4, Box 4) → Observer (T4.5) → World Partition & Layering (T5, Box 8) → Time & Metric (T6) → Op. Constraints (T6a, Box 5) → Hilbert Space (T7) → Born Rule (T8) → Projection (T9) → Consensus (T10) → Curvature (T11, Box 6) → Energy Analogue (T12) → Gauge/QFT/Cosmology (T13–T23, Box 7). Result: Observers who instantiate F0 (T24), closing the loop.

### 3.2 Collapse Path (T25 → F0)
This path shows that attempting to erase structure or reach the void state (S₀/T25) forces the re-emergence of contrast via the same SUR logic operating in reverse (optimizing *away* from featurelessness).

| From Tier | Assume structure is absent/uniform                   | Why state is unstable / costly under SUR               | What structure is forced next (Lower Tier) |
| :-------- | :--------------------------------------------------- | :--------------------------------------------------- | :--------------------------------------- |
| T24       | No F0 observers                                      | Loop broken, physics lacks grounding                 | T23 Nested Observers emerge              |
| T23       | No nested compression                                | Suboptimal global K                                  | T22 Qualia Bias (shared compression)     |
| T22       | No qualia seeding specific physics                   | Gauge choices arbitrary, higher K                    | T21 Comp. Irreducibility (patterns)      |
| T21       | All patterns fully compressible                      | Violates K bounds / infinite regress               | T20 Robust Codes (cost floor)            |
| T20       | No fault-tolerant codes                              | Unstable to noise D (Box 2)                          | T19 Stable Background (post-inflation)   |
| T19       | No inflation/structure seeds                         | Uniform state costly (high E for any prediction)     | T18 GR Equations (curvature needed)        |
| T18       | No GR / Cost-Curvature                               | Fails to explain large scale structure / SUR flow     | T17 SM Constants (λ_*≈137.036 fixed point)|
| T17       | No stable constants / plateaus                       | λ runs indefinitely, no stable scales              | T16 RG Flow required                     |
| T16       | No scale dependence / RG flow                        | Fails to link micro/macro physics                  | T15 Mode Factorization / QFT required    |
| T15       | No QFT / Mode Bundles                                | Cannot describe local excitations efficiently        | T13/14 Gauge Symmetry needed             |
| T13/14    | No Gauge Symmetry / Phase Freedom                    | Global phase tracking costly / redundant K           | T12 Energy Analogue (λ base)             |
| T12       | No conserved λ / Energy Analogue                     | Fails to link SUR cost to thermodynamics (Box 5)   | T11 Geometric Curve (metric base)        |
| T11       | No Info-Metric / Curvature                           | Cannot define path costs d_I (Box 4) consistently    | T10 Consensus Layer (shared basis)       |
| T10       | No Consensus / Shared Basis                          | Observers cannot efficiently compare models (high E) | T9 Projection (state selection)          |
| T9        | No Projection / Branch Pruning                       | Superpositions explode beyond capacity C (T2)        | T8 Born Rule (probability needed)        |
| T8        | No Born Rule / Probabilities                         | Cannot assign predictive weights efficiently (high E)| T7 Hilbert Space needed                  |
| T7        | No Hilbert Space Structure                           | Fails to satisfy Operational Constraints (T6a)       | T6a Operational Constraints required     |
| T6a       | No Op. Constraints (Reversibility, Additivity etc.)  | Suboptimal SUR cost (leaky/non-additive K)         | T6 Process Dynamics needed               |
| T6        | No Time Arrow / Metric d_I                           | Cannot order events or measure cost distance (Box 4)| T5 World Partition needed                |
| T5        | No Self/World Partition                              | Observer (T4.5) cannot model environment           | T4 Pattern Extraction required           |
| T4        | No Patterns / Self Cluster                           | Cannot predict / compress input stream (high K+E)    | T3 Compression required                  |
| T3        | No Compression / Memory                              | Violates Bottleneck C (T2)                           | T2 Bottleneck required                   |
| T2        | No Bottleneck / Infinite Capacity                    | Flattens Salience (T1)                               | T1 Phenomenology required                |
| T1        | No Salience / Memory Ref / Multiplicity              | Cannot support structured F0                         | T0 F0 (Registered Contrast)            |
| T0/T25    | No Contrast (S₀ / Void)                              | Unstable: Describing void creates contrast (Box 0)   | **F0 (Registered Contrast)**             |

### 3.3 Synthesis
The Generative Path (F0 → T24) builds structure from contrast via SUR.
The Collapse Path (T25 → F0) shows that eliminating contrast forces its re-emergence via SUR.
Reality operates as a self-consistent, resource-constrained informational loop (F0 ↔ T25) governed by SUR, where structure formation and the instability of featurelessness are two sides of the same coin.

## Appendix / Further Formalism (Outline- will build this out over time )

*   **Formal Proof Pack (Steps 0-4):** Details language, operator semantics, Δ-Factorisation proof, ΔCat ≅ FdHilb(ℂ) proof (snake fixed), SUR Lyapunov derivation, EFE derivation. *
*   Mapping of operational axioms (Hardy, CDP) to emergent SUR predicates.
*   SUR functional convergence proof details (Robbins-Monro application).
*   Detailed derivations for speculative tiers (T13+).
*   Formal Gödel-style argument for T25 instability (Box 0). [**TODO:** Add reference/location].
*   Discussion of Zeta Function connection (speculative).
*   Falsification points / Protocol E details.
