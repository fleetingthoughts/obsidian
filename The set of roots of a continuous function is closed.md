---
parent: "[[Understanding Analysis - 4.3 Continuous Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch3
date_created: 2026-09-19
---
Prove: If $h : \mathbf{R} \to \mathbf{R}$ is continuous on $\mathbf{R}$ and $K = \{x : h(x) = 0\}$, then $K$ is a closed set.
#### Notes
- Consider an arbitrary limit point $c$ of the set $K$.
    
- Construct a sequence $(x_n)$ contained entirely within $K$ that converges to $c$.
    
- Apply the sequential criterion for continuity to $h$ at $c$, yielding $\lim h(x_n) = h(c)$.
    
- Observe that $h(x_n) = 0$ for all $n$, which implies $h(c) = 0$.
    
- Conclude $c \in K$, establishing that $K$ contains all its limit points and is therefore closed.
