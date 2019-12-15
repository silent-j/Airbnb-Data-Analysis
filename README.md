# Regression-Analysis-of-AirBnB-Prices-in-Spain

This repository is for the Udacity Data Science Nanodegree. In the seventh project, Write a Data Science Blog Post, you are tasked with writing a Data Science blogpost on a subject of your choosing. The main purpose of this proejct is to showcase the CRISP-DM (cross-industry process for data mining). I went with one of the suggested topics of answering business questions AirBnB. This repository contains the datasets used, and the jupyter notebook containing exploratory data analysis, data cleaning, and modelling. 

This repository contains dataset.zip. This zipped archive contains 6 csv files. These files were downloaded from insideAirBnB.com on September 18, 2019.

The first 3 are datasets containing detailed information about AirBnB listings in each Spanish city. Rows correspond to an individual listing, and columns are a feature about the listed property.
  barcelona_list.csv
  madrid_list.csv
  valencia_list.csv
 
The last 3 are datasets containing date, availabiity and price informaiton for AirBnB listings in each Spanish city. Rows correspond to a property's listing id, and a date within the next 12 months (September 2019 to October 2020). 

  barcelona_cal.csv
  madrid_cal.csv
  valencia_cal.csv

Main Libraries used in this proejct are:

  Pandas - for easy dataset exploration, processing, and transformations
  Numpy - for regular mathematical operations
  Scikit-Learn - for feature engineering and Linear Regression modelling. In this repository, I explore RandomForest & GradientBoosting Regression
  Seaborn and Matplotlib - for data visualization

Datasets have been provided by insideairbnb.com
The blog post can be found on Medium.com here: https://medium.com/@james23mcdermott/hablas-airbnb-a2d2116a08c4

For this project, I sought out to answer the following questions about the AirBnB data for Barcelona, Madrid, and Valencia:

1. How does pricing compare among all 3 cities throughout the year? 

2. How does the distribution of prices for each city differ from one another?

3. Where might we find the most expensive listings in each city?

4. What features of an AirBnB listing influence price for major cities in Spain?

My findings, in brief:

1. All 3 cities experience rising listing prices at the end of March/beginning of April. Barcelona experiences the highest surge in prices, followed my Madrid. Valencia remains consistently low for the next 12 months.

2. Barcelona and Madrid, with greater numbers of AirBnB listings, experience 20 - 30% of listings priced at over $100 per night. A majority of listings (75% for Barcelona and 78% for Madrid) are priced below this threshold. In Valencia, nearly 50% of all listings are priced below $50 a night. 

3. Barcelona and Madrid have large clusters of expensive neighbourhoods. In Barcelona, these expensive neighbourhoods (determined by the average price per hood) are mainly clustered near the waterfront and the historic centre of the city, with the highest priced listings being furhter out of the city near the mountains. In Madrid, highly priced neighbourhoods are found on the perimeters of the city core. Valencia features highly priced listings along the waterfront - similar to Barcelona. However there are significantly less higher priced areas than the other two cities.

4. After performing a linear regression with GradientBoosting, 70% of the variance in predicted prices and true values was explained using the 'accommodates' feature. Other notably important features in this model are number of bedrooms per listing, bathrooms, cleaning fees, and whether the listing exists in Barcelona or Valencia (Barcelona likely influencing the price positively, and Valencia negatively). Other features to be considered when discussing what influences price include how many other listings a host is running, or whether the listing is for a private room vs an entire apartment/home.

  
