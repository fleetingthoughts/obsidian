---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#statistics"
  - "#robert_hogg"
  - "#math"
date_created: 2026-02-06
---
We now transfer our understanding of single-variable probability distributions to multivariate distributions. A lot of this chapter is getting used to the notation once we move multi-dimensions.

***Definition 2.1.1. (Random Vector).*** Given a sample space $C$ of a random experiment, if we have two random variables $X_1, X_2$ that map every element of the sample space onto real numbers such that given the element $c$, we have functions $X_1(c) = x_1$ and $X_2(c) = x_2$. We then say the ordered pair of random variables $(X_1, X_2)$ is the random vector and the space, $D$, of $(X_1, X_2)$ is the set of all ordered pairs $D = \{(x_1,x_2): x_1 = X_1(c), x_2= X_2(C), c \in C\}$.

Similar to the univariate random variables, we can define the probabilities of a random vector, $P_{X_1,X_2}$ in terms of the cdf:
$$F_{X_1,X_2}(x_1,x_2) = P[(X_1 \le x_1) \cap (X_2 \le x_2)]$$
Hence, the probabilities of all events of the form $(x_1, x_2] \times (x_3,x_4]$ can be determined. Note how the intersection of the ordered pairs is right inclusive (see definition of cdf from [1.5 Random Variables](Introduction%20to%20Mathematical%20Statistics%20-%201.5%20Random%20Variables.md) where the unstrict inequality introduces the right-hand continuity convention as opposed to the left-handed continuity of the cdf).

# 2.1.1 Marginal Distributions

Marginal distributions are derived from the multivariate distribution by restricting the number of dimensions. In the bivariate case, the marginal distribution is univariate, and this univariate distribution can be obtained from the original bivariate joint distribution. Essentially, the marginal distribution is the probabilities of a variable regardless of the outcomes of the other variables. Given a joint cdf, $F_{X_1,X_2}$ , the marginal distribution $F_{X_1}$ is the event where $\{X_1 \le x_1\}$, and this is equivalent to:
$$\{X_1 \le x_1\}=\{X_1 \le x_1\} \cap \{-\infty \lt X_2 \lt \infty\}$$
This equality follows from [the law of total probabilities](Introduction%20to%20Mathematical%20Statistics%20-%201.4%20Conditional%20Probability%20and%20Independence.md)
The equivalency is our way to determine the univariate distribution of any singular random variable given a joint distribution: 
$$F_{X_1}(x_{1}) = F_{X_1,X_2}(x_1,\infty)$$
In the case of discrete random variables, tables are frequently employed for bivariate distributions.

Its trivial to show that the marginal distributions satisfy the properties of being a pmf/pdf if we assumed that the joint distribution was a proper pmf/pdf. 
# 2.1.2 Expectation
When discussing expectation of a function involving a bivariate distribution, we have to distinguish whether the we want the number mean or vector mean. In this book, we will discuss the real-number mean in which case it doesn't make sense to discuss the expectation of a random vector and it only makes sense to discuss the expectation of a real-valued function. And so given a random vector $(X_1,X_2)$ with a cdf $F_{X_1,X_2}$, we can only look at expectation if there is a single-variable real-valued function $Y = g(X_1,X_2)$ that maps the real-vector to the real numbers (otherwise we can't do any math!). The expectation if defined analogously to [the univariate case](Introduction%20to%20Mathematical%20Statistics%20-%201.8%20Expectation%20of%20a%20Random%20Variable.md):
$$E(Y) = \int_{-\infty}^{\infty}\int_{-\infty}^{\infty}g(x_{1},x_2)f_{X_1,X_2}(x_1,x_2) dx_1dx_2$$ which must exists if it absolutely converges same condition as [univariate case](Introduction%20to%20Mathematical%20Statistics%20-%201.8%20Expectation%20of%20a%20Random%20Variable.md) in ***Theorem 1.8.1***. 

These definitions aren't arbitrary as the definition for the bivariate case reduces to the univariate case shares the same properties such as the linearity property:

***Theorem 2.1.1. (Linearity of the Expectation of a Random variable of a Random Vector).*** Let $(X_1,X_2)$ be a random vector and $Y = g(X_1,X_2)$  and $Y_2 = h(X_1,X_2)$ be  random variables that maps the random vector $R^2 \to R$ and their expectation exists, then:
$$E(k_1Y_1+k_2Y_2)=k_1E(Y_1)+k_2E(Y_2)$$The proof of the formula trivially follows from the additivity of integrals, but the existence of this expectation assuming the existence of the expectation of $Y_1$ and $Y_2$ uses the triangular inequality. The existence of the expression on the left-side of the equality is established by the assumed absolute convergence of the limts $E(Y_1)$ and $E(Y_2)$ and applying the triangular inequality to show that expectations of the sums also absolutely converges. The right-hand side of the equality is just the linearity of the integral.

