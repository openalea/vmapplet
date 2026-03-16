# VMAppleT

A refactored and enhanced implementation of MAppleT/StocaTree. Original sources copied and modified from [openalea/incubator](https://github.com/openalea-incubator/MAppleT).



[![Docs](https://readthedocs.org/projects/vmapplet/badge/?version=latest)](https://vmapplet.readthedocs.io/en/latest/?badge=latest)
[![Build Status](https://github.com/openalea/vmapplet/actions/workflows/openalea_ci.yml/badge.svg)](https://github.com/openalea/vmapplet/actions/workflows/openalea_ci.yml)
[![Python Version](https://img.shields.io/badge/3.10%20%7C%203.11%20%7C%203.12%20%7C%203.13-blue)](https://www.python.org/downloads/)
[![Anaconda-Server Badge](https://anaconda.org/openalea3/openalea.vmapplet/badges/version.svg)](https://anaconda.org/openalea3/openalea.vmapplet)
[![License](https://img.shields.io/badge/License--CeCILL-C-blue)](https://www.cecill.info/licences/Licence_CeCILL-C_V1-en.html)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jvail/vmapplet/master?urlpath=lab/tree/notebooks/simple_simulation.ipynb)

## Major changes compared to MAppleT/StocaTree

* Build system and dependencies: All outdated and unmaintained dependencies have been removed or replaced
* Modularization: The L-Py file has been splitted up into several smaller modules
* Markov: A Python implementation of the semi-hidden Markov chain
* Configuration: An extended simulation and a Markov model configuration file in toml format
* Jupyter integration: Run and visualize simulations in Jupyter lab notebooks

### Authors

> - Thomas Cokelaer
> - Colin Smith
> - Jan Vaillant
> - Frederic Boudon

### Institutes

CIRAD / inria / INRAE

### Status

Python package

### License

CecILL-C

## Install

A local conda/miniconda installation is required.
First clone/download the repository. The `mamba` install is optional but recommended.

### Installation

#### for user
Creating a new conda environment with vmapplet and its dependencies installed
```bash
mamba create -n vmapplet -c openalea3 -c conda-forge openalea.vmapplet
```
In an existing conda environment:
```bash
mamba install -c openalea3 -c conda-forge openalea.vmapplet
```

#### for developer
```bash
mamba env create -f ./conda/environment.yml
```

## Jupyter

```sh
conda activate vmapplet
jupyter-lab --notebook-dir=notebooks
```

[//]: # (## Script)

[//]: # ()
[//]: # (```sh)

[//]: # (activate vmapplet)

[//]: # (python -m vmapplet vmapplet/data/simulation.toml out_folder)

[//]: # (```)
