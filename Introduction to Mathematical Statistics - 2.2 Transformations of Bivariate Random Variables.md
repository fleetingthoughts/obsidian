---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#robert_hogg"
  - "#math"
  - "#statistics"
date_created: 2026-02-08
---
This chapter discusses the transformations of bivariate distributions that map the original random variables from $R^2 -> R^2$ that transforms it to another bivariate distribution. The majority of this chapter is just in examples to show the mathematical techniques to find the pmf or CDF of the transformed random variable if we know the original bivariate distribution. We extend the work we did in section [Introduction to Mathematical Statistics - 1.6 Discrete Random Variables](Introduction%20to%20Mathematical%20Statistics%20-%201.6%20Discrete%20Random%20Variables.md) and [Introduction to Mathematical Statistics - 1.7 Continuous Random Variables](Introduction%20to%20Mathematical%20Statistics%20-%201.7%20Continuous%20Random%20Variables.md). 


We start with the discrete case. Given a known joint distribution of $(X_1,X_2)$ that is $p_{X_1,X_2}(X_1,X_2)$ with the support on $S$. We seek the distribution of a transformation $Y_{1} = g(X_1,X_2)$  and $Y_2 =h(X_1,X_2)$ that maps the original support $S$ to $T$. The joint pmf of $(Y_1,Y_2)$ is then:
$$p_{Y_1,Y_2}(y_1,y_2) = p_{X_1,X_2}(w_1(y_1,y_2),w_2(y_1,y_2))$$
where $w_1, w_2$ are the single-valued inverse of $y_1=g(x_1,x_2)$ and $y_2 = h(x_1,x_2)$ respectively. Note that this means the transformation must be bijective so that an inverse function that maps $Y_1,Y_2 \to X_1,X_2$ exists.

If we simply care for only one of the transformed random variables, $Y_1$, and are only considered with the univariate case, we can simply find the marginal distribution of $p_{Y_1,Y_2}(y_1,y_2)$. Note that we NEED two "new variables" to perform the change of variable technique. There is no such change in variable for a $R^2 \to R$ function. 

Now we direct our attention to the continuous case. Similar to the univariate case, the continuous random variable is defined by the cdf and so we use the same techniques from [Introduction to Mathematical Statistics - 1.7 Continuous Random Variables](Introduction%20to%20Mathematical%20Statistics%20-%201.7%20Continuous%20Random%20Variables.md) to find the cdf of the transformed variable. From there we cam differentiate to find the pdf. Unlike with the discrete case, we do not find the pdf immediately. The derivative we use in the multivariate case is called the Jacobian. In the bivariate case, it is as follows:

$$J = \begin{vmatrix} \frac{\partial x_{1}}{\partial y_{1}} & \frac{\partial x_{1}}{\partial y_{2}}\\\frac{\partial x_{2}}{\partial y_{1}} & \frac{\partial x_{2}}{\partial y_{2}}\end{vmatrix}$$
Note that in the univariate case, this determinant collapses into one derivative. Given the same knowns as what we had described for the discrete case, the pdf of the transformed random variable is then:
$$f_{Y_1,Y_2}(y_1,y_2) = f_{X_1,X_2}(w_1(y_1,y_2), w_2(y_1,y_2))|J|$$
# Moment generating function (mgf) technique
We can use the fact that the mgf uniquely characterizes the distribution to find the distribution of functions of random variables which <u>works well for linear functions of random variables</u>. This technique is illustrated by example by Hogg.