# Free-from-event-effect and dynamic clinical risk estimation
- Compute updated risk estimate over event-free period. <br>
- Essential arguments include  <br>
1) RR: prespecifed relative risk (the hazard ratio or risk ratio ) of the history of prior events  <br>
2) rate: the hazard ratio or risk ratio of age per year. <br>
- Optional arguments include:  <br>
3) T: time (years) over which risk estimates are updated,  <br>
4) latency and ref_T: time period over which average HR is calibrated to the prespecifed relative risk (RR). <br>
Parameters will be determined so that the average relative risk over the inteval [latency, ref_T] is equal to the prespecifed relative risk RR <br>
-To specify a frailty distribution, use GammaFrailty class for gamma frailty, PVFFrailty class for other PVF family (a = 0.5 corresponds to inverse Gaussian, and a negative a to compound Poisson) <br>
- The argument, "constant = True or False", specifies whether the constant or average model will be used. This option is relevant to gamma and beta-binom. <br>
 <br>
Reference:
Nakamizo T and Misumi M. When Prior Events Predict Future Risk: The Freedom-from-Event Effect and Dynamic Clinical Risk Estimation with Frailty Models. (submitted)

