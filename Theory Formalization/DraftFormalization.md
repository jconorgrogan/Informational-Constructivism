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
        The set of all such possible non-zero "distinct amounts of repeats" yields the natural counting numbers, \(\mathbb{N} = \{1, 2, 3, 4, ...\}\).
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
**IC Constraint:** Any observer operates with finite memory and limited distinction operations (\(\Delta\) under constraint \(C\)).

---

## Table of Notation (Selected Symbols)

| Symbol                      | Meaning                                                                 | First Appearance (Part) |
| :-------------------------- | :---------------------------------------------------------------------- | :---------------------- |
| \(\mathcal{U}\), \(U_i\)    | Set of Types of Distinction, individual Type                            | I                       |
| \(\mathbb{N}\)              | Set of natural numbers (counting numbers)                               | I                       |
| \(\mathbb{P}\)              | Set of prime numbers                                                    | II (Axiom 3)            |
| \(S_0\)                     | Foundational substrate of Types                                         | II (Axiom 1)            |
| \(O\), \(C\)                | Observer, Constraint vector \((c_s, c_d, c_t)\)                         | II (Axiom 1)            |
| \(c_s, c_d, c_t\)           | Storage, depth, time/compute ceilings                                   | II (Axiom 5)            |
| \(\Delta_{\text{gen}}\)     | Generation-by-repetition operator                                       | II (Axiom 1)            |
| \(\Delta_{\text{compare}}\) | Operator for comparing quantities (was \(\Delta_{\text{proj}}\) on \(\mathbb{N}\)) | II (Axiom 2)            |
| \(\Delta_{\text{factor}}\)  | Operator for testing multiplicative irreducibility in \(\mathbb{N}\)       | II (Axiom 3)            |
| ISG, \((x,y)\)              | Integer Structure Grid, its coordinates                                 | II (Axiom 3)            |
| \(\Delta_{\text{self}}\)    | Recursive self-projection operator                                      | II (Axiom 4)            |
| \(G_O\)                     | Memory graph of observer \(O\)                                            | II (Axiom 5)            |
| \(\kappa(r_i, r_j)\)        | Curvature functional (cost asymmetry)                                   | II (Axiom 6)            |
| \(\delta_C\)                | Resolution threshold for curvature                                      | II (Axiom 6)            |
| \(\Sigma_C\)                | Resolution frontier / phase transition surface                          | II (Axiom 7)            |
| \(S(r)\)                    | Local entropy at record \(r\)                                           | II (Axiom 8)            |
| \(\Phi_S\)                  | Net entropy flux                                                        | II (Axiom 8)            |
| \(\tau(r)\), \(\vec{t}\)    | Temporal index, subjective time direction vector                        | II (Axiom 9)            |
| \(\mathcal{O}_C\)           | Set of observers under constraint \(C\)                                 | II (Axiom 10)           |
| \(F_O(C)\)                  | Informational Field of observer \(O\)                                     | II (Axiom 11)           |
| \(\mathrm{Mode}_L, \mathrm{Mode}_R\) | Stabilized memory, Potential distinction field                 | III                     |
| \(\Delta_{\text{stabilize}}\) | Operator from \(\mathrm{Mode}_R \to \mathrm{Mode}_L\) (was \(\Delta_{\text{proj}}^{\text{Mode}}\)) | III                     |
| \(H_k^\Delta\)              | \(\Delta\)-homology groups                                               | III                     |
| \(B_O(C)\), \(\Gamma\)       | \(\Delta\)-field bundle, Connection                                      | III                     |
| \(\mathfrak{D}_\text{Obs}\) | Category of \(\Delta\)-observers                                         | III                     |
| \(T_\Delta, M_C, U, R\)     | Functors on \(\mathfrak{D}_\text{Obs}\)                                  | III                     |
| \(\eta\)                    | Natural transformation                                                  | III                     |
| \(L_O\), \(H^i(L_O)\)        | Cotangent complex, its cohomology                                       | III                     |
| \(M_\Delta\)                | Moduli stack of \(\Delta\)-observers                                     | III                     |
| \(A(O)\)                    | Entropy-curvature potential                                             | III                     |
| \(Q_O\), \(Q \to M_\Delta\)  | Qualia coordinate space, Qualia bundle                                  | III                     |
| \(E(c)\)                    | Curvature-length energy functional for cycles                           | III                     |
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
    *   **Irreducibility:** Each \(U_{i}\) has no internal structure expressible in terms of elements of \(S_{0}\).
    *   **Finite Identifiability:** There is an injective code \(\mathrm{id}:S_{0}\to\{0,1\}^{<\infty}\) assigning every Type a finite binary label.

