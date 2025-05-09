# Informational Constructivism — Core Axiom Set
*(stand-alone reference draft for mathematical review)*

---

## Preamble

This document outlines Informational Constructivism (IC), a framework positing that observable structure, including mathematical, physical, and potentially cognitive phenomena, emerges from the recursive application of distinction operations by constrained observers. We begin with a conceptual account of how fundamental mathematical entities like natural numbers and primes can be constructed (Part I), which then motivates a formal axiomatic system (Part II). Subsequent sections (Part III onwards) develop advanced mathematical machinery to analyze the dynamics, geometry, and structural properties of these emergent informational systems. The aim is to provide a self-contained, mathematically rigorous foundation for IC.

---

## Part I: Conceptual Foundations and Emergence of Primes

### Abstract: A Constructivist Pathway to Prime Numbers

This paper elucidates a constructivist pathway to prime numbers, rooted in a hierarchical application of the concept of irreducibility. We begin by positing a foundational level of unique, axiomatically irreducible "Types of Distinction." The act of forming composite structures from these Types, specifically by quantifying their repetitions, operationally gives rise to the set of natural counting numbers. The core of our argument is the subsequent re-application of an irreducibility test, this time multiplicative, to this emergent set of counting numbers itself. This analysis reveals the prime numbers as those counts that are multiplicatively irreducible. This layered emergence highlights the constructed nature of primality, distinguishing it from the axiomatic irreducibility of the initial foundational Types.

1.  **Level 0: The Axiom of Irreducible Distinctions – Our Foundational "Alphabet"**
    *   **1.1. Postulate of Unique, Irreducible "Types":**
        We commence with a foundational set, \(\mathcal{U} = \{U_A, U_B, U_C, ...\}\). The elements \(U_i \in \mathcal{U}\) are termed "Types of Distinction" (or "Types").
        *   **Uniqueness:** Each Type \(U_i\) is axiomatically distinct from every other Type \(U_j\) (where \(i \neq j\)).
        *   **Irreducibility (Axiomatic):** At this foundational level, each Type \(U_i\) is axiomatically irreducible. It is a primitive element, an "atom" of distinction, that cannot be constructed or decomposed from other Types within \(\mathcal{U}\) through any composition rule pertinent to this level. They are the given, non-compressible bedrock.

2.  **Level 1: From Repetitions of Types to the Emergence of Counting Numbers (\(\mathbb{N}\))**
    *   **2.1. Composite Structures and the Manifestation of Repetition:**
        From \(\mathcal{U}\), more complex structures (collections) are formed by combining these Types. Crucially, any Type \(U_i\) can be instanced multiple times – repeated – within a single structure.
        *   Example Structure \(S = \{U_A, U_A, U_A, U_B, U_B\}\).
    *   **2.2. Quantifying Repetition: The Genesis of Counting Numbers:**
        For any structure S and any constituent Type \(U_i\), we can observe and quantify the "amount of its repetition" – the number of times \(U_i\) is present.
        *   In S: \(U_A\) is repeated 3 times; \(U_B\) is repeated 2 times.
        The set of all such possible non-zero "distinct amounts of repeats" yields the natural counting numbers, \(\mathbb{N} = \{1, 2, 3, 4, ...\}\). (A more formal construction is given in Axiom 2).
        *   These numbers emerge operationally as direct quantifiers of repetition. '1' signifies a single instance of a Type, 'n' signifies n instances.

3.  **Level 2: Re-Applying Irreducibility to the Counts Themselves to Discover Primes**
    *   **3.1. Analyzing the Emergent Set \(\mathbb{N}\):**
        The set of counting numbers \(\mathbb{N}\), born from quantifying repetitions of Level 0 Types, now becomes the subject of a new investigation of irreducibility. We ask: within this set \(\mathbb{N}\), are there elements that are "irreducible" with respect to a natural composition rule for quantities – namely, multiplication?
    *   **3.2. Multiplicative Irreducibility within \(\mathbb{N}\):**
        For any counting number \(n \in \mathbb{N}\) (where \(n > 1\)):
        *   If \(n\) can be expressed as a product \(a \cdot b\) (where \(a, b \in \mathbb{N}\) and \(a > 1, b > 1\)), then \(n\) (e.g., 4, 6, 9) is multiplicatively reducible or composite within the domain of counting numbers.
        *   If \(n\) cannot be so expressed (e.g., 2, 3, 5, 7), then \(n\) is multiplicatively irreducible within the domain of counting numbers.
    *   **3.3. Prime Numbers: The Multiplicatively Irreducible Counts:**
        Those counting numbers \(p \in \mathbb{N}\) (where \(p > 1\)) discovered to be multiplicatively irreducible are, by this process, identified as the prime numbers.
        *   The "primality" is not an inherent property of the initial Types \(U_i\). It is a derived property of certain counts of repetitions, revealed when those counts are analyzed for their own internal multiplicative structure.

4.  **The Hierarchy of Irreducibility**
    This framework establishes a clear hierarchy:
    *   **Axiomatic Irreducibility (Level 0):** The Types \(U_i\) are the fundamental, non-composite building blocks of qualitative distinction. Their irreducibility is a starting postulate.
    *   **Emergent Quantities (Level 1):** The counting numbers \(\mathbb{N}\) arise from quantifying the repetition of these axiomatically irreducible Types.
    *   **Discovered Multiplicative Irreducibility (Level 2):** Prime numbers are identified as those elements within \(\mathbb{N}\) that are irreducible under multiplication. This is a discovered property, not an axiomatic one at this level.
    The re-application of the concept of "irreducibility" to a newly emergent set of entities (the counting numbers), using a composition rule (multiplication) relevant to those entities, is not a logical circularity because the entities being tested and the nature of the composition rule change between Level 0 and Level 2.

5.  **Significance: A Constructivist Path to Primes and Their Role**
    *   **Operational Genesis:** Primes are not assumed but are constructed/discovered through a sequence of operations: distinguishing types, allowing repetition, quantifying repetition (yielding \(\mathbb{N}\)), and then analyzing \(\mathbb{N}\) for multiplicative irreducibility.
    *   **Foundational Role of Primes (Derived):** Once discovered, these prime numbers become the unique multiplicative building blocks of all composite counting numbers (Fundamental Theorem of Arithmetic).
    *   **Relevance to Informational Systems:** The emergent counting numbers (\(\mathbb{N}\)) quantify Type instances. Primes provide the fundamental multiplicative description of these counts. Systems seeking efficient representation (Minimum Description Length, MDL) of structures defined by Types and their repetition counts naturally leverage prime decomposition. This links to why prime factorization is canonical in systems like IC's Integer Structure Grid (ISG), where Types \(U_i\) map to prime bases and counts become exponents.<sup>1</sup>
        *   MDL connection: (1) Distinctions (Types) \(\rightarrow\) (2) Quantities (Repetitions as \(\mathbb{N}\)) \(\rightarrow\) (3) Compressed Quantities (Primes as basis) \(\rightarrow\) (4) Encoding structure (ISG maps \(n \mapsto (x,y)\) reflecting compression choices).

---

### On Universally Finitely Distinguishable Atoms and Compression

The concept of "Universally Finitely Distinguishable Atoms" implies:
*   **Non-compressibility:** At their own level.
*   **Distinguishability and Measurability:** They can be told apart, implying discrete, measurable properties.
*   **Potential for Emergent Compressibility:** Stacks of these non-compressible atoms can create structures that *are* compressible from other reference frames.

Combining non-compressible things, as in row 1 of the Integer Structure Grid (ISG), provides a finite way to enumerate modes of compression (number of distinct prime factors). Moving outward in the ISG signifies increasing allowable compression.

