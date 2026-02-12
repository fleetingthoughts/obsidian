---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#robert_hogg"
  - "#math"
  - "#statistics"
date_created: 2026-02-11
---
This chapter looks at bivariate joint distributions where the random variables are independent of each other and we begin by defining what that means.

In the context of the conditional random variable, we have by the definition of the conditional random variable:
$$f(x_1,x_2) = f_{2|1}(x_2|x_1)f_1(x_1)$$
if $f_{2|1}$ depended only on $x_2$ and irrespective of our choice of $x_1$, we can relate it to our definition of the marginal distribution $f_2(x) = \int_{-\infty}^{\infty}f(x_1,x_2)dx_2$. Since the definition of the conditional probability distribution assumes the existence of the marginal distribution for $X_1$, we find that
$$f_2(x)= \int_{-\infty}^{\infty}f(x_1,x_2)dx_1$$
$$f_2(x)= \int_{-\infty}^{\infty}f_{2|1}(x_2|x_1)f_1(x_{1})dx_1$$

And since the marginal distribution is itself a pdf that integrates to 1:
$$f_2(x)= f_{2|1}(x_2|x_1)$$
And so, if $X_2$ is independent of $X_1$ then we find that the marginal distribution is equivalent to the conditional distribution. This motivates the following definition for independence
***Definition 2.4.1 (Independent Random Variables).*** Let $(X_1,X_2)$ be random variables with the joint pdf $f(x_1,x_2)$. The random variables are said to be independent if and only if over the support of $f$ 
$$f(x_1,x_2) \equiv f_1(x_1)f_2(x_2)$$
The algorithm to determine whether a joint distribution consists of random variables is to compute the marginal distributions and see if the identity is equivalent to the original distribution, but the following theorem lets us determine independence without computing marginal probabilities by using other functions.

***Theorem 2.4.1 (Determine independence without using marginal distributions).*** Let the random variables $X_1$ and $X_2$ have supports $S_1$ and $S_2$ respectively with the joint pdf $f(x_1,x_2)$. The variables are independent if and only if there are nonnegative functions  $g$ and $h$ of $x_1$ and $x_2$ on their respective supports such that:
$$f(x_1,x_2) \equiv g(x_1)h(x_2)$$
Note that the preceding theorems involved pdfs, but from that definition, you can derive an analagous relationship with cdfs:

**Theorem 2.4.2 (Independence shown with the CDF)*** Given a joint distribution $f(x_1,x_2)$ with cdf $F(x_1,x_2)$ and marginal cdfs $F_1(x_1)$ and $F_2(x_2)$ . The random variables are independent if and only if for all $(x_1,x_2) \in R^2$ 
$$F(x_1,x_2) \equiv F_1(x_1)F_2(x_2)$$Note that this relationship is valid for all of $R^2$ instead of just the product space of the respective supports. This done by proving sufficiency condition and then the converse by the definition of the cdf and the definition of independence using the pdf.

We can also demonstrate independence by looking at the relationship of the raw probabilities without even knowing the analytical form of the original distribution

***Theorem 2.4.3 (Determine independence from the raw probabilities).*** The random variables $X_1$ and $X_2$ are said to be independent if the following relationship holds:
$$P(a \lt X_1 \le b, c \lt X_2 \le d) = P(a \lt X_1 \le b)P(c \lt X_2 \le d)$$
This can be easily proved by definition of the cdf and relating it to theorem 2.4.2. Note the right hand equalities are strict by [derived properties of the cdf](Introduction%20to%20Mathematical%20Statistics%20-%201.7%20Continuous%20Random%20Variables.md). 

Finally we can use the fact that the mgf, when it exists is unique and uniquely determines the probability distribution to demonstrate the independence of a variable.

***Theorem 2.4.5. (Determine Independence using the mgf).*** If the mgf $M(t_1,t_2)$ exists for the joint distribution of $X_1$ and $X_2$, then the random variables are independent if and only if:
$$M(t_1,t_2) \equiv M(t_1,0)M(0,t_2)$$ 