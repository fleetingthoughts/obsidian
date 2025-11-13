tags:: #math #math_tricks #math_toolbox 
following is a lemma of the [Binomial Theorem](Binomial%20Theorem.md). 
***Lemma (lower bound on binomials).*** If $h$ is a positive number and $n$ is a natural number, then:
$$1+nh\le (1+h)^n$$

The inequality follows trivially from the binomial formula as $1+nh$ is just the first two terms of the full summation. More generally, we can refine the lower bound further with a greater lower bound by adding on more terms from the binomial theorem for example:
$$\frac{n(n-1)}{2}+1+nh \le (1+h)^n$$
This lemma is useful for furnishing lower bounds in terms of more manageable polynomials. As an example, this lemma was used in Richard Courant and John Fritz's Calculus book to show that the $\sqrt[n]{p}$ ,  $\sqrt[n]{n}$  all tend to 1 as $n$ goes to infinity for some positive $p$ and $\alpha^n$ tends to 0 for $0\le \alpha \lt 1$ . The trick was to rewrite the terms as a binomial $(1+h_n)$ so that $\sqrt[n]{p} = \sqrt[n]{n} = (1+h_n)$ where $h_n$ depended on choice of $n$ and show that $h_n$ tends to 0. 

As an example I show that the sequence of $(a_n)$ where $a_n = \alpha^n$ tends to 0 for $0\le \alpha \lt 1$. Begin by rewriting $\alpha$ as a binomial and apply our lemma:
$$a_n = \alpha^n=\frac{1}{(1+h_n)^n}$$
and applying our lemma we obtain:
$$a_n = \alpha^n=\frac{1}{(1+h_n)^n} \le \frac{1}{1+nh} \lt \frac{1}{nh}$$
and we can certainly see that the right-most inequality tends to 0.
