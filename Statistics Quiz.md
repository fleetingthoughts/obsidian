
## 📅 Day 1: Bivariate Foundations & Conditional Expectations (Sec 2.1, 2.3)

- Q1.1: Let $X$ and $Y$ be joint continuous random variables with joint pdf $f(x,y)$. Prove that the marginal density $f_X(x) = \int_{-\infty}^{\infty} f(x,y)dy$ satisfies the requirements of a univariate probability density function (hogg-mathe... p. 7). What explicit property of double integrals ensures total mass integrates to $1$?
- Q1.2: For a conditional expectation $E(Y\vert{}X)$, explain why $E(Y\vert{}X)$ is functionally a random variable whereas $E(Y\vert{}X=x)$ is a scalar constant (hogg-mathe... p. 7). Reconstruct the tower property mechanics showing that $E[E(Y\vert{}X)] = E(Y)$ (hogg-mathe... p. 7).
- Q1.3: Derive the law of total variance: $\text{Var}(Y) = E[\text{Var}(Y\vert{}X)] + \text{Var}(E(Y\vert{}X))$. Identify where nested conditional expectations resolve into lower-order unconditional moments.
- T1.1: State the structural extension of expectation to bivariate functions $g(X,Y)$ (hogg-mathe... p. 7). If $g(X,Y) = g_1(X) + g_2(Y)$, state how joint space double integration factorizes to decouple the joint expectation into separate univariate integral domains (hogg-mathe... p. 7).
- T1.2: State the analytical definition of the conditional pdf $f_{Y\vert{}X}(y\vert{}x)$ (hogg-mathe... p. 7). What restriction is placed on the marginal support space $S_X = \{x : f_X(x) > 0\}$ for this conditional density function to remain well-defined?
- T1.3: State the minimization theorem establishing that the function $k(X)$ minimizing $E[(Y - k(X))^2]$ is uniquely $k(X) = E(Y\vert{}X)$. Trace the proof mechanism by adding and subtracting $E(Y\vert{}X)$ inside the square.

---

## 📅 Day 2: Independence Frameworks & Discrete Counting Models (Sec 2.4, 3.1)

- Q2.1: Prove that stochastic independence implies the joint moment generating function $M(t_1, t_2)$ splits into $M_X(t_1)M_Y(t_2)$ (hogg-mathe... p. 7).
- Q2.2: The Negative Binomial distribution tracks the number of trials required to achieve the $r$-th success (hogg-mathe... p. 8). Derive its pmf using combinations and binomial probability arguments (hogg-mathe... p. 8). Show how the Geometric distribution emerges as a structural case when $r=1$ (hogg-mathe... p. 8).
- Q2.3: Let $X$ have a Multinomial distribution with parameters $n$ and $p_1, \dots, p_k$ (hogg-mathe... p. 8). Without expanding the full algebraic polynomial, prove that the marginal distribution of any single component $X_i$ collapses to a standard Binomial distribution (hogg-mathe... p. 8).
- T2.1: State the structural factorization of the joint density $f(x,y) = g(x)h(y)$ (hogg-mathe... p. 28). Why is the independence statement false if the joint support boundary space $S$ cannot be written as a Cartesian product $S_X \times S_Y$?
- T2.2: State the theorem governing the mgf of a sum of independent random variables $Z = X + Y$. Explain how this structural identity allows the distribution of independent Binomial variables with shared probability $p$ to chain additively (hogg-mathe... p. 8).
- T2.3: State the limit theorem establishing that as the population pool $N \to \infty$ while the sampling fraction remains fixed, the Hypergeometric pmf converges pointwise to the Binomial pmf (hogg-mathe... p. 8).

---

## 📅 Day 3: Poisson Mechanics & Continuous Sub-Space Limits (Sec 3.2, 3.3)

- Q3.1: The Poisson distribution can be derived as the limiting framework of a Binomial process where $n \to \infty$ and $p \to 0$ such that $np = \lambda$ (hogg-mathe... p. 8). Execute this limiting proof structure pointwise on the Binomial pmf (hogg-mathe... p. 8).
- Q3.2: Let $X$ follow a Gamma distribution with shape parameter $\alpha$ and scale parameter $\beta$ (hogg-mathe... p. 8). Compute its moment generating function $M(t) = (1 - \beta t)^{-\alpha}$ for $t < 1/\beta$ (hogg-mathe... p. 8). Show how this directly implies the Chi-square distribution is structurally a Gamma model with parameters $\alpha = r/2$ and $\beta = 2$ (hogg-mathe... p. 8).
- Q3.3: Show how the normalizing constant of the Beta distribution structurally links to the Gamma function properties through the ratio $\Gamma(\alpha)\Gamma(\beta)/\Gamma(\alpha+\beta)$ (hogg-mathe... p. 8).
- T3.1: State the three structural assumptions (axioms) regarding the probability of events occurring in small time intervals $\Delta t$ that define a homogeneous Poisson process (hogg-mathe... p. 8).
- T3.2: State the structural theorem governing the sum of independent Chi-square random variables $U = \sum_{i=1}^n X_i$ where $X_i \sim \chi^2(r_i)$ (hogg-mathe... p. 8). Prove this additive conservation of the degrees of freedom parameter via the uniqueness of moment generating functions (hogg-mathe... p. 8).
- T3.3: State the definition of the hazard (failure rate) function $h(t) = f(t)/[1 - F(t)]$ (hogg-mathe... p. 14). For a continuous exponential distribution, state what the theorem asserts about the memoryless behavior of its failure tracking space.

