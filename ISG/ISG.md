**ISG**

1.  **Introduction and Purpose**
    This document describes the Integer Structure Grid (ISG), a derived conceptual tool for visualizing structural complexity within the framework of Informational Constructivism (IC). It is not an additional axiom of IC but rather arises naturally when representing the compositional structure of information built from irreducible primitives. The ISG provides a map to understand how structures balance novelty generation against self-reuse, offering insights into their potential cost profile under IC's resource constraints.
    Understanding the ISG assumes familiarity with core IC concepts:
    *   Δ<sub>gen</sub>: Introduction of a novel, irreducible distinction (primitive generator).
    *   Δ<sub>self</sub>: Reuse or self-application of an existing represented structure/code, potentially increasing exponents.
    *   Δ<sub>proj</sub>: Stabilization or efficient referencing of existing distinctions/codes, often by optimizing the internal representation (K) without generating new primitive instances or increasing maximal reuse depth (x, y). Operationally, this could involve finding shorter code descriptions, creating pointers/references, or eliminating redundancy between existing structures. Δ<sub>proj</sub> **typically does not change (x,y) because its goal is compression; exceptional Δ<sub>proj</sub> cascades that rewrite structure do move on the grid.**
    *   SUR Cost Ledger (L = K + λE): Balancing description length/complexity (K) against error/processing cost (E).
    *   Resource Constraints (C): Finite limits on memory, time, energy, etc.

2.  **Foundational Justification: Why Integers and Primes?**
    The use of integers and their prime factorization is not merely an analogy but emerges as the canonical representation for a core aspect of IC's structure generation:
    *   **IC's Basic Composition:** At its simplest level, IC involves generating irreducible distinctions (Δ_gen) and combining them. If this combination is associative and order-independent (commutative), the resulting mathematical structure is the free commutative monoid on the set of irreducible generators chosen by the observer.
    *   **Isomorphism:** Assuming a countable set of irreducible generators (a reasonable assumption for finite observers), the free commutative monoid on this set is mathematically isomorphic to the set of natural numbers greater than 1 under multiplication (ℕ_{>1}, ×).
        *   Each distinct irreducible generator (result of a unique type of Δ_gen) maps bijectively to a distinct prime number (pᵢ). **The bijection is not unique; any fixed mapping suffices and the grid is invariant up to relabel.**
        *   The commutative composition of generators maps directly to integer multiplication.
        *   The irreducibility of a generator maps to the primality of the corresponding integer.
    *   **Canonical Gödelisation:** Any specific set of irreducible generators can be relabelled using prime numbers without loss of structural information or change in the fundamental accounting under IC rules. Any specific bijection between the observer’s generator set and the primes produces an equivalent coding; the grid structure itself is invariant under such relabeling. Therefore, using (ℕ_{>1}, ×) is the minimal, lossless, and standard (Gödel-like) way to encode the structure of any system built via commutative composition of countable irreducibles.
    (Note: While the `RH.md` memo may offer independent IC-based arguments favouring ℕ, the algebraic isomorphism alone suffices to establish the legitimacy of using integers/primes for representing this compositional structure.)

3.  **Defining the Integer Structure Grid (ISG)**
    We associate representable structures built via commutative composition with integers n > 1. Domain is ℕ_{>1}; n=1 (empty multiset) represents ‘no structure’ and is omitted. Given the Fundamental Theorem of Arithmetic, any such integer has a unique prime factorization:
    n = p₁^e₁ \* p₂^e₂ \* ... \* pₖ^eₖ
    where pᵢ are distinct prime numbers (representing distinct irreducible generators) and eᵢ ≥ 1 are their exponents.
    From this factorization, we define two coordinates for the ISG:
    *   **x = max{e₁, e₂, ..., eₖ}: Maximal Reuse Depth.** The largest exponent among all prime factors in the factorization of n. **x ≥ 1.**
    *   **y = Σ eᵢ = e₁ + e₂ + ... + eₖ (Ω(n)): Total Primitive Instances.** The sum of all exponents, equivalent to the total number of prime factors counted with multiplicity. **y ≥ 1.**
    The **Integer Structure Grid (ISG)** is the set of all points (x, y) obtained from integers n > 1, plotted on a 2D lattice. Note that y ≥ x and **y ≥ k** (number of distinct primes). The first row of the grid consists of points where x = 1 (no factor reused more than once).

