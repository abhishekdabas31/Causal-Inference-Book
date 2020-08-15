# Matching

## Explanation

It is a method that strategically subsamples data into covariates into balanced covariate distribution into treated and control groups such that after matching both groups share equal probability of treatment

Matching is one of the several techniques established in the field of statistics that helps in estimating the Causal effect. It is suggested to use matching with regression for better results. There are different types of matching techniques that have been developed. There has been a development from **simple covariate matching to propensity score matching techniques**. A lot of new algorithmic matching techniques have been developed that search for optimal matches in both treatment and control groups according to their weights.

Matching is usually the **first step for estimating** the treatment effect. Matching prepares the data for further statistical analysis but in itself its not enough for estimation of the treatment effect.

This method originated after there were some problems with conducting A/B tests. The aim here was to define a good match and discard the unmatched observations, which can then lead to an unbiased estimation of the treatment effect.

![Source: Uber](../../.gitbook/assets/image%20%2851%29.png)

## Implementation:

In matching a metric needs to be defined according to which the treatment and control can be matched and other unmatched observations can be removed.  We want to find the appropriate metric that can lead to a perfect match resulting in a **covariate balance** between both the treatment and control groups.

If there is just one pre-treatment covariate, then we would sub-sample on that covariate such that, the pre-treatment variables for both the treatment and control group matches with each other. As and when these pre-treatment variables tend to increase we need to sub-sample all these covariates and match the covariates in such a way that the pre-treatment variates of both treatment and control variables are comparable. The process becomes more and more complex once these pre-treatment variables increase. Only after achieving a covariate balance, we can have a clearer picture of the true treatment effect. 