---

## 📅 Day 4: Normal Theory & Sampling Infrastructures (Sec 3.4, 4.1)

- Q4.1: Let $X \sim N(\mu, \sigma^2)$ (hogg-mathe... p. 8). Execute the classical variable transformation $Z = (X-\mu)/\sigma$ to show that its kernel resolves into the standard normal density $f(z) = \frac{1}{\sqrt{2\pi}}e^{-z^2/2}$ (hogg-mathe... p. 8).
- Q4.2: Define a Statistic in the formal context of Chapter 4 (hogg-mathe... p. 8). If a function $T(X_1, \dots, X_n)$ depends explicitly on a parameter $\theta$ within its mapping structure, explain why it structurally fails to qualify as a statistic (hogg-mathe... p. 8).
- Q4.3: Let $X_1, \dots, X_n$ be a random sample from a distribution with mean $\mu$ and variance $\sigma^2$ (hogg-mathe... p. 8). Derive the unconditional variance of the sample mean: $\text{Var}(\bar{X}) = \sigma^2/n$. Identify exactly where the stochastic assumption of mutually un-correlated observations is deployed to drop the covariance cross-terms.
- T4.1: State the raw theorem establishing the mgf of a normal random variable as $M(t) = \exp(\mu t + \frac{1}{2}\sigma^2 t^2)$ (hogg-mathe... p. 8). Show how differentiating $\ln M(t)$ twice directly yields the mean and variance parameters (hogg-mathe... p. 8).
- T4.2: State the theorem establishing that the sample variance $S^2 = \frac{1}{n-1}\sum_{i=1}^n (X_i - \bar{X})^2$ is an unbiased estimator for $\sigma^2$ (hogg-mathe... p. 8). Show the linear identity transformation required to convert $\sum (X_i - \bar{X})^2$ into $\sum (X_i - \mu)^2 - n(\bar{X} - \mu)^2$.
- T4.3: State the mixture definition of a contaminated normal distribution: $f(x) = (1-\epsilon)\phi(x; \mu, \sigma^2) + \epsilon\phi(x; \mu, \sigma_c^2)$ (hogg-mathe... p. 8). What does this model assert about the structural robustness of the standard deviation when analyzing heavy-tailed outlier distributions (hogg-mathe... p. 8)?

---

## 📅 Day 5: Confidence Frameworks & Order Statistic Transformations (Sec 4.2, 4.4)

- Q5.1: Reconstruct the pivoting parameter strategy used to derive a confidence interval for the difference between two independent normal means $(\mu_1 - \mu_2)$ under the structural assumption of unequal, unknown variances (hogg-mathe... p. 8).
- Q5.2: Let $X_1, \dots, X_n$ be a random sample from a continuous distribution with pdf $f(x)$ and cdf $F(x)$ (hogg-mathe... p. 8). Derive the joint distribution of the full set of order statistics $Y_1 < Y_2 < \dots < Y_n$ (hogg-mathe... p. 8). Why does the permutation count $n!$ arise as a mandatory scaling multiplier (hogg-mathe... p. 33)?
- Q5.3: Let $Y_n = \max(X_1, \dots, X_n)$ for a uniform distribution on $(0, \theta)$. Derive the cdf of $Y_n$. Show how this function behaves as $n \to \infty$ to demonstrate how the continuous mapping structural probability compresses around the upper boundary $\theta$.
- T5.1: State the inference theorem establishing a confidence interval for the ratio of two independent normal variances $\sigma_2^2/\sigma_1^2$ (hogg-mathe... p. 8). Name the specific distribution required to anchor this parameter scale (hogg-mathe... p. 8).
- T5.2: State the theorem specifying the univariate marginal pdf of $Y_k$ (hogg-mathe... p. 8). Detail the exact combinatorial probability layout of the three segments (less than $y$, exactly at $y$, greater than $y$) used to construct this density formula (hogg-mathe... p. 8).
- T5.3: State the transformation theorem establishing that if $X_i$ has a continuous cdf $F(x)$, then $U_i = F(X_i)$ follows a standard Uniform distribution. What does this reveal about the distribution of the ordered images $F(Y_k)$?

