---
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
tags:
  - "#math"
  - "#stephen_abbot"
  - "#understanding_analysis"
  - "#real_analysis"
date_created:
---
In this section, we now formalize a lot of intuition we have about the different fields within and including R and how $N, Q, Z$ fit into $R$ as well we deduce a theorem that formalizes the idea of the set of real numbers having no "gaps" in it. We derive the following properties of real numbers from the AoC:
1) The nested interval property
2) The Archimedean property
3) Density of rationals on $\mathbb{R}$
4) The existence of square roots on $\mathbb{R}$ 

The nested interval properties (NIP) colloquially says the real numbers have no gaps.

***Theorem 1.4.1. (The Nested Interval Property).*** For a given closed interval $I_n = [a_n, b_n]=\{x\in R: a_n \le x \le b_n\}$, with $I_n$ such that $I_n \subseteq I_{n-1} \subseteq \dots \subseteq I_1$ then  $\cap I_n \ne \emptyset$  

The NIP implies that any nested closed interval must always contain an element. A closed interval is required so that we can talk about a specific element being part of the set. The creativity in the [proof of the NIP](Proof%20of%20the%20Nested%20Interval%20Property%20as%20a%20Consequence%20of%20the%20Axiom%20of%20Completeness.md) is the use of two sequences to generally represent any arbitrary nesting rule we create for closed intervals. The representation of the nested intervals as sequences lets us leverage axioms in the set theory of real numbers such as the AoC.
# The natural numbers are not bounded on the reals. They have no supremum.
Now we look at how $\mathbb{N}$ is infinite within $\mathbb{R}$. The set of all natural numbers is not bounded and so has no least upper bound per the AoC:

***Theorem 1.4.2 (Archimedean property. The set of natural numbers is unbounded)***. Given any $x \in R$, there exists an $n \in N$ such that $n \gt x$. Furthermore, given any real number $y \gt 0$, there exists an $n \in N$ such that $1/n \lt y$ 

The Archimedean property states we can never find an upper bound for the set of all natural numbers and so there will never be a supremum. It seems like non-sense but the idea of $\mathbb{R}$ being an extension of $\mathbb{Q}$ necessitates us to double check we didn't unwittingly create upper bounds for $\mathbb{N}$ for there are ordered field extensions that actually do that. This can be proven by contradiction using Lemma 1.3.8 and using a specific case of $\epsilon$ =1 to show that no real number can be an upper bound. The proof assumes the AoC, but it also assumes that $\mathbb{N}$ is a closed under addition meaning if an additive operation is carried out on an $n\in \mathbb{N}$ then this $n+1$ (1 is a natural number) is still contained in $\mathbb{N}$ 

The Archimedean property also guarantees we can always construct a number smaller than any real number or find a real number larger than any given real number which is helpful in constructive proofs.
# The Rationals are dense on the reals in the sense that you can always find a rational number between any two real numbers
Using the Archimedean property, we can now formalize the idea that $\mathbb{R}$ is an "extension" of $\mathbb{Q}$ by containing all the irrational numbers as well. The idea is that $\mathbb{Q}$ is "infinitely dense" such that we can find a rational number between any two real numbers which is formalized as follows:

***Theorem 1.4.3 (Density of Q in R)***. For every two real numbers $a \lt b$ , there exists a rational number $r$ such that $a \lt r\lt b$.

Note that we use $\lt$ and not $\le$ resulting in a smaller set and stronger theorem . [The proof of the density of rationals](Proof%20of%20the%20Density%20of%20Rational%20Numbers%20in%20the%20Real.md) is a constructive proof develops an algorithm to produce a rational number between any two given real numbers. The proof also demonstrates the usefulness of the Archimedean property in constructive proofs. 

An analogous proof can be adopted for the density of irrational numbers (***Exercise 1.4.5***) by using a similar proof to what is used to prove the density of the rational numbers and making use of the fact that additive properties are not closed within irrational numbers (***Exercise 1.4.1***)

We can also prove the existence of certain irrational numbers like $\sqrt2$  in the real using only rational numbers by constructing a bounded set of rational numbers (therefore by the AoC it MUST have a supremum) and that the supremum must be some quantity $\alpha$ such that $\alpha^2 =2$. The proof by constructing a bounded set with a supremum equal to the number we want to prove the existence of shows a property resulting from AoC called the property or Dedekind cut and is a method of constructing the numbers we want to prove the existence of by partitioning a set into two precisely at the number we want to "construct" or prove the existence of. In fact this cut property is logically equivalent to AoC and we could use either as our starting point to define real numbers as the set of rational numbers with irrational numbers filling the gaps (see Exercise 1.3.10).

# Summary of 
# Exercises
- ***Exercise 1.4.1***: [[The set of Irrational numbers is not closed under addition or multiplication]]
- ***Exercise 1.4.3.*** Counter example of a specific nested open interval that cannot contain any set. The exercise emphasizes that the NIP applies for nested closed intervals and is not necessarily true for nested open intervals.

# Theorems

***Theorem 1.4.1. (The Nested Interval Property).*** For a given closed interval $I_n = [a_n, b_n]=\{x\in R: a_n \le x \le b_n\}$, with $I_n$ such that $I_n \subseteq I_{n-1} \subseteq \dots \subseteq I_1$ then  $\cap I_n \ne \emptyset$  

***Theorem 1.4.2 (Archimedean property. The set of natural numbers is unbounded)***. Given any $x \in R$, there exists an $n \in N$ such that $n \gt x$. Furthermore, given any real number $y \gt 0$, there exists an $n \in N$ such that $1/n \lt y$ .

***Theorem 1.4.3 (Density of Q in R)***. For every two real numbers $a \lt b$ , there exists a rational number $r$ such that $a \lt r\lt b$.
