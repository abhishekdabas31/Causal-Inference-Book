---
description: Be cautious and consider carefully!!
---

# Limitations of Causal Inference

1. **We cant estimate unit level effects\(ITE\).** The Average Treatment effect\(ATE\) is calculated with the causal methods.
2. There can be **many possible DAG'**s even for a reasonable number of variables, building the correct one from observational data is very hard.
3. **Multi-collinearity**: It is a big problem for Causal Models, as Causal Analysis mainly used regression Models\(according to current research\), wherein the **independent variables should have been independent**. If there is a high correlation between the independent variables, it causes problems in prediction by the model. It mainly undermines the statistical significance of an independent variable. Multi collinearity will affect the interpretability when we try to understand how we got there.
4. **Bias in Data**: A major goal in causal inference is getting data that is not biased. But in most cases, the data will be biased. The main issue is the variables are related to each other as well as the output variables. Such variables invalidate our conclusions.
5. **Results rely heavily on Observational Data:** Observational data does not control the data generating process, so we have to heavily depend on the theories for guided variables selections process. We can get stuck if no such theories are actually present. **This is the main concern of todays statisticians and why they do not accept causality.** 
6. **Historical data might not represent or be informative about causal effects.**
7. The World is very complicated. We can **not calculate all variables which are not observable.** 
8. There are **unobserved variables that cannot be controlled for. In such a case, we will get biased results even after applying the conditioning methods.**
9. We cannot measure the **strength of the causal relationships** from the DAG. Sometimes we need to know which features impact highly on the outcome.

