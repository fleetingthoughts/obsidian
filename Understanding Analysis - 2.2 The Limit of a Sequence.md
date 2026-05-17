---
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
tags:
  - math
  - understanding_analysis
  - stephen_abbot
  - real_analysis
date_created:
---
Historically, the field of calculus was developed without rigor leading to useful results but eventually run into unintuitive answers. To explain the unintuitive results, we go back to the results we derived and attempt to reduce the problem to the bare minimum definitions and properties required to produce these results. In calculus, many of the results were reduced to reduced to results about definitions of sequences, and so, the strategy is to crystallize the properties and definitions of sequences required to produce the desirable results and then re-derive all of calculus. This is precisely what we do in this chapter and explain the definitions and properties of sequences that derive the rest of calculus:
1) Definition of a sequence
2) ***Binary characterization of an infinite sequence.*** We wish to categorize infinite sequences in a binary fashion by whether they converge or diverge
3) ***Properties of convergent sequences.*** The limit of a convergent sequence is unique.

***Definition 2.2.1 (Sequences)*** A sequence is a function whose domain is the natural numbers $\mathbb{N}$. 

***Definition 2.2.3 (Convergence of a sequence)***. A sequence $(a_n)$ converges to a number $a$  if for any arbitrary positive $\epsilon \gt 0$, then $|a_n -a | \lt \epsilon$ for all $n > N$ for some natural number $N$.

This definition of convergence restated basically states that if the sequence converges to some specific number, then we can make an infinitely many terms of the sequence arbitrarily close to the limit. In other words, outside of some $N$ terms, we can make the infinite sequence within $\epsilon$ of the limit. We say that with a converging sequence, the "$\epsilon$ -neighborhood" of the limit $a$ contains all but a finite number of terms

***Definition 2.2.4 (the $\epsilon$ - neighborhood of $a$).*** Given a real number $a \in R$ and a positive $\epsilon > 0$ , then the  $\epsilon$ - neighborhood of $a$ is the following set:
$$V_{\epsilon}(a) = \{x\in R:|x-a| <\epsilon\}$$


The aim of these definitions is to produce useful results and one of the goals is to characterize convergent sequences by the limit. ***Theorem 2.2.7*** states that the limit is unique which can be proven by contradiction. If we have two limits, then by the triangle inequality, these two limits must be identical or we have a contradiction on the presumption of convergence.

By ***Definition 2.2.9***, a sequence that doesn't converge is said to diverge, so by definition, all sequences either converge or diverge with no in-between.

# Definitions

***Definition 2.2.1 (Sequences)*** A sequence is a function whose domain is the natural numbers $\mathbb{N}$. 

***Definition 2.2.3 (Convergence of a sequence)***. A sequence $(a_n)$ converges to a number $a$  if for any arbitrary positive $\epsilon \gt 0$, and for all $n > N$ for some natural number $N$, then $|a_n -a | \lt \epsilon$ 

***Definition 2.2.4 (the $\epsilon$ - neighborhood of $a$).*** Given a real number $a \in R$ and a positive $\epsilon > 0$ , then the  $\epsilon$ - neighborhood of $a$ is the following set:

***Definition 2.2.9 (Divergence).*** If a sequence does not converge, then it is said to diverge

# Theorems

***Theorem 2.2.7 (Uniqueness of Limits).*** The limit of a sequence, when it exists, must be unique. 
