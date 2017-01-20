---
ID: 17
post_title: PMM-Lab Installation
author: FRL_Admin
post_date: 2015-02-09 15:31:56
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/pmm-lab-installation/
published: true
---
In this Section we will go through the steps of installing PMM-Lab.

+ Visit <a href="http://www.knime.org/downloads/overview/" rel="nofollow">http://www.knime.org/downloads/overview/.</a>
+ Download the KNIME distribution that fits to your Operating System.
+ Locate the downloaded KNIME self-extracting archive file and execute it. You will be asked to specify a location where, on your hard disk, you wish to install KNIME.
+ Go to the specified KNIME directory and run the executable file called ‘knime.exe’ in the case of Windows users or plain ‘knime’ if you are a user of Linux or Mac OS X.
+ Note that KNIME doesn not include a JRE for the Mac. Therefore, Java needs to be installed on the machine. For PMM-Lab Java7 is needed!

<img src="https://sourceforge.net/p/pmmlab/wiki/Installation/attachment/step_install_new_software_small.jpg" alt="Install new software menu item" />

Then, the PMM-Lab plugin needs to be added to the KNIME instance. To achieve that please
<ul>
 	<li>Choose from the main menu
<ul>
 	<li>‘Help’</li>
 	<li>‘Install New Software...’ the ‘Available Software’ window opens.</li>
</ul>
</li>
 	<li>In the category ‘Work with’ please click the button ‘Add...’ the ‘Add Repository’ window opens.</li>
</ul>
<img src="https://sourceforge.net/p/pmmlab/wiki/Installation/attachment/step_add_local_small.jpg" alt="Add repository window" />
<ul>
 	<li>In the 'name:' field please enter a meaningful name like 'PMMlab install path' and in the text field ‘Location:’ please enter the following URL: https://dl.bintray.com/silebat/test/</li>
 	<li>Click Button ‘OK’.</li>
 	<li>Make sure all PMM-Lab items are selected in the table below the ‘Work with:’ section.</li>
</ul>
<img src="https://sourceforge.net/p/pmmlab/wiki/Installation/attachment/step_choose_package_small.jpg" alt="Available software window" />
<ul>
 	<li>Click the button ‘Next &gt;’ at the bottom of the window and wait while KNIME is ‘Calculating requirements and dependencies’. The ‘Install Details’ window opens.</li>
 	<li>Click the button ‘Next &gt;’.</li>
 	<li>Read the license agreement carefully, then activate the radio button ‘I accept the terms of the license agreement’</li>
 	<li>Click the button ‘Finish’. The ‘Installing Software’ window opens that lets you follow the installation progress.</li>
 	<li>KNIME lets you choose, whether to restart.</li>
</ul>
You accomplished installing an instance of KNIME and eventually adding the PMM-Lab plugin. You can now use the PMM-Lab nodes in the Node Repository to perform specific calculations in the field of predictive microbiology. Future versions of PMM-Lab can easily be installed via the Update functionality of KNIME. You will find it in the menu:
<ul>
 	<li>Choose from the main menu
<ul>
 	<li>‘Help’</li>
 	<li>’Check for Updates.’</li>
</ul>
</li>
</ul>
To make use of the HSQL database no further action is necessary. This database will be installed automatically inside the KNIME workspace directory when you start up KNIME for the first time.

&nbsp;
<div class="markdown_content">
<h4 id="disclaimer">Disclaimer</h4>
<ol>
 	<li>All reasonable efforts have been made to ensure that PMM-Lab is provided free of errors and up to date. Anyhow, no guarantee as to the accuracy and completeness of PMM-Lab or the work resulting from PMM-Lab application or the fitness of PMM-Lab for any purpose whatsoever is given.</li>
 	<li>PMM-Lab may change at any time without notice.</li>
 	<li>PMM-Lab is provided ‘as is’, without any conditions, warranties or other terms of any kind.</li>
 	<li>There is no liability for any loss or damage arising from any inability to use PMM-Lab.</li>
 	<li>The developers and the BfR exclude all liability and responsibility for any amount or kind of loss and damage that may result to you or a third party (including without limitation, any direct, indirect, punitive or consequential loss or damages), or loss of income, profits, goodwill, time, data, contracts, use of money, or loss or damages from or connected in any way to business interruption - including but not limited to loss or damage due to viruses that may infect your computer equipment, software, data or other property on account of your use of PMM-Lab or your downloading of any material from PMM-Lab or any web site linked to PMM-Lab.</li>
</ol>
</div>