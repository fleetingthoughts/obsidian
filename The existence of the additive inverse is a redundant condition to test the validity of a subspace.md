---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.3 Subspaces]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch1
date_created: 2026-07-24
---
> "List four commonly cited conditions for a subset to be a subspace (non-empty, contains the zero vector, closed under addition, closed under scalar multiplication), and prove which condition is redundant
#### Notes
Let $V$ be a vector space over a field $F$, and let $W$ be a subset of $V$. The four conditions sometimes used to evaluate if $W$ is a subspace are:

1. **Non-empty:** $W \neq \emptyset$
    
2. **Contains the zero vector:** $0 \in W$ (where $0$ is the zero vector of $V$)
    
3. **Closure under addition:** For all $x, y \in W$, the sum $x + y \in W$.
    
4. **Closure under scalar multiplication:** For all $c \in F$ and $x \in W$, the product $cx \in W$.
    

### Proof of redundancy

Depending on the chosen baseline, either condition 1 or condition 2 can be considered the redundant one. Most modern theorems omit condition 1, as proving condition 2 is more specific and mathematically useful.

**Condition 2 makes condition 1 redundant:**

If we prove condition 2 ($0 \in W$), it means the subset $W$ contains at least one specific element (the zero vector). By definition, a set containing an element cannot be empty. Therefore, $W \neq \emptyset$ (condition 1) is automatically true and requires no separate verification.

**Conditions 1 and 4 make condition 2 redundant:**

Alternatively, if we establish condition 1 ($W \neq \emptyset$), there exists at least one arbitrary vector $v \in W$.

If condition 4 holds, $W$ is closed under scalar multiplication, meaning $cv \in W$ for any scalar $c \in F$.

By choosing the scalar $c = 0$, we get:

$$0v = 0$$

Since the result of this scalar multiplication must remain in $W$, the zero vector $0$ must be in $W$. Therefore, condition 2 is inherently satisfied and redundant.

_(Note: If your specific source material defines the fourth condition as "contains additive inverses" instead of "is non-empty", that condition is also redundant. If $W$ is closed under scalar multiplication, you can multiply any vector $x \in W$ by the scalar $c = -1$. Because $-1x = -x$, the additive inverse is automatically guaranteed to be in $W$.)_
