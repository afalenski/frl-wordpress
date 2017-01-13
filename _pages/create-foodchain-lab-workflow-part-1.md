---
ID: 725
post_title: Create FoodChain-Lab Workflow Part 1
author: FRL_Admin
post_date: 2015-03-17 11:53:28
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/create-foodchain-lab-workflow-part-1/
published: true
---
<h4>Tasks</h4>
<ul>
<li>Import the Example XLS template to FoodChain-Lab.</li>
<li>You can download it from here: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/FCL_Example.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a></li>
<li>Via the <b>Tracing</b> node assign weights of "1" to the supermarkets in Hamburg, Karlsruhe, Ingolstadt and Hanover to mark them as outbreak locations.</li>
<li>Use the <b>Tracing View</b> to look at the delivery network.</li>
</ul>
<h5>1</h5>
<ul>
<li>Select <b>Food-Lab > Open DB Gui...</b> in the menu bar to open the database interface.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/1.png"/></a>
<h5>2</h5>
<ul>
<li>If you get a message saying the internal database has been created, click <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/2.png"/></a>
<h5>3</h5>
<ul>
<li>In the database interface click the <b>Table import</b> button in the upper left corner.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/3.png"/></a>
<h5>4</h5>
<ul>
<li>Now a file dialog will pop up.</li>
<li>*.xlsx files in FoodChain-Lab format can be selected here.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/4.png"/></a>
<h5>5</h5>
<ul>
<li>Download the example file from <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/FCL_Example.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Select the file in the dialog and press <b>Open</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/5.png"/></a>
<h5>6</h5>
<ul>
<li>When the importing is finished you see a dialog with errors/warnings, that occurred in the import process.</li>
<li>No errors ocurred, so just press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/6.png"/></a>
<h5>7</h5>
<ul>
<li>In the database interface, you can now look at the imported data and check the data for duplicates.</li>
<li>Close the dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/7.png"/></a>
<h5>8</h5>
<ul>
<li>Now we want to create a workflow, that uses the imported data.</li>
<li>Right click on <b>LOCAL</b> in the <b>KNIME Explorer</b> and select <b>New KNIME Workflow...</b></li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/8.png"/></a>
<h5>9</h5>
<ul>
<li>In the dialog set the name of the workflow to "MyFirstWorkflow" and click <b>Finish</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/9.png"/></a>
<h5>10</h5>
<ul>
<li>The created workflow will be shown in the editor in the center.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/10.png"/></a>
<h5>11</h5>
<ul>
<li>Drag the <b>Supply Chain Reader</b> from the <b>Node Repository</b> to the workflow.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/11.png"/></a>
<h5>12</h5>
<ul>
<li>We do not need to configure the <b>Supply Chain Reader</b>.</li>
<li>Right click on it and select <b>Execute</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/12.png"/></a>
<h5>13</h5>
<ul>
<li>The <b>Supply Chain Reader</b> has now read all data from the internal database.</li>
<li>Select the <b>Supply Chain Reader</b> in the workflow (so that a rect is drawn around it) and double click on the <b>Tracing</b> node in the <b>Node Repository</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/13.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/13.png"/></a>
<h5>14</h5>
<ul>
<li>The <b>Tracing</b> node should show up in the workflow and its three input ports should be automatically connected to the <b>Supply Chain Reader</b>.</li>
<li>Double click on the <b>Tracing</b> node to configure it.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/14.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/14.png"/></a>
<h5>15</h5>
<ul>
<li>You will notice tabs for "Station/Delivery Properties".</li>
<li>"Weight", "Cross Contamination" and "Kill Contamination" can be set there. Based on these properties a "Score" is computed for each station/delivery.</li>
<li>Additionally you can set "Observed" stations/deliveries.</li>
<li>Select the <b>Station Properties</b> and <b>Weight</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/15.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/15.png"/></a>
<h5>16</h5>
<ul>
<li>A table with all available stations will show up.</li>
<li>The weight can be set in the left column.</li>
<li>Since scrolling through all stations is very inefficient, we can filter out all desired stations.</li>
<li>Click on <b>Set Filter</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/16.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/16.png"/></a>
<h5>17</h5>
<ul>
<li>In this dialog you can specify which stations should appear in the table.</li>
<li>Press the button in the red circle to change the value for <b>Property</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/17.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/17.png"/></a>
<h5>18</h5>
<ul>
<li>Select "type of business".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/18.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/18.png"/></a>
<h5>19</h5>
<ul>
<li>We only want to specify weights for supermarkets, since that is where contaminated products were found.</li>
<li>Set <b>Value</b> to "Supermarket" and press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/19.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/19.png"/></a>
<h5>20</h5>
<ul>
<li>Now you only see supermarkets in the dialog.</li>
<li>Set a weight of "1" to the supermarkets in "Hamburg", "Karlsruhe", "Ingolstadt" und "Hanover" to indicate that contaminated products were found there.</li>
<li>Click <b>OK</b> to apply the settings and close the dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/20.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/20.png"/></a>
<h5>21</h5>
<ul>
<li>Right click on the <b>Tracing</b> node and select <b>Execute</b> to execute the node.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/21.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/21.png"/></a>
<h5>22</h5>
<ul>
<li>Drag the <b>Tracing View</b> from the <b>Node Repository</b> to the workflow.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/22.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/22.png"/></a>
<h5>23</h5>
<ul>
<li>Connect the output ports of the <b>Tracing</b> node to the first two input ports of the <b>Tracing View</b>.</li>
<li>Connect the third output port of the <b>Supply Chain Reader</b> to the third input port of the <b>Tracing View</b>.</li>
<li>Now you open the <b>Tracing View</b> and analyze the data. This will be shown in the second part of this tutorial.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/23.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/23.png"/></a>