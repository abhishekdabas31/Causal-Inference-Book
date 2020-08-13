# Inverse Propensity Weighting

IPW or inverse probability Weighting drawn from the concept of weighting itself. In this process, we initially consider the probability of every person being assigned to a treatment or control group. If some part of the population that has a higher probability of being in the treatment group, is assigned to the control group, are very valuable. Here we would want to weigh-up this population in the control group, and weigh-down the majority of the population which actually went into the treatment group.

**Example**:

$$
w(x)=  \frac{1}{p(x)}\\
w(x)=  \frac{1}{1-p(x)}
$$



