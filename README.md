# Nuanced interpretaion of clinical risk prediction incorporating between-individual heterogeneity in event risk

## risk_transfer.ipynb  <br>
This notebook provides code to map event risks predicted by risk scores derived from prevalent cohorts (observed between latency and ref_T) to event risk among the same-aged populations at the time fo diagnosis (incident cohort).
## risk_update.ipynb  <br>
This notebook provides code to compute updated risk estimates over an event-free period <br>
####  Arguments: <br>
1) RR: Prespecified relative risk (hazard ratio or risk ratio) of the history of prior events <br>
2) rate: Hazard ratio or risk ratio of age per year <br>
3) T: Time (in years) over which risk estimates are updated <br>
4) latency and ref_T: Time interval over which the average hazard ratio (HR) is calibrated to match the prespecified relative risk (RR). <br>
Parameters are determined so that the average relative risk over the interval [latency, ref_T] equals the prespecified RR <br>
####  Frailty Distribution:  <br>
1) GammaFrailty: Use this class to specify a gamma frailty distribution. <br>
2) PVFFrailty: Use this class for other distributions in the PVF family (e.g., a = 0.5 for inverse Gaussian, and a < 0 for compound Poisson) <br>
####  Additional Options:  <br>
constant = True/False: Specifies whether the constant or average model is used. This option is relevant for gamma and beta-binomial models.<br>

##  Reference: <br>
Nakamizo T and Misumi M. When Prior Events Predict Future Risk: The Freedom-from-Event Effect and Dynamic Clinical Risk Estimation with Frailty Models. (submitted)  <br>

## Caveat: <br>
This code provides theoretical predictions based on prespecified parameters and distributional assumptions for frailty. Users should exercise clinical judgment and consider all available information when making decisions.


