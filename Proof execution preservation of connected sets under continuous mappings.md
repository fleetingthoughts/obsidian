---
parent: "[[Understanding Analysis - 4.5 Intermediate Value Theorem]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch4
date_created: 2026-09-29
---
Prove: Let $f : G \to \mathbf{R}$ be continuous. If $E \subseteq G$ is connected, then $f(E)$ is connected.
#### Notes
- Assume for contradiction $f(E)$ is disconnected, meaning $f(E) = A \cup B$ for nonempty, disjoint sets $A, B$ where neither contains a limit point of the other.
    
- Define preimages $C = \{x \in E : f(x) \in A\}$ and $D = \{x \in E : f(x) \in B\}$, noting they are nonempty, disjoint, and $E = C \cup D$.
    
- Apply the sequential characterization of connectedness to $E = C \cup D$ to find a sequence in $C$ converging to a limit in $D$ (or vice versa).
    
- Apply the continuity of $f$ to show the sequence maps to limits violating the separation condition of $A$ and $B$, establishing $f(E)$ is connected.