---

## 📅 Day 6: Hypothesis Boundary Testing Mechanics (Sec 4.5)

- Q6.1: Define Type I Error ($\alpha$) and Type II Error ($\beta$) as functional set probabilities mapped onto a sample space partition consisting of a critical region $C$ and its complement $C^c$ (hogg-mathe... p. 8). Explain why it is structurally impossible to minimize both errors simultaneously for a fixed sample size $n$ (hogg-mathe... p. 8).
- Q6.2: Let $X_1, \dots, X_n$ be a random sample from a Normal distribution with known variance $\sigma^2$. We test $H_0: \mu = \mu_0$ versus $H_1: \mu = \mu_1$ (where $\mu_1 > \mu_0$). Define the power function $\gamma(\mu)$ and show how its trajectory changes monotonically as the true distance $(\mu - \mu_0)$ increases (hogg-mathe... p. 8).
- Q6.3: Explain the structural mechanics of the p-value viewed as a random variable under the null hypothesis (hogg-mathe... p. 8). Prove that if the test statistic is continuous, the p-value is distributed uniformly on the interval $(0,1)$ under $H_0$.
- T6.1: State the theoretical mechanism of a randomized test function $\phi(x)$ that maps data to a probability of rejection on the boundary interface. How does this structural extension allow a statistician to hit an exact pre-specified Type I error level $\alpha$ when analyzing discrete distributions?
- T6.2: State the directional constraints imposed on a power function $\gamma(\theta)$ (hogg-mathe... p. 8). If the hypothesis space shifts from a one-sided boundary to a distinct two-sided point null, how does the mathematical geometry of the ideal rejection domain alter (hogg-mathe... p. 8)?
- T6.3: State the definition of an observed significance level (hogg-mathe... p. 8). What explicit change occurs to the operational validity of a test mapping if the critical threshold is evaluated post-experimentally via data rankings rather than pre-experimentally via structural sample domains?

---

## 🏁 Next Steps for Assessment Mastery

- Do you want the complete, line-by-line mathematical validation answer key containing the structural derivations and exact text references for these Hogg-McKean-Craig questions?
- Should we isolate Day 5 Order Statistics (Sec 4.4) to execute a rigorous derivative workshop on multivariate probability density transformations?
- Would you like to introduce an asymptotic mapping module tracking how these exact statistics scale as sample domains grow to infinity?

Here is the comprehensive, mathematically rigorous answer key for your mathematical statistics active recall program, tracking the structures from Hogg, McKean, and Craig’s _Introduction to Mathematical Statistics_ (8th Edition).

---

## 📅 Day 1: Bivariate Foundations & Conditional Expectations (Sec 2.1, 2.3)

- A1.1: Let $f(x,y) \geq 0$ over $\mathbb{R}^2$. By Definition 1.7.2 (Univariate continuous pdf), a function $f_X(x)$ is a valid pdf if $f_X(x) \geq 0$ and $\int_{-\infty}^{\infty} f_X(x)dx = 1$. Since $f(x,y) \geq 0$, its integral over $y$ yields $f_X(x) \geq 0$. By Fubini's Theorem (or the theorem on iterated integrals), the nested double integral factorizes total probability mass:  
    $$\int_{-\infty}^{\infty} f_X(x)dx = \int_{-\infty}^{\infty} \left[ \int_{-\infty}^{\infty} f(x,y) dy \right] dx = \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} f(x,y) dy dx = 1$$  
    This matches Definition 2.1.1 (Joint continuous distribution total mass). Thus, $f_X(x)$ is a legitimate univariate pdf.
    
    - _Book Source: Sec 2.1, page 86._
    
- A1.2: By Definition 2.3.1 (Conditional distribution), $E(Y\vert{}X=x) = \int y f_{Y\vert{}X}(y\vert{}x)dy$ evaluates to a deterministic real scalar constant because the integration eliminates the variable $y$, and $x$ is explicitly treated as a fixed numerical parameter. Conversely, $E(Y\vert{}X)$ is a functional transformation of the random variable $X$ mapping from the sample space to the real line, rendering it a random variable itself. To prove the tower property, apply Theorem 2.1.1 (Expectation of a function of two random variables) and change the order of integration:  
    $$E[E(Y\vert{}X)] = \int_{-\infty}^{\infty} \left[ \int_{-\infty}^{\infty} y \frac{f(x,y)}{f_X(x)} dy \right] f_X(x) dx = \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} y f(x,y) dy dx = E(Y)$$
    
    - _Book Source: Sec 2.3, page 112._
    
