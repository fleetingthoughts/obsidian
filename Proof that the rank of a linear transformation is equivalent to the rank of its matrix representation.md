---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.4 Invertibility and Isomorphisms]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch2
date_created: 2026-09-23
---
Prove the following: Let $T: V \to W$ be a linear transformation from an $n$-dimensional vector space $V$ to an $m$-dimensional vector space $W$, and let $\beta$ and $\gamma$ be ordered bases for $V$ and $W$, respectively. Then $\text{rank}(T) = \text{rank}(L_A)$ and $\text{nullity}(T) = \text{nullity}(L_A)$, where $A = [T]_\beta^\gamma$
#### Notes
- Establish the commutative diagram relation between $T$ and its matrix representation: $\phi_\gamma \circ T = L_A \circ \phi_\beta$, where $\phi_\beta$ and $\phi_\gamma$ are the coordinate isomorphisms.
    
- For rank: Demonstrate that $\phi_\gamma(R(T)) = R(L_A)$ using the fact that $\phi_\beta$ is surjective. Apply the dimension-preserving property of the isomorphism $\phi_\gamma$ to conclude $\dim(R(T)) = \dim(R(L_A))$.
    
- For nullity: Either show $\phi_\beta(N(T)) = N(L_A)$ and use the dimension-preserving property of $\phi_\beta$, or invoke the Dimension Theorem (Rank-Nullity) on both $T$ and $L_A$, noting their domains share dimension $n$.
