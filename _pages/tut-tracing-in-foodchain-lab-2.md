---
ID: 784
post_title: Tracing in FoodChain-Lab
author: FRL_Admin
post_date: 2015-03-18 10:40:05
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/tut-tracing-in-foodchain-lab-2/
published: true
---
<h4>Aufgaben</h4>
<ul>
 	<li>Nutzen Sie den Beispiel Workflow von <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank" rel="noopener noreferrer">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
 	<li>Lassen Sie sich im <b>Tracing View</b> den Forward- und Backward-Trace von einer Station zeigen.</li>
 	<li>Dann deaktivieren Sie in der schwarzen Station die Kreuzkontamination und schauen Sie, wie sich der Forward Trace daraufhin ändert.</li>
</ul>
<h5>1</h5>
<ul>
 	<li>Importieren Sie den Example Workflow von <a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/workflows/FCL_Example.zip" target="_blank" rel="noopener noreferrer">https://github.com/SiLeBAT/BfROpenLab...</a>.</li>
 	<li>Öffnen Sie den <b>Tracing View</b> per Doppelklick.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/1.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/1.png" /></a>
<h5>2</h5>
<ul>
 	<li>Im Graphen sehen Sie 9 Ausbruchs-Stationen (rot) and eine Station, an den Kreuzkontamination angenommen wird (schwarz).</li>
 	<li>Die Größe jeder Station basiert auf ihrem "Score", welcher davon abhängt welche Ausbruchs-Stationen erreicht werden können.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/2.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/2.png" /></a>
<h5>3</h5>
<ul>
 	<li>Wir werden uns nun den Trace einer einzelnen Station im Detail anschauen.</li>
 	<li>Wählen Sie "Picking" als <b>Editing Mode</b> und machen Sie einen Doppelklick auf die Station im roten Kreis.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/3.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/3.png" /></a>
<h5>4</h5>
<ul>
 	<li>Ein Dialog mit allen Attributen der ausgewählten Station erscheint.</li>
 	<li>Im oberen Bereich können Sie die Werte der Attribute "Weight", "CrossContamination", "Kill Contamination" und "Observed" verändern.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/4.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/4.png" /></a>
<h5>5</h5>
<ul>
 	<li>Aktivieren Sie <b>Observed</b> und drücken Sie <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/5.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/5.png" /></a>
<h5>6</h5>
<ul>
 	<li>Alle Stationen/Lieferungen vom Forward-Trace sind orange gefärbt and diejenigen vom Backward-Trace sind magenta.</li>
 	<li>Drei Ausbruchs-Stationen haben nun orange Streifen. Das bedeutet, dass Sie auch auf dem Forward-Trace sind.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/6.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/6.png" /></a>
<h5>7</h5>
<ul>
 	<li>Nun schauen wir was sich verändert, wenn wir die Kreuzkontamination der Station im roten Kreis deaktivieren.</li>
 	<li>Machen Sie einen Doppelklick auf die Station.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/7.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/7.png" /></a>
<h5>8</h5>
<ul>
 	<li>Deaktivieren Sie <b>CrossContamination</b> und drücken Sie <b>OK</b>.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/8.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/8.png" /></a>
<h5>9</h5>
<ul>
 	<li>Das Deaktivieren der Kreuzkontamination hat den Forward-Trace der beobachteten Station ("Observed") verändert.</li>
 	<li>Nun können zwei Ausbruchs-Stations, die zuvor noch gestreift waren, nicht mehr erreicht werden.</li>
</ul>
<a href="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/9.png"><img class="aligncenter size-full" src="https://github.com/SiLeBAT/BfROpenLabResources/raw/master/GitHubPages/documents/foodchainlab_tracing/9.png" /></a>