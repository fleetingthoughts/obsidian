---
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
tags:
  - math
  - stephen_abbot
  - understanding_analysis
  - real_analysis
date_created:
---
We look at conditions that tell us whether a sequence converges. We begin by defining some of these conditions:

***Definition 2.4.1 (Monotonicity).*** A sequence $(a_n)$ is increasing if for all $n \in N$, $a_n \le a_{n+1}$ and decreasing if $a_n \ge a_{n+1}$. The sequence is called <u>monotone</u> if it is increasing or decreasing for all terms in this way.

With this definition we now establish a condition for convergence that <u>doesn't require us to know what beforehand what the limit is</u>

***Theorem 2.4.2 (Monotone Convergence Theorem).*** If a sequence is bounded and is monotone, then the sequence converges.

The proof involves choosing a candidate for the limit and we choose the supremum of the sequence $s = sup( {a_n: n \in N})$ and then applying [lemma](Understanding%20Analysis%20-%201.3%20The%20Axiom%20of%20Completeness.md#^e12bd5) to then show that:
$$s-\epsilon \le a_{N}\le a_{n} \le s \le s+\epsilon$$
which shows we satisfy the convergence criteria $|a_n-s|\lt \epsilon$ for some $n\gt N$. This proof also happens to show that<u> the supremum/Infinium of a monotonically increasing/decreasing sequence is the limit that the sequence converges to</u>

Armed with this theorem, we now formalize a relationship between sequences and series so that we can apply all our theorems for infinite sequences to an infinite series.

***Definition 2.4.3 (Convergence of a Series as a Convergence of a Sequence of its Partial Sums).*** Let $(b_n)$ be a sequence. An infinite series is a formal expression of the form
$$\sum_{n=1}^{\infty}b_{n}=b_{1}+b_{2}+\dots$$
With the partial sums $(s_m)$ defined as 
$$s_{m}=\sum_{n=1}^{m}b_{n}=b_{1}+b_{2}+\dots+b_{m}$$
We say the infinite series converges if the sequence $(s_m)$ converges to a real number $B$ .

Theorem 2.4.2 lets us determine that the series of $\frac{1}{n^2}$ converges but in trying to show divergence for a series like the harmonic series diverges, we cannot use the Theorem at all. Note that we did not prove that if the series is NOT bounded diverge or if we simply can't find a bound.  We are motivated to find a ***"if and only if"*** condition so that we can prove that a series actually diverges when we cannot find a bound and apply 2.4.3

***Theorem 2.4.6 (Cauchy Condensation Test: if and only if condition of convergence to prove a series can diverge).*** Suppose each term of the series $(b_n)$ is decreasing and satisfies ${b_n}\ge 0$ for all $n\in N$, then the series converges ***if and only if*** the following series converges:
$$\sum_{n=0}^{\infty}2^{n}b_{n}=b_{1}+2b_{2}+4b_{4}+8b_{8}\dots$$
Notice that we're not summing every $(b_n)$ term but rather every $2^k$ -th term.
***Proof.*** First we do the forward proof and show that if this special series converges, then the original $(s_m)$ series must converge. The forward proof takes advantage of the fact that each $b_n$ term is decreasing so we can replace each term in the series with a larger terms to produce an upper bound and satisfy Theorem 2.4.3 condition for convergence:
$$\sum_{n=0}^{\infty}b_{n}=b_{1}+b_{2}+b_{3}+b_{4}+b_{5}+b_{6}+b_{7}\dots$$$$\sum_{n=0}^{\infty}b_{n}=(b_{1})+(b_{2}+b_{3})+(b_{4}+b_{5}+b_{6}+b_{7})+\dots+(b_{2^k}+\dots+b_{2^{k+1}-1})$$ By grouping the terms into $2^{k}$ terms like this we can then replace each term within each bracket with the largest term to give us an upper bound.
$$\le \sum_{n=0}^{\infty}b_{n}=(b_{1})+(b_{2}+b_{2})+(b_{4}+b_{4}+b_{4}+b_{4}+b_{4})+\dots+(b_{2^k}+b_{2^k})$$
Notice that the above term must have two times less terms than the original sum. And with this new series as an upper bound, we already have by hypothesis that it converges and has a bound so then the original series must have a bound.

Some interesting notes from doing the exercises:
- ***Exercise 2.4.1 and 2.4.2 (Solving the limit of recursive sequence).*** We look at the sequence $(x_n)$ defined recursively by $x_{n+1}=f(x_n)$. 
	1) If the sequence is shown to converge, 
	2) It can be proven that $\lim x_{n+1}=\lim x_n=L$ so that 
	3) We can solve for $L$ by the equation $L=f(L)$ 
- ***Exercise 2.4.5:*** [[Newton's method or the Babylonian method for calculating Square Roots]]
- ***Exercise 2.4.6:*** [[The inequality of the arithmetic mean and geometric mean (AM-GM inequality)]] 


# Definitions
***Definition 2.4.1 (Monotonicity).*** A sequence $(a_n)$ is monotonically increasing if $a_{n}\le a_{n+1}$. A sequence is monotonically decreasing if $a_{n+1} \le a_{n}$. A monotonic sequence is either of these two. 

***Definition 2.4.3 (Convergence of a Series as a Convergence of a Sequence of its Partial Sums).*** Let $(a_n)$ be an infinite sequence. An infinite series is defined as the infinite summation of the sequence: $$\sum_{i=1}^{\infty}a_i=a_{1}+a_{2}+a_{3}+\dots$$
The partial sums are the sequence of $(s_m)$ that are the sums of the first $m$ terms: $$s_{m}=\sum_{i=1}^{m}a_i=a_{1}+a_{2}+a_{3}+\dots+a_{m}$$ An infinite series is said to converge if the sequence of its partial sums $(s_m)$ converges.
# Theorems
***Theorem 2.4.2 (Monotone Convergence Theorem).*** A sequence that is monotonic and bounded is guaranteed to converge.

***Theorem 2.4.6 (Cauchy Condensation Test: equivalence condition for convergence of an infinite series).*** Given an infinite sequence $(b_n)$, the infinite series of the sequence converges if and only if the following conditions are satisfied:
1) $b_{n+1}\le b_{n}$ $\forall n$
2) $0\le b_{n}$ $\forall n$ 
3) The following modified sum converges: $$\sum_{k=0}^{\infty}2^kb_{2^k}= b_{1}+2b_{2}+4b_{4}+8b_{8}+16b_{16}+32b_{32}+\dots$$ 
