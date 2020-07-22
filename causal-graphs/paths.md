---
description: D-connection & D-separation
---

# Paths

This concept is formalized by Judea Perl in 1995,  and Spirtes, Glymour, Scheines. it is a key part of Causal Graphs Theory. It is used to study the Independence properties of sub-graphs.

* **Path -**   Consecutive sequence of arrows between the nodes irrespective of direction, disregarding their directionalities
* **Blocked Path -** A collider in the paths, blocks the path.
* **Unblocked Path -** No collider between the path, means its unblocked

**Note**: A path can be blocked by conditioning on the variable or nodes in the path. example: conditioning on a mediator or a confounder can block the path. Completely opposite happens when we condition on a collider 

_D-connected and D-Separated **\(D stands for Directional\):**_

* **D-connection:** x and y are d-connected if there is an unblocked path between them. ****
* **D-separation** is a criterion for deciding, from a given a causal graph, whether a set X of variables is independent of another set Y, given a third set Z. 

**Note:** The idea of this is to **associate “connectedness” to “dependence”** and **“Independence” to “separation”.  "D-Separation = Statistical Independence"**

**A path is D-seperated** if the variables on both ends are independent of each other. If A and B are d-separated then  ![{\displaystyle \(A\perp \!\!\!\perp B\)\mid C}](https://wikimedia.org/api/rest_v1/media/math/render/svg/bb5a126208b708ce2ce62d8d4aa802418aa5311d), where C is the adjustment set.

**D-separation rules:**

1. If there are no variables being conditioned on a path is blocked if and only if two arrowheads on the path collide at some variable on the path.
2. Any path that contains a non-collider that has been conditioned on is blocked.
3. A collider that has been conditioned on does not block the path
4. A collider that has a descendant that has been conditioned on does not block a path

**Two variables are D-separated if all paths between them are blocked**. 

\*\*\*\*

![X is D-connected to Y ](https://lh5.googleusercontent.com/is0nxWcWuZw21rkxdIJgNXbamOgdvIIduK038vX5j7MKm7h04mJCsNz6FSSOOxpRI_ozsGADavofLEWd94DHX2k2rSOGLEOvljPMhOJBmP2daKqEXSOTCHFYk3eVwCIxvT253P4E)



![ X and Y are not D-connected due to the collider B](https://lh6.googleusercontent.com/re3OIWEIJDZFdCCiBXYKbIAdBTQen666AoHz-4nD5qpnYatPxi-2E_TcUqivT1rCES_NIZS0EH56jPctDVSjx2Rdht-4LM1HIUdJAHX2OOGQ5PlYqx575HCN7BFY9ND0MQDZEr69)

\*\*\*\*

**Example**: As we see 1 has a **D-Connection** to 5;  2 is a **D-Separator** for connection between these as its dependent on 2 

![](../.gitbook/assets/image%20%286%29.png)

**Direct connection between X and Y can be :**

1. Directly connected : X -&gt; Y

 **Indirect connections between X and Y can be in 4 ways:**

1. Indirect cause :  X -&gt; Z -&gt; Y
2. Indirect effect : X &lt;- Z &lt;- Y
3. Common cause : X &lt;- Z -&gt; Y
4. Common effect : X -&gt; Z &lt;- Y

**Conditional Independence:** It is important to understand that, two variables are only related if there is a path between them so that we can focus on the important paths between variables. The concept of conditional independence helps us understand and tells us whether a variable is independent or other or not.  

![](../.gitbook/assets/image%20%2811%29.png)

A and B are independent only when we condition on the variable "C", or we can say they become conditionally independent, conditioned on "C". **or we can say A and B are not independent, unless we condition on C.**

Describing the interventions in the way has some immediate consequences**:**

1. X can only have some causal inference on Y if there is at least one directed path between X and Y. This is because if there is no directed path, with respect to the interventional graph the parents of X have been removed, so X⊥⊥Y in the intervential graph.
2.  If there are _only_ directed paths between XX and YY, then the the causal influence of XX on YY is given by the simply by the conditional distribution P\(Y∣X\)P\(Y∣X\). This is because the interventional graph has the same paths between XX and YY as the observational distribution.
3.  If there is a unblocked, but not completely directed path between XX and YY, it means that both XX and YY share a common ancestor. This common ancestor is what is called a [_confounder_](https://en.wikipedia.org/wiki/Confounding), and will mean that if we try to estimate P\(Y∣do\(X\)\)P\(Y∣do\(X\)\) from P\(Y∣X\)P\(Y∣X\) of estimates will be biased. 



