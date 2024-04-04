# MicroMobility Service Provider - Hypothesis Testing

<div align="center">
  <img src="https://github.com/yashika-malhotra/MicroMobility-Service-Provider---Hypothesis-Testing/assets/154385962/03ccdd43-3a2a-47e2-a5c8-96f179930cf6" width = 200 height =150/>
  <img src="https://github.com/yashika-malhotra/MicroMobility-Service-Provider---Hypothesis-Testing/assets/154385962/c580cabc-efb5-45a1-a0d0-7625d2c77fed" width = 200 height =150/>
  <img src="https://github.com/yashika-malhotra/MicroMobility-Service-Provider---Hypothesis-Testing/assets/154385962/d9dbc2de-b2ef-4ad7-bb00-356526fe4712" width = 200 height =150/>
</div>

## 📚 About Data
Yulu is India’s leading micro-mobility service provider, which offers unique vehicles for the daily commute. Starting off as a mission to eliminate traffic congestion in India, Yulu provides the safest commute solution through a user-friendly mobile app to enable shared, solo and sustainable commuting.

Yulu zones are located at all the appropriate locations (including metro stations, bus stands, office spaces, residential areas, corporate offices, etc) to make those first and last miles smooth, affordable, and convenient!

Yulu has recently suffered considerable dips in its revenues. They have contracted a consulting company to understand the factors on which the demand for these shared electric cycles depends. Specifically, they want to understand the factors affecting the demand for these shared electric cycles in the Indian market.

## 🎯 Objective
The company wants to know:

Which variables are significant in predicting the demand for shared electric cycles in the Indian market?
How well those variables describe the electric cycle demands

## MicroMobility Service Provider Data: Cleaning, Analysis and Visualization
Data Analysis and Visualization on Walmart Data to provide insights and recommendations to improve their userbase.

Column | Description | 
|:--------|:------------|
|datetime| datetime |  
|season| season (1: spring, 2: summer, 3: fall, 4: winter)|
|holiday| whether day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)|
|workingday| if day is neither weekend nor holiday is 1, otherwise is 0.|
|temp| temperature in Celsius|
|atemp| feeling temperature in Celsius|
|humidity| humidity|
|windspeed| wind speed|
|casual| count of casual users|
|registered| count of registered users|
|count - Total_riders| count of total rental bikes including both casual and registered|

- weather

|Category|Details|
|:------|:--------|
|1| Clear, Few clouds, partly cloudy, partly cloudy|
|2| Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist|
|3| Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds|
|4| Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog|


## Performed following Tasks
1. Data Cleaning
2. Exploratory Data Analysis
3. Visualization
4. Hypothesis Testing
   
- Observations on the shape of data, data types of all the attributes, conversion of categorical attributes to 'category', missing value detection, statistical summary

- Non-Graphical Analysis: Value counts and unique attributes ​
- Visual Analysis after pre-processing of the data -
  * Univariate (distribution plots of all the continuous variable(s) barplots/countplots of all the categorical variables),
  * Bivariate (Relationships between important variables such as workday and count, season and count, weather and count)
    
- For continuous variable(s): Distplot, countplot, histogram for univariate analysis 
- For categorical variable(s): Boxplot 
- For correlation: Heatmaps, Pairplots 
- Missing Value & Outlier check

- Explored relation between the dependent and independent variable (Dependent “Count” & Independent: Workingday, Weather, Season etc)
- Performed approriate testing on all of the below mentioned questions: 
  * Working Day has effect on number of electric cycles rented
  * No. of cycles rented similar or different in different seasons
  * No. of cycles rented similar or different in different weather
  * Weather is dependent on season (check between 2 predictor variable)

- Performed Hypothesis Testing: 
  * Set up Null Hypothesis (H0)
  * State the alternate hypothesis (H1)
  * 2- Sample T-Test to check if Working Day has an effect on the number of electric cycles rented 
  * ANNOVA to check if No. of cycles rented is similar or different in different 1. weather 2. season 
  * Chi-square test to check if Weather is dependent on the season

- Checked assumptions of the test (Normality, Equal Variance) using Histogram, Q-Q plot or statistical methods like levene’s test, Shapiro-wilk test 
- Calculate test Statistics

- Insights - based on EDA (Exploratory Data Analysis) 
  * Visual analysis 
  * Hypothesis formulation 
  * Selection of the appropriate test 
  * Checked test assumptions 
  * Find the p-value
  * Conclusion based on the p-value 

- Business Insights & Recommendations : Includes patterns observed in the data along with what can infer from it. 

### Description about files in repository <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Hand%20gestures/Backhand%20Index%20Pointing%20Down%20Light%20Skin%20Tone.png" alt="Backhand Index Pointing Down Light Skin Tone" width="30" height="30" />:


**Yulu - Hypothesis Testing Business Case Study.ipynb** - Colaboratory notebook containing the code for analysis
