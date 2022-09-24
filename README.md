# Ex03-Univariate-Analysis
## Aim:
To read the given data and perform the univariate analysis with different types of plots.

## Explanation:
Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## ALGORITHM:
## Step1
Read the given data.
## Step2
Get the information about the data.
## Step3
Remove the null values from the data.
## Step4
Mention the datatypes from the data.
## Step5
Count the values from the data.
## Step6
Do plots like boxplots,countplot,distribution plot,histogram plot.

## PROGRAM:
Developed by : RAGUL M
Registration Number : 212221230080
~~~
import pandas as pd
import numpy as np
import seaborn as sns

df=pd.read_csv('superstore.csv')
df

df.head()
df.info()
df.describe()
df.isnull().sum()
1
df.dtypes

df['Postal Code'].value_counts()

sns.boxplot(x='Postal Code', data=df)
sns.countplot(x='Postal Code',data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x='Postal Code',data=df)
~~~
## OUTPUT:
## DATA
![output](https://github.com/ragulmani936/Ex03-Univariate-Analysis/blob/main/image1.jpg) 

## DATA HEAD
![output](https://github.com/ragulmani936/Ex03-Univariate-Analysis/blob/main/image2.jpg)

## DATA INFORMATION
![output](https://github.com/ragulmani936/Ex03-Univariate-Analysis/blob/main/image3.jpg)

## DATA DESCRIBE
![output](https://github.com/ragulmani936/Ex03-Univariate-Analysis/blob/main/image4.jpg)

## DATA NULL VALUES
![output](https://github.com/ragulmani936/Ex03-Univariate-Analysis/blob/main/image5.jpg)

## DATA'S DATATYPES
![output](https://github.com/ragulmani936/Ex03-Univariate-Analysis/blob/main/image6.jpg)

## DATA'S VALUECOUNT
![output](https://github.com/ragulmani936/Ex03-Univariate-Analysis/blob/main/image7.jpg)

## BOXPLOT
![output](https://github.com/ragulmani936/Ex03-Univariate-Analysis/blob/main/image8.jpg)

## COUNTPLOT
![output](https://github.com/ragulmani936/Ex03-Univariate-Analysis/blob/main/image9.jpg)

## DISTRIBUTION PLOT
![output](https://github.com/ragulmani936/Ex03-Univariate-Analysis/blob/main/image10.jpg)
## HISTOGRAM PLOT
![output](https://github.com/ragulmani936/Ex03-Univariate-Analysis/blob/main/image11.jpg)

## RESULT:
Thus we have read the given data and performed the univariate analysis with different types of plots.
