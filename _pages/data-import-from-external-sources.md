---
ID: 2104
post_title: Data Import from External Sources
author: cthoens
post_date: 2017-05-24 16:20:10
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/data-import-from-external-sources/
published: true
---
<h4>Content</h4>
<ul>
<li>This tutorial shows how data can imported into FoodChain-Lab without using the Excel templates.</li>
<li>Therefore the external data has to read into KNIME tables.</li>
<li>KNIME provides a multitude of reader nodes for various data formats (e.g. csv, SQL databases, ...).</li>
<li>Here we just show which tables are needed by FoodChain-Lab and which columns they must contain. To do so the we have created these tables with <b>Table Creator</b> nodes.</li>
</ul>
<h5>1</h5>
<ul>
<li>Import the workflow from <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Import.knwf" target="_blank">https://github.com/SiLeBAT/BfROpenLa...</a>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/1.png"/></a>
<h5>2</h5>
<ul>
<li>FoodChain-Lab needs three tables to perform a tracing analysis: <b>Stations</b>, <b>Deliveries</b> and <b>Delivery Relations</b>.</li>
<li>The <b>Table Creator</b> nodes on the left show all mandatory columns for these three tables.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/2.png"/></a>
<h5>3</h5>
<ul>
<li>Double click on the <b>Table Creator</b> for the <b>Stations</b> table to open its dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/3.png"/></a>
<h5>4</h5>
<ul>
<li>As you can see the only mandatory column in the <b>Stations</b> table is the column <b>ID</b> of type string.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/4.png"/></a>
<h5>5</h5>
<ul>
<li>Double click on the <b>Table Creator</b> for the <b>Deliveries</b> table to open its dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/5.png"/></a>
<h5>6</h5>
<ul>
<li>The <b>Deliveries</b> table has three mandatory columns: <b>ID</b>, <b>from</b> and <b>to</b> (all of type string)</li>
<li>The <b>from</b> and <b>to</b> columns contain the source station and target station <b>IDs</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/6.png"/></a>
<h5>7</h5>
<ul>
<li>Double click on the <b>Table Creator</b> for the <b>Delivery Relations</b> table to open its dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/7.png"/></a>
<h5>8</h5>
<ul>
<li>The <b>Delivery Relations</b> table has the columns <b>from</b> and <b>to</b> of type string.</li>
<li>These columns contain <b>IDs</b> from the <b>Delivery</b> table and are meant to connect two deliveries.</li>
<li>The <b>from</b>-delivery is a part/ingredient of the <b>to</b>-delivery. A contamination can spread from "<b>from</b>" to "<b>to</b>".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/8.png"/></a>
<h5>9</h5>
<ul>
<li>Now we will look the <b>Table Creator</b> nodes on the right which show the optional columns for the three tables.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/9.png"/></a>
<h5>10</h5>
<ul>
<li>Double click on the <b>Table Creator</b> for the <b>Stations</b> table to open its dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/10.png"/></a>
<h5>11</h5>
<ul>
<li>The optional columns for the <b>Stations</b> table are <b>Address</b>, <b>Country</b>, <b>Latitude</b> and <b>Longitude</b>.</li>
<li><b>Latitude</b> and <b>Longitude</b> are used for the geographical visualization in the <b>Tracing View</b> and <b>Address</b> and <b>Country</b> can be used for geocoding, if <b>Latitude</b> and <b>Longitude</b> are not known yet.</li>
<li>Any other arbitrary columns of this table can also be used in the <b>Tracing View</b> for highlighting etc.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/11.png"/></a>
<h5>12</h5>
<ul>
<li>The <b>Geocoding</b> node in the upper right corner shows how <b>Address</b> and <b>Country</b> can be used for geocoding to compute <b>Latitude</b> and <b>Longitude</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/12.png"/></a>
<h5>13</h5>
<ul>
<li>Double click on the <b>Table Creator</b> for the <b>Deliveries</b> table to open its dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/13.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/13.png"/></a>
<h5>14</h5>
<ul>
<li>The optional columns are <b>Date Delivery</b>, <b>Date Delivery Arrival</b>, <b>Lot ID</b>, <b>Amount</b> and <b>Amount Unit</b>.</li>
<li>The date columns are of type string and in YYYY-MM-DD format. They used for computing cross contamination.</li>
<li>If the <b>Lot ID</b> column (of type string) is provided, lot-based scores are computed.</li>
<li>The amount columns are just used for plausibility checks.</li>
<li>Any other arbitrary columns of this table can also be used in the <b>Tracing View</b> for highlighting etc.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/14.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/14.png"/></a>
<h5>15</h5>
<ul>
<li>Double click on the <b>Table Creator</b> for the <b>Deliveries Relations</b> table to open its dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/15.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/15.png"/></a>
<h5>16</h5>
<ul>
<li>The <b>Delivery Relations</b> table does not have any optional columns.</li>
<li>All columns other than <b>from</b> and <b>to</b> are ignored.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/16.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_import_data/16.png"/></a>