---
parent: "[[Understanding Analysis - 6.5  Power Series]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove if a power series $\sum_{n=0}^{\infty} a_n x^n$ converges at some point $x_0 \in \mathbf{R}$, then it converges absolutely for any $x$ satisfying $\vert{}x\vert{} < \vert{}x_0\vert{}$
#### Notes
- Acknowledge that convergence at $x_0$ implies the sequence of terms $(a_n x_0^n)$ is bounded by some constant $M$.
- Rewrite the absolute terms for any $x \in (-\vert{}x_0\vert{}, \vert{}x_0\vert{})$ as $\vert{}a_n x^n\vert{} = \vert{}a_n x_0^n\vert{} \vert{}x / x_0\vert{}^n \le M \vert{}x / x_0\vert{}^n$.
- Establish that $\sum M \vert{}x / x_0\vert{}^n$ converges as a geometric series since $\vert{}x / x_0\vert{} < 1$.
- Conclude absolute convergence of $\sum a_n x^n$ via the comparison test.
