# Instrumental Variables

Instrumental Variables are used to control the confounding and measurement error in observational studies. They allow for the possibility of making Causal inferences with Observational Data. Instrumental Variables can adjust for both observed and unobserved data confounding effects.

Observational studies usually are implemented as a substitute for or complement to clinical trials. The problem with using observational trials to make a causal inference is that an individual may be more likely to receive treatment because the individual has one or more co-morbid reasons which would not be the case in a controlled experiment like the A/B test. The outcome may be influenced by the fact that some of the individuals received the treatment because of their personal or health characteristics.

Steps of **Instrument Variable Analysis**

1\) We observe a variable Z, called the Instrument which is correlated to our outcome variable B.

2\) We will assume that this variable Z, **does not** have a causal relationship on B.

3\) We will assume that Z **does** have a correlation with the treatment variable A.

4\) Given our assumption in Step 2, we will now randomly assign Z.

5\) If our assumption on 3 is right then Z will still have a correlation with A and that will be Z's causal effect on A.

6\) Since Z is randomly assigned, it is no longer correlated to any other possible confounder except the treatment \(A\) The treatment\(A\) in turn is only correlated to the outcome. \(B\)

## **Resources**:

[The Logic of Instumental Variables](https://www.youtube.com/watch?v=4xF_DMbL14w)

