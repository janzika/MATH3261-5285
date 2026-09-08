# MATH3261-5285: Fluids, Oceans and Climate

Repository of learning materials for Fluids, Oceans and Climate, a course at UNSW.

This course aims to provide a solid foundation for the analysis of geophysical flows that arise in the study of the ocean, the atmosphere, and their interactions in the climate system. This course introduces the fundamental equations of motion and conservation laws that govern the fluid dynamics of the atmosphere and the ocean. These equations are then systematically simplified and solved to quantitatively model key phenomena selected from the enormously rich variety of atmospheric and oceanic flows.

A key skill to be developed in this course is a physical understanding of fluid flows. Students will study and perform numerical experiments of simplified geophysical systems in order to see beyond the mathematical formalism and gain a robust understanding of the sometimes counter-intuitive behaviour of geophysical flows.

Currently this repostiory contains ipython notebook for a set of computer labs that will be held throughout the course. The labs can be completed online from any browser window using Google Colaboratory (Colab) or locally by installing the necessary libraries in a `conda` environment (see below for instructions).
These labs were first written by [Dr Shane Keating](https://www.unsw.edu.au/staff/shane-keating) with some later edits by Drs [Jan Zika](https://www.unsw.edu.au/staff/jan-zika) and [Josef Bisits](https://jbisits.github.io).

## Opening the notebooks using Google Colab (Recommended - no experience needed)

Open one of the notebooks (`.ipynb` files above) and click on the colab button <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> at the top.
After that save a copy to your google drive so you can edit and access later on and you should be good to go!

## Local installation and usage in JupyterLab or VS Code (Some knowledge of computing environments using conda assumed)

To install the required packages in a `conda` environment you will need to have `conda` installed.
This can be done using [`miniconda`](https://docs.anaconda.com/miniconda/) or [`Anaconda`](https://docs.anaconda.com/anaconda/), [here](https://docs.anaconda.com/distro-or-miniconda/) is some information about which is most suited to you.

To run the notebooks in this repository locally first clone (or fork) this repository to your machine in a terminal

```terminal
git clone https://github.com/janzika/MATH3261-5285
```

then change to the directory where the clone is. E.g.

```terminal
cd /FILEPATH/MATH3261-5285
```

After that build the `conda` environment from the `MATH3261_5285.yaml` file

```terminal
conda env create -f MATH3261_5285.yaml
```

The notebooks can then be run using [JupyterLab](https://jupyter.org/), installed using `conda` and an additional package to allow a distinct `kernel' for these notebooks.

```terminal
conda install jupyterlab nb_conda_kernels
```

or Microsoft's [vs-code](https://code.visualstudio.com/) with the [jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter).

**Note:** when running the notebooks in [Jupyterlab](https://doc.cocalc.com/howto/jupyter-kernel-selection.html) or [vs-code](https://code.visualstudio.com/docs/datascience/jupyter-kernel-management) make sure the MATH3261_5285 python notebook kernel is selected.
