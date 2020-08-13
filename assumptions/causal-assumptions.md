# Causal Assumptions

Identifiability of causal effects requires making some untestable assumptions. Because of the problem in Causal Inference, that we do not see both the potential outcomes within the data, it is required to make some strong assumptions. Some of these assumptions are untestable, these untestable assumptions are the **causal assumptions**. These assumptions are about the observed data, i.e treatment, outcome, and the set of pre-treatment covariates. 

**The most common assumptions are:**

1. SUTVA - Stable Unit Treatment Value Assumptions - \(potential outcomes \)
2. Consistency
3. Ignorability
4. Positivity

* **SUTVA - Stable Unit Treatment Value Assumptions**

SUTVA helps us write the potential outcome for a person in terms of only that specific person's treatments. SUTVA has 2 components:

1. **No Interference**: Units do not interfere with each other. Treatment applied to one unit does not affect the treatment assignment for another unit. ex. peer pressure
2. **No hidden variations of the treatment.** There is only one single version of each treatment. Single versions of treatment make the potential outcome well defined, multiple versions make it very complex.

* **Consistency Assumptions**

The potential outcome under treatment A=a, Y^a, is equal to the observed outcome if the actual treatment received is A=a. So the observed outcome is assumed to be equal to the potential outcome.

* **Ignorability Assumptions**

This assumption states that conditional on pre-treatment covariates, the treatment assignment is independent of the potential outcomes. The treatment has to be randomly assigned and should not be dependent on the other covariates. If we are assigning the treatment to a population, it should be independent of who would be benefited from the treatment. Conditioning on variables \(confounders\) can help us make the treatment assignment randomized. This assumption can also be called "**No Unmeasured confounders**"

**Ideal Experiment**: the potential outcomes, Y1 and Y0, must be jointly independent \(“∐”\) of treatment assignment

$$
Y1 , Y0\perp \!\!\!\perp T
$$

**Observational Studies:**  The potential outcomes, Y1 and Y0, must be jointly independent \(“∐”\) of treatment assignment within groups defined by the value of X.

$$
Y0 , Y1\perp \!\!\!\perp Y   | X
$$

* **Positivity Assumption**

For every set of values for X, treatment assignment is not deterministic. It makes sure that even after controlling for variables, not all the population receives a particular treatment. This makes sure we have observational data on all the treatments for making correct assumptions about the potential outcome. Variability in treatment assignment is important for identification.

**Hence, These Assumptions are very important to link the Observed data with the potential outcome.**







