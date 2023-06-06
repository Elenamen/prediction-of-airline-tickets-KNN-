# prediction-of-airline-tickets-KNN

**Highlights**

      -df['Column'].apply(lambda) method for applying functions in data series
      
      -eval()
      
**Sidenote** feature encoding:

Categorical data refers to a data type that can be stored into groups/categories/labels 
such as: age group, educational level,blood type etc.. 

Numerical data refers to the data that is in the form of numbers, 
Examples of numerical data are height, weight, age etc.. 

Numerical data has two categories: discrete data and continuous data:
      -Discrete data : 1, 2, 3, 4, 5, and so on.                             
      -Continuous data :  amount of sugar , 11.2 kg  , temp of a city  , your bank balance !
                  
We are using 2 basic Encoding Techniques to convert Categorical data into some numerical format
      -Nominal data --> data are not in any order --> OneHotEncoder is used in this case
      -Ordinal data --> data are in order -->       LabelEncoder is used in this case
      
!! While feature encoding beware of curse of dimensionality !! --> optimized features technique

__Target Guided Mean Encoding

gold source = https://towardsdatascience.com/dealing-with-categorical-variables-by-using-target-encoder-a0f1733a4c69
The main idea behind the target encoder is to encode the categories by replacing them for a measurement of the effect they might have on the target.

__List of data visualization plots to spot the outliers
1. Box and whisker plot (box plot).
2. Scatter plot.
3. Histogram.
4. Distribution Plot

__Cause for outliers 

Data Entry Errors:- Human errors such as errors caused during data collection, recording, or entry can cause outliers in data.
Measurement Error:- It is the most common source of outliers. This is caused when the measurement instrument used turns out to be faulty.

visualization plots to spot the outliers:
1. Box and whisker plot (box plot).
2. Scatter plot.
3. Histogram.
4. Distribution Plot.


If Features Are Skewed We Use the below Technique which is IQR
Data which are greater than IQR +1.5 IQR and data which are below than IQR - 1.5 IQR are my outliers
where ,  IQR = 75th%ile data - 25th%ile data

& IQR +- 1.5 IQR  will be changed depending upon the domain ie it could be sometimes IQR +- 3IQR 
