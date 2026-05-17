---
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
tags:
  - math
  - understanding_analysis
  - stephen_abbot
  - real_analysis
date_created:
---
The strategy in analysis is to reduce problems to that of sequences, so it is advantageous for us to determine properties of sequences as it relates to infinity. We are interested in the following things about sequences:
1) Definition of a sequence
2) ***Binary characterization of an infinite sequence.*** We wish to categorize infinite sequences in a binary fashion by whether they converge or diverge
3) ***Properties of convergent sequences.*** The limit of a convergent sequence is unique.

***Definition 2.2.1 (Sequences)*** A sequence is a function whose domain is the natural numbers $\mathbb{N}$. 

***Definition 2.2.3 (Convergence of a sequence)***. A sequence $(a_n)$ converges to a number $a$  if for any arbitrary positive $\epsilon \gt 0$, then $|a_n -a | \lt \epsilon$ for all $n > N$ for some natural number $N$.

This definition of convergence restated basically states that if the sequence converges to some specific number, then we can make an infinite amount of the sequence arbitrarily close to the limit. In other words, outside of some $N$ terms, we can make the infinite sequence within $\epsilon$ of the limit. We say that with a converging sequence, the "$\epsilon$ -neighborhood" of the limit $a$ contains all but a finite number of terms

***Definition 2.2.4 (the $\epsilon$ - neighborhood of $a$).*** Given a real number $a \in R$ and a positive $\epsilon > 0$ , then the  $\epsilon$ - neighborhood of $a$ is the following set:
$$V_{\epsilon}(a) = \{x\in R:|x-a| <\epsilon\}$$
Template for a proof that $(x_n)$ → $x$  :
- “Let $\epsilon$ > 0 be arbitrary.”
- Demonstrate a choice for N ∈ N. This step usually requires the most work, almost all of which is done prior to actually writing the formal proof.
- Now, show that $N$  actually works.
- “Assume $n \ge N$ .”
- With $N$ well chosen, it should be possible to derive the inequality $|x_{n} − x| < \epsilon$ 


***Theorem 2.2.7 (Uniqueness of Limits).*** The limit of a sequence, when it exists, must be unique. 

This can be proven assuming if a sequence converges and it converges to two separate limits, then by triangular inequality, these two limits must be identical or we have a contradiction on the presumption of convergence.

We also have a word for what happens when a sequence doesn't converge

***Definition 2.2.9 (Divergence).*** If a sequence does not converge, then it is said to diverge

So by this definition, all sequences either converge or diverge with no in-between.

# Definitions

***Definition 2.2.1 (Sequences)*** A sequence is a function whose domain is the natural numbers $\mathbb{N}$. 

***Definition 2.2.3 (Convergence of a sequence)***. A sequence $(a_n)$ converges to a number $a$  if for any arbitrary positive $\epsilon \gt 0$, then $|a_n -a | \lt \epsilon$ for all $n > N$ for some natural number $N$.

***Definition 2.2.4 (the $\epsilon$ - neighborhood of $a$).*** Given a real number $a \in R$ and a positive $\epsilon > 0$ , then the  $\epsilon$ - neighborhood of $a$ is the following set:

# Theorems

***Theorem 2.2.7 (Uniqueness of Limits).*** The limit of a sequence, when it exists, must be unique. 
