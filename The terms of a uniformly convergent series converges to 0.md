---
parent: "[[Understanding Analysis - 6.4  Series of Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: If $\sum_{n=1}^{\infty} g_n(x)$ converges uniformly on $A$, then the sequence of functions $(g_n)$ converges uniformly to zero on $A$.
#### Notes
Let $s_n(x) = \sum_{k=1}^n g_k(x)$. Because the sequence of partial sums $(s_n)$ converges uniformly, it is uniformly Cauchy. For any $\epsilon > 0$, there exists $N$ such that $\vert{}s_n(x) - s_{n-1}(x)\vert{} < \epsilon$ for $n > N$ and all $x \in A$. Since $g_n(x) = s_n(x) - s_{n-1}(x)$, we have $\vert{}g_n(x)\vert{} < \epsilon$, establishing uniform convergence to zer
