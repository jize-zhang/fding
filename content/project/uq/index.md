+++
date = "2019-03-09T2:28:40-04:00"
math = false
title = "Inflow uncertainty quantification using GPU programming"

[image]
  caption = ""
  focal_point = "Right"
+++

## Description
Uncertainties exist in CFD-based simulations of wind flow around structures and the associated loads. For instances, inflow uncertainty is associated with the inherent variability of atmospheric flows, while the model-form uncertainty could be induced by the mathematical approximation for the unresolved small-scale turbulent eddies. Those uncertainties could largely impact the predictive capabilities of quantities of interest (QoIs) through CFD analyses. Therefore, they need to be appropriately quantified and propagated into the aerodynamic load-response-design cycle.
{{< figure library="1" src="Picture5.jpg">}}

In particular, parallel programming has been explored to generate random velocity fields on the inflow boundary by harnessing the power of the computer's graphics process unit (GPU). The time sequences of the velocity vector at each
grid point on the inflow boundary can be computed by executing the kernel function on an allocated thread of a GPU. Consequently, the entire inflow velocity field can be computed by running on thousands of threads in parallel. In comparison to the traditional data processing pipeline that involves the use of a single or multiple CPU processor(s) for inflow velocity generation, GPU programming has proven to speed up data processing in orders of magnitude.
{{< figure library="1" src="Picture6.jpg">}}
