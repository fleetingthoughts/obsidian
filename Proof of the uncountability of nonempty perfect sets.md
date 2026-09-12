---
parent: "[[Understanding Analysis - 3.4 Perfect Sets and Connected Sets]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch3
date_created: 2026-09-11
---
Prove that perfect sets are uncountable
#### Notes
- Assume for contradiction that $P$ is countable, and write $P = \{x_1, x_2, x_3, \dots\}$.
- Construct a closed interval $I_1$ containing $x_1$ in its interior, and because $x_1$ is not an isolated point, select $y_2 \in P \cap \text{int}(I_1)$ with $y_2 \neq x_1$ to construct a nested closed interval $I_2 \subseteq I_1$ centered at $y_2$ such that $x_1 \notin I_2$ and $I_2 \cap P \neq \emptyset$.
- Inductively construct a sequence of closed intervals $I_n$ satisfying $I_{n+1} \subseteq I_n$, $x_n \notin I_{n+1}$, and $I_n \cap P \neq \emptyset$.
- Define $K_n = I_n \cap P$, noting each $K_n$ is nonempty, closed, and bounded (hence compact), forming a nested sequence $K_{n+1} \subseteq K_n$.
- Apply the Nested Compact Set Property to conclude that $\bigcap_{n=1}^\infty K_n \neq \emptyset$, producing an element $x \in P$ that satisfies $x \neq x_n$ for all $n \in \mathbf{N}$, which contradicts the enumeration.
