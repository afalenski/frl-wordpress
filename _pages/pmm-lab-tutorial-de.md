---
ID: 960
post_title: PMM-Lab Tutorial
author: FRL_Admin
post_date: 2015-03-31 09:06:38
post_excerpt: ""
layout: page
permalink: >
  https://foodrisklabs.bfr.bund.de/index.php/pmm-lab-tutorial-de/
published: true
---
PMM-Lab is an extension of the Konstanz Information Miner (KNIME). For getting started, you may want to make yourself familiar with this software product. Documentation can be obtained from <a href="http://tech.knime.org/documentation" rel="nofollow">http://tech.knime.org/documentation</a>.

Nevertheless for this introduction no prior knowledge on KNIME is required. In this section we will give you a short introduction to the Scientific Workflow concept and KNIME. Furthermore, we will give an introducing example for the application of PMM-Lab to predictive microbiology.
<h4 id="the-concept-of-scientific-workflows">The concept of Scientific Workflows</h4>
KNIME is a Scientific Workflow Management system. A Scientific Workflow consists of interconnected task nodes. Each task node is responsible for a specific data processing step. The connections between task nodes describe the data dependencies between the tasks. Such tasks may be the data loading, storing or manipulation. After describing all necessary data processing task in a so called workflow, this workflow can be executed and the calculations will be performed in a transparent and repeatable fassion. The same concept is applied in PMM-Lab where workflows serve as an easy to understand user interface to the dataprocessing steps which can easily adapted by the user to its specific needs. The graphical description of data processing steps is usually considered as an intuitive way to increase transparency within data analysis and modeling tasks.
<h4 id="organization-of-the-knime-user-interface">Organization of the KNIME user interface</h4>
The KNIME graphical user interface divides the screen into a set of different compartments (views). For us, the most important views are:
1. Workspace (KNIME_project)
2. Node Repository
3. Console
4. Node Description
5. Workflow Projects
When starting up KNIME, an empty workspace is shown. In the workspace we can assemble a workflow out of nodes and connecting arrows that represents the data flow and, hence, the Scientific Workflow. In the node repository view, all task nodes are listed that can be utilized in a workflow. KNIME comes with a set of standard nodes libraries. PMM-Lab is essentially a new extension to this node repository. After installing the PMM-Lab plugin, a new node library folder called ‘PMM-lab’ can be found in the node repository. The Console view prints out messages, warnings and errors that are produced by configuring or executing the workflow. Eventually, in the Node Description view gives information on the functionality and configuration options of each node. The Workflow Projects view shows all workflows in the current workspace. It is possible to organize workflows in folders and to rename, copy or move them.
<h4 id="setting-up-an-example-workflow">Setting up an example Workflow</h4>
We will now set up a simple workflow for the purpose of introducing the basic operations that can be performed with PMM-Lab. We will go through the assembly of the Workflow step by step and explain the way each node works and how these are interconnected in a meaningful way. If you want an overview about the functionality that PMM-Lab provides, please refer to the feature description section. If you want to explore the available KNIME nodes and what they can do, please go to the node description section. The first thing we will have to accomplish is to create a new KNIME workflow.
<ol>
	<li>‘File’</li>
	<li>‘New…’ the ‘Select a wizard’ window opens.</li>
	<li>Select ‘New KNIME Workflow’ from the ‘Wizards:’ list.</li>
	<li>Click the button ‘Next &gt;’</li>
	<li>You may enter a custom workflow name in the text field ‘Name of the workflow to create:’</li>
	<li>Click the button ‘Finish’</li>
</ol>
An empty KNIME workflow tab will open. Note that the new workflow appears in the ‘Workflow Projects’ window where you can organize all workflows you created. In our example workflow we will create primary growth models from data sets. After the creation of the model we will visualize the result and save the models to the PMM-Lab database.

<img src="https://sourceforge.net/p/pmmlab/wiki/Tutorial/attachment/PMM-Lab%20-%20Primary%20Model%20Generation%20Workflow.png" alt="PMM-Lab - Primary Model Generation Workflow" />

This workflow demonstrates how to fit primary models to experimental microbial data.

Step 1a: Read in microbial data to work with (e.g. with ComBase Reader, Data Reader etc.). If necessary you can visualize and select data by applying the Data Selection node - in this case we select all DMFit test data.

Step 1b: Select the model formulas which should be fitted to the data by configuring the Formula Reader node. In the example below the full Baranyi growth model (iPMP model eq. 6), the Huang model (iPMP model eq.5) and the three-phase linear model (iPMP model eq. 8) are selected. Equally well a formula would work that a user enters in the Formula Creator node or in the Model Creator node. Attention: the Creator nodes give you also the opportunity to assign units to the variables!

Step 2: Connect the Formula Reader and Data Selection node out-ports with the in-ports of the PMM Joiner node and then configure the PMM Joiner node. To do the latter either double-click the node, right-click and choose 'Configure...' or press F6 on the keyboard. In the configuration menu you need to assign the correct columns from the data table to the independent / dependent variables of the formula(s). Then the PMM Joiner node can be executed. Attention: based on the unit of the dependent variable the experimental data will be transformed by this node, e.g. if the formula expects ln()-scaled values the log10()-scaled measured data will be transformed automatically. If you do not want that you have to provide a formula with a log10()-scaled dependent variable.

Step 3: Execute the Model Fitting node. In case the standard setting does not provide a sufficiently good fitting result, tick 'Expert settings' and providing starting values for any of the model parameters. Fitting itself may take a while, depending on the number of models and data sets to be fitted.

Step 4: Look at the model fitting results by application of the Primary Model Selection node. This node allows the manual selection / deselection of models according to your personal criteria (e.g. RMS, RSquare, model type etc.). In the node GUI you can also configure which columns in the tabular listing of fitted models should be on display. Attention: SSE, RMSE, MSE are scaled to the log-transformation defined by the selected formula. Only RSquared can be used to compare models with different log-transformation directly. This node also provides the opportunity to select models for further processing - in the example below all models fitted to the three-phase linear formular (iPMP eq. 8) are selected. After execution, the green outport of the Primary Model Selection node contains the graph as PNG image.

Step 5: Depending on the individual preference you can save the selected models to the PMM-Lab database or write them to a KNIME data table (Table Writer). In case of the first option you could verify that the models have been written correctly with all relevant parameters into the DB table "Estimated models" via the Menu item "PMM-Lab -&gt; Open DB GUI ..." . The Model Reader node enables the user to retrieve the models back from the PMM-DB.