# Back Door Paths

## **Explanation:**

These are the non-causal paths from the treatment to the outcome. These are called "Back-door" because they flow backward, out of the treatment. These are the arrows pointing towards the treatment. They are the other paths of getting from the treatment to the outcome. It could be considered as a sneaky or unofficial path from the treatment to the outcome.

Backdoor paths are the paths that remain if you remove the direct causal paths or the front door paths from the DAG.

We need to block these Back-Door Paths so as to find the estimated causal effect of one variable on another. It is a method for adjustment criteria for conditioning on non-causal variables. The key goal here is to remove the non-causal association and remove the bias from the model.

**Example**: Simplest possible Back-Door path is shown below

![](../.gitbook/assets/image%20%2840%29.png)

Back-Door path, where Z is the common cause of X and Y

$$
X \leftarrow  Z  \rightarrow Y
$$

Back Door Paths helps in determining which set of variables to condition on for identifying the causal effect. Once we block or close all the back door paths by making adjustments\(conditioning on the confounders etc\) we can identify the true causal relationship between the variables.

**Surrogate Confounders:** These are usually the child nodes of a confounder. If we can not block a Back-Door Path directly in a case, then we can try and condition on a child of the Counfouder, which will help reduce the confounder effect, if not eliminate it.

## **Back Door Criterion:** 

A set of variables {Z} satisfies the backdoor criterion relative to an ordered pair of variables \( Treatment \(T\), Outcome \(Y\) \) in a DAG if : 

1. no node in {Z} is a descendant of T 
2. {Z} blocks \( or d-separates\) every path between T and Y that contain an arrow into T \(so-called “backdoor paths”\).

This means that you need to understand precisely the mechanism by which D \(let's now say it's smoking\) affects Y \(lung cancer\). Let's say it all flows through variable M \(tar in lungs\): D \(smoking\) affects M \(tar\), and M \(tar\) affects Y; there is no direct causal effect. Then, to find the effect of D on Y, compute the effect of smoking on tar, and then the effect of tar on cancer - possibly through backdoor adjustment - and multiply the effect of D on M with the effect of M on Y.

## **Back Door Adjustment**

We need to block all non-causal paths from Treatment to Outcome

* Paths starting “T -&gt;” \(arrow pointing away from the treatment\) are either causal paths of interest or naturally blocked non-causal paths. Therefore, we do not need to do anything here.

**Note**: We should not condition on descendants of the treatment, as it could block the causal path from the treatment to the outcome.

* Backdoor Paths starting “-&gt; T” \(arrow pointing towards the treatment\), however, are always non-causal, and they may or may not be open. Thus, we may need to block these.

## **Important Questions**

Back-Door Criterion helps us answer questions like:

1. Can we identify the causal effect of Interest?
2. What variables do we need to identify the causal effect? \(Only if we have data on the confounding variable, we can identify the effect\)
3. Are there any common causes of Treatment and the Outcome? or any Backdoor Path from treatment to outcome?

## **Solution**:

The Solution identifying a causal relationship between variables is to first identify all the paths between both the variables\(Treatment and Outcome\), then classifying them as **Front Door or Back Door Paths**. What we want is to **close all the Back-Door Paths** and make sure all the Front-Door Paths remain open. To identify this causal effect we need to **adjust or control for the variables**\(it means holding the variable constant\). To understand the effect of X on Y, we have to make sure we have closed all the Back-Door paths while leaving all the Front-Door Paths open. We can close back door paths by controlling the variables on those back door paths. We can do that by statistically holding these variables constant.  **Example**: If we are trying to understand the relationship between being sick and going to the doctor, then there might be a confounder, "Past health issues". People with past health issues are more likely to go to the doctor when sick. People with no past health issues less likely to go to the doctor. To understand the effect of being sick and going to the doctor, here we have to condition on the variable "Past health issues". By **controlling the variables** in Back-Door Path we want to make sure we are comparing the effect on the same population.

## **Resource**:

1. [https://www.ssc.wisc.edu/~felwert/causality/wp-content/uploads/2013/06/2-elwert\_dags.pdf](https://www.ssc.wisc.edu/~felwert/causality/wp-content/uploads/2013/06/2-elwert_dags.pdf)
2. A good source - [Nick Huntington-Klein](https://www.youtube.com/watch?v=eBij0BFc-RM&list=PLcTBLulJV_AKmUTH-nUsxxFyRQoWnUzxU) 's Youtube videos on Causality

