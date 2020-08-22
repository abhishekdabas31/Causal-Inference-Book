---
description: Understanding the Causal Effects in Potential Outcomes Framework
---

# Potential Outcomes Framework

Potential Outcome Framework has helped in giving causal effects very precise definitions.

**The Potential outcome** is the outcome that would be observed if an individual is given a specific value of the treatment. It is the study of the effect of treatment at an individual level. For every Individual one can not simultaneously observe the 2 potential Outcomes, we can only observe one. Here, the unobserved outcome is called the **"Counterfactual Outcome ".**

**Two possible treatments, T - Treatment received or not received\(Placebo\)**

$$
T ∈ \{0,1\}
$$

**Two possible outcomes, Y - the outcome is there or not there**

$$
\{Y_i (0) ,Y_i(1)\}
$$

**Note: Quantities we are trying to measure here is not observable!!**

**Example:** What is the causal effect of doing a Master's degree and getting a high paying job?

* Treatment: doing Master's \(T=1\) & not doing Master's \(T=0\)
* Every individual person has 2 potential outcomes, Yt=0 & Yt=1 .
* Yt=0 -&gt; Potential Outcome when not doing Masters
* Yt=1 -&gt; Potential Outcome when doing Masters

## **ITE**

_\*\*_Individual Treatment Effect is the difference between the 2 potential outcomes for a particular individual. We cannot measure ICE as we would need counterfactual value for the individual.

$$
ICE = Y1 - Y0
$$

## **ATE**

Average Treatment Effect is the average difference between the 2 potential outcomes averaged over the entire population of interest. It is the population level average of the Individual Causal Effect\(ICE\).

$$
ATE = E[Yi1] - E[Yi0]
$$

* **Note**: Even though an Individual Causal Effect is non zero, the Average causal effect can be Zero.

