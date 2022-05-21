# When Should You Adjust Standard Errors for Clustering&mdash;Simulation Study with a Continuous Covariate

Masashi Yoshioka

May 21, 2022

## Description

This repository contains my paper "When Should You Adjust Standard Errors for Clustering&mdash;Simulation Study with a Continuous Covariate" along with its source code.

## Abstract

I have simulated a model with a continuous covariate and showed that the discussion of Abadie et al. (2017, 2021) could apply to the case with a continuous covariate. The results have implied that when the coefficient is fixed, we can always use Liang&ndash;Zeger cluster-robust variance estimator for samples that have a group structure. However, if the coefficient is random and correlated within clusters, Liang&ndash;Zeger cluster-robust variance estimator can be too conservative. The within-cluster correlation of covariate matters in this situation. If it is close to zero, the heteroskedasticity-robust variance estimator will be correct. If it is close to one, Liang&ndash;Zeger cluster-robust variance estimator will be correct. If it is neither small nor large, both estimators will fail. On the other hand, the within-cluster correlation of error term does not matter. Based on the results, I have proposed one potential strategy for clustering adjustments, which first estimates the within-cluster correlation of covariate to determine which variance estimator should be used.

## References

Abadie, A., Athey, S., Imbens, G. W., \& Wooldridge, J. (2017). *When should you adjust standard errors for clustering?* (NBER Working Paper No. 24003). National Bureau of Economic Research. https://www.nber.org/papers/w24003

Abadie, A., Athey, S., Imbens, G. W., \& Wooldridge, J. (2021, October 8). *When should you adjust standard errors for clustering?* [Conference presentation]. The Gary Chamberlain Online Seminar in Econometrics. https://www.chamberlainseminar.org/past-seminars/autumn-2021\#h.i4t9eedzteeb

Liang, K. Y., \& Zeger, S. L. (1986). Longitudinal data analysis using generalized linear models. *Biometrika*, 73(1), 13--22.
	
Moulton, B. R. (1986). Random group effects and the precision of regression estimates. *Journal of Econometrics*, 32(3), 385--397.
