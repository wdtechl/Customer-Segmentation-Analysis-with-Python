# Customer-Segmentation-Analysis-with-Python
import pandas as pd

import numpy as np

import matplotlib.pyplot as plt

%matplotlib inline

import pandas_profiling

import autoviz

from sklearn.preprocessing import OneHotEncoder

from sklearn.preprocessing import StandardScaler

from sklearn.cluster import KMeans

import seaborn as sns
# loading data
data=pd.read_csv('../input/customer-segmentation-tutorial-in-python/Ma 11 Customers.csv')

data.head()

data.info()

data.describe().T

#EDA

pandas_profiling. Profile Report(data, title="Pandas Profiling Report", explorative=True)
