# Installation

DataFusion is easy to install, just like any other Python library.

## Using Pip

``` bash
pip install datafusion
```

## conda & JupyterLab setup

This section explains how to install DataFusion in a conda environment with other libraries that create a really nice JupyterLab setup.  This setup is completely optional.  These steps are only needed if you'd like to run DataFusion in a Jupyter notebook like this:

![DataFusion in Jupyter](https://github.com/MrPowers/datafusion-book/raw/main/src/images/datafusion-jupyterlab.png)

Create a conda environment with DataFusion, Jupyter, and other nice dependencies in the `datafusion-env.yml` file:

```
name: datafusion-env
channels:
  - conda-forge
  - defaults
dependencies:
  - python=3.9
  - ipykernel
  - nb_conda
  - jupyterlab
  - jupyterlab_code_formatter
  - isort
  - black
  - pip
  - pip:
    - datafusion

```

Create the environment with `conda env create -f datafusion-env.yml`.

Activate the environment with `conda activate datafusion-env`.

Run `jupyter lab` or open the [JupyterLab Desktop application](https://github.com/jupyterlab/jupyterlab-desktop) to start running DataFusion in a Jupyter notebook.


