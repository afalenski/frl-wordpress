---
ID: 770
post_title: Geo-Clustering in FoodChain-Lab
author: FRL_Admin
post_date: 2015-03-18 10:34:08
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/geo-clustering-in-foodchain-lab-2/
published: true
---
<h4>Aufgaben</h4>
<ul>
<li>Nutzen Sie folgenden Workflow: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a></li>
<li>Clusters Sie alle französischen Primärproduzenten mit Hilfe des <b>GIS Cluster</b>-Knotens.</li>
<li>Nutzen Sie dabei eine <b>Max Neighborhood Distance</b> von 100km.</li>
<li>Das bedeutet, dass zwei Stationen in das selbe Cluster kommen, wenn Sie weniger als 100km voneinander entfernt sind.</li>
</ul>
<h5>1</h5>
<ul>
<li>Importieren Sie den Beispiel Workflow von <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/1.png"/></a>
<h5>2</h5>
<ul>
<li>Ziehen Sie den <b>GIS Cluster</b>-Knoten aus dem <b>Node Repository</b> in den Workflow.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/2.png"/></a>
<h5>3</h5>
<ul>
<li>Verbinden Sie den Ausgabe-Port des <b>Joiner</b>-Knotens mit dem Eingabe-Port vom <b>GIS Cluster</b>-Knoten.</li>
<li>Verbinden Sie den Ausgabe-Port des <b>GIS Cluster</b>-Knotens mit dem Eingabe-Port vom <b>Tracing View</b>.</li>
<li>Machen Sie einen Doppelklick auf den <b>GIS Cluster</b>-Knoten um dessen Dialog zu öffnen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/3.png"/></a>
<h5>4</h5>
<ul>
<li>In dem Dialog können den Algorithmus zum Geo-Clustern konfigurieren.</li>
<li>Klicken Sie auf <b>Set Filter</b> um zu definieren welche Stationen geclustert werden sollen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/4.png"/></a>
<h5>5</h5>
<ul>
<li>Sie sollten jetzt diesen Dialog sehen.</li>
<li>Klicken Sie auf den rot markierten Button um für <b>Property</b> einen anderen Wert zu wählen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/5.png"/></a>
<h5>6</h5>
<ul>
<li>Wählen Sie "Country".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/6.png"/></a>
<h5>7</h5>
<ul>
<li>Nun wählen Sie "FR" als <b>Value</b>, da wir ja nur Stationen in Frankreich clustern wollen.</li>
<li>Klicken Sie danach auf <b>Add</b> um eine weitere Bedingung hinzuzufügen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/7.png"/></a>
<h5>8</h5>
<ul>
<li>Für die neue Bedingung wählen Sie "type of business" als <b>Property</b> und "Primary Producer" als <b>Value</b>, denn wir wollen ja nur Primärproduzenten clustern.</li>
<li>Nun klicken Sie auf <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/8.png"/></a>
<h5>9</h5>
<ul>
<li>Setzen Sie die <b>Max Neighborhood Distance</b> auf 100km. Stationen mit einer Distanz von unter 100km landen also im selben Cluster.</li>
<li>Klicken Sie <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/9.png"/></a>
<h5>10</h5>
<ul>
<li>Machen Sie einen Rechtsklick auf den <b>GIS Cluster</b>-Knoten und wählen Sie <b>Execute</b> um den Knoten auszuführen.</li>
<li>Die Ergebnisse des Cluster-Algorithmus werden in der <b>ClusterID</b> Spalte gespeichert. Diese Spalte benutzen wir dann im <b>Tracing View</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/10.png"/></a>
<h5>11</h5>
<ul>
<li>Öffnen Sie den <b>Tracing View</b> per Doppelklick.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/11.png"/></a>
<h5>12</h5>
<ul>
<li>Sie sollten nun ein Fenster mit dem Liefernetz-Graphen sehen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/12.png"/></a>
<h5>13</h5>
<ul>
<li>Machen Sie einen Rechtsklick in den Graphen und wählen Sie <b>Collapse by Property</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/13.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/13.png"/></a>
<h5>14</h5>
<ul>
<li>Hier benutzen wir die <b>ClusterID</b>-Spalte mit den Ergebnissen vom <b>GIS Cluster</b>-Knoten.</li>
<li>Wählen Sie <b>ClusterID</b> und klicken Sie <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/14.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/14.png"/></a>
<h5>15</h5>
<ul>
<li>Klicken Sie einfach auf <b>OK</b>, da wir kein Cluster ausschließen wollen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/15.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/15.png"/></a>
<h5>16</h5>
<ul>
<li>Alle französischen Primärproduzenten wurden nun zu Gebieten geclustert.</li>
<li>Jede selektierte Meta-Station (blue circle) ist ein Gebiet in Frankreich.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/16.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/16.png"/></a>
<h5>17</h5>
<ul>
<li>Wählen Sie "Picking" als <b>Editing Mode</b> and klicken Sie an eine leere Stelle des Graphen um alle Station zu deselektieren.</li>
<li>Nun können Sie sehen, dass eine der Meta-Stationen gelb ist. Das bedeutet, dass dieses französische Gebiet eine Verbindung zu allen Ausbruchs-Stationen hat.</li>
<li>Klicken Sie <b>Switch to GIS</b> um zu schauen wo dieses Gebiet ist.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/17.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/17.png"/></a>
<h5>18</h5>
<ul>
<li>Das Gebiet befindet sich in Südfrankreich.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/18.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocluster/18.png"/></a>