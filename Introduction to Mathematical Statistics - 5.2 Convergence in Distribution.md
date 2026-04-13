---
tags:
  - math
  - statistics
  - robert_hogg
date_created: 2026-03-20
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
Sometimes, we cannot find a parameter that converges in probability to our parameter of interest, but we can determine a weaker form of convergence called "convergence in distribution" which allows us to answer the following:
- How close is a statistic to the estimator?
- Can we obtain the error of estimation?
***Definition 5.2.1*** defines convergence in probability, and the distribution that it converges to is called the <u>asymptotic distribution</u> or <u>limiting distribution</u>. While convergence in probability is a way of saying a random variables becomes essentially identical to another random variable (with some error), the convergence in distribution is seen as a weaker form that shows merely the cdfs become close to identical which is what ***Theorem 5.2.1*** states. 

Unlike with random variables that converge in probability that shares a lot of the usual algebraic properties as real numbers, their are more restrictions on what we can do with random variables that only converge in distribution. The properties are summarized as follows:
- The one time convergence in distribution is sufficient for convergence to probability: if a random variable converges in distribution to a constant, then it converges in probability
- Criteria for convergence in distribution with the sum and product of random variables: 
	- ***Theorem 5.2.3.*** The sum of two random variables converges to the asymptotic distribution of one its addends if the addend converges in distribution to said asymptotic distribution and the other <u>addend converges in probability to 0</u>
	- ***Theorem 5.2.5***: Slutsky's theorem demonstrates another condition for the convergence in distribution of multiple random variables if one of them converges to an asymptotic distribution while the others converge in probability to a constant
- ***Theorem 5.2.4***: Convergence in distribution is sufficient for the convergence in distribution of the transformation of the random variable where the distribution it converges to is the transformation of original asymptotic distribution as long as the transformation is continuous
A common problem we try to solve in statistics is determining the distribution of a function of a random variable if we know the distribution of the original random variable which is demonstrated 

The strength in the convergence of probability is its ability to provide a measure of the error in our estimators called the "bound in probability" defined in ***Definition 5.2.2***. ***Theorem 5.2.6*** shows that random variables that converge in distribution are bounded in probability, but the converse is not true.

The remainder of this section discusses ways that we can determine the limiting distribution of the random variable of which two are discussed:
- The $\triangle$-method
- The MGF technique
The search for the limiting distribution of a random variable or transformation of a random variable with a known limiting distribution is the central question in a field called asymptotic theory. One result that came from this theory is the $\triangle$-method which is a method to derive the asymptotic distribution of a random variable and specifically when a transformation of a random variable leads to a normal distribution. We have the following results from the $\triangle$-method which leads to the following results:
- ***Theorem 5.2.8*** provides a condition for when a random variable converges in distribution to 0.
- ***Theorem 5.2.9*** shows how the transformation of a random variable converges in distribution to the normal distribution with mean 0.

Another approach to determining the limiting distribution of a sequence of random variables is to make use of the fact that the mgf completely characterizes the cdf of a function. Namely as ***Theorem 5.2.10*** shows, if we can show that the mgf of a random variable converges with increasing sample size, to the mgf of a known distribution, then that known distribution is the asymptotic distribution

# Definitions
For all definitions and theorems, $(X_n)$ will represent a random sample of size of a random variable with distribution $F_X$.

- ***Definition 5.2.1 (Convergence in distribution).*** Given a sequence of random variables $(X_n)$ and a random variable $X$ with cdf $F_{X_n}$ and $F_X$ respectively, $X_n$ is said to converge in distribution to $F(X)$ if we have the following:$$\lim_{ n \to \infty }F_{X_{n}}(x)=F(x)\text{\quad for all }x\in C(F_{X}) $$
Where $C(F_X)$ denotes the set of all points where $F_X$ is continuous. The convergence in distribution in the above relation is also denoted $X_n \xrightarrow{D} X$.
- ***Definition 5.2.2 (Bounded in probability).*** We say that the sequence of randomvariables $(Xn)$ is bounded in probability if, for all $\epsilon > 0$ , there exist a constant $B_{\epsilon}>0$ and an integer $N_{\epsilon}$ such that:$$P(|X_{n}|\le B_{_{\epsilon}}) \ge 1-\epsilon \text{\quad for n such that } n\ge N_{\epsilon}$$
- ***Unofficial definition (little o-notation and big O-notation).*** The little and big o-notation has the following meaning for random variables $X_n$ and $Y_n$:
	- $Y_n = o_p(X_n)$ if and only if $\frac{Y_n}{X_n} \xrightarrow{P} 0$ as $n \to \infty$ 
# Theorems
- ***Theorem 5.2.1 (Convergence in probability implies convergence in distribution)*** If $X_n$ converges in probability to $X$, then it is sufficient that $X_n$ converges in distribution to $X$. The converse is not true.
- ***Theorem 5.2.2 (Condition for convergence in distribution for sum of random variables).*** If we have the following:
	- $X_n$ converges in distribution to $X$
	- $Y$ converges in probability to 0
Then $X_n+Y$ converges in distribution to $X$.

- ***Theorem 5.2.4 (convergence in distribution of transformation of random variables).*** Suppose $X_n$ converges to $X$ in distribution and $g$ is a continuous function on the support of $X$. Then $g(X_n)$ converges to $g(X)$ in distribution.

- ***Theorem 5.2.5 (Slutsky's Theorem).*** Let $X_{}n$, $X$, $A_{n}$, and $B_n$ be random variables and let $a$ and $b$ be constants. If $X_n \xrightarrow{D} X$, $A_n \xrightarrow{P} a$, and $B_n \xrightarrow{P} b$, then the following convergence occurs: $$A_{n}+B_{n}X_{n}\xrightarrow{D}a+bX$$
- ***Theorem 5.2.6 (sufficiency condition for bounded in probability).*** If $X_n \xrightarrow{D} X$, then $X_n$ is bounded in probability
- ***Theorem 5.2.7***. Let $(X_n)$ be a sequence of random variables bounded in probability and let $(Y_n)$ be a sequence of random variables that converges to 0 in probability. Then we have the following: $$X_{n}Y_{n}\xrightarrow{P} 0$$
- ***Theorem 5.2.8***. Suppose $(Y_n)$ is a sequence of random variables that is bounded in probability. Suppose $X_n = o_p(Y_n)$. Then $X_n \xrightarrow{P} 0$, as $n → ∞$.
- ***Theorem 5.2.9 (Sufficiency for convergence in distribution to the normal distribution).*** If we have $\sqrt{n}(X_n-\theta) \xrightarrow{D}N(0,\sigma^2)$. Then given a function $g(x)$ that is differentiable at $\theta$ with $g'(\theta)\ne 0$ then we have the following convergence in distribution for a transformation of $g(X_{n})$: $$\sqrt{n}(g(X_n))-g(\theta)) \xrightarrow{D} N(0,\sigma^2(g'(\theta))^2)$$
- Theorem 5.2.10. Let $(Xn)$ be a sequence of random variables with mgf $M_{X_n}(t)$ that exists for $−h<t<h$  for all $n$. Let $X$ be a random variable with mgf $M(t$),which exists for $|t| ≤ h_{1} ≤ h$. If  $\lim\limits_{ n \to \infty }M_{X_{n}}(t)$ for $|t| ≤ h_{1}$, then $X_n\xrightarrow{D} X$.
- 