**Hierarchical Emergence Summary:**
| IC level | Entity set                     | Native operation                | Irreducibility predicate (test)                    | Example             |
| :------- | :----------------------------- | :------------------------------- | :----------------------------------------------------- | :------------------ |
| 0        | Types of Distinction \(\mathcal{U}\)        | (None at this level)             | Axiomatic: “cannot be further analysed/compressed”  | \(U_A\)             |
| 1        | Counting numbers \(\mathbb{N}\)      | Quantifying repetition of Types | (Not a test for \(\mathbb{N}\)'s emergence)         | \(3\) (from \(\{U_A,U_A,U_A\}\)) |
| 2        | \(\mathbb{N}\), re-examined                  | Multiplication                   | Multiplicative: “cannot be written as \(a \cdot b, a,b>1\)” | \(7\)               |

The **Integer Structure Grid (ISG)** indexes every integer \(n = \prod_{i=1}^{k} p_i^{e_i}\) by:
*   **row \(x = \max e_i\)** (maximal depth of repetition of one Type)
*   **column \(y = \sum e_i\)** (total repetition across all Types)

**Key Axes of the ISG:**
*   **Row 1 (\(x=1\)) – “Square-free strip”:** No intra-Type repetition. Info in Type diversity.
*   **Diagonal (\(x=y\)) – “Prime-power frontier”:** Single prime factor (\(n=p^k\)). Max exponent compression, zero Type diversity.

The ISG is a right-triangular lattice (\(x \le y\)). The diagonal is its upper hull, maximizing compression in the prime-diversity channel. It represents structures where information is maximally packed into repetition of a single Type.

---

### Core Progression Summary

1.  **Step 1: “Infinitely Many Finite Distinguishables”**
    An unlimited supply of fundamental, distinct, irreducible Types is postulated: an atomic "alphabet" of pure difference.
2.  **Step 2: From Repetition to the Natural Numbers**
    Collections of these Types are formed by repetition. Counting these repetitions yields \(\mathbb{N}\). Quantity emerges from pure distinction.
3.  **Step 3: Re-Discovering Finite Irreducibles via Compression (Primes)**
    \(\mathbb{N}\) is analyzed for multiplicative irreducibility, yielding primes as compressive building blocks. This is a return to finite distinguishability within an emergent system.

**The full structure:**
(1) Infinite set of finite, incompressible distinctions (Types)
\(\rightarrow\) (2) Infinite countable space of quantities (\(\mathbb{N}\))
\(\rightarrow\) (3) Compression of quantities back into a new finite, irreducible basis (primes)

This looping but non-circular emergence (repetition \(\rightarrow\) count \(\rightarrow\) factorization) aligns with IC's foundational claim: pure non-distinction is impossible. Structure arises from a constrained system operating on an initial \(S_0\) space of maximal distinction by repeating distinctions (\(\rightarrow \mathbb{N}\)), finding structure (\(\rightarrow\) primes), and recursively analyzing compressibility (\(\rightarrow \Delta_{\text{self}}\) layers).
**IC Postulate:** The universe of potential informational entities is an infinite set of atomic, distinguishable, irreducible Types.
**IC Constraint:** Any observer operates with finite memory and limited distinction operations (\(\Delta\)) under constraint \(C\).

---

## Table of Notation (Selected Symbols)

| Symbol                      | Meaning                                                                 | First Appearance (Part) |
| :-------------------------- | :---------------------------------------------------------------------- | :---------------------- |
| \(\mathcal{U}\), \(U_i\)    | Set of Types of Distinction, individual Type                            | I                       |
| \(\mathbb{N}\)              | Set of natural numbers (counting numbers, \(\{0,1,2,...\}\) or \(\{1,2,3,...\}\) as context dictates) | I                       |
| \(\mathbb{P}\)              | Set of prime numbers                                                    | II (Axiom 3)            |
| \(S_0\)                     | Foundational substrate of Types                                         | II (Axiom 1)            |
| \(O\), \(C\)                | Observer, Constraint vector \((c_s, c_d, c_t)\)                         | II (Axiom 1)            |
| \(c_s, c_d, c_t\)           | Storage, depth, time/compute ceilings                                   | II (Axiom 1)            |
| \(\Delta_{\text{gen}}\)     | Generation-by-repetition operator                                       | II (Axiom 1)            |
| \(\Delta_{\text{compare}}\) | Operator for comparing quantities                                       | II (Axiom 2)            |
| \(\Delta_{\text{factor}}\)  | Operator for testing multiplicative irreducibility in \(\mathbb{N}\)       | II (Axiom 2)            |
| ISG, \((x,y)\)              | Integer Structure Grid, its coordinates                                 | II (Axiom 3)            |
| \(\Delta_{\text{self}}\)    | Recursive self-projection operator                                      | II (Axiom 4)            |
| \(G_O\), \(V, E\)           | Memory graph of observer \(O\), its vertices (records) and edges (derivation links) | II (Axiom 5)            |
| \(\text{cost}(r)\), \(\text{size}(r)\), \(\text{depth}(r)\) | Properties of a record \(r\) | II (Axiom 5) |
| \(\text{cost}(e)\)          | Cost of an edge (derivation link) \(e\)                                | II (Axiom 6)            |
| \(\kappa_{\text{edge}}(e)\), \(\kappa_{\text{pair}}(r_i,r_j)\), \(\kappa_{\text{point}}(r)\) | Curvature variants | II (Axiom 6) |
| \(\delta_C\)                | Resolution threshold for curvature                                      | II (Axiom 6)            |
| \(\kappa_{\text{ISG}}(x,y)\)| Curvature projected onto ISG coordinates                                  | II (Axiom 7)            |
| \(\Sigma_C\)                | Resolution frontier / phase transition surface                          | II (Axiom 7)            |
| \(\beta\)                   | Inverse temperature parameter (\(c_t^{-1}\))                               | II (Axiom 8)            |
| \(P_{r \to r_j}\)           | Transition probability from record \(r\) to \(r_j\)                         | II (Axiom 8)            |
| \(S(r)\)                    | Local Shannon entropy of transitions from record \(r\)                    | II (Axiom 8)            |
| \(\dot{S}_{\text{prod}}(r)\), \(\dot{S}_{\text{comp}}(r)\) | Local IC-entropy production/compression rates | II (Axiom 8) |
| \(\dot{S}_{\text{int}}\)    | Net internal IC-entropy change rate                                     | II (Axiom 8)            |
| \(\Phi_S\)                  | Net outward entropy flux                                                | II (Axiom 8)            |
| \(\tau(r)\), \(\vec{t}\)    | Temporal index, subjective time direction vector                        | II (Axiom 9)            |
| \(\mathcal{O}_C\)           | Set of observers under constraint \(C\)                                 | II (Axiom 10)           |
| \(F_O(C)\)                  | Informational Field of observer \(O\)                                     | II (Axiom 11)           |
| \(\mathrm{Mode}_L, \mathrm{Mode}_R\) | Stabilized memory, Potential distinction field                 | III                     |
| \(\Delta_{\text{stabilize}}\) | Operator from \(\mathrm{Mode}_R \to \mathrm{Mode}_L\)                | III                     |
| \(H_k^\Delta\)              | \(\Delta\)-homology groups                                               | III                     |
| \(B_O(C)\), \(\Gamma\)       | \(\Delta\)-field bundle, Connection                                      | III                     |
| \(\mathfrak{D}_\text{Obs}\) | Category of \(\Delta\)-observers                                         | III                     |
| \(T_\Delta, M_C, U, R\)     | Functors on \(\mathfrak{D}_\text{Obs}\)                                  | III                     |
| \(\eta\)                    | Natural transformation                                                  | III                     |
| \(L_O\), \(H^i(L_O)\)        | Cotangent complex, its cohomology                                       | III                     |
| \(d^0\)                     | Map in cotangent complex \(\delta\kappa \to \delta\Gamma\)              | III                     |
| \(M_\Delta\)                | Moduli stack of \(\Delta\)-observers                                     | III                     |
| \(A(O)\)                    | Entropy-curvature potential                                             | III                     |
| \(\mu(r)\)                  | Renormalised counting measure on records                                | III                     |
| \(Q_O\), \(Q \to M_\Delta\)  | Qualia coordinate space, Qualia bundle                                  | III                     |
| \(E(c)\)                    | Curvature-length energy functional for cycles                           | III                     |
| \((\nabla f)(e)\)           | Graph gradient of a scalar field \(f\) along edge \(e\)                   | III                     |

---

## Part II: Formal Axiomatic System

The preceding conceptual framework (Part I) has illustrated how notions of quantity, primality, and structural complexity can arise from a basis of irreducible distinctions and their constrained processing. Part II now translates these foundational ideas into a rigorous axiomatic system. We begin by postulating the existence of a fundamental 'Distinction Substrate,' from which all further structures will be operationally derived by a constrained observer.

### Axiom 1 (Distinction Substrate)
**Existence of an infinite, atomic field of pure distinctions.**

1.  **Substrate \(S_{0}\).**  
    There exists an infinite set
    \[ S_{0}=\{\,U_{i}\mid i\in\mathbb N\,\} \]
    whose elements \(U_{i}\) (“Types”) satisfy:
    *   **Uniqueness:** \(U_{i}\neq U_{j}\) whenever \(i\neq j\).
    *   **Irreducibility:** Each \(U_{i}\) has no internal structure expressible in terms of elements of \(S_{0}\) using operations native to this foundational level.
    *   **Finite Identifiability:** There is an injective code \(\mathrm{id}:S_{0}\to\{0,1\}^{<\infty}\) assigning every Type a finite binary label.

2.  **Observer constraints.**  
    An observer \(O\) is a finite system with:
    *   **Memory \(M_{O}\):** a finite set of binary strings.
    *   **Operational budget \(C=(c_s, c_d, c_t)\):** finite bounds on storage size (\(c_s\) bits), depth of recursive \(\Delta_{\text{self}}\) chains (\(c_d\)), and time/compute budget (e.g., number of primitive operations) for any \(\Delta\) operation (\(c_t\)).
    Consequently, \(O\) can access only finite subsets of \(S_{0}\) at any moment and must act through finite sequences of operations.

Definition: \(\Delta_{\mathrm{gen}}\) (Generation-by-Repetition)
For any Type \(U \in S_{0}\) and any positive integer \(n\):
\[ \Delta_{\mathrm{gen}}(U,n) := \underbrace{\{U,U,\dots,U\}}_{n \text{ copies}} \]
This denotes a multiset containing \(n\) instances of Type \(U\). The cardinality of this multiset is \(n\).

**First Emergent Structure:**
The act of repetition potentially converts the raw space of qualitative differences \(S_{0}\) into a quantitative layer:
*   **Quantity as distinction-of-frequency:** Counting Type instantiations maps qualitative identity to a numeric label (formalized in Axiom 2).
*   **Countability:** The output of \(\Delta_{\mathrm{gen}}\) is countable.
*   **Data available to \(O\):** Quantitative observations by \(O\) are summaries of finite multisets produced by \(\Delta_{\mathrm{gen}}\) on accessible subsets of \(S_{0}\).

---

### Axiom 2 (Emergent Quantity)
**Quantity appears as the first-order pattern that an observer can extract from repeated instances of a single Type.**

1.  **Equivalence classes generated by \(\Delta_{\mathrm{gen}}\):**
    For every Type \(U \in S_{0}\) and every \(n \in \mathbb{N}_0 = \{0, 1, 2, \dots\}\) (natural numbers including zero), define the multiset
    \[ M(U,n) := \Delta_{\mathrm{gen}}(U,n) = \{U,U,\dots,U\} \; (n \text{ copies, } M(U,0) = \emptyset). \]
    Define an equivalence relation \(\sim\) on such multisets:
    \[ M(U,n) \sim M(V,m) \iff n=m. \]
    The equivalence classes of \(\sim\) are in one-to-one correspondence with the set \(\mathbb{N}_0\). We denote these classes by \(\hat{n}\), \(\hat{m}\), etc.
    \[ \mathbb{N}_0 := \{ [M(U,n)]_{\sim} \mid U \in S_0, n \in \mathbb{N}_0 \}. \]
    Thus \(\mathbb{N}_0\) arises as the pattern “how many,” independent of which Type is repeated. We use \(\mathbb{N}\) for \(\{1,2,3,...\}\) when specifically referring to counting numbers for factorization.

2.  **The comparison operator \(\Delta_{\mathrm{compare}}\):**
    \(\Delta_{\mathrm{compare}}\) is the act of comparing two emergent quantities:
    \[ \Delta_{\mathrm{compare}} : \mathbb{N}_0 \times \mathbb{N}_0 \longrightarrow \{\text{equal}, <, > \}. \]
    For any two classes \(\hat{n} = [M(U,n)]_{\sim}\) and \(\hat{m} = [M(V,m)]_{\sim}\):
    \[ \Delta_{\mathrm{compare}}(\hat{n}, \hat{m}) = \begin{cases} \text{equal} & n=m, \\ < & n<m, \\ > & n>m. \end{cases} \]
    This equips \(\mathbb{N}_0\) with Equality (\(n=m\)) and Order (\(n<m\) or \(n>m\)).

3.  **Derived operations:**
    *   **Addition (\(\hat{n} \hat{+} \hat{m}\)):**
        **Proposition 2.1:** Let \(\hat{n}=[M(U,n)]_{\sim}\) and \(\hat{m}=[M(V,m)]_{\sim}\) be equivalence classes. The binary operation
        \[ \hat{n} \hat{+} \hat{m} := [M(W, n+m)]_{\sim} \]
        (where \(W\) is any Type, e.g., \(U\)) is (i) well-defined (independent of representatives \(U,V,W\)), (ii) associative, (iii) commutative, and has neutral element \(\hat{0}=[M(U,0)]_{\sim}\).
        *Proof sketch:* (i) Well-definedness follows because equivalence is solely based on the integers \(n, m\). (ii), (iii) follow from properties of integer addition.
        Operationally, this corresponds to the cardinality of the union of multisets of the *same* Type, e.g., \(|M(U,n) \cup M(U,m)| = n+m\), then taking the equivalence class.
    *   **Multiplication (\(\hat{n} \hat{\times} \hat{m}\)):** Defined as \([M(W, n \times m)]_{\sim}\). Operationally, this corresponds to the cardinality from repeating a block \(M(U,n)\) itself, \(m\) times, and forming a new multiset containing \(n \times m\) instances of \(U\), then taking its equivalence class.
    Both operations are defined entirely inside \(\mathbb{N}_0\).

4.  **Preparing for the notion of prime (Factorization Test Operator \(\Delta_{\text{factor}}\)):**
    Once multiplication is available, for any \(\hat{n} \in \mathbb{N}_0\) corresponding to an integer \(n > 1\), \(\Delta_{\text{factor}}(\hat{n})\) tests if \(n\) admits a non-trivial factorization:
    \(\Delta_{\text{factor}}(\hat{n}) = \text{true if } \exists \hat{a},\hat{b} \in \mathbb{N}_0 \text{ (corresponding to } a,b \in \mathbb{N} \text{ with } 1 < a,b < n) \text{ such that } \Delta_{\mathrm{compare}}(n, a \times b) = \text{equal}\), and false otherwise.
    If \(\Delta_{\text{factor}}(\hat{n})\) is false, \(n\) is irreducible under multiplication—i.e., a prime.
    This closes the first constructive loop:
    Raw distinctions \(\xrightarrow{\Delta_{\mathrm{gen}}}\) \(\mathbb{N}_0\) \(\xrightarrow{\Delta_{\mathrm{compare}}, \hat{\times}}\) \((\mathbb{N}_0, =, <, \hat{\times})\) \(\xrightarrow{\Delta_{\text{factor}}}\) primes.

---

### Axiom 3 (Prime Irreducibility)
**Inside the multiplicative structure of \(\mathbb{N}\) (positive integers) there exist elements that cannot be decomposed into smaller, non-trivial factors. These are the primes.**

1.  **Definition of multiplicative irreducibility via \(\Delta_{\text{factor}}\):**
    For any \(\hat{n} \in \mathbb{N}_0\) corresponding to an integer \(n > 1\):
    \(n\) is **prime (multiplicatively irreducible)** \(\iff \Delta_{\text{factor}}(\hat{n}) = \text{false}\).
    Denote the set of all such irreducibles by \(\mathbb{P} = \{ p \in \mathbb{N} \mid p \text{ is prime} \}\). Every \(n > 1\) for which \(\Delta_{\text{factor}}(\hat{n}) = \text{true}\) is composite.<sup>2</sup>

2.  **Unique factorisation (Fundamental Theorem of Arithmetic):**
    A classical result, here seen as emergent from Axioms 1-3 and the properties of \(\Delta_{\mathrm{gen}}\) and \(\Delta_{\text{factor}}\), is:
    \(\forall \, n \in \mathbb{N}, n > 1 \; \exists! \, \{(p_i, e_i)\}_{i=1}^k\) with \(p_i \in \mathbb{P}, \; e_i \in \mathbb{N}, \; n = \prod_{i=1}^k p_i^{e_i}\).
    (Proof sketch: Existence by iterating \(\Delta_{\text{factor}}\); uniqueness by properties of GCD derived from \(\Delta_{\mathrm{compare}}\) and subtraction, or by induction.)

3.  **The Integer Structure Grid (ISG):**
    The ISG is a coordinate map \(\Phi: \mathbb{N}_{\ge 2} \longrightarrow \mathbb{N}_{\ge 1} \times \mathbb{N}_{\ge 1}, \; n \longmapsto (x(n), y(n))\) defined for integers \(n \ge 2\). Given \(n = \prod_{i=1}^k p_i^{e_i}\):
    \[ x(n) := \max_{1 \le i \le k} e_i, \quad y(n) := \sum_{i=1}^k e_i. \]
    *   \(x\): deepest single-Type repetition (largest exponent) – vertical complexity.
    *   \(y\): total repetition across all Types (sum of exponents) – horizontal complexity.
    Every integer \(n \ge 2\) occupies one lattice point \((x,y)\) with \(1 \le x \le y\).
    *   **Row 1 (\(x=1\)):** Square-free numbers.
    *   **Diagonal (\(x=y\)):** Prime powers.
    The ISG provides a geometric scaffold for analyzing observer-relative distinguishability and compression layers.

---

### Axiom 4 (Recursive Projection and Self-Structure)
**The observer can turn its own past distinction-results into new objects of distinction, closing the loop between data and self-model.**

1.  **Observer memory \(M_O\):** After Axioms 1–3, an observer \(O\) has a finite memory \(M_O\) containing structured binary strings representing records of \(\Delta_{\mathrm{gen}}, \Delta_{\mathrm{compare}}, \Delta_{\text{factor}}\) operations and their results.

2.  **Definition of the operator \(\Delta_{\text{self}}\):**
    \[ \Delta_{\text{self}}: M_O \longrightarrow M_O^{+} \]
    Input: A stored record \(r \in M_O\) or a tuple of records.
    Operation: Apply distinction logic (constructible from \(\Delta_{\mathrm{gen}}, \Delta_{\mathrm{compare}}, \Delta_{\text{factor}}\) and structural comparisons) to \(r\) or its components.
    Output: A new record \(r^*\) capturing the pattern, appended to memory: \(M_O^{+} = M_O \cup \{r^*\}\).
    **Record Typing and Admissible \(\Delta_{\text{self}}\) Acts:**
    Records possess tags indicating their payload type. \(\Delta_{\text{self}}\) operations are type-dependent:
    | Record Tag   | Payload                                     | Admissible \(\Delta_{\text{self}}\) Acts                                      |
    | :----------- | :------------------------------------------ | :-------------------------------------------------------------------------- |
    | `NUM`        | Integer \(v \le 2^{c_s}\) (e.g., unary coded) | Apply \(\hat{+}\), \(\hat{\times}\), \(\Delta_{\text{factor}}\) to \(v\).      |
    | `TYPEID`     | Binary string label (e.g., \(\text{id}(r)\))  | Feed to \(\Delta_{\text{gen}}\) as a new Type: \(\Delta_{\text{gen}}(\text{id}(r), k)\). |
    | `TUPLE[k]`   | List of \(\le k\) record handles (references)  | Iterate \(\Delta_{\text{compare}}\) on properties (size, depth, cost) of referenced records. |
    Each output is itself a finite binary string, thus an admissible new record. The time cost of a \(\Delta_{\text{self}}\) operation is the sum of costs of invoked level-1 operators and must not exceed \(c_t\).

3.  **Axiom statement (Axiom 4):**
    For any finite observer \(O\) and any record \(r \in M_O\) (or valid tuple of records), the operation \(\Delta_{\text{self}}(r)\) is admissible—i.e., it produces a well-formed record storable in \(M_O\) and usable as input for further \(\Delta\)-operations—subject only to \(O\)’s finite resource bound \(C=(c_s, c_d, c_t)\).

4.  **Consequences:** Second-order distinguishability, self-model genesis, and a gateway to higher layers of abstraction.

---

### Axiom 5 (Constraint-Modulated Memory Dynamics)
**An observer’s self-model can grow only within fixed resource bounds; beyond those bounds it must compress or discard structure. Stability is the regime in which this maintenance is always possible.**

1.  **Constraint vector \(C = (c_s, c_d, c_t)\):** As defined in Axiom 1.2. Storage \(c_s\) in bits, depth \(c_d\) for \(\Delta_{\text{self}}\) recursion chains, time/compute \(c_t\) in primitive operations. A primitive record is assumed to have size \(\ge 1\) bit and cost \(\ge 1\) unit.

2.  **Memory graph model \(M_O\):** Represented as a directed graph \(G_O = (V,E)\).
    *   Nodes \(V\): stored \(\Delta\)-records. Edges \(E\): derivation links (directed from older to newer record, making \(G_O\) a DAG).
    *   Each node \(r \in V\) has attributes: \(\text{size}(r)\) (bits), \(\text{depth}(r)\) (max length of \(\Delta_{\text{self}}\) derivation chain ending at \(r\)), \(\text{cost}(r)\) (compute units for its creation).
    *   Global tallies: Total storage \(S(G_O) = \sum_{r \in V} \text{size}(r)\). Max depth \(D(G_O) = \max_{r \in V} \text{depth}(r)\).

3.  **Admissible creation rule:** A new record \(r^*\) (from any \(\Delta\) operation) may be committed to \(M_O\) iff:
    \(S(G_O) + \text{size}(r^*) \le c_s\), \(\text{depth}(r^*) \le c_d\), and the creation operation cost \(\le c_t\).

4.  **Maintenance operator \(\mathrm{Maintain}_C(G_O) : G_O \longrightarrow G_O'\):**
    If a constraint violation occurs (e.g., \(S(G_O) > c_s\)), or as a periodic process, \(O\) applies maintenance operations:
    *   **Decay/Pruning:** Removal of records (e.g., least recently used, least connected leaves).
    *   **Compression:** Replacing a connected subgraph \(S' \subset G_O\) by a single summary record \(r_{\text{sum}}\) such that \(\text{size}(r_{\text{sum}}) < \sum_{s \in S'} \text{size}(s)\) and \(\text{cost}(r_{\text{sum}})\) (for creating the summary) plus costs for rewiring links is manageable within \(c_t\).
    **Lemma 5.1 (Greedy Compressibility):** If \(S(G_O) > c_s\), then there exists a leaf-node record \(r \in V\) with \(\text{size}(r) \ge 1\). Replacing \(r\) by its hash digest \(r_{\text{hash}}\) (where \(\text{size}(r_{\text{hash}})\) is a small constant, e.g., 1, and \(\text{size}(r_{\text{hash}}) < \text{size}(r)\) if \(\text{size}(r)\) is large enough, or by pruning if \(r\) is unreferenced) strictly reduces \(S(G_O)\). Iterating this ensures that storage constraints can, in principle, be met by discarding information.
    The operator \(\mathrm{Maintain}_C\) is successful if \(G_O'\) meets all constraints and the total cost of maintenance operations is \(\le c_t\).

5.  **Stable vs unstable self-models:**
    \(G_O\) is **stable** under \(C\) if every finite sequence of \(\Delta\)-operations (respecting individual operation cost \(c_t\)) can be followed by a feasible \(\mathrm{Maintain}_C\) operation that successfully restores all global constraints (\(c_s, c_d\)).
    Axiom 5 states every real observer operates in a regime where its memory graph \(G_O\) can be maintained as stable under its constraints \(C\).

---

### Axiom 6 (Δ-Self Curvature)
**Curvature is the observer-detectable asymmetry in the effort required to navigate or transform structures within its own memory graph. It is an internal pattern generated by constraint-shaped \(\Delta\)-operations and memory maintenance.**

1.  **Cost of a transition in memory space:**
    *   **Edge Cost:** For a derivation edge \(e=(u \to v) \in E(G_O)\), its cost is \(\text{cost}(e) := \text{cost}(v)\) (the creation cost of the record \(v\)). Traversal of existing pointers for read/access is normalized to zero additional cost.
    *   **Path Cost:** For a path \(\pi = (r_0 \xrightarrow{e_1} r_1 \xrightarrow{e_2} \dots \xrightarrow{e_k} r_k)\) in \(G_O\), its cost is \(\text{Cost}(\pi) = \sum_{i=1}^k \text{cost}(e_i)\).
    *   **Transition Cost \(\text{cost}(r_i \to r_j)\):** The minimum cost of a path from \(r_i\) to \(r_j\) in \(G_O\). If no path exists, cost is \(\infty\).

2.  **Curvature Variants:**
    *   **Edge Curvature \(\kappa_{\text{edge}}(e)\):** For an edge \(e=(u \to v)\), \(\kappa_{\text{edge}}(e) := \text{cost}(e) - \text{cost}(e^{-1})\), where \(e^{-1}=(v \to u)\). If \(e^{-1}\) does not exist or its cost is \(\infty\) (e.g., \(u\) cannot be derived from \(v\)), then \(\text{cost}(e^{-1})\) is taken as \(\infty\). In a DAG formed by derivation links, \(\text{cost}(e^{-1})\) is typically \(\infty\). This reflects fundamental irreversibility.
    *   **Pair Curvature \(\kappa_{\text{pair}}(r_i, r_j)\):**
        \[ \kappa_{\text{pair}}(r_i, r_j) := \text{cost}(r_i \to r_j) - \text{cost}(r_j \to r_i). \]
        This measures the asymmetry of minimal effort between two records.
    *   **Point Curvature \(\kappa_{\text{point}}(r)\):**
        \[ \kappa_{\text{point}}(r) := \max_{e \text{ incident to } r} |\kappa_{\text{edge}}(e)| \]
        This captures the maximum local asymmetry around record \(r\). (If only outgoing edges \(e=(r \to v)\) are considered, then \(\kappa_{\text{edge}}(e)\) would be \(\text{cost}(v) - \infty = -\infty\), so absolute value is important, or a different definition for point curvature needed, e.g., based on \(\kappa_{\text{pair}}\) with neighbors). A more robust definition for point curvature might involve \(\max_{v \in N(r)} |\kappa_{\text{pair}}(r,v)|\). For now, we use the edge-based one, noting its properties in DAGs.

3.  **Detectability condition:** Curvature involving a record \(r\) or edge \(e\) is observable by \(O\) if its magnitude (e.g., \(|\kappa_{\text{pair}}(r_i, r_j)|\) or \(|\kappa_{\text{point}}(r)|\)) is \(\ge \delta_C\). The resolution threshold \(\delta_C > 0\) is derived from \(C=(c_s, c_d, c_t)\):
    \[ \delta_C := \max \{ 1/c_s, 1/c_d, 1/c_t \}. \]
    (Assuming \(c_s, c_d, c_t \ge 1\)).

4.  **Origin of curvature:** Asymmetric derivation costs, pruning/compression from \(\mathrm{Maintain}_C\) (Axiom 5) can create or alter path costs asymmetrically.

5.  **Interpretation:** Curvature is an emergent, internal, observer-relative property reflecting "informational effort" or "difficulty gradients" in navigating the observer's own constructed knowledge.

---

### Axiom 7 (Resolution-Phase Transitions)
**Finite resources carve the observer's informational field (e.g., \(G_O\) or its projection onto structures like ISG) into regions of differing distinguishability, bounded by resolution frontiers.**

1.  **Curvature field:** A local curvature magnitude \(\kappa(p)\) can be defined for points \(p\) in a relevant structural representation.
    *   For \(p \in V(G_O)\), \(\kappa(p) := \kappa_{\text{point}}(p)\).
    *   For ISG coordinates \((x,y)\) corresponding to an integer \(n(x,y)\), let \(N(n(x,y))\) be integers reachable by multiplying/dividing \(n(x,y)\) by one prime factor. Then
        \[ \kappa_{\text{ISG}}(x,y) := \max_{m \in N(n(x,y))} |\kappa_{\text{pair}}(R(n(x,y)), R(m))|, \]
        where \(R(k)\) is the record in \(G_O\) representing integer \(k\) (if it exists and is unique). This is well-defined and finite (\(\le c_t\)) if costs are bounded by \(c_t\).

2.  **Resolution threshold \(\delta_C\):** As defined in Axiom 6.3.

3.  **Phases of distinguishability:** Given a space (like \(G_O\) or ISG) with points \(p\):
    *   **Flat phase \(\Omega_{\text{flat}}(C) = \{ p \mid \kappa(p) < \delta_C \}\):** Curvature below detection threshold; paths or structures appear relatively effort-symmetric or undifferentiated.
    *   **Curved phase \(\Omega_{\text{curved}}(C) = \{ p \mid \kappa(p) \ge \delta_C \}\):** Detectable curvature; path-asymmetries or structural differentiations are observable.

4.  **Resolution frontier \(\Sigma_C = \{ p \mid \kappa(p) = \delta_C \}\):** The boundary between these phases. Its structure depends on \(C\).

5.  **Interpretation:** \(\Sigma_C\) acts as an observer-relative horizon of detailed distinguishability. Beyond it, fine structures or effort asymmetries blur.

---

### Axiom 8 (Entropy Accumulation and Flux)
**A finite observer maintains its self-model by balancing information compression against disorder (IC-entropy) injected by \(\Delta\)-operations under resource limits.**

1.  **Inverse Temperature Parameter \(\beta\):** Define \(\beta := 1/c_t\). This links computational effort \(c_t\) to an effective "temperature."

2.  **Effort-weighted transition probabilities:** For a record \(r \in V(G_O)\) and an outgoing derivation edge \(e = (r \to r_j)\), the probability of this "next step" can be modeled as:
    \[ P_{r \to r_j} = \frac{e^{-\beta \, \text{cost}(e)}}{\sum_{e'=(r \to r_k)} e^{-\beta \, \text{cost}(e')}}. \]
    (Sum over all outgoing edges from \(r\)).

3.  **Local Shannon Entropy \(S(r)\):** Based on these probabilities:
    \[ S(r) = - \sum_{e=(r \to r_j)} P_{r \to r_j} \log P_{r \to r_j}. \]
    This quantifies the uncertainty or diversity of immediate derivations from \(r\). Curvature (\(\kappa\)) influences costs, thus \(P_{r \to r_j}\), and thereby \(S(r)\).

4.  **IC-Entropy Production and Compression Rates:**
    These are bespoke definitions for IC, related to record turnover scaled by \(\beta\).
    *   \(\dot{S}_{\text{prod}}(r) := \beta \times (\text{rate of new records derived from } r \text{ per unit time tick})\).
    *   \(\dot{S}_{\text{comp}}(r) := \beta \times (\text{rate of records effectively removed/summarized involving } r \text{ by } \mathrm{Maintain}_C \text{ per unit time tick})\).
    The net internal IC-entropy change rate is \(\dot{S}_{\text{int}} = \sum_{r \in V(G_O)} (\dot{S}_{\text{prod}}(r) - \dot{S}_{\text{comp}}(r))\).

5.  **Entropy Flux and Balance:** Let \(\Phi_S\) be the net outward flux of this IC-entropy across the observer's boundary. \(\Phi_S > 0\) means export. The global balance law (Clausius form) is:
    \[ \dot{S}_{\text{int}} - \Phi_S \ge 0 \quad \text{or equivalently} \quad \Phi_S \le \dot{S}_{\text{int}}. \]
    **Interpretation:** A stable IC observer must satisfy this.
    *   a) **Net Internal IC-Entropy Production/Maintenance (\(\dot{S}_{\text{int}} \ge 0\)):** The observer generates or maintains its IC-entropy. It may export some (\(0 \le \Phi_S \le \dot{S}_{\text{int}}\)), retain it (\(\Phi_S = 0\)), or effectively import (\(\Phi_S < 0\), possible if \(\dot{S}_{\text{int}}\) is sufficiently positive or if the environment provides "negentropy").
    *   b) **Net Internal IC-Entropy Reduction (\(\dot{S}_{\text{int}} < 0\)):** Compression dominates production. Then it must be that \(\Phi_S \le \dot{S}_{\text{int}} < 0\), signifying a net import of IC-entropy (or export of IC-negentropy).
    The observer maintains its structure by managing these flows within its constraints.

