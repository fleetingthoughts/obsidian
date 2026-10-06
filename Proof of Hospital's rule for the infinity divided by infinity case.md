---
parent:
tags:
  - "#flashcard"
date_created: "2026-10-04"
---
Prove: Assume $f$ and $g$ are differentiable on $(a, b)$ and $g'(x) \ne 0$ for all $x \in (a, b)$. If $\lim_{x \to a} g(x) = \infty$ (or $-\infty$) and $\lim_{x \to a} \frac{f'(x)}{g'(x)} = L$, then $\lim_{x \to a} \frac{f(x)}{g(x)} = L$.
#### Notes
- For a given $\epsilon > 0$, choose $t = a + \delta_1$ such that $\left\vert{} \frac{f'(x)}{g'(x)} - L \right\vert{} < \frac{\epsilon}{2}$ for all $x \in (a, t)$.
- Apply the Generalized mean value theorem to $[x, t]$ for $x \in (a, t)$ to obtain bounds on $\frac{f(x) - f(t)}{g(x) - g(t)}$.
- Multiply the inequality by $1 - \frac{g(t)}{g(x)}$ to isolate $\frac{f(x)}{g(x)}$.
- Choose tighter bounds ($\delta_2, \delta_3$) such that the diverging $g(x)$ is large enough to bound the residual terms within $\frac{\epsilon}{2}$.
- Set $\delta = \min(\delta_1, \delta_2, \delta_3)$ to guarantee the limit definition $\left\vert{} \frac{f(x)}{g(x)} - L \right\vert{} < \epsilon$ is satisfied.