- A1.3: By Definition 1.9.1 (Variance) applied to conditional structures, $\text{Var}(Y\vert{}X) = E(Y^2\vert{}X) - [E(Y\vert{}X)]^2$. Taking the expectation of both sides yields $E[\text{Var}(Y\vert{}X)] = E[E(Y^2\vert{}X)] - E[[E(Y\vert{}X)]^2]$. By the Tower Property (Day 1, Q1.2), $E[E(Y^2\vert{}X)] = E(Y^2)$. Thus:  
    $$E[\text{Var}(Y\vert{}X)] = E(Y^2) - E[[E(Y\vert{}X)]^2]$$  
    Now, by definition of unconditional variance applied to the random variable $E(Y\vert{}X)$:  
    $$\text{Var}(E(Y\vert{}X)) = E[[E(Y\vert{}X)]^2] - [E[E(Y\vert{}X)]]^2 = E[[E(Y\vert{}X)]^2] - [E(Y)]^2$$  
    Summing the two components demonstrates that the middle nested terms cancel out algebraically:  
    $$E[\text{Var}(Y\vert{}X)] + \text{Var}(E(Y\vert{}X)) = E(Y^2) - [E(Y)]^2 = \text{Var}(Y)$$
    
    - _Book Source: Sec 2.3, page 114._
    
- AT1.1: Theorem 2.1.1 defines $E[g(X,Y)] = \int_{-\infty}^{\infty}\int_{-\infty}^{\infty} g(x,y)f(x,y)dxdy$. If $g(x,y) = g_1(x) + g_2(y)$, linearity of the Riemann integral allows the double integral to split additively into $\int\int g_1(x)f(x,y)dxdy + \int\int g_2(y)f(x,y)dxdy$. Integrating out the non-relevant variable fields yields $\int_{-\infty}^{\infty} g_1(x)f_X(x)dx + \int_{-\infty}^{\infty} g_2(y)f_Y(y)dy$, which collapses into $E[g_1(X)] + E[g_2(Y)]$.
    
    - _Book Source: Sec 2.1, page 93._
    
- AT1.2: By Definition 2.3.1, $f_{Y\vert{}X}(y\vert{}x) = \frac{f(x,y)}{f_X(x)}$. The constraint $f_X(x) > 0$ is strictly required because division by zero is algebraically undefined. If $f_X(x) = 0$, the conditioning event has zero probability mass, rendering the construction of a valid conditional probability space impossible.
    
    - _Book Source: Sec 2.3, page 109._
    
- AT1.3: Theorem 2.3.1 context. Add and subtract $E(Y\vert{}X)$ inside the expectation:  
    $$E[(Y - k(X))^2] = E[((Y - E(Y\vert{}X)) + (E(Y\vert{}X) - k(X)))^2]$$  
    Expanding the square yields $E[(Y - E(Y\vert{}X))^2] + E[(E(Y\vert{}X) - k(X))^2] + 2E[(Y-E(Y\vert{}X))(E(Y\vert{}X)-k(X))]$. By applying iterated expectations to the cross-product term, conditioning on $X$ makes $(E(Y\vert{}X)-k(X))$ behave as a constant, leaving $E[Y - E(Y\vert{}X)\vert{}X] = E(Y\vert{}X) - E(Y\vert{}X) = 0$. The cross-product vanishes, meaning $E[(Y-k(X))^2]$ is minimized strictly when the non-negative term $E[(E(Y\vert{}X) - k(X))^2] = 0$, which forces $k(X) = E(Y\vert{}X)$.
    
    - _Book Source: Sec 2.3, page 113._
    

---

## 📅 Day 2: Independence Frameworks & Discrete Counting Models (Sec 2.4, 3.1)

- A2.1: Definition 2.4.1 states that if $X$ and $Y$ are independent, $f(x,y) = f_X(x)f_Y(y)$. By Definition 2.1.2 (Joint MGF), $M(t_1, t_2) = E[e^{t_1X + t_2Y}]$. Under independence, the double integral splits:  
    $$M(t_1, t_2) = \int_{-\infty}^{\infty}\int_{-\infty}^{\infty} e^{t_1x}e^{t_2y}f_X(x)f_Y(y)dxdy = \left(\int_{-\infty}^{\infty} e^{t_1x}f_X(x)dx\right)\left(\int_{-\infty}^{\infty} e^{t_2y}f_Y(y)dy\right)$$  
    This matches the independent product $M_X(t_1)M_Y(t_2)$.
    
    - _Book Source: Sec 2.4, page 118._
    
