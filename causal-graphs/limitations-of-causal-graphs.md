# Limitations of Causal Graphs

1. Causal graphs do not depict the size or quantify the strength of the relationship
2. There is always a possibility of uncontrolled confounding in DAG, which can not be estimated
3. A DAG is dependent on the information provided. Lack of information can lead to wrong analysis.
4. In most cases, we construct multiple DAG, without being able to choose the correct one.
5. A variable can be a mediator, collider, and confounder simultaneously, which can be interpreted differently in different research questions leading to different results.
6. If we interpret a collider as a confounder and condition on it, it can lead to a false causal relationship.