2.  **Observer constraints.**  
    An observer \(O\) is a finite system with:
    *   **Memory \(M_{O}\):** a finite set of binary strings.
    *   **Operational budget \(C=(c_s, c_d, c_t)\):** finite bounds on storage size (\(c_s\)), depth of recursive \(\Delta_{\text{self}}\) chains (\(c_d\)), and time/compute budget for any \(\Delta\) operation (\(c_t\)).
    Consequently, \(O\) can access only finite subsets of \(S_{0}\) at any moment and must act through finite sequences of operations.

Definition: \(\Delta_{\mathrm{gen}}\) (Generation-by-Repetition)
For any Type \(U \in S_{0}\) and any positive integer \(n\):
\[ \Delta_{\mathrm{gen}}(U,n) := \underbrace{\{U,U,\dots,U\}}_{n \text{ copies}} \]
The cardinality of this multiset is \(n\). Collecting the cardinalities of all such multisets yields the natural numbers \(\mathbb{N} = \{1,2,3,\dots\}\).

**First Emergent Structure:**
The act of repetition converts the raw space of qualitative differences \(S_{0}\) into a quantitative layer:
*   **Quantity as distinction-of-frequency:** Counting Type instantiations maps qualitative identity to a numeric label.
*   **Countability:** The output of \(\Delta_{\mathrm{gen}}\) is countable.
*   **Data available to \(O\):** Quantitative observations by \(O\) are summaries of finite multisets produced by \(\Delta_{\mathrm{gen}}\) on accessible subsets of \(S_{0}\).

---

### Axiom 2 (Emergent Quantity)
**Quantity appears as the first-order pattern that an observer can extract from repeated instances of a single Type.**

1.  **Equivalence classes generated by \(\Delta_{\mathrm{gen}}\):**
    For every Type \(U \in S_{0}\) and every \(n \in \mathbb{N}\), define the multiset
    \[ M(U,n) := \Delta_{\mathrm{gen}}(U,n) = \{U,U,\dots,U\} \; (n \text{ copies}). \]
    Define an equivalence relation \(\sim\) on such multisets:
    \[ M(U,n) \sim M(V,m) \iff n=m. \]
    The equivalence classes of \(\sim\) are in one-to-one correspondence with the set \(\mathbb{N}\).
    \[ \mathbb{N} := \{ [M]_{\sim} \mid M=M(U,n) \text{ for some } U,n \}. \]
    Thus \(\mathbb{N}\) arises as the pattern “how many,” independent of which Type is repeated.

2.  **The comparison operator \(\Delta_{\mathrm{compare}}\):**
    \(\Delta_{\mathrm{compare}}\) is the act of comparing two emergent quantities:
    \[ \Delta_{\mathrm{compare}} : \mathbb{N} \times \mathbb{N} \longrightarrow \{\text{equal}, <, > \}. \]
    For any two classes \([M(U,n)]_{\sim}, [M(V,m)]_{\sim}\):
    \[ \Delta_{\mathrm{compare}}([M(U,n)]_{\sim}, [M(V,m)]_{\sim}) = \begin{cases} \text{equal} & n=m, \\ < & n<m, \\ > & n>m. \end{cases} \]
    This equips \(\mathbb{N}\) with Equality (\(n=m\)) and Order (\(n<m\) or \(n>m\)).

3.  **Derived operations:**
    *   **Addition (\(n+m\)):** Operationally, the class from concatenating repetition-multisets: \(M(U,n) \cup M(U,m) \mapsto n+m\).
    *   **Multiplication (\(n \times m\)):** The class from repeating the block \(M(U,n)\) itself, \(m\) times: \( \underbrace{(M(U,n) \cup \dots \cup M(U,n))}_{m \text{ blocks}} \mapsto n \times m \).
    Both operations are defined entirely inside \(\mathbb{N}\).

4.  **Preparing for the notion of prime (Factorization Test Operator \(\Delta_{\text{factor}}\)):**
    Once multiplication is available, \(\Delta_{\text{factor}}\) tests if \(n > 1\) admits a non-trivial factorization:
    \(\Delta_{\text{factor}}(n) = \text{true if } \exists a,b \in \mathbb{N}, 1 < a,b < n \text{ such that } \Delta_{\mathrm{compare}}(n, a \times b) = \text{equal}\), and false otherwise.
    If \(\Delta_{\text{factor}}(n)\) is false, \(n\) is irreducible under multiplication—i.e., a prime.
    This closes the first constructive loop:
    Raw distinctions \(\xrightarrow{\Delta_{\mathrm{gen}}}\) \(\mathbb{N}\) \(\xrightarrow{\Delta_{\mathrm{compare}}, \times}\) \((\mathbb{N}, =, <, \times)\) \(\xrightarrow{\Delta_{\text{factor}}}\) primes.

