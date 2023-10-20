
# Pandas_Profiling

Pandas-profiling is an open-source Python library that generates profile reports from a pandas DataFrame. The profiling report is like an "overview" of the dataset, telling you about the types of data, missing data, and other various statistics which can be useful when doing preliminary analysis of the dataset.

Here's what pandas-profiling typically provides:-
* Essentials: Type, unique values, missing values
* Quantile statistics like minimum value, Q1, median, Q3, maximum, range, interquartile range
* Descriptive statistics like mean, mode, standard deviation, sum, median absolute deviation, coefficient of variation, kurtosis, skewness
* Most frequent values
* Histogram
* Correlations highlighting highly correlated variables, Spearman, Pearson and Kendall matrices


### Code: 
*#Importing all the necessary libraries and packages*  
pip install pandas pandas-profiling  
import pandas as pd  
from pandas_profiling import ProfileReport  

*#Reading the CSV file*  
file_path = "csvfile.csv"  
df = pd.read_csv(file_path)  

*#Generating the profiling report*  
profile = ProfileReport(df, title="Pandas Profiling Report", explorative=True)  

*#Saving the report to an HTML file*  
output_path = "output_report.html"  
profile.to_file(output_path)  


![Pandas_Profiling](https://github.com/dheerajsk26/Pandas_Profiling/assets/77773902/cba51e0d-a33f-4a09-a032-3df31fbd081c)

