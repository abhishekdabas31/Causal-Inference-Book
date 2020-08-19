# Real-World Implementations

The field of causal AI is developing very rapidly and a lot of fields are currently adopting the graph-based approaches with causality.  

## [**Revolutionizing Biotech and Pharmaceuticals**](https://opendatascience.com/fastest-growing-sectors-of-ai-investment/)**:**

Research has shown that the next biggest piece of investment of the AI will be in revolutionizing the Biotech Industry. The first one is autonomous driving, but this one is getting very close. AI is after reducing the [overall cost of experimentation](https://www.policymed.com/2014/12/a-tough-road-cost-to-develop-one-new-drug-is-26-billion-approval-rate-for-drugs-entering-clinical-de.html),\(cost to develop one new drug is $2.6 billion\) which is really high currently. AI is expected to breakthrough with cancer research. And because these health issues are so complex, it required huge data preprocessing, something that humans cant do.

A very good read: [The future of clinical Trials](https://www.cbinsights.com/research/clinical-trials-ai-tech-disruption/)

## [**GNS Healthcare: A Boston Healthcare company**](https://www.gnshealthcare.com/)\*\*\*\*

**AIM**:  GNS Healthcare accelerates the discovery and development of drugs to improve patient outcomes and significantly reduce total cost of patient care. Our causal AI technology integrates and transforms a wide variety of patient data types into _in silico_ patients which reveal the complex system of interactions underlying disease progression and drug response. The _in silico_ patients enables the simulation of drug response at the individual patient level across oncology, auto-immune, neurology, and cardio-metabolic disease in partnership with the world’s largest biopharma companies and health plan

## **Uber:**

![](.gitbook/assets/image%20%2854%29.png)

[**Using causal Inference to improve the Uber user-experience**](https://eng.uber.com/causal-inference-at-uber/)**:**

Uber is using causal inference methods that enable us to bring richer insights to operations analysis, product development, and other areas critical to improving the user experience on our platform.  Causal Inference provides information that is critical to both improving the user experience as well as making business decisions through better understanding the impact of key initiatives.  For example, if we are able to translate intangible variables such as customer satisfaction to business metrics, we can then use that information to help prioritize new features and tools. If we are able to understand the short-term and long-term impact of a new program such as [Uber Pro](https://www.uber.com/newsroom/uberpro/), that will help us build more sustainably and inform future product development decisions.

![Ubers Food Discovery Remcomending : https://eng.uber.com/uber-eats-recommending-marketplace/](.gitbook/assets/image%20%283%29.png)

"We’ve found it invaluable to bring causal inference methods to our work at Uber, as it enables us to solve challenging but critical data science questions that would otherwise be impossible to tackle, such as estimating the treatment effect when a randomized controlled experiment is not possible or addressing additional complexities within the experimental data." - Uber

**It can help companies build better products through effective decision making** - Uber

* [**Mediation Modelling at Uber**](https://eng.uber.com/mediation-modeling/)**:**

**Uber Labs has been using Mediation analysis as well.** Mediation modeling goes beyond simple cause and effect relationships in an attempt to understand what underlying mechanisms led to a result. Using this type of analysis, we can fine-tune product changes and develop new ones that focus on the underlying mechanisms behind successful features on the Uber platform.

**Note:** _Online Controlled Experiments are the core of the decision-making process at big companies like Amazon, eBay, Facebook, Google, Microsoft, and Yahoo. As these companies are big and popular, using a simple AB test is not effective. These companies have been working on various different problems and solutions to effectively conduct AB test for better results. A small change in some metrics could cause a big impact on the uses of these companies._  

## **Netflix:**

![](.gitbook/assets/image%20%2856%29.png)

[**Experimentation and Causal Inference:** ](https://research.netflix.com/research-area/experimentation-and-causal-inference)\*\*\*\*

Netflix uses A/B tests for testing almost every new product. When A/B tests are not possible, Quasi-experiments and other causal Inference Methods are used. This helps them infer what works best and what doesn't work.

\*\*\*\*[**Improving Sensitivity of Online Controlled Experiments: Case Studies at Netflix** ](https://www.kdd.org/kdd2016/papers/files/adp0945-xieA.pdf)\*\*\*\*

## **Booking.com** 

![](.gitbook/assets/image%20%2853%29.png)

The company has been using controlled experiments \(A/B tests\) for testing its products which produce some effects on their customers. Even small changes can reflect in huge revenue differences. At Booking.com a new technique called CUPED is implemented for testing, which is proven very effective. 

{% embed url="https://booking.ai/how-booking-com-increases-the-power-of-online-experiments-with-cuped-995d186fff1d" %}

## **LinkedIn**

![](.gitbook/assets/image%20%2855%29.png)

LinkedIn uses A/B testing extensively for improving its ads over time. Linkedin has been researching different methods and using these tests for understanding the treatment and control effects very extensively in their production system. This has helped in increasing the impact of the ads and effective usage of the champaign budgets.

[Causal inference from observational data: Estimating the effect of contributions on visitation frequency at LinkedIn](https://arxiv.org/pdf/1903.07755.pdf)

## **Trip Advisor:** 

![](.gitbook/assets/image%20%2852%29.png)

Trip Advisor considers the A/B test as a powerful technique for effective decision making. They have been using techniques like **Stratification, Control Variables** using approaches like **Regression & CUPED**. The company has been using these tests for inferring the impact of even small changes on the homepage, and there has been a substantial improvement after using such methods. They have been trying different methods by incorporating pre-experiment data which has proven to be more effective in reducing the variance in the experimental measurements. Read more [Here](https://www.tripadvisor.com/engineering/reducing-a-b-test-measurement-variance-by-30/).

