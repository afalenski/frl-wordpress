---
ID: 754
post_title: Tracing in FoodChain-Lab
author: FRL_Admin
post_date: 2015-03-18 10:18:25
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/tracing-in-foodchain-lab/
published: true
---
<h4>Tasks</h4>
<ul>
<li>Use the example workflow from <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Visualize the forward and backward trace of a station via the <b>Tracing View</b>.</li>
<li>Deactivate "Cross Contamination" for the black station and see how the trace changes.</li>
</ul>
<h5>1</h5>
<ul>
<li>Import the Example Workflow from <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Open the <b>Tracing View</b> by double-clicking on it.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/1.png"/></a>
<h5>2</h5>
<ul>
<li>In the delivery graph you can see 9 <b>Outbreak</b> stations (red) and one station where <b>Cross Contamination</b> is assumed (black).</li>
<li>The size of each station is based on its "Score", which depends on the <b>Outbreak</b> stations that can be reached from the station.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/2.png"/></a>
<h5>3</h5>
<ul>
<li>We will now observe the trace of a single station in detail.</li>
<li>Set "Picking" as <b>Editing Mode</b> and double click on the station in the red circle.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/3.png"/></a>
<h5>4</h5>
<ul>
<li>A dialog will pop up, that all attributes of the station.</li>
<li>Additionally you can change "Weight", "Cross Contamination", "Kill Contamination" and "Observed".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/4.png"/></a>
<h5>5</h5>
<ul>
<li>Select <b>Observed</b> and press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/5.png"/></a>
<h5>6</h5>
<ul>
<li>All stations/deliveries of the forward trace are orange-colored and the ones of the backward trace are purple.</li>
<li>Three <b>Outbreak</b> stations are also orange striped now. That means they are also on the forward trace of the observed station.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/6.png"/></a>
<h5>7</h5>
<ul>
<li>Let's see what happens if we deactivate cross contamination in the station in the red circle.</li>
<li>So double click on it.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/7.png"/></a>
<h5>8</h5>
<ul>
<li>Uncheck <b>CrossContamination</b> and press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/8.png"/></a>
<h5>9</h5>
<ul>
<li>Deactivating cross contamination changed the forward trace of the observed station.</li>
<li>Now two of <b>Outbreak</b> stations, that were striped before, cannot be reached anymore.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/9.png"/></a>