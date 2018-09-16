# lightMM

In biochemistry, the Michaelis-Menten model is the one of the best-known and useful approaches to enzyme kinetics. The model provides extremely valuable knowledge for researchers in form of kinetic parameters that explain properties of a particular enzyme. To determine the kinetic parameters by the standard approach, at least couple (e.g., eight or more) different substrate concentration must be used in experiments. In order to speed up the process, various computer programs were provided, however, the experimental procedure remains almost the same.

Here, we report the discovery of a novel tool for calculating kinetic constants in the Michaelis-Menten equation from two substrate concentrations called lightMM. This extremely useful framework gives wider possibilities in determination of kinetic parameters by reducing cost and time, primarily by lowering amount of needed enzymes that are very often difficult (requiring) to isolate, store and use in experiments.

# Implementation

lightMM is a stand-alone program that is implemented in Python using NumPy. The program is supported on Linux and MS Windows.

# Usage

1. A user needs to prepare data in .csv file where the first row contains data at a larger level of the substrate concetration and the second row contains data at a lower level of the substate concentration.
2. A user needs to prepare a configuration file (.json) that contains all necessary information about the data and method (please see examples in examples folder).
3. Put your data and configuration file together with the program file(s) (Linux: lighmm.so and run.py, MS Windows: lightmm.exe) in the save directory.
4. Run the program:
- Linux: in terminal type python run.py
- MS Windows: in cmd type lightmm.exe
5. Provide name of your configuration file and wait for results. 

REMARK. If no result is provided, please check the following:
- the name of your data file;
- the name of your configuration file;
- lower and upper values of the kinetic constants (maybe higher or lower values are necessary);
- time step (in seconds) of the experiment and how long the experiment lasted (in minutes);
- initial values of the substrate and enzyme concentrations. 

# License

The program is distributed under CC BY-NC-ND 4.0 license.
