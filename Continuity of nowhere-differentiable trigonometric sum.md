---
parent: "[[Understanding Analysis - 6.4  Series of Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: The series $g(x) = \sum_{n=0}^{\infty} \frac{\cos(2^n x)}{2^n}$ is continuous on $\mathbf{R}$.
#### Notes
For all $x \in \mathbf{R}$, $\vert{}\frac{\cos(2^n x)}{2^n}\vert{} \le \frac{1}{2^n}$. Setting $M_n = \frac{1}{2^n}$, the series of constants $\sum_{n=0}^{\infty} M_n$ is a convergent geometric series. By the Weierstrass M-test, $g(x)$ converges uniformly on $\mathbf{R}$. Because each term $\frac{\cos(2^n x)}{2^n}$ is continuous, the uniform limit $g(x)$ is continuous on $\mathbf{R}$.
