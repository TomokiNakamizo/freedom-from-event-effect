# Dymanic clinical risk prediction incorporating freedom-from-event effect

## risk_update.ipynb  <br>
This notebook provides code to compute updated risk estimates over an event-free period. <br>
####  Essential arguments: <br>
1) RR: Prespecified relative risk (hazard ratio or risk ratio) of the history of prior events. <br>
2) rate: Hazard ratio or risk ratio of age per year. <br>
####  Optional arguments:  <br>
3) T: Time (in years) over which risk estimates are updated.  <br>
4) latency and ref_T: Time interval over which the average hazard ratio (HR) is calibrated to match the prespecified relative risk (RR). <br>
Parameters are determined so that the average relative risk over the interval [latency, ref_T] equals the prespecified RR <br>
####  Frailty Distribution:  <br>
1) GammaFrailty: Use this class to specify a gamma frailty distribution. <br>
2) PVFFrailty: Use this class for other distributions in the PVF family (e.g., a = 0.5 for inverse Gaussian, and a < 0 for compound Poisson) <br>
####  Additional Options:  <br>
constant = True/False: Specifies whether the constant or average model is used. This option is relevant for gamma and beta-binomial models.<br>

## risk_update.ipynb  <br>
This notebook provides code to conduct simulations exploring how HR would be estimated in a real-world cohort study under a given set of parameters and study time periods. <br>
Users can specify settings in the Parameters and Cohort Setting sections. <br>

## Simulated_HR_across_various_scenarios.xlsx  <br>
This Excel file provides estimated hazard ratios (HRs) of prior events in simulations across various scenarios. It also contains the characteristics of the simulated populations, such as the proportion of individuals with prior histories in the whole population and the proportion of events among subpopulations with or without prior history. <br>

## Pointwise_HR.xlsx  <br>
This excel file shows time-varying (point-wise) HR under various scenarios.<br>

##  Reference: <br>
Nakamizo T and Misumi M. When Prior Events Predict Future Risk: The Freedom-from-Event Effect and Dynamic Clinical Risk Estimation with Frailty Models. (submitted)  <br>

## Caveat: <br>
This code provides theoretical predictions based on prespecified parameters and distributional assumptions for frailty. Users should exercise clinical judgment and consider all available information when making decisions.


