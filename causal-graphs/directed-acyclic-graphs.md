# Build your DAG

**Steps**:

1. Draw the Causal DAG
2. Write all the Paths from X to Y
3. Identify Front door and Back Door Paths
4. On a given path, is there is a collider

**Characteristics** : 

* _**Controlling Confounder Paths :**_

1. Increase precision of model
2. Reducing Bias within the models prediction

* _**Collider Paths :**_

1. Collider automatically blocks the back door path
2. Sometimes a variable is collider and confounder on different paths.

* _**Mediators Path** :_ 

1. No need to control mediators if you are interested in total effect from X -&gt; Y
2. It introduces indirect effect from X -&gt; Y

**Problems**: 

1. Data does not always contains enough information to know whether a variable is a confounder or not. To deal with confounding we need expert knowledge.

**Solution:** 

1. **Randomization :**  If we are checking the effect of treatment  T on outcome Y, then we can randomly assign Treatment to a population. Then there might be other causes of Outcome Y, but Treatment has only once cause that is random flip of coin. So overall it has no common cause or back door path.

* **A/B Testing :**

  Two statistical data sets are compared, or a data set obtained by sampling is compared against a synthetic data set from an idealized model. A hypothesis is proposed for the statistical relationship between the two data sets, and this is compared as an alternative to an idealized null hypothesis that proposes no relationship between two data sets.

**Problem with Randomization:** 

* **Unethical and not always possible**. Testing smoking effects cancer or not, is something we can not force people to do.
* **Self Selection Bias:** It occurs when different members of the populations of interest have different probabilities of arriving in the sample. If the sample is not representative of the whole population the conclusions we make would be unutrustworthy. When we are running an A/B Test, we plan on testing it on a random sample of population, which is not always possible. **Example** : In case of an E-commerce platform testing, the test is run on people present \(Online, in case of an e-commerce website testing\). We have to be sure about the effect that we are testing, really what we are looking for?  **Solution to Selection Bias :** define the population of interest according to the data that is accessible!!  [Link ](https://towardsdatascience.com/were-21-of-new-york-city-residents-really-infected-with-covid-19-aab6ebefda0)

**We can not always do experiments and use the Experimental data, which is why we need to use observational data, big/Huge observational data \(Data that needs to be adjusted for confounders\)**

**2. Conditioning:**  Condition on the confounder to get the subset of the data which the back door path blocked, for the analysis. Conditioning on confounders removes the bias from the model.

* **Statification :**  Condition the confounder, to get a subset of data for analysis. Example: condition that Confounder = 0 \(No heart disease patients, if heart disease is confounder\).  The main idea here is to identify a strata and compute the causal effects only within that strata
* A more sophisticated way is Regression Analysis????????
* **Matching:** Matching tries to predict the outcome, by associating the similar pair of elements within the data, where we can find one is treated and the other is not.We can use Propensity Score for matching.Matching eliminates the back door path, but it cant be represented by DAG. **Example:** Matching every person who took aspirin and had a heart attack, with person who did not take aspirin and had a heart attack. And also, people who took aspirin and did not have a hear attack, with person who took aspirin and also did not have an heart attack. We then restrict the analysis to those who matched.

**Requirements for all these methods:**‌

1. All these Methods Require data on confounders, Any method can be used unless its time Varying, in which case we need G methods.‌
2. All require knowledge of true causal Graphs

**NOTE :** _**With these Methods we can try to reduce the bias within our Model. It does not completely remove the bias.**_

