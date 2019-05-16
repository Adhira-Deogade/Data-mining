# Data mining

1. Data importing
2. Cleaning
3. Transforming
4. Visualization
5. Summary statistics


## Data mining using Numpy, Pandas, matplotlib
All codes in Jupyter notebook

### A. [Data munging](https://github.com/Adhira-Deogade/Data-mining/tree/master/Data%20munging)

#### 1. Selecting and retrieving data [1.1](https://github.com/Adhira-Deogade/Data-mining/blob/master/Data%20munging/1.%20Selecting%20and%20retrieving%20data.ipynb)
  1. Creating dataframe
  2. SLicing dataframe
  3. Data comparison
  4. Filtering with scalars
  5. Setting values with scalars
     
#### 2. Handling missing data [1.2](https://github.com/Adhira-Deogade/Data-mining/blob/master/Data%20munging/2.%20Handling%20missing%20data.ipynb)
  1. Figuring out what data is missing
  2. Filling missing values with "0"
  3. Filling missing values with desired values
  4. Filling missing values with "front-fill method"
  5. Counting missing values
  6. Filtering out missing values

#### 3. Removing duplicates [1.3](https://github.com/Adhira-Deogade/Data-mining/blob/master/Data%20munging/3.%20Removing%20duplicates.ipynb)
   1. Obtaining duplicated values ```DF_obj.duplicated()```
   2. Removing duplciates ```DF_obj.drop_duplicates(['column 3'])```
   
#### 4. Concatenating and transforming data [1.4](https://github.com/Adhira-Deogade/Data-mining/blob/master/Data%20munging/4.%20Concatenating%20and%20transforming%20data.ipynb)
   - ```axis=1``` signifies column operation
  1. Two dataframes side-by-side ```pd.concat([DF_obj, DF_obj_2], axis=1)```
  2. Two dataframe one below the other ```pd.concat([DF_obj, DF_obj_2])```
  3. Dropping data ```DF_obj.drop([0,2], axis=1)```
  4. Create and name a series object -> add it as a new column to our dataframe
  5. This can be done in two ways; either by ```df.join``` or by ```df.append```
  6. Sorting values; ```by="column_name``` and ```oreder="ascending/desccending"```
  
#### 5. Grouping and data aggregation [1.5](https://github.com/Adhira-Deogade/Data-mining/blob/master/Data%20munging/5.%20Grouping%20and%20data%20aggregation.ipynb)
  1. Grouping data by column index ```cars.groupby(cars['cyl'])```
  
### B. [Data visualization](https://github.com/Adhira-Deogade/Data-mining/tree/master/Visualization)

#### 1. Creating standard plots [2.1](https://github.com/Adhira-Deogade/Data-mining/blob/master/Visualization/1.%20Creating%20standard%20plots.ipynb)
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

#### 2. Scaling and subplotting [2.2](https://github.com/Adhira-Deogade/Data-mining/blob/master/Visualization/2.%20Scaling%20and%20subplotting.ipynb)
  1. Scaling axes ```ax.set_xlim([1,9])``` and ```ax.set_ylim([0,5])```
  2. Subplotting charts:
  ```python
  fig = plt.figure()
  fig, (ax1,ax2) = plt.subplots(1,2)
  ax1.plot(x)
  ax2.plot(x, y)
```
#### 3. Histograms, pie-charts, overlapping line charts [2.3](https://github.com/Adhira-Deogade/Data-mining/blob/master/Visualization/3.%20Histograms%2C%20piecharts%2C%20overlapping%20line%20charts.ipynb)
  1.Adjusting colours
  2. Customizing line styles
  3. Marker styles
  
#### 4. Creating labels and annotations [2.4](https://github.com/Adhira-Deogade/Data-mining/blob/master/Visualization/4.%20Creating%20labels%20and%20annotation.ipynb)
  1. Functional method:
  ![Image of functional method](https://github.com/Adhira-Deogade/Data-mining/blob/master/Images/hist.jpg)
  2. Object oriented annotation:
  ![Annotation image](https://github.com/Adhira-Deogade/Data-mining/blob/master/Images/cars.jpg)
  
#### 5. Time series [2.5](https://github.com/Adhira-Deogade/Data-mining/blob/master/Visualization/5.%20Time%20series.ipynb)
  1. Sample and plot data
  2. Check out next repo for analysis

#### 6. Density, boxplots, summary statistics [2.6](https://github.com/Adhira-Deogade/Data-mining/blob/master/Visualization/6.%20Density%2C%20boxplots%2C%20summary%20statistics.ipynb)
  1. Density plot ```sb.distplot(mpg)```
  2. Scatter plot
  3. Regression plot
  4. Pairplot
  5. Pair plot with column colouring
  6. Boxplots ```cars.boxplot(column='mpg', by='am')```
  ![Boxplot image](https://github.com/Adhira-Deogade/Data-mining/blob/master/Images/boxplot.jpg)
