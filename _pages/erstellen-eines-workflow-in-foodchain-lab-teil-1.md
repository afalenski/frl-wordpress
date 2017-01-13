---
ID: 787
post_title: >
  Erstellen eines Workflows in
  FoodChain-Lab Teil 1
author: FRL_Admin
post_date: 2015-03-18 10:41:32
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/erstellen-eines-workflow-in-foodchain-lab-teil-1/
published: true
---
<h4>Aufgaben</h4>
<ul>
<li>Importieren Sie das Beispiel-Excel-Template von: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/FCL_Example.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a></li>
<li>Vergeben mit Hilfe des <b>Tracing</b>-Knotens ein Gewicht ("Weight") von "1" an die Supermärkte in Hamburg, Karlsruhe, Ingolstadt und Hanover um diese als Ausbruchsorte zu markieren.</li>
<li>Nutzen Sie den <b>Tracing View</b> um das Liefernetz zu visualisieren.</li>
</ul>
<h5>1</h5>
<ul>
<li>Wählen Sie <b>Food-Lab > Open DB Gui...</b> in der Menüleiste um das Datenbank-Fenster zu öffnen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/1.png"/></a>
<h5>2</h5>
<ul>
<li>Falls Sie eine Meldung bekommen, dass eine interne Datenbank erstellt wurde, klicken Sie <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/2.png"/></a>
<h5>3</h5>
<ul>
<li>Im Datenbank-Fenster klicken Sie den <b>Table import</b>-Button links oben.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/3.png"/></a>
<h5>4</h5>
<ul>
<li>Es öffnet sich nun ein Dateidialog, in dem *.xlsx Dateien im FoodChain-Lab Format ausgewählt werden können.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/4.png"/></a>
<h5>5</h5>
<ul>
<li>Laden Sie die Beispieldatei von <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/FCL_Example.xlsx" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Wählen Sie diese Datei im Dialog aus und drücken Sie <b>Open</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/5.png"/></a>
<h5>6</h5>
<ul>
<li>When der Import beendet ist, werden Sie einen Dialog mit Fehlern/Warnungen sehen, die beim Importieren aufgetreten sind.</li>
<li>Es sind keine Fehler aufgetreten, also drücken Sie einfach <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/6.png"/></a>
<h5>7</h5>
<ul>
<li>Im Datenbank-Fenster können Sie sich die importierten Daten nun anschauen, nach Duplikaten suchen usw..</li>
<li>Schließen Sie den Dialog.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/7.png"/></a>
<h5>8</h5>
<ul>
<li>Nun werden wir einen Workflow erzeugen, der die importierten Daten nutzt.</li>
<li>Machen Sie einen Rechtsklick auf <b>LOCAL</b> im <b>KNIME Explorer</b> and wählen Sie <b>New KNIME Workflow...</b></li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/8.png"/></a>
<h5>9</h5>
<ul>
<li>Im erscheinenden Dialog wählen Sie als Name "MyFirstWorkflow" and klicken Sie <b>Finish</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/9.png"/></a>
<h5>10</h5>
<ul>
<li>Der erzeugte Workflow wird im Editor in der Mitte des Fensters erscheinen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/10.png"/></a>
<h5>11</h5>
<ul>
<li>Ziehen Sie den <b>Supply Chain Reader</b> aus dem <b>Node Repository</b> in den Workflow.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/11.png"/></a>
<h5>12</h5>
<ul>
<li>Der <b>Supply Chain Reader</b> muss nicht konfiguriert werden.</li>
<li>Also machen Sie einen Rechtsklick auf den Knoten und wählen Sie <b>Execute</b> um den Knoten auszuführen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/12.png"/></a>
<h5>13</h5>
<ul>
<li>Der <b>Supply Chain Reader</b> hat nun alle Daten aus der internen Datenbank gelesen.</li>
<li>Selektieren Sie den <b>Supply Chain Reader</b> im Workflow (sodass ein Rechteck um den Knoten erscheint) und machen Sie einen Doppelklick auf den <b>Tracing</b>-Knoten im <b>Node Repository</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/13.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/13.png"/></a>
<h5>14</h5>
<ul>
<li>Der <b>Tracing</b>-Knoten sollte nun im Workflow erscheinen and alle Eingabe-Ports sollten automatisch mit dem <b>Supply Chain Reader</b> verbunden werden.</li>
<li>Machen Sie einen Doppelklick auf den <b>Tracing</b>-Knoten um diesen zu konfigurieren.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/14.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/14.png"/></a>
<h5>15</h5>
<ul>
<li>Im oberen Bereich des Dialogs sehen Sie die Tabs für die "Station/Delivery Properties".</li>
<li>Es können jeweils "Weight", "Cross Contamination" und "Kill Contamination" gesetzt werden. Basierend darauf wird für jede Station/Lieferung ein "Score" berechnet.</li>
<li>Zusätzlich können Stationen/Lieferungen mit dem Attribut "Observed" versehen werden.</li>
<li>Wählen Sie <b>Station Properties</b> und dann <b>Weight</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/15.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/15.png"/></a>
<h5>16</h5>
<ul>
<li>Eine Tabelle mit allen verfügbaren Stationen erscheint.</li>
<li>Das Gewicht ("Weight") kann in der ganz linken Spalte vergeben werden.</li>
<li>Da es sehr ineffizient ist durch eine so große Anzahl von Station zu scrollen, können wir einen Filter setzen um nur die gewünschten Station anzeigen zu lassen.</li>
<li>Klicken Sie auf <b>Set Filter</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/16.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/16.png"/></a>
<h5>17</h5>
<ul>
<li>In diesem Dialog können Sie festlegen, welche Stationen in der Tabelle erscheinen sollen.</li>
<li>Klicken Sie auf den rot markierten Button und den Wert für <b>Property</b> zu ändern.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/17.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/17.png"/></a>
<h5>18</h5>
<ul>
<li>Wählen Sie "type of business".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/18.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/18.png"/></a>
<h5>19</h5>
<ul>
<li>Wir wollen nur für Supermärkte Gewichte vergeben, da dort kontaminierte Produkte gefunden wurden.</li>
<li>Wählen Sie "Supermarket" bei <b>Value</b> und klicken Sie <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/19.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/19.png"/></a>
<h5>20</h5>
<ul>
<li>Nun sehen Sie nur Supermärkte in der Tabelle.</li>
<li>Vergeben Sie ein Gewicht von "1" an die Supermärkte in "Hamburg", "Karlsruhe", "Ingolstadt" und "Hanover", da dort kontaminierte Produkte gefunden wurden.</li>
<li>Klicken Sie auf <b>OK</b> um die Eingabe zu beenden.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/20.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/20.png"/></a>
<h5>21</h5>
<ul>
<li>Machen Sie einen Rechtsklick auf den <b>Tracing</b>-Knoten und wählen Sie <b>Execute</b> um den Knoten auszuführen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/21.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/21.png"/></a>
<h5>22</h5>
<ul>
<li>Ziehen Sie den <b>Tracing View</b> aus dem <b>Node Repository</b> in den Workflow.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/22.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/22.png"/></a>
<h5>23</h5>
<ul>
<li>Verbinden Sie die Ausgabe-Ports des <b>Tracing</b>-Knotens mit den beiden ersten Eingabe-Ports vom <b>Tracing View</b>.</li>
<li>Verbinden Sie den dritten Ausgabe-Port vom <b>Supply Chain Reader</b> mit dem dritten Eingabe-Port vom <b>Tracing View</b>.</li>
<li>Nun öffnen Sie den <b>Tracing View</b> and analysieren Sie die Daten. Dies wird im zweiten Teil des Tutorials gezeigt.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/23.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_1/23.png"/></a>