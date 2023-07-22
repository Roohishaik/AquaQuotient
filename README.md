# AquaQuotient
A model visualizing United Nations Sustainable Development (UNSDG) Goal 6 of clean water and sanitation

United Nations Sustainable Development (UNSDG) Goal 6 focuses on ensuring safe water and sanitation for all. I have made a model which takes different attributes which contribute to the cleaniness and safety of water over different states in world and visualized the data using Tableau.

##  Table of Contents
- [Problem Statement](#-problem-statement)
- [Objective](#-objective)
- [Dataset](#-dataset)
- [Technology Used](#️-SMOTE)
- [Requirements](#-requirements)


# Problem Statement
Safe and easily accessible water is important to public health, whether it is used for drinking, domestic, food  or recreational purposes. Better water supply and sanitation and better management of water resources can significantly contribute  to poverty reduction and economic growth. Contaminated water and poor sanitation contribute to the spread of  cholera, diarrhea, dysentery, hepatitis A, typhoid and polio. Those without  clean water and sanitation face avoidable health risks. 

# Objective
To understand what constitutes safe, potable water and distinguish between potable and non-potable water by applying machine learning techniques.

# Dataset
The [dataset](https://www.kaggle.com/adityakadiwal/water-potability) contains water quality metrics for 3276 different water bodies.
- ph: pH of water (0 to 14).
- Hardness: Capacity of water to precipitate soap in mg/L.
- Solids: Total dissolved solids in ppm.
- Chloramines: Amount of Chloramines in ppm.
- Sulfate: Amount of Sulfates dissolved in mg/L.
- Conductivity: Electrical conductivity of water in μS/cm.
- Organic_carbon: Amount of organic carbon in ppm.
- Trihalomethanes: Amount of Trihalomethanes in μg/L.
- Turbidity: Measure of light emitting property of water in NTU.
- Potability: Indicates if water is safe for human consumption. Potable - 1 and Not potable - 0

#### Importing Dataset
```
df=pd.read_csv('water_potability.csv')
```
If your notebook and csv files are in different places you can write the whole path to import the file.
```
df=pd.read_csv('../input/water-potability/water_potability.csv')
```
# Technology Used

The data was highly imbalanced, hence we used **Synthetic Minority Oversampling TEchnique**, or SMOTE for short to balance the data.


# Models used for training

- **Logistic Regression** 
- **Support Vector Classifier** 
- **Random Forest Classifier** 
- **XGBoost -** 
  
##  Requirements 

### Libraries

The following python libraries were used to perform the various actions on the dataset from loading to preprocessing to visualizing and predicting the results.
 ```
import numpy as np 
import pandas as pd 
import matplotlib.pyplot as plt
import seaborn as sns
import plotly.express          as ex
import plotly.graph_objs       as go
import plotly.offline          as pyo
import scipy.stats             as stats
import pymc3                   as pm
import theano.tensor           as tt
```
[Numpy](https://github.com/numpy/numpy)- NumPy is the fundamental package needed for scientific computing with Python.

[Pandas](https://github.com/pandas-dev/pandas) - Python library used to analyze data.

[Matplotlib](https://github.com/matplotlib/matplotlib) - Most of the Matplotlib utilities lies under the pyplot submodule.

[Seaborn](https://seaborn.pydata.org/) - An open-source Python library built on top of matplotlib. It is used for data visualization and exploratory data analysis.

[Plotly](https://plotly.com/python/) - provides online graphing, analytics, and statistics tools for individuals and collaboration, as well as scientific graphing libraries for Python, R, MATLAB, Perl, Julia, Arduino, and REST.

[Scikit-learn](https://github.com/scikit-learn/scikit-learn) - tool for predictive data analysis built on numpy, scipy and matplotlib.

# Data visualization on Tableau 


https://github.com/Roohishaik/AquaQuotient/assets/94975857/41a1bb7d-56e0-4e29-b3a5-e762ad1ed466



https://github.com/Roohishaik/AquaQuotient/assets/94975857/f254637b-fa2d-4a6e-b27d-b6d4eaca91c2


![pic 3](https://github.com/Roohishaik/AquaQuotient/assets/94975857/76b91c80-2555-47a1-a83e-8de2753ccd36)


