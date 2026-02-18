---
tags:
  - "#math"
  - "#real_analysis"
  - "#understanding_analysis"
  - "#stephen_abbot"
date_created: 2026-02-16
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
The issue with double summations and double products of infinite series is related to the problem of rearrangement discussed in [Understanding Analysis - 2.7 Properties of Infinite Series](Understanding%20Analysis%20-%202.7%20Properties%20of%20Infinite%20Series.md). We have a choice in how we want to order the iterations in a double summation, but Abbot shows a counter-example with an infinite matrix that:
$$\Sigma_{j=1}^{\infty}\Sigma_{i=1}^{\infty}a_{ij} \ne \Sigma_{i=1}^{\infty}\Sigma_{j=1}^{\infty}a_{ij}$$
In other words, just like in the single index case, our rearrangement of the terms in the infinite series matters as addition is not necessarily commutative in an infinite series. As we have shown in Chapter 2.7, the condition for the limit being immutable under rearrangement of the sums is absolute convergence and it is the same here.

***Theorem 2.8.1. (Condition for the limit of a double summation to be immutable under rearragement).*** Let $\{a_{ij}: i, j \in \mathbb(N)\}$ be a doubly indexed array of real numbers. If the series absolutely converges, that is if:
$$\Sigma_{j=1}^{\infty}\Sigma_{i=1}^{\infty}|a_{ij}|$$
converges, then any rearrangement of the summation converges to the same limit:
$$\\lim_{ n \to \infty } s_{nn} =\Sigma_{j=1}^{\infty}\Sigma_{i=1}^{\infty}a_{ij} = \Sigma_{i=1}^{\infty}\Sigma_{j=1}^{\infty}a_{ij}
$$

where 
$$s_{nn} = \Sigma_{j=1}^{n}\Sigma_{i=1}^{n}a_{ij}$$
The [[proof of the convergence of a double summation by absolute convergence]] is closely related to our proof for an single-index infinite series in 2.7

# Product of Series
Similar to the issue with double summation, we face the same issue with the product of series in how we choose to commute the additions. One particular rearrangement of the terms of the addition is the Cauchy product:

***Unofficial Definition (Cauchy Product).*** Given two infinite series $\Sigma_{i=1}^{\infty}b_{i}$ and $\Sigma_{j=1}^{\infty}a_{j}$, the Cauchy Product commutes the terms of the product of the two series as follows:
$$(\Sigma_{i=1}^{\infty}b_{i})(\Sigma_{j=1}^{\infty}a_{j})= (a_1+a_2+a_3+...)(b_1+b_2+b_3+...)$$
$$= a_1b_1 + (a_1b_2+a_2b_1)+(a_3b_1+a2b_2+a_1b_3)$$
$$=\Sigma_{k=2}^{\infty}d_{k} \text{\quad where \quad}d_{k}=a_1k_{k-1}+a_2b_{k-2}+...+a_kb_1$$
But this is just one choice of rearrangement and again the condition of absolute convergence will equate the Cauchy Product with other ways to iterate the summation:

***Exercise 2.8.7 (Convergence of the product of an Infinite Series).*** If $\Sigma_{i=1}^{\infty}b_{i}$ and $\Sigma_{j=1}^{\infty}a_{j}$ converges absolutely to $B$ and $A$ respectively, then $\Sigma_{j=1}^{\infty}\Sigma_{i=1}^{\infty}|a_{i}b_j|$ also absolutely converges. Therefore applying Theorem 2.8.1, we then find any rearrangement of the sum converges to the same limit. We also find that:
$$\lim_{ n \to \infty } s_{nn}=\Sigma_{j=1}^{\infty}\Sigma_{i=1}^{\infty}a_{i}b_{j}=\Sigma_{i=1}^{\infty}\Sigma_{j=1}^{\infty}a_{i}b_{j} AB
$$
Therefore by Theorem 2.8.1:
$$
\lim_{ n \to \infty }  s_{nn} = \lim_{ n \to \infty } \Sigma_{j=1}^{n}\Sigma_{i=1}^{n}a_{i}b_{j}=\Sigma_{i=1}^{\infty}\Sigma_{j=1}^{\infty}a_{i}b_{j}=\Sigma_{k=2}^{\infty}d_{k}=AB
$$
where $\Sigma_{k=2}^{\infty}d_{k}$ is the Cauchy Product.