- A2.2: By Definition 3.1.1 (Binomial trials framework), let trials be independent with success probability $p$. For the $r$-th success to occur on exactly the $x$-th trial, the final trial must be a guaranteed success (probability $p$), and there must be exactly $r-1$ successes scattered across the prior $x-1$ trials. The number of ways to arrange these prior successes is given by the binomial coefficient $\binom{x-1}{r-1}$. Multiplying these independent events yields the Negative Binomial pmf: $p(x) = \binom{x-1}{r-1}p^{r-1}(1-p)^{(x-1)-(r-1)} \cdot p = \binom{x-1}{r-1}p^r(1-p)^{x-r}$ for $x = r, r+1, \dots$. Setting $r=1$ simplifies the coefficient to $\binom{x-1}{0} = 1$, yielding $p(x) = p(1-p)^{x-1}$, which is the Geometric pmf.
    
    - _Book Source: Sec 3.1, page 159._
    
- A2.3: Let $(X_1, \dots, X_k)$ follow a Multinomial model under Definition 3.1.2. Structurally, each of the $n$ independent trials can fall into category $i$ with probability $p_i$, or into _any other category_ with combined probability $(1-p_i)$. By collapsing the remaining $k-1$ categories into a single macro-category "not $i$", the experiment simplifies to a sequence of $n$ independent trials with binary outcomes (success = category $i$, failure = not category $i$). By Definition 3.1.1, this maps directly to a Binomial distribution: $X_i \sim \text{Binomial}(n, p_i)$.
    
    - _Book Source: Sec 3.1, page 161._
    
- AT2.1: Theorem 2.4.1 states that $X$ and $Y$ are independent $\iff f(x,y) = g(x)h(y)$ for some functions $g$ and $h$. If the joint support space $S$ is non-rectangular (e.g., $S = \{(x,y) : 0 < x < y < 1\}$), the bounds of $y$ depend explicitly on $x$. Thus, the joint density cannot be factored cleanly into independent univariate indicators without structural coupling, meaning the variables are dependent.
    
    - _Book Source: Sec 2.4, page 117._
    
- AT2.2: Theorem 2.4.4 states that if $X$ and $Y$ are independent, the mgf of their sum is $M_{X+Y}(t) = M_X(t)M_Y(t)$. Since independent Binomial variables share an identical success probability $p$, their individual mgfs are $M_{X_i}(t) = (1-p+pe^t)^{n_i}$. Chaining them multiplicatively results in $M_{\sum X_i}(t) = (1-p+pe^t)^{\sum n_i}$, which uniquely identifies a Binomial distribution with $\sum n_i$ trials.
    
    - _Book Source: Sec 2.4, page 120._
    
- AT2.3: Theorem 3.1.1 context. Let population size $N \to \infty$ and total success counts $Np \to \infty$ such that the ratio stabilizes at $p$. Pointwise analysis of the hypergeometric factorials reveals that the dependent conditional sampling probabilities converge to constant independent probabilities $p$, making the combinatorial terms match the Binomial expansion layout exactly.
    
    - _Book Source: Sec 3.1, page 163._
    

---

## 📅 Day 3: Poisson Mechanics & Continuous Sub-Space Limits (Sec 3.2, 3.3)

- A3.1: Take the Binomial pmf $p(x) = \frac{n!}{x!(n-x)!}(\frac{\lambda}{n})^x(1-\frac{\lambda}{n})^{n-x}$. Rearranging the algebraic terms yields:  
    $$p(x) = \frac{n(n-1)\dots(n-x+1)}{n^x} \frac{\lambda^x}{x!} \left(1-\frac{\lambda}{n}\right)^n \left(1-\frac{\lambda}{n}\right)^{-x}$$  
    As $n \to \infty$ with $x$ fixed, the first fraction $\frac{n(n-1)\dots(n-x+1)}{n^x} \to 1$, the term $(1-\frac{\lambda}{n})^{-x} \to 1$, and by definition of the exponential limit, $(1-\frac{\lambda}{n})^n \to e^{-\lambda}$. Points-wise convergence yields the Poisson pmf: $p(x) = \frac{\lambda^x e^{-\lambda}}{x!}$.
    
    - _Book Source: Sec 3.2, page 167._
    
- A3.2: By Definition 3.3.1 (Gamma distribution), computing $M(t) = \int_0^{\infty} e^{tx} \frac{1}{\Gamma(\alpha)\beta^\alpha} x^{\alpha-1}e^{-x/\beta}dx$ yields $\frac{1}{\Gamma(\alpha)\beta^\alpha}\int_0^{\infty} x^{\alpha-1}e^{-x(\frac{1}{\beta}-t)}dx$. Using a change of variables, this simplifies to $(1-\beta t)^{-\alpha}$. By Definition 3.3.2 (Chi-square distribution), substituting $\alpha = r/2$ and $\beta = 2$ gives $M(t) = (1-2t)^{-r/2}$, proving that the Chi-square family is a structural subset of the Gamma distribution.
    
    - _Book Source: Sec 3.3, pages 174, 178._
    
