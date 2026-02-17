---
parent:
tags:
  - "#math"
  - "#real_analysis"
  - "#proof"
date_created: 2026-02-16
---
To prove that convergence is necessary for a sequence satisfying the Cauchy Criterion (i.e. a sequence that satisfies the Cauchy criterion is sufficient for convergence), we make use of the Bolzano-Weierstrass theorem to provide the condition for the limit to exist and use the convergent subsequence, $x_{n_k}$ as our proposed limit.

In order to make use of the Bolzano-Weierstrass theorem, we must show the following:

***Lemma 2.6.3.*** Cauchy sequences are bounded

To prove, we make use of the same strategy from another proof by using an actual number (not a general one) and showing that all but a finite # of terms must be bounded

Proof. Given that for $n,m>N$ we have $|x_n-x_m|<\epsilon$, we can then just choose $N$ that is large enough for $\epsilon=1$ and see that all but an $N$ # of terms must be bounded:

$$|x_n-x_N|<\epsilon$$
$$|x_{n}|-|x_{N}|<|x_n-x_N|<1$$

$$|x_{n}|<1+|x_{N}| \text{\qquad for n > N}$$
then the bound is simply the largest of the finite # $N-1$ terms or this bound for the infinite # of terms $$max\{|x_1|,|x_2|,|x_{3}|,...|x_{N-1}|, 1+|x_N|\}$$
Now that we've established that the Cauchy sequence satisfies the condition for the Bolzano-Weierstrass theorem, we use the limit of the subsequence as the proposed limit to prove the convergence of a Cauchy sequence, that is, our proposed limit will be the following:
$$x = \lim_{ k \to \infty }x_{n_k}$$


