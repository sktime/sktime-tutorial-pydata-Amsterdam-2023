Welcome to the sktime tutorial at pydata Amsterdam 2023
=======================================================

Abstract

[skpro]: https://skpro.readthedocs.io/en/latest
[sktime]: https://sktime.net

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sktime/sktime-tutorial-pydata-Amsterdam-2023/main?filepath=notebooks) [![!discord](https://img.shields.io/static/v1?logo=discord&label=discord&message=chat&color=lightgreen)](https://discord.com/invite/54ACzaFsn7) [![!slack](https://img.shields.io/static/v1?logo=linkedin&label=LinkedIn&message=news&color=lightblue)](https://www.linkedin.com/company/scikit-time/)

## :rocket: How to get started

In the tutorial, we will move through notebooks section by section.

You have different options how to run the tutorial notebooks:

* Run the notebooks in the cloud on [Binder] - for this you don't have to install anything!
* Run the notebooks on your machine. [Clone] this repository, get [conda], install the required packages (`sktime`, `seaborn`, `jupyter`) in an environment, and open the notebooks with that environment. For detail instructions, see below. For troubleshooting, see sktime's more detailed [installation instructions].
* or, use python venv, and/or an editable install of this repo as a package. Instructions below.

[Binder]: https://mybinder.org/v2/gh/sktime/sktime-tutorial-europython-2023/main?filepath=notebooks
[clone]: https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository
[conda]: https://docs.conda.io/en/latest/
[installation instructions]: https://www.sktime.net/en/latest/installation.html

Please let us know on the [sktime discord](https://discord.com/invite/54ACzaFsn7) if you have any issues during the conference, or join to ask for help anytime.

## :bulb: Description

Description

## :movie_camera: Other Tutorials:

- [EuroPython 2023 - General sktime introduction](https://github.com/sktime/sktime-tutorial-europython-2023)

- [Pydata Berlin 2022 - Advanced Forecasting Tutorial](https://www.youtube.com/watch?v=4Rf9euAhjNc)

- [Pydata London 2022 - How to implement your own estimator in sktime](https://www.youtube.com/watch?v=S_3ewcvs_pg)

- [Pydata Global 2022 - Feature extraction, Pipelines, Tuning](https://github.com/sktime/sktime-tutorial-pydata-global-2022)

- [Pydata London 2023 - Time Series Classification, Regression, Distances & Kernels](https://github.com/sktime/sktime-tutorial-pydata-london-2023)

## :wave: How to contribute

If you're interested in contributing to sktime, you can find out more how to get involved [here](https://www.sktime.net/en/latest/get_involved.html).

Any contributions are welcome, not just code!

## Installation instructions for local use

To run the notebooks locally, you will need:

* a local repository clone
* a python environment with required packages installed

### Cloning the repository

To clone the repository locally:

`git clone https://github.com/sktime/sktime-tutorial-pydata-Amsterdam-2023.git`

### Using conda env

1. Create a python virtual environment:
`conda create -y -n tutorial_env python=3.9`
2. Install required packages:
`conda install -y -n tutorial_env pip skpro sktime seaborn jupyter pmdarima statsmodels`
3. Activate your environment:
`conda activate tutorial_env`
4. If using jupyter: make the environment available in jupyter:
`python -m ipykernel install --user --name=tutorial_env`

### Using python venv

1. Create a python virtual environment:
`python -m venv tutorial_env`
2. Activate your environment:
`source tutorial_env/bin/activate`
3. Install the requirements:
`pip install skpro sktime seaborn jupyter pmdarima statsmodels`
4. If using jupyter: make the environment available in jupyter:
`python -m ipykernel install --user --name=tutorial_env`