4.  **The Nature of the (x, y) Projection: Intentional Coarse-Graining**
    The mapping from a full structural description (represented by the exponent vector (e₁, e₂, ...) for primes p₁, p₂, ...) to the single point (x, y) is an **intentional coarse-graining**. It discards information about:
    *   Which specific generators (primes) are used.
    *   The detailed distribution of exponents, beyond the maximum and the sum.
    *   The number of distinct prime factors k = |{p₁, ..., pₖ}|.
    This projection is valid and useful **if and only if** the SUR cost L or the aspect of the system being analyzed is primarily sensitive to the maximal reuse depth (x) and the total count of primitive instances (y). If ledger cost depends on the number of distinct generators k, extend the projection to (x, y, k) or note explicitly that the present grid assumes uniform overhead per generator.
    Think of the ISG as a coarse phase diagram summarizing complexity profiles based on depth vs. breadth. When the identity of specific generators matters or when interactions introduce costs not captured by x and y alone, the full exponent vector or other richer descriptions must be employed.

5.  **Interpretation of Coordinates: Mapping to IC Operations and SUR Cost**
    The (x, y) coordinates capture aggregate properties relevant to IC operations and potentially the SUR cost ledger (L = K + λE, where **λ is the cost-weighting parameter** balancing description vs energy/error costs).
    *   **x (Maximal Reuse Depth):** Represents the deepest level of self-application (Δ_self) applied sequentially to any single irreducible generator (pᵢ) within the structure n. Reuse depth here means multiplicity of an irreducible generator in the factor multiset, not the depth of a run‑time call stack (**e.g. in a pointer-rich data structure K may rise with x faster than E**). If an implementation penalises algorithmic depth, add another coordinate or a tag. A high x indicates significant reuse of at least one component. Under specific cost model assumptions (e.g., where physical implementation makes deep repetition energetically costly or reduces reliability), x may correlate strongly with:
        *   Processing or energetic cost (λE), especially for iterative operations (e.g., E might scale non-linearly with x).
        *   Potential overhead in description length (K) for managing deep repetition.
        *   **Caveat:** When the cost λE is insensitive to repetition depth in the chosen physical model, the x coordinate becomes less predictive of the total SUR cost.
        *   **Handling Ties:** When several generators share the same maximum exponent, the current model treats them as equivalent. If split reuse carries a different cost, introduce x₂ = second‑largest exponent (or a full ordered exponent vector).
    *   **y (Total Primitive Instances):** Counts the total number of primitive building blocks used in the structure n. This includes the initial introduction of each distinct generator type (via Δ_gen) plus every subsequent reuse (via Δ_self) that contributes to the exponents. This count often directly reflects:
        *   The baseline description length (K) required to list the primitive constituents (e.g., K might have a term proportional to y).
    Therefore, the (x, y) coordinates provide a profile of a structure's assembly strategy in terms of depth of reuse vs. total component count, which corresponds to its general position within the SUR cost landscape, **given a specific cost model relating x and y to K and E.**

