# Informational Constructivism

4/28/24: I've been thinking about the problem with pure mathematics (as distinct from applied mathematics) for a while now. I'm not alone here (For instance: see N J Wildberger's recent comments https://www.youtube.com/watch?v=YhN4X56E7iM). Instead of just complaining, I figured I would try to think through alterantive systems. The following are speculative musings on information as the root of mathematics and our observable universe. I expect to gradually build out this theory over time, altering it as I learn more. Below is a rough intro of what I hope to flesh out over time: 


### Introduction

#### 1.1 The Limitations of Current Mathematical Foundations

Mathematics, as currently understood, rests on a foundation established primarily by set theory. This system, developed between the late 19th and early 20th centuries, offers a rigorous framework for defining mathematical objects and deducing theorems. Despite the substantial capabilities of set theory, it faces several inherent limitations. Firstly, set theory is based on axioms, such as the axiom of choice. These axioms serve as arbitrary starting points; varying these axioms can lead to different mathematical outcomes. Secondly, as Gödel's incompleteness theorems reveal, any sufficiently complex axiomatic system, including set theory, contains true but unprovable statements within its structure, highlighting fundamental limitations to what mathematics can prove. Lastly, set theory’s reliance on abstract, infinite collections distances it from practical applications in the physical sciences and computation, creating a conceptual divide. Good overview of this basic disconnect can be found here: https://www.youtube.com/watch?v=U75S_ZvnWNk

#### 1.2 The Potential of an Information-Theoretic Approach

Considering these constraints, we advocate for a novel foundational approach based on information theory, rather than sets. Originating from the work of Claude Shannon in the mid-20th century, information theory provides a robust framework for quantifying and analyzing information properties. By prioritizing information as the fundamental element, our approach seeks to align mathematics more closely with computation and the physical sciences, addressing several of set theory's limitations. We view mathematical objects and structures as patterns of information, with mathematical operations and proofs functioning as processes of information transformation and transmission. This perspective aims to deliver a more integrated and accessible understanding of mathematics, as well as unintuitive concepts such as infinity.

#### 1.3 Goals and Structure of the Paper

This paper aims to outline a framework for an information-theoretic foundation of mathematics. We will begin by defining the concept of information, exploring its essential properties and operations. Subsequently, we will reinterpret fundamental mathematical concepts such as numbers, functions, and spaces through an informational lens. We will examine how this approach can address some of the paradoxes and constraints of set theory. Then we will look into how this approach could apply to our observable universe and close with some ideas for future avenues for research.

### 2.1 Historical Background and Context

The modern framework of information theory owes much to Claude Shannon's contributions in the 1940s. Working at Bell Labs, Shannon tackled the problem of efficient message transmission across noisy communication channels. His pivotal 1948 paper, "A Mathematical Theory of Communication," introduced a quantitative measure of information, exploring its role in defining the limits of communication and computation.

Central to Shannon's theory is a precise definition of information: it measures the uncertainty or surprise associated with a message or event. The more unexpected or improbable a message, the higher its informational content.

Formally, given a set of possible messages or events, each with a specific probability of occurrence, the information content of a message is defined as the negative logarithm of its probability. This definition implies that rare or surprising events convey more information than those that are common or anticipated.

This definition adheres to certain intuitive properties. For instance, if two events are independent, the information content of their combined occurrence equals the sum of their individual contents. Moreover, the information content of a deterministic event (one that invariably occurs or never happens) is zero.

### 2.2 Key Properties and Operations of Information

From this definition, several properties and operations of information emerge:

- **Additivity**: The information content of independent events is cumulative. If A and B are independent, the information content of their joint occurrence, I(A, B), equals I(A) + I(B).
  
- **Monotonicity**: As the probability of an event increases, its information content decreases. If P(A) > P(B), then I(A) < I(B).
  
- **Symmetry**: The information content is independent of the sequence of events. Thus, I(A, B) is the same as I(B, A).
  
- **Conditioning**: Prior knowledge about an event can alter its information content. The conditional information of A given B, I(A|B), typically differs from the unconditional information I(A).

Essential operations on information include:

- **Encoding**: This is the process of formatting information for storage or transmission, often involving the assignment of codewords to messages to minimize average encoded message length.
  
- **Channel**: The medium or method through which information is conveyed. Channels can be noisy, introducing errors into transmitted messages.
  
- **Decoding**: This involves reconstructing the original message from its encoded form, even in the presence of noise or errors.

### 2.3 Foundational Principles of Information for Mathematics

To establish a robust foundation for mathematics based on information theory, we propose two principles:

#### 2.3.1 The Principle of Distinguishability

The core property of information is its capacity to differentiate between various possibilities. Information can be fundamentally defined by what it distinguishes or excludes.

Consider a simple binary scenario, such as a coin toss. The result of the toss (heads or tails) provides information because it differentiates between two possibilities. Without such distinction (e.g., if both sides of the coin were identical), the toss would yield no information.

This principle can be extended to any set of mutually exclusive options. The information content of an event is determined by the possibilities it excludes. The more possibilities that are excluded, the greater the informational content of the event.

Mathematically, this can be expressed using set theory. If Ω represents the set of all possible outcomes and A ⊆ Ω is an event, then the information content of A is related to its complement, Aᶜ (the set of outcomes that A excludes).

In an information-theoretic approach to mathematics, the fundamental elements are not sets themselves but the distinctions or differences between sets.

#### 2.3.2 The Principle of Constraints

The second principle is that information inherently arises from constraints. Without constraints, information cannot exist.

Consider a variable capable of assuming any real value. Without any constraints, this variable conveys no information. Information begins to emerge when constraints are applied (e.g., the variable must be positive or less than 10).

Constraints can be viewed as the rules or conditions that limit possibilities, enhancing the specificity of the information provided. In mathematics, these constraints often manifest as equations or inequalities. The solutions to these constraints constitute the informative content. More broadly, mathematical structures (such as groups, rings, or spaces) are defined by the constraints they fulfill.

This principle implies that in an informational approach to mathematics, the emphasis should be on the constraints or rules that define mathematical objects, rather than on the objects themselves.

#### 3.1 Building on These Principles

In this theory, we diverge from the traditional probabilistic interpretation of information and instead view it as a measure of the degree to which a given state or outcome is specified or determined by the available data or constraints.

Consider a set Ω representing all possible states or configurations of a system. For example, in a simple coin toss system, Ω might be {H, T}, representing the two possible outcomes, heads and tails. We define a partial order ≤ on Ω, where x ≤ y signifies that state y is at least as specified or constrained as state x. In other words, if x ≤ y, then all the data or constraints that specify x also specify y, but the converse may not be true.

We can now define the information content I(x) of a state x ∈ Ω as the "height" of x in this partial order—that is, the length of the longest chain of states leading up to x. States with more information are more fully specified and thus higher in the order.

Formally:
I(x) = max{n : there exists a chain x₀ < x₁ < ... < xₙ = x in Ω}

This definition captures the essence of information as the accumulation of constraints or specifications that narrow down the set of possible states. In the coin toss example, if we consider the state space Ω = {H, T}, without any additional constraints, both states H and T would have information content 0. However, if we add the constraint that the coin is fair (i.e., P(H) = P(T) = 0.5), this would introduce a new state F representing a fair coin toss, with H < F and T < F. In this augmented state space, I(H) = I(T) = 0, but I(F) = 1, reflecting the additional specifying constraint.

## 3.2 Distinguishability as Incomparability

 Two states x, y ∈ Ω are distinguishable if they are incomparable under the information partial order, i.e., if neither x ≤ y nor y ≤ x. This means that the data or constraints that specify x and y are mutually exclusive—they cannot both be satisfied simultaneously.

To quantify distinguishability, we introduce a metric d on Ω, where d(x, y) is the minimum number of "steps" needed to go from x to y in the partial order. Formally:
d(x, y) = min{n : there exists a chain x = x₀ < x₁ < ... < xₙ = y or y = y₀ < y₁ < ... < yₙ = x in Ω}

If no such chain exists (i.e., if x and y are incomparable), we set d(x, y) = ∞.

This metric provides a way to quantify the degree of distinguishability between states. States that are further apart under this metric are more distinguishable, as they require more "steps" of specification or constraint to connect them. In the coin toss example, d(H, T) = ∞, reflecting their complete distinguishability, while d(H, F) = d(T, F) = 1, indicating that they are "one step apart" in terms of specification.

## 3.3 Constraints as Building Blocks of Information

A constraint is any piece of data or condition that restricts the set of possible states. Formally, a constraint C is a subset of Ω, representing the states that satisfy the constraint.

The information content of a state x is determined by the constraints it satisfies. The more constraints a state satisfies, the more information it contains. We define the set of constraints satisfied by a state x as:
C(x) = {C ⊆ Ω : x ∈ C}

The partial order on states is then induced by the subset relation on their constraint sets:
x ≤ y if and only if C(x) ⊆ C(y)

This formalizes the idea that a state y is more informative than a state x if it satisfies all the constraints that x does, and possibly more. In the coin toss example, we have C(H) = C(T) = {Ω}, while C(F) = {Ω, {H, T}}, reflecting the additional fairness constraint satisfied by F.

## 3.4 Axiomatization and Properties

To create a complete deductive system, we can formalize our definitions as axioms:

1. (State Space) Ω is a non-empty set representing all possible states of the system.

2. (Partial Order) ≤ is a partial order on Ω, i.e., for all x, y, z ∈ Ω:
   - (Reflexivity) x ≤ x
   - (Antisymmetry) If x ≤ y and y ≤ x, then x = y
   - (Transitivity) If x ≤ y and y ≤ z, then x ≤ z

3. (Information Content) For any x ∈ Ω, I(x) = max{n : there exists a chain x₀ < x₁ < ... < xₙ = x in Ω}

4. (Distinguishability Metric) d is a metric on Ω, i.e., for all x, y, z ∈ Ω:
   - (Non-negativity) d(x, y) ≥ 0, and d(x, y) = 0 if and only if x = y
   - (Symmetry) d(x, y) = d(y, x)
   - (Triangle Inequality) d(x, z) ≤ d(x, y) + d(y, z)

5. (Constraints) A constraint C is a subset of Ω. For any x ∈ Ω, C(x) = {C ⊆ Ω : x ∈ C}

6. (Partial Order from Constraints) For any x, y ∈ Ω, x ≤ y if and only if C(x) ⊆ C(y)

...to be continued.


