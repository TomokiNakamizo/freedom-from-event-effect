# free-f-e
Compute updated risk estimate after event-free period. 
Essential arguments include 1) RR: RR (HR) of the history of prior events and 2) rate: RR (HR) of age (per year).
Optional arguments include 3) T: time period (years) over which risk estimates are updated, 4) latency and ref_T: time period (years) over which average HR is calibrated to a prespecifed HR (argument RR above). The parameters will be determined such that the average over inteval [latency, ref_T] is equal to a prespecifed HR (argument RR above)
To specify a frailty distribution, use GammaFrailty class for gamma frailty, PVFFrailty for other PVF family (a = 0.5 corresponds to inverse Gaussian, and a negative a, to compound Poisson)
The argument, constant, specified whether constant or average model will be used.

Reference:

