---
parent: "[[Understanding Analysis - 1.2 Some Preliminaries]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch4
date_created: 2026-08-29
---
Let $g: \mathbf{R} \to \mathbf{R}$ be an arbitrary function and let $A, B \subseteq \mathbf{R}$:
- State the exact relationship between the preimage of the intersection, $g^{-1}(A \cap B)$, and the intersection of the preimages. 
- State the exact relationship between the preimage of the union, $g^{-1}(A \cup B)$, and the union of the preimages.

How does it differ from the image of an intersection of sets?
#### Notes
$g^{-1}(A \cap B) = g^{-1}(A) \cap g^{-1}(B)$. 
- **Forward Inclusion ($\subseteq$):** Let $x \in g^{-1}(A \cap B)$. By definition of the preimage, $g(x) \in A \cap B$.
    
- By definition of intersection, $g(x) \in A$ and $g(x) \in B$.
    
- Thus, $x \in g^{-1}(A)$ and $x \in g^{-1}(B)$, which implies $x \in g^{-1}(A) \cap g^{-1}(B)$.
    
- **Reverse Inclusion ($\supseteq$):** Let $x \in g^{-1}(A) \cap g^{-1}(B)$. This means $x \in g^{-1}(A)$ and $x \in g^{-1}(B)$.
    
- Therefore, $g(x) \in A$ and $g(x) \in B$, meaning $g(x) \in A \cap B$. By definition of the preimage, $x \in g^{-1}(A \cap B)$.

$g^{-1}(A \cup B) = g^{-1}(A) \cup g^{-1}(B)$.
- - **Forward Inclusion ($\subseteq$):** Let $x \in g^{-1}(A \cup B)$. By definition of the preimage, $g(x) \in A \cup B$.
    
- By definition of union, $g(x) \in A$ or $g(x) \in B$.
    
- Thus, $x \in g^{-1}(A)$ or $x \in g^{-1}(B)$, which implies $x \in g^{-1}(A) \cup g^{-1}(B)$.
    
- **Reverse Inclusion ($\supseteq$):** Let $x \in g^{-1}(A) \cup g^{-1}(B)$. This means $x \in g^{-1}(A)$ or $x \in g^{-1}(B)$.
    
- Therefore, $g(x) \in A$ or $g(x) \in B$, meaning $g(x) \in A \cup B$. By definition of the preimage, $x \in g^{-1}(A \cup B)$.

The preimage always preserves the intersection of sets, the image of an intersection of a set is a subset of the intersection of the images. The image is only equivalent if the function is injective.
