---
description: Causal Glossary
---

# Key Causal Terms and related Questions

* **What is the Causal Effect?**

The Causal effect can be defined as the difference or comparison between the true Potential outcomes of receiving and not receiving treatment. It is denoted as: Y\(Treatment\) - Y\(No-Treatment\)

* **What does Cause Mean?**

It has been defined multiple times from Aristotle. But generally what we mean is that if we change one variable, does it lead to change in the other one as well, keeping everything else constant.

* **Purpose of Causality?**

To understand the true cause and effect relationship. For Example: if X causes and outcome Y or not? Does smoking cause cancer or not?

* **What is Causal Lens or Data Generating process?** 

There is an **unknown but true Data Generating Process \(DGP\)** that exists and explains the world. It explains the question which we really need answers for, from the data. **Task**: Infer properties of DGP using data and assumptions\(since we dont know about\) about other properties of DGP. By this **we are trying to predict the consequences of interventions.**

* **What is Causal Inference?**

Causal Inference is process of drawing a conclusion about a causal connection based on the condition of the occurrence of the effect. A method of taking inputs and producing answers to causal questions.

**Inputs**:

1. What we wish to know?
2. What we do already know?
3. Available Data? - **Experimental and observational data**

**Outputs**:

1. Effects of pending interventions
2. Effect of undoing past events \(**Counterfactual**\)
3. **What is meant by Treatment and Outcome?**

Treatment can be defined as a cause that leads to some effect on an object or a person. That effect of this treatment on that object/Person is termed as Outcome.

* **What is the Gold Standard for Causal Analysis?**

In causal Analysis **Randomized controlled trials**, where the subjects are randomly assigned to a treatment and a controlled\(not given treatment\) group. The **difference between these distributions of outcomes of treated and controlled** represents the causal effect. Although this method is not always feasible. **The other method then is observational data\(uncontrolled experiments\)**

* **Predictive Modeling vs Causal Modeling:** 

**Predictive Modeling** is about predicting the outcomes. **Example:** predicting weather, elections, predict videos one will watch

**Causal Modeling** is used to control the outcomes. **Example**: can I control the weather?, can I influence the patient's weather?, how can I influence the next video you watch?

* **Examples of Causal Questions or Questions we can answer by knowing Causal Inference:**
* How effective was a treatment in preventing a disease?
* Does drinking Wine prevent Heart disease?
* Does passive smoking affect the mortality of non-smokers?
* To what degree Covid-19 outcomes are affected by lung problems?
* Was it the new tax break that caused sales to go up ? or the marketing campaign?
* Does adding business hours attribute to an increase in user engagement?
* Does rerouting users from the mobile site to downloading the mobile app increase page views?
* **Where causality fits in Machine learning**:

**Causal Inference is like unsupervised Regression** : Causal effect Coefficients are unknown from the data, whose real-world values are not known and cant be used for training. Ex: How much does X cause Y.

**Causal Structure Learning is like Unsupervised Classification**: Causal Structures are unknown and cant be used for training, thus they are unknown. Ex: What variables causes X, what variables don't cause X?

1. **Challenges in Causal Analysis**:
2. \*\*Association is not Causation\*\*
3. Combatting Bias: There are many Possible sources of Bias in data
4. Confounding
5. Uncertainty in Causal Directionality

We are trying to remove the bias associations so that we get the real causes and effects

![](.gitbook/assets/image%20%281%29.png)

\*\*\*\*

