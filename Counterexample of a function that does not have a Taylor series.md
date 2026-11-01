---
parent: "[[Understanding Analysis - 6.6 Taylor Series]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Construct a counterexample demonstrating: An infinitely differentiable function on $\mathbf{R}$ whose Taylor series centered at $0$ converges everywhere on $\mathbf{R}$, yet equals the function only at $x = 0$.
#### Notes
Define $g: \mathbf{R} \to \mathbf{R}$ by:

$$g(x) = \begin{cases} e^{-1/x^2} & x \neq 0 \\ 0 & x = 0 \end{cases}$$

Since $g^{(n)}(0) = 0$ for all $n \ge 0$, its Maclaurin series is identically $0$, which converges everywhere on $\mathbf{R}$ to $0$, whereas $g(x) \gt 0$ for all $x \neq 0$.
