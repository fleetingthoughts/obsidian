---
parent: "[[Introduction to Calculus I by Fritz and Courant - 1.1 Continuum of Numbers]]"
tags:
  - "#flashcard"
  - micro/math/courant_calc1/ch1
date_created: 2026-07-24
---
State and derive the Rational Root theorem and its implication for determining the rationality of a number
#### Notes
- **Statement:** If a polynomial $P(x) = a_nx^n + a_{n-1}x^{n-1} + \dots + a_1x + a_0$ with integer coefficients has a rational root $x = \frac{p}{q}$ (where $p$ and $q$ are coprime integers), then $p$ divides the constant term $a_0$ and $q$ divides the leading coefficient $a_n$.
    
- **Derivation 1 (Substitution):** Set $P(\frac{p}{q}) = 0$ and multiply the entire equation by $q^n$ to clear the denominators:
$$a_np^n + a_{n-1}p^{n-1}q + \dots + a_1pq^{n-1} + a_0q^n = 0$$
    
- **Derivation 2 (Proving $p\vert{}a_0$):** Isolate the $a_0$ term to obtain $a_0q^n = -p(a_np^{n-1} + \dots + a_1q^{n-1})$. The right side is a multiple of $p$, meaning $p$ divides $a_0q^n$. Because $p$ and $q$ are coprime ($\gcd(p,q)=1$), $p$ must strictly divide $a_0$.
- **Derivation 3 (Proving $q\vert{}a_n$):** Isolate the $a_n$ term to obtain $a_np^n = -q(a_{n-1}p^{n-1} + \dots + a_0q^{n-1})$. The right side is a multiple of $q$, meaning $q$ divides $a_np^n$. Because $p$ and $q$ are coprime, $q$ must strictly divide $a_n$.

**Implication for Rationality**
- **Monic Polynomials:** Consider a number like $\sqrt[k]{c}$ (where $c$ is an integer). It is a root of the monic polynomial $x^k - c = 0$.
- **Integer Constraint:** Applying the theorem, any rational root $p/q$ must have its denominator $q$ divide the leading coefficient ($a_n = 1$). Therefore, $q = \pm 1$, meaning any rational root is forced to be an integer.
- **Conclusion:** This implies that the $k$-th root of an integer is strictly either an integer or an irrational number; it is mathematically impossible for it to be a non-integer rational fraction
