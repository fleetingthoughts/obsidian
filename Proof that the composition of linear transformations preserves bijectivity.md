---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.3 Compositions of Linear Transformations and Matrix Multiplication]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Let $V, W$, and $Z$ be vector spaces, and let $T:V \to W$ and $U:W \to Z$ be linear. If $T$ and $U$ are both surjective (onto), then the composite $UT$ is surjective and the same for injectivity
#### Notes
- **Target Setup:** Let $z \in Z$ be an arbitrary vector in the codomain of the composite transformation.
    
- **Apply Outer Surjectivity:** Because $U: W \to Z$ is onto, there exists a vector $w \in W$ such that $U(w) = z$.
    
- **Apply Inner Surjectivity:** Because $T: V \to W$ is onto, for that specific vector $w \in W$, there exists a vector $v \in V$ such that $T(v) = w$.
    
- **Composition Conclusion:** Substitute $T(v)$ for $w$ in the first equation to yield $U(T(v)) = z$. By definition of composition, $(UT)(v) = z$. Since $z$ was arbitrary, $UT$ is onto.



- **Null Space Setup:** Assume $x \in N(UT)$. By definition, this means $(UT)(x) = 0$, which evaluates to $U(T(x)) = 0$.
    
- **Apply Outer Injectivity:** Since $U$ is one-to-one, its null space is trivial ($N(U) = \{0\}$). Because $U$ maps the vector $T(x)$ to $0$, it must be that $T(x) = 0$.
    
- **Apply Inner Injectivity:** Since $T(x) = 0$, it follows that $x \in N(T)$. Because $T$ is also one-to-one, its null space is trivial ($N(T) = \{0\}$).
    
- **Conclusion:** This strictly implies that $x = 0$. Since assuming $x \in N(UT)$ leads directly to $x = 0$, $N(UT) = \{0\}$, proving $UT$ is one-to-one.
