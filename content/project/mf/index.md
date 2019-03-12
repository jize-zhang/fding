+++
date = "2019-03-11T2:27:40-04:00"
math = false
summary = "Multi-fidelity surrogate modeling and sequential surrogate model updating"
title = "Multi-fidelity surrogate modeling and sequential surrogate model updating"

[image]
  caption = ""
  focal_point = "Right"
+++

{{< figure library="1" src="Picture3.jpg">}}

## Description
The success of using surrogate models largely depends upon the accuracy of the simulation data that are used for model calibration. In the context of CFD simulations, two fundamental approaches in numerically capturing the complexity of massively separated high Reynolds flows around structures are Reynolds-averaged Navier-Stokes (RANS) and Large Eddy simulation (LES). The high-fidelity CFD analyses such as LES preform considerably better than RANS as they resolve the large-scale turbulence and only require modeling of the small-scale one. However their high computational cost allows only a small sample size to be generated at the computational budget of RANS samples. This makes it difficult to construct a reliable surrogate model solely based on high-fidelity model like LES. 
Multi-fidelity approaches that utilize hierarchical surrogate models relating low-fidelity (RANS) to high-fidelity (LES) models are emerging as an attractive avenue in obtaining high quality surrogate prediction with a computational effort comparable to RANS. 

Another challenge regarding the validation of the adequacy of the simulated data lies in the modeling of multi-fidelity surrogates. If the data is insufficient for surrogate model calibration, new CFD simulations should be conducted, which is referred to as sequential design.
Sequential sampling can be applied both globally and locally. The goal of global sampling over the entire design space is to reduce the overall prediction error and thus to enhance the global accuracy of the surrogate model. The local exploitation of the surrogate model by confining the positions of the infill points at the regions of interest, e.g., local minimum or maximum regions, aims at driving a more accurate search towards optimization. Furthermore, it would be computationally efficient if sequential sampling has the capability of generating multiple infill points for each cycle of surrogate model updating in order to make full use of the computational resources. In view of the above challenges, a parallel sequential sampling scheme containing those two phases of model updating has been developed in our study.
