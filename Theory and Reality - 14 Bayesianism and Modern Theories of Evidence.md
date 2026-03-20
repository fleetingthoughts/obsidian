---
tags:
  - science
  - philosophy
  - peter_godfrey_smith
date_created: 2026-03-20
parent: "[[Theory and Reality - Introduction to the Philosophy of Science]]"
---
We return to the topic of confirmation after the failed attempts by the logical positivists in chapter 3. This chapter discusses the most current view of the problem of confirmation called Bayesianism which PGS is not an advocate of.  The chapter is outlined as follows:
- The shape of philosophical discussion since the failures of logical positivism regarding confirmation
- The breakdown of the components and what is required for confirmation using Bayes' theorem
- Interpretation of the priori probabilities and the criteria of "rational individuals"

Since the failures of logical positivism in establishing a theory of confirmation, it has placed the "objective view" of science in a shaky place that has invited views from outside of science giving rise to the Science Studies. The most recent views on confirmation theory is Bayesianism. 

The difference between Bayesianism and logical positivism can be highlighted by the terminology. While the positivists used terms like confirmation to look at relationships between statements without looking at the contents of the statements ([in chapter 3, it was noted they followed the structure of deductive logic with the focus on form rather than contents of the statemets](Theory%20and%20Reality%20-%203%20Induction%20and%20Confirmation.md), Bayesianism does care about the contents of the statements themselves. In "statements" place is a "evidence" that have an intrinsic property of a probability ascribed to it. The difference is not highlighted by PGS.

# The Bayesian model of confirmation
The goal of Bayesianism is to view every statement and decision in terms of probabilities. Instead of verifying a hypothesis, we are increasing or decreasing the probability that a hypothesis is true. The way Bayesianism views confirmation is as follows:
1) An evidence confirms a hypothesis if it raises the probability of that hypothesis
2) The probabilities (to an individual) should be updated per Bayes' theorem
Rather than view induction as a logical relation (confirmation) between two statements, according to 1), Bayesianism look at realized events from a probability space called "evidence" and the core tenant of Bayesianism is that this evidence should update the probability that a hypothesis is true. How does it update the probabilities? We then follow 2). Bayes Theorem using [the total law of probabilities](Introduction%20to%20Mathematical%20Statistics%20-%201.4%20Conditional%20Probability%20and%20Independence.md): $$P(H|e)=\frac{P(e|H)P(H)}{P(e|H)P(H)+P(e|H^c)P(H^c)}$$
Where each term is as follows:
- $e$ is the probabilistic event of the evidence. Note this differs from the positivists who focused on general relationships without considering the content of the statements. In Bayesianism, the content matters for every "evidence" has an intrinsic attribute (i.e. probability).
- $H$ is the probabilistic event of the hypothesis
- $P(H)$  called the <u>prior probabilities</u>. This is the base probabilities to be updated
- $P(e|H)$ called<u> likelihoods</u> The probability that we should see $e$ if $H$ is true
- $P(H|e)$ called the <u>posterior probability</u> and is the final updated values
So with this formula, the rules of confirmation in light of "evidence" is established:
- If $P(H|e)>P(H)$, then the evidence confirms $H$
- Otherwise it does not confirm it

The method provides a formulaic way of updating probabilities, but when it comes to actually determining the likelihoods and prior probabilities, how do we determine the inputs for Bayes' formula: Is there some separate reality where there is a "true probability" that we need to find? That question invites the same problems scientific realism has. Instead, the idea is to keep probabilities internal to the individual themselves. This idea is called subjectivist probabilities
# Subjectivist interpretation of probabilities
Traditionally, frequentist had a sort of realism perspective on the nature of probabilities where there is an external reality that would hypothetically have a certain expected value if the probabilities were realized enough times. But the work in Bayesianism detaches probabilities from this "external reality" and consider probabilities to instead to be "degrees of belief" of an individual. Doing so keeps probabilities internal and actually lets us compute likelihood, and prior probabilities. There is no "universal" probability that everyone subscribes to, but it is instead a subjective matter that is internal to everyone.

The subjectivist interpretation therefore views probabilities as the "degree of belief" in a proposition. Prior probabilities and likelihoods are subjective degree of belief in their respective propositions, and one's probabilities is not the same as another. The act of confirmation is therefore the updating of the degree of belief in a prior probability in light evidence to become a posterior probability and this becomes the new prior probability to be tested again when new evidence comes to light. As PGS puts it: "Today's priors becomes tomorrows posteriors (p.206)".

The subjective interpretation of probability stems from decision theory which treats every thought and action as a series of "gambles" and probabilities are therefore the parameters that determines the individuals decision in a gamble. One's belief in a hypothesis is therefore a "gamble" in that sense and confirmation is the act of updating these beliefs that determine our decisions. In doing so, the beliefs must follow the math of probabilities (i.e. follow Kolmogorov's axioms) or one's decisions would lead to self-contradictions. If a person's belief system follows these axioms, then their belief system is considered "coherent" and they are called a "rational" individual. The importance of criteria of coherence an rationality is expressed in Dutch Book arguments that illustrate the potential contradictions that arise from incoherent belief systems

An individual is considered coherent if their subjective probabilities conform to Kolmogorov's axioms of probability:
1) All probabilities are between 0 and 1.
2) If a proposition is a tautology (i.e. analytically true), then it trivially has a probability of 1.
3) If two propositions are disjoint from each other, then the probability of either being true is the sum of the probabilities of each
4) The definition of conditional probabilities: $P(H|j) = \frac{P(H \cap j)}{P(j)}$ 
As an example, if someone's internal beliefs are such that his probability of believing and not believing something are both 60%, then they are not rational because it contradicts 3). The importance for individual to stay rational is illustrated by Dutch Book arguments to show that an irrational individual will always lead to a self-contradiction. In the example used by PGS, a person who does not have a rational coherent system of probabilities ascribed to their beliefs will always lose a gamble to a Dutch Bookie.

Bayesianism with the subjectivist interpretation therefore models confirmation as follows:
1) Beliefs are subjective to an individual and there is no universal number for everyone
2) The beliefs must be coherent
3) Beliefs are updated following Bayes' Theorem
# Assessing Bayesianism

How can people agree on anything if prior probabilities are subjective?
How does it address Goodman's riddle of induction
- Convergence


# Terms
- Bayesianism
- evidence (as opposed to confirmation)
- prior probabilities
- liklihoods
- posterior probabilities
- subjectivist interpretation of probability
# People and Historical Events
- Frank Ramsey and Bruno de Finetti's works in pioneering subjectivist interpretation of probabilities
