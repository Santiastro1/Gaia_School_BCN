# Gaia_School_BCN

[COST WG1 Milky Way Gaia School '20](https://indico.icc.ub.edu/event/52/)

This repository is meant to help COST-WG1 MWG School 2020 (MWG_BCN20) participants to set up a work environment for the hands-on sessions of the workshop, as well as donwload some example datasets to be used during these sessions. 

It is assumed that there exists a **working [anaconda3](https://www.anaconda.com/distribution/) installation** on the target machine. 

## Installation

Clone the repository:

```console
$ git clone https://github.com/Santiastro1/Gaia_School_BCN.git
```

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

## Testing the conda environment

Before starting with the ```MWG_BCN20``` we highly recommend you to test the conda environment you have just created. 
First, try to open a ```jupyter notebook``` in your brownser.

```console
$ jupyter notebook
```

Now, in order to test some of the python libraries, you will need to download extra files:

### 1- Used by ```yt```: Data files from N-body simulations obtained using a large variety of numerical codes: https://yt-project.org/data/.

Here we will usedata from ART and RAMSES numerical codes so we recommend you to download the following files and move them to the ```Gaia_SChool_BCN``` folder:

http://yt-project.org/data/sizmbhloz-clref04SNth-rs9_a0.9011.tar.gz

```console
$ mv ~/Downloads/sizmbhloz-clref04SNth-rs9_a0.9011.tar.gz ~/Gaia_School_BCN/
```

```console
$ cd ~/Gaia_School_BCN/
```

```console
$ tar -zxvf sizmbhloz-clref04SNth-rs9_a0.9011.tar.gz
```

http://yt-project.org/data/output_00080.tar.gz

```console
$ mv ~/Downloads/output_00080.tar.gz ~/Gaia_School_BCN/
```

```console
$ cd ~/Gaia_School_BCN/
```

```console
$ tar -zxvf output_00080.tar.gz
```

### 2- Used by pynbody:

Download and extract the following files to your Gaia_School_BCN folder

http://star.ucl.ac.uk/~app/testdata.tar.gz

```console
$ mv ~/Downloads/testdata.tar.gz ~/Gaia_School_BCN/
```

```console
$ cd ~/Gaia_School_BCN/
```

```console
$ tar -zxvf testdata.tar.gz
```

Now open the ```MWG_BCN20_envtest.ipynb``` and run each one of the cells in order to test the yt, pynbody and ```Python3.7``` libraries installation.

If you succeed on running all cells in this notebook, you are now ready to work on the ```MWG_BCN20``` school hands-on sessions.

If you have had problems on running any of the cells, please get in contact with sroca01 at ucm dot es, in order to have this problems solved before the school starts.

## Updating installation

Should you need to update an already existing ```MWG_BCN20``` environment with a newer ```Gaia_School_BCN_env.yml``` version:

```console
$ conda env update --name MWG_BCN20 -f Gaia_School_BCN_env.yml --prune
```

## Contact

In case of trouble with the installation please contact Santi Roca-Fàbrega (sroca01 at ucm dot es) or open an issue [here](https://github.com/Santiastro1/Gaia_School_BCN/issues).
