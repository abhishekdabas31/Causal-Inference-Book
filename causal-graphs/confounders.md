# Confounders

**Confounding**: A falsification within the association between an exposure and an outcome can be considered as counfounding. Any common cause of both a covariate and outcome may be a confounding effect. If there is an association and no causal effect between nodes, there might be a counfounding. Confounding is another type of **Bias**. But unlike a lot of other biases, this one can be controlled for within the analysis.  We need to adjust for variables to eliminate the effect of confounding in the analysis. **Examples**:  There is potential for confounding in Health Problems. If past health affecting the treatment assignment and the outcome then the past health history is a confounder. Age is a very common confounder in such health-related causal questions

**The question we ask here is If we can remove this confounding effect ?**

L is a **confounder** of the effect of A on Y, if L meets 3 conditions: 

1. L is associated with A
2. L is associated with Y conditional on A
3. L is not on a causal pathway from A to Y.

![](../.gitbook/assets/image%20%286%29.png)

In the above picture, If we have to condition on confounder and do not have enough data on the variables then we have to condition on one of the variables, "Z" in this case to restrict the back door path\(If we don't have data on U\) . We can condition on only 1 variable to restrict the backdoor path.

* **Causal Path : X &gt; Y**
* **Backdoor path :  X &lt; Z &lt; U &gt; Y**
* **If we condition on U or Z  or both U and Z**

X - Medication , Y - stroke,  Z - History of heart disease , U - Weak arteries

![](../.gitbook/assets/image%20%287%29.png)

