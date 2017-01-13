---
ID: 742
post_title: Create FoodChain-Lab Workflow Part 2
author: FRL_Admin
post_date: 2015-03-18 10:13:34
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/create-foodchain-lab-workflow-part-2/
published: true
---
<h4>Tasks</h4>
<ul>
<li>Use the <b>Tracing View</b> to display the delivery graph in a clearly arranged way.</li>
<li>Apply the <b>Default Highlighting</b> to color the graph.</li>
<li>Visualize the backward and forward trace for an arbitrary station.</li>
</ul>
<h5>1</h5>
<ul>
<li>This is the second part of the tutorial.</li>
<li>You can either do the first part to create this workflow or download it from <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/MyFirstWorkflow.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Double click on the <b>Tracing View</b> to open its dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/1.png"/></a>
<h5>2</h5>
<ul>
<li>In the <b>Tracing View</b> you can see the imported delivery network.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/2.png"/></a>
<h5>3</h5>
<ul>
<li>To arrange the network in a better way right click in the graph and select <b>Apply Layout > Fruchterman-Reingold</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/3.png"/></a>
<h5>4</h5>
<ul>
<li>This layout process is not deterministic. That means you will get a different result each time.</li>
<li>You can apply the layout again, if you are not satisfied with the current result.</li>
<li>You can also apply a layout for certain stations only. Therefore you have to select the stations you want to be layouted and apply the layout again.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/4.png"/></a>
<h5>5</h5>
<ul>
<li>Right click in the graph to open the context menu and select <b>Set default Highlighting</b>.</li>
<li>Highlighting uses colors and sizes to visualize certain properties of stations/deliveries.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/5.png"/></a>
<h5>6</h5>
<ul>
<li>You will notice, that 4 stations are colored red now and some stations increased in size.</li>
<li>The red stations are the supermarkets, where we set the weight to "1".</li>
<li>The size of each station is based on its "Score".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/6.png"/></a>
<h5>7</h5>
<ul>
<li>Activate <b>Show Legend</b> to get a legend for the defined colors.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/7.png"/></a>
<h5>8</h5>
<ul>
<li>Now we can observe a station to see its delivery trace.</li>
<li>Set "Picking" as <b>Editing Mode</b> and double click on any station.</li>
<li>We clicked on the station in the red circle.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/8.png"/></a>
<h5>9</h5>
<ul>
<li>A dialog will pop up, that shows all attributes of the station.</li>
<li>Additionally you can change "Weight", "Cross Contamination", "Kill Contamination" and "Observed".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/9.png"/></a>
<h5>10</h5>
<ul>
<li>Select <b>Observed</b> and press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/10.png"/></a>
<h5>11</h5>
<ul>
<li>All stations/deliveries of the forward trace are orange-colored and the ones of the backward trace are purple.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/11.png"/></a>
<h5>12</h5>
<ul>
<li>Click at an empty area of the graph to deselect all stations.</li>
<li>Now you can see, that the "Observed" station is green.</li>
<li>Then activate "Join Deliveries" to simplify the graph. Deliveries with the same supplier and recipient are joined now.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/12.png"/></a>