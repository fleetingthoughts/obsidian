---
parent: "[[Understanding Analysis - 7.2 Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: A bounded function $f: [a, b] \to \mathbb{R}$ is Riemann-integrable on $[a, b]$ if and only if there exists a sequence of partitions $(P_n)_{n=1}^\infty$ of $[a, b]$ such that $\lim_{n \to \infty} [U(f, P_n) - L(f, P_n)] = 0$, in which case $\int_a^b f = \lim_{n \to \infty} U(f, P_n) = \lim_{n \to \infty} L(f, P_n)$.
#### Notes
- **Forward construction ($\implies$):** For each $n \in \mathbb{N}$, apply the Darboux integrability criterion with $\epsilon = 1/n$ to obtain $P_n$ satisfying $0 \le U(f, P_n) - L(f, P_n) \lt 1/n$, which converges to $0$ by the squeeze theorem.
    
- **Backward verification ($\impliedby$):** Given $\epsilon \gt 0$, convergence to $0$ provides $N \in \mathbb{N}$ such that $U(f, P_N) - L(f, P_N) \lt \epsilon$, satisfying the Darboux integrability criterion.
    
- **Integral value squeeze:** Combine $L(f, P_n) \le L(f) = \int_a^b f = U(f) \le U(f, P_n)$ with $U(f, P_n) - L(f, P_n) \to 0$ to conclude $\lim_{n \to \infty} U(f, P_n) = \lim_{n \to \infty} L(f, P_n) = \int_a^b f$.
