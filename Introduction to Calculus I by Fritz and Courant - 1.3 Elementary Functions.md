---
tags:
  - "#calculus"
  - "#real_analysis"
  - "#math"
  - "#richard_courant"
date_created: 2026-02-17
parent: "[[Introduction to Calculus and Analysis I]]"
---
An important property is that compound functions are continuous if the functions that make it up are continuous as well. 

***Theorem on Continuity of Compound functions (p.55).*** Given the compound function $g(\theta(x))=f(x)$, $f(x)$ is continuous if $g$ and $\theta$ are.

Proof. For by the definition of continuity we must satisfy: $$|f(x)-f(x_{o})| = |g(\theta(x))-g(\theta(x_0))| \lt \epsilon \text{\quad for \quad }|\theta(x)-\theta(x_o)| < \delta$$
Since $g$ is continuous, it can be made arbitrarily small granted if we can make $\theta(x)$ within the desired $\delta$ but this is also guaranteed as $\theta$ is continuous and can be made arbitrarily small as long as we make $x$ close enough to $x_o$ proving that $f$ is continuous.

This also gives us a direct way of proving the continuity of functions that we can break down into smaller parts. For example, the function $\sqrt{1-x^2}$ is a compound of two functions, $\sqrt{x}$ and $1-x^2$ that we can more easily prove the continuity of individually.
