---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.1 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-19
---
Prove the relationship between the eigenvector of a linear operator and the eigenvector of its corresponding matrix representation.
#### Notes
et $T$ be a linear operator on an $n$-dimensional vector space $V$, $\beta$ be an ordered basis for $V$, and $A = [T]_\beta$. We show that $v \in V$ is an eigenvector of $T$ corresponding to $\lambda \iff \phi_\beta(v)$ is an eigenvector of $A$ corresponding to $\lambda$:

- Suppose $v$ is an eigenvector of $T$ corresponding to $\lambda$, meaning $T(v) = \lambda v$.
    
- Then $A\phi_\beta(v) = L_A\phi_\beta(v) = \phi_\beta T(v) = \phi_\beta(\lambda v) = \lambda\phi_\beta(v)$.
    
- Now $\phi_\beta(v) \neq 0$ because $\phi_\beta$ is an isomorphism and $v \neq 0$. Hence, $\phi_\beta(v)$ is an eigenvector of $A$.
    
- This argument is reversible.
    

An equivalent formulation is that for an eigenvalue $\lambda$, a vector $y \in F^n$ is an eigenvector of $A \iff \phi_\beta^{-1}(y)$ is an eigenvector of $T$ corresponding to $\lambda$.

