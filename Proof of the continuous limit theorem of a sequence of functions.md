---
parent: "[[Understanding Analysis - 6.2  Uniform Convergence of a Sequence of Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: If a sequence of functions $(f_n)$ converges uniformly to $f$ on $A \subseteq \mathbf{R}$ and each $f_n$ is continuous at $c \in A$, then $f$ is continuous at $c$.
#### Notes
- Fix $\epsilon > 0$. Use uniform convergence to select $N \in \mathbf{N}$ such that $\vert{}f_N(x) - f(x)\vert{} < \epsilon/3$ for all $x \in A$.
    
- Use the continuity of $f_N$ at $c$ to choose $\delta > 0$ such that $\vert{}x - c\vert{} < \delta$ implies $\vert{}f_N(x) - f_N(c)\vert{} < \epsilon/3$.
    
- Apply the 3-$\epsilon$ triangle inequality: decompose $\vert{}f(x) - f(c)\vert{}$ by inserting $f_N(x)$ and $f_N(c)$.
