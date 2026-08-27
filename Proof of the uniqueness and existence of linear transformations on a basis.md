---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.1 Linear Transformations, Null Spaces, and Ranges]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Prove the conditions for the uniqueness and existence of a linear transformation. Let $V$ and $W$ be vector spaces over $F$, and suppose that $\{v_1, v_2, \dots, v_n\}$ is a basis for $V$. For any vectors $w_1, w_2, \dots, w_n$ in $W$, there exists exactly one linear transformation $T:V \to W$ such that $T(v_i) = w_i$ for $i = 1, 2, \dots, n$.
#### Notes
- **Construction:** For $x = \sum a_i v_i$, explicitly define $T(x) = \sum a_i w_i$.
    
- **Linearity Verification:** Take $u, v \in V$ and scalar $d$. Expand both into basis components, apply the defined mapping, and factor out $d$ to show $T(du+v) = dT(u) + T(v)$.
    
- **Basis Mapping Check:** Set $x = v_i$ (coefficients $a_i=1$, others $0$) to show $T(v_i) = w_i$.
    
- **Uniqueness:** Assume another linear transformation $U$ maps $v_i \to w_i$. Apply $U$ to $x = \sum a_i v_i$, use linearity to extract $U(v_i)$, substitute $w_i$, and conclude $U(x) = T(x)$.
