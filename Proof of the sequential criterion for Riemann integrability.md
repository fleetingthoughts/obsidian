---
parent: "[[Understanding Analysis - 7.2 Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: A bounded function $f: [a, b] \to \mathbb{R}$ is Riemann-integrable on $[a, b]$ if and only if there exists a sequence of partitions $(P_n)_{n=1}^\infty$ of $[a, b]$ such that $\lim_{n \to \infty} [U(f, P_n) - L(f, P_n)] = 0$, in which case $\int_a^b f = \lim_{n \to \infty} U(f, P_n) = \lim_{n \to \infty} L(f, P_n)$.
#### Notes
1. **($\Rightarrow$)** For each $n \in \mathbb{N}$, apply the Integrability Criterion with $\epsilon = \frac{1}{n}$ to get $P_n$ satisfying $0 \le U(f, P_n) - L(f, P_n) < \frac{1}{n}$. By the Squeeze Theorem, $\lim [U(f, P_n) - L(f, P_n)] = 0$.
2. **($\Leftarrow$)** Fix $\epsilon > 0$. Since $U(f, P_n) - L(f, P_n) \to 0$ and $U \ge L$, there exists $N \in \mathbb{N}$ such that $U(f, P_N) - L(f, P_N) < \epsilon$. Taking $P_\epsilon = P_N$, $f$ is integrable by the Integrability Criterion.
3. **Limit Value:** Since $L(f, P_n) \le L(f) = \int_a^b f = U(f) \le U(f, P_n)$ for all $n$, both $U(f, P_n) - \int_a^b f$ and $\int_a^b f - L(f, P_n)$ lie in $\big[0,\; U(f, P_n) - L(f, P_n)\big]$. Since the right endpoint $\to 0$, the Squeeze Theorem gives $\lim U(f, P_n) = \lim L(f, P_n) = \int_a^b f$. $\blacksquare$
<!--SR:!fsrs,2026-11-25T22:36:05.802Z,0,1.2931,5.11217071,1,1,0,0,2026-11-25T22:30:05.802Z-->
    
- **Backward verification ($\impliedby$):** Given $\epsilon \gt 0$, convergence to $0$ provides $N \in \mathbb{N}$ such that $U(f, P_N) - L(f, P_N) \lt \epsilon$, satisfying the Darboux integrability criterion.
    
- **Integral value squeeze:** Combine $L(f, P_n) \le L(f) = \int_a^b f = U(f) \le U(f, P_n)$ with $U(f, P_n) - L(f, P_n) \to 0$ to conclude $\lim_{n \to \infty} U(f, P_n) = \lim_{n \to \infty} L(f, P_n) = \int_a^b f$.
