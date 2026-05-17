---
tags:
  - math
  - real_analysis
date_created: 2026-05-17
---
***Theorem 2.3.2 (Convergence of bounded sequences).*** Every convergent sequence is bounded.


By assumption of convergence we can determine a bound for a sequence $(x_n)$ know that it must be contained in the some interval around the limit, $l$, for a sufficient large $n$. Say we take $\epsilon = 1$ so that $x_n$ is contained in $(l-1,l+1)$ . The bound for these infinite terms outside of a finite $N$ number of terms is then by the [reverse triangle inequality.](Reverse%20Triangle%20inequality..md): 
$$|x_{n}|\le |l|+1$$

![](Pasted%20image%2020251028223048.png)

Then we can determine the maximum of the other finite $N$ terms and take the bound $M$ to be the the maximum of the magnitude of the finite terms and the bound of the remaining infinite terms:
$$M = max(|x_{1}|,x_{2}|,\dots |x_{N-1}|,|l|+1)$$

