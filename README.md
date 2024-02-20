# YLESimulator
___
This repository contains jupyter notebooks associated with the publication "A Y chromosome-linked genome editor for efficient population suppression in the malaria vector Anopheles gambiae" available at TBC.

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
