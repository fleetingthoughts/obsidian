---
parent: "[[Understanding Analysis - 7.3 Uniform Convergence and the Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: Every finite subset $A = \{x_1, \dots, x_N\} \subseteq [a, b]$ has content zero.
#### Notes
Given $\epsilon \gt 0$, cover each point $x_n \in A$ with the open interval $O_n = \left(x_n - \frac{\epsilon}{2N}, x_n + \frac{\epsilon}{2N}\right)$. Then $A \subseteq \bigcup_{n=1}^N O_n$ and $\sum_{n=1}^N \vert{}O_n\vert{} = \sum_{n=1}^N \frac{\epsilon}{N} = \epsilon$.
