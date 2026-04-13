---
tags:
  - math
  - real_analysis
  - stephen_abbot
date_created: 2026-04-09
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---

# Definitions
***Definition 5.3.7 (Boundless limit).*** Given $g\to R$ and a limit point $c$ of $A$ that is not necessarily in $A$, we say that $lim_{x \to a}g(x)=\infty$ if there exists an $M >0$ such that we can find a $\delta >0$ so that $g(x)$ is larger than that $M$. That is given the challenge of an $M$, we can find a $\delta$ such that $$0<|x-c|<\delta \implies g(x)\ge M$$

# Theorems
***Theorem 5.3.1 (Rolle's Theorem).*** Let $f: [a,b,]\to R$ be continuous on $[a,b]$ and differentiable on $(a,b)$. If $f(a)=f(b)$ then there exists a point $c\in (a,b)$ such that $f'(c)=0$.

***Theorem 5.3.2 (Mean Value Theorem).*** Let $f: [a,b,]\to R$ be continuous on $[a,b]$ and differentiable on $(a,b)$. There exists a point $c \in (a,b)$ such that the derivative equals the difference quotient over the entire interval, that is: $$\frac{f(b)-f(a)}{b-a}=f'(c)\text{\quad for }c\in(a,b)$$
***Corollary 5.3.3 to the Mean Value Theorem (sufficient condition to show a function is a constant).*** Let $f: [a,b,]\to R$ be continuous on $[a,b]$ and its derivative $g'(x)=0$ for all $x\in [a,b]$, then $g(x)=k$ for some $k\in \mathbb{R}$ 

***Corollary 5.3.4 to the Mean Value Theorem (Sufficiency condition to show 2 functions only differ by a constant).*** If $f$ and $g$ are differentiable on $A$ with $f'(x)=g'(x)$ for $x\in A$, then $f(x)=g(x)+k$ for some $k\in \mathbb{R}$

***Theorem 5.3.5 (Generalized Mean Value Theorem).*** Let $g,f: [a,b,]\to R$ be continuous on $[a,b]$ and differentiable on $(a,b)$. There exists a point $c \in (a,b)$ such that: $$\frac{f'(c)}{g'(c)}=\frac{f(b)-f(a)}{g(b)-g(a)}$$
***Theorem 5.3.6 (L'Hospital's Rule for the 0/0 indeterminate form).*** If functions $f,g$ have the following assumptions:
1) Continuous in an interval containing $x=a$
2) Differentiable in the same interval but possibly NOT differentiable at the point $a$
3) $f(a)=g(a)=0$
Then we have the following sufficiency condition: $$\lim_{ x \to a }\frac{f'(x)}{g'(x)}=L \implies \lim_{ x \to a } \frac{f(x)}{g(x)}=L$$

***Theorem 5.3.8 (L'Hospital's Rule for the $\infty$/$\infty$  indeterminate form).*** If functions $f,g$ have the following assumptions:
-  Continuous in an interval containing $x=a$
- Differentiable in the same interval but possibly NOT differentiable at the point $a$
- $\lim_{ x \to a }g(a)=\infty$ (or $-\infty$)
Then we have the following sufficiency condition: $$\lim_{ x \to a }\frac{f'(x)}{g'(x)}=L \implies \lim_{ x \to a } \frac{f(x)}{g(x)}=L$$