# Informational Constructivism

4/28/24: I've been thinking about the problem with pure mathematics (as distinct from applied mathematics) for a while now. I'm not alone here (For instance: see N J Wildberger's recent comments https://www.youtube.com/watch?v=YhN4X56E7iM). Instead of just complaining, I figured I would try to think through a way out. The following are speculative musings on information as the root of mathematics and our observable universe that I think might address some of the root unaddressed issues. I hope to gradually build out this theory over time. Below is a rough intro of what I hope to accomplish: 


### Introduction

#### 1.1 The Limitations of Current Mathematical Foundations

Mathematics, as currently understood, rests on a foundation established primarily by set theory. This system, developed between the late 19th and early 20th centuries, offers a rigorous framework for defining mathematical objects and deducing theorems. Despite the substantial capabilities of set theory, it faces several inherent limitations. Firstly, set theory is based on axioms, such as the axiom of choice, which have sparked considerable debate. These axioms serve as arbitrary starting points; varying these axioms can lead to different mathematical outcomes. Secondly, as Gödel's incompleteness theorems reveal, any sufficiently complex axiomatic system, including set theory, contains true but unprovable statements within its structure, highlighting fundamental limitations to what mathematics can prove. Lastly, set theory’s reliance on abstract, infinite collections distances it from practical applications in the physical sciences and computation, creating a conceptual divide.

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
  
- **Compression**: This process reduces message size by eliminating redundancy or employing more efficient encoding techniques. Lossless compression allows for perfect reconstruction of the original message, whereas lossy compression permits some degradation.


