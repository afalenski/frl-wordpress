---
ID: 773
post_title: Geocoding in FoodChain-Lab
author: FRL_Admin
post_date: 2015-03-18 10:35:25
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/geocoding-in-foodchain-lab-2/
published: true
---
<h4>Aufgaben</h4>
<ul>
<li>Führen Sie ein Geocoding auf Basis folgenden Workflows durch: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/Geocoding.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Nutzen "Street", "HouseNumber", "City" und "Country" als Eingabeparameter für das Geocoding.</li>
<li>Verwenden Sie den MapQuest Geocoding Service.</li>
</ul>
<h5>1</h5>
<ul>
<li>Importieren Sie den Geocoding Workflow von <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/Geocoding.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>In diesem Tutorial benutzen wir den MapQuest Geocoding Service.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/1.png"/></a>
<h5>2</h5>
<ul>
<li>Für MapQuest müssen Sie sich registrieren und einen App-Key erstellen unter: <a href="https://developer.mapquest.com" target="_blank">https://developer.mapquest.com</a></li>
<li>Dieser App-Key muss in den KNIME-Einstellungen eingegeben werden.</li>
<li>Wählen Sie <b>File < Preferences</b> in der Menüleiste.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/2.png"/></a>
<h5>3</h5>
<ul>
<li>Nun erscheint der Einstellungs-Dialog.</li>
<li>Hier können Sie alle Einstellungen für KNIME und FoodChain-Lab vornehmen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/3.png"/></a>
<h5>4</h5>
<ul>
<li>Wählen Sie <b>KNIME < Geocoding</b> im Navigations-Baum auf der linken Seite.</li>
<li>Geben Sie ihren <b>MapQuest Application Key</b> ein und klicken Sie <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/4.png"/></a>
<h5>5</h5>
<ul>
<li>Um das Geocoding auszuführen benötigen wir eine Spalte mit Adressen. Der <b>Supply Chain Reader</b> gibt allerdings alle Teile der Adresse (Straße, Stadt, ...) in verschiedenen Spalten aus.</li>
<li>Die Adress-Spalte wir mit dem <b>Address Creator</b>-Knoten erstellt.</li>
<li>Machen Sie einen Doppelklick auf diesen Knoten um den Konfigurationsdialog zu öffnen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/5.png"/></a>
<h5>6</h5>
<ul>
<li>In diesem Dialog können Sie definieren welche Spalten für die Adress-Spalte benutzt werden sollen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/6.png"/></a>
<h5>7</h5>
<ul>
<li>Da wir das Geocoding basierend auf "Street", "HouseNumber", "City" and "Country" durchführen wollen, müssen wir <b>Country Column</b> auf "Country" setzen und <b>Postal Code Column</b> auf "none"</li>
<li>Klicken Sie <b>OK</b> um den Dialog zu schließen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/7.png"/></a>
<h5>8</h5>
<ul>
<li>Da wir die Einstellungen geändert haben, muss der Knoten resettet werden.</li>
<li>Klicken Sie <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/8.png"/></a>
<h5>9</h5>
<ul>
<li>Wir haben den <b>Address Creator</b> nun passend konfiguriert und ihn neu ausführen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/9.png"/></a>
<h5>10</h5>
<ul>
<li>Machen Sie einen Rechtsklick auf den <b>Address Creator</b> und wählen Sie <b>Execute</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/10.png"/></a>
<h5>11</h5>
<ul>
<li>Nun können wir das Geocoding konfigurieren.</li>
<li>Machen Sie einen Doppelklick auf den <b>Geocoding</b>-Knoten um den Dialog zu öffnen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/11.png"/></a>
<h5>12</h5>
<ul>
<li>Hier können Sie welchen <b>Service Provider</b> Sie nutzen möchten und welche Spalte die Adressen enthält.</li>
<li>Beide Einstellungen sind bereits korrekt, also brauchen wir hier nichts ändern.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/12.png"/></a>
<h5>13</h5>
<ul>
<li>Es passiert häufig, dass der Geocoding Service zu einer Anfrage mehrere Resultate liefert (z.B. wenn es mehrere Straßen mit demselben Name in einer Stadt gibt).</li>
<li>Wir müssen definieren was in diesem Fall passieren soll: kein Resultat nehmen, das erste Resultat nehmen oder das passende Resultat manuell auswählen.</li>
<li>Manuelles Auswählen ist bei großen Datenmengen sehr arbeitsaufwendig, deshalb wählen wir hier einfach <b>Use first</b> und klicken <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/13.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/13.png"/></a>
<h5>14</h5>
<ul>
<li>Machen Sie einen Rechtsklick auf den <b>Geocoding</b>-Knoten und wählen Sie <b>Execute</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/14.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/14.png"/></a>
<h5>15</h5>
<ul>
<li>Die Ausführung kann eine Weile dauern.</li>
<li>Unter dem Knoten wird angezeigt welcher Prozentsatz der Daten bereits bearbeitet wurde.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/15.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/15.png"/></a>
<h5>16</h5>
<ul>
<li>Wenn die Ausführung beendet ist, können wir uns die Resultate anschauen.</li>
<li>Machen Sie einen Rechtsklick auf den <b>Geocoding</b>-Knoten und wählen Sie <b>Coordinates</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/16.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/16.png"/></a>
<h5>17</h5>
<ul>
<li>In dem Dialog können Sie sich die gesamte Datentabelle anschauen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/17.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/17.png"/></a>
<h5>18</h5>
<ul>
<li>Scrollen Sie ganz nach rechts um sich die Spalten mit geographischer Breite und Länge anzuschauen (die zwei Spalten ganz rechts).</li>
<li>Bei mehrere Geocoding Anfragen haben wir falsche Ergebnisse. MapQuest hat Koordinaten für die USA geliefert, obwohl alle Addressen aus Deutschland sind.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/18.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_geocoding/18.png"/></a>