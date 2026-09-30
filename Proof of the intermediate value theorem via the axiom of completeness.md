---
parent: "[[Understanding Analysis - 4.5 Intermediate Value Theorem]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch4
date_created: 2026-09-29
---
Prove: Let $f : [a, b] \to \mathbf{R}$ be continuous. If $f(a) < 0 < f(b)$, then there exists a point $c \in (a, b)$ where $f(c) = 0$.
#### Notes
- Define $K = \{x \in [a, b] : f(x) \le 0\}$ and observe it is nonempty and bounded above by $b$.
    
- Invoke the Axiom of completeness to set $c = \sup K$.
    
- Rule out $f(c) > 0$: continuity implies a neighborhood where $f(x) > 0$, making $c - \delta$ an upper bound, contradicting $c = \sup K$.
    
- Rule out $f(c) < 0$: continuity implies a neighborhood where $f(x) < 0$, yielding elements of $K$ greater than $c$, contradicting $c$ as an upper bound.
    
- Conclude by trichotomy that $f(c) = 0$.