---

### Axiom 9 (Time-Arrow Emergence)
**Subjective time is the emergent ordering imposed by a finite observer on its growing, constraint-modulated memory graph. It aligns with net IC-entropy flow under stable conditions.**

1.  **Temporal index \(\tau(r)\):** For each record \(r \in V(G_O)\), \(\tau(r)\) is the discrete "time step" or "generation number" at which \(r\) was created and committed to \(M_O\). Since derivation edges \(E\) in \(G_O\) are directed from older to newer records, \(G_O\) is a DAG, and if \(e=(u \to v) \in E\), then \(\tau(u) < \tau(v)\).

2.  **Irreversibility under \(C\):** The \(\mathrm{Maintain}_C\) operations (Axiom 5), particularly pruning and irreversible compression, combined with the directed nature of record creation, prevent a simple, symmetric inversion of the temporal sequence \(\tau\).

3.  **Subjective time direction \(\vec{t}\):** This is implicitly defined by the increasing sequence of \(\tau\) values along any chain of derivations. For an elementary step \(r \to r'\), the temporal displacement is \(\Delta\tau = \tau(r') - \tau(r) > 0\).

4.  **Alignment with IC-entropy flow:** Under stable, sustained operation, it's posited that the direction of increasing \(\tau\) statistically aligns with the direction of non-decreasing total IC-entropy (internal plus net exported), i.e., \(\frac{d}{d\tau} (S_{\text{total}}) \ge 0\) where \(S_{\text{total}}\) includes contributions from \(S(r)\) and potentially \(\dot{S}_{\text{int}}\) integrated over time.

