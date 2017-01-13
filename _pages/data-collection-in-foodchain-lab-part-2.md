---
ID: 1475
post_title: Data Collection in FoodChain-Lab Part 2
author: FRL_Admin
post_date: 2015-11-10 15:13:44
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/data-collection-in-foodchain-lab-part-2/
published: true
---
<h4>Tasks</h4>
<ul>
<li>In this part of the tutorial we will do a back- and forward-tracing from the "Frozen Fruit Sales" station.</li>
<li>You can either complete part 1 of the tutorial or directly import the following files into an empty database before starting this tutorial.</li>
<li>Start Template: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/Start_Tracing_Caterers.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a></li>
<li>Caterer 1 Template: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/Backtrace_request_Caterer 1.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a></li>
<li>Caterer 2 Template: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/Backtrace_request_Caterer 2.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a></li>
</ul>
<h5>1</h5>
<ul>
<li>You should have the database interface open.</li>
<li>Press the button for generating backtracing templates, which is marked by the red circle.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/1.png"/></a>
<h5>2</h5>
<ul>
<li>Since we want to do the backtracing for the supplier "Frozen Fruit Sales", select <b>Supplier</b> only and press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/2.png"/></a>
<h5>3</h5>
<ul>
<li>In the file dialog that appears, you can specify the folder where the generated templates should be saved.</li>
<li>Select the desired folder and press <b>Save</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/3.png"/></a>
<h5>4</h5>
<ul>
<li>You'll be noticed, that one template was generated in the folder you specified.</li>
<li>Press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/4.png"/></a>
<h5>5</h5>
<ul>
<li>Open the generated template "Backtrace_request_Frozen Fruit Sales.xlsx".</li>
<li>Add the stations from the screenshot to the <b>Stations</b> sheet.</li>
<li>These station include 3 strawberry suppliers that delivered strawberries to "Frozen Fruit Sales" and also a caterer that received strawberries.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/5.png"/></a>
<h5>6</h5>
<ul>
<li>In the <b>BackTracing</b> sheet you can see the three outgoing deliveries of "Frozen Fruit Sales".</li>
<li>These deliveries belong to lots "108" and "139".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/6.png"/></a>
<h5>7</h5>
<ul>
<li>Now scroll to the <b>Ingredients for Lot(s)</b> section.</li>
<li>Enter the 3 deliveries, that were used as ingredients for lot "108", from the screenshot.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/7.png"/></a>
<h5>8</h5>
<ul>
<li>Lot "108" was not only delivered to "Caterer 1" and "Caterer 2", but also to a third caterer.</li>
<li>We can add this information in the <b>ForwardTracing_Opt</b> sheet.</li>
<li>Enter the delivery to "Caterer 3" from the screenshot.</li>
<li>Save the completed document ("Backtrace_request_Frozen Fruit Sales.xlsx").</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/8.png"/></a>
<h5>9</h5>
<ul>
<li>To import this file click on the <b>Table import</b> button in the upper left corner of the database interface.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/9.png"/></a>
<h5>10</h5>
<ul>
<li>In the file dialog that appears, select "Backtrace_request_Frozen Fruit Sales.xlsx" and press <b>Open</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/10.png"/></a>
<h5>11</h5>
<ul>
<li>You'll be notified, that some warnings occurred during import.</li>
<li>Press <b>Show Details</b> to have at look at the warnings.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/11.png"/></a>
<h5>12</h5>
<ul>
<li>730kg of strawberries went into lot "108", but all the deliveries of frozen strawberries from lot "108" just add up to 99.75kg.</li>
<li>Warnings like these are supposed to help finding errors in the data.</li>
<li>In this tutorial we just ignore the warning. So press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/12.png"/></a>
<h5>13</h5>
<ul>
<li>We now know that lot "108" was also delivered to "Caterer 3" and we have imported this delivery into the database.</li>
<li>Let's do a forward tracing from "Caterer 3".</li>
<li>Press the button for generating the forward template for a specific station marked by the red circle.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/13.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/13.png"/></a>
<h5>14</h5>
<ul>
<li>In the dialog that appears, you must select the station for which the template should be generated.</li>
<li>Enter "cate" in the field after <b>Enter Search Query</b> and you will see that the table below only shows the caterers now.</li>
<li>Press the <b>Select</b> button for "Caterer 3".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/14.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/14.png"/></a>
<h5>15</h5>
<ul>
<li>In the file dialog that appears, you can specify the folder where the generated templates should be saved.</li>
<li>Select the desired folder and press <b>Save</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/15.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/15.png"/></a>
<h5>16</h5>
<ul>
<li>You'll be noticed, that one template was generated in the folder you specified.</li>
<li>Press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/16.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/16.png"/></a>
<h5>17</h5>
<ul>
<li>Open "StationFwdtrace_request_Caterer 3.xlsx".</li>
<li>Enter the station from the screenshot in the <b>Stations</b> sheet.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/17.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/17.png"/></a>
<h5>18</h5>
<ul>
<li>In the <b>FwdTracing</b> sheet you first have to enter all relevant outgoing lots of "Caterer 3". So add lot "C3M1" to the <b>Lot Information</b> section as shown on the screenshot (red rectangle).</li>
<li>Now you can specify, that the delivery of "Frozen Strawberries" was used as an ingredient in this lot (red circle).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/18.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/18.png"/></a>
<h5>19</h5>
<ul>
<li>Scroll down to the <b>Products Out</b> section to specify the outgoing deliveries from lot "C3M1".</li>
<li>Add the deliveries as shown on the screenshot.</li>
<li>Save the completed document ("StationFwdtrace_request_Caterer 3.xlsx").</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/19.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/19.png"/></a>
<h5>20</h5>
<ul>
<li>To import this file click on the <b>Table import</b> button in the upper left corner of the database interface.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/20.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/20.png"/></a>
<h5>21</h5>
<ul>
<li>In the file dialog that appears, select "StationFwdtrace_request_Caterer 3.xlsx" and press <b>Open</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/21.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/21.png"/></a>
<h5>22</h5>
<ul>
<li>You'll see a message that the import was successful.</li>
<li>Press <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/22.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/22.png"/></a>