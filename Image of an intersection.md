---
parent:
tags:
  - "#flashcard"
date_created: 2026-07-24
---
For an arbitrary function $g$ and subsets $A, B$ of its domain, what is the general set-theoretic relationship between the image of their intersection $g(A \cap B)$ and the intersection of their images $g(A) \cap g(B)$? What kind of function $g$ is required for them to be equal? Prove both assertions
#### Notes
For any general function $g$, the relationship is as follows: $g(A \cap B) \subseteq g(A) \cap g(B)$. The relation is an equality if $g$ is injective.

- Let $y \in g(A \cap B)$. By definition, there exists an $x \in A \cap B$ such that $g(x) = y$.
    
- Since $x \in A \cap B$, it follows that $x \in A$ and $x \in B$.
    
- Therefore, $g(x) \in g(A)$ and $g(x) \in g(B)$, which implies $y \in g(A) \cap g(B)$.

If we add the assumption that $g$ is injective, then we can prove the converse because if $b \in B$ and $a\in A$ such that $g(a)=g(b)=y$ then $a=b$ so for $y \in g(A) \cap g(B)$ there must be an $x \in A \cap B$ 