---
parent: "[[Understanding Analysis - 5.2 Derivatives and the Intermediate Value Property]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-03
---
Prove: If $f$ is uniformly differentiable on an interval $A$, then $f'$ is continuous on $A$.
#### Notes
- Given $y \in A$ and $\epsilon > 0$, uniform differentiability yields $\delta > 0$ such that $0 < \vert{}x - y\vert{} < \delta \implies \left\vert{} \frac{f(x) - f(y)}{x - y} - f'(y) \right\vert{} < \epsilon/2$.
- For any $z \in A$ with $0 < \vert{}z - y\vert{} < \delta$, uniform differentiability at $z$ yields $\left\vert{} \frac{f(y) - f(z)}{y - z} - f'(z) \right\vert{} < \epsilon/2$.
- Combine inequalities via the triangle inequality to obtain $\vert{}f'(z) - f'(y)\vert{} < \epsilon$, establishing continuity of $f'$ at $y$.
