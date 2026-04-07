---
tags:
  - math
  - real_analysis
  - stephen_abbot
date_created: 2026-04-07
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
fd
# Definitions
***Definition 5.2.1 (Differentiability).*** Let $g: A\to \mathbb{R}$ be a function on an interval $A$. Given $c\in A$, the derivative of $g$ at $x=c$ is defined by the following if it exists: $$g'(c)=\lim_{ x \to c }\frac{g(x)-g(c)}{x-c}$$
If this limit exists, we say "$g$ is differentiable at $c$. If $g$ is differentiable on all $x\in A$ then we say $g$ is differentiable on $A$.
# Theorems
***Theorem 5.2.3 (Differentiability at a point is sufficient for continuity at a point).*** If $g: A\to \mathbb{R}$ is differentiable at $x=c$, then it is continuous at $x=c$ as well. Furthermore, $\lim\limits_{x \to c}g(x)=g(c)$

***Theorem 5.2.4 (Algebraic properties of differentiable functions).*** Let $f$  and $g$ be functions defined on an interval $A$, and assume both are differentiable at the same point $c\in A$. Then the following properties are satisfied:
1) <u>Addition property:</u> $(f+g)'(c)=f'(c)+g'(c)$
2) <u>Scalar multiplication: </u>$(kf)'(c)=kf'(c)$ for $k\in \mathbb{R}$ 
3) <u>Muliplicative property:</u> $(fg)'(c) =f'(c)g(c)+f(c)g'(c)$
4) <u>Divisive property</u>: $(f/g)'(c)=\frac{g(c)f'(c)-f(c)g'(c)}{[g(c)]^2}$

***Theorem 5.2.5 (Chain Rule).*** Let $f : A → \mathbb{R}$ and $g : B → \mathbb{R}$ satisfy $f(A) ⊆ B$ so that the composition $g ◦ f$ is defined. If $f$ is differentiable at $c ∈ A$ and if $g$ is differentiable at $f(c) ∈ B$, then $g ◦ f$ is differentiable at $x=c$ as $(g \circ f)'(x)=g'(f(c))f'(c)$

***Theorem 5.2.6 (Interior Extremum Theorem. Also known as Fermat's Theorem).*** Let f be differentiable on an open interval $(a, b)$. If $f$ attains a maximum value at some point $c ∈ (a, b)$
(i.e., $f(c) ≥ f(x)$ for all $x ∈ (a, b)$), then $f'(c)=0$. The same is true if $f(c)$ is a minimum value.

***Theorem 5.2.7 (Darboux’s Theorem).***
# Invoked Theorems

