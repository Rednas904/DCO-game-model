# DCO game model
An Python implementation of a risk assessment and advisory model for Defensive Cyber Operations. This model is designed to be less reliant on Subject Matter Expert estimations and to offer more concrete and less ambigious options when compared to traditional models such as risk matrix based ones. The model is a multi-layered network graph representation combined with game and graph-based analysis techniques implemented as a constraint program.

The model is made for my master thesis research project. For verification and validation of the mathematical model, the resulting MINLP is implemented in Jupyter Notebook with a Python kernel, Pyomo as modelling language and SCIP AMPL as solver.

## Dependencies
A Python 3.7.11 kernel is used. There are several dependencies that need to be installed for core functionality. These packages are:
- pyomo (works with version 6.2)
- collections
- math
- functools
- operator
- itertools

Besides these packages a solver is needed. The solver used in this implementation is the AMPL version of SCIP, which can be downloaded from the SCIP website (works with version 7.0.0) : https://www.scipopt.org/download.php?fname=scipampl-7.0.0.win.x86_64.intel.opt.spx2.exe.zip. Just put it somewhere and make a reference to the executable when calling the solver. In the notebook this is marked with \[DRIVE AND PATH TO EXECUTABLE].

There are also several optional packages. These are needed for visualisation (recommended):
- matplotlib
- networkx
- grandalf. This package is used for the graph layout, but it is not working perfectly for this implementation. So there is still some code for manual placement of nodes.

Finally, a package is used to suppress annoying log warnings. Off course, this is also optional:
- logging
