# Hetero-Functional Graph Theory Toolbox
The Hetero-Functional Graph Theory (HFGT) is a rigorous modeling platform that can model the structure and function of highly interconnected
and heterogeneous engineering systems seen in systems-of-systems. A detailed explaination of the theory and the underlying mathematics can be found in the book [A Hetero-functional Graph Theory for Modeling Interdependent Smart City Infrastructure](https://www.springer.com/gp/book/9783319993003). This toolbox facilitates the instantiation of the seven mathematical models of the HFGT from a single XML input file.

A paper that serves as a user guide on how to use this toolbox has currently been submitted to Scientific Reports and is currently under review. If and when accepted, it shall be uploaded to this repository for further clarity. 

The toolbox contains two principal modules: XML2LFES() and raw2FullLFES() that are executed in sequence. In brief, the XML2LFES() module serves to import the input XML file and create the myLFES data structure in a “raw"
structure. Then, the raw2Full() module makes the HFGT calculations necessary to convert the myLFES data structure to the “full" state.  The module raw2Full() is utilizes sparse tensors in its calculations and thus is dependent on the Tensor Toolbox for Matlab which is found and can be install here: www.tensortoolbox.org

<img src="Images/HFGTToolbox_overview.png">

The input XML file - "Example_Network.xml" provided in this repository depicts a simplistic 4-Node Smart City Network. The topology of this example network and some of the associated graphs of the HFGT mathematical models are presented below. An input XML file for any engineering system can be generated along the same lines and the engineering system's HFGT models can be computed using this toolbox.

<img src="Images/Example_Network_Graphs.png">

The HFGT toolbox modules XML2LFES() and raw2FullLFES() are used in the Petri net Graphical User Interface (GUI) with an updated XML input file -"Example_Network_PN.xml" and scheduled event list CSV input file - "exampleEventList.csv".   The GUI visualizes the flow of operands through the Hetero-functional graph system as degrees of freedom are fired.

<img src="Images/Example_Network_GUI.png">