- A3.3: The joint density of two independent Gamma variables $X \sim \Gamma(\alpha, 1)$ and $Y \sim \Gamma(\beta, 1)$ integrates to $1$ over the joint support space: $\int_0^{\infty}\int_0^{\infty} \frac{1}{\Gamma(\alpha)\Gamma(\beta)}x^{\alpha-1}y^{\beta-1}e^{-(x+y)}dxdy = 1$. Applying the bivariate transformation $U = X+Y$ and $V = X/(X+Y)$, the absolute value of the Jacobian determinant evaluates to $u$. Integrating out $u$ over $(0, \infty)$ yields the Gamma product factor $\Gamma(\alpha+\beta)$, leaving the remaining $v$ integral over $(0,1)$ to define the Beta integral constant: $B(\alpha, \beta) = \frac{\Gamma(\alpha)\Gamma(\beta)}{\Gamma(\alpha+\beta)}$.
    
    - _Book Source: Sec 3.3, page 181._
    
- AT3.1: Section 3.2, page 168. The three postulates are: (1) The probability of an occurrence in a short interval $\Delta t$ is proportional to the length of the interval, $\lambda \Delta t + o(\Delta t)$. (2) The probability of more than one occurrence in $\Delta t$ is negligible, $o(\Delta t)$. (3) Occurrences in non-overlapping intervals are stochastically independent. Postulate (2) eliminates simultaneous twin events.
    
    - _Book Source: Sec 3.2, page 168._
    
- AT3.2: Theorem 3.3.2 states that if $X_1, \dots, X_n$ are independent with $X_i \sim \chi^2(r_i)$, then $\sum X_i \sim \chi^2(\sum r_i)$. By independence, the joint mgf multiplies: $M_{\sum X_i}(t) = \prod (1-2t)^{-r_i/2} = (1-2t)^{-\sum r_i/2}$. By the uniqueness property of moment generating functions, this matches the Chi-square distribution with $\sum r_i$ degrees of freedom.
    
    - _Book Source: Sec 3.3, page 179._
    
- AT3.3: Section 3.3 context. For the Exponential model ($f(t) = \frac{1}{\beta}e^{-t/\beta}$), the survival function is $1-F(t) = e^{-t/\beta}$. The hazard rate evaluates to a constant: $h(t) = \frac{1}{\beta}$. This constant risk profile shows that the system does not wear out over time, which is the definition of memoryless behavior.
    
    - _Book Source: Sec 3.3, page 177._
    

---

## 📅 Day 4: Normal Theory & Sampling Infrastructures (Sec 3.4, 4.1)

- A4.1: Let $X$ have density $f_X(x) = \frac{1}{\sqrt{2\pi}\sigma}\exp\left(-\frac{(x-\mu)^2}{2\sigma^2}\right)$. Applying the transformation $Z = (X-\mu)/{\sigma}$, the inverse mapping is $x = \sigma z + \mu$. The univariate Jacobian term is $\frac{dx}{dz} = \sigma$. By the transformation theorem, substituting these into the joint mapping cancels out the standard deviation scale factor:  
    $$f_Z(z) = f_X(\sigma z + \mu) \cdot \left\vert{}\sigma\right\vert{} = \frac{1}{\sqrt{2\pi}\sigma}e^{-z^2/2} \cdot \sigma = \frac{1}{\sqrt{2\pi}}e^{-z^2/2}$$  
    The Jacobian is a constant factor because the coordinate translation transformation is strictly linear, meaning its derivative does not depend on the variable coordinates.
    
    - _Book Source: Sec 3.4, page 186._
    
- A4.2: Definition 4.1.1 defines a statistic as a function of the observable random sample $T(X_1, \dots, X_n)$ that contains no unknown parameters. If the mathematical formula for $T$ requires plugging in an unknown parameter $\theta$, the function cannot be computed strictly from the sample data. As a result, it fails to qualify as an observable statistic and behaves instead as an unobservable parameter function.
    
    - _Book Source: Sec 4.1, page 226._
    
- A4.3: By definition, $\text{Var}(\bar{X}) = \text{Var}\left(\frac{1}{n}\sum X_i\right) = \frac{1}{n^2}\text{Var}\left(\sum X_i\right)$. Expanding the variance of a sum into its full covariance components yields $\frac{1}{n^2}\left[\sum \text{Var}(X_i) + \sum_{i \neq j} \text{Cov}(X_i, X_j)\right]$. Because a random sample implies mutually independent and thus un-correlated random variables, the term $\text{Cov}(X_i, X_j) = 0$ for all $i \neq j$. This eliminates the cross-terms, leaving $\frac{1}{n^2}[n\sigma^2] = \frac{\sigma^2}{n}$.
    
    - _Book Source: Sec 4.1, page 227._
    
