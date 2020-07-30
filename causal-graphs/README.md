# Causal Graphs

Causal graphs are referred to as **DAG -** Directed Acyclic Graphs!!!

* **There are 2 types of graphs:**

1. **Undirected graphs** have edges that do not have a direction.
2. **Directed graphs** have edges with direction.

Causal Diagrams represent association and causation both, simultaneously. They help us think better. We need expert knowledge to construct causal DAG, which in many cases might not be possible. So we construct multiple DAG, without being able to choose the correct one.

We require the graph to be acyclic to prevent "causal loops".

**Causal DAGs consist of three elements:** 

1. Variables \(nodes, vertices\) 
2. Arrows \(directed edges, arcs\): possible direct causal effects. The arrows order the variables in time.
3. Missing arrows; sharp assumptions about absent direct causal effects.

Helps us :

1. Identifying variables to control for
2. Explicit the assumptions about origin of data 

**Applications:**

1. **Model testing**
2. **Structure learning**
3. **Reduce "what if i do questions to symbolic calculus**
4. **reducing scientific questions to symbolic calculus**

**Solutions:**

**Experimental data is too expensive and also illegal sometimes,**



