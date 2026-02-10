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
Hence, the probabilities of all events of the form $(x_1, x_2] \times (x_3,x_4]$ can be determined. Note how the intersection of the ordered pairs is right inclusive (see definition of cdf from 1.5).

# 2.1.1 Marginal Distributions

Marginal distributions are derived from the multivariate distribution by restricting the number of dimensions. In the bivariate case, the marginal distribution is univariate, and this univariate distribution can be obtained from the original bivariate joint distribution. Essentially, the marginal distribution is the probabilities of a variable regardless of the outcomes of the other variables. Given a joint cdf, $F_{X_1,X_2}$ , the marginal distribution $F_{X_1}$ is the event where $\{X_1 \le x_1\}$, and this is equivalent to:
$$\{X_1 \le x_1\}=\{X_1 \le x_1\} \cap \{-\infty \lt X_2 \lt \infty\}$$
This equality follows from [the law of total probabilities](Introduction%20to%20Mathematical%20Statistics%20-%201.4%20Conditional%20Probability%20and%20Independence.md)
The equivalency is our way to determine the univariate distribution of any singular random variable given a joint distribution: 
$$F_{X_1}(x_{1}) = F_{X_1,X_2}(x_1,\infty)$$
In the case of discrete random variables, tables are frequently employed for bivariate.

Its trivial to show that the marginal distributions satisfy the properties of being a pmf/pdf if we assumed that the joint distribution was a proper pmf/pdf
# 2.1.2 Expectation
When discussing expectation of a function involving a bivariate distribution, we have to distinguish whether the we want the number mean or vector mean. In this book, we will discuss the real-number mean in which case it doesn't make sense to discuss the expectation of a random vector and it only makes sense to discuss the expectation of a real-valued function. And so given a random vector $(X_1,X_2)$ with a cdf $F_{X_1,X_2}$, we can only look at expectation if there is a single-variable real-valued function $Y = g(X_1,X_2)$ that maps the real-vector to the real numbers (otherwise we can't do any math!). The expectation if defined analogously to [the univariate case](Introduction%20to%20Mathematical%20Statistics%20-%201.8%20Expectation%20of%20a%20Random%20Variable.md):
$$E(Y) = \int_{-\infty}^{\infty}\int_{-\infty}^{\infty}g(x_{1},x_2)f_{X_1,X_2}(x_1,x_2) dx_1dx_2$$ which must exists if it absolutely converges (same condition as the univariate case). 

These definitions aren't arbitrary as the univariate case should be obtainable from the definition in the bivariate case and also share the same properties such as the linearity property:

***Theorem 2.1.1. (Linearity of the Expectation of a Random variable of a Random Vector).*** Let $(X_1,X_2)$ be a random vector and $Y = g(X_1,X_2)$  and $Y_2 = h(X_1,X_2)$ be  random variables that maps the random vector $R^2 \to R$ and their expectation exists, then:
$$E(k_1Y_1+k_2Y_2)=k_1E(Y_1)+k_2E(Y_2)$$Proof. The existence of the expression on the left-side of the equality is established by the assumed absolute convergence of the limts $E(Y_1)$ and $E(Y_2)$ and applying the triangular inequality to show that expectations of the sums also absolutely converges. The right-hand side of the equality is just the linearity of the integral.

Now using the expectation, we define the moment generating function.
***Definition 2.1.2 (Moment Generating Function of a Random Vector).*** Let $(X_1,X_2)$ be a random vector. If $E(e^{t_1X_1+t_2X_2)})$ exists for $|t_1| < h_1$ and $|t_2|<h_2$ where $h_1$ and $h_2$ are positive, then that expectation is called the moment generating function and denoted $M_{X_1,X_2}(t_1,t_2)$.

Note that this definition and the summing of the random variables in the exponential isn't arbitrary for the univariate "marginal moment generating function" can be obtained by setting one of $t's$ to zero for then we have:
$$M_{X_1,X_2}(t_1,0)  = \int_{-\infty}^{\infty}\int_{-\infty}^{\infty}e^{t_{1}X_{1}}f_{X_1,X_2}(x_1,x_2) dx_1dx_2$$ And then applying the definition of the marginal probability distribution:
$$= \int_{-\infty}^{\infty}e^{t_{1}X_{1}}f_{X_1}(x_1) dx_1$$
This explanation I have offers the mechanical way we can obtain the original univariate definition of the moment generating function, but I still need to think of a moral way of explaining why setting $t_2 =0$ works and what axiom that comes from.