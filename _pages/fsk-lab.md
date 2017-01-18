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
<img class="size-full wp-image-1858 aligncenter" src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2015/02/FSKlab7-1.png" alt="FSK-Lab Logo" width="150" height="150" />

&nbsp;

FSK-Lab is an open-source extension plugin to the Konstanz Information Miner (<a href="https://knime.org">KNIME</a>). FSK-Lab enables KNIME users to work with FSK models within KNIME.
<h2>Installation</h2>
A running instance of KNIME is a prerequisite. It can be downloaded <a href="https://www.knime.org/downloads/overview">here</a> and installed following these <a href="https://tech.knime.org/installation-0">instructions</a>.
In addition, there is the option to modify the KNIME.ini in the installation folder of KNIME while the program is not running:</br>
1. In order to extend the RAM available in KNIME, simply change the value in the line '-Xmx1024m'. An example would be '-Xmx4g' if 4GB (=4x1024m) of 8GB RAM should be used.
2. If the connection to a KNIME-Server through KNIME fails, it might help to increase the response time. Simply add the line '-Dcom.knime.enterprise.client.connect-timeout=10000' to the ini-file. 

<h3>Installing FSK-Lab</h3>

<div>FSK-Lab needs to be installed as a KNIME feature through the FSK-Lab update site (<a href="https://www.knime.org/downloads/update">more info here</a>):</br>
1. Add the repository to KNIME via Help &gt; Install New Software &gt; Add. The corresponding URL (https://dl.bintray.com/silebat/fsklab) should to be entered in the 'Add Repository' dialogue along with a meaningful name.

<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSKlabinstall0.png" alt="" width="757" height="580" class="aligncenter size-full wp-image-1972" />

2. Now this repository can be selected in the installation menu via Help &gt; Install New Software &gt; 'Work with'-pull down menu.

<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSKlabinstall1.png" alt="" width="757" height="580" class="aligncenter size-full wp-image-1973" />

3. Tick FSK Lab nodes and follow the promts after pressing Next.</br>
4. After a reboot, FSK-Lab Feature should appear now in KNIME under Help &gt; Installation Details.</div>
<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSKlabinstall2-1.png" alt="" width="888" height="359" class="aligncenter size-full wp-image-1977" />

<h3>Installing R</h3>

<div>FSK-Lab is based on R (<a href="https://www.r-project.org" target="_blank">https://www.r-project.org</a>), which can also be installed as a KNIME feature through the FSK-Lab update site under WINDOWS (<a href="https://www.knime.org/downloads/update">more info here</a>). If you want to integrate your own R version or the one <a href="https://dl.bintray.com/silebat/FSK_example_models/R-3.3.0working.7z">used</a> by us, please continue with step 5 applying your R installation path:</br>

1. The R repository should be already available in the installation menu via Help &gt; Install New Software &gt; if All Available Sites is choosen in the 'Work with'-pull down menu.</br>
3. Fold open KNIME & Extensions and tick KNIME R Statistics Integration (Windows binarys).</br>
4. Follow the promts after pressing Next and after a reboot, the R binary feature should appear in KNIME under Help &gt; Installation Details.</br>
5. In this last step, KNIME needs to know were the R binarys are installed via File > Preferences. In the menu choose KNIME > BfR R settings and on the right site Browse to the local path of the binarys. If installed via the update site they are located in the KNIME installation folder > plugins > org.knime.ext.r3.bin.win32.x86_...R-Inst. Don't use a subfolder of R-Inst! Press Apply and enter the same path in the Menu under KNIME > R and press ok. HINT: If a seperate R version is used and the KNIME message 'no R.exe file found in the R-folder' appears, even if its there, the reason might be a wrong bit version was installed. The 32bit version can be found in the folder 'bin/i386' and the 64bit version in 'bin/x64'.  </br>
6. If you received a message that the package Rserve needs to be installed you need to start R.exe directly from its installation folder. In the R console enter "install.packages('Rserve')" and press enter. There should pop up a list of download sites than. Choose one nerby and confirm. After the message that the library was sucessfully downloaded, you can close are via "q()". In the library folder of R should a new folder Rserve appear now.</br>

 
 <h3>Example files</h3>
 
 <div>In order to test the FSK-Lab nodes in KNIME, there is a <a href="https://dl.bintray.com/silebat/FSK_example_models/example_models.zip">zip-file provided here</a>. It contains the needed files for a example models allowing to create FSKX-files by using the FSKX-Creator-node in KNIME. Please, make sure to assign the corresponding files in the configuration dialogue of the Creator-node.
 </div>
 
 
  
 <h2>Details on FSK-Lab</h2> 
<h3>FSK port object</h3>
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
<div class="panel-body">

Reads an FSK object from an FSKX file. <img src="https://silebat.github.io/FSK-Lab/fskxreader.png" />
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
<div class="panel-body">

Writes an FSK object into an FSKX file. <img src="https://silebat.github.io/FSK-Lab/fskxwriter.png" />
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
<div class="panel-body">

Creates an FSK object. <img src="https://silebat.github.io/FSK-Lab/fskcreator.png" />
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
<div class="panel-body">

This node runs an FSK model <img src="https://silebat.github.io/FSK-Lab/fskrunner.png" />
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
<div class="panel-body">

Edit the metadata in an FSK object. <img src="https://silebat.github.io/FSK-Lab/fskmetadataeditor.png" />
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
<div class="panel-body">

Extracts the R workspace out of an FSK object. The R workspace may be used with KNIME R nodes. <img src="https://silebat.github.io/FSK-Lab/fsk2r.png" />
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
<div class="panel-body">

Extracts metadata from an FSK object. <img src="https://silebat.github.io/FSK-Lab/fsk2metadata.png" />
<ul>
 	<li>Inputs: FSK object</li>
 	<li>Outputs: KNIME table with metadata</li>
</ul>
Behaviour. Extracts the metadata in an FSK object into a KNIME table

</div>
</div>