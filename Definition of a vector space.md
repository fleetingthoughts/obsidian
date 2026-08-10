---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.2 Vector Spaces]]"
tags:
  - "#flashcard"
  - arnold_friedberg
  - micro/math/friedberg/ch1
date_created: 2026-07-24
---
State the definition of a vector space and the axioms it must satisfy
#### Notes
A vector space (or linear space) over a field $F$ (such as the real numbers $\mathbb{R}$ or complex numbers $\mathbb{C}$) is a non-empty set $V$ of objects, called vectors, equipped with two operations:
- **Vector addition:** A rule that assigns to any two vectors $u, v \in V$ a third vector in $V$, denoted as $u + v$.
- **Scalar multiplication:** A rule that assigns to any scalar $c \in F$ and any vector $v \in V$ a new vector in $V$, denoted as $cv$.

_(Note: The requirement that $u + v$ and $cv$ must always result in a vector that is also within the set $V$ is known as **closure**. While sometimes listed as the first two axioms, closure is inherently required by the definition of these mathematical operations.)_
## The axioms
For $V$ to be a valid vector space, the operations of vector addition and scalar multiplication must satisfy the following eight axioms for all vectors $u, v, w \in V$ and all scalars $a, b \in F$:
**Axioms of addition**
1. **Commutativity:** $u + v = v + u$
2. **Associativity:** $(u + v) + w = u + (v + w)$
3. **Additive identity:** There exists an element $0 \in V$, called the zero vector, such that $v + 0 = v$ for all $v \in V$.
4. **Additive inverse:** For every $v \in V$, there exists an element $-v \in V$ such that $v + (-v) = 0$.
**Axioms of scalar multiplication**
5. **Compatibility:** $a(bv) = (ab)v$
6. **Identity element:** $1v = v$, where $1$ denotes the multiplicative identity of the field $F$.
7. **Distributivity over vector addition:** $a(u + v) = au + av$
8. **Distributivity over field addition:** $(a + b)v = av + bv$
