---
ID: 687
post_title: Clustering in FoodChain-Lab
author: FRL_Admin
post_date: 2015-03-10 17:20:34
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/clustering-in-foodchain-lab/
published: true
---
<h4>Tasks</h4>
<ul>
<li>Perform a clustering using the following workflow: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a></li>
<li>Cluster all French primary producers based on their city.</li>
<li>That means all stations from the same city should be put into one meta-station.</li>
</ul>
<h5>1</h5>
<ul>
<li>Import the Example Workflow from <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Open the <b>Tracing View</b> by double-clicking on it.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/1.png"/></a>
<h5>2</h5>
<ul>
<li>A window showing the delivery network opens.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/2.png"/></a>
<h5>3</h5>
<ul>
<li>Right click in the graph to open the context menu and select <b>Set Selected Stations</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/3.png"/></a>
<h5>4</h5>
<ul>
<li>You should see this dialog now.</li>
<li>Press the button in the red circle to change the <b>Property</b> value.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/4.png"/></a>
<h5>5</h5>
<ul>
<li>Select "Country".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/5.png"/></a>
<h5>6</h5>
<ul>
<li>Now select "FR" as <b>Value</b>, since we want to cluster stations in France.</li>
<li>Afterwards press <b>Add</b> to add another condition.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/6.png"/></a>
<h5>7</h5>
<ul>
<li>For the new condition select "type of business" as <b>Property</b> and "Primary Producer" as <b>Value</b>, since we want to cluster primary producers only.</li>
<li>Now press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/7.png"/></a>
<h5>8</h5>
<ul>
<li>All French primary producers are selected now, which is indicated by the blue color.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/8.png"/></a>
<h5>9</h5>
<ul>
<li>Right click in the graph to open the context menu and select <b>Collapse by Property</b> to cluster the selected stations.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/9.png"/></a>
<h5>10</h5>
<ul>
<li>Select <b>Yes</b> to only cluster selected stations.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/10.png"/></a>
<h5>11</h5>
<ul>
<li>We want to cluster on city level. That means all stations from the same city will be merged.</li>
<li>Select <b>City</b> and press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/11.png"/></a>
<h5>12</h5>
<ul>
<li>Just press <b>OK</b>, since we do not want to exclude any cities.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/12.png"/></a>
<h5>13</h5>
<ul>
<li>All French primary producers have been clustered to cities.</li>
<li>Each selected station (blue circle) is a French city.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/13.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/13.png"/></a>
<h5>14</h5>
<ul>
<li>Select "Picking" as <b>Editing Mode</b> and click in the graph to deselect all stations.</li>
<li>You can now see, that one of the stations is yellow. That means, that this station (French city) is connected to all outbreak spots (red circles).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/14.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/14.png"/></a>
<h5>15</h5>
<ul>
<li>Since the graph looks confusing now, we should reapply the layout algorithm.</li>
<li>Right click in the graph and select <b>Apply Layout > Fruchterman-Reingold</b> in the context menu.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/15.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/15.png"/></a>
<h5>16</h5>
<ul>
<li>The stations should be arranged in better way now.</li>
<li>The layout algorithm is not deterministic, therefore your result will look different from the screenshot.</li>
<li>To see which city is connected to all outbreak spots double click on the yellow circle.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/16.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/16.png"/></a>
<h5>17</h5>
<ul>
<li>As you can see in the dialog the city is "Perpignan".</li>
<li>Press <b>Switch to GIS</b> to see the city and its relations on a map.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/17.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/17.png"/></a>