# Data driven insights of Seattle AirBnB listings data

This project was done as a part of Udacity Data Scientist Nanodegree.

### Table of Contents
1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Data](#data)
4. [Running the code](#running)
5. [Results](#results)
6. [Acknowledgements](#acknowledgements)

### Introduction<a name="introduction"></a>
In this repository, I shall be analyzing AirBnB listings data of Seattle from January, 2016 to January, 2017. The aim of this 
project is to perform analyses on AirBnB data and answer the following questions which I constructed after initial assessment of the data:

1. What factors highly influence the prices of listings in Seattle?
2. What is the seasonal pattern of prices?
3. What is the relationship of reviews with price?

This project follows CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology. It consists of business understanding to evaluation.
Steps followed in this project:
- **Business objective:** Analyze factors that influence prices, understand seasonal trends for demand of listings, and examine impact of reviews.
- **Data Processing:** Applied certain data cleaning and transformation techniques, handled missing data, removed the outliers, lemmatization, etc.
- **Modeling:** Observed different distributions of interesting fields in data used them to conclude what aggregate method will be most appropriate.
- **Evaluation/Visualization:** Visualized the analyses and obtained answers to the questions devised above.

### Prerequisites<a name="prerequisites"></a>
- Pandas (for data loading and analysis)
- NumPy (for computing)
- Matplotlib (for visualizations)
- Seaborn (for visualizations)
- NLTK (Natural Language Toolkit for analysis of descriptions and reviews)
- Wordcloud (displaying wordclouds)
- Langdetect (analysis of reviews)
- Jupyter (to run notebooks)

### Data<a name="data"></a>
There are three files in the dataset.
- listings.csv - includes full descriptions and average review score
- calendar.csv - includes listing id and the price and availability for that day
- reviews.csv - includes unique id for each reviewer and detailed comments
We'll be using all three files individually for analysis.

### Running the code<a name="running"></a>

There are three files - one each for analysis of individual data files.
- [`FactorsAffectingPrices.ipynb`](https://github.com/chaitanyakasaraneni/seattle_airbnb_dataAnalysis/blob/master/code/FactorsAffectingPrices.ipynb) 
contains the analysis of factors that influence prices of a listing. [`listings.csv`](https://github.com/chaitanyakasaraneni/seattle_airbnb_dataAnalysis/blob/master/data/listings.csv) data is used for this part.
- [`SeasonalPatternofPrices.ipynb`](https://github.com/chaitanyakasaraneni/seattle_airbnb_dataAnalysis/blob/master/code/SeasonalPatternofPrices.ipynb)
contains seasonal pattern analysis of prices. [`calendar.csv`](https://github.com/chaitanyakasaraneni/seattle_airbnb_dataAnalysis/blob/master/data/calendar.csv) data is used for this part.
- [`ReviewRelationtoPrices.ipynb`](https://github.com/chaitanyakasaraneni/seattle_airbnb_dataAnalysis/blob/master/code/ReviewRelationtoPrices.ipynb) 
contains analysis of relationship between reviews by other customers and prices. [`reviews.csv`](https://github.com/chaitanyakasaraneni/seattle_airbnb_dataAnalysis/blob/master/data/reviews.csv) data is used for this part.

### Results<a name="results"></a>
- Factors affecting prices
  - The type of room chosen by the traveller and mostly booking an Entire property costs maximum followed by private room and shared apartment.
  - Price of a listing also depends upon the number of bedrooms the property have and the same also depends upon the neighborhood of the property
- Seasonal pattern analysis of prices
  - Summer months, specifically July and August are the peak times to visit Seattle with the highest of $156.5 
- Analysis of relationship between reviews
  - The words "great host", "clean", "comfortable" and "highly recommended" are most used.
  All these reviews and comments plays a big role in attracting the attention of travellers and if there are comments such as "highly recommended" then traveller surely takes a look at the listing.
  
### Acknowledgements<a name="acknowledgements"></a>
- This dataset is only a small part of AirBnB inside. Original can be found [here](http://insideairbnb.com/get-the-data.html)
