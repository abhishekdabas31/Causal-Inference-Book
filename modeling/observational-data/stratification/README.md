# Stratification

## Explanation:

Stratification is defined as the act of sorting data, people, and objects into distinct groups or layers. It is a technique used in combination with other data analysis tools. When data from a variety of sources or categories have been lumped together, the meaning of the data can be difficult to see. This data collection and analysis technique separates the data so that patterns can be seen and is considered one of the seven basic quality tools.

_**Stratum** refers to a single subgroup or layer!!!_

Stratification is done by obtaining a treatment effect within each stratum and them pooling across every stratum, weighting by the probability of each stratum. **Stratification is a very effective causal method**. We gather enough observational data and condition on variables, assuming that within each stratum the treatment assignment would be randomized. **Example**: We cannot control for the health of a person, but gathering enough data on the health of people so that we condition on variables like age, weight, heart disease assuming that under such stratum the treatment assignment would be randomized.

There is a causal effect within each stratum, as the treatment can be thought of as randomized here.

**Standardization:** From the data, you could estimate a treatment effect then by just computing means under for each treatment, within each stratum. And then pooling across the stratum where we're weighting by the size of the stratum. When the whole population is bunched together and not stratified on a particular variable, our inference can be very different than what it would be, had the stratification been performed.

From the definition, it is clear to see that stratification is exactly what solves the [Simpson's Paradox](https://github.com/abhishekdabas31/Causal-Inference-Book/tree/090cfeee8785ef0e136cfe1996bd2897326fdd57/modeling/observational-data/bias/simpsons-paradox.md).

![](../../../.gitbook/assets/image%20%282%29.png)

Let's consider a stratification and Non-stratification data \***comparision**\*

## **Problem:**

1. There might be a big collection of variables that need to be controlled. In such cases, we need data on the combination of all these variables, which would not always be true. Example: If we have to stratify on age and treatment, then we need data on all possible combinations of age and treatment
2. Other methods to achieve this are: matching inverse probability of treatment weighting and propensity score methods

## **Solution**:

* Determining the variables that should and should not be controlled for is an important step of a causal inference analysis and involves close collaboration between researchers and domain experts who have substantive knowledge of the business problem in question.

## **Resource** :

[Coursera: A Crash Course in Causality: Inferring Causal Effects from Observational Data](https://www.coursera.org/lecture/crash-course-in-causality/stratification-xEcaf)

[Principal Stratification — Uses and Limitations](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3154088/)

