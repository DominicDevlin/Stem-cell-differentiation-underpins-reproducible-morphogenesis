Code and Data for "Stem-cell differentiation underpins reproducible morphogenesis"

https://doi.org/10.5061/dryad.pk0p2ngxx

This repository contains the data and source code associated with the manuscript "Stem-cell differentiation underpins reproducible morphogenesis".

source-code/: This directory includes all core files required for running evolutionary simulations. The code base is built with the Qt framework, so ensure that the necessary Qt libraries are installed.

visualisation-code/: This directory provides scripts for generating visualisations, including cell state spaces and UMAP visualizations of cell states.

data.ods: Contains genomes of all evolved organisms across all selection criteria. Key data points include:

Reproducibility Scores

Average Morphological Complexity

Presence/absence of stem-cell system

Compilation and Execution

Navigate to the source-code/ directory and choose a target file in CellularPotts2.pro to specify the simulation to run. Available target files include:

sorting.cpp: Simulates a Cellular Potts model that develops one organism. The associated gene regulatory network (GRN) can either be randomised or set manually in parameter.cpp.

evolution.cpp: Runs a multithreaded evolutionary simulation of morphogenesis.

Additional targets include multisort.cpp, transition.cpp, and potency.cpp.

To run an executable, use the following commands:
qmake

make

./"executable name here"