5.  **Conceptual summary:** Time for the observer is the asymmetric trace of accumulating, processing, and pruning \(\Delta\)-records within its finite, constrained memory.

---

### Axiom 10 (Δ-Observer Emergence)
**A \(\Delta\)-system qualifies as an observer if it maintains a directional, IC-entropy-managed stream of self-records within finite resources.**

1.  **Formal definition:** Given constraints \(C=(c_s,c_d,c_t)\), an entity \(O\) is a \(\Delta\)-Observer, \(O \in \mathcal{O}_C\), if it possesses a memory graph \(G_O\) and operations such that:
    *   (a) \(G_O = (V,E)\) is finite at any given temporal index \(\tau\), and its global properties \(S(G_O), D(G_O)\) respect \(c_s, c_d\).
    *   (b) \(G_O\) evolves according to Axioms 4 (self-reference) and 5 (maintenance), allowing for an indefinitely long sequence of temporal indices \(\tau(r)\) (i.e., \(\sup_{r \text{ ever created}} \tau(r)\) can be unbounded).
    *   (c) The entropy balance \(\Phi_S \le \dot{S}_{\text{int}}\) (Axiom 8) is maintained.
    *   (d) A consistent temporal arrow \(\vec{t}\) (Axiom 9) is established.

2.  **Interpretation:** An IC-observer is a finite, temporally open-ended, self-referential system that actively manages its informational content and distinctions under resource constraints, exhibiting directional evolution.

