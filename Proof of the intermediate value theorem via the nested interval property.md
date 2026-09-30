---
parent: "[[Understanding Analysis - 4.5 Intermediate Value Theorem]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch4
date_created: 2026-09-29
---
Prove: Let $f : [a, b] \to \mathbf{R}$ be continuous. If $f(a) < 0 < f(b)$, then there exists a point $c \in (a, b)$ where $f(c) = 0$.
#### Notes
- Initialize $I_0 = [a, b]$. Bisect $I_0$ at the midpoint $z$, selecting the half where the function changes sign to form $I_1$.
    
- Inductively construct nested closed intervals $I_n = [a_n, b_n]$ satisfying $f(a_n) < 0 \le f(b_n)$ with lengths tending to 0.
    
- Apply the Nested interval property to obtain a unique $c \in \bigcap_{n=0}^\infty I_n$, implying $\lim a_n = c = \lim b_n$.
    
- Apply the continuity of $f$ to establish $f(c) = \lim f(a_n) \le 0$ and $f(c) = \lim f(b_n) \ge 0$, forcing $f(c) = 0$.
