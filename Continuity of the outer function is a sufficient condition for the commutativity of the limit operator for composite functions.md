---
parent: "[[Understanding Analysis - 4.3 Continuous Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch4
date_created: 2026-09-27
---
Prove: Let $f: A \to B$ and $g: B \to \mathbb{R}$. If $\lim_{x \to c} f(x) = q$ and $g$ is continuous at $q$, then $\lim_{x \to c} g(f(x)) = g(q)$
#### Notes
1. Let $\epsilon > 0$.     
2. Invoke the continuity of $g$ at $q$ to find $\alpha > 0$ such that $\vert{}y - q\vert{} < \alpha$ implies $\vert{}g(y) - g(q)\vert{} < \epsilon$.
3. Invoke $\lim_{x \to c} f(x) = q$ to find $\delta > 0$ such that $0 < \vert{}x - c\vert{} < \delta$ implies $\vert{}f(x) - q\vert{} < \alpha$.
4. Conclude that for $0 < \vert{}x - c\vert{} < \delta$, the condition $\vert{}f(x) - q\vert{} < \alpha$ holds, which forces $\vert{}g(f(x)) - g(q)\vert{} < \epsilon$.