---
parent: "[[Understanding Analysis - 6.5  Power Series]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove if $g(x) = \sum_{n=0}^{\infty} a_n x^n$ converges at $x = R > 0$, then the series converges uniformly on $[0, R]$
#### Notes
- Express the power series in terms of the boundary point as $\sum_{n=0}^{\infty} (a_n R^n) (x/R)^n$.
- Given $\epsilon > 0$, apply the Cauchy criterion to the convergent series $\sum a_n R^n$ to bound its tail below $\epsilon/2$ for indices beyond $N$.
- Observe that for any fixed $x \in [0, R]$, the sequence $((x/R)^n)$ is non-negative, monotone decreasing, and bounded by $1$.
- Apply the Abel lemma to bound the tail sum $\vert{}\sum_{k=m+1}^n (a_k R^k) (x/R)^k\vert{}$ by $\epsilon/2 (x/R)^{m+1} \le \epsilon/2$.
- Conclude uniform convergence on $[0, R]$ via the Cauchy criterion for uniform convergence of series.
