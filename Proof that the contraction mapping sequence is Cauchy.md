---
parent: "[[Understanding Analysis - 4.3 Continuous Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch4
date_created: 2026-09-27
---
Prove: For a contraction mapping $f : \mathbf{R} \to \mathbf{R}$ with constant $0 < c < 1$ and any $y_1 \in \mathbf{R}$, the sequence defined by $y_{n+1} = f(y_n)$ is a Cauchy sequence.
#### Notes
- Observe that successive differences decay geometrically: $\vert{}y_{n+1} - y_n\vert{} \le c\vert{}y_n - y_{n-1}\vert{} \le \dots \le c^{n-1}\vert{}y_2 - y_1\vert{}$.
    
- For $m > n$, use the triangle inequality to bound $\vert{}y_m - y_n\vert{}$ by a geometric series: $\sum_{k=n}^{m-1} c^{k-1}\vert{}y_2 - y_1\vert{}$.
    
- Evaluate the infinite geometric series bound $\frac{c^{n-1}}{1-c}\vert{}y_2 - y_1\vert{}$, which vanishes as $n \to \infty$ since $c < 1$, proving the sequence is Cauchy
