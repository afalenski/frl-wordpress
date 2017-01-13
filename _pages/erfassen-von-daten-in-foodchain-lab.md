---
ID: 1041
post_title: >
  Erfassen von Daten in FoodChain-Lab Teil
  1
author: FRL_Admin
post_date: 2015-06-01 12:44:02
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/erfassen-von-daten-in-foodchain-lab/
published: true
---
<h4>Aufgaben</h4>
<ul>
<li>In diesem Tutorial werden wir zeigen, wie man mit unseren Excel-Templates Lieferdaten in FoodChain-Lab importiert.</li>
<li>Wir werden zunächst die initialen Daten der Ausbruchsorte importieren und dann sukzessive Daten von Caterern und anderen Lieferanten mit Hilfe von autogenerieten Rückwärts- und Vorwärts-Tracing-Templates hinzufügen.</li>
<li>In FoodChain-Lab ist es auch möglich das gesamte Liefernetz aus einer Excel-Datei zu importieren, aber dieses Feature wird hier nicht beschrieben. Das zugrundeliegende "All In One Template" kann heruntergeladen werden von: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/templates/All_In_One_Template.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
</ul>
<h5>1</h5>
<ul>
<li>Wählen Sie <b>Food-Lab > Open DB Gui...</b> in der Menüleiste um die Datenbank-Oberfläche zu öffnen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/1.png"/></a>
<h5>2</h5>
<ul>
<li>Die Datenbank-Oberfläche erscheint nun.</li>
<li>Hier können Sie Lieferdaten importieren, editieren und validieren.</li>
<li>Um den Import zu starten, müssen Sie das "Start Tracing Template" herunterladen, ausfüllen und importieren.</li>
<li>Das Template kann heruntergeladen werden unter: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/templates/Start_Tracing_Template.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/2.png"/></a>
<h5>3</h5>
<ul>
<li>Für dieses Tutorial haben wir bereits ein ausgefülltes  "Start Tracing Template" vorbereitet.</li>
<li>Downloaden sie es von <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/Start_Tracing_Caterers.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Im <b>Stations</b>-Blatt dieser Datei sind mehrere Bildungseinrichtungen (<b>Educational Institutions</b>) und zwei <b>Caterer</b> definiert.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/3.png"/></a>
<h5>4</h5>
<ul>
<li>Krankheitsfälle wurden in diesen Bildungseinrichtungen, welche von <b>Caterern</b> beliefert wurden, gemeldet.</li>
<li>Die Lieferungen von den <b>Caterern</b> an die Bildungseinrichtungen sind im <b>Deliveries</b>-Blatt definiert.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/4.png"/></a>
<h5>5</h5>
<ul>
<li>Um diese Datei zu importieren klicken Sie auf  <b>Table import</b> in der linken oberen Ecke des Datenbankfensters.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/5.png"/></a>
<h5>6</h5>
<ul>
<li>In dem Dateidialog, der erscheint, selektieren sie "StartTracing_Caterers.xlsx" und klicken Sie auf <b>Open</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/6.png"/></a>
<h5>7</h5>
<ul>
<li>Sie werden darüber benachrichtigt, dass der Import erfolgreich war.</li>
<li>Klicken Sie auf <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/7.png"/></a>
<h5>8</h5>
<ul>
<li>Sie werden bemerken, dass im Datenbankfenster nun Einträge in der zuvor leeren Tabelle zu sehen sind.</li>
<li>Nun wollen wir ein Rückwärts-Tracing von den Caterern aus durchführen, um zu sehen wo diese die Zutaten für die verschiedenen erworben haben.</li>
<li>Drücken sie den Button zum Erzeugen von Rückwärts-Tracing-Templates (siehe roter Kreis).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/8.png"/></a>
<h5>9</h5>
<ul>
<li>Da wir ein Rückwärts-Tracing für die Caterer durchführen wollen, wählen Sie nur <b>Caterer</b> und klicken sie auf <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/9.png"/></a>
<h5>10</h5>
<ul>
<li>In dem Dateidialog, der erscheint, können Sie den Ordner auswählen, in dem die generierten Templates gespeichert werden sollen.</li>
<li>Wählen oder erzeugen Sie den gewünschten Ordner und klicken Sie auf <b>Save</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/10.png"/></a>
<h5>11</h5>
<ul>
<li>Sie werden benachrichtigt, dass zwei Templates generiert wurden.</li>
<li>Klicken Sie auf <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/11.png"/></a>
<h5>12</h5>
<ul>
<li>Um dieses Tutorial kurz zu halten, werden wir nur die Lieferungen von einem Lieferanten eingeben, "Frozen Fruit Sales".</li>
<li>Geben Sie alle Informationen über "Frozen Fruit Sales" im <b>Stations</b>-Blatt der Datei "Backtrace_request_Caterer 1.xlsx" ein, wie im Screenshot zu sehen ist.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/12.png"/></a>
<h5>13</h5>
<ul>
<li>Wechseln Sie zum <b>BackTracing</b>-Blatt.</li>
<li>Im <b>Products Out</b>-Bereich sind alle Lieferungen zu "Caterer 1" gelistet.</li>
<li>Dies sind die Lieferungen, die wir aus "StartTracing_Caterers.xlsx" importiert haben.</li>
<li>Die Lieferungen gehören zu zwei Lots, "C1M1" und "C1M2".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/13.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/13.png"/></a>
<h5>14</h5>
<ul>
<li>Scrollen Sie in den <b>Ingredients for Lot(s)</b>-Bereich.</li>
<li>Hier können Sie alle Lieferungen eintragen, die "Caterer 1" empfangen hat und spezifizieren in welchen Lot die jeweilige Lieferung als Zutat gegangen ist.</li>
<li>Geben Sie alle Informationen der "Frozen Strawberries"-Lieferung von "Frozen Fruit Sales" ein (siehe Screenshot).</li>
<li>Speichern Sie das Dokument ("Backtrace_request_Caterer 1.xlsx").</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/14.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/14.png"/></a>
<h5>15</h5>
<ul>
<li>Nun öffnen Sie das andere generierte Template: "Backtrace_request_Caterer 2.xlsx".</li>
<li>Fügen Sie "Frozen Fruit Sales" zu dem <b>Stations</b>-Blatt hinzu, so wie Sie es beim ersten Template gemacht haben.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/15.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/15.png"/></a>
<h5>16</h5>
<ul>
<li>Wechseln Sie zum <b>BackTracing</b>-Blatt.</li>
<li>Geben Sie die zwei Lieferungen vom Screenshot im <b>Ingredients for Lot(s)</b>-Bereich ein.</li>
<li>Speichern Sie das Dokument ("Backtrace_request_Caterer 2.xlsx").</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/16.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/16.png"/></a>
<h5>17</h5>
<ul>
<li>Um die beiden Templates in die Datenbank zu importieren, klicken Sie den Button <b>Table import</b> in der linken oberen Ecke des Datenbank-Fensters.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/17.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/17.png"/></a>
<h5>18</h5>
<ul>
<li>Im Dateidialog, der erscheint, markieren Sie "Backtrace_request_Caterer 1.xlsx" und "Backtrace_request_Caterer 2.xlsx".</li>
<li>Dann klicken Sie auf <b>Open</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/18.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/18.png"/></a>
<h5>19</h5>
<ul>
<li>Sie bekommen eine Nachricht, dass der Import erfolgreich war.</li>
<li>Klicken Sie auf <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/19.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_datacollecting_1/19.png"/></a>