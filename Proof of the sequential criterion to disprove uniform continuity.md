---
parent:
tags:
  - "#flashcard"
date_created: "2026-09-27"
---
Prove: A function $f : A \to \mathbf{R}$ fails to be uniformly continuous on $A$ if and only if there exists $\epsilon_0 > 0$ and sequences $(x_n), (y_n) \subseteq A$ satisfying $\lim \vert{}x_n - y_n\vert{} = 0$ while $\vert{}f(x_n) - f(y_n)\vert{} \ge \epsilon_0$.
#### Notes
- Forward: Negate uniform continuity to fix $\epsilon_0 > 0$. For every $\delta_n = 1/n$, select corresponding $x_n, y_n$ satisfying $\vert{}x_n - y_n\vert{} < 1/n$ and $\vert{}f(x_n) - f(y_n)\vert{} \ge \epsilon_0$.
    
- Backward: Assume sequences exist. For any candidate $\delta > 0$, select $N$ such that $\vert{}x_N - y_N\vert{} < \delta$.
    
- Conclude that $\vert{}f(x_N) - f(y_N)\vert{} \ge \epsilon_0$ demonstrates no $\delta$ satisfies the uniform continuity condition.
