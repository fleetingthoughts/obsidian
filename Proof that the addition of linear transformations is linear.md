---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.2 The Matrix Representation of A Linear Transformation]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
State the definition for the addition operation between linear transformations and prove that the sum of linear transformations is also linear
#### Notes
- **Setup Linearity Test:** Let $x, y \in V$ and $c \in F$. Consider $(aT+U)(cx+y)$.

- **Apply Pointwise Definitions:** Expand to $(aT)(cx+y) + U(cx+y)$, and then to $aT(cx+y) + U(cx+y)$.
    
- **Exploit Inherited Linearity:** Use the linearity of $T$ and $U$ individually to get $a[cT(x) + T(y)] + [cU(x) + U(y)]$.
    
- **Regroup (Vector Space Axioms in W):** Distribute and factor to isolate $c$: $c[aT(x) + U(x)] + [aT(y) + U(y)]$.