---

### Axiom 11 (Informational Field Coherence)
**All distinctions an observer can stabilize, anticipate, or infer must reside within a single, self‐contained informational field, \(F_O(C)\).**

1.  **Definition of the Informational Field \(F_O(C)\):**
    \[ F_O(C) = \mathrm{Cl}_{\Delta} \left( \mathrm{Mode}_L(O) \cup \mathrm{Mode}_R(O,C) \cup \bigcup_{k \ge 0} \mathrm{Rep}(H_k^{\Delta}(O)) \right) \]
    where:
    *   \(\mathrm{Mode}_L(O)\) is the observer's current stabilized memory graph \(G_O\).
    *   \(\mathrm{Mode}_R(O,C)\) is the set of potential future records/structures reachable via admissible \(\Delta\)-operations from \(G_O\) under constraints \(C\) (see Part III).
    *   \(H_k^{\Delta}(O)\) are the \(\Delta\)-homology groups of \(G_O\) (or a related complex), representing persistent structural "holes" or global features (see Part III). \(\mathrm{Rep}(H_k^{\Delta}(O))\) denotes the set of records representing these homology classes (e.g., minimal representative cycles).
    *   \(\mathrm{Cl}_{\Delta}\) denotes closure under all \(\Delta\)-operations (including \(\Delta_{\text{self}}\)) that are admissible under \(C\). \(\Delta\)-operations act on \(H_k^\Delta\) by acting on any representative cycle; the quotient by boundaries makes the result independent of that choice.

