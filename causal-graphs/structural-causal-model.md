# Structural Causal Model

**Definition**: The structural Causal Model tries to represent the data generating process\(DGP\) by explicitly defining causal relationships. 

In term of Judea Pearl:

SCM is a tuple \(V, U, F, P\(U\)\) where 

V = {V1,....Vn} which is endogenous variabes \(observable variables\)

U = {U1,...Un} which is exogenous variable\(Unobserved variable\)

F = {F1....Fn} which is the fuctions \(the arrows in causal graph\)

P\(u\) = It is the distribution of U or the unobserved variables. 

**Note**: With the Structural Causal Model, which helps to unbox the real-world black-box model. Helps us in Interpretability. 

The Structural Causal Model tries to formalize the causal relationships in the form of a graph. Then using some of the defined algorithms we can determine whether the effect can be calculated through the data available or not. **These tools are as good as the assumptions feed to the system.** 

The SCM helps us in identifying the testable implications from the causal graph which can be used to come to causal conclusions. These testable functions could be really easy such as Linear functions, or as complex as cubic functions.

