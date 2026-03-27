---
tags:
  - math
  - logical_empiricism
  - proof
date_created: 2026-03-26
---
This note goes over a counterintuitive idea of something being "vacuously true" and what it means for a proof to be vacuously true and the motivating set theory principles behind it. The concept is derived from the result in set theory that the empty set is a subset of all sets, that is, for any set $A$:
$$\{\emptyset\}\subseteq A$$
The proof for this results from axioms in set theory that I will not go into, but to provide a moral answer for why this intuitively works, try to determine a counterexample. If we try to disprove by counterexample by saying there must be an element in the null set that is not contained in $A$, because the null set has no elements by definition, we are unable to find a counter example so this is always true.

What this means for proofs is that is that if we have a statement $P \implies Q$, then if $S$ is the empty set, it is always false. This means the implication $P \implies Q$ is always true! Recall that sufficiency is only false if $P$ is true while $Q$ is false. But since $P$ can never be true then we can never disprove this statement. This is fundamentally saying "we can never find a counter example to disprove the sufficiency statement". 
![](Pasted%20image%2020260326201332.png)
The vacuous truth is derived from our result in set theory because the statement $P \implies Q$ can be expressed in set theory terms: $$  x \in P \implies x\in Q$$
or :$$P \subseteq Q$$
But if $P$ is a null set, then it is a subset of all sets and no matter what $Q$ is, the proposition is true!