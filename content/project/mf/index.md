+++
date = "2019-03-10T2:27:40-04:00"
math = false
title = "Multi-fidelity surrogate modeling and sequential surrogate model updating"

[image]
  caption = ""
  focal_point = "Right"
+++

{{< figure library="1" src="Project2.jpg">}}

## Description
The success of using surrogate models largely depends upon the accuracy of the simulation data that are used for model calibration. In the context of CFD simulations, two fundamental approaches in numerically capturing the complexity of massively separated high Reynolds flows around structures are Reynolds-averaged Navier-Stokes (RANS) and Large Eddy simulation (LES). The high-fidelity CFD analyses such as LES preform considerably better than RANS as they resolve the large-scale turbulence and only require modeling of the small-scale one. However their high computational cost allows only a small sample size to be generated at the computational budget of RANS samples. This makes it difficult to construct a reliable surrogate model solely based on high-fidelity model like LES. 
Multi-fidelity approaches that utilize hierarchical surrogate models relating low-fidelity (RANS) to high-fidelity (LES) models are emerging as an attractive avenue in obtaining high quality surrogate prediction with a computational effort comparable to RANS. 


