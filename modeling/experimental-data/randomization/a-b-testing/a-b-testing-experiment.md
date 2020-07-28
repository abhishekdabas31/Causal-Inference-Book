# Experiment

![](../../../../.gitbook/assets/image%20%2821%29.png)

As we saw in the last section, randomization without bias is a super important aspect of A/B testing. However, while drawing a conclusion from the test performed, one should be certain that there are no external factors that might be affecting the way the results are showing up.

One such example could be: Let's say a website was looking to test a new version of the website. Suppose post the running of the A/B test and getting the p-value the company determines that there is no significant difference between the old and the new website. However, old people who mostly visited the website in the morning loved the old website, and the young people who mostly visited the website in the evening loved the new one.

However, because their likes are the polar opposites of each other the significance in the difference of the 2 websites goes down close to 0. This is not the case though. The new website is drawing different results, however since we have not accounted for external factors such as time of day and the age of customers we end up with a false inference.

This is exactly why the process of Causal Inference is necessary. This false inference could have been avoided by simply understanding the results in a broken down format.

To get a better understanding of the topic, have a look at:

[The Trap of A/B testing for too long.](https://medium.com/swlh/the-trap-of-a-b-testing-for-too-long-a4706066a692)

To play with the simulation, spoken about in the article use the following colab notebook: [A/B Testing Simulation](https://colab.research.google.com/drive/1kRSvmD0SPu0-uumEu2ofTqU4bcKiDxZh?usp=sharing).

