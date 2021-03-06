---
ID: 1845
post_title: FSK-Lab
author: laval
post_date: 2017-01-16 18:54:03
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/fsk-lab_de/
published: true
---
<img class="size-full wp-image-1858 aligncenter" src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2015/02/FSKlab7-1.png" alt="FSK-Lab Logo" width="150" height="150" />

&nbsp;

FSK-Lab is an open-source extension plugin to the Konstanz Information Miner (<a href="https://knime.org" target="_blank">KNIME</a>). FSK-Lab enables KNIME users to work with FSK models within KNIME.
<h2>Installation</h2>
<h3>Installing KNIME</h3>
A running instance of KNIME is a prerequisite. It can be downloaded <a href="https://www.knime.org/downloads/overview" target="_blank">here.</a> Due to avoid installing issues under WINDOWS, the provided zip-version should be used and unzipped then. The KNIME folder itself can be placed and run from anywhere under Windows without admin rights. After starting KNIME, the user will be asked to create the KNIME-WORKSPACE, were all the workflows will be stored. After restarting KNIME, please make sure to select the right one to access your files (it will be preselected). </br>HINT: In order to avoid later issues, never copy the KNIME_WORKSPACE, import it only!</br>

Please following these <a href="https://tech.knime.org/installation-0" target="_blank">instructions</a> to get further instructions how to install knime .
In addition, there is the option to modify the KNIME.ini in the installation folder of KNIME while the program is not running:</br>
1. The amount of RAM available in KNIME might be extended by changing the value in the line '-Xmx1024m'. An example would be '-Xmx4g', if 4GB (=4x1024m) of 8GB RAM should be used.</br>
2. If the connection to a KNIME-Server through KNIME fails, it might help to increase the response time. Simply add the line '-Dcom.knime.enterprise.client.connect-timeout=10000' to the ini-file. 

<h3>Installing FSK-Lab</h3>

