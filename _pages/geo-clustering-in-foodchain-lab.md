---
ID: 698
post_title: Geo-Clustering in FoodChain-Lab
author: FRL_Admin
post_date: 2015-03-10 19:07:47
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/geo-clustering-in-foodchain-lab/
published: true
---
<h4>Tasks</h4>
<ul>
<li>Perform a clustering using the following workflow: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a></li>
<li>Cluster all French primary producers by using the <b>GIS Cluster</b> node.</li>
<li>Use a <b>Max Neighborhood Distance</b> of 100km.</li>
<li>That means two stations are put into the same cluster if their distance is less than 100km.</li>
</ul>
<h5>1</h5>
<ul>
<li>Import the Example Workflow from <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/1.png"/></a>
<h5>2</h5>
<ul>
<li>Drag the <b>GIS Cluster</b> node from <b>FoodChain-Lab</b> in the <b>Node Repository</b> to the <b>Workflow Editor</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/2.png"/></a>
<h5>3</h5>
<ul>
<li>Connect the output of <b>Joiner</b> to the input of <b>GIS Cluster</b>.</li>
<li>Connect the output of <b>GIS Cluster</b> to the first input of <b>Tracing View</b>.</li>
<li>Double click on the <b>GIS Cluster</b> node to open its dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/3.png"/></a>
<h5>4</h5>
<ul>
<li>In this dialog you can set up an algorithm for geographical clustering based on latitude and longitude.</li>
<li>Click on <b>Set Filter</b> to define which stations should be clustered.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/4.png"/></a>
<h5>5</h5>
<ul>
<li>You should see this dialog now.</li>
<li>Press the button in the red circle to change the <b>Property</b> value.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/5.png"/></a>
<h5>6</h5>
<ul>
<li>Select "Country".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/6.png"/></a>
<h5>7</h5>
<ul>
<li>Now select "FR" as <b>Value</b>, since we want to cluster stations in France.</li>
<li>Afterwards press <b>Add</b> to add another condition.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/7.png"/></a>
<h5>8</h5>
<ul>
<li>For the new condition select "type of business" as <b>Property</b> and "Primary Producer" as <b>Value</b>, since we want to cluster primary producers only.</li>
<li>Now press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/8.png"/></a>
<h5>9</h5>
<ul>
<li>Set the <b>Max Neighborhood Distance</b> to 100km. That means that stations with distance of less than 100km are put into the same cluster. For details on the algorithm look here: <a href="https://en.wikipedia.org/wiki/DBSCAN" target="_blank">https://en.wikipedia.org/wiki/DBSCAN</a></li>
<li>Press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/9.png"/></a>
<h5>10</h5>
<ul>
<li>Right click on <b>GIS Cluster</b> to open its context menu and select <b>Execute</b> to execute the node.</li>
<li>The results of the clustering are put into the new column <b>ClusterID</b>. This column will now be used in the <b>Tracing View</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/10.png"/></a>
<h5>11</h5>
<ul>
<li>Open the <b>Tracing View</b> by double-clicking on it.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/11.png"/></a>
<h5>12</h5>
<ul>
<li>A window showing the delivery network should open now.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/12.png"/></a>
<h5>13</h5>
<ul>
<li>Right click in the graph to open the context menu and select <b>Collapse by Property</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/13.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/13.png"/></a>
<h5>14</h5>
<ul>
<li>The clustering will be done based on the results of the <b>GIS Cluster</b> node.</li>
<li>Select <b>ClusterID</b> and press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/14.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/14.png"/></a>
<h5>15</h5>
<ul>
<li>Just press <b>OK</b>, since we do not want to exclude any area.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/15.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/15.png"/></a>
<h5>16</h5>
<ul>
<li>All French primary producers have been clustered to areas.</li>
<li>Each selected station (blue circle) is an area in France.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/16.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/16.png"/></a>
<h5>17</h5>
<ul>
<li>Select "Picking" as <b>Editing Mode</b> and click in the graph to deselect all stations.</li>
<li>You can now see, that one of the stations is yellow. That means, that this stations (French area) is connected to all outbreak spots (red circles).</li>
<li>Press <b>Switch to GIS</b> to see where this area is.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/17.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/17.png"/></a>
<h5>18</h5>
<ul>
<li>The area is in Southern France.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/18.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/18.png"/></a>