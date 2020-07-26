# Simpsons Paradox

Simpsons Paradox is a very common phenomenon in Probability and Statistics. It occurs when we see trends in our data \(which is actually separated into groups\) but because the is aggregated together it shows trends which are not causal. When data is separate is shows different trends, whereas when aggregated it shows different trends.

It is important to understand and resolve Simpsons Paradox, because the data we see is not all the data that is there. This shows us that how easy it is to fall into a paradox when relying only on intuition about data and unaided statistical methods. It tell us the limits of statistical methods and why causality is necessary to avoid these paradoxical conclusions.

**Examples**: 

1. A study shows that in UC Berkley the admissions are biased towards men, and difference was big so it was unlikely due to chance. The study later showed that women tend to apply in more competitive departments with less acceptance rate, whereas men tend to apply to less competitive department with high rate of admission.

![](../.gitbook/assets/image%20%282%29.png)

**2.** Simpson Paradox on Reddit : Avg Comment weight decresed over time? what should be done?.... If we split the data we see that the avg comment length increases with time the user joined the platform. So its just that new users have been added on the platform

3. Covid 19 Dataset: [http://causality.cs.ucla.edu/blog/index.php/2020/07/06/race-covid-mortality-and-simpsons-paradox-by-dana-mackenzie/](http://causality.cs.ucla.edu/blog/index.php/2020/07/06/race-covid-mortality-and-simpsons-paradox-by-dana-mackenzie/)

**Solution** : This paradox is resolved when there is a proper Causal Relations addressed between statistical modeling. We have to think Causally. Causal Model for the data need to be built. Consider the data generating process and applying causal model, we can resolve simpsons paradox.

Unless these analysis are done, its hard to understand it. Causality is important to make sense out of this data

Conclusion:

1. Aggregated data and disaggregated data might show different results which leads to confusion in understanding or analysing the data.
2.  Interrogating the data using correctly phrased causal queries is really important



**Resources**:

1. [TowardsDataScience](https://towardsdatascience.com/simpsons-paradox-how-to-prove-two-opposite-arguments-using-one-dataset-1c9c917f5ff9)
2. [Understanding Simpsons Paradox- Judea Perl](https://ftp.cs.ucla.edu/pub/stat_ser/r414.pdf)
3. [Simpsons Paradox Unraveled ](https://academic.oup.com/ije/article/40/3/780/746837)



