---
ID: 766
post_title: Clustering in FoodChain-Lab
author: FRL_Admin
post_date: 2015-03-18 10:32:26
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/clustering-in-foodchain-lab-2/
published: true
---
<h4>Aufgaben</h4>
<ul>
<li>Nutzen Sie folgenden Workflow: <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a></li>
<li>Clustern Sie alle französischen Primärproduzenten basierend auf dem Attribut "City".</li>
<li>Das bedeutet alle Stationen aus derselben Stadt werden in eine Meta-Station gepackt.</li>
</ul>
<h5>1</h5>
<ul>
<li>Importieren Sie den Beispiel-Workflow von <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
<li>Öffnen Sie den <b>Tracing View</b> per Doppelklick.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/1.png"/></a>
<h5>2</h5>
<ul>
<li>Ein Fenster mit dem Graphen des Liefernetzes sollte erscheinen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/2.png"/></a>
<h5>3</h5>
<ul>
<li>Machen Sie einen Rechtsklick in den Graphen und wählen Sie <b>Set Selected Stations</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/3.png"/></a>
<h5>4</h5>
<ul>
<li>Sie sollten jetzt diesen Dialog sehen.</li>
<li>Klicken Sie auf den rot markierten Button um für <b>Property</b> einen anderen Wert zu wählen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/4.png"/></a>
<h5>5</h5>
<ul>
<li>Wählen Sie "Country".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/5.png"/></a>
<h5>6</h5>
<ul>
<li>Nun wählen Sie "FR" als <b>Value</b>, da wir ja nur Stationen in Frankreich clustern wollen.</li>
<li>Klicken Sie danach auf <b>Add</b> um eine weitere Bedingung hinzuzufügen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/6.png"/></a>
<h5>7</h5>
<ul>
<li>Für die neue Bedingung wählen Sie "type of business" als <b>Property</b> und "Primary Producer" als <b>Value</b>, denn wir wollen ja nur Primärproduzenten clustern.</li>
<li>Nun klicken Sie auf <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/7.png"/></a>
<h5>8</h5>
<ul>
<li>Alle französischen Primärproduzenten sind jetzt selektiert (blau markiert).</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/8.png"/></a>
<h5>9</h5>
<ul>
<li>Machen Sie einen Rechtsklick in den Graphen und wählen Sie <b>Collapse by Property</b> um die selektierten Stationen zu clustern.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/9.png"/></a>
<h5>10</h5>
<ul>
<li>Wählen Sie <b>Yes</b> um nur die selektierten Stationen fürs Clustern zu nutzen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/10.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/10.png"/></a>
<h5>11</h5>
<ul>
<li>Da wir auf Basis des Attributs "City" clustern wollen, wählen Sie dieses und klicken Sie <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/11.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/11.png"/></a>
<h5>12</h5>
<ul>
<li>Klicken Sie einfach nur <b>OK</b>, da wir keine Städte ausschließen wollen.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/12.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/12.png"/></a>
<h5>13</h5>
<ul>
<li>Alle französischen Station sind nun nach "City" geclustert.</li>
<li>Jede selektierte Meta-Station (blau) ist eine französische Stadt.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/13.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/13.png"/></a>
<h5>14</h5>
<ul>
<li>Wählen Sie "Picking" als <b>Editing Mode</b> and klicken Sie an eine leere Stelle des Graphen um alle Station zu deselektieren.</li>
<li>Nun können Sie sehen, dass eine der Meta-Station gelb ist. Das bedeutet, dass diese französische Stadt eine Verbindung zu allen Ausbruchs-Stationen hat.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/14.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/14.png"/></a>
<h5>15</h5>
<ul>
<li>Da der Graph jetzt recht unübersichtlich aussieht, sollten einen Layout-Algorithmus anwenden.</li>
<li>Machen Sie einen Rechtsklick in den Graphen und wählen Sie <b>Apply Layout > Fruchterman-Reingold</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/15.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/15.png"/></a>
<h5>16</h5>
<ul>
<li>Der Graph sollte jetzt übersichtlicher angeordnet sein.</li>
<li>Der Algorithmus ist nicht deterministisch. Deshalb wird ihr Graph anders aussehen als der Screenshot hier.</li>
<li>Um zu schauen welche französische Stadt eine Verbindung zu allen Ausbruchsorten hat, machen Sie einen Doppelklick auf die gelbe Station.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/16.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/16.png"/></a>
<h5>17</h5>
<ul>
<li>Wie im Dialog zu sehen, handelt es sich um die Stadt "Perpignan".</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/17.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_cluster/17.png"/></a>