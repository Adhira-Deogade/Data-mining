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
  [Image of functional method](https://github.com/Adhira-Deogade/Data-mining/blob/master/Functional%20labelling.png)
  2. Object oriented annotation:
  [Annotation image](https://github.com/Adhira-Deogade/Data-mining/blob/master/Object%20oriented%20annotation.png)
  
### 9. 
