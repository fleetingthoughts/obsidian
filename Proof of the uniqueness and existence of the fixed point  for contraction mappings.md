---
parent: "[[Understanding Analysis - 4.3 Continuous Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch4
date_created: 2026-09-27
---
Prove: If $f : \mathbf{R} \to \mathbf{R}$ is a contraction mapping and $(y_n)$ is an iteration sequence converging to $y$, then $y$ is the unique fixed point of $f$. 

If $f : \mathbf{R} \to \mathbf{R}$ is a contraction mapping with fixed point $y$, then for any arbitrary $x \in \mathbf{R}$, the sequence $(x, f(x), f(f(x)), \dots)$ converges to $y$.
#### Notes
- Existence: Take the limit of the recurrence $y_{n+1} = f(y_n)$. By the continuity of $f$, $\lim y_{n+1} = f(\lim y_n)$, establishing $y = f(y)$.
    
- Uniqueness: Assume two fixed points $y$ and $z$. Then $\vert{}y - z\vert{} = \vert{}f(y) - f(z)\vert{} \le c\vert{}y - z\vert{}$.
    
- Conclude that since $0 < c < 1$, this inequality forces $\vert{}y - z\vert{} = 0$, so $y = z$

Proof of global convergence:
We have $\vert{}x_{n+1} - y\vert{} = \vert{}f(x_n) - f(y)\vert{} \le c\vert{}x_n - y\vert{}$. By induction, $\vert{}x_n - y\vert{} \le c^{n-1}\vert{}x_1 - y\vert{}$. Since $c < 1$, the distance $c^{n-1}\vert{}x_1 - y\vert{} \to 0$ as $n \to \infty$, thus $\lim x_n = y$.
