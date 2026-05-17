---
tags:
  - math
  - real_analysis
date_created: 2026-05-17
---
***Theorem 2.3.3 (Algebraic Limit Theorem).*** Let  $lim_{n \to \infty}a_n=a$
and $lim_{n \to \infty}b_n=b$. Then we have:
(i) $lim(ca_n)$ = ca, for all $c ∈ R$; 
(ii) $lim(a_n + b_n) = a + b$; (proved using the triangular inequality)
(iii) $lim(a_nb_n) = ab$; (prove using triangular inequality and using the trick of adding extra terms that sum to 0. We also have to apply Theorem 2.3.2)
(iv) $lim(a_n/b_n) = a/b$ , provided $b \ne  0$ 

The proof from each of these theorems involve setting our presumed convergent series $|a_n-a| \lt \text{anything we like}$ which by hypothesis we can do by setting $n >N$. Then algebraically manipulate it to our goal of $$|\text{(terms of sequence)} - \text{(proposed limit) } | < \epsilon$$
But to determine that "anything we like" we do some math toolbox-esque "black magic" to construct it.

I think it is useful to see the proof for (iv) to show the math tricks involved to prove convergence and its application of the [Reverse Triangle inequality.](Reverse%20Triangle%20inequality..md) Proof: Assuming (iii) is true, it is then sufficient to prove (iv) by showing $(b_n) \to b \implies \frac{1}{b_n} \to \frac{1}{b}$ . We now apply our math toolbox-esque "black magic" to reverse engineer the $|\frac{1}{b_n} \to \frac{1}{b}| \lt \text{anything we like}$
1) $$ \frac{1}{b_n} \to \frac{1}{b} = \frac{|b_n-b|}{|b_n||b|}$$

The difficulty here is with the $|b_n|$ term which is not a constant and we cannot apply Theorem 2.3.2 to replace it with a constant, but we do take advantage of the fact that we can make $b_n$ close to $b$ then to 0 namely by assumption we can select $n \ge N_1$ such that:
2) $$|b_n-b| \lt \frac{|b|}{2}$$
By [Reverse Triangle inequality.](Reverse%20Triangle%20inequality..md):
3) $$|b_n|-|b| \le |b_n - b|$$
so combining 3) into 2) we have:
$$|b_n| \lt \frac{3|b|}{2}$$
4) $$|b_n| \gt \frac{3|b|}{2}\gt \frac{|b|}{2}$$
So overall we have our target epsilon reverse engineered by combining 4) into 1):
$$\frac{1}{b_n} \to \frac{1}{b} = \frac{|b_n-b|}{|b_n||b|}\lt \frac{2|b_n-b|}{|b|^2}$$So if we simply set $n >N_{2}$ such that $|b_n - b| \lt \epsilon\frac{|b|^2}{2}$ while simultaneously letting $n \gt N_1$ to satisfy 2) by setting $n \gt max(N_1,N_2)$, then we obtain our desired convergence criteria for $|\frac{1}{b_n} \to \frac{1}{b}| \lt \epsilon$ 

