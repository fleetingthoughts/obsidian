---
parent: "[[Understanding Analysis - 1.3 The Axiom of Completeness]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch3
date_created: 2026-07-24
---
Prove that the cut property of real numbers is equivalent to the axiom of completeness
#### Notes
The axiom of completeness implies the cut property:
- Let $A$ and $B$ be nonempty, disjoint sets partitioning $\mathbb{R}$ such that $a < b$ for all $a \in A$ and $b \in B$.
    
- Observe that the set $A$ is nonempty and bounded above (by any element $b \in B$).
    
- Invoke the Axiom of Completeness to define $c = \sup A$.
    
- **Left Bound Constraint:** By the definition of supremum, $c$ is an upper bound for $A$, so $x \le c$ for all $x \in A$.
    
- **Right Bound Constraint:** Every $y \in B$ is an upper bound for $A$. Since $c$ is the _least_ upper bound, $c \le y$ for all $y \in B$, meaning $x \ge c$ whenever $x \in B$.

The cut property implies the axiom of completness:

- Let $E \subseteq \mathbb{R}$ be a nonempty set that is bounded above.
    
- Define $B$ as the set of all upper bounds of $E$, and define $A = \mathbb{R} \setminus B$.
    
- Verify that $A$ and $B$ are nonempty, disjoint, and satisfy $A \cup B = \mathbb{R}$. Furthermore, show that $a < b$ for all $a \in A$ and $b \in B$.
    
- Apply the Cut Property to produce a real number $c$ separating $A$ and $B$.
    
- **Upper Bound Condition:** Prove $c$ is an upper bound for $E$. (Assume for contradiction it is not, meaning there exists $e \in E$ such that $c < e$, and locate a point between $c$ and $e$ that forces a contradiction).
    
- **Least Upper Bound Condition:** Prove $c$ is the _least_ upper bound by showing that no number strictly less than $c$ can be in $B$.
