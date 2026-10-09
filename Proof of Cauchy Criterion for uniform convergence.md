---
parent: "[[Understanding Analysis - 6.2  Uniform Convergence of a Sequence of Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: A sequence of functions $(f_n)$ defined on $A \subseteq \mathbf{R}$ converges uniformly on $A$ if and only if for every $\epsilon > 0$ there exists an $N \in \mathbf{N}$ such that $\vert{}f_n(x) - f_m(x)\vert{} < \epsilon$ whenever $m, n \ge N$ and $x \in A$.
#### Notes
- ($\implies$): Assume uniform convergence. Use the $\epsilon/2$ uniform bound on $\vert{}f_n(x) - f(x)\vert{}$ and the triangle inequality to bound $\vert{}f_n(x) - f_m(x)\vert{}$.
    
- ($\impliedby$): Fix $x \in A$. $(f_n(x))$ is Cauchy in $\mathbf{R}$, yielding a pointwise limit $f(x)$.
    
- Given $\epsilon > 0$, fix $N$ from the Cauchy condition using $\epsilon/2$. Let $m \to \infty$ in $\vert{}f_n(x) - f_m(x)\vert{} < \epsilon/2$ to obtain $\vert{}f_n(x) - f(x)\vert{} \le \epsilon/2 < \epsilon$ for all $x \in A$ simultaneously.
