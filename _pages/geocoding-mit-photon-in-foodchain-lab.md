---
ID: 2449
post_title: Geocoding mit Photon in FoodChain-Lab
author: FRL_Admin
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/geocoding-mit-photon-in-foodchain-lab/
published: true
post_date: 2017-11-07 17:06:00
---
<h4>Aufgaben</h4>
<ul>
<li>Führen Sie ein Geocoding auf Basis folgenden Workflows durch: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/Geocoding_with_Photon.knwf" target="_blank">https://github.com/SiLeBAT/BfROpenLa...</a>.</li>
<li>Fügen Sie den <b>FoodChain-Lab</b> <b>Geocoding</b> Knoten hinzu.</li>
<li>Verwenden Sie den Photon Geocoding Service.</li>
</ul>
<h5>1</h5>
<ul>
<li>Importieren Sie den Geocoding Workflow von <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/Geocoding_with_Photon.knwf" target="_blank">https://github.com/SiLeBAT/BfROpenLa...</a>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/1.png"/></a>
<h5>2</h5>
<ul>
<li>Um den Geocoding Service zu nutzen muss der <b>FoodChain-Lab</b> <b>Geocoding</b> Knoten hinzugefügt werden.</li>
<li>Fügen Sie den <b>FoodChain-Lab</b> <b>Geocoding</b> Knoten hinzu durch einen Doppelklick darauf im <b>Node Repository</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/2.png"/></a>
<h5>3</h5>
<ul>
<li>Ein <b>Geocoding</b> Knoten wurde zum Workflow hinzugefügt. Er ist verbunden mit dem <b>SupplyChainReader</b> und muss konfiguriert werden.</li>
<li>Öffnen Sie den Konfigurationsdialog durch einen Doppelklick auf den Knoten oder durch Benutzung des Kontextmenüs (Rechtsklick auf den Knoten).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/3.png"/></a>
<h5>4</h5>
<ul>
<li>Setzen Sie den <b>Service Provider</b> auf <b>Photon</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/4.png"/></a>
<h5>5</h5>
<ul>
<li>Die <b>Address</b> ist passend gesetzt.</li>
<li>Sie müssen die <b>Server Address</b> eingeben. Dafür können Sie <b>http://photon.komoot.de</b> nutzen, einen öffentlich verfügbaren Dienst.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/5.png"/></a>
<h5>6</h5>
<ul>
<li>Es passiert häufig, dass der Geocoding Service zu einer Anfrage mehrere Resultate liefert (z.B. wenn es mehrere Straßen mit demselben Name in einer Stadt gibt).</li>
<li>Wir müssen definieren was in diesem Fall passieren soll: kein Resultat nehmen, das erste Resultat nehmen oder das passende Resultat manuell auswählen.</li>
<li>Manuelles Auswählen ist bei großen Datenmengen sehr arbeitsaufwendig, deshalb wählen wir hier einfach <b>Use first</b> und klicken <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/6.png"/></a>
<h5>7</h5>
<ul>
<li>Machen Sie einen Rechtsklick auf den <b>Geocoding</b>-Knoten und wählen Sie <b>Execute</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/7.png"/></a>
<h5>8</h5>
<ul>
<li>Die Ausführung kann eine Weile dauern.</li>
<li>Unter dem Knoten wird angezeigt welcher Prozentsatz der Daten bereits bearbeitet wurde.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/8.png"/></a>
<h5>9</h5>
<ul>
<li>Wenn die Ausführung beendet ist, können wir uns die Resultate anschauen.</li>
<li>Machen Sie einen Rechtsklick auf den <b>Geocoding</b>-Knoten und wählen Sie <b>Coordinates</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/9.png"/></a>
<h5>10</h5>
<ul>
<li>In dem Dialog können Sie sich die gesamte Datentabelle anschauen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/10.png"/></a>
<h5>11</h5>
<ul>
<li>Scrollen Sie ganz nach rechts um sich die Spalten mit geographischer Breite und Länge anzuschauen (die zwei Spalten ganz rechts).</li>
<li>Eine Geocoding Anfragn lieferte keine Ergebnisse.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding_with_photon/11.png"/></a>