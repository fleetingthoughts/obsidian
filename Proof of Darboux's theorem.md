---
parent: "[[Understanding Analysis - 5.2 Derivatives and the Intermediate Value Property]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-03
---
Prove: If $f$ is differentiable on an interval $[a, b]$, and if $\alpha$ satisfies $f'(a) < \alpha < f'(b)$, then there exists a point $c \in (a, b)$ where $f'(c) = \alpha$.
#### Notes
- Define $g(x) = f(x) - \alpha x$ on $[a, b]$, making $g$ differentiable with $g'(x) = f'(x) - \alpha$ and $g'(a) < 0 < g'(b)$.
    
- Because $g'(a) < 0$ and $g'(b) > 0$, show $g$ cannot attain its minimum at $a$ or $b$.
    
- By the Extreme Value Theorem, $g$ attains a minimum at some interior point $c \in (a, b)$.
    
- Apply the Interior Extremum Theorem to $g$ at $c$ to obtain $g'(c) = 0 \implies f'(c) = \alpha$.
