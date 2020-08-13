---
description: Causal Glossary
---

# Key Causal Terms and FAQ

* **What is the Causal Effect?**

The Causal effect can be defined as the difference or comparison between the true Potential outcomes of receiving and not receiving treatment. It is denoted as:

$$
Y(Treatment) - Y(no Treatment)
$$

* **What does Cause Mean?**

It has been defined multiple times from Aristotle. But generally what we mean is that if we change one variable, does it lead to change in the other one as well, keeping everything else constant.

* **Purpose of Causality?**

To understand the true cause and effect relationship. For **Example**: if X causes and outcome Y or not? Does smoking cause cancer or not?

* **What is Causal Reasoning?**

Causal reasoning is the process of understanding causality. A cause must be present for an effect to occur. If A causes B, then B will not occur without A. Thus this process of reasoning the causes and effects are known as Causal Reasoning.

* **What is an Estimand?** 

Causal Estimand can be defined as the expectations of potential outcomes. It is the treatment effect that has to be estimated in statistical analysis or a clinical trial.

* **What is the Causal Lens or Data Generating process?** 

There is an **unknown but true Data Generating Process \(DGP\)** that exists and explains the world. It explains the question which we really need answers for, from the data. **Task**: Infer properties of DGP using data and assumptions\(since we don't know about\) about other properties of DGP. By this **we are trying to predict the consequences of interventions.**

* **What is Causal Inference?**

Causal Inference is the process of drawing a conclusion about a causal connection based on the condition of the occurrence of the effect. A method of taking inputs and producing answers to causal questions.

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

1. **Predictive Modeling** is about predicting the outcomes. **Example:** predicting weather, elections, predict videos one will watch?
2. **Causal Modeling** is used to control the outcomes. **Example**: can I control the weather?, can I influence the patient's weather?, how can I influence the next video you watch?

![](.gitbook/assets/image%20%2843%29.png)

* **Examples of Causal Questions or Questions we can answer by knowing Causal Inference:**

1. How effective was a treatment in preventing disease?
2. Does drinking Wine prevent Heart disease?
3. Does passive smoking affect the mortality of non-smokers?
4. To what degree Covid-19 outcomes are affected by lung problems?
5. Was it the new tax break that caused sales to go up ? or the marketing campaign?
6. Does adding business hours attribute to an increase in user engagement?
7. Does rerouting users from the mobile site to downloading the mobile app increase page views?

* **Where causality fits in Machine learning**:

1. **Causal Inference is like unsupervised Regression**: Causal effect Coefficients are unknown from the data, whose real-world values are not known and cant be used for training. Ex: How much does X cause Y.
2. **Causal Structure Learning is like Unsupervised Classification**: Causal Structures are unknown and cant be used for training, thus they are unknown. Ex: What variables causes X, what variables don't cause X?

* **Challenges in Causal Analysis**:

1. \*\*Association is not Causation\*\*
2. **Combatting Bias:** There are many Possible sources of Bias in data
3. Confounding
4. Uncertainty in Causal Directionality

We are trying to remove the bias associations so that we get the real causes and effects

* **What is the Causal Hierarchy?**

It is also known as Pearl causal Hierarchy or ladder of causation. 

![](.gitbook/assets/image%20%2832%29.png)

1. **Association**: The initial level at which most Machine learning models operate
2. **Intervention**: The 2nd level where we understand how our actions affect the environment
3. **Counterfactuals**: The level at which we can ask the "what if" questions

**Note**: The lower you go into the table the more you know about the real world causal Model. The higher in the level you are, the better idea we have about the real world.

**Facts**: you can only move across the level if you have the Structural Causal Model \(Causal graph for that environment\)

* **What is Intervention?**

If we take a variable and set a manually to a different value\( a change that specific value to something different\), without changing anything else is known as the process of doing an Intervention. We do it all the time with the causal model to understand causal relationships. It can be thought of as coming from outside and doing some change in the model manually and try to make an inference about the output after that intervention. 

* **Structural Causal Model vs Structural Equation Model?**

**bayesian network+intevention** 

**sem----think**

* **Evidence-based Pyramid**

The Evidence-Based pyramid is frequently used to understand and formalize the knowledge of the hierarchy of evidence and how this evidence can be used for formulating the recommendation for practice. The different levels of evidence are appropriately represented by the pyramid of evidence as shown below. The levels from bottom to top reflects an increase in the quality of the research design. **Example**: Systematic reviews are of higher quality than just expert opinion. 

**Note**: Randomized control trials\(RCT\) are considered on the 2nd top, in the Evidence Pyramid

![](.gitbook/assets/image%20%2838%29.png)