---

### Axiom 3 (Prime Irreducibility)
**Inside the multiplicative structure of \(\mathbb{N}\) there exist elements that cannot be decomposed into smaller, non-trivial factors. These are the primes.**

1.  **Definition of multiplicative irreducibility via \(\Delta_{\text{factor}}\):**
    For any \(n \in \mathbb{N}\) with \(n > 1\):
    \(n\) is **prime (multiplicatively irreducible)** \(\iff \Delta_{\text{factor}}(n) = \text{false}\).
    Denote the set of all such irreducibles by \(\mathbb{P} = \{ p \in \mathbb{N} \mid p \text{ is prime} \}\). Every \(n > 1\) for which \(\Delta_{\text{factor}}(n) = \text{true}\) is composite.

2.  **Unique factorisation (Fundamental Theorem of Arithmetic):**
    A classical result, here seen as emergent from Axioms 1-3 and the properties of \(\Delta_{\text{gen}}\) and \(\Delta_{\text{factor}}\), is:
    \(\forall \, n > 1 \; \exists! \, \{(p_i, e_i)\}_{i=1}^k\) with \(p_i \in \mathbb{P}, \; e_i \in \mathbb{N}_{\ge 1}, \; n = \prod_{i=1}^k p_i^{e_i}\).
    (Proof sketch: Existence by iterating \(\Delta_{\text{factor}}\); uniqueness by properties of GCD derived from \(\Delta_{\text{compare}}\) and subtraction, or by induction.)

3.  **The Integer Structure Grid (ISG):**
    The ISG, conceptually introduced in Part I as a means to visualize compression patterns, is here formalized. A coordinate map \(\Phi: \mathbb{N}_{\ge 2} \longrightarrow \mathbb{N}_{\ge 1} \times \mathbb{N}_{\ge 1}, \; n \longmapsto (x(n), y(n))\) is defined. Given \(n = \prod_{i=1}^k p_i^{e_i}\):
    \[ x(n) := \max_{1 \le i \le k} e_i, \quad y(n) := \sum_{i=1}^k e_i. \]
    *   \(x\): deepest single-Type repetition (largest exponent) – vertical complexity.
    *   \(y\): total repetition across all Types (sum of exponents) – horizontal complexity.
    Every integer \(n \ge 2\) occupies one lattice point \((x,y)\) with \(1 \le x \le y\).
    *   **Row 1 (\(x=1\)):** Square-free numbers.
    *   **Diagonal (\(x=y\)):** Prime powers.

    **Why the ISG matters in IC:** It provides a geometric scaffold for analyzing observer-relative distinguishability, compression layers, recursion paths, and resolution transitions (see Axioms 5-8).

---

### Axiom 4 (Recursive Projection and Self-Structure)
**The observer can turn its own past distinction-results into new objects of distinction, closing the loop between data and self-model.**

1.  **Observer memory as first-order structure:**
    After Axioms 1–3, an observer \(O\) has a finite memory \(M_O \subseteq \{\text{finite records of } \Delta_{\text{gen}}, \Delta_{\text{compare}}, \Delta_{\text{factor}}\}\). Each record \(r \in M_O\) is a structured object.

2.  **Definition of the operator \(\Delta_{\text{self}}\):**
    \[ \Delta_{\text{self}}: M_O \longrightarrow M_O^{+} \]
    Input: A stored record \(r \in M_O\).
    Operation: Apply distinction logic (constructible from \(\Delta_{\text{gen}}, \Delta_{\text{compare}}, \Delta_{\text{factor}}\)) to \(r\) itself.
    Output: A new record \(r^*\) capturing the pattern, appended to memory: \(M_O^{+} = M_O \cup \{r^*\}\).

3.  **Axiom statement (Axiom 4):**
    For any finite observer \(O\) and any record \(r \in M_O\), the operation \(\Delta_{\text{self}}(r)\) is admissible—i.e., it produces a well-formed record storable in \(M_O\) and usable as input for further \(\Delta\)-operations (including another \(\Delta_{\text{self}}\))—subject only to \(O\)’s finite resource bound \(C=(c_s, c_d, c_t)\).

