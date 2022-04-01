# DCO game model
An Python implementation of a risk assessment and advisory model for Defensive Cyber Operations. This model is designed to be less reliant on Subject Matter Expert estimations and to offer more concrete and less ambigious options when compared to traditional models such as risk matrix based ones. The model is a multi-layered network graph representation combined with game and graph-based analysis techniques implemented as a constraint program.

The model is made for my master thesis research project. For verification and validation of the mathematical model, the resulting MINLP is implemented in Python Notebook with a Python 3.7.11 kernel, Pyomo 6.2 as modelling language and SCIP AMPL 7.0.0 as solver.

## Dependencies
The solver is the AMPL version of SCIP, which can be downloaded from the SCIP website: https://www.scipopt.org/download.php?fname=scipampl-7.0.0.win.x86_64.intel.opt.spx2.exe.zip. Just put it somewhere and make a reference to the executable when calling the solver. In the notebook this is marked with \[DRIVE AND PATH TO EXECUTABLE]
