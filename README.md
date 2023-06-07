# prediction-of-airline-tickets-KNN

**Highlights**

      -df['Column'].apply(lambda) method for applying functions in data series
      
      -eval()
      
      -pickle.load(model) / pickle.dumb(model,file)
      
**Sidenote** feature encoding:

Categorical vs Numerical (discrete data and continuous data)

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

If Features Are Skewed We Use the below Technique which is IQR
Data which are greater than IQR +1.5 IQR and data which are below than IQR - 1.5 IQR are my outliers
where ,  IQR = 75th%ile data - 25th%ile data

& IQR +- 1.5 IQR  will be changed depending upon the domain ie it could be sometimes IQR +- 3IQR 

__Feature Selection 

Mutual info: if the MI between 2 features is 0 it means that they don't correlate

__Hyperparameter Tuning/ Optimization

1.Choose following method for hyperparameter tuning
    a.RandomizedSearchCV --> Fast way to Hypertune model
    b.GridSearchCV--> Slower way to hypertune my model
2.Choose ML algo that u have to hypertune
2.Assign hyperparameters in form of dictionary or create hyper-parameter space
3.define searching &  apply searching on Training data or  Fit the CV model 
4.Check best parameters and best score


