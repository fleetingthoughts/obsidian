---
parent:
tags:
  - "#math"
  - "#statistics"
  - "#probability"
date_created: 2026-02-15
---
When looking at the formula for the birthday problem, the probability that at least 1 pair of people have the same birthday out of $n\ge2$ people assuming all 365 birthdates are likely is:
$$P(A)=1-\frac{P^{365}_{n}}{365^n}$$
But why is a permutation chosen? Wouldn't it make sense that we don't care about the order? That is because in our choice of denominator, we had already considered the sample space to be ordered with replacement! In fact we could try to manipulate the sample space so that we don't care for order and use combinations in the numerator, but the elements that then make up the sample space are not equally likely (unordered tuple with 3 of the same elements vs unordered tuple with 2 of the same elements) and it would be too hard to compute.

The takeaway is that you have to be consistent in the choice of sample space and the way you count. Its either all ordered or unordered.

In general, situations that involve independent identical trials are more easily modeled by ordered (i.e. distinguishable trials) so that each element in the sample space is equally likely. For example, the question what is the probability of getting three different numbers when rolling three dice (which IS the birthday problem with 6,3 in place of 365,n) is much easier to do if we imagine the dice as distinguishable (i.e. $6×5×4/6^3$ ) than by enumerating ordered partitions of 3 into 6 pieces and figuring out the relative frequency of each type.