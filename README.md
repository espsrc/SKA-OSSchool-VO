# SKA Open Science School - The Virtual Observatory
![imagen](https://user-images.githubusercontent.com/7033451/236428499-32af9f82-7bf5-4128-a8af-b935e5b4a337.png)


This repository contains the tools and working environment to follow the workshop on the Virtual Observatory led by Jesús Salgado within the SKA Open Science School: https://www.granadacongresos.com/skaopenscience

The slides of this talk are available at 

https://docs.google.com/presentation/d/10EC7POY7ueFcOrtmap5OBOwP9zjyMELKJiFA43JemfY/edit#slide=id.g2398ceb5730_1_32.

When working with scientific software and packages, it is important to have a reproducible and easily accessible environment. There are several ways to achieve this, and three popular options are using Python environments, BinderHub, and JupyterHub.

* [Virtual Observatory workshop from a Python Environment](#virtual-observatory-from-a-python-environment)
* [Virtual Observatory workshop from a BinderHub Environment](#virtual-observatory-from-a-binderhub-environment)
* [Virtual Observatory from a Google Colab Notebook](#virtual-observatory-from-a-google-colab-notebook)
* [Virtual Observatory workshop from a JupyterHub within the Spanish SKA Regional Centre infrastructure](#virtual-observatory-from-a-jupyterhub-within-the-spanish-ska-regional-centre-infrastructure)

## Virtual Observatory from a Python Environment

Python environments, such as conda or virtualenv, allow you to create a separate environment for each project or task, with its own set of packages and dependencies. This ensures that each project is self-contained and reproducible, without conflicts between packages or libraries. Python environments can be easily created and managed using command-line tools, and they can be shared with collaborators or published for others to use. With conda, for example, you can create an environment file that lists all the packages and dependencies needed for your project, and then share it with others, who can easily create the same environment on their own system.

1. Open a terminal or command prompt and navigate to the directory containing your project files.
2. Clone this repository with `git clone https://github.com/spsrc/SKA-OSSchool-VO.git` and move to the folder created: `cd SKA-OSSchool-VO`
2. Create a new virtual environment using the following command:

``python -m venv myvoenv``

3. Activate the virtual environment using the following command:

``source myvoenv/bin/activate``

This will activate the virtual environment and any packages you install will be installed in this environment.

4. Install the dependencies listed in the `requirements.txt` file using the following command:

``pip install -r requirements.txt``

5. Install `jupyter notebooks`:

``pip install jupyterlab``

6. Finally run:

``jupyter-lab``

7. Then access to the `pleiades.ipynb`

## Virtual Observatory from a BinderHub Environment

Binder is another option for creating reproducible environments for scientific software and packages. Binder allows you to turn a repository containing Jupyter notebooks or Python scripts into an interactive environment, which can be accessed and run through a web browser. With Binder, you can easily share your work with others, without them needing to install any software or dependencies on their own system. This can be particularly useful for workshops or tutorials like this on Virtual Observatory.

To use this environment in order to play with the Virtual Observatory, click in the next link:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/spsrc/SKA-OSSchool-VO/HEAD)


## Virtual Observatory from a Google Colab Notebook

BinderHub is a public service that have several limitations. One of them is related with the number of users that can access to the repository to build a BinderHub during a period of time. Once these limits are reached you can not open this BinderHub. To avoid it, we've included a more stable solution by including this Virtual Observatory Notebook in a Google Colab service:

https://colab.research.google.com/drive/10eSWWWtjmspTW_cNhnvNp0HmHaZHb-6y?usp=sharing

*Click in this link and then click in "Connect", to allocate computing resources for this Notebook*


## Virtual Observatory from a JupyterHub within the Spanish SKA Regional Centre infrastructure

JupyterHub is a fourth option for creating reproducible environments for scientific software and packages. JupyterHub is a multi-user version of Jupyter Notebook, which allows you to create a shared environment for a group or team. With JupyterHub, each user can have their own environment, with its own set of packages and dependencies, while still sharing resources and collaborating with others. JupyterHub can be installed on a local server or on a cloud platform, such as Google Cloud or Amazon Web Services.

To use this environment, simply click on the below's link and authenticate with your credentials. In this case use your registration email as username and password.

[JupyterHub @ SPSRC](https://spsrc-jupyter.iaa.csic.es/soos/)

