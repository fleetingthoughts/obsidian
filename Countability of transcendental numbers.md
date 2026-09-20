---
parent: "[[Understanding Analysis - 1.5 Cardinality]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch1
date_created: 2026-09-19
---
What can we say about the countability of the transcendental numbers and prove it.
#### Notes
For a fixed $n \in \mathbf{N}$, the set $A_n$ of algebraic numbers obtained as roots of polynomials with integer coefficients of degree $n$ is countable
- Establish a bijection mapping the coefficients of degree $n$ integer polynomials to a subset of $\mathbf{Z}^{n+1}$.
- State that the set of such polynomials is countable, as finite Cartesian products of countable sets are countable.
- Apply the property that every polynomial has a finite number of roots.
- Conclude $A_n$ is a countable union of finite sets, which is countable.
Prove: The set of all algebraic numbers is countable.
- Define $A_n$ as the set of algebraic numbers obtained from integer polynomials of degree $n$.
- Express the set of all algebraic numbers as the union $\bigcup_{n=1}^{\infty} A_n$.
- Apply the theorem that a countable union of countable sets is countable.
**Front:** Prove: The set of all transcendental numbers is uncountable.

**Back:**
1. State that the set of real numbers $\mathbf{R}$ is the union of algebraic and transcendental numbers.
2. Note that $\mathbf{R}$ is uncountable and the set of algebraic numbers is countable.
3. Conclude by contradiction: if transcendental numbers were countable, the union of two countable sets would produce the uncountable set $\mathbf{R}$.
