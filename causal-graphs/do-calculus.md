# do-calculus

Interventions and counterfactuals are represented by **do\(x\)**, which simulate the physical interventions by deleting certain functions from the model and replacing them with constant X=x, while keeping the rest of the model unchanged.

When we intervene on a variable, we have a constant variable for the treatment

With observational data, we can build the causal Graph on the left hand side and to better understand the causal relationships we do an intervention on X and observe the effects of the intervention. The right graph helps us answer what would happen if we do an intervention

Interventions:

![Graphical Representaion of Intervention](../.gitbook/assets/image%20%2813%29.png)

In the figure above, 

$$
Left: Title\:Length \leftarrow Author's\: Skill \\
Right: Title\:Length \leftarrow Yes(Constant)
$$

Interventional Distritution:

$$
P(CTR, Authors Skill \:| \: do(X=Yes)
$$

