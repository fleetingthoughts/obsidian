---
tags:
  - math
  - calculus
  - theorem
date_created: 2026-04-05
---
Frequently in calculus, we algebraically manipulate a function that is undefined at a point to determine various limits like the derivative. The trick that is commonly employed is to algebraically manipulate it so we have an identical function that just so happens to also be defined at that point so that we can evaluate its limit. There is a subtle theorem that is being taken advantage of here that I prove:

***Let $f$ is continuous but $f(c)$ is not defined. If $f$ is identical to the function $g$ that is continuous on the same domain such that $g(c)$ is defined, then $\lim\limits_{x \to c}f(x)$ exists and is $\lim\limits_{x \to c}f(x)=\lim\limits_{x \to c}g(x)=g(c)$***

Since $g(x)$ is assumed to be continuous over the entire domain such that it is also defined at the point $x=c$ where $f(c)$ is not defined, we have by assumption for any $\epsilon >0$ we can find a $\delta$ such that: $$|x-c|<\delta \implies |g(x)-g(c)|<\epsilon$$
But since $g(x)=f(x)$ is identical everywhere then we can substitute in the $\epsilon$-neighborhood about $g(c)$ so then we also have: $$|x-c|<\delta \implies |f(x)-g(c)|<\epsilon$$
Therefore, $f(x)$ has a limit at $x=c$ and that limit is precisely $g(c)$. 

This proof demonstrates that limits are a neighborhood property that don't really care what happens at a specific point. They only care about what happens at the neighborhood around that point of interest. This theorem justifies why we can evaluate the limit of a function at a point that it is undefined at $x=c$ by using another function that is identical and happens to be defined at $x=c.
