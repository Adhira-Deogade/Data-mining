# Data mining

1. Data importing
2. cleaning
3. transforming
4. visualization
5. summary statistics


## Data mining using Numpy, Pandas, matplotlib
### 1. Selecting and retrieving data [Selecting and retrieving data.ipynb](Selecting and retrieving data.ipynb)
  1. Creating dataframe
  2. SLicing dataframe
  3. Data comparison
  4. Filtering with scalars
  5. Setting values with scalars
     
### 2. Handling missing data [01_02](Handling missing data.ipynb)
  1. Figuring out what data is missing
  2. Filling missing values with "0"
  3. Filling missing values with desired values
  4. Filling missing values with "front-fill method"
  5. Counting missing values
  6. Filtering out missing values

### 3. Removing duplicates [01_03](Removing duplicates.ipynb)
   1. Obtaining duplicated values ```DF_obj.duplicated()```
   2. Removing duplciates ```DF_obj.drop_duplicates(['column 3'])```
   
### 4. Concatenating and transforming data [01_04](Concatenating and transforming data.ipynb)
   - ```axis=1``` signifies column operation
  1. Two dataframes side-by-side ```pd.concat([DF_obj, DF_obj_2], axis=1)```
  2. Two dataframe one below the other ```pd.concat([DF_obj, DF_obj_2])```
  3. Dropping data ```DF_obj.drop([0,2], axis=1)```
  4. Create and name a series object -> add it as a new column to our dataframe
  5. This can be done in two ways; either by ```df.join``` or by ```df.append```
  6. Sorting values; ```by="column_name``` and ```oreder="ascending/desccending"```
  
### 5. Grouping and data aggregation [01_05](Grouping and data aggregation.ipynb)
  1. Grouping data by column index ```cars.groupby(cars['cyl'])```