6.  **Mapping IC Operations to Grid Movements**
    Assuming distinct primes map to distinct irreducible Δ_gen events:
    *   **Primes (Point (1, 1)):** Represent structures created by a single Δ_gen event (n = p). Here x=1, y=1.
    *   **Adding a Distinct Prime (Δ_gen Composition):** Composing (n -> n * p') with a new, distinct prime p' corresponds to the move (x, y) -> (x, y+1). This increases total primitive instances `y` without changing maximal reuse depth `x`.
    *   **Applying Δ_self to a Generator:** Increasing the exponent of an existing prime factor pᵢ (eᵢ -> eᵢ + 1) corresponds to the move (x, y) -> (x', y+1), where x' is the new maximum exponent (x' = max(x, eᵢ+1)). This increases `y` by one and may increase `x`, **and can raise or lower K depending on representation efficiency.**
    *   **Projection and Refactoring (Δ_proj):** By definition, Δ_proj aims to optimize the representation (reduce K) or stabilize existing structures, typically *without* adding new primitive instances or increasing the maximal reuse depth. Therefore, Δ_proj itself does not correspond to a move that increments `x` or `y` on the ISG. Instead, its effect might be modelled as:
        *   Reducing the underlying K cost associated with a point (x, y).
        *   Increasing the *probability weight* or *relevance* (changing the count `N_n(x, y)` in the observer's distribution, see Section 9) associated with an existing point (x, y) if that structure becomes more predictively useful or efficiently represented.
        *   Facilitating complex **refactorings** that correspond to a path across the grid ultimately leading to a lower L state.
    **Inverse Mapping:** The mapping n -> (x, y) is unique. However, the inverse mapping from (x, y) to n is **many-to-one**. A single point (x, y) represents an exponent profile (a specific combination of reuse depth and total instance count), which can be realized by multiple integers using different prime labels (e.g., 12 = 2²3¹ and 18 = 2¹3² both map to (x=2, y=3)). The ISG visualizes the profile, not the fully specified structure.

7.  **Multiplication as Baseline Composition**
    Integer multiplication n₁ \* n₂ corresponds to concatenating the prime multisets of n₁ and n₂. If n₁ and n₂ share a prime factor p, their exponents simply add in the product, e_{n₁\*n₂}(p) = e_{n₁}(p) + e_{n₂}(p); this is still order-independent. In IC terms, multiplication represents the simplest, **minimal form of composition**:
    *   Commutative and Associative: The order of composition doesn't matter.
    *   Non-Interacting: Assumes the components of n₁ and n₂ simply co-exist in the resulting structure without introducing new interactions or dependencies that would alter the cost beyond the sum of parts. **If the factor sets are identical, composition is equivalent to a batch Δ_self on those generators.**
    This multiplication model captures the **baseline substrate** of structure building. When real systems involve:
    *   Ordered Composition: Use sequences, words, or tuples instead of multisets (requiring additional representational structure).
    *   Interactions/Dependencies: Add specific coupling terms to the SUR cost L, or represent links/relations with additional factors or annotations (e.g., via adjacency matrices alongside the ISG profile).
    Richer structures are built by adding constraints or information **on top** of the fundamental integer monoid backbone.

8.  **Example: Reading an Integer on the Grid**
    Consider n = 72 = 2³ \* 3².
    *   x = max(3, 2) = 3 (Maximal Reuse Depth)
    *   y = 3 + 2 = 5 (Total Primitive Instances)
    The point on the ISG is (3, 5).
    **IC Interpretation:** This structure's profile involves a maximal reuse depth (multiplicity) of 3 (applied to the generator '2') and requires a total of 5 primitive instances ('2', '2', '2', '3', '3'). The coordinate (3, 5) encapsulates this specific trade-off between reuse depth (potentially affecting E) and total instance count (affecting K), relevant to its SUR cost L.

9.  **Observers as Distributions on the ISG**
    An observer's memory state Sₙ at a given time can be visualized as a distribution Nₙ(x, y) over the ISG, where Nₙ(x, y) counts the number of structures (or their total weight/relevance) in memory that map to the point (x, y). **All formulas hold if N stores real weights instead of integer counts.** This distribution reveals the **observer's** current structural complexity profile.
    *   **Evolution:** The sequence N₀, N₁, N₂, ... depicts the evolution of the observer's internal complexity.
    *   **SUR Dynamics:** Tend to pull the distribution towards regions of lower cost L = K + λE. Depending on the specific cost model parameters (how K scales with y, how E scales with x and y, and the value of λ), this optimal region might favour low x and low y, or potentially higher y if deep reuse (high x) is heavily penalized. The accessible region is also constrained by the Ledger C limits (e.g., M bounds ΣN, τ bounds max x).
    *   **Concrete Cost Example:** Let K = αy and E = βx², where α represents the cost per primitive instance and β the cost scaling with squared maximal reuse depth. Then the total cost is L = αy + λβx². For example, if α = 1, β = 1, λ = 0.1, then the iso-cost contour for L=10 is defined by `y + 0.1 x² = 10`, a parabola opening leftward (y decreases as x increases). A point like (x=2, y=6) would have cost L = 1\*6 + 0.1\*1\*2² = 6.4. Observers under SUR would tend to populate regions intersected by the lowest possible iso-L contour accessible via IC operations.
    *   **Inputs/Processing:** External inputs (Δ_gen) or internal processing (Δ_self, Δ_proj) can shift the distribution, potentially pushing it towards higher complexity regions or refining weights within existing regions.

10. **Summary and Key Takeaways**
    *   **Canonical Basis:** The ISG uses integers/primes because (ℕ_{>1}, ×) is the canonical representation (via isomorphism) of the free commutative monoid generated by countable irreducible IC primitives (Δ_gen), invariant under relabeling.
    *   **SUR Profile:** The coordinates x (Max Reuse Depth/Multiplicity) and y (Total Primitive Instances) capture fundamental aspects of structural assembly relevant to the SUR cost L = K + λE, under specific cost model assumptions and caveats about the meaning of 'depth'.
    *   **Intentional Projection:** The map to (x, y) is a deliberate coarse-graining, valid when the SUR cost or analysis focuses primarily on these two aggregate measures (depth vs. breadth), potentially requiring extension to (x, y, k) if generator diversity is costly.
    *   **Baseline Composition:** Integer multiplication represents the minimal, order-independent, non-interacting composition within IC; more complex interactions require augmenting this model.
    *   **Visualization Tool:** The ISG provides a valuable conceptual grid for visualizing complexity profiles, comparing structures, and understanding the evolution of an observer's state under SUR dynamics and a given cost model.
    *   **Limitations:** **ISG fails when ordering or inter-component coupling dominates cost; then an ordered or graph-valued factorisation replaces plain integers.**
