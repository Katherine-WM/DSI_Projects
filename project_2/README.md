## Project 2: Ames Housing Price Prediction

### Problem Statement
There are over 80 features associated with a house which can possibly affect how much it is worth for. This means that there are as many areas which a real estate company should pay attention to when developing their projects. However, some features are naturally worth more as compared to others. By including these featuers, companies can expect a boost in their SalePrice.

As a consultant in real estate company in City of Ames, my job is to uncover what are the top 25 features contributing to a high property saleprice and to what extend is each individual factor affecting the final SalePrice. In this way, my stakeholders can make the right decision both in investing and developing the right property to boost company revenue.

### Flow of This Analysis
Detailed data on computing assessed values for individual residential propoerties sold in Ames from 2006 to 2010 is made avaible for this project. There are 2051 observations and 81 variables of which 80 are features of a house and 1 is SalePrice (our target variable). This analysis will start with exploratory data analysis to observe the pattern relationship among features. The following section will detail the process and result of features selected for this analysis, after which we will build the correct model which minimizes errors in our prediction to prove feasibility of our model. Lastly, it will end with recommendations of top 30 features which real estate companies should look out for and how much impact each of them have on SalePrice of a house.

### Contents:
Exploratory Data Analysis
- Deal with Missing Values
- Distribution of Target Variable
Feature Selection and Feature Engineering
Round 2 Feature Selection
Data Modeling
- Linear Regression
- LassoCV and Lasso
- RidgeCV and Ridge
Conclusion

### Data Dictionary
Here is the list of features in this data set.

|Feature             |Type |Dataset                             |Description
|:------------------  |:----|:-----------------------------------|:-------------------------------------------------------
|Gr Liv Area         |int64|Final Cleaned Training Data.csv|Above grade (ground) living area in sqft (Range: 334sqft - 5642sqft)
|Overall Score       |int64|Final Cleaned Training Data.csv|Overall score of a houe (Range: 1-25)
|house_age           |int64|Final Cleaned Training Data.csv|Years since house is built (Range: 0yrs - 136yrs)
|Fireplaces          |uint8|Final Cleaned Training Data.csv|Having fireplaces in house (tes/no)
|MS Zoning_RL        |uint8|Final Cleaned Training Data.csv|Residential Low Density (yes/no)
|MS Zoning_RM        |uint8|Final Cleaned Training Data.csv|Residential Medium Density (yes/no)
|MS Zoning_RH        |uint8|Final Cleaned Training Data.csv|Residential High Density (yes/no)
|MS Zoning_FV        |uint8|Final Cleaned Training Data.csv|Floating Village Residential (yes/no)
|MS Zoning_C (all)   |uint8|Final Cleaned Training Data.csv|Commercial Residential (yes/no)
|Bsmt Exposure_Gd    |uint8|Final Cleaned Training Data.csv|Good basement exposure (yes/no)
|Mas Vnr Type_None   |uint8|Final Cleaned Training Data.csv|Masonry veneer type is none (yes/no)
|Mas Vnr Type_Stone  |uint8|Final Cleaned Training Data.csv|Masonry veneer type is stone (yes/no)
|Exter Qual_Fa       |uint8|Final Cleaned Training Data.csv|Fair material on the exterior (yes/no)
|Exter Qual_Gd       |uint8|Final Cleaned Training Data.csv|Good material on the exterior (yes/no)
|Exter Qual_TA       |uint8|Final Cleaned Training Data.csv|Average material on the exterior (yes/no)
|Foundation_not PConc|uint8|Final Cleaned Training Data.csv|Not PConc Type of foundation (yes/no)
|Bsmt Qual_TA        |uint8|Final Cleaned Training Data.csv|Average basement quality (yes/no)
|Bsmt Qual_Gd        |uint8|Final Cleaned Training Data.csv|Good basement quality (yes/no)
|Kitchen Qual_Fa     |uint8|Final Cleaned Training Data.csv|Fair quality kitchen (yes/no)
|Kitchen Qual_Gd     |uint8|Final Cleaned Training Data.csv|Good quality kitchen (yes/no)
|Kitchen Qual_TA     |uint8|Final Cleaned Training Data.csv|Average quality kitchen (yes/no)
|Total Bsmt SF       |float|Final Cleaned Training Data.csv|Total basement area in sqft (Range: any positive value)
|Mas Vnr Area        |float|Final Cleaned Training Data.csv|Masonry veneer area in square feet (Range: 0sqft - 1600sqft)
|Garage Area         |float|Final Cleaned Training Data.csv|Size of garage in square feet (Range: 0sqft - 1418sqft)
|Lot Area            |float|Final Cleaned Training Data.csv|Lot size in square feet (Range: 1300sqft - 159000sqft)


### Conclusions and Recommendations
After thorough analysis of the avaiable data, both models helped us identify 25 most impactful features according to their analysis but they differ by 8 features. Two models we have gave us difference selection of features. Though two models both give us the correct selection, however, from a real estate company point of view, we focus more on the bigger picture such as location of the house rather than which type of finish the basement uses. Therefore, my recommendation to stakeholders are based on Ridge Regression model.

Some recommendations to boost saleprice:

we want to increase size and number of the following attibutes:
Ground living area, basement, Mas Veneer Area, garage, lot area, fireplaces.
we want to develop/invest houses in the following area:
medium residential density area, floating village area, high residential density area, commercial area
we want better quality in the following attributes:
overall condition/quality, basement exposure, exterior condition/quality, use PCone for house foundation, kitchen quality
we want to invest in newer houses rather than the old ones.
It is proven from our model that by implementing the aboved suggestions, average saleprice will increase.