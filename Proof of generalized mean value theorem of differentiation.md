---
parent: "[[Understanding Analysis - 5.3 The Mean Value Theorems]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-04
---
Prove: If $f$ and $g$ are continuous on $[a, b]$ and differentiable on $(a, b)$, then there exists a point $c \in (a, b)$ where $[f(b) - f(a)] g'(c) = [g(b) - g(a)] f'(c)$.
#### Notes
- Define $h(x) = [f(b) - f(a)] g(x) - [g(b) - g(a)] f(x)$ on $[a, b]$.
    
- Verify $h$ is continuous on $[a, b]$ and differentiable on $(a, b)$, satisfying $h(a) = f(b)g(a) - f(a)g(b) = h(b)$.
    
- Apply Rolle's theorem to $h$ to obtain $c \in (a, b)$ where $h'(c) = 0$.
    
- Differentiate $h(x)$ to conclude $[f(b) - f(a)] g'(c) - [g(b) - g(a)] f'(c) = 0$.
