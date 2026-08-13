---
parent: "[[Understanding Analysis - 1.5 Cardinality]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch1
date_created: 2026-07-24
---
Prove that the finite union of countable sets is countable.
#### Notes
- Base case ($m=2$): Let $A_1$ and $A_2$ be countable. Isolate unique elements by replacing $A_2$ with the disjoint set $B_2 = A_2 \setminus A_1$.
- Show $A_1 \cup A_2 = A_1 \cup B_2$, transforming the problem into a disjoint union of countable (or finite) sets.
- Prove the union of two disjoint countable sets is countable by alternating elements into a single sequence.
- Extend inductively: Assume the union of $k$ countable sets is countable, then group $k+1$ sets as $(A_1 \cup \dots \cup A_k) \cup A_{k+1}$, reducing it to the union of two countable sets.
