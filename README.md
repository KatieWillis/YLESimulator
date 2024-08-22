# YLESimulator
___
This repository contains jupyter notebooks associated with the manuscript "A Y chromosome-linked genome editor for efficient population suppression in the malaria vector Anopheles gambiae" currently under review.

Ignacio Tolosana1, Katie Willis1, Austin Burt1, Matthew Gribble1, Tony Nolan2*, Andrea Crisanti1 & Federica Bernardini1

1 Department of Life Sciences, Imperial College London, London, UK.

2 Department of Vector Biology, Liverpool School of Tropical Medicine, Liverpool, UK.


For correspondence regarding the code: katie.willis@imperial.ac.uk

___
## Requirements

* Julia 1.9 or above
* Jupyter notebook
* This analysis was performed on macOS Sonoma 14.3, however any system which can run Julia 1.9 should be suitable.  
* All dependencies can be installed by running the following code in julia from the location of the downloaded files to initiate the environment (This only needs to be done once)
```
using Pkg
Pkg.activate("./Environment/")
Pkg.instantiate()
```

The environment can loaded at the beginning of each jupyter session by running:
```
] activate "./Environment/"
```

And the required packages can be loaded by running:
```
using NBInclude
@nbinclude("./Environment/Setup.ipynb");
```

Alternatively the packages can be installed manually:
```
CSV v0.10.12
DataFrames v1.6.1
DelimitedFiles v1.9.1
JLD2 v0.4.45
NBInclude v2.3.0
Plots v1.39.0
PyPlot v2.11.2
SymPy v2.0.1
Distributed
LinearAlgebra
```

Installation is not expected to take more than 30 minutes
___
## User notes

- The YLEScript.ipynb is a jupyter notebook which contains the code used to generate the figures and values associated with the deterministic modelling element of the project.
- The YLECageSimulator.ipynb is a jupyter notebook which contains the code used to simulate the cage trial and infer an unknown parameter.
- The YLEScript.ipynb script calls functions which define the model contained within the YLEModel.ipynb file.
- The YLE and YLEXS folders contain human readable .csv files with inheritance probabilities and fitness costs associated with each genotype (or pair of genotypes) which are used alongside the functions within YLEModel.ipynb and to define the model.
___

## Timing:

Results requiring only a few time series simulations take only a few seconds. Results requiring more simulations, such as parameter sweeps or calucating release rate requirements, can take several minutes. 
___