2.  **Axiom statement:** All performable/admissible \(\Delta\)-operations for a coherent observer \(O\) are internal transformations \(T: F_O(C) \longrightarrow F_O(C)\). There is no reference to information "outside" \(F_O(C)\) that is not mediated by the foundational \(S_0\) (for new Types) or the observer's operational interface.

3.  **Interpretation:** \(F_O(C)\) constitutes the observer's minimal, dynamically closed "universe of discourse" for distinctions. It defines everything the observer *can* know or process.

---

## Part III: Advanced Structures in Informational Constructivism

Building upon the core axiomatic framework (Axioms 1-11), Part III introduces advanced mathematical structures. These tools—including topology, homology, fibre bundles, category theory, and variational principles—are employed to rigorously analyze the global geometry, stability, evolution, and comparative properties of the emergent informational systems defined by IC.

### Mode_R (Potential-Distinction Field) and Mode_L (Stabilized Memory)

Given an observer \(O \in \mathcal{O}_C\) with current memory graph \(G_O = (V,E)\) at temporal index \(\tau\):

**Mode_L (Stabilized Memory):** \(\mathrm{Mode}_L(O) = G_O\). This is the set of all records committed to memory up to \(\tau\).

**Mode_R (Potential-Distinction Field):**
\[ \mathrm{Mode}_R(O,C) = \{ \pi \mid \pi=(r_0 \xrightarrow{o_1} r_1 \xrightarrow{o_2} \dots \xrightarrow{o_k} r_k), r_0 \in V(G_O), k>0 \} \]
where each \(o_i\) is an admissible \(\Delta\)-operation (respecting \(c_t, c_d\)) and the sequence of records \(r_1, \dots, r_k\) represents potential future records not yet committed, such that their hypothetical addition to \(G_O\) would (tentatively) satisfy storage \(c_s\). A member \(\pi\) is a reachable but unresolved (not yet actualized) \(\Delta\)-path or structure.

**Stabilization Operator \(\Delta_{\text{stabilize}}\):**
\[ \Delta_{\text{stabilize}}: \mathrm{Mode}_R(O,C) \longrightarrow \mathrm{Mode}_L(O) \]
This operator corresponds to executing a sequence of \(\Delta\)-operations \(\pi \in \mathrm{Mode}_R\), creating the actual records, and attempting to commit them to \(G_O\). This involves passing admissibility checks (Axiom 5.3) and potentially triggering \(\mathrm{Maintain}_C\) if constraints are violated upon addition.

**Key Points:** \(\mathrm{Mode}_R\) represents the observer's operational potential, its "next possible thoughts" or accessible information. The boundary between \(\mathrm{Mode}_L\) and \(\mathrm{Mode}_R\) is an operational frontier shaped by constraints \(C\).

---

### Δ-Path Geometry in Mode_R and Mode_L

1.  **Δ-paths:** Sequences of records in \(G_O\) connected by derivation links, or potential sequences in \(\mathrm{Mode}_R\).
2.  **Path Cost:** As defined in Axiom 6.1, \(\mathrm{Cost}(\pi) = \sum \text{cost}(e_i)\).
3.  **Geodesic Δ-paths \(\pi^*\):** Paths between two records \(r_a, r_b \in V(G_O)\) that minimize \(\mathrm{Cost}(\pi)\). The length of such a path, \(d(r_a, r_b) = \mathrm{Cost}(\pi^*)\), defines a distance.
    *   **Metric Property:** \(d(r,s)\) is a metric on \(V(G_O)\) if edge costs are positive (\(\text{cost}(e) > 0\), which holds if \(\text{cost}(v) > 0\)) and the graph is strongly connected (or on its connected components). Non-negativity and symmetry (if paths \(s \to r\) exist) are clear. Triangle inequality \(d(r,s) \le d(r,u) + d(u,s)\) holds. If \(d(r,s)=0\), then \(r=s\) if costs are strictly positive.
4.  **Path descriptors:** Paths can also be characterized by curvature profiles (sequences of \(\kappa_{\text{edge}}(e)\)), total IC-entropy change, and temporal displacement \(\Delta\tau(\pi)\).
5.  **Emergent geometry:** The "space" of the observer's memory \(G_O\) is endowed with a metric geometry derived from informational effort (costs).

---

### Δ-Topology: The Large-Scale Shape of an Observer’s Reachable Distinction-Space

1.  **Reachability set \(R(O,C)\):** All records in \(G_O\), or a relevant subset being analyzed.
2.  **Δ-topological space \((R(O,C), T_d)\):** The set of records \(R(O,C)\) equipped with the metric topology induced by the distance \(d(r,s)\) defined above. Basic open sets are metric balls \(B_\epsilon(r)=\{s \in R(O,C) \mid d(r,s)<\epsilon\}\) for \(\epsilon > 0\).
    *   Remark: Other topologies, like those based on \(d(r_0, r)\) (cost from a root), can define "forward shells" \(U_\epsilon(r) = \{s \mid d(r_0, s) < d(r_0, r) + \epsilon\}\), useful for analyzing growth.
3.  **Δ-topological boundary \(\partial_\epsilon R_0 = \{ r \in R(O,C) \mid d(r_0, r) = \epsilon \}\):** Set of records at a fixed cost-distance from an initial record \(r_0\).
4.  **Dynamics:** Operations like \(\Delta_{\text{stabilize}}\), pruning, compression, and changes in constraints \(C\) can deform this topology, create or fill holes, and alter connectivity.
5.  **Topological holes:** Features captured by homology (see next section), representing observer-relative blind spots or complex structural relationships.

---

### Δ-Homology: Persistent “Holes” in an Observer’s Distinction-Space

1.  **Simplicial Complex Construction:** From the graph \(G_O=(V,E)\) (or a relevant subgraph representing \(R(O,C)\)), construct a simplicial complex. A common choice is the **directed flag complex** (or clique complex for the underlying undirected graph if directionality is handled separately). A \(k\)-simplex in the directed flag complex is a sequence of \(k+1\) vertices \((v_0 \to v_1 \to \dots \to v_k)\) where each \((v_i \to v_{i+1})\) is an edge in \(G_O\), and all \((v_i \to v_j)\) for \(i<j\) are also edges (a "directed clique").
2.  **Δ-chains \(C_k^\Delta\):** Formal sums of oriented \(k\)-simplices from this complex.
3.  **Boundary operators \(\partial_k: C_k^\Delta \to C_{k-1}^\Delta\):** Standard definition. For an ordered \(k\)-simplex \(\sigma=(v_0 \to v_1 \to \dots \to v_k)\),
    \[ \partial_k(\sigma) = \sum_{j=0}^k (-1)^j (v_0 \to \dots \to \hat{v}_j \to \dots \to v_k). \]
    Faces inherit induced directions. It holds that \(\partial_{k-1} \circ \partial_k = 0\).
