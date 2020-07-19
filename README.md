# torque-ripple
Permanent magnet motors incorporate inherent torque ripple, which should be minimized, as it degrades performance of the machine. Software based torque ripple reduction was studied with good success. This repository contains material related to torque ripple research.

## Installation
It is recommended to use virtual environment:  
`python -m venv env`

The project has been split into several repositories. 
In order to obtain everything project related, run:  
`git submodule --recursive --init`

# Project structure
This repository consists of several submodules:
```
torque-ripple
│─ compensation
│─ data-analysis
│─ latex
|─ reinforcement-learning
└─ ...
```
## Compensation
Contains compensation related C/C++ code. Includes ILC and Q-learning based compensator implementations and pulsation model that can be used to generate torque pulsations in simulator.

## Data analysis
Contains simulation and measurements data. In addition, contains scripts that were used for plotting and visualizing the data.

## Latex
This repository contains the TEX files and images that were used for generating the PDF file.

## Reinforcement learning
Includes python code implementation of the q-learning based compensator. Python version allows faster prototyping, but it can be run only in a simulator. The simulator is not provided, therefore this repository may be uninteresting. Moreover, this version
