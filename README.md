# Basics of Python [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/simklein/basics-of-python/master?filepath=index.ipynb)
This is an attempt of collecting and summarizing knowledge on Python and Python packaging. The collection of Jupyter Notebooks are meant to cover all basic information needed for the development of the [ITA Toolbox](https://git.rwth-aachen.de/mbe/haiopy) in Python.  
**Feel free to add any useful content.**


## Getting Started
The Jupyter Notebooks are available

* Online as [static web pages](http://nbviewer.ipython.org/github/simklein/basics-of-python/blob/master/index.ipynb) 
* Online for [interactive use](https://mybinder.org/v2/gh/simklein/basics-of-python/master?filepath=index.ipynb) using [binder](http://mybinder.org/)
* Local (offline) use on your computer

If you want to use the notebooks on your own computer, you will need a local Jupyter/IPython installation. If you don't have it installed jump to the [Anaconda](#anaconda) section. 
For a local version of this repo clone it with git. 
```
git clone https://github.com/simklein/basics-of-python.git
``` 


## Python
All Jupyter Notebooks in this project are based on Python.
Therefore you need Python installed to start them.
You can check if Python is already installed on your system by using the following commands:
```
python --version
```
Python 3 is recommended. Installation can be done on several ways:

On Windows or MacOSX, you can just download it from [python.org](https://www.python.org/downloads/).
On Linux, you should use your system's packaging system. For example, on Debian or Ubuntu:
```
sudo apt-get update
sudo apt-get install python3
```
An even simpler option is to download and install [Anaconda](https://www.anaconda.com/distribution/) for setting up Python the first time. Anaconda is a distribution of Python that comes with several packages, an IDE and a virtual environment manager.


## Anaconda
You should create an isolated environment for your projects to manage the varying dependencies. You can do this by using the following command:
```
conda create -n myenv anaconda
```
This will create a new virtual environment in the Anaconda directory with all packages installed that come with Anaconda. 

Use 
```
conda activate myenv
```
to work in this environment.
```
conda list
``` 
shows all the packages installed in the active environment.
You can install additional packages with
```
conda install ...
```

## Pip
Pip is another package installer for python that refers to the [Python Package Index](https://pypi.org/)(PyPi).
You can also [create virtual environments with Pip](https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/).  

First you should update to the current version
```
python -m pip install --user pip
```

If a package is not available on Conda you can use the following command to install packages:
```
pip install ...
```

The possible confusion between Pip and Conda can be resolved [here](https://www.anaconda.com/understanding-conda-and-pip/).


## Starting Jupyter Notebooks
You can start Jupyter by simply calling:
```
jupyter notebook
```
This will open up a new browser window (or a new tab) showing the Notebook Dashboard.
If your browser does not open automatically, visit [localhost:8888][linkLocalhost].
You can now see the contents of the current directory and are able to navigate to the desired Notebook Document.

Now you can go through the notebooks to get to know even more about Python.
