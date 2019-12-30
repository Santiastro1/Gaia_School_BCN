# Gaia_School_BCN

[COST WG1 Milky Way Gaia School '20](https://indico.icc.ub.edu/event/52/)

This repository is meant to help COST-WG1 MWG School 2020 (MWG_BCN20) participants to set up a work environment for the hands-on sessions of the workshop, as well as donwload some example datasets to be used during these sessions. 

It is assumed that there exists a **working [anaconda3](https://www.anaconda.com/distribution/) installation** on the target machine. 

## Installation

Clone the repository:

```console
$ git clone https://github.com/Santiastro1/Gaia_School_BCN.git

Change directory into the cloned repository:

```console
$ cd Gaia_School_BCN
```
Create a new environment:

```console
$ conda env create -f Gaia_School_BCN_env.yml
```
Activate the new environment:

```console
$ conda activate MWG_BCN20
```
Verify that the new environment was correctly installed:

```console
$ conda env list
```
The name of the new environment, ```MWG_BCN20```, should show up in the list. 

## Updating installation

Should you need to update an already existing ```MWG_BCN20``` environment with a newer ```Gaia_School_BCN_env.yml``` version:

```console
$ conda env update --name MWG_BCN20 -f Gaia_School_BCN_env.yml --prune
```

## Contact

In case of trouble with the installation please contact Santi Roca-Fàbrega (sroca01 at ucm dot es) or open an issue [here](https://github.com/Santiastro1/Gaia_School_BCN/issues).
