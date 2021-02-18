Exploratory Data Analysis for Machine Learning


DATA DESCRIPTION:

Dataset I used was obtained from Kaggle, it contains data from car sales with actual prices they were sold and the market price and also the description of individual car like type of the car, model, miles per gallon and more. Here is the link of the data source: https://www.kaggle.com/ljanjughazyan/cars1
The dataset consists of 15 columns and 428 entries, from which 8 are numeric and 7 are categorical, 2 entries have 2 values.


INITIAL PLANFOR DATA EXPLORATION:

I will detect null values and then try to deal with them. MSRP and Invoice columns are strings and have special characters so must delete them first in order to convert the columns into numeric.
I am going to detect and drop unique values and drop them because they will not help my initial model. 
I am going to create a data frame with o the significant statistical values.
I will detect values values and make them categorical.
Perform the skew transformation.
target variable invoice separate feature and target variables, for polynomial transformation in order to prepare the data for linear regression machine learning analysis.
I will formulate 3 hypothesis  about this data and conduct a formal significance test.
After every transformation I will try to make some visual representation of the result to get insight.


ACTIONS TAKEN

Found 2 null values, which were under the column Cylinders for the car Model RX-8, after search found out that that car has no cylinders and dropped the 2 rows.
MSRP and Invoice are objects. I am transforming them into numeric values. To do so first i have to get rid of special characters like $ and  , and then transformed them. 
Added Range and median in the stats.
And made visual representation of most significant attributes for my model using scatter and hist plots, with the help of python library matplolib.
Detected some outliers in Invoice that were above 90000 and deleted them. Also deleted rows from columns Cylinders with values of 3,5,10,12, because again they were outliers, and would damage my model.
Made a new categorical which will take  values from EngineSize, and group them by the size from 1-2, 2-3, 3-4, 4-5, 6-7. And then transform the new column into string. 
Get all the sting values and make categorical values to dummies
Checked for skewness. Tha data has right skewness, so I will apply log1p from numpy and visualize the result with matplotlib and then with the help of seaborn with pairplot, to be able to compare all the values. 
Separate feature and target variables, target variable in my case is Invoice.
Then transformed all the features into second degree polynomial.
Next Steps

Have to be done more hypothesis tests in the future to come up with more insights.
I must compare more features to get more results.
And finally I want to apply some machine learning algorithms.

SUMMERIZE

The dataset I worked on had a few null values and outliers. After some feature engineering that I did, is ready to apply machine learning algorithms.
The data set had not a lot of entries, near 400, I have to try to find same dataset with more entries, in order to get better insight from the data, and get better results from machine learning 
