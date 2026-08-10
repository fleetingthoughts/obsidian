---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.6 Bases and Dimension]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch1
date_created: 2026-07-24
---
Prove that the basis is a subset of a finite set that generates a vector space
#### Notes
- Eliminate trivial case $S = \emptyset$ or $\{0\}$.
- Iteratively choose $u_1, \dots, u_k \in S$ to form a maximally linearly independent subset $\beta$.
- Since $S$ is finite, this terminates.
- For any $y \in S \setminus \beta$, $\beta \cup \{y\}$ is dependent. Because expanding a linearly independent set by an element outside its span makes it dependent, $y \in \text{span}(\beta)$.
- Therefore, $S \subseteq \text{span}(\beta)$. Since $S$ spans $V$, $\text{span}(\beta) = V$. Thus $\beta$ is a basis.