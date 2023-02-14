# Pywake-start 
It's just talk about how to install Pywake and check if it is successfully donload as a starter.

#### *Note:* This is my experience as a novice installing Pywake and the problems I encountered. From the beginning when I didn't even understand the basic concepts of python environment and such, to the final successful installation of Pywake, just as a souvenir and to help other beginners similar to me who started from scratch. 

#### Note: It is 2023 Feb. 12, I just successfully download the Pywake and run some Examples, and in the further steps like adjust the parameters will be discuss in the future.

# First

## Basic 

A python environment needs to be downloaded. In my design, the Anacoda-Navigator is used.

1. Download Anacoda-Navigator (Python 3.x version, 64 bit installer is recommended) on its official website: [Anacoda-Navigator](https://www.anaconda.com/products/distribution)
2. Update the root Anaconda environment(Do it in terminal):
```
conda update --all
```
3. Activate the Anaconda root environment(also in ternimal):
```
activate
```

#### Until now, python environment is installed.

To check if it is already installed successfully, run the code below:
```
python --version
```

If it is installed, you can see the terminal return the following words:
```
Python 3.x.x
```
Here shows your Python edition.

# Second

## Install PyWake

You can think of PyWake as one of the python library files. Once you have downloaded PyWake, you can run the contents of PyWake in code.

1. Download PyWake by one of below:

+ Install from PyPi.org (official releases):
```
pip install py_wake
```

+ Install from GitLab (includes any recent updates):
```
pip install git+https://gitlab.windenergy.dtu.dk/TOPFARM/PyWake.git
```

+ Another method
```
conda install pywake
```

#### Until now, PyWake is installed.

To check if it is already installed successfully, run the code below:
```
pywake --version
```

If it is installed, you can see the terminal return the following words:
```
PyWake 0.x.x
```
Here shows your PyWake edition.



