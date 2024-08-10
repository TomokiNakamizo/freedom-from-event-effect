# free-f-e
-Compute updated risk estimate after event-free period. <br>
-Essential arguments include 1) RR: RR (HR) of the history of prior events and 2) rate: RR (HR) of age (per year). <br>
-Optional arguments include 3) T: time period (years) over which risk estimates are updated, 4) latency and ref_T: time period (years) over which average HR is calibrated to a prespecifed HR (argument RR above). The parameters will be determined such that the average over inteval [latency, ref_T] is equal to a prespecifed HR (argument RR above) <br>
-To specify a frailty distribution, use GammaFrailty class for gamma frailty, PVFFrailty for other PVF family (a = 0.5 corresponds to inverse Gaussian, and a negative a, to compound Poisson) <br>
-The argument, constant, specifies whether constant or average model will be used. <br>
 <br>
Reference:

