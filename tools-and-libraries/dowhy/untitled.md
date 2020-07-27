# Workflow

**This workflow can be captured by four key verbs in DoWhy:**

* model - encodes prior knowledge as a formal causal graph
* identify - uses graph-based methods to identify the causal effect
* estimate - uses statistical methods for estimating the identified estimand
* refute - tries to refute the obtained estimate by testing robustness to assumptions

**Difference estimation methods for causal inference:**

1. **Regression:** Linear Regression Method used
2. **Stratification:** Propensity Score used for Stratification
3. **Matching:** Propensity Score used for Matching
4. **Weighting:**  Inverse Propensity Scoring technique used to assign weights to units
   1. Vanilla Inverse Propensity Score weighting \(IPS\) \(weighting\_scheme=“ips\_weight”\) 
   2. Self-normalized IPS weighting \(also known as the Hajek estimator\) \(weighting\_scheme=“ips\_normalized\_weight”\) 
   3. Stabilized IPS weighting \(weighting\_scheme = “ips\_stabilized\_weight”\)
5. **Instrumental Variable** - Wald estimator used
6. **Regression Discontinuity**



**Installing library:**

```text
pip install dowhy
```

