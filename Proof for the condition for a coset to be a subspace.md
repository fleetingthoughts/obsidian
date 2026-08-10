---
parent:
tags:
  - "#flashcard"
  - macro/math/friedberg/ch1
date_created: 2026-07-24
---
Prove given a vector space $V$ and a subspace $W$, the coset $v + W$ is a subspace of $V$ if and only if **$v \in W$**.
#### Notes
**Forward implication (If $v + W$ is a subspace, then $v \in W$):**
    By definition, every subspace must contain the zero vector, $0$. Therefore, if the coset $v + W$ is a subspace, it must be true that $0 \in v + W$. This means there exists some vector $w \in W$ such that:$$0 = v + w$$Solving for $v$ gives:$$v = -w$$Since $W$ is a subspace, it is closed under scalar multiplication. Therefore, if $w \in W$, its additive inverse $-w$ is also in $W$. Consequently, $v \in W$.
    
**Reverse implication (If $v \in W$, then $v + W$ is a subspace):**
    If $v \in W$, we must show that $v + W = W$.
    1. Let $x$ be an arbitrary element in $v + W$. Then $x = v + w$ for some $w \in W$. Since $W$ is a subspace, it is closed under vector addition. Because both $v \in W$ and $w \in W$, their sum $x$ must also be in $W$. Thus, $v + W \subseteq W$.
    2. Let $y$ be an arbitrary element in $W$. We can rewrite $y$ as $y = v + (y - v)$. Since $W$ is closed under addition and scalar multiplication, the vector $(y - v)$ is in $W$. Therefore, $y$ is the sum of $v$ and an element in $W$, meaning $y \in v + W$. Thus, $W \subseteq v + W$.
Since $v + W \subseteq W$ and $W \subseteq v + W$, we conclude that $v + W = W$. Because $W$ is given as a subspace, $v + W$ is therefore a subspace.
