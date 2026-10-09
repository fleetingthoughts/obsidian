---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.1 Inner Products and Norms]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: If $x$ and $y$ are orthogonal in an inner product space, $\vert{}x + y\vert{}^2 = \vert{}x\vert{}^2 + \vert{}y\vert{}^2$.
#### Notes
$\vert{}x + y\vert{}^2 = \langle x + y, x + y \rangle = \vert{}x\vert{}^2 + \langle x, y \rangle + \langle y, x \rangle + \vert{}y\vert{}^2$. Since orthogonal, $\langle x, y \rangle = \langle y, x \rangle = 0$, yielding $\vert{}x\vert{}^2 + \vert{}y\vert{}^2$.
