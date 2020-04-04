+++
date = "2019-03-09T2:28:40-04:00"
math = false
title = "Uncertainty quantification in CFD & Inflow velocity generation using GPUs"

[image]
  caption = ""
  focal_point = "Right"
+++

## Description
Uncertainties exist in CFD-based simulations of wind flow around structures and the associated loads. For instances, inflow uncertainty is associated with the inherent variability of atmospheric flows, while the model-form uncertainty could be induced by the mathematical approximation for the unresolved small-scale turbulent eddies. Those uncertainties could largely impact the predictive capabilities of quantities of interest (QoIs) through CFD analyses. Therefore, they need to be appropriately quantified and propagated into the aerodynamic load-response-design cycle.
{{< figure library="1" src="Picture5.jpg">}}

Therefore, the focus is on developing a strategy to enable inflow and model-form uncertainty to be quantified in a coupled fashion using surrogate modeling. Particularly, inflow uncertainty can be characterized as the probability density function of the inflow parameters. Model-form uncertainty is represented by the multi-fidelity CFD model discrepancy between Reynolds-averaged Navier- Stokes (RANS) and Large Eddy Simulation (LES). Based on the derived surrogate model, Monte Carlo simulation are conducted, from which the output statistics are obtained. Through this scheme, uncertainties are propagated to the QoIs of the building for aerodynamic design under uncertainty.
{{< figure library="1" src="Project3_2.jpg">}}

Generation of appropriate inflow boundary conditions satisfying prescribed statistical properties is essential for running a successful CFD simulation in a turbulent flow. Now with the advances in high-performance computing, parallel programming can be explored to generate turbulent velocity fields on the inlet patch by harnessing the power of the computer’s graphics process unit (GPU). The emergence of GPU programming has been applied to many high-performance applications including deep neural networks, image processing as well as CFD. In terms of inflow velocity generation, the time sequence of the velocity vector at each grid point on the inlet patch is computed by executing the kernel function on an allocated thread of a GPU. As a result, the entire inflow velocity field can be computed by running on thousands of threads in parallel. The proposed GPU programming in inflow generation has the promise to enhance the computational performance in orders of magnitude, and then being integrated into the real-time CFD simulation carried out using open-source software OpenFOAM. This technique can also be developed to facilitate real-time flow control through tuning inflow parameters or uncertainty quantification of inflow conditions in CFD analyses. 
{{< figure library="1" src="Picture6.jpg">}}
