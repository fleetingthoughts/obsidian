---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.1 Inner Products and Norms]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: In an inner product space, $\vert{}x + y\vert{} \le \vert{}x\vert{} + \vert{}y\vert{}$.
#### Notes
- Expand the squared norm: $\vert{}x + y\vert{}^2 = \langle x + y, x + y \rangle$.
- Combine cross terms using the real part: $\langle x, y \rangle + \langle y, x \rangle = 2 \text{Re}\langle x, y \rangle$.
- Bound the real part: $2 \text{Re}\langle x, y \rangle \le 2\vert{}\langle x, y \rangle\vert{}$.
- Apply the Cauchy-Schwarz inequality to substitute $\vert{}\langle x, y \rangle\vert{} \le \vert{}x\vert{} \vert{}y\vert{}$.
- Factor the bounded expression into $(\vert{}x\vert{} + \vert{}y\vert{})^2$ and take the square root.
