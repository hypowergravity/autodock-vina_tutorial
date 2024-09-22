# AutoDock Tutorial: Docking Beta-Lactamase with Purpurogalin

This repository contains a tutorial for using AutoDock Vina to dock [Purpurogalline](https://pubchem.ncbi.nlm.nih.gov/compound/5281571) to a zinc-dependent beta-lactamase, along with a reference compound. The tutorial guides users through installation, setup, and running the docking simulations.

Details of the docking can be found on the following [**website**]().


## Table of Contents
- [Installation](#installation)
- [Objective](#objective)
- [Setup](#setup)
- [Running the Docking](#running-the-docking)
- [Results](#results)
- [References](#references)

## Installation

AutoDock Vina can be installed by following the instructions on the [official documentation](https://autodock-vina.readthedocs.io/en/latest/installation.html). 

### Conda Environment (Recommended)

It is recommended to use a Conda environment for managing dependencies. To create and activate a new Conda environment for AutoDock Vina, follow these steps:

~~~bash
conda create -n autodock vina
conda activate autodock
~~~
After activating the environment, follow the installation guide linked above.
## Objective

The objective of this tutorial is to dock the compound Purpurogalline to a zinc-dependent beta-lactamase, using a reference compound for comparison.
## Setup

  Prepare the protein and ligand structures.
      Download the protein structure for zinc-dependent beta-lactamase.
      Retrieve the Purpurogalline ligand structure from PubChem.

  Prepare the protein and ligand files by converting them to the appropriate format for docking with AutoDock Vina.

  Set up the configuration file for the docking simulation, specifying the search space and grid box parameters.

## Running the Docking

To run the docking process, use the following command after preparing the necessary input files:
~~~bash
vina --config config.txt --log docking_log.txt
~~~
he configuration file should specify the receptor, ligand, and grid box parameters. The vina command will run the docking simulation, outputting a log file and the docking poses.
## Results

Once the docking process is complete, analyze the output files to identify the best docking pose and binding affinity for Purpurogalline and the reference compound.
## References

* AutoDock Vina [Official Documentation](https://autodock-vina.readthedocs.io/en/latest/installation.html).
* Purpurogalline on [PubChem](https://pubchem.ncbi.nlm.nih.gov/compound/5281571).
