---
parent: "[[Understanding Analysis - 1.2 Some Preliminaries]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch1
date_created: 2026-07-24
---
Given non-empty finite sets in the reals $A_1, A_2,....$ such that $A_{n+1} \subseteq A_n$ and all, what can we say about $\bigcap\limits^{\infty}_{i=1}A_i$?
#### Notes
The infinite intersection is non-empty and must contain an element. There is a limit on how small the size that $A_i$ can be to stay non-empty.
<!--SR:!fsrs,2026-11-26T06:02:15.917Z,54,53.75786403,4.01060897,2,2,0,0,2026-10-03T06:02:15.917Z-->

***Proof outline by contradiction.*** We can prove by contradiction. Assume that the infinite intersection is empty then since $A_1$ is the largest set with a finite $n$ number of elements, we can apply induction and show that there exists a set that contains none of it so it must be empty contradicting our hypothesis.
