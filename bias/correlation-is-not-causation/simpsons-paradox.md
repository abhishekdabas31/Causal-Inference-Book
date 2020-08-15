# Simpsons Paradox

Simpsons Paradox is a very common phenomenon in Probability and Statistics. It occurs when we see trends in our data \(which is actually separated into groups\) but because it is aggregated together it shows trends that are not causal. When data is separate is shows different trends, whereas when aggregated it shows different trends.

![](../../.gitbook/assets/image%20%2843%29.png)

It is important to understand and resolve Simpsons Paradox because the data we see is not all the data that there is. This shows us how **easy it is to fall into a paradox** when relying only on intuition about data and unaided statistical methods. It tells us the limits of statistical methods and why causality is necessary to avoid these paradoxical conclusions.

**Examples**: 

1. **Biased Admissions:** A study shows that in UC Berkley the admissions are biased towards men, and the difference was huge so it was unlikely to be due to chance. The study later showed that women tend to apply in _more competitive departments_ which have less acceptance rate, whereas men tend to apply to _less competitive departments_ that have a high rate of acceptance.
2. **Simpson Paradox on Reddit**: Avg Comment weight decreased over time? what should be done?.... If we split the data we see that the avg comment length increases with time the user joined the platform. So it's just that new users have been added on the platform
3. **COVID-19 Dataset**:  According to research results, whites make up a lower percentage of deaths than cases. But when we aggregate all of the ages, whites have a higher fatality rate. The reason is simple: whites are older. According to U.S. census data \(not shown here\), 9 percent of the white population in the United States is over age 75. [ReadMore](http://causality.cs.ucla.edu/blog/index.php/2020/07/06/race-covid-mortality-and-simpsons-paradox-by-dana-mackenzie/)

* The COVID 19 dataset shows that such problems are really serious and raises a fundamental question that does the data reflect reality?

**Solution**: A solution here would be Stratification. Conditioning on the variables can solve this problem here.

This paradox is resolved when there is a proper Causal Relations addressed between statistical modeling. We have to think Causally. Causal Model for the data needs to be built. Consider the data generating process\(DAG\) and applying the causal model, we can resolve Simpsons Paradox.

**Conclusion:**

1. Aggregated data and disaggregated data might show different results that can lead to confusion in understanding, analyzing, and Inferring from the data.
2.  Interrogating the data and using correctly phrased causal queries is really important.
3. Unless the analyses on data are done effectively, it's hard to understand and resolve such problems. Hence, Causality is important to make sense out of this data



**Resources**:

1. [TowardsDataScience](https://towardsdatascience.com/simpsons-paradox-how-to-prove-two-opposite-arguments-using-one-dataset-1c9c917f5ff9)
2. [Understanding Simpsons Paradox- Judea Perl](https://ftp.cs.ucla.edu/pub/stat_ser/r414.pdf)
3. [Simpsons Paradox Unraveled ](https://academic.oup.com/ije/article/40/3/780/746837)



