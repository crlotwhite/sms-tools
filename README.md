sms-tools
========= 

How to install in 2025 for coursera course.

Windows Evironment

Install Ubuntu 18.04
```
wsl --install Ubuntu-18.04
```

Install python and dependencies
```
sudo apt update -y && sudo apt upgrade -y && sudo apt install -y build-essential
sudo apt install python2.7
sudo apt install python-pip
git clone https://github.com/MTG/sms-tools.git
cd sms-tools/
git checkout 762d2006d3ab1a730a49a6a36179861332135ee8
sudo apt-get install python-dev ipython python-numpy python-matplotlib python-scipy cython
cd software/models/utilFunctions_C/
python2.7 compileModule.py build_ext --inplace
```

Test
```
cd software/models_interface
python models_GUI.py 
```

Mac os
WIP...

original README.md
=========

Sound analysis/synthesis tools for music applications written in python.

The package includes the following sound analysis/synthesis models:

* dftModel.py: models based on the Discrete Fourier Transform
* stft.py: models based on the Short-Time Fourier Transform
* sineModel.py: models based on a Sinusoidal Model
* harmonicModel.py: models based on a Harmonic Model
* stochasticModel.py: models based on a Stochastic Model
* sprModel.py: models based on a Sinusoidal plus Residual Model
* spsModel.py: models based on a Sinusoidal plus Stochastic Model
* hprModel.py: models based on a Harmonic plus Residual Model
* hpsModel.py: models based on a Harmonic plus Stochastic Model


Installation
------------

Install using pip:

    pip install sms-tools

Binary packages are available for Linux, macOS (Intel & Apple Silicon) and Windows (64 bit) on all recent python versions.

To build and install the package locally you can use the python packaging tools:

    pip install build
    python -m build


Jupyter Notebooks
-------
We provide a separate repository of examples and teaching materials in the form of Jupyter notebooks.
You can find them at https://github.com/MTG/sms-tools-materials

License
-------

sms-tools is made available under the terms of the Affero GPL license (http://www.gnu.org/licenses/agpl-3.0.en.html). 
