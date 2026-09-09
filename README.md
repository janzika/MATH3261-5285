# MATH3261-5285: Fluids, Oceans and Climate

Repository of learning materials for Fluids, Oceans and Climate, a course at UNSW.

This course aims to provide a solid foundation for the analysis of geophysical flows that arise in the study of the ocean, the atmosphere, and their interactions in the climate system. This course introduces the fundamental equations of motion and conservation laws that govern the fluid dynamics of the atmosphere and the ocean. These equations are then systematically simplified and solved to quantitatively model key phenomena selected from the enormously rich variety of atmospheric and oceanic flows.

A key skill to be developed in this course is a physical understanding of fluid flows. Students will study and perform numerical experiments of simplified geophysical systems in order to see beyond the mathematical formalism and gain a robust understanding of the sometimes counter-intuitive behaviour of geophysical flows.

Currently this repostiory contains ipython notebook for a set of computer labs that will be held throughout the course. The labs can be completed online from any browser window using Google Colaboratory (Colab) or locally by installing the necessary libraries in a `conda` environment (see below for instructions).
These labs were first written by [Dr Shane Keating](https://www.unsw.edu.au/staff/shane-keating) with some later edits by Drs [Jan Zika](https://www.unsw.edu.au/staff/jan-zika) and [Josef Bisits](https://jbisits.github.io).

## Opening the notebooks using Google Colab (secommended - no experience needed)

Open one of the notebooks (`.ipynb` files above) and click on the colab button <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a> at the top.
After that save a copy to your google drive so you can edit and access later on and you should be good to go!

## Local installation and usage in JupyterLab or VS Code (some knowledge of computing environments with python package management is needed)

We use a python package manager called [pixi](https://pixi.prefix.dev/latest/) to ensure reproducability.

First clone this repository, you can create your own fork first if you prefer,

```
git clone https://github.com/janzika/MATH3261-5285
```

To install the required packages, change into the directory where this repository is cloned and, after [installing pixi](https://pixi.prefix.dev/latest/installation/), run:

```
pixi install --locked
```

This will download and build all the depednecies required.
If you encounter something unusal please raise an issue.

To run the notebooks, use

```
pixi run jupyter-lab
```

and select the Python (pixi) or Python (ipykernel) kernel for running the notebooks.
**NOTE:** there is a a jupyter-lab installation specific for these notebooks inside the pixi environmet so make sure to use `pixi run jupyter-lab` within the directory you have cloned the repository into.
Microsoft's [vs-code](https://code.visualstudio.com/) with the [jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter) should be able to be used; just make sure you have selected the correct kernel.

