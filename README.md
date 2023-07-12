# Encode_Scale_Transform
Detailed Practice of Scaling, Encoding and Transforming the dataframe

Dummies,Onehotencoder and ordinal takes multiple labels at a time

label encoder are mostly used in target varaiable it can take only one label at a time

Frequency encoding -- replaces the labels with the percentage of subclasses present in the nominal categorical feature with respect to target variable

Feature encoding creates same percentage if there is same proportion of labels present in the encoding column.This will make confusion to encode different labels 

Target Encoding -- 
Is used in case of categorical target variable it is also called as mean ,Each value in the independent varibale (categorical nominal variable ) is replace by mean of the target variable for its respective subclass

Frequency of occurance- Histplot
probablity of occurance of each of the value -- Density -- Distplot

Z-Score
By normal distibution we can only mark each variable based on the data Ex:age
So Standard deviation,We create z-score by (forumal data-mean)/standard_deviation

they plot with x-axis as Z-score and mean will always be zero and Standard deviation will be one 

Types of scaling:

Standard scaler uses a standard normal distribution formula,It gets affected the outlier
MinMaxScaler is also a scaling techinc where the result ranges between 0 to 1,We will Not to be able to find the outlier. MinMaxScaler subtracts the minimum value in the feature and then divides by the range. The range is the difference between the original maximum and original minimum.

https://towardsdatascience.com/scale-standardize-or-normalize-with-scikit-learn-6ccc7d176a02

Transformation is a techinic using which the distributioin of the data is made into near normal distrubtion
There are differnet transformation technic
log transformation changes each value of the variable into its corresponding log value.log transformation canot be used for a variable which has zero and negative values.Since the value of zero and negative values are undefined.

Power Transformer: There are 2 types
Box-cox[Can't be used with 0 and -1] lambda
Yeo-Johnson 

first do transformer and then do scaler

Feature scaling is the process of normalizing the range of features in a dataset.

https://towardsdatascience.com/what-is-feature-scaling-why-is-it-important-in-machine-learning-2854ae877048

Real-world datasets often contain features that are varying in degrees of magnitude, range, and units. Therefore, in order for machine learning models to interpret these features on the same scale, we need to perform feature scaling.

Two methods to find the ouliers are Z-Score and IQR(inter-Quartile Range)
