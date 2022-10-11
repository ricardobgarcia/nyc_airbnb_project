# nyc_airbnb_project

This is a Data Science project aimed at deriving insights from data analysis to solve business problems. This project was inspired by the DS course of the Comunidade DS https://www.comunidadedatascience.com/.

## 1. Business problem 
The NY Real Estate Company is a fictious company located in New York City. The company is focused on buying apartments for renting the apartment or private rooms in booking sites like airbnb.

The Company currently have 200 properties in Manhattan and the strategic plan is to increase the portfolio up to 400 properties, including properties outside but near Manhattan.

The business problem is finding properties with high potential profitability in Manhattan and surrounding neighbourhoods outside Manhattan. To estimate the profitability of a property, the following formula is used by the business team:

$$ profitability = \frac{price * (minimum\\_nights + 1) * number\\_of\\_reviews}{\sqrt{availability\\_365}} $$

The Data Scientist was requested to:
- Analyze the airbnb dataset in search of the best properties for buying in the target neighbourhoods. 
- Use exploratory data analysis for understanding the location distribution, the price and popularity (rate of reviews) patterns in different boroughs and neighbourhoods of NYC.
- Plot maps for visualizing the location of properties in NYC boroughs and neighbourhoods, as well as for visualizing the median prices and number of reviews per neighbourhood.
- Analyze and compare price patterns in different regions of Manhattan (Lower, Mid, Central Park, Upper)
- Analyze prices around the Central Park

**The dataset:** https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data

## 2. Assumptions

- The NY Company is focused on properties with rental price from US\$ 20.00 to US\$ 500.00, of the types 'entire appartment' and 'private room'.
- The `AB_NYC_2019.csv` is the portfolio of properties listed in the market

## 3. Solution strategy
This project was developed following these steps:<br>
- ETL: the dataset was extracted, the data consistency was analyzed and the appropriate transformations were made, including those imposed by the project’s assumptions.<br>
- EDA: exploratory analyses revealed the distribution of properties in NYC, the median price, profitability and popularity (reviews) per neighbourhoods.   
- Insights: some hypotheses with actionable business implications were evaluated.<br>
- Algorithm: an algorithm was developed for selecting best properties for buying - those with reviews per month rate above the median, availability and profitability in the 4th quartile.   
- Evaluation: the business/financial implications and the characteristics of the resulting portfolio were evaluated.<br> 

This repository contains the jupyter notebook of this project.

## 4. Main insights
- The listings are mainly located in Manhattan or near Manhattan in Brooklyn and Queens.
- The most popular neighborhoods are in Manhattan, or outside but near Manhattan in Brooklyn and Queens.
- The most expensive and profitable neighborhoods are in Lower Manhattan, Mid Manhattan, Central Park Manhattan, and Brooklyn near Manhattan.
- There is little price variation near and around the Central Park.
- In Manhattan, the most reviewed listings are 11% cheaper than the least reviewed.
- In Manhattan, the most popular listings (high rate of reviews per month) are 5.3% more expensive than the least popular. 


## 5. Business/Financial implications

- The median profitability of the selected properties is 396.6% higher than the target sample
- The median reviews per month of the selected properties is 105.5% higher than the target sample
- The median number of reviews of the selected properties is 710% higher than the target sample
- The median availability of the selected properties is 108.1% higher than the target sample

## 6. Concluding remarks
This project aimed at deriving insights from data analysis to solve the business problem of selecting the best properties available for renting in the Airbnb portfolio. The exploratory data analysis and the verification of hypotheses helped to understand patterns of price, profitability, and popularity (reviews) in NYC boroughs and neighbourhoods.

- The solution produced a diversified portfolio of properties with buy recommendation.
- The solution identified the properties with reviews per month above the median, availability in the 4th quartile and profitability in the 4th quartile.
- The most profitable properties are mainly located in Manhattan and Brooklyn near Manhattan, and few were located in Queens and only one in Bronx.
- Based on the selected properties, the business team may contact hosts and negociate acquisitions.

## 7. Next steps

- Identify NYC main attractions and their locations.
- For each property, indicate the main attractions within a 1 mile distance.
- Identify NYC subway stations and indicate the nearest stations for each property.

## 8. Lessons learned

- To address business problems using data analysis for deriving actionable insights. <br>
- To use geopandas for plotting geospatial information and maps. <br>

