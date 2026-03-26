---
tags:
  - math
  - real_analysis
date_created: 2026-03-26
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---

# Definitions
***Definition 4.3.1 (Continuity)*** A function $f:A \to R$ is "continuous at a point $c\in A$"  if for all $\epsilon>0$, there exists a $\delta >0$ such that: $$|f(x)-f(c)| <\epsilon \text{\quad if \quad} |x-c|<\delta$$
# Theorems
***Theorem 4.3.2 (Equivalent statements to the condition of continuity).*** Let $f: A\to \mathbb{R}$, and let $c\in A$. The function $f$ is continuous at $c$ if and only if any of the three conditions is met:
1) For all $\epsilon>0$ there exists a $\delta$ such that when $|x-c|< \delta$ then $|f(x)-f(c)|<\epsilon$ and $x\in A$.
2) For all $V_{\epsilon}(f(c))$ there exists a $\delta$ such that whenever $x\in V_\delta(c)$ and $x\in A$ then $f(x) \in V_{\epsilon}(f(c))$ 
***Corollary 4.33 (Criterion for Discontinuity).*** Let $f: A\to \mathbb{R}$, and let $c\in A$ be a limit point of $A$. If there exists a sequence $(x_n)\subseteq A$ where $(x_n)\to c$ such that $f(x_n)$ does not converge to $f(c)$, then $f$ is not continuous at $x=c$ 

***Theorem 4.3.4 (Algebraic Continuity Theorem).*** Assume $f: A\to R$ and $g: A\to R$ are continuous at point $c\in A$. Then we have the following properties:
- Scalar multiplication: $kf(x)$ is continuous at $c$ for all $k\in \mathbb{R}$
- Addition of continuous functions: $f(x)+g(x)$ is continuous at $c$
- Multiplication of continuous functions: $f(x)g(x)$ is continuous at $c$
- Division of continuous functions: $f(x)/g(x)$ is continuous at $c$, provided the quotient is defined