4.  **Consequences:**
    *   **Second-order distinguishability.**
    *   **Self-model genesis:** Iterating \(\Delta_{\text{self}}\) builds a graph of records-about-records.
    *   **Curvature / resolution feedback.**
    *   **Gateway to higher layers of abstraction.**

---

### Axiom 5 (Constraint-Modulated Memory Dynamics)
**An observer’s self-model can grow only within fixed resource bounds; beyond those bounds it must compress or discard structure. Stability is the regime in which this maintenance is always possible.**

1.  **Constraint vector \(C = (c_s, c_d, c_t)\):** (As defined in Axiom 1.2).

2.  **Memory graph model \(M_O\):** Represented as \(G_O = (V,E, \text{size}, \text{depth}, \text{cost})\).
    *   Nodes \(V\): stored \(\Delta\)-records. Edges \(E\): derivation links.
    *   Each node \(r \in V\) has weights: \(\text{size}(r)\), \(\text{depth}(r)\), \(\text{cost}(r)\).
    *   Global tallies: \(S(G_O) = \sum_{r \in V} \text{size}(r)\), \(D(G_O) = \max_{r \in V} \text{depth}(r)\).

3.  **Admissible creation rule:** A new record \(r^*\) may be committed iff:
    \(S(G_O) + \text{size}(r^*) \le c_s\), \(\text{depth}(r^*) \le c_d\), \(\text{cost}(r^*) \le c_t\).

