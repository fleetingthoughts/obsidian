---
parent: "[[Understanding Analysis - 1.2 Some Preliminaries]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch1
date_created: 2026-07-24
---
For an arbitrary function $g$ and subsets $A, B$ of its domain, prove the set-theoretic relationship between the image of their union $g(A \cup B)$ and the union of their images $g(A) \cup g(B)$?
#### Notes
$g(A \cup B) = g(A) \cup g(B)$.

- **Forward Inclusion ($\subseteq$):** Let $y \in g(A \cup B)$. There exists $x \in A \cup B$ such that $g(x) = y$. Since $x \in A$ or $x \in B$, $y \in g(A)$ or $y \in g(B)$, meaning $y \in g(A) \cup g(B)$.
    
- **Reverse Inclusion ($\supseteq$):** Let $y \in g(A) \cup g(B)$. Then $y \in g(A)$ or $y \in g(B)$, meaning $y = g(x)$ for some $x \in A$ or $x \in B$. In either case, $x \in A \cup B$, so $y \in g(A \cup B)$.