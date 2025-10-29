tag: #math #statistics 
parent::[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig](Introduction%20to%20Mathematical%20Statistics%208th%20ed.%20-%20Hogg,%20McKean,%20Craig.md) [_MOC Fleeting](_MOC%20Fleeting.md)
# 1.3 The Probability Set Function

We aim

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
Three counting rules from elementary algebra:
1) multiplication rule: Given set $A= \{x_1, x_2,...x_{m}\}$ and $B=\{y_1,y_2,..., y_n\}$, then then there are $m \times n$ ordered pairs $(x_i, y_j)$. This is [the cartesian product](1%20Real%20Numbers.md) of $A \times B$ 
2) Permutations. The k-tuple permutation of a set $A$ with $n$-elements, then the set of tuples containing elements distinct from each other is the permutation denoted $P^{n}_{k}=\frac{n!}{(n-k)!}$ 
## 1.3.2 Additional properties of probability
***Theorem 1.3.7 (Boole's Inequality)***

***Remark 1.3.2 (Inclusion Exclusion Formula)***. There is a special case which gives the Bonferroni's inequality

