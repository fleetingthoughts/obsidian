---
parent: "[[Understanding Analysis - 6.6 Taylor Series]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: If $f$ is differentiable $N+1$ times on $(-R, R)$ and $S_N(x) = \sum_{n=0}^N \frac{f^{(n)}(0)}{n!} x^n$, then for any $x \neq 0$ in $(-R, R)$, there exists $c$ with $\vert{}c\vert{} \lt \vert{}x\vert{}$ such that $E_N(x) = f(x) - S_N(x) = \frac{f^{(N+1)}(c)}{(N+1)!} x^{N+1}$.
#### Notes
- Observe that $E_N^{(n)}(0) = f^{(n)}(0) - S_N^{(n)}(0) = 0$ for all $0 \le n \le N$, and $E_N^{(N+1)}(t) = f^{(N+1)}(t)$ since $\deg(S_N) \le N$.
- Assuming $x \gt 0$ (and analogously for $x \lt 0$), apply the Generalized Mean Value Theorem to $E_N(t)$ and $t^{N+1}$ on $[0, x]$ using $E_N(0) = 0$ to find $x_1 \in (0, x)$ such that $\frac{E_N(x)}{x^{N+1}} = \frac{E_N'(x_1)}{(N+1) x_1^N}$.
- Apply the Generalized Mean Value Theorem inductively $N$ additional times on $[0, x_k]$ using $E_N^{(k)}(0) = 0$ to obtain nested points $0 \lt x_{N+1} \lt x_N \lt \dots \lt x_1 \lt x$ satisfying:$$\frac{E_N(x)}{x^{N+1}} = \frac{E_N^{(N+1)}(x_{N+1})}{(N+1)!}$$
- Set $c = x_{N+1} \in (0, x)$ and substitute $E_N^{(N+1)}(c) = f^{(N+1)}(c)$ to obtain $E_N(x) = \frac{f^{(N+1)}(c)}{(N+1)!} x^{N+1}$.
