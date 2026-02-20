---
tags:
  - "#math"
  - "#real_analysis"
  - "#stephen_abbot"
date_created: 2026-02-19
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
Historically, the Cantor set is a mathematical object that laid the foundations for modern topology and so Abbot starts the chapter by giving an intuitive idea of the properties surrounding the Cantor set. These seemingly counterintuitive properties will provide a better understanding of the nature of subsets on the real line and serves as a testing ground and object of comparison for other mathematical ideas. 

The standard cantor set, $C_o$ is constructed with the single closed unit interval $[0,1]$ and removing the open middle third interval thereby splitting the original interval into two forming a new set, $C_1$, that is a union of these two sets. Mathematically, this creation of $C_1$ is denoted as
$$C_1 =C_0 \setminus (\frac{1}{3}, \frac{2}{3}) = [0,\frac{1}{3}] \cup  []\frac{2}{3},1]$$
$C_1$ is then subjected to the same process: its two subintervals divided to form the union of 4 subintervals $C_2$
$$C_2 = ([0,\frac{1}{9}]\cup [\frac{2}{9},\frac{1}{3}]) \cup([\frac{2}{3},\frac{7}{9}] \cup [\frac{8}{9},1])$$
Iterating this process infinitely, we then refer to the Cantor set, $C$, as the intersection of all $C_n$:
$$C= \cap^{\infty}_{n=0}C_{n}$$
It is tempting to think that this set contains nothing, but Abbot provides a moral answer by a figure showing that the endpoints of the subintervals created from every set minus is retained ![](Pasted%20image%2020260220003600.png)
And so $C$ contains at least these endpoints. Now in going over the properties, Abbot shows that there is some logic to show that the Cantor set has 0 length.

But an interesting property is that the Cantor Set is uncountable which Abbot tries to provide a intuitive appeal by providing an example of a function that maps the elements of a Cantor set to a set of sequences.

Another way to understand the Cantor set is by its dimensions. Abbot applies the idea of dimensions by the way it scales (i.e. creates new copies of itself) when its components are scaled by a factor. For instance if we try to scale various objects by 3, a dot doesn't scale, a line scales linearly by 3, a unit square increases in area by a factor of 9 (creates 9 copies of itself), a cube increases in volume by a factor of 27 (creates 27 copies of itself). In this sense, dimension is the power to which a scaling factor is raised by to determine how an object of said dimension would scale:
![](Pasted%20image%2020260220004609.png)

In trying to apply this concept to the Cantor set, we can define the "scaling" of  the Cantor set by a factor of 3 by scaling the length of $C_0$ and then subjecting it to the iterative set minus operation. The original $C_0=[0,1]$ would then become $[0,3]$ and when we set minus this, $C_1 = [0,1] \cup [2,3]$, and we see that we have essentially produced two copies of the original $C_o$. Somehow, by our understanding of dimension, the Cantor set seemingly has a dimension between 0 and 1!

