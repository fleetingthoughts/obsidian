---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#robert_hogg"
  - "#math"
  - "#statistics"
date_created: 2026-02-11
---
This chapter looks at bivariate joint distributions where the random variables are independent of each other and we begin by defining what that means. The chapter then proves 4 different ways of determining whether the random variables in the joint distribution are independent:
1) By the definition using the marginal distributions
2) Using arbitrary nonnegative functions of the random variables (equivalent condition).
3) Using the CDFs (equivalent condition).
4) Using the product of the marginal cdf
5) Using the raw probabilities.
6) Using the mgf

In the context of the conditional random variable, we have by the definition of the conditional random variable:
$$f(x_1,x_2) = f_{2|1}(x_2|x_1)f_1(x_1)$$
<u>if $f_{2|1}$ depended only on $x_2$ and irrespective of our choice of $x_1$, </u>we can relate it to our definition of the marginal distribution $f_2(x) = \int_{-\infty}^{\infty}f(x_1,x_2)dx_2$. Since the definition of the conditional probability distribution assumes the existence of the marginal distribution for $X_1$, we find that
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
Note that the preceding theorems involved pdfs, but from that definition, you can derive an analogous relationship with the cdf. Note that the condition of Theorem 2.4.1 also rests on this new product having a support on the product space of the original support, that is the new support for $g(x_1)h(x_2)$ has a support on the cartesian product of $S_1 \times S_2$. An actual derivation of independence implying a product space of the support is beyond the scope of this book. Therefore, we would require the supports to be independent of each other. Supports such as $0 < x_1 < x_2 < 1$ will not result in an independent random variable

**Theorem 2.4.2 (Independence shown with the CDF)*** Given a joint distribution $f(x_1,x_2)$ with cdf $F(x_1,x_2)$ and marginal cdfs $F_1(x_1)$ and $F_2(x_2)$ . The random variables are independent if and only if for all $(x_1,x_2) \in R^2$ 
$$F(x_1,x_2) \equiv F_1(x_1)F_2(x_2)$$This relationship is valid for all of $R^2$ instead of just the product space of the respective supports. This done by proving sufficiency condition and then the converse by the definition of the cdf and the definition of independence using the pdf.

We can also demonstrate independence by looking at the relationship of the raw probabilities without even knowing the analytical form of the original distribution

***Theorem 2.4.3 (Determine independence from the raw probabilities).*** The random variables $X_1$ and $X_2$ are said to be independent if the following relationship holds:
$$P(a \lt X_1 \le b, c \lt X_2 \le d) = P(a \lt X_1 \le b)P(c \lt X_2 \le d)$$
This can be easily proved by definition of the cdf and relating it to ***Theorem 2.4.2***. Note the right hand equalities are strict by [derived properties of the cdf](Introduction%20to%20Mathematical%20Statistics%20-%201.7%20Continuous%20Random%20Variables.md). 

***Theorem 2.4.3*** shows that the calculation of probabilities is greatly simplified and we can look at the variables one at a time. This simplification extends to other important parameters as well:

***Theorem 2.4.4. (The expectation of independent random variables).*** If $(X_1,X_2)$ are independent random variables and $u(x_1)$ and $v(x_2)$ are functions on the support of the random variable, then the product of the functions is as follows:
$$E[u(x_1)v(x_2)]=E[u(x_1)]E[v(x_2)]$$

Finally we can use the fact that the mgf, when it exists is unique and uniquely determines the probability distribution to demonstrate the independence of a variable.

***Theorem 2.4.5. (Determine Independence using the mgf).*** If the mgf $M(t_1,t_2)$ exists for the joint distribution of $X_1$ and $X_2$, then the random variables are independent if and only if:
$$M(t_1,t_2) \equiv M(t_1,0)M(0,t_2)$$The proof follows from the definition of the mgf to prove the sufficiency and converse and applying the properties of exponentials and integrals.

