# mynotebook

import pandas as pd
import numpy as np
from sklearn.datasets import load_diabetes

#Load our diabetes dataset
diabetes = load_diabetes()

#Convert the data to a pandas dataframe
my_df = pd.DataFrame (diabetes.data, columns=diabetes.feature_names)

#Add the target - 25 to 346
my_df['target'] = diabetes.target

#Grab the head
my_df.head()