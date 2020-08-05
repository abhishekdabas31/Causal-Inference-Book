---
description: Bayesian Network
---

# Testable Implications

**DAG can help us with probability Distributions as well:**

1. Variables that are independent from each other
2. variables conditionally independent from each other
3. methods to factor and simplify the joint distribution

DAG are the model representation of how we think the world works. DAG is becoming a very essential tool in the field of Data Science.

**Dependencies and Independencies are important to know and understand as it can tell us alot of information.** 

![](../.gitbook/assets/image%20%2827%29.png)

**Example**:

![](../.gitbook/assets/image%20%2818%29.png)

**Decomposition of Joint distribution :**

$$
P(A,B,C,D,E,F,G) = P(A) P(G) P(B|A) P(D|G,B) P(C|B) P(E|B,C,D) P(F|E)
$$

**Note**: We start from the root node\(which has no parent and move from there to subsequent child nodes\)

**Probability distributions from DAG**

* B is dependent on A

$$
P(B|A)
$$

* F is **independent** of A, B, C, D, G **conditional** on E \(The only thing that affects F is E, so if we condition on E we can control what affects F \)

$$
P(F|A,B,C,D,E,G) = P(F|E)  \\
F\perp \!\!\!\perp A,B,C,D,F |E
$$

* F & C are **marginally dependent or marginally associated** with each other

$$
P(F|C) \neq  P(F)
$$

Similarly, we can check the dependency for other variables. Thus we just saw that probability and this DAG are compatible with each other. 

\*\*\*\*