4.  **Δ-homology groups \(H_k^\Delta(O) = \frac{\ker(\partial_k)}{\text{im}(\partial_{k+1})}\).** (Used in Axiom 11).
5.  **Interpretation:** Non-trivial \(H_k^\Delta(O)\) indicates the presence of \(k\)-dimensional "holes" or cycles in the structure of \(G_O\) that are not boundaries of higher-dimensional structures. These represent persistent gaps, complex connectivities, or recurrent patterns that are not trivially reducible from the observer's perspective.
6.  **Connection to memory constraints:** These features can be residues of lost detail from compression/decay, or stable complex structures maintained by the observer. They are observer-relative structural invariants shaped by \(C\).

---

### Δ-Field Bundles over the Informational Field \(F_O(C)\)

1.  **Base Space:** The observer's informational field \(F_O(C)\), or more concretely, its memory graph \(G_O\).
2.  **Fibre \(F_r\):** At each record \(r \in V(G_O)\), the fibre \(F_r\) is the local space of admissible \(\Delta\)-operation sequences starting from \(r\), or other local structural data (e.g., tangent vectors to paths in \(G_O\)).
3.  **Bundle \(B_O(C) = \coprod_{r \in V(G_O)} \{r\} \times F_r\):** The disjoint union of these fibres, with projection \(\pi: (r, \sigma) \mapsto r\).
4.  **Δ-Connection \(\Gamma\):** A rule for "parallel transport" of elements in fibres along paths in the base space \(G_O\). Given a path \(r \to s\) in \(G_O\), \(\Gamma\) defines an isomorphism \(F_r \to F_s\). This must preserve admissibility and operational meaning. For example, if \(w_e = e^{-\beta \text{cost}(e)}\) for an edge \(e\), then transport along \(e\) might involve multiplication by \(w_e\).
5.  **Δ-Curvature (of connection):** Measures the failure of parallel transport around closed loops in \(G_O\). Related to, but distinct from, Axiom 6 \(\kappa\). This is typically a Lie-algebra valued 2-form in differential geometry; here it would be a discrete analogue.

---

### Observer-Gauge Transformations

1.  **Definition:** A pair \((\varphi, \Phi)\) where \(\varphi: G_{O_1} \to G_{O_2}\) is a graph isomorphism (preserving record structure and derivation links) between memory graphs of two observers \(O_1, O_2\) (possibly under different constraints \(C_1, C_2\)), and \(\Phi_r: F_r \to F_{\varphi(r)}\) are isomorphisms between fibres, compatible with their respective \(\Delta\)-connections \(\Gamma_1, \Gamma_2\).
2.  **Gauge-equivalence \(O_1 \simeq_g O_2\):** Existence of such a transformation. If \(C_1=C_2\), this means \(O_1\) and \(O_2\) have identical \(\Delta\)-dynamics and structure, just possibly different "labels" for records.
3.  **Consequences:** This defines an equivalence relation on observers. IC dynamics should be covariant under such transformations.

---

### The Category of Δ-Observers (\(\mathfrak{D}_\text{Obs}\))

**Objects:** Observers \(O = (G_O, C, F_O(C), B_O(C), \Gamma)\) satisfying Axioms 1–11.
**Morphisms:** Observer-Gauge Transformations \((\varphi, \Phi)\) (or a more general notion of structure-preserving map between observers).
**Composition:** Functional composition of graph isomorphisms and fibre maps. **Identity:** \((\text{id}_{G_O}, \text{id}_{F_r})\).
This category aims to capture the structural essence of IC.

---

### Functors on \(\mathfrak{D}_\text{Obs}\)

