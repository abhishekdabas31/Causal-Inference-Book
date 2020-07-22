# Back Door Paths

**Back door path:** Arrows pointing towards the treatment are essentially the back door paths. These are the other paths of getting from the treatment to the outcome. It could be considered as a sneaky or unofficial path from the treatment to outcome.

We need Back-door Paths so as to find the estimated causal effect of one variable on another,  by blocking the other paths. It is a method for adjustment criteria for conditioning on non-causal variables. The key goal is to remove the non-causal association and remove the bias in the model.

**Back Door Paths helps in determining which set of variables to condition on for identifying the causal effect.**

**Back Door Adjustments:** 

**Defination:** A set of variables {Z} satisfies the backdoor criterion relative to an ordered pair of variables \(T,Y\) in a DAG if: 1. no node in {Z} is a descendant of T, and 2. {Z} blocks \(d-separates\) every path between T and Y that contain an arrow into T \(so-called “backdoor paths”\).

This means that you need to understand precisely the mechanism by which D \(let's now say it's smoking\) affects Y \(lung cancer\). Let's say it all flows through variable M \(tar in lungs\): D \(smoking\) affects M \(tar\), and M \(tar\) affects Y; there is no direct effect. Then, to find the effect of D on Y, compute the effect of smoking on tar, and then the effect of tar on cancer - possibly through backdoor adjustment - and multiply the effect of D on M with the effect of M on Y.

**Surrogate Confounder :** If we can not block a back door path directly in a case, then we can try and condition on a child of the Counfouder, which will help reduce the condounder effect \(if not reduce it\)

**It answers Questions like:**

1. Can we identify the causal effect of Interest?
2. What variables do i need to identify that effect? \(Only if i have data on the confounding variable, we can identify the effect?\)
3. Are There any common causes of Treatment and outcome? or any Backdoor path from treatment to outcome

**Solution**:

The Solution identifying a causal relationship between variable is to first identify all the paths between both the variables, then classifying them as Front Door or Back Door Paths. What we want is to close all the Back Door paths and make sure all the Front Door paths remain open. To identify the this causal effect we need to adjust or control for the variables. In layman terms it means holding the variable constant. To understand the effect of X on Y, we have to make sure we have closed all the Back-door paths while leaving all the Front-Door Paths open. We can close back door paths by controlling the variables on those back door paths. We can do that by statistically holding these variables constant.  **Example**: If we are trying to understand the relation between being sick and going to doctor, then there might be a confounder, "Past health issues". People with past health issues -&gt; more likely to go to doctor when sick. People with no past health issues less likely to go to doctor. To understand the effect of being sick and going to doctor, here we have to condition on the variable "Past health issues". By controlling the variables in back door path we want to make sure we are comparing the effect on same population.





Resource: [https://www.ssc.wisc.edu/~felwert/causality/wp-content/uploads/2013/06/2-elwert\_dags.pdf](https://www.ssc.wisc.edu/~felwert/causality/wp-content/uploads/2013/06/2-elwert_dags.pdf)

A good resource is : [Nick Huntington-Klein](https://www.youtube.com/watch?v=eBij0BFc-RM&list=PLcTBLulJV_AKmUTH-nUsxxFyRQoWnUzxU) 's Youtube videos on Causality

