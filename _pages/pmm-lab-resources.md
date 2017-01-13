---
ID: 906
post_title: PMM-Lab Resources
author: FRL_Admin
post_date: 2015-03-30 14:15:45
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/pmm-lab-resources/
published: true
---
<a href="#Sample Workflows">Sample Workflows</a>
<a href="#Microbiological data for model fitting">Microbiological data for model fitting</a>
<a href="#formula notation">Formula notation</a>
<a href="#curve fitting">Curve fitting</a>
<a href="#model selection">Model selection</a>

<h4 id="Sample Workflows">Sample Workflows</h4>
When the installation of PMM-Lab is finished we suggest to start working with the program by downloading our <a class="" href="http://sourceforge.net/projects/pmmlab/files/workflows">sample workflows</a> for primary and secondary model estimation.

After downloading you can import them one by one via:
File -&gt; Import Knime Workflows -&gt; Select archive file -&gt; browse ... -&gt; Finish;

You find the workflow in the KNIME Explorer Window under "LOCAL (Local Workspace)". By double clicking the selected workflow will be opened and you can execute / modify / play with it.

If you would like to extend these workflows you can use all nodes from the node library in the Node Repository. There also the PMM-Lab node repository is located.

<h4 id="Microbiological data for model fitting">Microbiological data for model fitting</h4>
A popular online resource for microbial data is the <a class="" href="http://www.combase.cc" rel="nofollow">ComBase</a>. It comprises a plethora of growth and inactivation data and PMM-Lab provides a compatibility layer that lets you import and export files formatted in the way they are offered by ComBase. The 'ComBase Reader' and the 'ComBase Writer' nodes accomplish these tasks.

In scientific literature results of microbial growth, survival or inactivation experiments are described heterogeneously in different units. In some cases it is impossible to transform this data to a more standardized unit lateron, like e.g. log10(CFU/g) or log10(CFU/ml).
In PMM-Lab the data model defines cell concentration the way that the cell/virus concentration is represented in log10(cells/CFU/units/vp/pfu per g) or log10(cells/CFU/units/vp/pfu per ml) (decadic logarithm). Time is always represented in hours.

This treatment of units has been selected to be consistent with the data handling in the ComBase as documented in a <a class="" href="http://www.combase.cc/index.php/en/downloads/file/9-tutorial-for-submitting-data-to-combase" rel="nofollow">Tutorial for submitting data to ComBase</a>.

<a href="#top">Go to top</a>

<h4 id="formula notation">Formula notation</h4>
PMM-Lab comes with a number of preset formulas that you can deploy right away. You may, however, want to create your own models. The node "Model Creator" gives you the possibility to create and edit model formulas inside PMM-Lab. For these formulas PMM-Lab uses infix notation and a number of common math functions are available. You may use
<ul>
	<li>sqrt(<em>x</em>) to calculate the square root of the expression <em>x</em></li>
	<li>...</li>
</ul>
An important part of PMM-Lab formula notation is the disambiguation of the logarithm function. In contrast to other programming languages, in PMM-Lab, the function log(<em>x</em>) refers to the decadic logarithm. To avoid ambituity among the various logarithm functions, you may prefer to use the functions ln(<em>x</em>) for the natural logarithm with base <em>e</em> and log10(<em>x</em>) to refer to the decadic logarithm.

In your formulas you can also use conditional operators. For example

<em>t</em>&lt;=1

evaluates 1 if t is smaller or equals 1 whereas it evaluates 0 otherwise. You may use the following operators accordingly:
<ul>
	<li>\&lt;</li>
	<li>&gt;</li>
	<li>\&lt;=</li>
	<li>&gt;=</li>
	<li>&amp;&amp;</li>
	<li>||</li>
</ul>

<strong id="initialization-range-of-formula-parameters">Initialization range of formula parameters</strong>
For each parameter in a formula you can impose an initialization range. This range will be used for initializing the algorithm that tries to find the optimal parameter set. It is not mandatory that the actual parameters lie within this range. You will, however, be notified if estimated parameters lie outside their initial definition range.

<a href="#top">Go to top</a>
<h4 id="curve fitting">Curve fitting</h4>
Curve fitting is a central aspect of PMM-Lab. In this section we will present, in what kind of use cases you may want to fit a curve and how to accomplish that. Furthermore, we will introduce, how the fitted models can be further processed and how to visualize the obtained results.

<strong id="use-cases">Use cases</strong>
There are two distinct scenarios in which you might want to fit a curve.
<ul>
	<li>Given a microbial data set, you want to derive a model that approximates the tenacity behavior under just the same conditions that gave rise to this data set.</li>
	<li>Given the model parameters derived under a variety of conditions, you want to derive a model that approximates the value of the model parameters dependent on these conditions.</li>
</ul>
While the first scenario describes the estimation of a <em>Primary Model</em>, the latter scenario represents a <em>Secondary Model</em>. We will refer to these two concepts quite frequently. Hence, its understanding is paramount for the upcoming discussion.

