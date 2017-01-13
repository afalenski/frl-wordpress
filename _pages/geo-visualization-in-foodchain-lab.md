---
ID: 748
post_title: Geo-Visualization in FoodChain-Lab
author: FRL_Admin
post_date: 2015-03-18 10:16:00
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/geo-visualization-in-foodchain-lab/
published: true
---
<h4>Tasks</h4>
<ul>
<li>Use the following workflow: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Visualize the delivery network in the GIS mode of the <b>Tracing View</b>.</li>
<li>Select all stations in Poland and check out where these stations are located in the Graph mode.</li>
</ul>
<h5>1</h5>
<ul>
<li>Import the Example Workflow from <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Open the <b>Tracing View</b> by double-clicking on it.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/1.png"/></a>
<h5>2</h5>
<ul>
<li>Now you should see a graphical representation of the delivery network.</li>
<li>To switch to the geographical representation click <b>Switch to GIS</b> in the upper right corner.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/2.png"/></a>
<h5>3</h5>
<ul>
<li>The country borders, which where read from a shapefile, are used for geographical visualization.</li>
<li>To zoom to a certain area of the graph select "Transforming" as <b>Editing Mode</b> and zoom/move the graph by using the mouse wheel and the left mouse button (works as in Google Maps).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/3.png"/></a>
<h5>4</h5>
<ul>
<li>If you are online, you can change the type of visualization.</li>
<li>Select e.g. "Mapnik" as <b>GIS Type</b>.</li>
<li>Now you should see a visualization with OpenStreetMap data.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/4.png"/></a>
<h5>5</h5>
<ul>
<li>We can now select certain stations based on geography.</li>
<li>Select "Picking" as <b>Editing Mode</b> and select all stations in Poland by dragging with the left mouse button a rect around the stations.</li>
<li>The selected stations are now colored blue.</li>
<li>Switch back to the graphical view by clicking <b>Switch to Graph</b> in the upper right corner.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/5.png"/></a>
<h5>6</h5>
<ul>
<li>The blue stations are the ones you selected in the geographical view, since changes you make in any of the view are automatically applied to the other view.</li>
<li>That makes it easy to switch back and forth between both representations and use the benefits of both.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/6.png"/></a>
<h5>7</h5>
<ul>
<li>Lets now select a certain "cluster" in the graphical view and see where the stations are in the geographical view.</li>
<li>So select the "cluster" in the red circle and click <b>Switch to GIS</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/7.png"/></a>
<h5>8</h5>
<ul>
<li>As you can see the stations of the cluster are located all over France.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/8.png"/></a>