Now using the expectation, we define the moment generating function.
***Definition 2.1.2 (Moment Generating Function of a Random Vector).*** Let $(X_1,X_2)$ be a random vector. If $E(e^{t_1X_1+t_2X_2)})$ exists for $|t_1| < h_1$ and $|t_2|<h_2$ where $h_1$ and $h_2$ are positive, then that expectation is called the moment generating function and denoted $M_{X_1,X_2}(t_1,t_2)$.

We define the marginal mgf such that it is the expectation $E[e^{tX_1}]$ where $X_1$ is our random variable of interest, and the pdf is the marginal distribution. From this definition we have a general procedure to obtain the marginal mgf by setting the $t_i$ parameters to 0 for the random variables we don't care about:
$$M_{X_1,X_2}(t_1,0)  = \int_{-\infty}^{\infty}\int_{-\infty}^{\infty}e^{t_{1}X_{1}}f_{X_1,X_2}(x_1,x_2) dx_1dx_2$$ And then applying the definition of the marginal probability distribution:
$$= \int_{-\infty}^{\infty}e^{t_{1}X_{1}}f_{X_1}(x_1) dx_1$$
The above provides a way to generate the marginal moment generating function, but we can still determine the marginal moments without the specific "marginal moment generating function" but with the overall moment generating function of the random vector by taking partial derivatives:
$$\begin{align*} 
M(t_1,t_{2}) & = E(e^{t_{1}X_{1}+t_{2}X_{2}})\\
M(t_1,t_{2}) & = \int_{-\infty}^{\infty}\int_{-\infty}^{\infty}e^{t_{1}x_{1}+t_{2}x_{2}}f(x_{1},x_{2}) dx_{1}dx_{2}\\
\frac{\partial M}{\partial t_{1}} & =\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}x_{1}e^{t_{1}x_{1}+t_{2}x_{2}}f(x_{1},x_{2})dx_{2}dx_{1} \\
\frac{\partial M(0,0)}{\partial t_{1}} & =\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}x_{1}f(x_{1},x_{2}) dx_{2}dx_{1} \\
\frac{\partial M(0,0)}{\partial t_{1}} & =\int_{-\infty}^{\infty}x_{1}f_{x_{1}}(x_{1}) dx_{1}\\
\frac{\partial M(0,0)}{\partial t_{1}} & =E(X_{1})

\end{align*}$$
So we can also determine the marginal expectations by taking partial derivatives of the overall moment generating function if we already have it. There is no need to try to determine the marginal moment generating function.

# Summary
- Joint cdf defined by the intersection of the relevant sets
- Marginal distribution of a joint distribution is the cdf where we only have one variable of interest (in the bivariate case) such that the other variables can take any value. The marginal cdf is obtained by completely integrating over all the possible values of the variable we don't care about.
- Obtain marginal mgf by setting the $t_i$ of the random variable we don't care about to 0.
# Definitions
***Definition 2.1.1. (Random Vector).*** Given a sample space $C$ of a random experiment, if we have two random variables $X_1, X_2$ that map every element of the sample space onto real numbers such that given the element $c$, we have functions $X_1(c) = x_1$ and $X_2(c) = x_2$. We then say the ordered pair of random variables $(X_1, X_2)$ is the random vector and the space, $D$, of $(X_1, X_2)$ is the set of all ordered pairs $D = \{(x_1,x_2): x_1 = X_1(c), x_2= X_2(C), c \in C\}$.

***Definition 2.1.2 (Moment Generating Function of a Random Vector).*** Let $(X_1,X_2)$ be a random vector. If $E(e^{t_1X_1+t_2X_2)})$ exists for $|t_1| < h_1$ and $|t_2|<h_2$ where $h_1$ and $h_2$ are positive, then that expectation is called the moment generating function and denoted $M_{X_1,X_2}(t_1,t_2)$.
# Theorems

***Theorem 2.1.1. (Linearity of the Expectation of a Random variable of a Random Vector).*** Let $(X_1,X_2)$ be a random vector and $Y = g(X_1,X_2)$  and $Y_2 = h(X_1,X_2)$ be  random variables that maps the random vector $R^2 \to R$ and their expectation exists, then:
$$E(k_1Y_1+k_2Y_2)=k_1E(Y_1)+k_2E(Y_2)$$