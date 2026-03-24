---
tags:
  - math
  - real_analysis
  - stephen_abbot
date_created: 2026-03-24
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
With the challenge presented by Thomae and Dirichlet's function, we are motivated to formalize what it means to take the limit of functions that do not just have the domain of $\mathbb{N}$ (i.e. sequences),  so that we can avoid the ambiguous situations they present. In this chapter we do the following:
- Define the functional limit both analytically and topologically
- Derive a theorem that shows how the limit of a function depends on the possible sequences in its domain
- Provide corollaries that show the advantage of this definition to permit the usual algebraic operations and avoids the ambiguous situations in the pathological functions such as Thomae and Dirichlet's functions.

Some important things to remember from previous sections:
- limits points do not necessarily belong to a set unless it is closed. 
# Definition
***Definition 4.2.1 (Functional limits or limits on functions).*** Let $f:A\to \mathbb{R}$ be a function and c be a limit point on the domain of $A$. We say that $\lim_{x\to c}f(x)=L$ if for any arbitrary $\epsilon >0$, we can find a $\delta$ such that we have the following: $$|f(x)-f(c)|<\epsilon \text{\quad for all }  x \in A \text{ such that \quad}  0 < |x-c| <\delta$$
***Definition 4.2.1B (Topological definition of functional limit).*** Let $c$ be a limit point in $A$ that is a domain of $f: A\to \mathbb{R}$. We say that $\lim_{x\to c}f(x)=L$ if for every $\epsilon$-neighborhood $V_{\epsilon}(L)$, there exists a $\delta$-neighborhood such that all $x\in V_{\delta}(c)$ contained in $A$ but different from $c$ with the property that $f(x) \in V_{\epsilon}(L)$ 
# Theorem
***Theorem 4.2.3 (Criteria for Functional Limits using Sequences).*** Given the a function $f: A\to R$, where the domain has a limit point $c$ that it does not necessarily contain. Then the following two statements are equivalent:
1) $\lim\limits_{ x \to c } f(x)=L$
2) For ALL sequences $(x_n)$ that converges to $c$, it follows that the sequence $f(x_n)$ converges to $L$.
***Corollary 4.2.4 (Algebraic Limit Theorem for Functional Limits).*** Let $g$ and $f$ be defined on the same domain $A \subseteq \mathbb{R}$, and assume $\lim_{x\to c}f(x)=L$ and $\lim_{x\to c}g(x)=M$. Then we have the following properties:
- Scalar multiplication: $\lim\limits_{ x \to c } kf(x)=kL$
- Additive properties: $\lim\limits_{ x \to c } [f(x)+ g(x)]=L+M$
- Multiplicative properties $\lim\limits_{ x \to c }[f(x)g(x)]=LM$
- Divisive properties $\lim\limits_{ x \to c }\frac{f(x)}{g(x)}=\frac{L}{M}$ provided that $M \ne 0$ 
***Corollary 4.2.5.*** Given the a function $f: A\to R$, where the domain has a limit point $c$ that it does not necessarily contain, if there exists two sequences $(x_n)$ and $(y_n)$ in $A$ with $x_n\ne c$ and $y_n \ne c$. Then the function diverges if we find the following:$$\lim_{ n \to \infty }x_{n}=\lim_{ n \to \infty } y_{n}=c \text{\quad but \quad} \lim_{ x \to c }f(x_{n})\ne \lim_{ x \to c }f(y_{n}) $$