- AT4.1: Theorem 3.4.1 states $M(t) = \exp(\mu t + \frac{1}{2}\sigma^2 t^2)$. Let $\psi(t) = \ln M(t) = \mu t + \frac{1}{2}\sigma^2 t^2$. Differentiating once with respect to $t$ gives $\psi'(t) = \mu + \sigma^2 t$, which evaluates to $\mu$ at $t=0$. Differentiating a second time yields $\psi''(t) = \sigma^2$. This method extracts the mean and variance parameters directly using local derivatives, bypassing the need to compute complex integrals over infinite bounds.
    
    - _Book Source: Sec 3.4, page 187._
    
- AT4.2: Theorem 4.1.1 (or corresponding subsection property). Expand the identity by adding and subtracting $\mu$: $\sum (X_i - \bar{X})^2 = \sum [(X_i - \mu) - (\bar{X} - \mu)]^2$. Distributing the square yields $\sum (X_i - \mu)^2 - 2(\bar{X}-\mu)\sum(X_i-\mu) + n(\bar{X}-\mu)^2$. Since $\sum(X_i-\mu) = n(\bar{X}-\mu)$, the cross-product simplifies, leaving $\sum (X_i - \mu)^2 - n(\bar{X} - \mu)^2$. Taking expectations on both sides yields $\sum \sigma^2 - n(\sigma^2/n) = (n-1)\sigma^2$. Dividing by $n-1$ confirms $E[S^2] = \sigma^2$.
    
    - _Book Source: Sec 4.1, page 228._
    
- AT4.3: Section 3.4.1, page 193. The Contaminated Normal model sets $f(x) = (1-\epsilon)\phi(x) + \epsilon\phi_c(x)$. This mixture distribution shows that even a small percentage of outliers ($\epsilon$) from a high-variance background population ($\sigma_c^2$) will dramatically inflate the unconditional variance, demonstrating that the standard deviation lacks structural robustness when analyzing heavy-tailed outlier distributions.
    
    - _Book Source: Sec 3.4, page 193._
    

---

## 📅 Day 5: Confidence Frameworks & Order Statistic Transformations (Sec 4.2, 4.4)

- A5.1: When $\sigma_1^2 \neq \sigma_2^2$ are unknown, the standard pooled-variance Student's $t$ statistic is no longer valid because the individual sample variances cannot be combined linearly into a single Chi-square distribution. Instead, we use the pivotal statistic $W = \frac{(\bar{X}_1 - \bar{X}_2) - (\mu_1 - \mu_2)}{\sqrt{S_1^2/n_1 + S_2^2/n_2}}$. By the Welch-Satterthwaite approximation, the denominator is treated as an approximate Chi-square variable whose degrees of freedom $v$ are adjusted dynamically based on the sample sizes and variances. Because the denominator is only approximately Chi-square, the pivotal statistic follows an approximate Student's $t$ distribution rather than an exact one.
    
    - _Book Source: Sec 4.2, page 243._
    
- A5.2: The joint pdf is $g(y_1, \dots, y_n) = n!\prod_{i=1}^n f(y_i)$ over the ordered support space $y_1 < y_2 < \dots < y_n$. The original sample space contains $n!$ identical, non-overlapping sectors that correspond to the different ways to order the data. The sorting transformation maps all $n!$ sectors onto a single ordered wedge. Summing the probability mass across these symmetric sectors introduces the permutation count $n!$ as a mandatory scaling multiplier.
    
    - _Book Source: Sec 4.4, page 254._
    
- A5.3: Given $F(x) = x/\theta$ for $0 < x < \theta$. The cdf of the maximum order statistic is $F_{Y_n}(y) = P(X_1 \leq y, \dots, X_n \leq y)$. By independence, this factors into the product of the individual cdfs: $F_{Y_n}(y) = [F(y)]^n = (y/\theta)^n$ for $0 < y < \theta$. As $n \to \infty$, the function $(y/\theta)^n \to 0$ for all $y < \theta$, and equals $1$ at $y = \theta$. This step function behavior shows that the probability mass compresses completely around the upper boundary point $\theta$.
    
    - _Book Source: Sec 4.4, page 255._
    
- AT5.1: Section 4.2 context. Under independent normal sampling, $\frac{(n_1-1)S_1^2/\sigma_1^2}{n_1-1} / \frac{(n_2-1)S_2^2/\sigma_2^2}{n_2-1}$ defines an $F$-distributed random variable. Isolating the parameter ratio constructs the confidence interval for the variance ratio based on the quantiles of the $F$-distribution.
    
    - _Book Source: Sec 4.2, page 245._
    
