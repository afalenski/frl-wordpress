---
ID: 2354
post_title: >
  FSK-ML (Food Safety Knowledge Markup
  Language)
author: FRL_Admin
post_date: 2017-09-06 09:10:55
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/fsk-ml-food-safety-knowledge-markup-language/
published: true
---
Food safety risk assessments, control of food production processes as well as the development of new food products are nowadays supported by application of mathematical modeling and data analysis techniques. This creates an increasing demand for resources facilitating the efficient, transparent and quality proven exchange of relevant information, e.g. analytical data, mathematical models, simulation setting as well as simulated data. For example, new parameterized microbial models are frequently made publicly available only in written mode via scientific publications. However, in order to apply these models to a given practical decision support question (e.g. on the growth/no-growth of a microorganism in a specific food matrix under given processing conditions) the interested end-user would have to re-implement the model based on information provided in a publication. Here it would be more efficient if those who create parameterized models could provide their model additionally as a file complying with a standardized file format that is also capable of transferring all relevant meta-information. Such a file could e.g. be provided as a supplement to the publication and could be read-in by the end user’s software tools (thus overcoming an error-prone re-implementation process).
The required standardized file format has been proposed in the “Predictive Modelling in Food Markup Language (PMF-ML) Software Developer Guide”. This document describes in detail how experimental data and mathematical models from the domain of predictive microbial modeling (and beyond) can be saved and encoded in a software independent manner. Here we further extend the PMF-ML format in order to enable in addition the exchange of knowledge / information that is embedded in specific script-based programming languages (e.g. “R”, Matlab, Python). I.e. the FSK-ML guidance document primarily aims at harmonizing the exchange of food safety knowledge (e.g. predictive models) including the associated meta-information where this knowledge is only available in a software-dependent format.
The FSK-ML format therefore relaxes and adapts certain specifications of the PMF-ML format while at the same time maintaining the highest possible synergies between both formats. This will also help to make sure that food safety models encoded in a software-independent manner (using PMF-ML) can easily be interpreted by FSK-ML import and export software functions in the future.

&nbsp;

The FSK Guidance Document:

<a href="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/09/FSK_guidance_document_20170823.pdf">FSK_guidance_document_20170823</a>