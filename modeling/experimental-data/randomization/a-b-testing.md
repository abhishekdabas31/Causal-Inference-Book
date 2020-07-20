# A/B Testing

A/B testing is an example of a completely randomized trial. It is considered as standard and basic test for randomized controlled experiments.

It is a very basic way of testing two versions of things and figure out which version performs better. It is a randomized experiment testing method with two variants **A and B**, statistically testing these. The main responsibility of A/B testing is to experiment with new ideas for testing Machine Learning Models and actions to improve existing ones. It does the testing and reports the statistics for it. In A/B testing we are actually **controlling** how to allocate users to different groups. It is a gold standard method for understanding the **causal relationship.**

**A/B testing is commonly used method for causal Interpretation.**

> In a lot of cases, getting the data for the entire population is very hard. The solution to this would be taking a sample \(ex. selecting 1000 from 100000 people\) and doing statistical analysis on the sample data to predict how the remaining\(99,000 people\) are going to perform. This process of selecting a small portion from larger population is called **sampling** \(this sample can represent the overall population\). Example: If 10% from 1000 people buy a product, then if we select a sample of 10 people, 1 would buy the product. The ratio will remain the same.

**Hypothesis Testing:** A statistical hypothesis test is a method of statistical inference. Commonly, two statistical data sets are compared, or a data set obtained by sampling is compared against a synthetic data set from an idealized model. A hypothesis is proposed for the statistical relationship between the two data sets, and this is compared as an alternative to an idealized null hypothesis that proposes no relationship between two data sets.

**Hypothesis Testing Steps**:

1. Come up with a new hypothesis: Null Hypothesis\(New features have no effect, it is a baseline assumption that there is no relationship between 2 datasets\)
2. Gather relevant data 
3. Test statistics \(Statistical significance,p=value\)

P-Value\( **It is the specific probability of getting results as extreme as we have if the null hypothesis were true\)**

**A/B test** starts by deciding what hypothesis we want to test. **Example**: size of the subscribers button. The metric here is how many people click on the button. To run the test we show different buttons to different people and then conclude which size of button made more CTR. In this case there is is very important to understand that there might be different factors influencing the clicks on the button, screen size ? mobile & laptop version? which can influence the result of our analysis. By **randomization**, we are minimizing these factors here. If population of these are not similar, we can consider diving the population with screen size \(Conditioning on the confounder\). Usually in such cases, we need to identify the effects and incorporate assumptions within the process of causal effect estimation, which can otherwise lead to wrong conclusions.

**Assumptions are an important part of modeling in causal Inference. Hence If we disregard the assumptions before modeling, it can lead to miscellaneous results!!**

**Multivariate testing :** A/B testing can further be used for testing multiple variables, we can end up doing A/B/C/D testing

**Example**: A-B testing, If p-values is 0.0216, which is less than 0.05, we reject null hypothesis by saying there is a 2.16% chance of Alternate hypothesis coming from random noise.**We are just proving there is a correlation between the conditions but not causation \( a relation between new ads and higher people coming in\)**

**Use case:**

* Companie use this method for testing everything from website designs to offers and product descriptions etc.  A/B testing is a very important concept to gather both quantative and qualitaitve user insights and use them to understand the potential customers and optimize the conversion funnel based on data. 

**Problems:**

1. **Self Selection Bias:** When we are running an AB Test, we plan on testing it on random sample of people that represent the whole population. But is that really True? , The test is running on people present\(Online, in case of a e-commerce website testing\). We have to be sure about the effect that  we are testing, really what we are looking for?
2. It is very difficult to have a perfect, clean A/B test, when we are increasing the scale of people or the target audience
3. Looking at too many metrics \(risk of spurious correlations\)
4. Ending the AB test too soon. It usually takes a lot of time \(3-4 weeks of running time\)
5. Multi-split testing

**Solution**:

1. To ensure the sampling is random, we have to run our test every day of the week \(Longer duration\)
2. Avoid small sample size by calculating the min sample size required before test
3. Make sure the test is not stopped too soon  
4. Retesting is important, to remove the possibility of contradictory results.

**Conclusion**:

AB Testing checks the effect of the treatment over a population that selects themselves into AB Test









Resource : [https://towardsdatascience.com/data-science-you-need-to-know-a-b-testing-f2f12aff619a](https://towardsdatascience.com/data-science-you-need-to-know-a-b-testing-f2f12aff619a)

[Statistical significance](https://towardsdatascience.com/statistical-significance-hypothesis-testing-the-normal-curve-and-p-values-93274fa32687)

[what AB Testing is acctually measuring](https://medium.com/@akelleh/what-do-ab-tests-actually-measure-e89ebd63a73e)

[https://hbr.org/2017/06/a-refresher-on-ab-testing](https://hbr.org/2017/06/a-refresher-on-ab-testing)

[https://www.invespcro.com/blog/ab-testing-14-sampling-issues-that-can-ruin-your-test/](https://www.invespcro.com/blog/ab-testing-14-sampling-issues-that-can-ruin-your-test/)