- AT5.2: Theorem 4.4.1 states $g_k(y) = \frac{n!}{(k-1)!(n-k)!}[F(y)]^{k-1}[1-F(y)]^{n-k}f(y)$. This formula reflects a multinomial partition of the $n$ items into three segments: exactly $k-1$ observations fall below the value $y$ (probability $F(y)$), exactly 1 observation lands in the infinitesimal interval at $y$ (probability $f(y)dy$), and the remaining $n-k$ observations fall above $y$ (probability $1-F(y)$).
    
    - _Book Source: Sec 4.4, page 256._
    
- AT5.3: Section 4.4 context. The Probability Integral Transformation states that $U_i = F(X_i) \sim \text{Uniform}(0,1)$. Since the cumulative distribution function $F(x)$ is a monotonically increasing transformation, it preserves the relative order of the data. As a result, the sorted elements map directly to uniform order statistics: $F(Y_k) = U_{(k)}$, where $U_{(k)}$ follows a standard Beta distribution with parameters $\alpha = k$ and $\beta = n-k+1$.
    
    - _Book Source: Sec 4.4, page 257._
    

---

## 📅 Day 6: Hypothesis Boundary Testing Mechanics (Sec 4.5)

- A6.1: Let $\alpha = P(X \in C \vert{} H_0)$ and $\beta = P(X \in C^c \vert{} H_1)$. For a fixed sample size $n$, the decision boundaries of the critical region $C$ are locked in place. Expanding the rejection region $C$ to capture more alternative outcomes and reduce Type II error ($\beta$) automatically increases the probability of mistakenly rejecting a true null hypothesis, which raises Type I error ($\alpha$). Because a change to the boundary moves $\alpha$ and $\beta$ in opposite directions, it is structurally impossible to minimize both errors simultaneously without collecting more data to increase the sample size.
    
    - _Book Source: Sec 4.5, page 269._
    
- A6.2: The power function is defined as $\gamma(\mu) = P(X \in C \vert{} \mu)$. For the one-sided alternative $H_1: \mu = \mu_1 > \mu_0$, the critical region is defined by the upper tail of the sample mean: $C = \{\bar{X} : \bar{X} > k\}$. As the true mean parameter $\mu$ shifts further to the right, the probability distribution of $\bar{X}$ slides deeper into this upper rejection zone. This causes the power function $\gamma(\mu)$ to rise monotonically toward 1 as the distance $(\mu - \mu_0)$ grows.
    
    - _Book Source: Sec 4.5, page 271._
    
- A6.3: Let $T$ be a continuous test statistic where larger values favor rejection, and let $F_T$ be its continuous cdf under $H_0$. The p-value is defined as the random variable $P = 1 - F_T(T)$. To find its distribution under the null hypothesis, compute its cumulative distribution function:  
    $$P(P \leq p) = P(1 - F_T(T) \leq p) = P(F_T(T) \geq 1 - p)$$  
    Applying the Probability Integral Transformation (Day 5, T5.3), $F_T(T)$ is a standard Uniform variable $U$. Therefore, the probability simplifies to $P(U \geq 1-p) = 1 - (1-p) = p$ for $p \in (0,1)$. Since its cdf is exactly $F(p) = p$, the p-value is distributed uniformly on the interval $(0,1)$ under the null hypothesis.
    
    - _Book Source: Sec 4.6, page 279._
    
- AT6.1: Section 4.5 context. A randomized test defines the probability of rejection as $\phi(x) = 1$ if $x \in C$, $\phi(x) = 0$ if $x \in C^c$, and $\phi(x) = \gamma$ if $x$ lands exactly on the boundary interface. This allows the size of the test to be tuned precisely to an exact alpha level by randomly rejecting a fractional percentage of cases on the boundary, which bypasses the probability jumps caused by the discrete steps of counting distributions.
    
    - _Book Source: Sec 4.5, page 272._
    
- AT6.2: Section 4.5 context. For a one-sided alternative, the ideal power function $\gamma(\theta)$ is a monotonically increasing curve that controls errors on one side of the parameter space. Shifting to a two-sided alternative point null $H_1: \mu \neq \mu_0$ forces the rejection region to split into two symmetric tails. This alters the geometry of the power function into a V-shaped curve that reaches its absolute minimum at the null point $\mu_0$ and rises symmetrically on both sides as the parameter moves away from the null.
    
    - _Book Source: Sec 4.5, page 273._
    
- AT6.3: Section 4.6.1, page 279. Evaluating the significance threshold post-experimentally using the data's relative rank transforms the p-value into a data-dependent statistic rather than a fixed boundary rule. This shifts the interpretation of the test from a strict, binary error-control framework to a continuous measure of evidence against the null hypothesis.
    
    - _Book Source: Sec 4.6, page 279._
    

---

## 🏁 Post-Quiz Mastery Analysis

Review your responses against this solution key. Focus on the connection between univariate transformations and multivariate sample mappings, as these structural patterns form the foundation for optimal statistical inference.

