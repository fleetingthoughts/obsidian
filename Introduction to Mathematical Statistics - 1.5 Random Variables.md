tag: #math #statistics #robert_hogg
parent:[Introduction to Mathematical Statistics - 1 Probability and Distributions](Introduction%20to%20Mathematical%20Statistics%20-%201%20Probability%20and%20Distributions.md)


***Definition 1.5.1 (Random Variables).*** Given a sample space $C$. A function $X$ which assigns each element $c \in C$ to one and only one number $X(c) =x$ is called a random variable. The space or range of $X$ is the set of real numbers.

We try to ascribe some kind of math object to represent our sample space and often preferably with real numbers. Notice that we defined the image of the random variable as the set of ALL real numbers? We can simply set the other numbers that obviously aren't part of the sample as just 0. The probability function instead of mapping our sample space can now map real numbers to other real numbers with our random variable function. The probability functions that act on random variables (i.e. real numbers) are referred to as the probability mass function (pmf) in the case of discrete random variables and probability density functions (pdf) in the case of continuous random variables.
***Definition 1.5.2 (Cumulative Distribution Function).*** For random variable $X$, its <u>cumulative distribution function (cdf) </u> is defined by $F_X(x)$ where
$$F_{x}(x)= P_{x}((-\infty , x ])=P({c \in C: X(c) \le x})$$
It is the "cumulative" probabilities of all the random variables leading up to $x$ . The pdf uniquely determine the cdf and vice versa by the fundamental theorem of calculus. Not sure about the pmf. Normally the cdf is the more desirable function to have because differentiating to the pdf is easy but integration may not easily yield an analytical solution.

From this definition of cdf, we can derive some properties:

***Theorem 1.5.1 (Properties of the cdf).*** Given the random variable $X$ with its cumulative distribution function $F(x)$ :
1) if $a \lt b$ then $F(a) \le F(b)$ 
2) $lim_{x \to -\infty} F(x) = 0$ 
3) $lim_{x \to +\infty} F(x) = 1$ 
4) $lim_{x \to +x_{o}} F(x) = F(x_{o})$ (the cdf is right continuous)
Proof of 1) follows from [Theorem 1.3.3](Introduction%20to%20Mathematical%20Statistics%20-%201.1%20to%201.3.md).  

Proof of 4) is demonstrated by constructing a a decreasing set of $(-\infty , y_i)$  where $(y_i)$ is a sequence of decreasing numbers with $lim_{n \to \infty} y_n = x_o$. The sequence of sets is decreasing with $\cap_{n=1}^{\infty}C_n = \{x \le x_o\}$ and the probability of the limit of this sequence of set follows from [Theorem 1.3.6](Introduction%20to%20Mathematical%20Statistics%20-%201.1%20to%201.3.md). Notice that an attempt to construct an increasing set will never actually contain the point $x_o$. The right-continuity of $F(x)$ is guaranteed because $F(x) = P(X\le x)$ contains the point $x$ and is NOT $F(x) = P(X \lt x)$. If we want to force the CDF to be left continuous but not right continuous then we must define it to not contain the point that is: $F(x) = P(X \lt x)$ in which case our proof of 4) cannot hold because we cannot create a decreasing set that does not contain $x_o$. This simply makes the CDF left-continuous by changing the convention to not contain the point, but it does not change the fact that at $X = x_o$, we still have CDF at this point be right-continuous. This distinction becomes important for the case where we have discontinuities in the CDF:

***Theorem 1.5.3 (probabilities at jump discontinuities)*** $P(X= x) = F_X (x)- F_x (x-)$ for all $x \in R$ where $F_X(x-) = \lim_{z \to x}F_X(z)$.



