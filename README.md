# Data mining

1. Data importing
2. Cleaning
3. Transforming
4. Visualization
5. Summary statistics


## Data mining using Numpy, Pandas, matplotlib
All codes in Jupyter notebook

### 1. Selecting and retrieving data [1.1](https://github.com/Adhira-Deogade/Data-mining/blob/master/Selecting%20and%20retrieving%20data.ipynb)
  1. Creating dataframe
  2. SLicing dataframe
  3. Data comparison
  4. Filtering with scalars
  5. Setting values with scalars
     
### 2. Handling missing data [1.2](https://github.com/Adhira-Deogade/Data-mining/blob/master/Handling%20missing%20data.ipynb)
  1. Figuring out what data is missing
  2. Filling missing values with "0"
  3. Filling missing values with desired values
  4. Filling missing values with "front-fill method"
  5. Counting missing values
  6. Filtering out missing values

### 3. Removing duplicates [1.3](https://github.com/Adhira-Deogade/Data-mining/blob/master/Removing%20duplicates.ipynb)
   1. Obtaining duplicated values ```DF_obj.duplicated()```
   2. Removing duplciates ```DF_obj.drop_duplicates(['column 3'])```
   
### 4. Concatenating and transforming data [1.4](https://github.com/Adhira-Deogade/Data-mining/blob/master/Concatenating%20and%20transforming%20data.ipynb)
   - ```axis=1``` signifies column operation
  1. Two dataframes side-by-side ```pd.concat([DF_obj, DF_obj_2], axis=1)```
  2. Two dataframe one below the other ```pd.concat([DF_obj, DF_obj_2])```
  3. Dropping data ```DF_obj.drop([0,2], axis=1)```
  4. Create and name a series object -> add it as a new column to our dataframe
  5. This can be done in two ways; either by ```df.join``` or by ```df.append```
  6. Sorting values; ```by="column_name``` and ```oreder="ascending/desccending"```
  
### 5. Grouping and data aggregation [1.5](https://github.com/Adhira-Deogade/Data-mining/blob/master/Grouping%20and%20data%20aggregation.ipynb)
  1. Grouping data by column index ```cars.groupby(cars['cyl'])```
  
  
### 6. Creating standard plots [2.1](https://github.com/Adhira-Deogade/Data-mining/blob/master/Creating%20standard%20plots.ipynb)
  1. Required [seaborn](https://seaborn.pydata.org/) library
  2. Run the code as it is in python notebook ```! pip install Seaborn```
  3. Needed ```import matplotlib.pyplot as plt```
  4. Instant plot results ```%matplotlib inline ```
  5. Set figure size ```rcParams['figure.figsize']=5,4```
  6. Set figure style ```sb.set_style('whitegrid')```
  7. Creating line chart
  8. Ploting a line chart from pandas object/ dataframe
  9. Creating bar charts
  10. Bar charts from dataframes
  11. Creating pie charts
  12. Saving plots (as images)

### 7. Scaling and subplotting [2.2](https://github.com/Adhira-Deogade/Data-mining/blob/master/Scaling%20and%20subplotting.ipynb)
  1. Scaling axes ```ax.set_xlim([1,9])``` and ```ax.set_ylim([0,5])```
  2. Subplotting charts:
  ```python
  fig = plt.figure()
  fig, (ax1,ax2) = plt.subplots(1,2)
  ax1.plot(x)
  ax2.plot(x, y)
```
### 8. Creating labels and annotations [2.3](https://github.com/Adhira-Deogade/Data-mining/blob/master/Creating%20labels%20and%20annotation.ipynb)
  1. Functional method:
  [Images of functional method](data:image/png;base64,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%0ADEVEAPg/m/P3O1ldFFgAAAAASUVORK5CYII=%0A)
  