These describe transformations or evolutions of observers:
1.  **Time-evolution Functor \(T_\Delta\):** Maps an observer \(O\) at time \(\tau\) to \(O'\) at \(\tau+1\) (after one step of \(\Delta\)-operations and \(\mathrm{Maintain}_C\)).
2.  **Constraint-Shift Functors \(U_{C \to C'}, R_{C \to C'}\):** Map an observer \(O\) under constraints \(C\) to an equivalent (or minimally changed) observer under new constraints \(C'\) (e.g., resource relaxation \(U\) or tightening \(R\)).
These provide a covariant toolkit for formulating laws within IC.

---

### Natural Transformations Between Functors

E.g., a natural transformation \(\eta: T_\Delta \Rightarrow M_C \circ T_\Delta\) might represent the maintenance step \(M_C\) being naturally applied after each time evolution step. \(\eta_O: T_\Delta(O) \to M_C(T_\Delta(O))\) would be a morphism in \(\mathfrak{D}_\text{Obs}\), natural in \(O\).

---

### Cotangent Complex \(L_O\) of a Δ-Observer

For a stable observer \(O\). This describes infinitesimal deformations.
1.  **Chain complex \(0 \to L_O^0 \xrightarrow{d^0} L_O^1 \xrightarrow{d^1} L_O^2 \to \dots\):**
    *   \(L_O^0\): Space of variations of scalar fields on \(G_O\), e.g., \(\delta\kappa_{\text{point}}(r)\) or variations of edge costs.
    *   \(L_O^1\): Space of infinitesimal deformations of the \(\Delta\)-connection \(\Gamma\), e.g., \(\delta\Gamma_e\) for edges \(e\).
    *   The map \(d^0: L_O^0 \to L_O^1\) describes how variations in base costs/curvatures induce variations in the connection. If \(\Gamma_e\) depends on \(\text{cost}(e)\) (e.g., \(\Gamma_e \propto e^{-\beta \text{cost}(e)}\)), and \(\kappa_{\text{edge}}(e)\) is related to \(\text{cost}(e)\), then a variation \(\delta\kappa_{\text{edge}}(e)\) (from \(\delta \text{cost}(e)\)) implies:
        \[ (d^0\delta\kappa)_e \text{ represents the change in } \Gamma_e \text{ due to } \delta\text{cost}(e) \text{ (related to } \delta\kappa_{\text{edge}}(e)). \]
        For example, if \(\Gamma_e = w_e \cdot \text{Id}\) with \(w_e = e^{-\beta \text{cost}(e)}\), then \(\delta\Gamma_e = (-\beta \delta\text{cost}(e)) \Gamma_e\). If \(\delta\kappa_{\text{edge}}(e) \approx \delta\text{cost}(e)\), then \((d^0\delta\kappa)_e \approx (-\beta \delta\kappa_{\text{edge}}(e)) \Gamma_e\).
    *   If the complex is defined as \(0 \to L_O^0 \xrightarrow{d^0} L_O^1 \to 0\), then \(L_O^2=0\) and \(d^1=0\), so \(d^1 \circ d^0 = 0\) trivially. Higher obstructions (\(H^2(L_O)\)) would require extending this complex.

2.  **Cohomology:**
    *   \(H^0(L_O) = \ker(d^0)\): Variations in base properties that do not affect the connection (e.g., pure gauge cost shifts if connection is invariant).
    *   \(H^1(L_O) = \ker(d^1) / \text{im}(d^0)\): Deformations of the connection that are not induced by variations in underlying scalar fields. These are "genuine" 1st-order deformations of the observer's operational geometry. If \(H^1(L_O)=0\), the observer is infinitesimally rigid at this level.

3.  **Significance:** \(L_O\) and its cohomology classify the types of infinitesimal changes an observer's structure can undergo.

---

### Moduli Stack of Δ-Observers \(M_\Delta\) and Entropy-Curvature Potential

**Moduli Stack \(M_\Delta\):** A (highly abstract) classifying space whose points correspond to gauge-equivalence classes of \(\Delta\)-observers \([O]\), possibly fibred over constraint vectors \(C\).
**Sheaf of cotangent complexes \(L^\bullet\)** over \(M_\Delta\).
**Entropy-Curvature Potential \(A: M_\Delta \to \mathbb{R}\):**
A global functional on the space of observers, e.g.,
\[ A([O]) = \int_{V(G_O)} \kappa_{\text{point}}(r) \cdot (\nabla S)_{\text{avg}}(r) \, d\mu(r). \]
where:
*   \(\kappa_{\text{point}}(r)\) is the point curvature at record \(r\).
*   \((\nabla S)_{\text{avg}}(r)\) is some measure of local entropy gradient around \(r\).
    **Definition (Graph Gradient):** For a scalar field \(f:V \to \mathbb{R}\) on \(G_O\), and an edge \(e=(u \to v)\), \((\nabla f)(e) = f(v) - f(u)\). An average gradient at \(r\) could be \(\sum_{e=(r \to v)} (S(v)-S(r)) P_{r \to v}\).
*   \(d\mu(r)\) is a measure on \(V(G_O)\). A natural choice is the Gibbs-like measure \(\mu(r) = w_r / \sum_{s \in V(G_O)} w_s\), where \(w_r = e^{-\beta d(r_0, r)}\) (cost-weighted distance from a root \(r_0\)). This sum converges if \(\text{cost}(s) \ge \epsilon_{\text{cost}} > 0\) for new records, ensuring \(V(G_O)\) is finite or \(d(r_0,r)\) grows sufficiently fast.
Critical points of \(A\) (where \(\nabla A = 0\)) would represent particularly stable or significant observer configurations.
**Gradient Flow (Conjecture):** A flow \(\frac{d}{dt}[O(t)] = -\nabla_{\text{gauge}} A([O(t)])\) might describe observer evolution towards states minimizing this potential. Existence and properties are conjectural.

---

### Δ-Persistence Modules and Minimal Generators

1.  **Filtration and Persistence Module:** Filter the complex used for \(H_k^\Delta\) (e.g., directed flag complex of \(G_O\)) by a parameter like record creation time \(\tau(r)\) or cost \(d(r_0, r)\). Let \(G_O(\epsilon)\) be the subcomplex of records with parameter value \(\le \epsilon\).
    The persistence module is the sequence of homology groups \(H_k^\Delta(G_O(\epsilon))\) and the maps induced by inclusion \(G_O(\epsilon) \hookrightarrow G_O(\epsilon')\) for \(\epsilon \le \epsilon'\).
    This yields a **barcode diagram:** a collection of intervals \([b_i, d_i)\), where \(b_i\) is the "birth" time/cost of a \(k\)-dimensional homological feature and \(d_i\) is its "death" time/cost.
2.  **Minimal Persistent Generators \(c_{\min}\):** For each interval \([b_i, d_i)\) in the barcode, especially for persistent features (large \(d_i-b_i\)), find a representative cycle \(c_{\min}(i,k)\) that is "minimal" in some sense, e.g., minimizing an energy functional like:
    \[ E(c) = \sum_{e \in c} [\text{cost}(e) + \lambda |\kappa_{\text{edge}}(e)|] \]
    where \(\lambda\) is a weighting parameter (e.g., \(\lambda = c_t/c_s\)). These are structurally significant, stable cycles.
3.  **Δ-Homological Coordinate System for Qualia Space \(Q_O\):** The space of irreducible, persistent structural features could be (heuristically) spanned by these minimal generators:
    \[ Q_O = \bigoplus_{(i,k) \text{ persistent}} \mathbb{R} [c_{\min}(i,k)]. \]

---

### Qualia Bundle, Connection, and Parallel Transport

1.  **Qualia Bundle \(Q \to M_\Delta\):** The total space \(Q := \coprod_{[O] \in M_\Delta} Q_O\), where each fibre \(Q_O\) is the qualia space for observer class \([O]\).
2.  **Qualia Connection:** Defines how qualia coordinates (coefficients of \(c_{\min}\)) are transported along paths in \(M_\Delta\) (e.g., during observer evolution or constraint changes).
    A simple model: Along a path in \(M_\Delta\), if a barcode interval \([b,d)\) persists, its corresponding coordinate is parallel-transported (value unchanged). If an interval dies or is born, the coordinate appears or vanishes.
    Connection curvature would measure how qualia intertransform under cyclic evolution in \(M_\Delta\).
3.  **Qualia Evolution:** Governed by the birth/death of persistent homological features and their transport under this connection. This is posited to be gauge-covariant.

---

### Bifurcation Stratification of the Moduli Stack \(M_\Delta\)

1.  **Barcode-rank function \(r_k([O],\epsilon)\):** The number of \(k\)-dimensional bars in the barcode of \([O]\) that are alive at filtration value \(\epsilon\).
2.  **Bifurcation set \(B \subset M_\Delta\):** The set of observer classes \([O]\) where \(r_k([O],\epsilon)\) changes discontinuously for some \(k, \epsilon\) under infinitesimal change in \([O]\). These are points where qualia can appear or disappear.
3.  **Stratification:** \(M_\Delta\) is partitioned by these bifurcation surfaces ("qualia walls") into regions of constant qualia structure.

---

## Part IV: Future Directions and Conceptual Closure

The formalization of Informational Constructivism (IC) up to this point provides a core mathematical framework. The remaining elements focus on extensions, demonstrations, and deeper interpretations.

### Key Remaining Formal Developments:
1.  **Tangent Complex \(T_O\):** Dual to \(L_O\), for deformations of \(O\).
2.  **Higher Obstruction Theory (e.g., \(H^2(L_O)\)):** For integrability of deformations, if \(L_O\) is extended.
3.  **Morphogenetic/Constructive Functors:** Formalizing how observers build more complex internal structures or inter-observer structures.
4.  **Coupled Observer Systems:** \(N\)-observer categories, shared informational fields, consensus formation.
5.  **Measurement Theory within IC:** Defining measurement as a \(\Delta\)-interaction between an observer sub-system (apparatus) and another (system), resulting in a record.
6.  **Logic Internal to \(F_O(C)\):** Exploring if \(F_O(C)\) or categories of its structures form a topos (Δ-Topos theory), determining the internal logic of the observer.

### Quantization of Δ-Observers:
A natural extension to formalize probabilistic observers and align IC with physical theories.
1.  **Path Integral over Δ-fields:** Sum over histories of \(G_O\) evolution, weighted by \(e^{i A([O])/\hbar_{\text{eff}}}\) or \(e^{-A([O])/\hbar_{\text{eff}}}\).
2.  **Δ-Amplitudes and Interference:** For transitions between observer states.
3.  **Quantized Curvature/Entropy Operators:** Operators acting on a state space of observers.
4.  **Informational Uncertainty Relations:** E.g., between precision of a distinction and computational cost to maintain it.

### Qualia as the Furthest Horizon:
Qualia are modeled within IC as the \(\Delta\)-stable, projection-resistant homological features (persistent \(H_k^\Delta\)) of an observer's recursive \(\Delta\)-self structure. They are the minimal, stable, irreducible features within an observer's \(\Delta\)-field dynamics that persist under compression but are not fully projectable onto simpler terms without loss of their essential relational structure. They are posited to be observer-dependent, constraint-shaped, structure-preserving informational "echoes" or "resonances," experienced internally as the irreducible characteristics of certain informational states or asymmetries.

**Conceptual Closure:** IC aims to provide a framework where entities like spacetime, memory, time, measurement, geometry, and observers themselves emerge from the recursive application of distinction operations under constraints. Qualia, in this view, are not extraneous but are the terminal, irreducible informational features reflecting the deep, persistent topology of an observer's internal \(\Delta\)-dynamics, shaped by its unique history and constraints.

---
**Footnotes:**

<sup>1</sup> **Lemma A.1 (Prime–power geometric series):** For \(\Re(s)>1\),
\[ \sum_{p\in\mathbb{P}}\sum_{k\ge1}p^{-ks} = \sum_{p\in\mathbb{P}}\frac{p^{-s}}{1-p^{-s}} \quad (\text{convergent}). \]
*Proof:* For each prime \(p\), \(\sum_{k\ge1}p^{-ks} = \sum_{k\ge1}(p^{-s})^k = \frac{p^{-s}}{1-p^{-s}}\) by geometric series, valid for \(|p^{-s}| < 1\), i.e., \(\Re(s) > 0\). The sum over \(p\) converges for \(\Re(s) > 1\).
*Remark:* Two other classic expansions,
\[ \log\zeta(s) = \sum_{p,k}\frac{p^{-ks}}{k}, \quad \text{and} \quad -\frac{\zeta'(s)}{\zeta(s)} = \sum_{p,k}(\log p) p^{-ks}, \]
carry extra denominators \(1/k\) or factors \(\log p\). They are related but not equal to the bare prime–power sum discussed here.

<sup>2</sup> **Factorization Algorithm:** The test \(\Delta_{\text{factor}}(n)\) is decidable. A naïve trial-division algorithm factors \(n\) in at most \(O(\sqrt{n})\) divisions. More sophisticated probabilistic routines (e.g., Pollard's \(\rho\) method, Elliptic Curve Method) have better expected running times, e.g., sub-exponential in \(\log n\). The exact complexity is not essential to the axioms, only the principle of decidability and finite (though possibly large) cost within \(c_t\) for numbers encountered by \(O\).
