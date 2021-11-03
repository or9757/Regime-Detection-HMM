# Regime-Detection-HMM
This case study uses the Hidden Markov Model to correctly identify different market regimes in the US financial markets and provide the investment strategy depending on the current regime. We assume that there are two market states : 
• low uncertainty (relatively stable and resilient) market 
• high uncertainty (relatively chaotic and fragile) market
Detecting and shifting regimes are always challenging for investors since Performance, risk and behavior of portfolio may impacts on significantly.

## HMM

A Hidden Markov Model is a statistical model that can be used to describe the evolution of observable events that depends on interval factors, which are not directly observable. 

Main issues using HMM: 

-	Decoding Problem
	Given HMM M = (A,B,p), and the observation sequence O = o_1, .. o_k, calculate the most likely sequence of hidden states S_i that produced this observation sequence O. 
-	Learning Problem
	Given some training observation sequences, O= o_1, o_2, …o_k and general structure of HMM, determine HMM parameters M = (A,B,p) that best fit training data 
  
Usually, Decoding problem is solving by Viterbi Algorithm and B-W algorithm is used for the Learning Problem. 
Here, we used HMM.GaussianHmm Python Package is used to get the decoding and learning problem of HMM

## Steps to run the project on each machine 

#### Python 3
In this project, we would like to Python. Usually, Python 3 is already installed on many systems these days. By checking the version of the python, any version of Python 3 should be enough to run this model. 
```
pip -V #Returns the path and version of the Python 3
```


If you do not have python 3, please go to the link below and download. 
>https://www.python.org/download/releases/3.0/

#### Anaconda
Once you check you have Python 3, downloading the Anaconda is recommended. Anaconda is a distribution of the Python and R programming languages for scientific computing that aims to simplify package management and deployment. 

* Anaconda installation guideline for Window Users :
>https://docs.anaconda.com/anaconda/install/windows/

* Anaconda installation guideline for Mac OS Users :
>https://docs.anaconda.com/anaconda/install/mac-os/

#### Jupyter Notebook
Now, You can download and start Jupyter Notebook  start on your terminal. 
```
conda install -c conda-forge notebook
```
Then type 
```
jupyter notebook 
```

#### Python Packages
Now, you need to download the packages those are required to run our model 
```
pip install pandas

pip install numpy

pip install matplotlib

pip install seaborn

pip install hmmlearn
```

If Jupyter notebook is running properly, need to install several Python libraries to run our project. 
```
import pandas as pd

import numpy as np

import matplotlib.pyplot as plt

from matplotlib import cm

import seaborn as sns

from hmmlearn import hmm 
```

Then simply follow our steps that we show in HMM.ipython file

Data is private. But you can download SPY or other index from Yahoo Finance or other websites. 
References
https://www.mdpi.com/1911-8074/13/12/311/htm https://github.com/Marblez/HMM_trading/blob/master/hmm.ipynb
Dynamic Portfolio Optimization across Hidden Market Regimes 


 

