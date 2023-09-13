Welcome to the sktime tutorial at pydata Amsterdam 2023
=======================================================

This tutorial is about making probabilistic predictions, probabilistic forecasts with [sktime],
and probabilistic supervised regression with [skpro]:

* `sktime` is a unified framework for various time series related machine learning tasks including forecasting, classification, regression.
* `skpro` is a unified framework for tabular probabilistic predictions and tabular probability distributions.

`sktime` and `skpro` are designed interoperable, and both contains algorithms and tools for building, applying, evaluating modular pipelines and composites. Both packages are easily extensible by anyone, and interoperable with the python data science stack including `sklearn`, `skbase`, and `pandas`.

The presentation will showcase probabilistic prediction in ``skpro`` and ``sktime``:

* probabilistic prediction interfaces
* probabilistic prediction metrics, e.g., quantile loss, or CRPS, log-loss for distribution forecasts
* tuning using probabilistic metrics
* conformal probabilistic intervals for any pipeline
* compositors to make any point prediction estimator probabilistic
* for time series: hierarchical and global probabilistic forecasts, reduction to regression

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

Probabilistic predictions make statements about the uncertainty or likely variation of the forecast, e.g., intervals at nominal coverage or conditional distributions.
They appear in probabilistic forecasting as well as in probabilistic supervised (tabular) regression.
This tutorial presents probabilistic forecasting capability in the `skpro` and `sktime` packages, combined with a methodological overview.

`sktime` is a widely used package for time series, `skpro` covers probabilistic (tabular) regression. Both are based on `skbase`, and designed for interoperability with each other and `sklearn`.

This tutorial presents the joint designs for probabilistic predictions and modular estimator interfaces. It also gives an overview of pipelines, tuning using probabilistic metrics, and compositors that can be used to turning any point forecaster into probabilistic forecasters, such as conformal or empirical interval estimators.

The presentation will showcase `skpro` and `sktime`, for tabular and time series tasks:

* probabilistic prediction interfaces
* metrics, e.g., quantile loss, or CRPS, log-loss for distribution forecasts
* tuning using probabilistic metrics
* conformal probabilistic intervals for any pipeline
* compositors to make any point prediction estimator probabilistic
* for time series: hierarchical and global probabilistic forecasts, reduction to regression

From a methodological perspective, we will cover:

* interval forecasts: producing intervals with a nominal probability of the observation to be contained in the interval
* quantile forecasts: specifying one or multiple quantiles of a predictive forecast distribution
* fully probabilistic forecasts: producing a symbolic representation of a predictive forecast distribution
* simulators or samplers from probabilistic forecasting models

As research on software interfaces and mathematical conceptualization in this area is still an ongoing endeavour, challenges will also be discussed, with invitations to contribute.

`sktime` and `skpro` are developed by an open community, with aims of ecosystem integration in a neutral, charitable space.
We welcome contributions and seek to provides opportunity for anyone worldwide.
We invite anyone to get involved as a developer, user, supporter (or any combination of these).

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
