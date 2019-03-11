+++
date = "2019-03-11T2:27:40-04:00"
math = false
summary = "Computational fact checking from knowledge networks"
tags = ["dbpedia", "fact-checking"]
title = "Computational Fact-checking"

[image]
  caption = ""
  focal_point = "Center"
+++

## Description
Numerical advances in storm surge prediction over the past couple of decades have produced high-fidelity simulation models that permit a detailed representation of hydrodynamic processes and therefore support high-accuracy forecasting. Unfortunately, the computational burden of such numerical models is large, requiring thousands of CPU hours for each simulation,
something that limits their applicability for emergency response management and hurricane risk assessment. During landfalling events such models can only be utilized to provide a small number of high-fidelity, deterministic predictions, but cannot support thousand-run ensembles to examine the impact of forecasting errors in the predicted track or provide fast prediction updates once the new storm track information becomes available. Their implementation for regional hurricane risk assessment faces similar challenges.

The use of interpolation methodologies and metamodels (Irish, Resio et al. 2009;
Das, Jung et al. 2010; Jia and Taflanidis 2013; Taflanidis, Kennedy et al. 2013; Kim,
Melby et al. 2015) has been examined to address the aforementioned challenge. These
approaches can provide fast predictions using a database of high-fidelity, synthetic
storms, with the goal of maintaining the accuracy of the numerical model utilized to
produce this database, while providing greatly enhanced computational efficiency.
Leveraging this efficiency they can support emergency response management (Smith,
Westerink et al. 2011) and comprehensive risk assessment (Resio, Irish et al. 2009).
Relevant efforts are further promoted by the fact that various such databases are
constantly created and updated for regional flooding and coastal hazard studies
(Niedoroda, Resio et al. 2010; Kennedy, Westerink et al. 2012; USACE 2015). Kriging
has been demonstrated in a number of studies (Jia and Taflanidis 2013; Jia, Taflanidis et
al. 2015; Rohmer, Lecacheux et al. 2016) to offer great versatility as a surrogate model in
this context: it has provided high-accuracy predictions for both storm surge and waves
17
and for either peak or time-series responses, has been efficiently applied for databases of
different sizes and characteristics, and has been utilized to provide predictions over large
coastal regions, with thousands of save points for which the storm response needs to be
evaluated. For enhanced computational efficiency for the latter type of implementation,
combination with principal component analysis as a dimension reduction technique has
been advocated (Jia and Taflanidis 2013). 

Important topics we explored in this project include: 

(a) the adaptive selection of synthetic storms for creating the database that will inform the surrogate model development [existing databases are typically established with the joint
probability optimal with sampling (JPM-OS) method or with orthogonal DoE; 

(b) adjustments to support two implementation issues that might become more relevant due to climate change considerations: including the prediction for intensified storms exceeding all available ones in initial synthetic-storm database (which
unavoidably requires implementation for extrapolating predictions), and the surge estimation for sea level rise (SLR) scenarios.

## Software

* [Knowledge Linker <sup><i class="fas fa-external-link-alt"></i></sup>](//github.com/glciampaglia/knowledge_linker)
* [Knowledge Stream <sup><i class="fas fa-external-link-alt"></i></sup>](//github.com/shiralkarprashant/knowledgestream)
* [RelSifter <sup><i class="fas fa-external-link-alt"></i></sup>](//github.com/shiralkarprashant/samphire), aka the Samphire Triple Scorer at the [2017 WSDM Cup](//wsdm-cup-2017.org).
