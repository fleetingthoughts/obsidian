tag: #math #statistics #robert_hogg
parent: [Introduction to Mathematical Statistics - 1 Probability and Distributions](Introduction%20to%20Mathematical%20Statistics%20-%201%20Probability%20and%20Distributions.md)


# 1.2 Sets
Some basic definitions and theorems for set theory:

***(Monotone sequence sets)*** . A <u>nondecreasing sequence</u> (nested upward) of sets $A_n$ occurs if $A_{i-1} \subset A_i$. For such a sequence we define:
$$\lim_{ n \to \infty }A_{n}=\cup^{\infty}_{n=1}A_{n} $$
For a <u>nonincreasing sequence of sets</u> (nested downward) where $A_{i} \subset A_{i-1}$ , we similarly define
$$\lim_{ n \to \infty }A_{n}=\cap^{\infty}_{n=1}A_{n} $$
Put another way, an finite or infinite sequence of monotonic sets converges to a singular set. For example the set $A = \{1,3,5,7 2n-1\}$ is a nondecreasing and by definition we have $\lim_{ n \to \infty }A_{n}= \{1,3,5, 7,....\}$ 

DeMorgan's Laws:
$$(A\cap B)^c=(A^c \cup B^c)$$
$$(A \cup B)^c = (A^c \cap B^c)$$ 
# 1.3 The Probability Set Function

In this chapter, we start to establish probabilities of events that are [countable](Understanding%20Analysis%20-%201.5%20Cardinality.md) and the rules associated with counting them. There are technicalities with ascribing probabilities to infinite sample spaces outside the scope of this book so we constrain ourselves to collection of events that are closed under complements and countable unions. DeMorgan's Laws then state that the collection is also closed under countable intersections. Such a collection of "countable" events that this section will concern itself with is called a $\sigma$ -field of subsets

***Definition 1.3.1*** Let $C$ be a sample space and let $B$ be the set of events. Let $P$ be a real-valued function defined on $B$. Then $P$ is a probability set function if P satisfies the following 3 conditions
1. $P(A)\ge 0$ for all $A \in B$ 
2. $P(C) = 1$
3. if $\{A_n\}$ is a sequnce of events in $B$ and $A_m \cap A_n = \emptyset$ for all $m \ne n$, then $P(\cup_{n=1}^{\infty} A_n) = \sum_{k=0}^{\infty} k = P(A_{n})$ 
We refer to a mutually exclusive and exhaustive collection of events of the sample space forms what's called a partition of the sample space.

We can develop several properties of the probability set function for a collection of events $A$ and $B$ in the sample space
1) ***Theorem 1.3.1.*** For each event $A \in B$ , $P(A) = 1- P(A^c)$ 
2) ***Theorem 1.3.2.*** The probability of the null set is zero: $P(\emptyset)=0$ 
3) ***Theorem 1.3.3.*** If $A$ and $B$ are events such that $A\subset B$ then $P(A) \le B$ 
4) ***Theorem 1.3.4.*** For each $A \in B$ , $0 \le P(A) \le 1$ 
5) ***Theorem 1.3.5.*** If $A$ and $B$ are events in the sample space $C$ , then $P(A \cup B)=P(A)+P(B)-P(A\cap B)$. (see p. 15 for the proof)

## 1.3.1 Counting Rules
Three counting rules from elementary algebra for a set $A$ containing $n$ elements:
1) <u>Multiplication rule</u>: Given set $A= \{x_1, x_2,...x_{m}\}$ and $B=\{y_1,y_2,..., y_n\}$, then then there are $m \times n$ ordered pairs $(x_i, y_j)$. This is [the cartesian product](Book%20of%20Proof%20-%201%20Real%20Numbers.md) of $A \times B$ 
2) <u>Permutations. </u>The k-tuple permutation of a set $A$ with $n$-elements is the set of k-tuples containing unique elements of the set $A$  is the permutation denoted $P^{n}_{k}=\frac{n!}{(n-k)!}$. Note that for tuples, the order of the elements make them distinct for each other for a 3-tuple $(x_1,x_2,x_3) \ne (x_2, x_1, x_3)$, but note that the permutations demand that components within the tuple do not repeat so $(x_1,x_1, x_2)$ is not a permutation of $A$. The permutation set is a subset of all the possible k-tuples of $A$ which by the <u>multiplication rule</u> is $n^k$ 
3) <u>Combinations</u>. The number of subsets containing $k$ elements of the set $A$ is the combination denoted $C^{n}_{k}=\frac{n!}{k!(n-k)!}$=$\binom{n}{k}$ . The combinations is a subset of the permutations of $A$,  $\{P^{n}_{k}\}$ as the combinations are essentially permutations where we do not care for the ordering. We are no longer looking at ordered k-tuples but just the sets containing k-elements. Another way to see this is to take any given permutation of k-tuples and see that each of them can be ordered $k!$ different ways.
## 1.3.2 Additional properties of probability
***Theorem 1.3.6 (Continuity Theorem of Probability).*** Let ${C_n}$ be a nondecreasing sequence of events. Then:
$$\lim_{ n \to \infty } P(C_{n})=P(\cup^{\infty}_{n=1}C_{n}) $$
Let ${C_n}$ be a nonincreasing sequence of events. Then:
$$\lim_{ n \to \infty } P(C_{n})=P(\cap^{\infty}_{n=1}C_{n})$$
Theorem 1.3.6 essentially establishes the <u>conditions that allow us to interchange the limit and the probability set function.</u>

Now we add a useful <u>inequality that applies for any arbitrary unions</u>
***Theorem 1.3.7 (Boole's Inequality)*** Let $\{C_n\}$ be an arbitrary sequence of events, then
$$P(\cup^{\infty}_{n=1}C_{n})\le \sum^{\infty}_{n=1}P(C_{n})$$
This can intuitively be seen as the sum of probabilities of a collection is valid if the events are disjoin from each other, so once we take the union of these collection of events, then there may be overlapping events so the probability of this union is less. This inequality gives us a universal upper bound for the probability on the union of countable sets.

As a final corollary, we can extend theorem 1.3.5 to more than just two events: 

***Remark 1.3.2 (Inclusion Exclusion Formula)***. 
$$P(C_{1}\cup C_{2} \cup C_{3})=p_{1}-p_{2}+p_{3}$$
where:
$p_{1} = P(C_{1})+ P(C_2)+P(C_3)$
$p_2 = P(C_1 \cap C_2) + P(C_1 \cap C_3) + P(C_2\cap C_3)$
$p_3 = P(C_1 \cap C_2 \cap C_{3})$

Put in words, every $p_k$ is just a summation of all the possible intersections between k-number of collections so the summation will have $C^n_k$ combinations. We obviously don't care about the ordering of the intersections! Proof of this corollary is in Exercise 1.3.9

It can be seen that $p_k\le p_{k-1} \le \dots \le p_2 \le p_1$ by Boole's inequality. 

For the Inclusion Exclusion formula in the case where $k=2$ we can derive a special inequality using the axiom for probability set functions:
$$P(C_1 \cap C_2) \le 1$$
a then applying Inclusion Exclusion Formula we have the <u>Bonferroni Inequality</u>:
$$P(C_1)+P(C_2)-1 \le P(C_1 \cap C_2)$$

