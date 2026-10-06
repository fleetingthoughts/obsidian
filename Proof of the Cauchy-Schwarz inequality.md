---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.1 Inner Products and Norms]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: In an inner product space, $\vert{}\langle x, y \rangle\vert{} \le \vert{}x\vert{} \cdot \vert{}y\vert{}$.
#### Notes
- Establish trivial case: equality holds if $y = 0$.
- For $y \neq 0$, define scalar $c \in F$ and expand positivity axiom $0 \le \langle x - cy, x - cy \rangle$.
- Substitute $c = \frac{\langle x, y \rangle}{\langle y, y \rangle}$ to force cancellation of cross terms.
- Simplify to $0 \le \vert{}x\vert{}^2 - \frac{\vert{}\langle x, y \rangle\vert{}^2}{\vert{}y\vert{}^2}$.
- Rearrange algebraically and take the square root.
