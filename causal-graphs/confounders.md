# Confounders

**Confounder:** The variable which is the common cause of 2 variables\(Referring to treatment and the outcome\)

**Confounding Effect**: A falsification within the association between an exposure and an outcome can be considered as a confounding effect. Any common cause of both a covariate and outcome may be a confounding effect. If there is an association and no causal effect between nodes, there might be confounding. Confounding is another type of **Bias**. But unlike a lot of other biases, this one can be controlled for within the analysis. We need to adjust for variables to eliminate the effect of confounding in the analysis. **Examples**: There is potential for confounding in Health Problems. If past health affecting the treatment assignment and the outcome then the past health history is a confounder. Age is a very common confounder in such health-related causal questions

![](../.gitbook/assets/image%20%2848%29.png)

Z is a **confounder** of the effect of X on Y if Z meets **3 conditions**:

1. Z is associated with X
2. Z is associated with Y conditional on X
3. Z is not on a causal pathway from X to Y.

**The question we ask here is If we can remove this confounding effect?**

We can remove the confounding effect by the method of stratification.

**Example**: **X** - _Medication_**;** **Y** - _stroke_; **Z** - _History of heart disease_; **U** - _Weak arteries_

![](../.gitbook/assets/image%20%287%29.png)

In the above picture, If we have to condition on confounder and do not have enough data on the variables then we have to condition on one of the variables, "Z" in this case to restrict the back door path\(If we don't have data on U\). We can condition on either one of them\(Z or U\) or both of the two variables \(Z and U\) to restrict the backdoor path.

* **Causal Path :** 

$$
X \rightarrow Y
$$

* **Backdoor path:**

$$
X \leftarrow Z \leftarrow U \rightarrow Y
$$

**Problem**: A lot of times we are unaware or misinterpret the confounders within the data which can cause bias and be risky for our Causal Model.

**Note**: If we are not aware of confounders and do not control them, it can lead to bias within the causal relationship. As well as misinterpreting confounding and controlling for them can lead to biased results.

