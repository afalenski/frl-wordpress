---
ID: 609
post_title: Einführung in FoodChain-Lab
author: FRL_Admin
post_date: 2015-03-05 14:49:34
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/foodchain-lab-uberblick/
published: true
---
<h4>FoodChain-Lab Konzepte 1</h4>
<ul>
<li><b>Delivery (Lieferung)</b>: Wird von A nach B an einem bestimmten Datum versendet. Eine Lieferung kann Folgelieferungen und vorhergehende Lieferungen haben (z.B. Erdbeer-Lieferung -> Erdbeerkuchen-Lieferung).</li>
<li><b>Station</b>: Lebensmittelunternehmen oder Person, das/die Lieferungen empfängt und/oder versendet.</li>
<li><b>Trace</b>: Pfad, den eine Kontamination nehmen kann. Eine Station/Lieferung "B" ist auf dem <b>Forward Trace</b> von einer Station/Lieferung "A", falls sich eine Kontamination über das Liefernetz von "A" nach "B" ausbreiten kann. Wenn "B" auf dem <b>Forward Trace</b> von "A" ist, dann ist "A" auf dem <b>Backward Trace</b> von "B".</li>
</ul>
<h4>FoodChain-Lab Konzepte 2</h4>
<ul>
<li><b>Weight (Gewicht)</b>: Wird an Stationen/Lieferungen vergeben, die in einen Ausbruch involviert sind (z.B. ein Restaurant in dem Kunden infiziert wurden). Verschiedene Gewichte können benutzt werden, um Unterschiede zwischen den involvierten Stationen/Lieferungen zu modellieren (z.B. höheres Gewicht = größere Wahrscheinlichkeit, dass Station/Lieferung involviert ist).</li>
<li><b>Cross Contamination (Kreuzkontamination)</b>: Kontamination ausgehender Lieferungen durch eingehende Lieferungen (bei Stationen). Wird Kreuzkontamination auf Lieferungen angewendet, bedeutet das, dass die gewählten eingehenden Lieferungen einer Station ihre Folgelieferungen kontaminieren.</li>
<li><b>Kill Contamination</b>: Wenn auf Station/Lieferung angewendet, wird jede Kontamination dort entfernt, sodass diese nicht auf Nachfolgelieferungen und -stationen überspringen kann.</li>
<li><b>Score</b>: Wird auf Basis der vergebenen Gewichte und Kreuzkontamination berechnet. Soll helfen, die Wahrscheinlichkeit abzuschätzen, dass eine Station/Lieferung die Quelle des Ausbruchs ist (höherer Score = höhere Wahrscheinlichkeit, dass Quelle des Ausbruchs).</li>
</ul>
<h4>FoodChain-Lab Score Berechnung 1</h4>
<ul>
<li>s<sub>i</sub>: i-te Station oder Lieferung</li>
<li>w<sub>j</sub>: Gewicht ("Weight") der j-ten Station oder Lieferung</li>
<li>t<sub>ij</sub>: hat einen Wert von 1, falls es einen Trace von s<sub>i</sub> nach s<sub>j</sub> gibt, ansonsten 0</li>
<li>n: Anzahl aller Stationen und Lieferungen</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/score.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/score.png"/></a>
<h4>FoodChain-Lab Score Berechnung 2</h4>
<ul>
<li>FoodChain-Lab erlaubt auch negative Gewichte an Station/Lieferungen zu vergeben.</li>
<li>Ein negatives Gewicht soll andeuten, dass eine Station/Lieferung nicht an einem Ausbruch beteiligt ist.</li>
<li>Wenn negative Gewichte verwendet werden, erfolgt die Score-Berechnung wie hier zu sehen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/new_score.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/new_score.png"/></a>
<h4>KNIME-Einführung</h4>
<ul>
<li>KNIME ist eine Open Source Datenanalyse-Platform, die es dem Nutzer erlaubt Daten-Pipelines (sogenannte "Workflows") zu bauen</li>
<li>Ein Workflow wird erstellt indem Knoten aus dem <b>Node Repository</b> in den <b>Workflow Editor</b> gezogen und verbunden werden (<a href="https://tech.knime.org/workbench" target="_blank">https://tech.knime.org/workbench</a>).</li>
<li>Knoten sind Datenverarbeitungs-Einheiten mit Ein- und/oder Ausgabe-Ports.</li>
<li>Daten können über eine Verbindung vom Ausgabe-Port zum Eingabe-Port eines anderen Knotens übermittelt werden.</li>
<li>Ausführlicher KNIME quickstart guide: <a href="https://tech.knime.org/files/KNIME_quickstart.pdf" target="_blank">https://tech.knime.org/files/KNIME_qu...</a>.</li>
<li>Einführungsvideo zu KNIME: <a href="https://www.youtube.com/watch?v=ft7Ksgss3Tc" target="_blank">https://www.youtube.com/watch?v=ft7Ks...</a>.</li>
</ul>
<h4>Verfügbare Knoten</h4>
<ul>
<li>Die detaillierten Beschreibungen aller Knoten finden Sie in der <b>Node Description</b> in KNIME (<a href="https://tech.knime.org/workbench" target="_blank">https://tech.knime.org/workbench</a>).</li>
<li>Eingehende und ausgehende Daten sind entweder Daten-Tabellen (repräsentiert durch Dreiecke an den Knoten) oder Bilder (repräsentiert durch grüne Quadrate). Diese Datentypen werden standardmäßig in KNIME verwendet (z.B. beim <b>Row Filter</b> oder <b>Image Port Writer</b>), so dass KNIME-Knoten ebenfalls in FoodChain-Lab-Workflows verwendet werden können.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/1.png"/></a>
<h4>Tracing</h4>
<ul>
<li>Daten zu Lieferketten werden aus der internen Datenbank mit dem <b>Supply Chain Reader</b> in den Workflow geladen.</li>
<li>Diese Daten können mit dem <b>Tracing View</b> visualisiert werden. Außerdem kann der <b>Tracing View</b> auch ein Tracing auf den Daten durchführen.</li>
<li>Der <b>Tracing</b>-Knoten erlaubt es ein Tracing ohne Visualisierung durchzuführen (z.B. als Vorverarbeitungsschritt für den <b>Tracing View</b>).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/2.png"/></a>
<h4>Verwenden von Geodaten</h4>
<ul>
<li>Der <b>Geocoding</b> Knoten ermittelt anhand von Adressen die geographische Breite und Länge.</li>
<li>Mit diesen Daten können dann im <b>GIS Cluster</b>-Knoten "Cluster" (regionale Zusammenhänge) errechnet werden.</li>
<li>Der Tracing View kann die Lieferketten auf einer Landkarte visualisieren, welche aus einer ESRI-Shapefile mit dem <b>Shapefile Reader</b> eingelesen wird.</li>
<li>ESRI-Shapefiles für Deutschland sind frei verfügbar unter: <a href="http://www.geodatenzentrum.de/geodaten/gdz_rahmen.gdz_div?gdz_akt_zeile=5" target="_blank">http://www.geodatenzentrum.de/geodate...</a></li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_overview/3.png"/></a>