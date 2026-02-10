---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - math
  - statistics
  - robert_hogg
---



The conditional probability of an event $B$ given $A$ occurred is represented as follows:
$$P(B|A) = P(A \cap B|A)$$
This can be interpreted as $A$ which was a subset of the original sample space now being the new sample space to compute the probability of $B$ . 

***Definition 1.4.1*** Let $B$ and $A$ be events with P(A)>0. Then we define the conditional probability of $B$ given $A$ as:
$$ P(B|A)=\frac{P(A\cap B)}{P(A)}$$
The frequentist interpretation of conditional probability can be seen from the "multiplication" rule of probabilities $P(B|A)P(A)=P(A\cap B)$.

It is possible for us to describe the probability of an event in terms of the conditional probabilities. In general, given any sample space that is partitioned by $k$ events $A_1, A_2, A_3,...,A_k$, then we can see that any event $B$ can be described as:
$$B = B \cap (A_1 \cup A_2 \cup A_3 \cup ... \cup A_k)$$
$$B = (B \cap A_1) \cup (B \cap A_2) \cup (B \cap A_3) \cup... \cup (B \cap A_k)$$
As each $(B \cap A_i)$ is mutually exclusive with each other, we then have for the probability of B the sum of every $P(B \cap A_i) = P(A_i)P(B|A_i)$ which is referred to as the <u>law of total probability</u>:
$$P(B) = \sum_{i=1}^{k} P(A_i)P(B|A_i)$$The law of total probability leads to the following important theorem which lets us relate conditional probabilities that are the "reverse" of each other namely it lets us relate This theorem relates $P(B|A)$ to $P(A|B)$
***Theorem 1.4.1 (Bayes' Theorem)*** . Let $A_1,...A_k$ be events with $P(A_i)>0$, for $i = 1,2,..k$ and that they form a partition of the sample space. For any event B then:
$$P(A_j|B) = \frac{P(B|A_j)P(A_j)}{P(B)}=\frac{P(B|A_j)P(A_j)}{\sum_{i=1}^{k}P(A_i)P(B|A_{i})}$$The proof of this is derived from the definition of conditional probabilities and then applying the law of total probabilities to determine $P(B)$. This is a useful relation for us when we need to determine a conditional probability but the "reversed" conditional probability is easier to solve

### 1.4.1 Independence

***Definition 1.4.2***. Let $A,  B$ be two events. $A$ and $B$ are independent of each other if $P(A \cap B) = P(A)P(B)$ . 

It follows from the definition of independence given two mutually independent events $A$ and $B$ that the conditional probabilities are $P(B|A)=P(B)$  and $P(A|B) = P(A)$


Often times using the term "independent" means that two events are "mutually independent" of each other. Sometimes $A$ may be independent of $B$ but $B$ may depend on $A$.
