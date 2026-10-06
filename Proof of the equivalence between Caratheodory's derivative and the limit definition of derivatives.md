---
parent: "[[Understanding Analysis - 5.2 Derivatives and the Intermediate Value Property]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-03
---
A function $h : A \to \mathbf{R}$ is differentiable at $a \in A$ if and only if there exists a function $l : A \to \mathbf{R}$ that is continuous at $a$ and satisfies $h(x) - h(a) = l(x)(x - a)$ for all $x \in A$.
#### Notes
- $(\implies)$ Set $l(x) = \frac{h(x) - h(a)}{x - a}$ for $x \neq a$ and $l(a) = h'(a)$; continuity of $l$ follows from the definition of $h'(a)$.
- $(\impliedby)$ Take $\lim_{x \to a} \frac{h(x) - h(a)}{x - a} = \lim_{x \to a} l(x) = l(a) = h'(a)$.