<div>FSK-Lab needs to be installed as a KNIME feature through the FSK-Lab update site (<a href="https://www.knime.org/downloads/update" target="_blank">more info here</a>):</br>
1. Add the repository to KNIME via Help &gt; Install New Software &gt; Add. The corresponding URL (https://dl.bintray.com/silebat/fsklab) should be entered in the 'Add Repository' dialogue along with a meaningful name.

<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSKlabinstall0.png" alt="" width="757" height="580" class="aligncenter size-full wp-image-1972" />

2. Now this repository can be selected in the installation menu via Help &gt; Install New Software &gt; 'Work with'-pull down menu. Tick 'FSK Lab Feature' and follow the prompts after pressing Next.</br>

<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSKlabinstall1.png" alt="" width="757" height="580" class="aligncenter size-full wp-image-1973" />


3. After restarting KNIME, FSK-Lab Feature should appear now in KNIME under Help &gt; Installation Details.</div>
<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSKlabinstall2-1.png" alt="" width="888" height="359" class="aligncenter size-full wp-image-1977" />

<h3>Installing R</h3>

<div>FSK-Lab is based on R (<a href="https://www.r-project.org" target="_blank">https://www.r-project.org</a>), which can also be installed as a KNIME feature through the FSK-Lab update site under WINDOWS (<a href="https://www.knime.org/downloads/update" target="_blank">more info here</a>). If you want to integrate your own R version or the one <a href="https://dl.bintray.com/silebat/FSK_example_models/R-3.3.0working.7z">used</a> by us, please continue with step 5 applying your R installation path:</br>

1. The R repository should be already available in the installation menu via Help &gt; Install New Software &gt; if All Available Sites is chosen in the 'Work with'-pull down menu.</br>
2. Fold open KNIME & Extensions and tick KNIME R Statistics Integration (Windows binarys).

<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/R_install.png" alt="" width="930" height="579" class="aligncenter size-full wp-image-1988" />

3. Follow the prompts after pressing Next and after a reboot, the R binary feature should appear in KNIME under Help &gt; Installation Details.</br>
4. In this last step, KNIME needs to know were the R binarys are installed via File > Preferences. In the menu choose KNIME > BfR R settings and on the right site browse to the local path of the binarys. If installed via the update site they are located in the KNIME installation folder > plugins > org.knime.ext.r3.bin.win32.x86_...R-Inst. Don't use a subfolder of R-Inst! Press Apply and enter the same path in the Menu under KNIME > R and press ok.</br>HINT1: If a seperate R version is used and the KNIME message 'no R.exe file found in the R-folder' appears, even if its there, the reason might be a wrong bit version was installed. The 32bit version should be present in the subfolder 'bin/i386' and the 64bit version in 'bin/x64'.</br>HINT2: The 'BfR R settings' exists only for the use along with FSK-Lab and in parallel to the regular'R'-setting of KNIME. This allows to use different R folders/versions if needed.</br>

<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/R.png" alt="" width="622" height="419" class="aligncenter size-full wp-image-1979" />

5. If you received a message that the package Rserve needs to be installed you need to start R.exe directly from its installation folder. In the R console enter "install.packages('Rserve')" and press enter. There should pop up a list of download sites then. Choose one nearby and confirm. After the message that the library was sucessfully downloaded, you can close it via "q()". In the library folder of R should a new folder Rserve appear now.

<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/Rserve.png" alt="" width="627" height="248" class="aligncenter size-full wp-image-1982" />
 

<h3>Installing R on MacOS</h3>

For R running in MACOS, there is a specific R version for MacOS required which may be <a href="http://mirrors.dotsrc.org/cran/" target="_blank">downloaded from here</a>.
FSK-Lab requires the R packages: 'Rserve', 'miniCRAN' and 'Cairo', which may be installed with the install.packages() command within the R-console:

install.packages('Rserve')
install.packages('miniCRAN')
install.packages('Cairo')

Besides these three packages, MacOS requires also the XQuartz software which can be obtained at <a href="http://xquartz.macosforge.org">http://xquartz.macosforge.org</a>.

The path to the R folder to be entered in KNIME (as described for WINDOWS) should be:</br>
/Library/Frameworks/R.framework/Resources/

<h3>Installing R on Linux (UBUNTU)</h3>

First, Linux requires some development libraries for the R packages which can be installed through the apt-get command in the console under UBUNTU via: </br>
sudo apt-get install libcurl4-openssl-dev libssl-dev libxml2-dev

The R-binarys may be also installed via apt-get:</br>
sudo apt-get install r-base

In order to install the R packages for FSKlab, please make sure to start R in the UBUNTU console with the sudo command to avoid writing right problems:</br>
sudo R

The R packages 'Rserve' and 'miniCRAN' are required, which may be installed with the install.packages() command within the R-console: </br>
install.packages('Rserve')
install.packages('miniCRAN')



The path to the R folder to be entered in KNIME (as described for WINDOWS) should be: </br>
/usr/lib/R

 <h3>Example files</h3>
 
 <div>In order to test the FSK-Lab nodes in KNIME, there is a <a href="https://dl.bintray.com/silebat/FSK_example_models/example_models.zip">zip-file provided here</a>. It contains the needed files to create FSKX-model-files by using the FSKX-Creator-node in KNIME. Please, make sure to assign the corresponding files in the configuration dialogue of the Creator-node.
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
<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSK_Creator_node.png" alt="" width="123" height="122" class="alignleft size-full wp-image-2004" />
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
<h3 class="panel-title">FSK Creator</h3>
</div>
<div class="panel-body">

Creates an FSK object.</br>
<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSK_Creator_node.png" alt="" width="123" height="122" class="alignnone size-full wp-image-2004" /></br>
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
Behaviour: Creates an FSK object with the script and metadata provided by the user.

</div>
</div>
<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSKX Writer</h3>
</div>
<div class="panel-body">

Writes an FSK object into an FSKX file.</br>
<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSK_FSKX_Writer_node.png" alt="" width="120" height="121" class="alignnone size-full wp-image-2009" /></br>
<ul>
 	<li>Inputs: FSK object</li>
 	<li>Outputs: none</li>
</ul>
Settings:
<ul>
 	<li>Location to file. May be an <i>absolute URL</i>, a <i>mountpoint relative URL</i> or a <i>local path</i>.</li>
</ul>
Behaviour: Creates an FSKX file with the scripts, metadata and libraries in the FSK object.

</div>
</div>

<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSKX Reader</h3>
</div>
<div class="panel-body">

Reads an FSK object from an FSKX file.</br> 
<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSK_FSKX_Reader_node.png" alt="" width="121" height="122" class="alignnone size-full wp-image-2010" /></br>
<ul>
 	<li>Inputs: None</li>
 	<li>Outputs: FSK object</li>
</ul>
Settings:
<ul>
 	<li>Location to file. May be an <i>absolute URL</i>, a <i>mountpoint relative URL</i> or <i>local path</i>.</li>
</ul>
Behaviour: Creates an FSK object with the scripts, metadata and libraries in the referred FSKX file.

</div>
</div>


<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSK Runner</h3>
</div>
<div class="panel-body">

This node runs an FSK model</br>
<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSK_Runner_node.png" alt="" width="122" height="121" class="alignnone size-full wp-image-2015" /></br>
<ul>
 	<li>Inputs: FSK object and optional metadata table</li>
 	<li>Outputs: FSK object and generated image</li>
</ul>
Behaviour: Runs the input model and updates its workspace with the model results. A chart or plot is generated if a visualization script is provided.

</div>
</div>
<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSK Metadata Editor</h3>
</div>
<div class="panel-body">

Edit the metadata in an FSK object.</br>
<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSK_Metadata_Editor_node.png" alt="" width="127" height="119" class="alignnone size-full wp-image-2016" /></br>
<ul>
 	<li>Inputs: FSK object</li>
 	<li>Outputs: FSK object</li>
</ul>
Behaviour: Modifies the metadata in an FSK object.

</div>
</div>
<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSK to R</h3>
</div>
<div class="panel-body">

Extracts the R workspace out of an FSK object. The R workspace may be used with KNIME R nodes.</br>
<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSK_FSK_to-R_node.png" alt="" width="121" height="122" class="alignnone size-full wp-image-2017" /></br>
<ul>
 	<li>Inputs: FSK object</li>
 	<li>Output: RPortObject</li>
</ul>
Behaviour: Extracts the R workspace out of an FSK object and places it into the output RPortObject. If the R workspace is null or non-existent (as when the model has not been run), the generated RPortObject would be null.

</div>
</div>

<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSK to metadata</h3>
</div>
<div class="panel-body">

Extracts metadata from an FSK object.</br>
<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSK_FSK_to_Metadata_node.png" alt="" width="121" height="120" class="alignnone size-full wp-image-2018" /></br>
<ul>
 	<li>Inputs: FSK object</li>
 	<li>Outputs: KNIME table with metadata</li>
</ul>
Behaviour: Extracts the metadata in an FSK object into a KNIME table

</div>
</div>


<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSK Editor</h3>
</div>
<div class="panel-body">

Edit the scripts in an FSK object.</br>
<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSK_Editor_node.png" alt="" width="120" height="122" class="alignnone size-full wp-image-2020" /></br>
<ul>
 	<li>Inputs: FSK object (Optional)</li>
 	<li>Outputs: FSK object</li>
</ul>
Behaviour: Edit the scripts in an FSK object: model, parameters and visualization scripts. In case there is no input model connected then it will create a new model from the user interface.

</div>
</div>



<div class="panel panel-primary">
<div class="panel-heading">
<h3 class="panel-title">FSK Editor JS</h3>
</div>
<div class="panel-body">

Edit the scripts in an FSK object.</br>
<img src="https://foodrisklabs.bfr.bund.de/wp-content/uploads/2017/01/FSK_Editor_JS_node.png" alt="" width="121" height="122" class="alignnone size-full wp-image-2023" /></br>
<ul>
 	<li>Inputs: FSK object</li>
 	<li>Outputs: FSK object</li>
</ul>
Behaviour: Edit the scripts in an FSK object: model, parameters and visualization scripts. JavaScript based, its user interface may be also used in a browser in the KNIME web server.
</div>
</div>