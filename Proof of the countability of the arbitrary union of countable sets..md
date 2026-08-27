---
parent: "[[Understanding Analysis - 1.5 Cardinality]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch1
date_created: 2026-07-24
---
Prove that the infinite union of countable sets is countable
#### Notes
- Arrange the elements of the countable sets $A_1, A_2, A_3, \dots$ into a two-dimensional grid array where row $i$ lists the elements of set $A_i$.
    
- Traverse the grid systematically using a diagonal path (e.g., listing elements where the sum of their row and column indices is a constant $k$, incrementing $k$).
    
- Enumerate the elements consecutively along this path, bypassing any duplicated elements to maintain a 1-1 correspondence.
    
- Conclude that this enumeration forms a bijection with $\mathbf{N}$, proving the infinite union is countable.
