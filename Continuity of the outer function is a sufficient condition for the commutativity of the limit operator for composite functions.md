---
parent:
tags:
  - "#flashcard"
date_created: "2026-09-27"
---
Prove: Let $f: A \to B$ and $g: B \to \mathbb{R}$. If $\lim_{x \to c} f(x) = q$ and $g$ is continuous at $q$, then $\lim_{x \to c} g(f(x)) = g(q)$
#### Notes
- Let $(x_n) \subseteq A$ be an arbitrary sequence converging to $c$ with $x_n \neq c$.
    
- By the sequential criterion for limits, $\lim f(x_n) = q$.
    
- Apply the sequential criterion for continuity to $g$ at $q$ to deduce that the image sequence converges: $\lim g(f(x_n)) = g(q)$.
    
- Conclude via the sequential criterion for limits that the functional limit $\lim_{x \to c} g(f(x))$ exists and equals $g(q)$.
