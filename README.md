# Soapy-Updates
This project was supervised by Benjamin Monreal at Case Western Reserve University.

This repository hosts an update to the Adaptive Optics Simulation program Soapy, the documentation for which can be found at https://soapy.readthedocs.io/en/latest/index.html

I implemented architecture for the simulation of rectangular apertures  in Soapy, which previously only supported circular lenses.
The GUI can be run by executing
soapy -g <configFilename>
in your Python terminal. This reads in .yaml files into the confParse that I have updated to read new parameters to set rectangular dimensions, check my rect yaml conf file for reference.
The confParse file also has documentation for each of the parameters that should be gone over before creating your own configs.

The lens file has new functionality that draws a rectangle based off of the dimensions supplied in the square array of 0s and 1s that is used to map the lens against the atmosphere and in calculations for other components of the apparatus. 
