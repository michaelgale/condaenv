# Michael's Conda Environment Recipes

I use conda to manage several different python environments depending on what I'm working on.  This keeps development projects isolated from each other and allows for different python versions and package configurations.

## Installation

Get the miniconda installation script from [https://conda.io/miniconda.html](https://conda.io/miniconda.html)

Link to the official [Conda Sheet Sheet](https://conda.io/docs/_downloads/conda-cheatsheet.pdf).

## Updating conda

```
$ conda updata conda
```

## Creating a new environment

```
$ conda create --name mynewenv python=3.6
```

Create a new environment from an environment file:

```
$ conda env create -f newenv.yml
```

## Changing environments

List current environments:

```
$ conda env list
```

Change current active environment:

```
$ source activate mynewenv
```

## Conda packages

List all installed packages in the current active environment:

```
$ conda list
```

Install a new package to an environment:

```
$ conda install -n mynewenv newpackge
```

to specify an installation channel for the package:

```
$ conda install -n mynewenv -c conda-forge newpackge
```
