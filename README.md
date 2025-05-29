# Introduction to computing 
This is a collection of resources for the new members in the group to set up their computing environment, and gain basic knowledge of python programming, computational biology and AI/ML. 

## Command line interface
The workstations and HPC systems are accessible using command line interface. [A comprehensive introduction is available here](https://www.freecodecamp.org/news/command-line-for-beginners/). 

## Python
The group is using Python as the primary programming language, as its versatility in AI/ML and computational bio research. Certain level of proficiency is preferred working with all the projects. Following are various resource on Python. 

### Introduction and set up 
I have found the [data science course](https://datascience.quantecon.org/) from QuantEcon very useful. It contains software installation, Python fundamentals, scientific computing and some data science basics. It covers introduction to Python packages, such as matplotlib, numpy and pandas. The contents include the installation of the anaconda and setting up conda environment. 

>[!Notes]
>1. Personally I prefer [mamba](https://github.com/conda-forge/miniforge?tab=readme-ov-file#unix-like-platforms-macos-linux--wsl) over anaconda, as mamba is a lot more lightweight. 
>2. The Jupyter notebook can be replaced using [VS Code jupyter extension](https://code.visualstudio.com/docs/datascience/jupyter-notebooks). The Python interpolator still needs jupyter notebook installed. 
>3. Not all content from the course is useful for us, but overall good knowledge to have. 

### Conda/mamba
One of the most useful features of `conda` is setting up multiple python environments for different projects/test runs. [The instructions can be found here](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).The `mamba` is a faster version of `conda`. 

## Torch
Pytorch is the AI/ML framework, which enables the users to create and train their own AI models. It also hosts [PyTorch Hub](https://pytorch.org/hub/) for trained models. [The tutorial](https://docs.pytorch.org/tutorials/beginner/basics/intro.html) is a good place to start learning the basics of torch and neural network. 

## Molecular simulation
### OpenMM
[OpenMM](http://docs.openmm.org/latest/userguide/application/02_running_sims.html) is a molecular dynamics simulation engine that runs on GPUs and has a Python API. It can use topology files from Amber, Gromacs, and charmm. The topology file contains all the interactions in a system, including both bonded and unbonded forces. A typical simulation protocol is as follow: 
1. Find your target from PDB, experiments or folding programs, such as AlphaFold and ESMFold. The input file contains the position of each atoms. 
2. Build the topology base on the 3D coordinates file. 
3. Run your simulation, including equilibration and production runs. 
4. Analyze the results using MDAnalysis or other program. 

### Topology
The topology of the system can be built mainly using OpenMM modeller, Gromacs and Amber tleap. The OpenMM modeller is completely black box, but is suitable for simple system and fast testing. [The latter two are incorporated in a program here](https://github.com/hengma1001/md_setup/tree/master). 

### MDAnalysis
MDAnalysis is a package to analyze MD trajectory for various properties. [The tutorial is available here](https://www.mdanalysis.org/pages/getting_started/). 

### Biopython
[Biopython](https://biopython.org/) is primarily used when working with sequences. 


<!-- TO DO: add more details about me later -->
