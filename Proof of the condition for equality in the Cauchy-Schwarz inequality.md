---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.1 Inner Products and Norms]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: In an inner product space, $\vert{}\langle x, y \rangle\vert{} = \vert{}x\vert{} \vert{}y\vert{}$ if and only if one of $x$ or $y$ is a scalar multiple of the other.
#### Notes
- Forward dependency: Assume $x = cy$. Expand $\vert{}\langle cy, y \rangle\vert{}$ and verify it equals $\vert{}cy\vert{} \vert{}y\vert{} = \vert{}x\vert{}\vert{}y\vert{}$.
- Reverse dependency: Assume $\vert{}\langle x, y \rangle\vert{} = \vert{}x\vert{} \vert{}y\vert{}$ and $y \neq 0$.
- Construct scalar projection $a = \frac{\langle x, y \rangle}{\vert{}y\vert{}^2}$ and orthogonal component $z = x - ay$.
- Verify orthogonality: $\langle z, y \rangle = 0$.
- Apply Pythagorean theorem to $x = ay + z$, substitute equality assumption, forcing $\vert{}z\vert{}^2 = 0$, yielding $x = ay$.