# Conceptual Summary and nuances
- How to determine the support of a joint distribution given the support of the marginal distribution: the support of the joint probability of two independent random variables is the cartesian product of the supports. This means the support of the joint distribution changes to the cartesian product of the support of the respective marginal distributions
- If we are able to factorize a joint distribution into two nonnegative functions $f(x,y)=g(x)h(y)$, those two functions  differ from the marginal pdfs by a multiplicative constant, that is we have the following: $$f_x=c_1g(x) \quad \text{and\quad} f_y=c_2h(y)$$
# Computational Summary
1) How to determine if the random variables of a joint distribution are independent directly from the definition:
	- If we know the marginal distributions or compute the marginal distributions. Take the product and determine if we get back the joint distribution
2) Determine independence by factorization using ***Theorem 2.4.1***, ***Theorem 2.4.2.***, and ***Theorem 2.4.3.***:
	- ***Eyeballing the definition.*** if the joint distribution can be factored into a product of a function of solely the individual random variables. 
	- ***Division by marginal pdf.*** We can also compute one of the marginal pdfs and see if division results in a function of just the other random variable, in which case independence is confirmed. Then the dividend will necessarily be the marginal pdf of the other function hence we do not need to compute the other marginal pdf from first principles.
	- ***Factorize the joint CDF.*** See if the joint CDF factors into functions solely of the random variables
	- ***Factorize the joint MGF.*** See if the joint MGF factors into a product of the marginal mgfs
	- ***Factorize the joint mgf/cdf/pdf into arbitrary nonnegative functions with independent support.*** For all the above points about factorization into marginal cdfs/mgfs/probabilities is also true if the joint mgf/cdf factors into the product of nonnegative functions provided the respective supports are independent (i.e. the cartesian product of the support returns the original joint support).
3) Short cut to determine the expectation of the product of functions of independent random variables:
	- The expectation operator is multiplicative over the product of the respective functions

# Concepts from Exercises

# Definitions
***Definition 2.4.1 (Independence).*** Two random variables $X_1$ and $X_2$ with respective support $S_1$ and $S_2$ are said to be independent if the joint distribution is equivalent to the product of the marginal distributions with the support in the cartesian product $S_1 \times S_2$ . In the continuous case, this is denoted as follows: $$f(x_{1},x_{2})\equiv f_{X_{1}}(x_{1})f_{X_{2}}(x_{2})$$
# Theorems
***Theorem 2.4.1 (Equivalent condition condition for independence of two random variables given the joint distribution by factorization of arbitrary nonnegative functions).*** Given a joint distribution $f$ of two random variables $X_1$ and $X_2$ with the respective support $S_1$ and $S_2$. The random variables are independent <u>if and only if</u> the joint distribution can be written as the product of any two nonnegative arbitrary functions of each random variable respectively with the support in the cartesian product $S_1 \times S_2$ : $$f(x_1,x_2)\equiv g(x_1)h(x_2) \quad \text{ for \quad} x_{1}\in S_{1}, x_{2}\in S_{2}$$
***Theorem 2.4.2 (The factorizability of the joint cdf into the marginal cdfs as an equivalent condition to independence)*** Given a joint distribution $f(x_1,x_2)$ with cdf $F(x_1,x_2)$ and marginal cdfs $F_1(x_1)$ and $F_2(x_2)$ . The random variables are independent if and only if for all $(x_1,x_2) \in R^2$ 
$$F(x_1,x_2) \equiv F_1(x_1)F_2(x_2)$$
***Theorem 2.4.3 (Determine independence from the raw probabilities).*** The random variables $X_1$ and $X_2$ are said to be independent if the following relationship holds:
$$P(a \lt X_1 \le b, c \lt X_2 \le d) = P(a \lt X_1 \le b)P(c \lt X_2 \le d)$$
This can be easily proved by definition of the cdf and relating it to theorem 2.4.2. Note the right hand equalities are strict by [derived properties of the cdf](Introduction%20to%20Mathematical%20Statistics%20-%201.7%20Continuous%20Random%20Variables.md). 

***Theorem 2.4.4. (The expectation of independent random variables).*** If $(X_1,X_2)$ are independent random variables and $u(x_1)$ and $v(x_2)$ are functions on the support of the random variable, then the product of the functions is as follows: