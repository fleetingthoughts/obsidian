---
tags:
  - math
  - real_analysis
  - stephen_abbot
date_created: 2026-03-24
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
With the challenge presented by Thomae and Dirichlet's function, we are motivated to be careful with how we define what it means to take the limit of functions. We now go take limits of functions that do not just have a domain of $\mathbb{N}$ (i.e. sequences). We had first formulated the concept of a limit for the simpler sequences before proceeding to the more general case with functions. The idea of proving a concept with a simpler case (i.e. sequences are just simpler functions), lets establish results early that we can then apply to the more general case. This not only has pedagogical value, but this is an example of developing math by proving a simpler case so that we can apply the results to the general case which we will do for ***Theorem 4.2.3*** in linking sequential limits to functional limits. In this chapter we do the following:
1) Define the functional limit both analytically and topologically
2) Provide a bridge that lets us leverage results for sequences to functional limits: Derive a theorem that shows how the limit of a function depends on the behavior of the image for ALL presupposed convergent sequences in its domain (since limit points are assumed).
3) Show how 2) provides a way for us to provide a counterexample to disprove whether a point is a functional limit
4) Provide corollaries that show the advantage of this definition to permit the usual algebraic operations and avoids the ambiguous situations in the pathological functions such as Thomae and Dirichlet's functions.
Some important things to remember from previous sections:
- limits points do not necessarily belong to a set unless it is closed. 

Definition ***4.2.1*** and ***4.2.1b*** are equivalent definitions. The conversion of the statements in ***4.2.1*** to ***4.2.1b*** are as follows:
- ***4.2.1*** says $|x-c|<\delta \implies |f(x)-f(c)|<\epsilon$
- In the antecedent, setting $|x-c| <\delta$ is equivalent to saying $x \in V_{\delta}(c)$. Note we can do this because we assumed $c$ is a limit point
- In the consequent, saying $|f(x)-f(c)|<\epsilon$ is equivalent to saying $f(x) \in V_{\epsilon}(L)$ where $L=f(c)$ is the limit. 

Some nuances and things to note with these definitions
- The domain does not have to contain its limit points. We only require it to exist, that is, the domain is not necessarily a closed set.
- Because the domain is not necessarily a closed set, we can still determine a limit for a function even if that point does not exist in the domain of the function
- Note that we cannot arbitrarily set $\delta$ to be as large as we want since all the points $x$ have to be in $A$, but it DOES mean that if we establish a $\delta$-neighborhood at all for a certain $\epsilon$-neighborhood, then it has to contain a the smaller $\delta$' neighborhood that simultaneously satisfies the condition of being within the $\epsilon$-neighborhood. This last statement about "all $\delta$-neighborhoods leads to ***Theorem 4.2.3.*** 
***Theorem 4.2.3 (The Sequential Criterion for Functional Limits)*** links sequences to functional limits and, but  in the ii) statement,  it specifies ALL sequences that converge to the limit point must satisfy this property, and this emphasized in ***Corollary 4.2.5*** that states the negation where if we find two converging sequences that do not satisfy the property for a given $\epsilon$, then it must diverge. The theorem and corollary demonstrates how our particular definition completely sidesteps the paradoxical situation of the Dirichlet and Thomae functions by requiring all sequences to the limit point to satisfy the property. The key is in our definition of the functional limit, we required "for all" $x$'s (rather than $\exists$ $x$ ) in the $V_{\delta}(c)$ neighborhood essentially "trapping" and forcing all the $x$'s to satisfy the property.

The algebraic properties of the functional limits is another benefit of our definition. Because we are able to connect the functional limit to the sequential limit, we can leverage the "algebraic properties of limits of sequences" to prove "algebraic properties of limits of functions".
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