<strong id="primary-model-fitting">Primary Model Fitting</strong>
<img src="https://sourceforge.net/p/pmmlab/wiki/Fitting/attachment/primary_view_small.jpg" alt="Fitted primary model curve in PMM-Lab view" />

In Primary Model Fitting, we consider bacterial growth or inactivation as the concentration of a bacterial agent dependent on the time. So

<em>t -&gt; log10(C)</em>

In PMM-Lab this mapping is implemented as a function dependent on a set of parameters <em><strong>p</strong></em>. Hence,

<em>log10(C)=f(t|<strong>p</strong>)</em>

It is the goal of the Fitting process to derive a realization of the parameter set <em><strong>p</strong></em> that approximates a given data set <em>D</em> as accurately as possible. Consequently, the fitting of a Primary Model consumes a microbial data set <em>D</em> and outputs a set of parameters <em><strong>p</strong></em>, the primary model.

<strong id="secondary-model-fitting">Secondary Model Fitting</strong>
<img src="https://sourceforge.net/p/pmmlab/wiki/Fitting/attachment/secondary_view_small.jpg" alt="Fitted secondary model curve in PMM-Lab view" />

In Secondary Model Fitting, we assume that bacterial kinetics depend on the environmental conditions <em><strong>e</strong></em> under which the original experiment has been conducted. So

<em><strong>e</strong> -&gt; <strong>p</strong></em>

In PMM-Lab, a model that implements this mapping also depends on a set of parameters <em><strong>s</strong></em>. Hence,

<em><strong>p</strong>=f(<strong>e</strong>|<strong>s</strong>)</em>

So, in Secondary Model Fitting we try to find a parameter set <em><strong>s</strong></em> that approximates the parameters for a primary model as accurately as possible for given environmental conditions. Consequently Secondary Model Fitting consumes examples of environmental conditions <em><strong>e</strong></em> and the primary model parameters <em><strong>p</strong></em> associated to them, and produces a set of secondary parameters <em><strong>s</strong></em>.

<strong id="curve-fitting-in-pmm-lab">Curve fitting in PMM-Lab</strong>
In PMM-Lab, both Primary and Secondary Model Fitting are performed by a single KNIME node called "Model Fitting". The node knows, when to perform what from the KNIME table presented to it. If given a combination of a Microbial Data Set and a Primary Model Formulas, it performs a Primary Model fit. If presented a combination of fitted Primary Models and Secondary Models, if performs a Secondary model fit.

<a href="#top">Go to top</a>

<h4 id="model selection">Model selection</h4>
In PMM-Lab, it is possible to fit several models to the same data set. The advantage of this approach is the fact that one can choose the most appropriate model for the data set at hand. Models differ in their theoretical foundation, complexity, their robustness and their ease of interpretation. It is the researcher's responsibility to choose the model as a compromise according to the aforementioned aspects. This task is generally referred to as model selection.

PMM-Lab provides several measures with which the researcher can quantify the performance of his model.
<ul>
	<a href="#root-mean-square">Root Mean Square (RMS)</a>
	<a href="#statistic-coefficient-of-determination">Statistic coefficient of determination R<sup>2</sup></a>
	<a href="#akaike-information-criterion">Akaike Information Criterion (AIC)</a>
</ul>
The former two measures only quantify the error with respect to the training data set. The latter as well considers model complexity. I.e. simple models are preferred in favor of complex ones.

<strong id="root-mean-square">Root Mean Square</strong>
The Root Mean Square (RMS) error is a measure for the difference between a data set and a corresponding fit. The RMS asymptotically converges to the standard deviation from the model's predicted value for sufficiently large sizes of data sets.

<strong id="statistic-coefficient-of-determination">Statistic coefficient of determination</strong>
The R<sup>2</sup> value or statistical coefficient of determination is a measure for how well a regression model is capable of describing a data set. The R<sup>2</sup> does not explicitly consider model complexity. Its definintion range is (-inf,1]. Where 1 is a perfect fit while 0 is equivalent to the fit of an uninformed model that plainly predicts the expectation value of the dependent variable and is ignorant with respect to the independent variables. Hence, a model, that performs with an R<sup>2</sup> &lt; 0 is expected to lose information on observation of the set of dependent variables instead of gaining. This situation is, of course, undesirable.

<strong id="akaike-information-criterion">Akaike Information Criterion</strong>
Similarly to the BIC, the Akaike Information Criterion (AIC) describes the goodness of fit for a model with respect to model complexity. Penalty for complexity in the AIC is less severe than in BIC, thereby emphasizing accuracy over simplicity in comparison with the BIC.

<strong id="formulas">Formulas</strong>
Formulas used in PMM-Lab:
<img src="https://sourceforge.net/p/pmmlab/wiki/Model%20selection/attachment/formulas.png" alt="Formulas" />
<a href="#top">Go to top</a>