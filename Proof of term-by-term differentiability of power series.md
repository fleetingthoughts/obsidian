---
parent: "[[Understanding Analysis - 6.5  Power Series]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove if $\sum_{n=0}^{\infty} a_n x^n$ converges for all $x \in (-R, R)$, then the differentiated series $\sum_{n=1}^{\infty} n a_n x^{n-1}$ converges absolutely at each $x \in (-R, R)$
#### Notes
- Fix an arbitrary $x \in (-R, R)$ and select a real number $t$ such that $\vert{}x\vert{} < t < R$.
- Algebraically rewrite the differentiated term as $\vert{}n a_n x^{n-1}\vert{} = \frac{1}{t} \vert{}n (x/t)^{n-1}\vert{} \vert{}a_n t^n\vert{}$.
- Observe that because $0 < \vert{}x/t\vert{} < 1$, the sequence $(n (x/t)^{n-1})$ is bounded by a constant $M$.
- Bound the differentiated term by $\frac{M}{t} \vert{}a_n t^n\vert{}$.
- Because $\sum a_n t^n$ converges absolutely, apply the comparison test to deduce absolute convergence of the differentiated series.
