---
parent: "[[Understanding Analysis - 7.3 Uniform Convergence and the Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: Thomae's function $t : [0, 1] \to \mathbf{R}$, defined by $t(x) = \frac{1}{n}$ if $x = \frac{m}{n} \in \mathbf{Q}$ in lowest terms ($n \gt 0$), $t(0) = 1$, and $t(x) = 0$ if $x \notin \mathbf{Q}$, is Riemann-integrable on $[0, 1]$ with $\int_0^1 t = 0$.
#### Notes
- Observe that for any partition $P$ of $[0, 1]$, the density of irrationals in every subinterval forces $m_k = 0$, so $L(t, P) = 0$ and $L(t) = 0$.
    
- Given $\epsilon \gt 0$, observe that the set $D_{\epsilon/2} = \{x \in [0, 1] : t(x) \ge \frac{\epsilon}{2}\}$ is finite because there are only finitely many rationals in $[0, 1]$ with denominators $n \le \frac{2}{\epsilon}$.
    
- Let $N = \vert{}D_{\epsilon/2}\vert{}$ and construct a partition $P_\epsilon$ that encloses the $N$ points of $D_{\epsilon/2}$ inside subintervals whose combined length is less than $\frac{\epsilon}{2}$.
    
- Split $U(t, P_\epsilon) = \sum_{k=1}^m M_k \Delta x_k$ into subintervals intersecting $D_{\epsilon/2}$ (where $M_k \le 1$) and remaining subintervals (where $M_k \lt \frac{\epsilon}{2}$ and $\sum \Delta x_k \le 1$):
    
    $$U(t, P_\epsilon) \lt 1 \cdot \left(\frac{\epsilon}{2}\right) + \left(\frac{\epsilon}{2}\right) \cdot 1 = \epsilon$$
    
- Conclude $U(t, P_\epsilon) - L(t, P_\epsilon) \lt \epsilon$, so $t$ is integrable with $\int_0^1 t = L(t) = 0$.
