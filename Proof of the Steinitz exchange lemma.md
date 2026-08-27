---
tags:
  - flashcard
  - macro/math/friedberg/ch1
date_created: 2026-07-24
parent:
---
Prove the Steinitz Exchange Lemma
#### Notes
- Proceed by induction on $m$ (size of independent set $L$). Base $m=0$: $L=\emptyset$, choose $H=G$.
- Assume true for $m$. Let $L = \{v_1, \dots, v_{m+1}\}$ be independent. By the induction hypothesis, $m \le n$, and there exists $H_0 = \{u_1, \dots, u_{n-m}\} \subseteq G$ such that $L_m \cup H_0$ spans $V$.
- Express $v_{m+1}$ as a linear combo of $v_1 \dots v_m$ and $u_1 \dots u_{n-m}$. Since $L$ is independent, some $u_j$ coefficient must be non-zero (proving $m < n$).
- Assume $b_1 \neq 0$. Solve algebraically for $u_1$ in terms of $v_{m+1}$ and the remaining vectors.
- Substitute $u_1$ out of the generating set, replacing it with $v_{m+1}$. The new set still spans $V$ and has exactly $n - (m+1)$ vectors from $G$.
