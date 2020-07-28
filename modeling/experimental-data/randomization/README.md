# Randomization

[Randomized controlled](https://en.wikipedia.org/wiki/Randomized_controlled_trial) tests are best to date, as we believe and agree that randomization is not biased. In this process, we randomly divide units into treatment and control groups before the action or intervention takes place, in an attempt to make these units comparable. Both the groups  \(treatment and control\) are given different treatments. Randomization makes these croups comparable, after which the outcome is observed. If we believe that data is separated without any bias, this is a very good method to for quick conclusions.

E-Greedy Method

1. Randomized Experiments:

*  A/B testing

![](../../../.gitbook/assets/image%20%2819%29.png)

**Why Randomization?**

If a person knows that they are getting a placebo or an active drug, they might stop taking the drug which hence would introduce bias. If this study is not randomized then the causal difference might be due to how the patients reacted, which is actually not causal effect. being assigned Thus the allocation should be randomized. Randomization removes the worry about the treatment being correlated with other missing values. The extreme version of this correlation is confounding.  

A **randomized experiment hold the following true:**

1. **Non Deterministic**, Every unit has a small and equal chance of being given treatment/control
2. **Individualistic**, Treatment assignment probability doesn't depend on the potential outcome of other covariates of other units
3. **Unconfoudned**, It is unconfounded treatment assignment probability is independent of the potential outcome.

**Unconfoundedness** is very crucial in randomized experiments, as randomization does not remove counfoundedness. Ex: checking the effect of college on a good job, where there might be a confounding effect in this relation. But randomization is not possible and not the solution. As we can't make sure if the students were already smart or college made them smarter for getting good paying jobs.

**There are 4 types of Randomized experiments:**

1. Bernoulli trials: Every unit is assigned a treatment with same probability p
2. Completely randomized experiments: Random sample, is taken and assigned to treatment. Example: **A/B testing** 
3. Stratified randomized experiment: Subgroups based on covariates X, are given a completely randomized experiments
4. Paired Randomized experiments: Special case of stratified randomzied experiments with 2 samples in each group 

**Resource**: 

[https://kojinoshiba.com/causal%20inference/what-are-experiments/](https://kojinoshiba.com/causal%20inference/what-are-experiments/)

