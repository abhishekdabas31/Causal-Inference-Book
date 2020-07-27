# Assumptions

While learning about the cause and effect relationships within causal Inference, **assumptions** play a very important role. In Machine Learning models as well, we have assumptions. Its just that the assumptions are already embedded within the data, which we assume to be true. We do not have all the data we really need, hence we need to make some strong assumptions to fill these missing values. These assumptions are about how the Data Generating Process\(DGP\). 

Especially, when we are dealing with observational data \(which is largely most of the data that we have\), there is a necessity to add "**Assumptions**" for making causal conclusions.

**NOTE: If we had all the data we really need we would not need assumptions, because in that case, all  the assumptions about the population would be already present in the data.**

The misconception here is that statistical Inference on the selected data can be used for decisions. Lets start it from the beginning!!

**What is Population?** It is the collected data of all the existing items that are present in this world in regard to our question of interest.

**What is a Sample?** It is a random, small subset data of this population data. 

Take any example and consider the definition of these again. **Example**: avg height of men in United States. My Population here is every men \(**All of them**\) in the United states, that's what we need to consider for making a decision here. If we go and calculate the height of every men, its easy to conclude and make decision on this. But this is real world, and let's be realistic here, its not a smart approach. Now we take a sample of population of men and make a conclusion from their height. Since calculating the real height of every man is not possible here, we make the best guess about it using statistics. Now if your data is of all the tall people in US then your assumption about the height of men in US will be different from someone with data of men with shorter height.  Now no one is wrong here!!! **But the problem is that we are treating our sample as our population here**.  

Facts : 

1. The more accurate data you have more precise is your conclusion. 
2. Acknowledging the fact that we are dealing with uncertainty. 

**INFERENCE \(or Prediction\) = DATA + ASSUMPTIONS**

Now if we had data or facts about all the population of interest, we wouldn't need these assumptions. Now I think we can agree that in most cases we do not have the actual population data, hence we do not have the real facts with us. Which in other words mean there is a gap within what we know and what we wish we knew. Assumptions are the connecting path from our past data to making inferences about what we want to predict or infer.

_**The assumption is a very important part of decision-making process!!**_ 

When we analyze data, we assume all of it is captures without errors. The human brain also works on past data. We like something because our past experience has been positive in regards to that particular thing. It all works on past experiences or past examples or past data. But when we consider bias, or some misconceptions within these examples, it makes assumptions more important. **Maybe the word assumption makes it sound a little vague. We can consider assumptions as "teaching" or "data generating rules".** 

**Examples**: 

1. When we are using a calculator for adding our bills, we assume that the mathematical formulas embedded in the machine are correct
2. When we drive our Tesla, we trust the company for its 5-star safety promises. We trust the company
3. When we pay our bills or transfer the money to someone, we assume the systems are secure and the transaction will go as planned in right hands.

We all have been making some strong assumptions in our daily lives, which has been affecting our day to day decisions.

**Problem**: 

* People can have different assumptions which can lead to different conclusions. We see it while analyzing the data, different people come can come out with different conclusions.

**Solution**:

1. **Domain Expert**: This is where domain experts come in, and where their domain expertise can be used to unlock the true assumptions that we need to make about the data generating process. Example: A researcher in the field of Healthcare or a doctor would have more knowledge about the factors affecting COVID 19 compared to others. Hence their assumptions would be a more accurate depiction of the true Causal DAG.
2. **Sensitivity Analysis**
3. **Testing and specifying Assumptions:** 

**Conclusion**:

We need to formalize Assumptions. We make some assumptions, combine it with data and then make an actionable decision. Assumptions are the source for us to cope up with the facts and information that is lacking in our decision-making process.





**Resource**:

 [https://towardsdatascience.com/the-saddest-equation-in-data-science-e60e7819b63f](https://towardsdatascience.com/the-saddest-equation-in-data-science-e60e7819b63f)

[https://towardsdatascience.com/statistician-proves-that-statistics-are-boring-4fc22c95031b](https://towardsdatascience.com/statistician-proves-that-statistics-are-boring-4fc22c95031b)

