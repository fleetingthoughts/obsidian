---
tags:
  - real_analysis
  - math
  - stephen_abbot
date_created: 2026-03-28
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
The chapter explores some useful results of continuous mappings and specifically the results that come from the mapping of compact sets. The chapter is outlined as follows:
- Properties of sets (compactness, openness, etc..) in the domain that are in the image preserved when <u>mapped by a continuous function</u>
- What continuous mapping of a compact domain can tell you about the behavior of the function: the extreme value theorem.
- Uniform continuity and equivalent conditions to disprove whether a function is uniformly continuous or not
- Criteria for a uniformly continuous function: continuous mapping of a compact set.

When a set gets mapped, in general some of the set properties of the domain gets lost. For instance, open intervals and closed intervals do not always stay open or closed which can be shown by example. For an open set, the function $f(x) = x^2$ that maps the open interval $(1,-1)$ to a half open interval $[0,1)$. For a closed set we consider  the function $$g(x)=\frac{1}{1+x^2}$$
and it maps $[0,\infty]$ to (0,1]. 

The fact we had to use an unbounded closed interval to show closedness is not preserved is not a coincidence. ***Theorem 4.4.1.*** shows that compactness gets preserved from the domain to the image. The proof of this is a direct proof by non-construction to show that it contains all its limit points by showing any convergent subsequences in $f(K)$ also contains its limit points.:
1) Assume mapping is continuous in the domain and domain is compact (i.e. contains its limit points and is bounded so it must have limit points).
2) Now take any limit point in $f(K)$ say $y= f(x)$. 
3) Make use of continuity of $f$ to show that if there is a converging subsequence $(x_n)\to x$ then $y_n \to f(x)$. Continuity of $f$ shows that the image has limit points in $f(x)$. This is equivalent to showing it is bounded.
4) Make use of the fact that the domain $K$ is compact so $x$ must be contained so that $f(x)$ exists as well in the image. Compactness of the domain shows that the image must contain its limit points.

A consequence of the preservation of compactness in the mapping of a continuous function is an important existence theorem called the Extreme Value theorem ***Theorem 4.4.2.*** The theorem establishes the existence of a maximum and minimum in the image and is proven as follows
1) Because the image is compact, it is bounded therefore the AoC is satisfied and there is a supremum
2) Because the image is compact, it contains its limit points, so it contains the supremum as well. (this is formalized in Exercises 3.3.1).

***Definition 4.4.4*** defines a special kind of continuity that is stronger called uniform continuity. Colloquially, this property specifies that the modulus of continuity $\delta$ is independent of the point $x$ chosen and only depends on the $\epsilon$ we desire. Therefore if we want to say be $\epsilon <0.01$ close to point, then for a uniformly continuous function, if we find a $\delta$ that satisfies that condition for one $x=c$ it satisfies it for all $x$'s.

The first thing to do is to show how we can identify uniform continuity by showing how we can disprove it. ***Theorem 4.4.5*** shows how we can disprove uniform continuity by finding two sequences that converge to the same point in the domain but do not when we take their images. The theorem is a direct negation of the definition of uniform continuity (***Definition 4.4.4***) but expressed as sequences. Where uniform continuity requires $|x-y| < \delta \implies |f(x)-f(y)|<\epsilon$, the theorem essentially states that a function is not uniformly continuous if we find a counterexample where the condition is not satisfied.

***Theorem 4.4.7.*** then shows how we can prove a function is uniformly continuous by showing it is a continuous mapping of a compact set. For example, any continuous function that maps a closed interval is uniformly continuous in that interval. The proof of this is a proof by contradiction by supposing we have a situation described in ***Theorem 4.4.5***:
1) Goal. Assume $f$ is not uniformly continuous so that by ***Theorem 4.4.5***, we found a counterexample where $|x_n-y_n| < \delta$ such that $|f(x_n)-f(y_n)|\geq\epsilon_{0}>0$  and a contradiction results
2) Use the same logic we used for the proof of ***Theorem 4.4.1.*** because the domain is a compact set, we can always construct sequences that converge to the same limit point $x$. For example say $x_n$ is a subsequence then $y_n$ can be a subsequence of $x_n$ (i.e. a "subsubsequence"). Compactness of the domain implies we always have a convergent subsequence $\lim\limits_{n \to \infty}x_n = \lim\limits_{n \to \infty}y_n=x$ and that we also have limit points $f(x)$ in the image as well by ***Theorem 4.4.1.***
3) Because the mapping is continuous if $x$ is a limit point of the domain, $f(x)$ is a limit point in the image that we can be arbitrarily close to. Continuity of $f$ shows that the image has limit points in $f(x)$.
4) But point 3) contradicts our assumption in 1) which says that there will be a $\epsilon_o$ which we cannot shrink past. So we illustrate there's a contradiction if we assume the function is not uniformly continuous

# Definitions
***Definition 4.4.4 (Uniform Continuity).*** A function $f:A \to \mathbb{R}$ is uniformly continuous on $A$ if for every $\epsilon > 0$, there exists a $\delta >0$ such that for all $x, y \in A$, we have $|x-y|<\delta \implies |f(x)-f(y)| <\epsilon$ 
# Theorems
***Theorem 4.4.1 (Preservation of Compact Sets).*** Let $f: A \to \mathbb{R}$, then if there is a compact subset of the domain $K \subseteq A$, then the image of that subset is compact, that is $f(K)$ is a compact set as well.

***Theorem 4.4.2 (Extreme Value Theorem: The existence of a maximum and minimum).*** If $f: K \to \mathbb{R}$ is continuous on a compact set $K \subseteq \mathbb{R}$, then $f$ attains a maximum and minimum value. In other words, there exists $x_o, x_1 \in K$ such that $f(x_0) \le f(x) \le f(x_1)$ for all $x\in K$.

***Theorem 4.4.5 (Sequential Criterion to disprove uniform continuity).*** A function $f: A\to \mathbb{R}$ fails to be uniformly continuous on $A$ <u>if and only if</u> there exists a particular $\epsilon_o>0$ and two sequences $(x_n)$ and $(y_n)$ in $A$ such that the following is observed: $$|x_{n}-y_{n}| \text{\quad but \quad}|f(x_{n})-f(y_{n})|>\epsilon_{o}$$

***Theorem 4.4.7 (Criteria for uniform continuity using compact sets).*** A function that is continuous on a compact set $K$ is uniformly continuous on $K$.
