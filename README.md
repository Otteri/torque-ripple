# torque-ripple
Permanent magnet motors incorporate inherent torque ripple, which should be minimized, as it degrades performance of the machine. Software based torque ripple reduction was studied with good success. This repository contains material related to the torque ripple research.

## Installation
It is recommended to use virtual environment:  
`python -m venv env`

The project has been split into several submodules. 
In order to obtain all project related files, run:  
`git submodule update --recursive --init`

## Project structure
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
Contains simulation and measurement data, and scripts that were used for visualizing the captured data.

## Latex
This repository contains the TEX files and images that were used for generating the PDF file (thesis).

## Reinforcement learning
Includes python code implementation of the q-learning based compensator. Python version allows faster prototyping, but it can be run only in a simulator. The simulator code is not distributed and therefore it is not possible to test the scripts in this repository. However, a few images that illustrate execution are provided.
