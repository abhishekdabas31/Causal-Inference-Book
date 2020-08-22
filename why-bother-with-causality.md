# Why bother with Causality?

Statistical Inference seems to be serving the world well. Machine Learning and AI seem to have reached a completely different level and have been giving out results that would have seemed almost unimaginable years back. 

So why bother adding Causal Inference to mix and risk messing things up? 

Here is an [article](https://www.technologyreview.com/2019/01/21/137783/algorithms-criminal-justice-ai/) published by MIT that tells us exactly why. 

Machine Learning models these days focus primarily on correlation and not causation. Most people building these models tend to assume that just because a feature is highly correlated to what they are trying to predict, it is a good enough reason to make it a predictor variable. That simply is not true! 

As we saw in the article above using the Race as a feature to predict if a person is a criminal or not is simply absurd and not serving any purpose. Yes, the race might be correlated with the past data of people being criminals but there are a bunch of other factors that are the real cause of the crime and the race. 

This is the thought process that Causality looks to build in the Data Scientist building the model and this is why it is super important to understand and implement. 

Here is the use case of Causality on a real-world data set of school grades. 

Let's have a look at what the dataset looks like - 



![Preview of the School Data Set. ](.gitbook/assets/image%20%2815%29.png)

We see that we have a bunch of features and let's assume we are trying to predict a student's average grade across the 3 subjects given all of these features. 

If we were performing just the statistical analysis of these variables we would find the level of significance by performing a regression analysis. 

![](.gitbook/assets/image%20%2812%29.png)

We would see from the results above the p-value is less than our significance level of 0.05 and thus the race feature seems to be highly correlated. We thus will decide to use this as one of our predictor variables. 

However, let's think about this from a Causal Inference point of view. From our understanding of the world, we know that a student's race should not really have anything to do with the grade that the student is getting. 

Let's look at the effect of the other variables and how the performance of the grades of the different races changes when the other factors are kept constant. 

**First, let's look at the whole data -** 

![](.gitbook/assets/image%20%289%29.png)

**Now let us look at the grades across all races for the students whose parents only went to high school -** 

![](.gitbook/assets/image%20%281%29.png)

**And now let's look at those students whose parents have a Master's degree -** 

![](.gitbook/assets/image%20%2816%29.png)

So we see, how the average grade across students of all races changes depending on the education of the parent. The education of a parent has a far more causal relationship with the average grade of the students because it is more likely that a more educated parent would place further importance on education to the student\(it could be the other way around too. ;\) \). 

A similar analysis can be done with other features as well until the change of grades based on race is negated. Other factors that can lead to poor grades can be health factors, monetary factors etc. All of these might not be present in the collected data but they are important to be accounted for so that a variable like the race is not used to then in the future predict if a student will pass or fail. 

Therefore, to better the results of the statistical models, and to avoid biases that may be added to the model by just believing in satistical significance, scientists should start building causal diagrams trying to causally explain how the variables are affecting each other and then build a statistical model of causally significant variables for predictions. 

![](.gitbook/assets/image%20%285%29.png)

This book aims to take you through understanding how to build such causal diagrams and the other important factors to look for while determining a causal relationship. 

