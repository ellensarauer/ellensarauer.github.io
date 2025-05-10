---
title: "Physics-informed Machine Learning-Based Cloud Microphysics Parameterization for Earth System Models"
collection: publications
category: manuscripts
permalink: /publication/sarauer-2024-eds-ml-microphysics
excerpt: 'Submitted manuscript on machine learning-based cloud microphysics parameterization for Earth system models.'
date: 2024-09-01
venue: 'Submitted to Environmental Data Science'
paperurl: ''
bibtexurl: ''
citation: 'Sarauer, E., Schwabe, M., Lauer, A., Stier, P., Weiss, P. and Eyring, V. (2024). "Physics-informed Machine Learning-Based Cloud Microphysics Parameterization for Earth System Models." <i>Submitted to Environmental Data Science</i>.'
---

We develop a cloud microphysics parameterization for the Icosahedral Non-hydrostatic modeling framework
(ICON) model based on physics-informed machine learning (ML). By training our ML model on high-resolution
simulation data, we enhance the representation of cloud microphysics in Earth System Models (ESMs) compared
to traditional parameterization schemes, in particular by considering the influence of high-resolution dynamics
that are not resolved in coarse ESMs. We run a global, kilometer-scale ICON simulation with a one-moment
cloud microphysics scheme, the complex graupel scheme, to generate 12 days of training data. Our ML approach
combines a microphysics trigger classifier and a regression model. The microphysics trigger classifier identifies
the grid cells where changes due to the cloud microphysical parameterization are expected. In those, the workflow
continues by calling the regression model and additionally includes physical constraints for mass positivity and
water mass conservation to ensure physical consistency. The microphysics trigger classifier achieves an F1 score
of 0.93 on classifying unseen grid cells. The regression model reaches an R2 score of 0.72 averaged over all seven
microphysical tendencies on simulated days used for validation only. This results in a combined offline performance
of 0.78. Using explainability techniques, we explore the correlations between input and output features, finding a
strong alignment with the graupel scheme and hence, physical understanding of cloud microphysical processes.
This parameterization provides the foundation to advance the representation of cloud microphysical processes in
climate models with ML, leading to more accurate climate projections and improved comprehension of the Earth’s
climate system
*Status: Submitted to* _Environmental Data Science_, *September 2024.*
