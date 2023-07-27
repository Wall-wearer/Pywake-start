# Pywake-start 
It's just talking about how to install Pywake and check if it is successfully downloaded as a starter. And share my experience while doing my PyWake project.

#### *Note:* This is my experience as a novice installing Pywake and the problems I encountered. From the beginning when I didn't even understand the basic concepts of Python environment and such, to the final successful installation of Pywake, just as a souvenir and to help other beginners similar to me who started from scratch. 

#### Note: It is 2023 Feb. 12, I just successfully download the Pywake and run some Examples, and in further steps like adjusting the parameters will be discussed in the future.

# First

## Basic 

A Python environment needs to be downloaded. In my design, the Anacoda-Navigator is used.

1. Download Anaconda-Navigator (Python 3. x version, a 64-bit installer is recommended) on its official website: [Anacoda-Navigator](https://www.anaconda.com/products/distribution)
2. Update the root Anaconda environment(Do it in terminal):
```
conda update --all
```
Here, if use Windows, should run Anaconda-Navigator to start it and use the terminal inside.
3. Activate the Anaconda root environment(also in terminal):
```
activate
```

#### Until now, the Python environment is installed.

To check if it is already installed successfully, run the code below:
```
python --version
```

If it is installed, you can see the terminal return the following words:
```
Python 3. x.x
```
Here is your Python edition.

# Second

## Install PyWake

You can think of PyWake as one of the Python library files. Once you have downloaded PyWake, you can run the contents of PyWake in code.

1. Download PyWake by one of the below:

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

# Third

Now, try to run some examples. You can find it on [PyWake Official Git](https://github.com/DTUWindEnergy/PyWake)

~~1. Copy a code from that link.~~
~~2. Open a text software whatever you like, and paste it into the Text Editor. Save as **.py** file.~~
~~3. Find the folder you put the file in. Run the code below in the terminal:~~

~~#### Then, you can get results.~~

Later, I found it useful to use the Jupyter Notebook.

Then things change to just copying the code from the website column by column and creating a `xx.ipyk` file paste the code into it.

# Start coding

Once ready, you can coding now.

Start with 
```ruby
# Install PyWake if needed. Check if Pywake is successfully installed
try:
    import py_wake
except ModuleNotFoundError:
    !pip install git+https://gitlab.windenergy.dtu.dk/TOPFARM/PyWake.git
```

Then, put the basic elements of Python.

```ruby
# 导入python基本元素
import os
import numpy as np #用于处理数组的库
import matplotlib.pyplot as plt #绘图
```

And put the functions you need into the next column.

```ruby
# Here, input wind turbines.
from py_wake.wind_turbines import WindTurbine, WindTurbines
from py_wake.examples.data.hornsrev1 import V80
from py_wake.examples.data.iea37 import IEA37_WindTurbines, IEA37Site
from py_wake.examples.data.dtu10mw import DTU10MW
# setup site, wind turbines and wind farm model with the corresponding wake models
from ipywidgets import interact
from ipywidgets import IntSlider
from scipy.interpolate import interp1d
from py_wake.flow_map import HorizontalGrid
from py_wake.examples.data.iea37._iea37 import IEA37Site, IEA37_WindTurbines
from py_wake.deficit_models.gaussian import BastankhahGaussian
from py_wake.deflection_models.jimenez import JimenezWakeDeflection
from py_wake.deflection_models import FugaDeflection
from py_wake.deflection_models import GCLHillDeflection
from py_wake.deficit_models.gaussian import BastankhahGaussianDeficit
from py_wake.superposition_models import LinearSum
from py_wake.superposition_models import SquaredSum
from py_wake.superposition_models import MaxSum
from py_wake.wind_farm_models import PropagateDownwind
from py_wake.wind_farm_models.wind_farm_model import SimulationResult
from py_wake.deficit_models import ZongGaussianDeficit
from py_wake.deficit_models import NOJDeficit
from py_wake.utils.model_utils import get_models
from py_wake.deficit_models.deficit_model import WakeDeficitModel
from py_wake.wind_farm_models import All2AllIterative
from py_wake.deficit_models import FugaYawDeficit
from py_wake.deficit_models import FugaDeficit
from matplotlib import cm
from matplotlib.colors import ListedColormap, LinearSegmentedColormap
from py_wake.deficit_models.deficit_model import WakeDeficitModel, BlockageDeficitModel
from py_wake.deficit_models.no_wake import NoWakeDeficit
from py_wake.site._site import UniformSite
from py_wake.flow_map import XYGrid
from py_wake.turbulence_models import CrespoHernandez
from py_wake.utils.plotting import setup_plot
from py_wake.wind_farm_models import All2AllIterative
from py_wake.deficit_models import NOJDeficit, SelfSimilarityDeficit
from py_wake.turbulence_models import STF2017TurbulenceModel, IECWeight
from py_wake.turbulence_models.stf import STF2005TurbulenceModel
from py_wake.turbulence_models import GCLTurbulence
```




