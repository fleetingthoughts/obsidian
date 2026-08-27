---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.4 Invertibility and Isomorphisms]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-08-17
---
Prove that a linear transformation $T$ is invertible if and only if its matrix representation is invertible as well.
#### Notes
- Forward Direction ($\implies$): Suppose $T$ is invertible. Use the matrix representation of identities to show $I_n = [I_V]_\beta = [T^{-1}T]_\beta = [T^{-1}]_\gamma^\beta [T]_\beta^\gamma$ and similarly for $I_m$. This proves $[T]_\beta^\gamma$ is invertible.
    
- Reverse Direction ($\impliedby$): Assume $A = [T]_\beta^\gamma$ is invertible with inverse $B$.
    
- Use the $\Phi_\beta^\gamma$ isomorphism to define a unique linear transformation $U: W \to V$ such that $[U]_\gamma^\beta = B$.
    
- Compute $[UT]_\beta = BA = I_n$ and $[TU]_\gamma = AB = I_m$.
    
- Use the uniqueness of identity representations to conclude $UT = I_V$ and $TU = I_W$, meaning $T^{-1} = U$.
