---
tags:
  - math
  - calculus
  - richard_courant
date_created: 2026-04-18
parent: "[[Introduction to Calculus and Analysis I]]"
---
The chapter goes through several examples of integration by parts, but there are 3 outstanding topics to consider:
- The integral formula for $f(a)+f(b)$.
- Recursive formulae.
- Wallis's Infinite product for $\pi$.
Instead of the fundamental formula which expresses $f(b)-f(a)$ as a integral, we use integration by parts to express $f(a)+f(b)$ as an integral.  The trick is to introduce a new function $(x-m)$ for some constant $m$. We then set up the formula: $$f(x)(x-m)=\int f(x)dx+\int(x-m)f'(x)dx$$
Unravelling this so that we translate it for the definite integral from $a$ to $b$ and then choosing $m=(a+b)/2)$ we then obtain: $$\frac{b-a}{2}[f(a)+f(b)]=\int^b_{a} f(x)dx+\int^b_{a}(x-m)f'(x)dx$$

The recursive formulae for $\sin^n(x)$ is useful to compute $\pi$.

# Notes from exercises
- Problem 1 demonstrates $\int x^n e^{-x^2}$ can be reduced to elementary functions if $n$ is a positive odd number. 
- Problem 3 and 4 forms Cauchy's formula for repeated integration which lets us reduce repeated integration into a single integral.


