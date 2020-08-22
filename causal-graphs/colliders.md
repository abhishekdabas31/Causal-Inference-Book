# Colliders

**Colliders** are variables where two arrowheads meet. It blocks the dependency between the variables on the 2 ends.

**Note:** While adjusting the bias, we should adjust the confounders. Adjusting for a collider may introduce Bias. If a path has collider it is already blocked and we do not need to block or condition on it.

**Example:** If there is a child variable, with 2 parent variables pointing towards it. Child variables are affected you both parent \(a child had mixed characters of both parents\), but doesn't mean one parent is affected by another one.

![](../.gitbook/assets/image%20%2810%29.png)

