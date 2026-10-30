---
parent: "[[Understanding Analysis - 6.4  Series of Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: If $0 \le f_n(x) \le g_n(x)$ for all $x \in A$ and $\sum_{n=1}^{\infty} g_n$ converges uniformly on $A$, then $\sum_{n=1}^{\infty} f_n$ converges uniformly on $A$.
#### Notes
By the Cauchy criterion for uniform convergence of $\sum g_n$, for any $\epsilon > 0$, there exists $N$ such that $\sum_{k=m+1}^n g_k(x) < \epsilon$ for all $x \in A$ and $n > m \ge N$. Since $0 \le f_k(x) \le g_k(x)$, it follows that $\sum_{k=m+1}^n f_k(x) \le \sum_{k=m+1}^n g_k(x) < \epsilon$. Thus, $\sum f_n$ satisfies the Cauchy criterion and converges uniformly.
