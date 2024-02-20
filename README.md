# YLESimulator
___
This repository contains jupyter notebooks associated with the manuscript "A Y chromosome-linked genome editor for efficient population suppression in the malaria vector Anopheles gambiae" currently under review.

Ignacio Tolosana1, Katie Willis1, Austin Burt1, Matthew Gribble1, Tony Nolan2*, Andrea Crisanti1 & Federica Bernardini1

1 Department of Life Sciences, Imperial College London, London, UK.

2 Department of Vector Biology, Liverpool School of Tropical Medicine, Liverpool, UK.


For correspondence regarding the code: katie.willis@imperial.ac.uk

___
## Requirements

* Jupyter notebook
* Julia 1.9 or above
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

___
## User notes

- The YLEScript.ipynb is a jupyter notebook which contains the code used to generate the figures and values associated with the modelling element of the project.
- The YLEScript.ipynb script calls functions which define the model contained within the YLEModel.ipynb file.
- Within the YLE and YLEXS files are tables containing information on inheritance rules and fitness costs associated with each genotype which are used alongside the functions within YLEModel.ipynb to define the model.


