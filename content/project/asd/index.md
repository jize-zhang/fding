+++
date = "2019-03-11T2:27:40-04:00"
math = false
title = "CFD-enabled static form design of structures"

[image]
  caption = ""
  focal_point = "Right"
+++

{{< figure library="1" src="Project1_1.jpg">}}
{{< figure library="1" src="Project1_2.jpg">}}

## Description
Before moving to design of dynamic façade of the building, my initial research focused on aerodynamic shape tailoring of structures using computational fluid dynamics (CFD) and machine learning techniques.

Current trend in building design worldwide has been to build increasingly taller, elegant and complex structures. These buildings face many challenges due to their height and performance-oriented design objectives. Specifically, these slender structures are highly sensitive to wind-induced effects. 

The external envelope of a civil structure plays a particularly important role in determining the entity of its wind-induced loads. Therefore, a creative tailoring of the external geometry can benefit in reducing the magnitude of the governing wind loads and structural motions. In digital age with burgeoning growth in computational resources and parallel advances in CFD, computational simulations are evolving with a promise of becoming versatile, convenient and reliable means of assessing wind load effects. 

I have developed a computational platform for the aerodynamic shape tailoring of the structure. Relationship between the shape variation of the cross section of the building and its aerodynamic characteristics is systematically investigated through this digital design platform. One concern is the significant computational challenge posed by the multiple CFD simulations involved in the shape optimization process. One remedy is to use surrogate models that can replace computationally prohibitive simulations with computationally tractable approximate models.

A surrogate model is built based on regression against the limited set of observations from simulations. CFD is employed to evaluate the aerodynamic objectives on buildings with sampled geometric profiles. The response surfaces of the surrogate models are used to emulate the original CFD simulations to inform optimization that will guide the search of the optimal geometric configurations.
