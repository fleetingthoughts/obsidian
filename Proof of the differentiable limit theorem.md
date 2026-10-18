---
parent: "[[Understanding Analysis - 6.3  Uniform Convergence and Differentiation]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: Let $f_n \to f$ pointwise on the closed interval $[a, b]$, and assume that each $f_n$ is differentiable on $[a, b]$. If $(f_n')$ converges uniformly on $[a, b]$ to a function $g$, then $f$ is differentiable on $[a, b]$ and $f' = g$.
#### Notes
- Fix $c \in [a, b]$ and $\epsilon \gt 0$. For $x \neq c$ and $N \in \mathbf{N}$, apply the triangle inequality:
  $$\left\vert{} \frac{f(x) - f(c)}{x - c} - g(c) \right\vert{} \le \left\vert{} \frac{f(x) - f(c)}{x - c} - \frac{f_N(x) - f_N(c)}{x - c} \right\vert{} + \left\vert{} \frac{f_N(x) - f_N(c)}{x - c} - f_N'(c) \right\vert{} + \vert{}f_N'(c) - g(c)\vert{}.$$
- Choose $N_1$ so that $\vert{}f_n'(c) - g(c)\vert{} \lt \frac{\epsilon}{3}$ for $n \ge N_1$, and by the Cauchy criterion for uniform convergence of $(f_n')$, choose $N_2$ so that $\vert{}f_m'(t) - f_n'(t)\vert{} \lt \frac{\epsilon}{3}$ for all $m, n \ge N_2$ and $t \in [a, b]$; fix $N = \max\{N_1, N_2\}$.
- For any $m \ge N$ and $x \neq c$, apply the mean value theorem to $f_m - f_N$ on the interval between $c$ and $x$ to find $\alpha$ satisfying $\left\vert{} \frac{f_m(x) - f_m(c)}{x - c} - \frac{f_N(x) - f_N(c)}{x - c} \right\vert{} = \vert{}f_m'(\alpha) - f_N'(\alpha)\vert{} \lt \frac{\epsilon}{3}$; let $m \to \infty$ to bound the first term by $\frac{\epsilon}{3}$.
- Using differentiability of $f_N$ at $c$, choose $\delta \gt 0$ such that $0 \lt \vert{}x - c\vert{} \lt \delta$ implies $\left\vert{} \frac{f_N(x) - f_N(c)}{x - c} - f_N'(c) \right\vert{} \lt \frac{\epsilon}{3}$.
- Combine the three $\frac{\epsilon}{3}$ bounds for $0 \lt \vert{}x - c\vert{} \lt \delta$ to conclude $\left\vert{} \frac{f(x) - f(c)}{x - c} - g(c) \right\vert{} \lt \epsilon$.
