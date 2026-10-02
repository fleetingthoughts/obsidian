---
parent: "[[Understanding Analysis - 4.5 Intermediate Value Theorem]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch4
date_created: 2026-09-29
---
Let $g$ be continuous on an interval $A$. Let $F = \{x \in A : g(x) = g(y) \text{ for some } y \neq x, y \in A\}$. Then $F$ is either empty or uncountable.
#### Notes
- Assume $F \neq \emptyset$, taking distinct $x_1, x_2 \in A$ where $g(x_1) = g(x_2) = k$.
- By the Extreme value theorem on $[x_1, x_2]$, $g$ attains a local extremum $M \neq k$ at $c \in (x_1, x_2)$ (ignoring the trivial constant case which yields an interval).
- For any $y$ strictly between $k$ and $M$, apply the Intermediate value theorem to $[x_1, c]$ and $[c, x_2]$.
- Obtain distinct $z_1 \in (x_1, c)$ and $z_2 \in (c, x_2)$ with $g(z_1) = y = g(z_2)$.
- Conclude every value $y \in (k, M)$ produces a distinct pair in $F$, making $F$ uncountable.
<!--SR:!fsrs,2026-10-09T23:10:56.223Z,8,8.2956,1,2,1,0,0,2026-10-01T23:10:56.223Z-->
