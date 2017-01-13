---
ID: 1477
post_title: >
  Erfassen von Daten in FoodChain-Lab Teil
  2
author: FRL_Admin
post_date: 2015-11-10 15:14:08
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/erfassen-von-daten-in-foodchain-lab-teil-2/
published: true
---
<h4>Aufgaben</h4>
<ul>
<li>In diesem Teil des Tutorials werden wir ein Rückwärts- and Vorwärts-Tracing für "Frozen Fruit Sales" ausführen.</li>
<li>Sie müssen entweder erst Teil 1 des Tutorials bearbeiten oder folgende Dateien in eine leere Datenbank importieren, bevor sie mit diesem Teil des Tutorials starten.</li>
<li>Start Template: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/Start_Tracing_Caterers.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a></li>
<li>Caterer 1 Template: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/Backtrace_request_Caterer 1.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a></li>
<li>Caterer 2 Template: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/Backtrace_request_Caterer 2.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a></li>
</ul>
<h5>1</h5>
<ul>
<li>Sie sollten das Datenbank-Fenster geöffnet haben.</li>
<li>Drücken Sie den Button zum Generieren von Ruckwärts-Templates (roter Kreis).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/1.png"/></a>
<h5>2</h5>
<ul>
<li>Da wir ein Rückwärts-Tracing für den Lieferanten (Supplier) "Frozen Fruit Sales" durchführen wollen, wählen Sie nur <b>Supplier</b> und klicken sie auf <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/2.png"/></a>
<h5>3</h5>
<ul>
<li>In dem Dateidialog, der erscheint, können Sie den Ordner auswählen, in dem die generierten Templates gespeichert werden sollen.</li>
<li>Wählen oder erzeugen Sie den gewünschten Ordner und klicken Sie auf <b>Save</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/3.png"/></a>
<h5>4</h5>
<ul>
<li>Sie werden benachrichtigt, dass ein Template generiert wurden.</li>
<li>Klicken Sie auf <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/4.png"/></a>
<h5>5</h5>
<ul>
<li>Öffnen Sie das generierte Template "Backtrace_request_Frozen Fruit Sales.xlsx".</li>
<li>Fügen Sie die Stationen vom Screenshot zum <b>Stations</b>-Blatt hinzu.</li>
<li>Diese Stationen beinhalten 3 Erdbeer-Lieferanten, die Erdbeeren an "Frozen Fruit Sales" geliefert haben, und einen Caterer, der Erdbeeren bekommen hat.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/5.png"/></a>
<h5>6</h5>
<ul>
<li>Im <b>BackTracing</b>-Blatt können Sie die drei ausgehenden Lieferungen von "Frozen Fruit Sales" sehen.</li>
<li>Diese Lieferungen gehören zu den Lots "108" und "139".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/6.png"/></a>
<h5>7</h5>
<ul>
<li>Nun scrollen Sie zu dem <b>Ingredients for Lot(s)</b>-Bereich.</li>
<li>Tragen Sie die drei Lieferungen, welche als Zutaten für Lot "108" benutzt wurden, ein (siehe Screenshot).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/7.png"/></a>
<h5>8</h5>
<ul>
<li>Lot "108" wurde nicht nur an "Caterer 1" und "Caterer 2" geliefert, sondern auch an einen dritten Caterer.</li>
<li>Wir können diese Information im <b>ForwardTracing_Opt</b>-Blatt eintragen.</li>
<li>Tragen Sie die Lieferung an "Caterer 3" ein (siehe Screenshot).</li>
<li>Speichern Sie das Dokument ("Backtrace_request_Frozen Fruit Sales.xlsx").</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/8.png"/></a>
<h5>9</h5>
<ul>
<li>Um das Dokument zu importieren, klicken Sie auf den Button <b>Table import</b> in der linken oberen Ecke des Datenbank-Fensters.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/9.png"/></a>
<h5>10</h5>
<ul>
<li>Im Dateidialog, der erscheint, wählen Sie "Backtrace_request_Frozen Fruit Sales.xlsx" und klicken Sie auf <b>Open</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/10.png"/></a>
<h5>11</h5>
<ul>
<li>Sie werden benachrichtigt, dass es Warnungen beim Import gab.</li>
<li>Klicken Sie auf <b>Show Details</b> um sich diese Warnungen anzuschauen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/11.png"/></a>
<h5>12</h5>
<ul>
<li>730kg Erdbeeren sind in Lot "108" gegangen, aber alle Lieferungen von gefrorenen Erdbeeren aus Lot "108" summieren sich nur zu 99,75kg.</li>
<li>Warnungen wie diese, sollen helfen Fehler in den importierten Daten zu finden.</li>
<li>Diesmal ignorieren wir die Warnung einfach mal. Klicken Sie auf <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/12.png"/></a>
<h5>13</h5>
<ul>
<li>Wir wissen, dass Lot "108" auch an "Caterer 3" geliefert wurde und haben diese Lieferung in die Datenbank importiert.</li>
<li>Nun werden wir ein Vorwärts-Tracing für "Caterer 3" durchführen um zu schauen, wer noch mit ggf. kontaminierten Erdbeeren beliefert wurde.</li>
<li>Drücken Sie den Button zum Generieren des Vorwärts-Templates für eine spezifische Station (roter Kreis).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/13.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/13.png"/></a>
<h5>14</h5>
<ul>
<li>In dem Dialog, der erscheint, müssen Sie die Station auswählen, für die das Template generiert werden soll.</li>
<li>Geben "cate" in das Textfeld neben <b>Enter Search Query</b> ein und in der Tabelle darunter werden nur noch die Caterer zu sehen sein.</li>
<li>Drücken sie den <b>Select</b>-Button für "Caterer 3".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/14.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/14.png"/></a>
<h5>15</h5>
<ul>
<li>In dem Dateidialog, der erscheint, können Sie den Ordner auswählen, in dem die generierten Templates gespeichert werden sollen.</li>
<li>Wählen oder erzeugen Sie den gewünschten Ordner und klicken Sie auf <b>Save</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/15.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/15.png"/></a>
<h5>16</h5>
<ul>
<li>Sie werden benachrichtigt, dass ein Template generiert wurde.</li>
<li>Klicken Sie auf <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/16.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/16.png"/></a>
<h5>17</h5>
<ul>
<li>Öffnen Sie "StationFwdtrace_request_Caterer 3.xlsx".</li>
<li>Tragen Sie die Station vom Screenshot im <b>Stations</b>-Blatt ein.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/17.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/17.png"/></a>
<h5>18</h5>
<ul>
<li>Im <b>FwdTracing</b>-Blatt müssen Sie als erstes alle relevanten ausgehenden Lots von "Caterer 3" eintragen. Fügen Sie Lot "C3M1" im <b>Lot Information</b>-Bereich hinzu (rote Box im Screenshot).</li>
<li>Nun können Sie spezifizieren, dass die "Frozen Strawberries"-Lieferung als Zutat für dieses Lot genutzt wurde (roter Kreis).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/18.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/18.png"/></a>
<h5>19</h5>
<ul>
<li>Scrollen Sie runter zum <b>Products Out</b>-Bereich um die ausgehenden Lieferungen von Lot "C3M1" zu spezifizieren.</li>
<li>Fügen Sie die beiden Lieferungen aus dem Screenshot hinzu (rote Box).</li>
<li>Speichern Sie das ausgefüllte Dokument ("StationFwdtrace_request_Caterer 3.xlsx").</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/19.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/19.png"/></a>
<h5>20</h5>
<ul>
<li>Um das Dokument in die Datenbank zu importieren, klicken Sie den Button <b>Table import</b> in der linken oberen Ecke des Datenbank-Fensters.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/20.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/20.png"/></a>
<h5>21</h5>
<ul>
<li>Im Dateidialog, der erscheint, markieren Sie "StationFwdtrace_request_Caterer 3.xlsx" und klicken Sie auf <b>Open</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/21.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/21.png"/></a>
<h5>22</h5>
<ul>
<li>Sie bekommen eine Nachricht, dass der Import erfolgreich war.</li>
<li>Klicken Sie auf <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/22.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_2/22.png"/></a>