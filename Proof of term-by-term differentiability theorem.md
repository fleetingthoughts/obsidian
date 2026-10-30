---
parent: "[[Understanding Analysis - 6.4  Series of Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: Let $f_n$ be differentiable functions defined on an interval $A$. If $\sum_{n=1}^{\infty} f_n'(x)$ converges uniformly to $g(x)$ on $A$, and there exists $x_0 \in A$ where $\sum_{n=1}^{\infty} f_n(x_0)$ converges, then $\sum_{n=1}^{\infty} f_n(x)$ converges uniformly to a differentiable function $f(x)$ satisfying $f'(x) = g(x)$ on $A$.
#### Notes
- Define the partial sums $s_k(x) = \sum_{n=1}^k f_n(x)$ and their derivatives $s_k'(x) = \sum_{n=1}^k f_n'(x)$.
    
- Apply the strong differentiable limit theorem to the sequence of differentiable partial sums $(s_k)$.
    
- Because $(s_k')$ converges uniformly to $g$ on $A$ and $(s_k(x_0))$ converges at a point $x_0 \in A$, the theorem guarantees $(s_k)$ converges uniformly.
    
- Conclude the uniform limit $f(x)$ is differentiable and satisfies $f'(x) = g(x)$.
