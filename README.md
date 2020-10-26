# Capstone_project
## 1. Introduction
For the final capstone project in the IBM certificate course, we want to analyze the accident “severity” in terms of human fatality, traffic delay, property damage, or any other type of accident bad impact. The data was collected by Seattle SPOT Traffic Management Division and provided by Coursera via a link. This dataset is updated weekly and is from 2004 to present. It contains information such as severity code, address type, location, collision type, weather, road condition, speeding, among others.
The world as a whole suffers due to car accidents, including the USA. National Highway Traffic Safety Administration of the USA suggests that the economical and societal harm from car accidents can cost up to *$871 billion* in a single year. According to 2017 WSDOT data, a car accident occurs every 4 minutes and a person dies due to a car crash every 20 hours in the state of Washington while Fatal crashes went from *508* in 2016 to *525* in 2017, resulting in the death of *555* people. The project aims to predict how severity of accidents can be reduced based on a few factors.
## 2. Data
There are 194,673 observations and 38 variables in this data set. Since we would like to identify the factors that cause the accident and the level of severity, we will use SEVERITYCODE as our dependent variable Y, and try different combinations of independent variables X to get the result.
The dataset used for this project is based on car accidents which have taken place within the city of *Seattle, Washington* from the year *2004* to *2020*. This data is regarding the *severity of each car accidents* along with the time and conditions under which each accident occurred. The data set used for this project can be found **<a href="https://s3.us.cloud-object-storage.appdomain.cloud/cf-courses-data/CognitiveClass/DP0701EN/version-2/Data-Collisions.csv">here!</a>**. 
## 3. Objective
Luckily enough, The Seattle Police Department (SPD) has recorded all car collision accident from 2004 to present. Basing on those historical data (194,673 records), we can create a map and information chart to help us understand the high-risk areas, understand car injury factors to avoid accident, and plan our next trip to Seattle better.
## 4. Datasource
The datasource is: 
http://data-seattlecitygis.opendata.arcgis.com/datasets/5b5c745e0f1f48e7a53acec63a0022ab_0.csv
## 5. Methodology
We used Jupyter Notebook to do the data analysis. To generate the table and graph for the dataset, we imported Python libraries (Pandas, Numpy, Matplotlib, and Seaborn).
First we imported the data through pd.read_csv. We noticed that it had 194,673 rows and 38 columns. Therefore, we narrowed it down to 8 columns (‘Severity’, ‘X’, ‘Y’, ‘Location’, 'Vehcount’, ‘Weather’, ‘Roadcond’, ‘Lighdcond’) and delete the missing values, which made the final dataset with 184,167 observations and 8 variables.
Since most of the variable were categorical, it was hard to make the regression model. So, in this study, we focused more on the graphical data and the value count for different categories. There were around 135,000 (2/3) level 1 accidents and 60,000 (1/3) level 2 accidents.
<p align="center"><img src="https://github.com/alsheabi/Capstone_project/blob/main/count.png" width="700"/></p>
## 6. Requirements
`notebook==6.0.3`  
`sklearn==0.23.1`  
`pandas==1.0.1`  
`numpy==1.18.1`  
`scipy==1.4.1`  
`matplotlib==3.1.3`  
`seaborn==0.11.0`  
`imblearn==0.7.0`
