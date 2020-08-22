---
description: A powerful approach
---

# Do-Sampler

"do-sampler" - It is a new feature in do-why.

When we are checking for a causal relationship between a treatment and an outcome, we need to explicitly define our assumptions and build a causal DAG for estimating the causal effects. Using the library we can test these assumptions and if we have controlled for the confounders. In many cases, we just want to check for whether there is a causal relationship between the treatment and outcome for which we want to control for confounders. Do-Sampler does this for us. We can specify the treatment, the outcome, and the common causes or Confounders. We can pick methods like weighting or importance sampling along with specifying the variable type as "d" for discrete or "c" for continuous. The package does the rest.

Controlling for the confounder it can help us to know if there is a causal relationship between the treatment and the outcome or not.

The dowhy package implements the [do-sampler](https://github.com/microsoft/dowhy/tree/master/dowhy/do_samplers) using three different methods: simple weighting, kernel density estimation, and Monte Carlo methods. The do-sampler supports both continuous and discrete variables. The sampling method uses the inverse propensity weighting. The math of how these methods work is explained in the link below.

Resource: [Medium blog by @akelleh](https://medium.com/@akelleh/introducing-the-do-sampler-for-causal-inference-a3296ea9e78d)

