---
tags:
  - "#math"
  - "#real_analysis"
  - richard_courant
  - "#calculus"
date_created: 2026-02-19
parent: "[[Introduction to Calculus and Analysis I]]"
---
A specific definition of the limit is not offered here, but the author appeals to intuition to show that the sequence $(a_n)=\frac{c}{n}$ for any constant $c$ tends to 0 as $n\to \infty$ and uses this result to  determine the limit of other sequences $(a_{n})$ as $n \to \infty$  and the results are worth remembering:

Taking for granted that the $(1/n)\to 0$, we employ several mathematical tricks that allow us to employ Bernoulli's inequality:
1) $a_{n}=\sqrt[n]{p}=1$. Where $p>0$.  The proof applies the trick of [Bernoulli's inequality](Bernoulli's%20Inequality.md). Courant's proof was not rigorous enough. It presumed the sequence was bounded below by 1 when $p>0$.
2) $a_n= \alpha^n=0$ where $|\alpha|<1$. The trick is to substitute $\alpha = (1+h)^{-n}$ and apply the [Bernoulli's Inequality](Bernoulli's%20Inequality.md)
3) $a_n=\sqrt[n]{n}=1$. Proof again applies a refinement of the [Bernoulli's Inequality](Bernoulli's%20Inequality.md)

# Summary of computational concepts
1) Given an inequality involving integer powers of a number $n>1$, we can decompose it to a sum of two positive numbers $n=1+h$ which allows us to make use of Bernoulli's inequality.