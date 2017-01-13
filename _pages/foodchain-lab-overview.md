---
ID: 584
post_title: FoodChain-Lab Introduction
author: FRL_Admin
post_date: 2015-03-05 14:12:17
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/foodchain-lab-overview/
published: true
---
<h4>FoodChain-Lab Concepts 1</h4>
<ul>
<li><b>Delivery</b>: Something send from A to B at a certain date. A delivery can have preceding and subsequent deliveries (e.g. strawberry-delivery -> strawberry-cake-delivery).</li>
<li><b>Station</b>: Any food business operator, that sends and/or receives deliveries.</li>
<li><b>Trace</b>: The path a contamination can take. A station/delivery "B" is on the <b>forward trace</b> of a station/delivery "A", if a contamination at "A" can spread to "B" via the food chain network. If "B" is on the <b>forward trace</b> of "A", then "A" is on the <b>backward trace</b> of "B".</li>
</ul>
<h4>FoodChain-Lab Concepts 2</h4>
<ul>
<li><b>Weight</b>: Weights are assigned to stations/deliveries, that are involved in an outbreak (e.g. a restaurant where customers got sick). Different weights can be used to model differences between involved stations/deliveries (e.g. higher weight = higher likelihood that station is involved)..</li>
<li><b>Cross Contamination</b>: When it is applied at a station, its incoming deliveries contaminate its outgoing deliveries. When applied on delivery level, the selected incoming deliveries of station contaminate each others subsequent deliveries.</li>
<li><b>Kill Contamination</b>: When it is applied at a station/delivery, the contamination is killed there. That means it does not spread to subsequent stations/deliveries.</li>
<li><b>Score</b>: Is computed based on given weights and cross contamination. Should help to estimate the likelihood that a certain station is the origin of the outbreak (higher score = more/higher weighted stations on forward trace).</li>
</ul>
<h4>FoodChain-Lab Score Computation 1</h4>
<ul>
<li>s<sub>i</sub> is the i-th station or delivery</li>
<li>w<sub>j</sub> is the weight of the j-th station or delivery</li>
<li>t<sub>ij</sub> has a value of 1, if there is a trace from s<sub>i</sub> to s<sub>j</sub> and a value of 0 otherwise</li>
<li>n is the total number of stations and deliveries</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/score.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/score.png"/></a>
<h4>FoodChain-Lab Score Computation 2</h4>
<ul>
<li>FoodChain-Lab also allows to assign negative weights to stations/deliveries.</li>
<li>A negative weight should indicate, that a station/delivery is not involved in the outbreak.</li>
<li>When negative weights are used, the score computation changes to this formula.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/new_score.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/new_score.png"/></a>
<h4>Introduction to KNIME</h4>
<ul>
<li>KNIME is an open source data analytics platform, that allows users to assemble a data pipeline called "workflow".</li>
<li>A workflow is built by dragging nodes from the <b>Node Repository</b> onto the <b>Workflow Editor</b> and connecting them (<a href="https://tech.knime.org/workbench" target="_blank">https://tech.knime.org/workbench</a>).</li>
<li>Nodes are processing units with input- and/or output ports.</li>
<li>Data is transferred over a connection from an out-port to the in-port of another node.</li>
<li>A comprehensive KNIME quickstart guide can be found at <a href="https://tech.knime.org/files/KNIME_quickstart.pdf" target="_blank">https://tech.knime.org/files/KNIME_qu...</a>.</li>
<li>An introduction video is available at <a href="https://www.youtube.com/watch?v=ft7Ksgss3Tc" target="_blank">https://www.youtube.com/watch?v=ft7Ks...</a>.</li>
</ul>
<h4>Available Nodes</h4>
<ul>
<li>Detailed descriptions of all nodes are available in the <b>Node Description</b> view of the KNIME workbench (<a href="https://tech.knime.org/workbench" target="_blank">https://tech.knime.org/workbench</a>).</li>
<li>All inputs and outputs are either <b>data tables</b> (triangles) or <b>images</b> (green square). Therefore standard KNIME nodes (<b>Row Filter</b>, <b>Image Port Writer</b>, ...) can be used in FoodChain-Lab workflows.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/1.png"/></a>
<h4>Tracing</h4>
<ul>
<li>Supply chain data is read from the internal database via the <b>Supply Chain Reader</b>.</li>
<li>This data can be visualized with the <b>Tracing View</b>. The <b>Tracing View</b> also allows to perform a tracing on the data.</li>
<li>The <b>Tracing</b> node performs tracing without visualization. Its output can be used in the <b>Tracing View</b> (e.g. to perform some tracings as a preprocessing step)</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/2.png"/></a>
<h4>Using GIS data</h4>
<ul>
<li>The <b>Geocoding</b> node allows to acquire latitude/longitude data from addresses.</li>
<li>This data can be geographically clustered with the <b>GIS Cluster</b> node.</li>
<li>The <b>Tracing View</b> allows geographical visualization, if GIS data is provided from the <b>Shapefile Reader</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/3.png"/></a>