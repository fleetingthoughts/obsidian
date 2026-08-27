---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.6 Bases and Dimension]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch1
date_created: 2026-07-24
---
Prove that  $V=W_1\oplus W_2$  if and only if for $v\in V$ $v=w_1+w_2$ for a unique vector $w_1 \in W_1$ and a unique vector $w_2 \in W_2$ 
#### Notes
**Forward implication (If $V = W_1 \oplus W_2$, then the representation is unique):**

By the definition of a direct sum, $V = W_1 + W_2$ and $W_1 \cap W_2 = \{0\}$. Since $V = W_1 + W_2$, every $v \in V$ can be written as $v = w_1 + w_2$ for some $w_1 \in W_1$ and $w_2 \in W_2$.

To prove this representation is unique, assume there is another way to express $v$, such that $v = x_1 + x_2$ where $x_1 \in W_1$ and $x_2 \in W_2$. Equating the two expressions gives:

$$w_1 + w_2 = x_1 + x_2$$

Rearranging the terms yields:

$$w_1 - x_1 = x_2 - w_2$$

Because $W_1$ and $W_2$ are subspaces (and thus closed under addition and scalar multiplication), the left side ($w_1 - x_1$) is a vector in $W_1$, and the right side ($x_2 - w_2$) is a vector in $W_2$. Since they are equal, this single vector must belong to their intersection, $W_1 \cap W_2$.

We are given that $W_1 \cap W_2 = \{0\}$. Therefore:

$$w_1 - x_1 = 0 \implies w_1 = x_1$$

$$x_2 - w_2 = 0 \implies w_2 = x_2$$

This proves that the representation $v = w_1 + w_2$ is strictly unique.

**Reverse implication (If every $v \in V$ is uniquely represented as $v = w_1 + w_2$, then $V = W_1 \oplus W_2$):**

Since every $v \in V$ can be written as a sum of vectors from $W_1$ and $W_2$, it immediately follows that $V = W_1 + W_2$.

We must now show that $W_1 \cap W_2 = \{0\}$. Let $x$ be any vector in $W_1 \cap W_2$. We can write the zero vector $0 \in V$ in two ways:

1. $0 = 0 + 0$ (where the first $0 \in W_1$ and the second $0 \in W_2$).
    
2. $0 = x + (-x)$ (where $x \in W_1$ and $-x \in W_2$, since $x$ is in both subspaces).
    

Because the premise states that representations of vectors in $V$ as sums from $W_1$ and $W_2$ are unique, these two expressions for the zero vector must be identical. Therefore, $x = 0$ and $-x = 0$. Since the only vector in the intersection is the zero vector, $W_1 \cap W_2 = \{0\}$.

Combining $V = W_1 + W_2$ and $W_1 \cap W_2 = \{0\}$ satisfies the definition of the direct sum, $V = W_1 \oplus W_2$.
