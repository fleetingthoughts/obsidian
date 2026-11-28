---
parent: "[[Understanding Analysis - 4.3 Continuous Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch3
date_created: 2026-09-19
---
Prove: If $h : \mathbf{R} \to \mathbf{R}$ is continuous on $\mathbf{R}$ and $K = \{x : h(x) = 0\}$, then $K$ is a closed set.
#### Notes
 Let $(x_n)$ be a sequence in $K$ converging to $x \in \mathbb{R}$. By continuity of $h$, $h(x) = \lim_{n \to \infty} h(x_n) = 0$, so $x \in K$. Because $K$ contains all its limit points, $K$ is closed. (Alternatively, $K = h^{-1}(\{0\})$ is the preimage of the closed singleton $\{0\}$ under a continuous map.)
<!--SR:!fsrs,2026-12-06T04:57:24.073Z,8,8.2956,1,2,1,0,0,2026-11-28T04:57:24.073Z-->
    
- Construct a sequence $(x_n)$ contained entirely within $K$ that converges to $c$.
    
- Apply the sequential criterion for continuity to $h$ at $c$, yielding $\lim h(x_n) = h(c)$.
    
- Observe that $h(x_n) = 0$ for all $n$, which implies $h(c) = 0$.
    
- Conclude $c \in K$, establishing that $K$ contains all its limit points and is therefore closed.
