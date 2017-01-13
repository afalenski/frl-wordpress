---
ID: 745
post_title: Geocoding in FoodChain-Lab
author: FRL_Admin
post_date: 2015-03-18 10:14:51
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/geocoding-in-foodchain-lab/
published: true
---
<h4>Tasks</h4>
<ul>
<li>Perform a geocoding by using the Geocoding workflow from <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/Geocoding.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Use "Street", "HouseNumber", "City" and "Country" as input parameters.</li>
<li>Do the geocoding by using the MapQuest Geocoding Service.</li>
</ul>
<h5>1</h5>
<ul>
<li>Import the Geocoding workflow from <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/Geocoding.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>In this tutorial we are using the MapQuest Open Geocoding service.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/1.png"/></a>
<h5>2</h5>
<ul>
<li>For using MapQuest you have to register and create a key at <a href="https://developer.mapquest.com" target="_blank">https://developer.mapquest.com</a></li>
<li>This key has to be entered in the KNIME preferences.</li>
<li>Select <b>File < Preferences</b> in the menu bar.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/2.png"/></a>
<h5>3</h5>
<ul>
<li>The Preferences dialog will pop up.</li>
<li>Here you can specify all preferences for KNIME and FoodChain-Lab.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/3.png"/></a>
<h5>4</h5>
<ul>
<li>Select <b>KNIME < Geocoding</b> in the navigation tree on the left.</li>
<li>Enter your <b>MapQuest Application Key</b> and press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/4.png"/></a>
<h5>5</h5>
<ul>
<li>To perform geocoding we need one column with addresses in our data table. The <b>Supply Chain Reader</b> puts out all parts of the address (street, city, ...) in different columns.</li>
<li>The address column is created via the <b>Address Creator</b> node.</li>
<li>Double click on this node to open its dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/5.png"/></a>
<h5>6</h5>
<ul>
<li>In the dialog you can specify the columns that should used for creating the address column.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/6.png"/></a>
<h5>7</h5>
<ul>
<li>Since we want to do the Geocoding based on "Street", "HouseNumber", "City" and "Country", we have to set the <b>Country Column</b> to "Country" and the <b>Postal Code Column</b> to "none".</li>
<li>Press <b>OK</b> to close the dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/7.png"/></a>
<h5>8</h5>
<ul>
<li>Since we changed the settings, the node resets automatically.</li>
<li>Press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/8.png"/></a>
<h5>9</h5>
<ul>
<li>The configuration for the <b>Address Creator</b> has been updated.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/9.png"/></a>
<h5>10</h5>
<ul>
<li>Right click on the <b>Address Creator</b> node and select <b>Execute</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/10.png"/></a>
<h5>11</h5>
<ul>
<li>Now that we updated the <b>Address</b>, the geocoding can be set up.</li>
<li>Double click on the <b>Geocoding</b> node to open its dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/11.png"/></a>
<h5>12</h5>
<ul>
<li>Here you can specify the <b>Service Provider</b> for geocoding and the column that should be used.</li>
<li>Both are already correctly set, so we don't need to change anything here.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/12.png"/></a>
<h5>13</h5>
<ul>
<li>For many requests geocoding services return multiple results (e.g. when there are two streets with the same name).</li>
<li>To deal with this we have to decide if we just want to use the first or look at all choices and try to find the best.</li>
<li>Looking manually at all choices is a lot of work for large data sets. In this tutorial select <b>Use first</b> and press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/13.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/13.png"/></a>
<h5>14</h5>
<ul>
<li>Right click on the <b>Geocoding</b> node and select <b>Execute</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/14.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/14.png"/></a>
<h5>15</h5>
<ul>
<li>The execution can take a while.</li>
<li>The progress bar under the node shows what percentage of data has been processed.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/15.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/15.png"/></a>
<h5>16</h5>
<ul>
<li>When the execution is finished, we can look at the results.</li>
<li>Right click on the <b>Geocoding</b> node and select <b>Coordinates</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/16.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/16.png"/></a>
<h5>17</h5>
<ul>
<li>In the dialog that pops up, you can look at the whole data table.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/17.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/17.png"/></a>
<h5>18</h5>
<ul>
<li>Scroll to the right to look at the columns with latitude and longitude (the two rightmost columns).</li>
<li>Some geocoding requests were not successful. MapQuest returned US coordinates, although all addresses are in Germany.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/18.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/18.png"/></a>