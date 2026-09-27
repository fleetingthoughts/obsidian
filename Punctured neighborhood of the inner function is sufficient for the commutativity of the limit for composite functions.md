---
parent:
tags:
  - "#flashcard"
date_created: "2026-09-27"
---
Let $f: A \to B$ and $g: B \to \mathbb{R}$. If $\lim_{x \to c} f(x) = q$, $\lim_{y \to q} g(y) = L$, and $f(x) \neq q$ for all $x \neq c$ in some neighborhood of $c$, then $\lim_{x \to c} g(f(x)) = L$
#### Notes
- Given $\epsilon > 0$, invoke the limit of $g$ at $q$ to find $\delta_1 > 0$ such that $0 < \vert{}y - q\vert{} < \delta_1$ implies $\vert{}g(y) - L\vert{} < \epsilon$.
    
- Invoke the limit of $f$ at $c$ to find $\delta_2 > 0$ such that $0 < \vert{}x - c\vert{} < \delta_2$ implies $\vert{}f(x) - q\vert{} < \delta_1$.
    
- Restrict $\delta_2$ to the punctured neighborhood where $f(x) \neq q$, ensuring $0 < \vert{}f(x) - q\vert{}$.
    
- Chain the inequalities: for $0 < \vert{}x - c\vert{} < \delta_2$, let $y = f(x)$ to verify $0 < \vert{}f(x) - q\vert{} < \delta_1$, forcing $\vert{}g(f(x)) - L\vert{} < \epsilon$.
