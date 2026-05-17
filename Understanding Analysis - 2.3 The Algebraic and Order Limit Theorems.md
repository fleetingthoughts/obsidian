---
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
tags:
  - math
  - stephen_abbot
  - understanding_analysis
  - real_analysis
date_created:
---
Armed with an understanding of the definition of convergence from [2.2 The Limit of a Sequence](Understanding%20Analysis%20-%202.2%20The%20Limit%20of%20a%20Sequence.md), we can prove statements about convergent sequences in general that will form the foundation to derive all the intuitive and useful results in calculus. We are working backwards and deducing properties that will achieve our target results, but we have to start from the beginning. What's important is to know these results are developed with a specific end goal in mind.

It should be noted that the [definition for convergence](Understanding%20Analysis%20-%202.2%20The%20Limit%20of%20a%20Sequence.md) came only 150 years after calculus was developed and so this definition was not necessary for calculus to develop but rather to be used to prove statements about convergence in general. Infinite sequences or series do not necessarily have the same algebraic properties of addition, multiplication, distribution, and/or associative. But we can prove that algebraic operations are valid for infinite sequences or series that have convergent properties.

We first lay some foundations by defining some key terms like "bounded" in the context of sequences.

***Definition 2.3.1 (Bounded sequence).*** A sequence $(x_n)$ is bounded if there exists a number $M>0$ such that $|x_n|\le M$ for all $n \in N$. 

***Definition 2.3.1*** is different from the definition of [bounded above](Understanding%20Analysis%20-%201.3%20The%20Axiom%20of%20Completeness.md) when postulating the Axiom of Completeness. In this definition, we are describing a sequence that is contained within an interval $[-M, M]$. With the definition of boundedness, we prove the following:

***Theorem 2.3.2 (Convergence of bounded sequences).*** Every convergent sequence is bounded.

***Theorem 2.3.2*** is a sufficient condition for a bound to exist and is not necessary, that is, abounded sequence may not converge.

We now show that convergent infinite sequences behave well with respect to addition, subtraction, division, multiplication, and order as a property of the sequences, the limit, behaves as usual under these operations:

***Theorem 2.3.3 (Algebraic Limit Theorem).*** Let  $lim_{n \to \infty}a_n=a$
and $lim_{n \to \infty}b_n=b$. Then we have:
1. $\lim_\limits{n \to \infty}(ca_n)= ca$ = ca, for all $c ∈ R$.
2. $\lim_\limits{n \to \infty}(a_n + b_n) = a + b$; (proved using the triangular inequality).
3. $\lim_\limits{n \to \infty}(a_nb_n) = ab$; (prove using triangular inequality and using the trick of adding extra terms that sum to 0. We also have to apply Theorem 2.3.2).
4. $\lim_\limits{n \to \infty}= a/b$ , provided $b \ne  0$.


# Limits and Order

After showing that convergent sequences are well-behaved under algebraic operations, we show that they also respect order operations:



A remark on the properties we derived for limits. Convergence only depends on the what happens to the "tail-end" of a sequence. Notice that convergence assumes something about the infinite number of terms at the end of the term and excludes a finite number of $n < N_1$ terms. We essentially don't care what we tack on or how many of those finite terms there are as long as we expect a certain behavior from the infinite terms at the "tail-end" of the sequence. Generally we care about what happens "eventually" to a sequence

***Exercise 2.2.7 Eventually*** Given a set $A$, a property is "eventually" in the set if there exists $N_{1} \in N$ such that the property applies to all $a_n \in A$ when $n \ge N_1$ 

# Definitions
***Definition 2.3.1 (Bounded).*** A sequence $(x_n)$ is bounded if there exists a number $M>0$ such that $|x_n|\le M$ for all $n \in N$.

# Theorems

***Theorem 2.3.2 (Convergence of bounded sequences).*** Every convergent sequence is bounded.

***Theorem 2.3.3 (Algebraic Limit Theorem).*** Let  $lim_{n \to \infty}a_n=a$
and $lim_{n \to \infty}b_n=b$. Then we have:
(i)  $lim(ca_n)$ = ca, for all $c ∈ R$; 
(ii) $lim(a_n + b_n) = a + b$; (proved using the triangular inequality)
(iii) $lim(a_nb_n) = ab$; (prove using triangular inequality and using the trick of adding extra terms that sum to 0. We also have to apply Theorem 2.3.2)
(iv) $lim(a_n/b_n) = a/b$ , provided $b \ne  0$ 

***Theorem 2.3.4 (Order Limit Theorem).*** Assume $\lim_{n \to \infty}a_{n} = a$  and $\lim_{n \to \infty} b_n = b$.
1. If $a_n ≥ 0$  for all $n ∈ N$, then $a ≥ 0$.
2. If $a_n ≤ b_n$ for all $n ∈ N$, then $a ≤ b$ (proved by applying theorem 2.3.3)
3. If there exists $c ∈ R$ for which $c ≤ b_n$ for all $n ∈ N$, then $c ≤ b$. Similarly,
4. $a_n ≤ c$ for all $n ∈ N$, then $a ≤ c$.