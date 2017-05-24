---
ID: 2102
post_title: Data Import with All-in-one template
author: cthoens
post_date: 2017-05-24 16:16:46
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/data-import-with-all-in-one-template/
published: true
---
<h4>Tasks</h4>
<ul>
<li>In this tutorial we'll show you how to import delivery data to FoodChain-Lab via our All-in-one Excel template.</li>
<li>All data will be entered in one file.</li>
<li>The All-in-one template can be download from here: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/templates/All_In_One_Template.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLa...</a></li>
</ul>
<h5>1</h5>
<ul>
<li>Open "All_In_One_Template.xlsx" and select the <b>Stations</b> sheet.</li>
<li>Here you must enter all stations of the delivery network.</li>
<li>The <b>Company_ID</b> column is mandatory, all other columns are optional.</li>
<li>Next to <b>Additional Fields</b> you can specify your own columns, for which you would like to enter data.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/1.png"/></a>
<h5>2</h5>
<ul>
<li>Now select the <b>Deliveries</b> sheet.</li>
<li>Here you must enter all deliveries between the stations defined in the previous sheet.</li>
<li>The columns with the red headers are mandatory. In <b>Station</b> and <b>Recipient</b> you must enter <b>Company_IDs</b> from the previous sheet.</li>
<li>Next to <b>Additional Fields</b> you can specify your own columns, for which you would like to enter data.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/2.png"/></a>
<h5>3</h5>
<ul>
<li>Now select the <b>Deliveries2Deliveries</b> sheet.</li>
<li>Here you can connect two deliveries from the previous sheet. In both columns you must enter <b>DeliveryIDs</b>.</li>
<li>The <b>From</b>-delivery is a part/ingredient of the <b>To</b>-delivery. A contamination can spread from "<b>From</b>" to "<b>To</b>".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/3.png"/></a>
<h5>4</h5>
<ul>
<li>Switch back to the <b>Stations</b> sheet and enter the data from the screenshot.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/4.png"/></a>
<h5>5</h5>
<ul>
<li>Switch to the <b>Deliveries</b> sheet and enter the data from the screenshot.</li>
<li>The "Yogurt Factory" produces two lots of yogurt. Milk from delivery "L117_1" is used for the first lot ("LY1") and milk from deliveries "L117_2" and "L14_1" is used for the second lot ("LY2"). This ingredient information will be entered in the next sheet.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/5.png"/></a>
<h5>6</h5>
<ul>
<li>In this sheet you can only reference deliveries and not lots.</li>
<li>Therefore we have to connect "L117_1" to both deliveries of lot "LY1" ("LY1_1" and "LY1_2").</li>
<li>And "L117_2" and "L14_1" have to be connected to both deliveries of lot "LY2" ("LY2_1" and "LY2_2").</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/6.png"/></a>
<h5>7</h5>
<ul>
<li>After entering all data in the template, please open KNIME now.</li>
<li>Then select <b>Food-Lab > Open DB Gui...</b> in the menu bar to open the database interface.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/7.png"/></a>
<h5>8</h5>
<ul>
<li>To import this file click on the <b>Table import</b> button in the upper left corner of the database interface.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/8.png"/></a>
<h5>9</h5>
<ul>
<li>In the file dialog that appears, select "All_In_One_Template.xlsx" and press <b>Open</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/9.png"/></a>
<h5>10</h5>
<ul>
<li>You'll see a message that the import was successful.</li>
<li>Press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/10.png"/></a>
<h5>11</h5>
<ul>
<li>In the database interface you'll notice, that there is now data in the tables.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datatemplate/11.png"/></a>