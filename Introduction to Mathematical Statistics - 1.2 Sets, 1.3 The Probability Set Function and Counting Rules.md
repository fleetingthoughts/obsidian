---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - math
  - statistics
  - robert_hogg
date_created:
---
# 1.3 The Probability Set Function
In this chapter, we establish probabilities of events that are [countable](Understanding%20Analysis%20-%201.5%20Cardinality.md) and the rules associated with counting them. There are technicalities with ascribing probabilities to infinite sample spaces outside the scope of this book so we constrain ourselves to collection of events that are closed under complements and countable unions. DeMorgan's Laws then state that the collection is also closed under countable intersections. Such a collection of "countable" events that this section will concern itself with is called a $\sigma$ -field of subsets


The mathematical definition of probability and the probability set function relies on Kolmogorov's probability axioms in ***Definition 1.3.1*** and from these axioms, we can develop several properties of the probability set function for a collection of events $A$ and $B$ in the sample space:
- ***Theorem 1.3.1***: Complement rule
- *Theorem 1.3.2:* Probability of an impossible event
- ***Theorem 1.3.3***: The Monotonicity property of probability set functions
- ***Theorem 1.3.4***: The boundedness of probability
- ***Theorem 1.3.5***: The General Addition Rule of probability set functions.
	- The intuitive leap to prove theorem 1.3.5 is a sort of strategic addition of zero by taking advantage of the [[Absorption laws]]

## 1.3.1 Counting Rules
Three counting rules from elementary algebra for a set $A$ containing $n$ elements:
1) <u>Multiplication rule</u>: Given set $A= \{x_1, x_2,...x_{m}\}$ and $B=\{y_1,y_2,..., y_n\}$, then then there are $m \times n$ ordered pairs $(x_i, y_j)$. This is [the cartesian product](Book%20of%20Proof%20-%201%20Real%20Numbers.md) of $A \times B$ 
2) <u>Permutations. </u>The k-tuple permutation of a set $A$ with $n$-elements is the set of k-tuples containing unique elements of the set $A$  is the permutation denoted $P^{n}_{k}=\frac{n!}{(n-k)!}$. Note that for tuples, the order of the elements make them distinct for each other for a 3-tuple $(x_1,x_2,x_3) \ne (x_2, x_1, x_3)$, but note that the permutations demand that components within the tuple do not repeat so $(x_1,x_1, x_2)$ is not a permutation of $A$. The permutation set is a subset of all the possible k-tuples of $A$ which by the <u>multiplication rule</u> is $n^k$ 
3) <u>Combinations</u>. The number of subsets containing $k$ elements of the set $A$ is the combination denoted $C^{n}_{k}=\frac{n!}{k!(n-k)!}$=$\binom{n}{k}$ . The combinations is a subset of the permutations of $A$,  $\{P^{n}_{k}\}$ as the combinations are essentially permutations where we do not care for the ordering. We are no longer looking at ordered k-tuples but just the sets containing k-elements. Another way to see this is to take any given permutation of k-tuples and see that each of them can be ordered $k!$ different ways.
## 1.3.2 Additional properties of probability

***Theorem 1.3.6*** establishes the <u>conditions that allow us to interchange the limit and the probability set function.</u>:
- If a union of sets is nondecreasing and converges to a singular set, then computing the probability of the infinite union is equivalent to computing the probability of that singular convergent set that contains all the elements of the sequence (e.g. $A_n = [0, 1- 1/n]$ )
- If an intersection of sets is decreasing and converges to a singular set, then computing the probability of the infinite intersection of the set is the same as computing the probability of that final converging set.

Boole's inequality gives us an <u>inequality relation between arbitrary unions and the probabilities of the components of that union</u>. Boole's inequality can intuitively be seen as the sum of probabilities of a collection is valid if the events are disjoin from each other, so once we take the union of these collection of events, then there may be overlapping events so the probability of this union is less. This inequality gives us a universal upper bound for the probability on the union of countable sets.

As a final corollary, we can extend theorem 1.3.5 to more than just two events: 

***Remark 1.3.2 (Inclusion Exclusion Formula)***. 
$$P(C_{1}\cup C_{2} \cup C_{3})=p_{1}-p_{2}+p_{3}$$
where:
$p_{1} = P(C_{1})+ P(C_2)+P(C_3)$
$p_2 = P(C_1 \cap C_2) + P(C_1 \cap C_3) + P(C_2\cap C_3)$
$p_3 = P(C_1 \cap C_2 \cap C_{3})$

Put in words, every $p_k$ is just a summation of all the possible intersections between $k$-number of collections so the summation will have $C^n_k$ combinations. We obviously don't care about the ordering of the intersections! Proof of this corollary is in Exercise 1.3.9

It can be seen that $p_k\le p_{k-1} \le \dots \le p_2 \le p_1$ by Boole's inequality. 

For the Inclusion Exclusion formula in the case where $k=2$ we can derive a special inequality using the axiom for probability set functions:
$$P(C_1 \cap C_2) \le 1$$
a then applying Inclusion Exclusion Formula we have the <u>Bonferroni Inequality</u>:
$$P(C_1)+P(C_2)-1 \le P(C_1 \cap C_2)$$

# Definitions
***Definition 1.3.1 (Kolmogorov's Probability Axioms)*** Let $C$ be a sample space and let $B$ be the set of events. Let $P$ be a real-valued function defined on $B$. Then $P$ is a probability set function if P satisfies the following 3 conditions
1. No negative values in set functions: $P(A)\ge 0$ for all $A \in B$ 
2. Upper bound on set functions: $P(C) = 1$
3. Rules for additivity: if $\{A_n\}$ is a sequnce of events in $B$ and $A_m \cap A_n = \emptyset$ for all $m \ne n$, then $P(\cup_{n=1}^{\infty} A_n) = \sum_{k=0}^{\infty} k = P(A_{n})$ 
# Theorems
***Theorem 1.3.1.*** For each event $A \in B$ , $P(A) = 1- P(A^c)$ 
***Theorem 1.3.2.*** The probability of the null set is zero: $P(\emptyset)=0$ 
***Theorem 1.3.3.*** If $A$ and $B$ are events such that $A\subset B$ then $P(A) \le B$ 
***Theorem 1.3.4.*** For each $A \in B$ , $0 \le P(A) \le 1$ 
***Theorem 1.3.5.*** If $A$ and $B$ are events in the sample space $C$ , then $P(A \cup B)=P(A)+P(B)-P(A\cap B)$.

***Theorem 1.3.6 (Continuity Theorem of Probability).*** Let ${C_n}$ be a nondecreasing sequence of events. Then:
$$\lim_{ n \to \infty } P(C_{n})=P(\cup^{\infty}_{n=1}C_{n}) $$
Let ${C_n}$ be a nonincreasing sequence of events. Then:
$$\lim_{ n \to \infty } P(C_{n})=P(\cap^{\infty}_{n=1}C_{n})$$


***Theorem 1.3.7 (Boole's Inequality)*** Let $\{C_n\}$ be an arbitrary sequence of events, then
$$P(\cup^{\infty}_{n=1}C_{n})\le \sum^{\infty}_{n=1}P(C_{n})$$

***Remark 1.3.2 (Inclusion Exclusion Formula)***. 
$$P(C_{1}\cup C_{2} \cup C_{3})=p_{1}-p_{2}+p_{3}$$
where:
$p_{1} = P(C_{1})+ P(C_2)+P(C_3)$
$p_2 = P(C_1 \cap C_2) + P(C_1 \cap C_3) + P(C_2\cap C_3)$
$p_3 = P(C_1 \cap C_2 \cap C_{3})$