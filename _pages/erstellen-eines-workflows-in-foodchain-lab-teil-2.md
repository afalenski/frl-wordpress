---
ID: 790
post_title: >
  Erstellen eines Workflows in
  FoodChain-Lab Teil 2
author: FRL_Admin
post_date: 2015-03-18 10:42:51
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/erstellen-eines-workflows-in-foodchain-lab-teil-2/
published: true
---
<h4>Aufgaben</h4>
<ul>
<li>Nutzen Sie den <b>Tracing View</b> um das Liefernetz in einer übersichtlichen Art und Weise darzustellen.</li>
<li>Nutzen Sie das <b>Default Highlighting</b> zur farblichen Visualisierung.</li>
<li>Visualisieren Sie den Forward- und Backward-Trace von einer beliebigen Station.</li>
</ul>
<h5>1</h5>
<ul>
<li>Dies ist der zweite Teil des Tutorials.</li>
<li>Sie können den Workflow aus Teil 1 entweder selber erstellen oder hier herunterladen: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/MyFirstWorkflow.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Machen Sie einen Doppelklick auf den <b>Tracing View</b> um den Dialog zu öffnen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/1.png"/></a>
<h5>2</h5>
<ul>
<li>Im <b>Tracing View</b> sehen Sie das importierte Liefernetzwerk.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/2.png"/></a>
<h5>3</h5>
<ul>
<li>Um das Netzwerk übersichtlicher darzustellen machen Sie einen Rechtsklick in den Graphen und wählen Sie <b>Apply Layout > Fruchterman-Reingold</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/3.png"/></a>
<h5>4</h5>
<ul>
<li>Dieser Layout Prozess ist nicht deterministisch. Das heißt Sie bekommen jedes Mal ein anderes Ergebnis.</li>
<li>Sie können das Layout erneut berechnen lassen, falls Sie mit dem bisherigen Ergebnis nicht zufrieden sind.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/4.png"/></a>
<h5>5</h5>
<ul>
<li>Machen Sie einen Rechtsklick in den Graph um das Kontextmenü zu öffnen und wählen Sie <b>Set default Highlighting</b>.</li>
<li>Beim Highlighting werden bestimmte Attribute von Stationen/Lieferungen mit Hilfe von Farben und Größen visualisiert.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/5.png"/></a>
<h5>6</h5>
<ul>
<li>Sie werden bemerken, dass 4 Station nun rot gefärbt sind und manche Stationen größer sind als andere.</li>
<li>Die roten Stationen sind die Supermärkte, bei denen wir das Gewicht auf "1" gesetzt haben.</li>
<li>Die Größe jeder Station basiert nun auf ihrem "Score".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/6.png"/></a>
<h5>7</h5>
<ul>
<li>Aktivieren Sie <b>Show Legend</b> um eine Legende für die benutzen Farben zu erhalten.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/7.png"/></a>
<h5>8</h5>
<ul>
<li>Nun können wir eine Station als "Observed" markieren um uns ihren Trace anzeigen zu lassen.</li>
<li>Setzen Sie "Picking" als <b>Editing Mode</b> and machen Sie einen Doppelklick auf eine beliebige Station.</li>
<li>Wir haben auf die Station im roten Kreis geklickt.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/8.png"/></a>
<h5>9</h5>
<ul>
<li>Ein Dialog mit allen Attributen der gewählten Station erscheint.</li>
<li>Oben im Dialog können Sie die Werte für "Weight", "Cross Contamination", "Kill Contamination" und "Observed" verändern.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/9.png"/></a>
<h5>10</h5>
<ul>
<li>Aktivieren Sie <b>Observed</b> und klicken Sie <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/10.png"/></a>
<h5>11</h5>
<ul>
<li>Alle Stationen/Lieferungen vom Forward-Trace sind orange gefärbt and die Stationen/Lieferungen vom Backward-Trace sind magenta.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/11.png"/></a>
<h5>12</h5>
<ul>
<li>Klicken Sie an eine leere Stelle im Graphen um alle Stationen zu deselektieren.</li>
<li>Sie sehen nun, dass die als "Observed" markierte Station grün ist.</li>
<li>Aktivieren Sie außerdem "Join Deliveries" um den Graphen übersichtlicher zu gestalten. Lieferungen mit demselben Absender und Empfänger werden nun zusammengefasst.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_workflow_2/12.png"/></a>