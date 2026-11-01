---
parent: "[[Understanding Analysis - 6.6 Taylor Series]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: The Taylor series $\sum_{n=0}^\infty \frac{x^n}{n!}$ converges uniformly to $e^x$ on $[-R, R]$ for any $R \gt 0$, and $e^x \cdot e^{-x} = 1$.
#### Notes
- For $f(x) = e^x$, observe $f^{(N+1)}(t) = e^t \le e^R$ for all $t \in [-R, R]$.
    
- By Lagrange's remainder theorem, for any $x \in [-R, R]$, $\vert{}E_N(x)\vert{} = \frac{e^c}{(N+1)!}\vert{}x\vert{}^{N+1} \le \frac{e^R R^{N+1}}{(N+1)!} \to 0$ as $N \to \infty$ independently of $x$, establishing uniform convergence on $[-R, R]$.
    
- Multiply the absolutely convergent power series for $e^x$ and $e^{-x}$ via the Cauchy product to obtain $\sum_{n=0}^\infty d_n x^n$ where:
    
    $$d_n = \sum_{k=0}^n \frac{1}{k!} \frac{(-1)^{n-k}}{(n-k)!} = \frac{1}{n!} \sum_{k=0}^n \binom{n}{k} 1^k (-1)^{n-k} = \frac{(1-1)^n}{n!}$$
    
- Note $d_0 = 1$ and $d_n = 0$ for all $n \ge 1$, concluding $e^x \cdot e^{-x} = 1$.