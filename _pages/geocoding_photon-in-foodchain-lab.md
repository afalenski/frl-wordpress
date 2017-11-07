---
ID: 2444
post_title: Geocoding with Photon in FoodChain-Lab
author: FRL_Admin
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/geocoding_photon-in-foodchain-lab/
published: true
post_date: 2017-11-07 16:58:25
---
<h4>Tasks</h4>
<ul>
<li>Perform a geocoding by using the Geocoding workflow from <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/Geocoding_with_Photon.knwf" target="_blank">https://github.com/SiLeBAT/BfROpenLa...</a>.</li>
<li>Add the <b>FoodChain-Lab</b> <b>Geocoding</b> node.</li>
<li>Do the geocoding by using the Photon Geocoding Service.</li>
</ul>
<h5>1</h5>
<ul>
<li>Import the Geocoding workflow from <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/Geocoding_with_Photon.knwf" target="_blank">https://github.com/SiLeBAT/BfROpenLa...</a>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/1.png"/></a>
<h5>2</h5>
<ul>
<li>To perform geocoding we need to add the <b>FoodChain-Lab</b> <b>Geocoding</b> node.</li>
<li>Add the <b>FoodChain-Lab</b> <b>Geocoding</b> node by double clicking on it in the <b>Node Repository</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/2.png"/></a>
<h5>3</h5>
<ul>
<li>A <b>Geocoding</b> node was added to the workflow. It is connected to the <b>SupplyChainReader</b> and needs to be set up.</li>
<li>Open its configuration by double clicking on it or by using its context menue (right click on the node).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/3.png"/></a>
<h5>4</h5>
<ul>
<li>Set the <b>Service Provider</b> to <b>Photon</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/4.png"/></a>
<h5>5</h5>
<ul>
<li>The <b>Address</b> is properly set</li>
<li>You need to set the <b>Server Address</b>. You can use <b>http://photon.komoot.de</b>, which is a public available service.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/5.png"/></a>
<h5>6</h5>
<ul>
<li>For many requests geocoding services return multiple results (e.g. when there are two streets with the same name).</li>
<li>To deal with this we have to decide if we just want to use the first or look at all choices and try to find the best.</li>
<li>Looking manually at all choices is a lot of work for large data sets. In this tutorial select <b>Use first</b> and press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/6.png"/></a>
<h5>7</h5>
<ul>
<li>Right click on the <b>Geocoding</b> node and select <b>Execute</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/7.png"/></a>
<h5>8</h5>
<ul>
<li>The execution can take a while.</li>
<li>The progress bar under the node shows what percentage of data has been processed.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/8.png"/></a>
<h5>9</h5>
<ul>
<li>When the execution is finished, we can look at the results.</li>
<li>Right click on the <b>Geocoding</b> node and select <b>Coordinates</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/9.png"/></a>
<h5>10</h5>
<ul>
<li>In the dialog that pops up, you can look at the whole data table.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/10.png"/></a>
<h5>11</h5>
<ul>
<li>Scroll to the right to look at the columns with latitude and longitude (the two rightmost columns).</li>
<li>One geocoding request was not successful.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/11.png"/></a>