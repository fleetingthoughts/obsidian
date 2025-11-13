tags:: #math #math_tricks #stephen_abbot #understanding_analysis 

Working on exercises from chapter [2.4 The Monotone Convergence Theorem and a First Look at Infinite Series](2.4%20The%20Monotone%20Convergence%20Theorem%20and%20a%20First%20Look%20at%20Infinite%20Series.md), we furnished a way to determine the limit after establishing the existence of the limit for a recursively defined sequences $(x_n)$ with $$x_{n+1}=f(x_n)$$
Once we establish that the $(x_n)$ sequence converges to a limit $l$, the trick is then to take the limit of the equation $$\lim_{n\to \infty} x_{n+1}= \lim_{n\to \infty}f(x_n)$$
So to determine the limit, the equation we are solving for is then:
$$l =f(l)$$ As an example, the recursive sequence:
$$\{\sqrt2, \sqrt{2+\sqrt2}, \sqrt{2+\sqrt{2+\sqrt2}},\dots\}$$ Is defined recursively by the following with $x_1 = \sqrt2$ :
$$x_{n+1} = \sqrt{2+x_n}$$ After proving by induction that the sequence is increasing and bounded, we can then precisely determine the limit, $l$, by solving:
$$l = \sqrt{2+l}$$What I actually did for the problem was backwards: I determined the limit should be 2 and if it was 2, then 2 was a bound for the increasing sequence.

# Intuitively understanding this result
It seems strange to me that the result essentially makes use of the fact that $$\lim_{n\to \infty} x_{n+1} = \lim_{n\to \infty} x_{n}$$ We're trying to find the limit of one particular sequence but its as if we're comparing two different sequences, and in fact that's what we're doing. We are applying the squeeze theorem to show for a monotonically increasing sequence, then we "squeeze" it between two other sequences that are the original sequence shifted by one term: $$x_{n-1}\lt x_n \lt x_{n+1}$$
This is consistent with our understanding  [the tail of a sequence is all we care about and any operation done to a finite number of terms doesn't matter](2.3%20The%20Algebraic%20and%20Order%20Limit%20Theorems.md).


