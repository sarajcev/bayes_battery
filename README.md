## Bayesian data exploration of battery cells discharge measurements

Battery's internal impedance from multiple discharges, using a multilevel model with clustering on cells: 

- complete pooling: all data is lumped together,
- no pooling model: treats each cell as completely independent from others,
- partial pooling: recognizes each individual cell, but all cells share information through the higher level model structure.

Battery's internal impedance from multiple discharges, using a multilevel model with clustering on discharge cycles:

- partial pooling with a unique variance: recognizes each individual discharge cycle, with sharing of information between cycles and a unique variance on all cycles,
- partial pooling with individual variances: recognizes each individual discharge cycle, with sharing of information between cycles and individual variances for each cycles (also mutually informed through the higher level model structure).
- trend of the impedance evolution through discharge cycles.

Battery's internal impedance from multiple discharges, using a multilevel model with clustering on both cells and cycles at the same time.

Bayesian model comparison using leave-one-out cross-validation.

Bayesian models of battery cells discharge measurements using Gaussian process regression:

- battery impedance regression using GP and temperature measurements,
- incorporating measurements uncertainty or errors,
- exploring different correlation structures of the GP kernels, from:
	* battery geometry (cell distances),
	* cell connections resistances,
	* connections graph structure.