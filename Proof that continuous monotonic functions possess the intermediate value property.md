---
parent: "[[Understanding Analysis - 4.5 Intermediate Value Theorem]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch4
date_created: 2026-09-29
---
Prove: If $f$ is increasing on $[a, b]$ and satisfies the intermediate value property, then $f$ is continuous on $[a, b]$.
#### Notes
- Assume for contradiction $f$ is discontinuous at $c \in (a, b)$.
    
- Because $f$ is increasing, the left limit $L$ and right limit $R$ exist at $c$, with $L < R$.
    
- Select $y \in (L, R)$ such that $y \neq f(c)$.
    
- Observe $f(x) \le L$ for $x < c$ and $f(x) \ge R$ for $x > c$, meaning $y$ is never attained on $[a, b]$.
    
- Conclude this violates the intermediate value property, forcing continuity at $c$.
