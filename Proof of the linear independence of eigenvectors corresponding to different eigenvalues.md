---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: Let $T$ be a linear operator. If $S_1, \dots, S_k$ are linearly independent sets of eigenvectors corresponding to distinct eigenvalues $\lambda_1, \dots, \lambda_k$, then $\bigcup_{i=1}^k S_i$ is linearly independent.
#### Notes
- Proceed by induction on $k$. The base case $k = 1$ holds by hypothesis.
- For the inductive step, assume $\sum_{i=1}^k \sum_{j=1}^{n_i} a_{ij} v_{ij} = 0$.
- Apply the operator $T - \lambda_k I$ to both sides to annihilate the $S_k$ vectors, isolating a linear combination of vectors in $S_1 \cup \dots \cup S_{k-1}$ set to $0$.
- Invoke the inductive hypothesis to conclude $a_{ij} = 0$ for $i < k$, utilizing the fact that eigenvalues are distinct.
- Substitute these zeros back into the original sum and use the linear independence of $S_k$ to conclude $a_{kj} = 0$.
