---
ID: 778
post_title: Geo-Visualisierung in FoodChain-Lab
author: FRL_Admin
post_date: 2015-03-18 10:37:43
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/geo-visualisierung-in-foodchain-lab/
published: true
---
<h4>Aufgaben</h4>
<ul>
<li>Nutzen Sie folgenden Workflow: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Schauen Sie sich das Liefernetzwerk in der geographischen Ansicht vom <b>Tracing View</b> an.</li>
<li>Selektieren Sie alle Stationen in Polen und schauen Sie sich dann an wo sich diese Stationen in der graphischen Ansicht befinden.</li>
</ul>
<h5>1</h5>
<ul>
<li>Importieren Sie den Example Workflow von <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Öffnen Sie den <b>Tracing View</b> per Doppelklick.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/1.png"/></a>
<h5>2</h5>
<ul>
<li>Nun sehen Sie eine graphische Repräsentation des Liefernetzes.</li>
<li>Um zur geographischen Repräsentation zu wechseln wählen Sie <b>Switch to GIS</b> rechts oben.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/2.png"/></a>
<h5>3</h5>
<ul>
<li>Zur geographischen Visualisierung werden die Umrisse von Staaten genutzt, welche aus der Shapefile gelesen wurden.</li>
<li>Um auf auf ein bestimmtes Gebiet zu zoomen wählen Sie "Transforming" als <b>Editing Mode</b> und nutzen Sie das Mausrad und die linke Maustaste zum Zoomen und Bewegen des Graphen (funktioniert wie in Google Maps).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/3.png"/></a>
<h5>4</h5>
<ul>
<li>Falls Sie mit dem Internet verbunden sind, können Sie die Art der Visualisierung ändern.</li>
<li>Wählen Sie "Mapnik" als <b>GIS Type</b>.</li>
<li>Nun sehen Sie eine Visualisierung mit OpenStreetMap Daten.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/4.png"/></a>
<h5>5</h5>
<ul>
<li>Wir können nun Station aufgrund ihrer geographischen Lage auswählen.</li>
<li>Setzen Sie "Picking" als <b>Editing Mode</b> and wählen Sie alle Stationen in Polen aus, indem Sie ein Rechteck um diese Stationen ziehen.</li>
<li>The gewählten Stationen sollten nun blau markiert sein.</li>
<li>Wechseln Sie zurück zur graphischen Ansicht, indem Sie rechts oben <b>Switch to Graph</b> klicken.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/5.png"/></a>
<h5>6</h5>
<ul>
<li>Die blauen Stationen sind dieselben Stationen, die Sie in der geographischen Ansicht ausgewählt haben.</li>
<li>Denn Änderungen, die Sie in einer Ansicht machen, werden automatisch auf die andere Ansicht übertragen.</li>
<li>Das macht es einfach zwischen beiden Ansichten hin und her zu wechseln, um die Vorteile der jeweiligen Ansicht zu nutzen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/6.png"/></a>
<h5>7</h5>
<ul>
<li>Nun wählen wir ein "Cluster" von Stationen in der graphischen Ansicht und schauen uns dann die geographische Lage der Stationen an.</li>
<li>Also wählen Sie das "Cluster" im roten Kreis und klicken Sie <b>Switch to GIS</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/7.png"/></a>
<h5>8</h5>
<ul>
<li>Wie Sie sehen, sind die Stationen des Clusters über Frankreich verteilt.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geoview/8.png"/></a>