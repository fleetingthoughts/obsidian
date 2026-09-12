---
parent: "[[Understanding Analysis - 2.3 The Algebraic and Order Limit Theorems]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch2
date_created: 2026-09-11
---
Outline the proof that if the double limit $\lim_{m,n\to\infty} a_{mn}$ exists and both iterated limits exist, then all three limits must be equal.
#### Notes
First prove that if the double limit $\lim_{m,n\to\infty} a_{mn} = a$, and for each fixed $m$, $\lim_{n\to\infty} a_{mn} = b_m$, then $\lim_{m\to\infty} b_m = a$.
- Let $\epsilon > 0$. By the definition of the double limit, there exists $N_1 \in \mathbf{N}$ such that for all $m, n \ge N_1$, $\vert{}a_{mn} - a\vert{} < \epsilon/2$.
- Fix any $m \ge N_1$. Since $\lim_{n\to\infty} a_{mn} = b_m$, there exists an $N_2 \in \mathbf{N}$ such that for all $n \ge N_2$, $\vert{}a_{mn} - b_m\vert{} < \epsilon/2$.
- Choose an $n$ such that $n \ge \max(N_1, N_2)$. Using the triangle inequality, $\vert{}b_m - a\vert{} = \vert{}b_m - a_{mn} + a_{mn} - a\vert{} \le \vert{}b_m - a_{mn}\vert{} + \vert{}a_{mn} - a\vert{}$.
- Substituting our bounds, $\vert{}b_m - a\vert{} < \epsilon/2 + \epsilon/2 = \epsilon$.
- Since for any $m \ge N_1$, we have $\vert{}b_m - a\vert{} < \epsilon$, it follows by definition that $\lim_{m\to\infty} b_m = a$.

Now we prove all 3 limits are equal
- Let the double limit $\lim_{m,n\to\infty} a_{mn} = a$.
- By the hypothesis that the iterated limits exist, let the inner limit $\lim_{n\to\infty} a_{mn} = b_m$ for each $m$.
- By the result of the previous proof, since the double limit is $a$ and the inner limit is $b_m$, the outer limit $\lim_{m\to\infty} b_m$ must equal $a$. Therefore, $\lim_{m\to\infty} (\lim_{n\to\infty} a_{mn}) = a$.
- Apply the exact same logic symmetrically: let the other inner limit $\lim_{m\to\infty} a_{mn} = c_n$. The outer limit must evaluate to $a$, so $\lim_{n\to\infty} (\lim_{m\to\infty} a_{mn}) = a$.
- Thus, both iterated limits equal the double limit $a$.