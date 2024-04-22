# Network Visualisations
A repo containing python and Alteryx-python scripts that prepare data for network visualisations in Tableau.
These scripts use the "networkx" package, documentation is available [here](https://networkx.org/documentation/stable/index.html).

![Network Screenshot - Filtered](images/Network%20Screenshot%20-%20Filtered.JPG)

### Instructions
An instructional video on how to build a network visualisation in Tableau is available [here](https://youtu.be/N7JVM84b8aM?si=vRTDXvsn_vs5wAgz).
To create the Network, a certain data structure is required for Tableau. The first step is to create an input dataset that matches the following criteria:
  1. It must contain a column called "Target ID" which identifies the target node, and a column called "Source ID" which identifies the source node.
  2. It must contain a column called "Name" which links each edge with both the source node and the target node.

![Example Data Structure](images/Example%20Data%20Structure.JPG)

*For example, in a network representing knowledge flows among team members, if Sophie asks Andrew for advice on Database Management, the data needs to represent that link as above, with values otherwise repeated across the rows.*

With this input dataset configured, you can use the python scripts shared in this repository to create the coordinates needed to plot a network chart in Tableau. The script is available both as a Jupyter notebook and as a txt to be copied into Alteryx, to accommodate your data preparation preferences.

To interact with the "final product", view an example Tableau Network Chart [here](https://public.tableau.com/app/profile/sophie.hiscock/viz/NetworkCharts1/NetworkVisualisation).

