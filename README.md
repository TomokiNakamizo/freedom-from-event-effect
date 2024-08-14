# free-from-event-effect
-Compute updated risk estimate after event-free period. <br>
-Essential arguments include 1) RR: prespecifed relative risk (the hazard ratio or risk ratio ) of the history of prior events and 2) rate: the hazard ratio or risk ratio of age per year. <br>
-Optional arguments include 3) T: time period (years) over which risk estimates are updated, 4) latency and ref_T: time period over which average HR is calibrated to the prespecifed relative risk (argument RR above). The parameters will be determined such that the average relative risk over the inteval [latency, ref_T] is equal to the prespecifed relative risk <br>
-To specify a frailty distribution, use GammaFrailty class for gamma frailty, PVFFrailty class for other PVF family (a = 0.5 corresponds to inverse Gaussian, and a negative a, to compound Poisson) <br>
-The argument, "constant = True or False", specifies whether the constant or average model will be used. <br>
 <br>
Reference:

