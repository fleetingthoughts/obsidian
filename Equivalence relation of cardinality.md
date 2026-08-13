---
parent:
tags:
  - "#flashcard"
  - macro/math/abbott/ch1
date_created: 2026-07-24
---
Prove that cardinality is an equivalence relation
#### Notes
- Reflexivity: Show $A \sim A$ by explicitly defining the identity mapping $f(x) = x$, which is trivially 1-1 and onto.
    
- Symmetry: Assume $A \sim B$ via a bijective function $f : A \to B$. Show $B \sim A$ by utilizing the inverse function $f^{-1} : B \to A$, which is guaranteed to exist and be bijective.
    
- Transitivity: Assume $A \sim B$ via bijection $f$ and $B \sim C$ via bijection $g$. Show $A \sim C$ by constructing the composition $h = g \circ f$ and noting that the composition of two bijections is a bijection.
