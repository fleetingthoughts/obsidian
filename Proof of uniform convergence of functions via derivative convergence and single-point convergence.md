---
parent: "[[Understanding Analysis - 6.3  Uniform Convergence and Differentiation]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: Let $(f_n)$ be a sequence of differentiable functions defined on the closed interval $[a, b]$, and assume $(f_n')$ converges uniformly on $[a, b]$. If there exists a point $x_0 \in [a, b]$ where $(f_n(x_0))$ converges, then $(f_n)$ converges uniformly on $[a, b]$.
#### Notes
- Let $\epsilon \gt 0$. For any $x \in [a, b]$ and $m, n \in \mathbf{N}$, apply the triangle inequality:$$\vert{}f_n(x) - f_m(x)\vert{} \le \vert{}(f_n(x) - f_m(x)) - (f_n(x_0) - f_m(x_0))\vert{} + \vert{}f_n(x_0) - f_m(x_0)\vert{}.$$
- Apply the mean value theorem to $f_n - f_m$ between $x_0$ and $x$ to obtain $\alpha$ between $x_0$ and $x$ such that $(f_n(x) - f_m(x)) - (f_n(x_0) - f_m(x_0)) = (f_n'(\alpha) - f_m'(\alpha))(x - x_0)$.
- By the Cauchy criterion for uniform convergence of $(f_n')$, choose $N_1$ such that $\vert{}f_n'(t) - f_m'(t)\vert{} \lt \frac{\epsilon}{2(b - a)}$ for all $m, n \ge N_1$ and $t \in [a, b]$, bounding the first term by $\frac{\epsilon}{2(b - a)}\vert{}x - x_0\vert{} \le \frac{\epsilon}{2}$.
- By convergence of $(f_n(x_0))$, choose $N_2$ such that $\vert{}f_n(x_0) - f_m(x_0)\vert{} \lt \frac{\epsilon}{2}$ for all $m, n \ge N_2$.
- Set $N = \max\{N_1, N_2\}$ to obtain $\vert{}f_n(x) - f_m(x)\vert{} \lt \epsilon$ for all $m, n \ge N$ and $x \in [a, b]$, proving $(f_n)$ is uniformly Cauchy on $[a, b]$.
