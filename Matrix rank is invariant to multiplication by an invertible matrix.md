---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 3.2 The Rank of a Matrix and Matrix Inverses]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch3
date_created: 2026-09-23
---
How does multiplying an $m \times n$ matrix $A$ by invertible matrices $P$ and $Q$ affect its rank?
#### Notes
The rank is preserved: $\text{rank}(PAQ) = \text{rank}(A)$.
<!--SR:!fsrs,2026-10-11T05:59:58.019Z,8,8.2956,1,2,1,0,0,2026-10-03T05:59:58.019Z-->

- Right multiplication: Show $R(L_{AQ}) = R(L_A)$ because $L_Q$ is surjective, yielding $\text{rank}(AQ) = \text{rank}(A)$.
- Left multiplication: Show $\dim(L_P(R(L_A))) = \dim(R(L_A))$ because $L_P$ is an isomorphism, yielding $\text{rank}(PA) = \text{rank}(A)$.
- Combine both steps sequentially to conclude $\text{rank}(PAQ) = \text{rank}(PA) = \text{rank}(A)$.
