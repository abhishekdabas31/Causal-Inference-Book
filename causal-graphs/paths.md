---
description: The study of graphs!!
---

# Graph Theory

Graph theory has been a part of mathematics which was originated by Leonard Euler!! Later this concept was used and formalized by Judea Perl in 1995, and Spirtes, Glymour, Scheines. It is a key part of Causal Graphs Theory. It is used to study the Independence properties of sub-graphs.

**A graph** is a network of nodes connected together through edges.

* **Nodes** are vertices that correspond to objects. They are represented by circles\(but can be of any other shape as well\)
* **Edges** are the connections between objects. They are represented by lines with arrows.
* **Path -** Consecutive sequence of arrows between the nodes irrespective of direction, disregarding their directionalities
* **Blocked Path -** A collider in the paths, blocks the path.
* **Unblocked Path -** No collider between the path, means its unblocked

**Note**: A path can be blocked by conditioning on the variable or nodes in the path. **Example**: conditioning on a mediator or a confounder can block the path. Completely opposite happens when we condition on a collider

**Nodes & Edges:**

* The node at the entrance of the edge is called the **Parent node.**
* The node at the exit of the edge is called the **Child node.**
* Two noded connected edge to edge is called **Adjacent nodes.**
* The parents of the parent node are known as the **Ancestor nodes**
* The **Degree of a node** is the total number of edges coming in and going out of the node.

**Note:**

* The likelihood of a node depends on the likelihood of its predecessors or its parents in the DAG
* The properties of a graph change when we add, remove or change the direction of the paths.

_**D-connected and D-Separated \(**D stands for Directional**\):**_

* **D-connection:** x and y are d-connected if there is an unblocked path between them. _\*\*_
* **D-separation** is a criterion for deciding, from a given a causal graph, whether a set X of variables is independent of another set Y, given a third set Z. 

**Note:** The idea of this is to **associate “connectedness” to “dependence”** and **“Independence” to “separation”. "D-Separation = Statistical Independence"**

**A path is D-separated** if the variables on both ends are independent of each other. If A and B are d-separated then ![{\displaystyle \(A\perp \!\!\!\perp B\)\mid C}](https://wikimedia.org/api/rest_v1/media/math/render/svg/bb5a126208b708ce2ce62d8d4aa802418aa5311d), where C is the adjustment set.

**D-separation rules:**

1. If there are no variables being conditioned on a path is blocked if and only if two arrowheads on the path collide at some variable on the path.
2. Any path that contains a non-collider that has been conditioned on is blocked.
3. A collider that has been conditioned on does not block the path
4. A collider that has a descendant that has been conditioned on does not block a path

**Two variables are D-separated if all paths between them are blocked**.

![X is D-connected to Y ](https://lh5.googleusercontent.com/is0nxWcWuZw21rkxdIJgNXbamOgdvIIduK038vX5j7MKm7h04mJCsNz6FSSOOxpRI_ozsGADavofLEWd94DHX2k2rSOGLEOvljPMhOJBmP2daKqEXSOTCHFYk3eVwCIxvT253P4E)

![ X and Y are not D-connected due to the collider B](https://lh6.googleusercontent.com/re3OIWEIJDZFdCCiBXYKbIAdBTQen666AoHz-4nD5qpnYatPxi-2E_TcUqivT1rCES_NIZS0EH56jPctDVSjx2Rdht-4LM1HIUdJAHX2OOGQ5PlYqx575HCN7BFY9ND0MQDZEr69)

* **Example**: As we see 1 has a **D-Connection** to 5;  2 is a **D-Separator** for connection between these as its dependent on 2 

![](../.gitbook/assets/image%20%286%29.png)

**The Direct connection between X and Y can be :**

1. Directly connected : X -&gt; Y

   **Indirect connections between X and Y can be in 4 ways:**

2. Indirect cause : X -&gt; Z -&gt; Y
3. Indirect effect : X &lt;- Z &lt;- Y
4. Common cause : X &lt;- Z -&gt; Y
5. Common effect : X -&gt; Z &lt;- Y

**Conditional Independence:** It is important to understand that, two variables are only related if there is a path between them so that we can focus on the important paths between variables. The concept of conditional independence helps us understand and tells us whether a variable is independent or other or not.

![](../.gitbook/assets/image%20%2830%29.png)

A and B are independent only when we condition on the variable "C", or we can say they become conditionally independent, conditioned on "C". **or we can say A and B are not independent unless we condition on C.**

## **Causal Markov Condition:**

Also known as the **Markov Assumption.** The **Causal Markov \(CM\) condition** states that conditional on the set of all the direct causes\(Parent nodes\), a node is independent of all variables which are not direct causes or direct effects\(non-descendants\) of that node.

**Describing the interventions in the way has some immediate consequences:**

1. X can only have some causal inference on Y if there is at least one directed path between X and Y. This is because if there is no directed path, with respect to the interventional graph the parents of X have been removed, so X⊥⊥Y in the intervential graph.
2. If there are _only_ directed paths between XX and YY, then the causal influence of XX on YY is given by the simply by the conditional distribution P\(Y∣X\)P\(Y∣X\). This is because the interventional graph has the same paths between XX and YY as the observational distribution.
3. If there is an unblocked, but not completely directed path between XX and YY, it means that both XX and YY share a common ancestor. This common ancestor is what is called a [_confounder_](https://en.wikipedia.org/wiki/Confounding), and will mean that if we try to estimate P\(Y∣do\(X\)\)P\(Y∣do\(X\)\) from P\(Y∣X\)P\(Y∣X\) of estimates will be biased. 