4.  **Maintenance operator \(\mathrm{Maintain}_C(G_O) : G_O \longrightarrow G_O'\):**
    If violation occurs, \(O\) applies: Decay, Pruning, Compression.
    Successful if \(G_O'\) meets constraints and maintenance cost \(\le c_t\).

5.  **Stable vs unstable self-models:**
    \(G_O\) is **stable** under \(C\) if every finite sequence of \(\Delta\)-operations can be followed by feasible \(\mathrm{Maintain}_C\) restoring constraints.
    Axiom 5 states every real observer operates where \(\mathrm{Stable}(G_O,C)\) holds.

---

### Axiom 6 (Δ-Self Curvature)
**Curvature is the observer-detectable asymmetry in the effort required to move through its own memory graph. It is an internal pattern generated by constraint-shaped \(\Delta\)-operations.**

1.  **Cost of a transition in memory space:**
    For \(r_i, r_j \in V(G_O)\), \(\text{cost}(r_i \to r_j) = \min_{\pi} \left[ \sum_{k=0}^{|\pi|-1} \text{cost}(e_k) \right]\). (Remark: With pruning, edges can disappear, so \(\text{cost}(r_i \to r_j)\) can jump; it is upper semicontinuous under flows.)

2.  **Curvature functional \(\kappa: V \times V \longrightarrow \mathbb{R}\):**
    \[ \kappa(r_i, r_j) := \text{cost}(r_i \to r_j) - \text{cost}(r_j \to r_i). \]

3.  **Detectability condition:** Curvature at \((r_i, r_j)\) is observable by \(O\) iff \(|\kappa(r_i, r_j)| \ge \delta_C\), where \(\delta_C > 0\) is the resolution threshold from \(C=(c_s, c_d, c_t)\): \(\delta_C = \max \{ k_s/c_s, k_d/c_d, k_t/c_t \}\) for some observer-specific scaling constants \(k_s, k_d, k_t\), or simply related to inverse budget sizes (e.g., \(2^{-c_s}\) if \(c_s\) is bits).

4.  **Origin of curvature:** Maintenance rules (Axiom 5) can create path asymmetries.

5.  **Interpretation:** Curvature is emergent, internal, observer-relative. \(\kappa \neq 0\) implies “informational bends.”

---

### Axiom 7 (Resolution-Phase Transitions)
**Finite resources carve the observer's informational field (e.g., represented on ISG) into regions of differing distinguishability, bounded by resolution frontiers.**

1.  **Curvature field:** A local curvature magnitude can be defined over relevant structural representations (e.g., \(\kappa_{\text{ISG}}(x,y)\) for ISG, or more generally over \(G_O\)).

2.  **Resolution threshold \(\delta_C\):** (As defined in Axiom 6).

3.  **Phases of distinguishability:**
    *   **Flat phase \(\Omega_{\text{flat}}(C) = \{ \text{points } p \mid \kappa(p) < \delta_C \}\):** Paths appear effort-symmetric.
    *   **Curved phase \(\Omega_{\text{curved}}(C) = \{ \text{points } p \mid \kappa(p) \ge \delta_C \}\):** Path-asymmetry detectable.

4.  **Resolution frontier \(\Sigma_C = \{ \text{points } p \mid \kappa(p) = \delta_C \}\):**
    Boundary behavior depends on \(C=(c_s, c_d, c_t)\).

5.  **Informational-thermodynamic analogy:** Temperature \(\leftrightarrow \delta_C\). Phase boundary \(\leftrightarrow \Sigma_C\).

6.  **Observer-relative horizon:** \(\Sigma_C\) is a horizon of distinguishability.

---

### Axiom 8 (Entropy Accumulation)
**A finite observer maintains its self-model by balancing information compression against disorder injected by \(\Delta\)-operations under resource limits.**

1.  **Effort-weighted transition probabilities:** \(P_{r \to r_j} \propto e^{-\beta \, \text{cost}(r \to r_j)}\).

2.  **Local entropy \(S(r) = - \sum_{r_j \in N(r)} P_{r \to r_j} \log P_{r \to r_j}\).** (See Axiom 6 for \(\kappa\)).

3.  **Curvature drives entropy:** Path asymmetry \(|\kappa(r, r_j)|\) tends to increase local entropy \(S(r)\).

4.  **Resolution frontier and entropy flux:** Total entropy leaking across \(\Sigma_C\) is \(\Phi_S = \int_{\Sigma_C} (\nabla S \cdot \hat{n}) \, d\ell\).

5.  **Entropy–compression balance (equilibrium condition):**
    Local production \(\dot{S}_{\text{prod}}(r)\), local compression \(\dot{S}_{\text{comp}}(r)\).
    Equilibrium: \(\dot{S}_{\text{prod}}(r) - \dot{S}_{\text{comp}}(r) \le 0\) locally, and \(\int_{\Omega_{\text{flat}}(C)} (\dot{S}_{\text{prod}} - \dot{S}_{\text{comp}}) \, dA + \Phi_S \le 0\) globally.

---

### Axiom 9 (Time-Arrow Emergence)
**Subjective time is the emergent ordering imposed by a finite observer on its growing, constraint-modulated memory graph. It aligns with net entropy flow.**

1.  **Temporal index \(\tau: V(G_O) \longrightarrow \mathbb{N}\):** \(\tau(r) := \max_{\pi} |\pi|\) for paths from root \(r_0\).

2.  **Irreversibility under \(C=(c_s,c_d,c_t)\):** Maintenance (Axiom 5) prevents symmetric inversion of \(\tau\).

3.  **Subjective time direction \(\vec{t}(r)\):** Gradient of \(\tau\), \(\vec{t}(r \to r') = 1\).

4.  **Alignment with entropy flow:** At equilibrium (Axiom 8), \(\nabla S \cdot \vec{t} \ge 0\).

5.  **Conceptual summary:** Time is the asymmetric trace of accumulating/pruning \(\Delta\)-records.

---

### Axiom 10 (Δ-Observer Emergence)
**A \(\Delta\)-system qualifies as an observer if it maintains a directional, entropy-balanced stream of self-records within finite resources.**

1.  **Formal definition:** Given \(C=(c_s,c_d,c_t)\).
    \[ \mathcal{O}_C := \{ O \mid \text{(a) } G_O \text{ finite}; \text{ (b) } \exists \, \tau:V(G_O) \to \mathbb{N} \text{ with } \sup_r \tau(r) = \infty; \text{ (c) } \vec{t} \parallel \nabla S; \text{ (d) } \Phi_S \le 0 \}. \]
    (Conditions refer to Axioms 5, 8, 9).

2.  **Interpretation:** An IC-observer is finite, temporally open-ended, direction-aware, self-maintaining.

3.  **Conceptual summary:** Observers are emergent, temporal-distinction engines.

---

### Axiom 11 (Informational Field Coherence)
**All distinctions an observer can stabilize, anticipate, or infer must reside within a single, self‐contained informational field.**

1.  **Definition of the Informational Field \(F_O(C)\):**
    \[ F_O(C) = \mathrm{Cl}_{\Delta} \left( \mathrm{Mode}_L(O) \cup \mathrm{Mode}_R(O,C) \cup \bigcup_{k \ge 0} H_k^{\Delta}(O) \right) \]
    (\(\mathrm{Cl}_{\Delta}\) = closure under admissible \(\Delta\)-ops respecting \(C\). \(H_k^{\Delta}(O)\) are \(\Delta\)-homology classes for \(O\), see Part III).

2.  **Axiom statement:** All performable/admissible \(\Delta\)-operations for a coherent \(O\) are internal transformations \(T: F_O(C) \longrightarrow F_O(C)\). No reference outside \(F_O(C)\).

3.  **Interpretation:** \(F_O(C)\) is \(O\)'s minimal closed universe of distinctions.

---

## Part III: Advanced Structures in Informational Constructivism

Building upon the core axiomatic framework (Axioms 1-11), Part III introduces advanced mathematical structures. These tools—including topology, homology, fibre bundles, category theory, and variational principles—are employed to rigorously analyze the global geometry, stability, evolution, and comparative properties of the emergent informational systems defined by IC.

### Mode_R (Potential-Distinction Field) and Mode_L (Stabilized Memory)

Given an observer \(O \in \mathcal{O}_C\) with current memory graph \(G_O\):

**Mode_R (Potential-Distinction Field):**
\[ \mathrm{Mode}_R(O,C) = \{ \pi \mid \pi=(r_0 \to \dots \to r_k), r_0 \in V(G_O), k>0, \text{path } \pi \text{ admissible under } C=(c_s,c_d,c_t) \} \]
A member \(\pi\) is a reachable but unresolved \(\Delta\)-path.

**Mode_L (Stabilized Memory):** \(\mathrm{Mode}_L(O) = G_O\).

**Stabilization Operator \(\Delta_{\text{stabilize}}\):**
\[ \Delta_{\text{stabilize}}: \mathrm{Mode}_R(O,C) \longrightarrow \mathrm{Mode}_L(O) \]
Executes \(\pi \in \mathrm{Mode}_R\), appending new records to \(G_O\) if Axiom 5 admissibility holds.

**Key Points:** \(\mathrm{Mode}_R\) is operational potential. \(\mathrm{Mode}_R / \mathrm{Mode}_L\) boundary is a constraint-induced operational frontier.

---

### Δ-Path Geometry in Mode_R

1.  **Δ-paths:** Admissible sequences of operations starting from \(G_O\), respecting \(C=(c_s,c_d,c_t)\).
2.  **Path descriptors:** Curvature profile \(\kappa(\pi)\) (Axiom 6), entropy increment \(\Delta S(\pi)\) (Axiom 8), temporal displacement \(\Delta \tau(\pi)\) (Axiom 9).
3.  **Geodesic Δ-paths \(\pi^*\):** Minimize cost functional \(\mathrm{Cost}(\pi) = \sum \text{cost}(r_i \to r_{i+1})\).
4.  **Emergent geometry:** Distance = \(\mathrm{Cost}(\pi^*)\). Effective metric from \(G_O, C\).
5.  **Insight:** "Space" is information-access landscape.

---

### Δ-Topology: The Large-Scale Shape of an Observer’s Reachable Distinction-Space

1.  **Reachability set \(R(O,C)\):** All records reachable by admissible \(\Delta\)-paths.
2.  **Cost radius \(d(r)\):** Min cost from \(r_0\) to \(r\).
3.  **Δ-topological space \((R, T_\epsilon)\):** Base open sets \(U_\epsilon(r) = \{ s \in R \mid d(s) - d(r) < \epsilon \}\).
4.  **Δ-topological boundary \(\partial_\epsilon = \{ r \in R \mid d(r) = \epsilon \}\).**
5.  **Dynamics:** Pruning/compression/constraint changes deform topology, create/fill holes.
6.  **Topological holes:** Observer-relative blind spots.
7.  **Payoff:** Topology encodes accessible structure-space.

---

### Δ-Homology: Persistent “Holes” in an Observer’s Distinction-Space

1.  **Δ-chains \(C_k^\Delta\):** Formal sums of \(k\)-simplices (\(\Delta\)-path cycles).
2.  **Boundary operators \(\partial_k: C_k^\Delta \to C_{k-1}^\Delta\).** \(\partial_k \circ \partial_{k+1} = 0\).
3.  **Δ-homology groups \(H_k^\Delta(O) = \frac{\ker(\partial_k)}{\text{im}(\partial_{k+1})}\).** (Used in Axiom 11).
4.  **Interpretation:** Non-trivial \(H_k^\Delta(O)\) indicates unfillable distinction loops (persistent gaps/voids).
5.  **Connection to memory:** Residue of lost detail from compression/decay.
6.  **Blind spots/scars:** Observer-relative inaccessibilities imposed by \(C=(c_s,c_d,c_t)\).
7.  **Summary:** Algebraic quantification of deep, persistent inaccessibilities.

---

### Δ-Field Bundles over the Informational Field \(F_O(C)\)

1.  **Bundle construction:** Fibre \(F_r\) = local space of admissible \(\Delta\)-op sequences from \(r\).
    Bundle \(B_O(C) = \coprod_{r \in F_O(C)} \{r\} \times F_r\), \(\pi: (r, \sigma) \mapsto r\).
2.  **Local triviality:** \(\pi^{-1}(U) \cong U \times F\) for open \(U \subset F_O(C)\).
3.  **Δ-connections \(\Gamma\):** Rules for operational parallel transport, preserving admissibility and path functoriality.
4.  **Δ-curvature (of connection):** \(F: \ell \mapsto (\sigma \mapsto \Omega(\ell, \sigma) - \sigma)\), failure of transport around loops. (Related to Axiom 6 curvature).
5.  **Gauge equivalence:** Isomorphism of bundles preserving base space, fibres, and connections.

---

### Observer-Gauge Transformations

1.  **Definition:** Pair \((\varphi, \Phi)\) where \(\varphi: F_{O_1}(C_1) \to F_{O_2}(C_2)\) is base-space isomorphism, \(\Phi_r: F_r \to F_{\varphi(r)}\) are fibre bijections, compatible with connections.
2.  **Gauge-equivalence \(O_1 \simeq_g O_2\):** Existence of such transformation. Identical \(\Delta\)-dynamics.
3.  **Consequences:** Equivalence relation. IC dynamics covariant.

---

### The Category of Δ-Observers (\(\mathfrak{D}_\text{Obs}\))

**Objects:** \(O = (F_O(C), B_O(C), \Gamma)\) satisfying Axioms 1–11.
**Morphisms:** Observer-Gauge Transformations \((\varphi, \Phi)\).
**Composition:** Functional composition. **Identity:** \((\text{id}, \text{id}_r)\).
Captures IC's structural core.

---

### Functors on \(\mathfrak{D}_\text{Obs}\)

1.  **Time-evolution \(T_\Delta\):** \(\Delta\)-step + maintenance.
2.  **Δ-maintenance \(M_C\):** Pruning/compression to restore strict constraints.
3.  **Constraint-shift \(U_{C \to C'}, R_{C \to C'}\):** Resource relaxation/tightening.
Covariant toolkit for IC laws.

---

### Natural Transformations Between Functors

E.g., \(\eta: T_\Delta \Rightarrow M_C \circ T_\Delta\) (expand then clean cognitive micro-cycle).
\(\eta_O: T_\Delta(O) \to M_C(T_\Delta(O))\) is natural bundle projection. Gauge-invariant.

---

### Cotangent Complex \(L_O\) of a Δ-Observer

For stable \(O=(F_O(C), B_O(C), \Gamma)\).
1.  **Chain complex \(0 \to L_O^0 \xrightarrow{d^0} L_O^1 \to 0\):**
    *   \(L_O^0\): Curvature-gradient variations \(\delta\kappa\).
    *   \(L_O^1\): Infinitesimal connection deformations \(\delta\Gamma\).
    *   \(d^0\): Map from \(\delta\kappa\) to induced \(\delta\Gamma\).
2.  **Cohomology:** \(H^0(L_O)\) = pure gauge cost shifts. \(H^1(L_O)\) = persistent 1st-order operational geometry deformations. If \(H^1=0\), infinitesimally rigid.
3.  **Functoriality:** \(L_O\) is contravariant functor \(L^\bullet: \mathbf{\Delta Obs}^{\text{op}} \longrightarrow \mathbf{Ch}^+(\mathbf{Ab})\).
4.  **Significance:** \(L_O\) is dual to tangent space of moduli space. \(H^1(L_O)\) = informational moduli.

---

### Moduli Stack of Δ-Observers \(M_\Delta\) and Entropy-Curvature Potential

**Moduli Stack \(M_\Delta\):** Classifying space of gauge-equivalence classes of \(\Delta\)-observers, fibred over constraint vectors \(C\).
**Sheaf of cotangent complexes \(L^\bullet\)** over \(M_\Delta\).
**Entropy-Curvature Potential \(A: M_\Delta \to \mathbb{R}\):**
\[ A(O) = \int_{F_O(C)} \kappa(r) \cdot \nabla S(r) \, d\mu. \]
(Assumption: \(A\) is \(C^2\) on each stratum of \(M_\Delta\) and continuous across codimension-1 walls.)
Critical points of \(A\) are geometrically stable configurations.
**Gradient Flow:** Defined via \(L^2\)-type inner product on \(L_O^1\). Flow \(\frac{d}{dt}\Gamma(t) = -\nabla_g A_{O(t)}\). Gauge-equivariant.

---

### Δ-Persistence Modules and Minimal Generators

1.  **Filtration and Persistence Module:** Filter reachability \(R_\epsilon\) by cost \(\epsilon\). Module \(H_k^\Delta(\epsilon) := H_k^\Delta(R_\epsilon)\) gives \(\Delta\)-persistence barcode.
2.  **Minimal Persistent Generators \(c_{\min}\):** For each barcode interval, representative cycle minimizing curvature-length energy \(E(c) = \sum_{e \subset c} [\text{cost}(e) + \lambda |\kappa(e)|]\). (Note: \(\lambda\) can be set to 1 for simplicity or be an observer-specific parameter, e.g., \(\lambda \approx c_t/c_s\), reflecting resource trade-offs.)
3.  **Δ-Homological Coordinate System for Qualia Space \(Q_O = \bigoplus_{(i,k)} \mathbb{R} [c_{\min}(i,k)]\).**

---

### Qualia Bundle, Connection, and Parallel Transport

1.  **Qualia Bundle \(Q \to M_\Delta\):** Total space \(Q := \coprod_{O \in M_\Delta} Q_O\).
2.  **Qualia Connection:** Horizontal lift of entropy-curvature flow \(V_A(O)\) to \(Q\).
    Coordinates \(q_i\) tied to surviving barcodes are parallel-transported (\(\dot{q}_i=0\)). At barcode death \(\epsilon_d\), \(q_i \to 0\). (Remark: Jump-wise coordinate death is mathematically simple; smoother alternatives might involve stratified bundles and Stokes-like discontinuities.)
    Connection curvature along flow is zero.
3.  **Qualia Evolution:** Piecewise-constant magnitudes; changes only at barcode birth/death. Gauge-covariant.

---

### Bifurcation Stratification of the Moduli Stack \(M_\Delta\)

1.  **Barcode-rank function \(r_k(O,\epsilon)\).**
2.  **Bifurcation set \(B \subset M_\Delta\):** Observers where \(\frac{d}{dt}r_k(O(t),\epsilon)|_{t=0} \neq 0\).
3.  **Local normal form:** \(B\) is codim-1 hypersurface.
4.  **Stability spectrum:** From Hessian of \(A\). \(\lambda_\perp < 0 \implies\) supercritical stable. \(\lambda_\perp > 0 \implies\) subcritical unstable.
5.  **Stratification:** \(M_\Delta\) partitioned by "qualia walls."

---

## Part IV: Future Directions and Conceptual Closure

The formalization of Informational Constructivism (IC) up to this point provides a core mathematical framework. The remaining elements focus on extensions, demonstrations, and deeper interpretations.

### Key Remaining Formal Developments:
1.  **Tangent Complex \(T_O\).**
2.  **Higher Obstruction Theory (\(H^2(L_O)\)).**
3.  **Morphogenetic/Constructive Functors.**
4.  **Coupled Observer Systems.**
5.  **Measurement Theory within IC.**
6.  **Logic Internal to \(F_O(C)\) (Δ-Topos theory).**

### Quantization of Δ-Observers:
A natural extension to formalize probabilistic observers and align IC with physical theories.
1.  **Path Integral over Δ-fields.**
2.  **Δ-Amplitudes and Interference.**
3.  **Quantized Curvature/Entropy Operators.**
4.  **Informational Uncertainty Relations.**

### Qualia as the Furthest Horizon:
Qualia are modeled as \(\Delta\)-stable, projection-resistant homological features of recursive \(\Delta\)-self structure; minimal, stable, irreducible features within an observer's \(\Delta\)-field dynamics persisting under compression but not fully projectable. They are observer-dependent, constraint-shaped, structure-preserving informational scars or echoes, felt as irreducible informational asymmetries.

**Conceptual Closure:** IC provides a framework where spacetime, memory, time, measurement, geometry, and observers emerge from recursive distinction under constraint, with qualia as the terminal informational features reflecting the irreducible topology of internal \(\Delta\)-dynamics.

---
Footnotes:
<sup>1</sup> Zeta functions built upon these discovered primes can then encode distributional information about these fundamental multiplicative units of quantity. For instance, the properties of the Riemann zeta function \(\zeta(s) = \sum_{n=1}^\infty n^{-s} = \prod_p (1-p^{-s})^{-1}\) are deeply connected to the distribution of primes. The connection to ISG density (especially along the diagonal \(x=y\), representing prime powers \(p^k\)) can be explored via related series like \(\sum_p \sum_{k \ge 1} p^{-ks} = \sum_p \frac{p^{-s}}{1-p^{-s}}\), which is the logarithmic derivative \(\zeta'(s)/\zeta(s)\). This suggests that the structural parameters of the ISG directly relate to analytic properties studied in number theory.
