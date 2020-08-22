# Counterfactuals

## **Explanation**

**Counterfactual Analysis** is a comparison of what happened with the intervention and what would have happened in the absence of that intervention. We can determine the causal effect, by looking at the outcome, under both conditions. When there is a treatment and when there is no treatment given. We say there is a causal effect when these 2 potential outcomes are different.

Counterfactual Analysis is all about answering the question, "**what would have happened if?**". To understand and answer that question, we need to know what would have happened if a certain thing did not take place, which is a hypothetical or counterfactual outcome. Causal Inference is the general goal for counterfactual Analysis, as causality is considered to be the difference between the two potential outcomes under the intervention.

**Example**:

1. _Given that I have a beard, and that I have a PhD degree, and everything else we know about me, with what probability would I have obtained a PhD degree, had I never grown a beard._
2. A counterfactual question is **about a specific data point in this case PHD.**

_2. If a person dies after treatment, we can ask the counterfactual question, would the person die if the treatment was not given?, which can help us understand the causal relationship between treatment and outcome._

## **Problems**:

1. **The treated and untreated population should be comparable**. We cant observe the results if we distinguish people if they are healthy vs unhealthy people because in such case the outcome will definitely be different.
2. For answering these counterfactual questions we need Causal Diagrams to answer this for us\(Do calculus\). Counterfactuals are personalized, as they would change if you go from 1 person to another.

## **Solution**:

The simplest thing one can do to attempt to answer my counterfactual question: collect data about individuals. Some important solutions could be:

1. **Randomization** - It is the simplest answer to resolve Counterfactual Problems. It makes both the groups exchangeable. **Example:** Half of the population is given the treatment, and half of them are not, and then we observe the result. As a result, we observe the average effect on both the population.
2. **Build a Causal Structure**: We do not observe the counterfactuals in the real world. What we try to do is build a causal Structure, which can be used for answering the causal questions. If we have the causal structure and the probabilistic equation of the model, then we can try to answer the counterfactual questions. This, we can do this from the observed data. The approach here is to build a robust structure for the environment and then we can use it for answering different types of questions.

**Conflict Here:** Some researchers have been trained using causal DAG, while others have been trained using counterfactuals, the use of different language creates confusion sometimes.

## **Resource**:

1. [link](https://www.inference.vc/causal-inference-3-counterfactuals/) 
2. [Counterfactual prediction is not only for causal inference](https://link.springer.com/epdf/10.1007/s10654-020-00659-8?sharing_token=kV_G0mmo-GLt_VMxT1mAQve4RwlQNchNByi7wbcMAY42AdnWyM4OfVl8JP7D5adb3UNqXoMBumdL1pxYQD2LUm9m-c8_PzZXcjKx8x_DktYi5coJJY9kN0FptIhOklAgGc9znqVFZlAnBpLWkno67wS_g0diHlOzpCeO3_k6kLk%3D)

