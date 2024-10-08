# SLACPAS 2024 Class
Repository for the lab portion of SLACPAS course (August 2024). Some exercises and instructions are borrowed or expanded from the USPAS FEL class held in 2021 & 2024. Exercises from the USPAS classes can be found here [2024](https://github.com/uspas/fel2024/tree/main) and here [2021](https://github.com/uspas/FEL2021).


# Installation 

The software for the class can run natively on Linux and macOS. Windows users will need to install a Linux distribution (e.g. Ubuntu) using WSL2.
Or alternatively, you can request a Jupyter Lab account at [Sirepo.com](https://www.sirepo.com/en/). You will need to use your Stanford email and allow 1-2 days for approval.
Then you will be able to install and run the software in a browser. 


## Install Miniforge
***Note***, if you already have anaconda or miniconda on your laptop, you can skip this section!

Download and install Minforge using the instructions at: https://github.com/conda-forge/miniforge?tab=readme-ov-file#download. Note that:
- If you have a Mac with an M1, M2, or M3 processor, use the "Apple Silicon" link. For older MacBooks, use the x86-64 version. If unsure, click the Apple at the top left of your screen, "About this Mac" and look at the "Chip" line.
- For Windows on WSL2, choose the Linux x86-64 version (**not** the Windows build!).

Once installed, initialize conda on the command line with:
```bash
conda init
```
and restart the terminal.


## Clone this repository
All labs are uploaded to this repository. Please clone this repository using [GitHub Desktop](https://github.com/apps/desktop) or using `git` on the command line. 
To clone the repository on the command line use the following command in a terminal:
```
git clone https://github.com/slaclab/slacpas.git
```
The repository (folder) will then be in the location where you executed the ```git clone``` command. 


## Create the `slacpas24` software environment
In the same terminal, change directories to the slacpas repo you cloned:
```bash
cd slacpas
```

This repository contains a file `environment.yml`. 
This file will help you install all the software you need in a conda enviornment.
On the command line, execute the following command:
```bash
conda env create -f environment.yml
```

Now activate the `slacpas24` environment:
```bash
conda activate slacpas24
```
and test that Jupyter lab works:
```
jupyter lab
```

## Download Genesis4 examples 
Additional LUME-Genesis' (Genesis4) examples can be downloaded from  here: [lume_genesis_genesis4_examples](https://github.com/slaclab/lume-genesis/releases/download/v1.1.0/lume_genesis_genesis4_examples.zip).

Try these using Jupyter lab in the `slacpas24` environment.

The Genesis4 manual can also be found at the following repo: [https://github.com/svenreiche/Genesis-1.3-Version4](https://github.com/svenreiche/Genesis-1.3-Version4)

