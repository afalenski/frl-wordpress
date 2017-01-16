---
ID: 1849
post_title: FSK-Lab
author: laval
post_date: 2017-01-16 18:58:01
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/fsk-lab/
published: true
---
FSK-Lab is an open-source extension plugin to the Konstanz Information Miner (<a href="https://knime.org">KNIME</a>). FSK-Lab enables KNIME users to work with FSK models within KNIME.
<h2>Installation</h2>
FSK Lab may be installed through its update site: Steps:
<h3>Installing KNIME</h3>
KNIME may be installed as described in <a href="https://tech.knime.org/installation-0">https://tech.knime.org/installation-0</a>

<iframe src="https://www.youtube-nocookie.com/embed/yeHblDxakLk?rel=0" width="560" height="315" frameborder="0" allowfullscreen="allowfullscreen" data-mce-fragment="1"></iframe>
<h3>Installing FSK-Lab</h3>
<div>FSK-Lab may be installed as a KNIME feature through the FSK-Lab update site <a href="https://dl.bintray.com/silebat/fsklab">https://dl.bintray.com/silebat/fsklab</a>. More info of installation of KNIME features through update sites at <a href="https://www.knime.org/downloads/update">https://www.knime.org/downloads/update</a>.</div>
<h3>Starting FSK-Lab for the first time</h3>
If FSK-Lab was installed successfully, the FSK-Lab feature should appear now in the KNIME Installation Details dialog under Help &gt; Installation Details.

<img src="https://silebat.github.io/FSK-Lab/installationDetails.png" />
<h2>FSK port object</h2>
Fsk-Lab provides an additional port object called <code>FskPortObject</code> that expresses in deep detail an FSK model. It is composed of:
<ul>
 	<li>Model script</li>
 	<li>Parameters script</li>
 	<li>Visualization script</li>
 	<li>Libraries used</li>
 	<li>R workspace</li>
 	<li>Model metadata</li>
</ul>
<img src="https://silebat.github.io/FSK-Lab/port.png" />
<h3>Model metadata</h3>
The model metadata involved in the FSK models comprises the following.
<table class="table table-condensed">
<thead>
<tr>
<th>Property</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>Model name</td>
<td>Free text</td>
</tr>
<tr>
<td>Model id</td>
<td>Free text</td>
</tr>
<tr>
<td>Model link</td>
<td>URL</td>
</tr>
<tr>
<td>Organism</td>
<td>Hazard name.</td>
</tr>
<tr>
<td>Organism details</td>
<td>Hazard details</td>
</tr>
<tr>
<td>Matrix</td>
<td>Compartment name</td>
</tr>
<tr>
<td>Matrix details</td>
<td>Compartment details</td>
</tr>
<tr>
<td>Creator</td>
<td>Person contributed to the encoding of the model in its present form by implementing the model in the software solution.</td>
</tr>
<tr>
<td>Family name</td>
<td>Model family</td>
</tr>
<tr>
<td>Contact</td>
<td>Contact information</td>
</tr>
<tr>
<td>Software</td>
<td><code>R</code> or <code>Matlab</code></td>
</tr>
<tr>
<td>Reference description</td>
<td>Free text</td>
</tr>
<tr>
<td>Reference description link</td>
<td>URL</td>
</tr>
<tr>
<td>Created date</td>
<td>Date upon which the model was created. Format: MM/dd/yyyy.</td>
</tr>
<tr>
<td>Modified date</td>
<td>Date of last modification to the model. Format: MM/dd/yyyy.</td>
</tr>
<tr>
<td>Rights</td>
<td>Information about rights held in and over the resource. Typically, rights information includes a statement about various property rights associated with the resource, including intellectual property rights.</td>
</tr>
<tr>
<td>Notes</td>
<td>Model notes</td>
</tr>
<tr>
<td>Curated</td>
<td>Boolean</td>
</tr>
<tr>
<td>Model type</td>
<td><code>Experimental data</code>, <code>Primary model with data</code>, <code>Primary model without data</code>, <code>Two step seconday model</code>, <code>One step secondary model</code>, <code>Manual secondary model</code>, <code>Two step tertiary model</code>, <code>One step tertiary model</code> or <code>Manual tertiary model</code></td>
</tr>
<tr>
<td>Model subject</td>
<td><code>unknown</code>, <code>growth</code>, <code>inactivation</code>, <code>survival</code>, <code>growth/inactivation</code>, <code>inactivation/survival</code>, <code>growth/survival</code>, <code>growth/inactivation/survival</code>, <code>T</code>, <code>pH</code>, <code>aw</code>, <code>T/pH</code>, <code>T/aw</code>, <code>pH/aw</code> or <code>T/pH/aw</code></td>
</tr>
<tr>
<td>Food process</td>
<td>Free text</td>
</tr>
<tr>
<td>Dependent variable</td>
<td></td>
</tr>
<tr>
<td>Independent variables</td>
<td></td>
</tr>
<tr>
<td>Has data</td>
<td>Boolean</td>
</tr>
</tbody>
</table>
<table class="table">
<thead>
<tr>
<th>Variable field</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td>Name</td>
<td>Variable name</td>
</tr>
<tr>
<td>Unit</td>
<td>Variable unit</td>
</tr>
<tr>
<td>Data type</td>
<td><code>character</code>, <code>integer</code>, <code>numeric</code> or <code>array</code></td>
</tr>
<tr>
<td>Value</td>
<td>Variable value</td>
</tr>
<tr>
<td>Minimum value</td>
<td></td>
</tr>
<tr>
<td>Maximum value</td>
<td></td>
</tr>
</tbody>
</table>
<h2>Included nodes</h2>
<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSKX Reader</h3>
</div>
<div class="panel-body">Reads an FSK object from an FSKX file. <img src="https://silebat.github.io/FSK-Lab/fskxreader.png" />
<ul>
 	<li>Inputs: None</li>
 	<li>Outputs: FSK object</li>
