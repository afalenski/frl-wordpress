---
ID: 947
post_title: PMM-Lab FAQ
author: FRL_Admin
post_date: 2015-03-30 15:56:10
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/pmm-lab-faq-de/
published: true
---
Q: <i>I am working behind a proxy server. How can I set up KNIME to use my personal proxy settings?</i>

A: Should you be working behind a proxy server, it is necessary to configure KNIME correctly in order to be able to update and install software. You need to know the IP-address or the hostname of your proxy server as well as the TCP port that is routing outside. Follow the steps below to configure your Eclipse instance’s proxy settings:

From the main menu, please choose
‘Window’
‘Preferences’ the window ‘Preferences’ opens.
From the displayed category tree, please chose
+‘General’
+‘Network Connections’

Q: <i>After installing PMM-Lab, some nodes are missing. Especially nodes responsible for database IO seem not have been installed.</i>

A: Your installation may have had problems. Please close KNIME and try to start KNIME with the -clean parameter. In windows this would be

knime.exe -clean