</ul>
Settings:
<ul>
 	<li>Location to file. May be an <i>absolute URL</i>, a <i>mountpoint relative URL</i> or <i>local path</i>.</li>
</ul>
Behaviour. Creates an FSK object with the scripts, metadata and libraries in the referred FSKX file.

</div>
</div>
<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSKX Writer</h3>
</div>
<div class="panel-body">Writes an FSK object into an FSKX file. <img src="https://silebat.github.io/FSK-Lab/fskxwriter.png" />
<ul>
 	<li>Inputs: FSK object</li>
 	<li>Outputs: none</li>
</ul>
Settings:
<ul>
 	<li>Location to file. May be an <i>absolute URL</i>, a <i>mountpoint relative URL</i> or a <i>local path</i>.</li>
</ul>
Behaviour. Creates an FSKX file with the scripts, metadata and libraries in the FSK object.

</div>
</div>
<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSK Creator</h3>
</div>
<div class="panel-body">Creates an FSK object. <img src="https://silebat.github.io/FSK-Lab/fskcreator.png" />
<ul>
 	<li>Inputs: none</li>
 	<li>Outputs: FSK object</li>
</ul>
Settings:
<ul>
 	<li>Location to model script (mandatory)</li>
 	<li>Location to parameters script (optional)</li>
 	<li>Location to visualization script (optional)</li>
 	<li>Location to XLSX file with metadata (optional)</li>
</ul>
Behaviour. Creates an FSK object with the script and metadata provided by the user.

</div>
</div>
<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSK Runner</h3>
</div>
<div class="panel-body">This node runs an FSK model <img src="https://silebat.github.io/FSK-Lab/fskrunner.png" />
<ul>
 	<li>Inputs: FSK object and optional metadata table</li>
 	<li>Outputs: FSK object and generated image</li>
</ul>
Behaviour. Runs the input model and updates its workspace with the model results. A chart or plot is generated if a visualization script is provided.

</div>
</div>
<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSK Metadata Editor</h3>
</div>
<div class="panel-body">Edit the metadata in an FSK object. <img src="https://silebat.github.io/FSK-Lab/fskmetadataeditor.png" />
<ul>
 	<li>Inputs: FSK object</li>
 	<li>Outputs: FSK object</li>
</ul>
Behaviour. Modifies the metadata in an FSK object.

</div>
</div>
<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSK to R</h3>
</div>
<div class="panel-body">Extracts the R workspace out of an FSK object. The R workspace may be used with KNIME R nodes. <img src="https://silebat.github.io/FSK-Lab/fsk2r.png" />
<ul>
 	<li>Inputs: FSK object</li>
 	<li>Output: RPortObject</li>
</ul>
Behaviour. Extracts the R workspace out of an FSK object and places it into the output RPortObject. If the R workspace is null or non-existent (as when the model has not been run), the generated RPortObject would be null.

</div>
</div>
<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSK to metadata</h3>
</div>
<div class="panel-body">Extracts metadata from an FSK object. <img src="https://silebat.github.io/FSK-Lab/fsk2metadata.png" />
<ul>
 	<li>Inputs: FSK object</li>
 	<li>Outputs: KNIME table with metadata</li>
</ul>
Behaviour. Extracts the metadata in an FSK object into a KNIME table

</div>
</div>