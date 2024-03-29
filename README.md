# **Key to happiness**

## Table of contents

1. Objective
2. Introduction
3. File descriptions and Index of Repositories
4. Tasks
5. Analysis Process
6. Findings
7. Data Sources

## Objective

To understand on a data-driven level the factors contributing to and correlating with World Happiness. We will examine the relationships between several metrics of individual countries or regions and their happiness scores or ranks to determine their influences and effects.


## Introduction

In this project, we utilized the World Happiness Report dataset at Kaggle.com to perform an analysis of different factors contributing to, detracting from or  correlating with world happiness We also use variables from other datasets to predict happiness scores for countries and compare with the stats.

We decided on utilizing five attributes of interest when creating the classification models using the mean of the happiness score as the main Variable:

1. Healthcare
2. Social Support
3. Unemployment
4. Type Governments
5. Weather


## Files Description and index of Repository

With this project, there are six main Jupyter notebooks regarding the data exploration and one for visualizations.
  
 * [Government](https://github.com/reginesgit/project1/tree/main/Government) (Folder):
   * [Gov:](https://github.com/reginesgit/project1/blob/main/Government/Gov.ipynb)jupyter notebook used to clean and merge original datasets from ave\_Happiness and DataBase\_of Political\_Institutions
    - [Resources (Folder)](https://github.com/reginesgit/project1/tree/main/Government/Resources)

    - [Database\_of\_Political\_Institutions\_2017.csv](https://github.com/reginesgit/project1/blob/main/Government/Resources/Database_of_Political_Institutions_2017.csv) - Original Dataset from the World Bank
    - [cleaned\_gov\_file.csv](https://github.com/reginesgit/project1/blob/main/Government/Resources/cleaned_gov_file.csv)Cleaned Version of the DPI
    - [merge\_happiness\_gov.csv](https://github.com/reginesgit/project1/blob/main/Government/Resources/merge_happiness_gov.csv)file containing records that are in both the happiness and the DPI

- [Unemployment](https://github.com/reginesgit/project1/tree/main/Unemployment) (Folder):

    - [Unemployment\_Data](https://github.com/reginesgit/project1/blob/main/Unemployment/Unemployment_Data%20-%20Cleaning%20and%20Initial%20Analysis.ipynb) - Cleaning and Initial Analysis : jupyter notebook used to clean original dataset from The World Economic Outlook (WEO) Database and merge resulting data with the unemployment dataset
    - [Unemployment\_Visuals](https://github.com/reginesgit/project1/blob/main/Unemployment/Unemployment_Visuals.ipynb): jupyter notebook used to check for outliers and create visuals for trends within and correlations between happiness and unemployment
    - [Resources](https://github.com/reginesgit/project1/tree/main/Unemployment/Resources) (Folder):

        - [Unemployment\_raw.csv](https://github.com/reginesgit/project1/blob/main/Unemployment/Resources/Unemployment_raw.csv) - original dataset from The World Economic Outlook (WEO) Database
        - [happiness\_unemployment\_summary.csv](https://github.com/reginesgit/project1/blob/main/Unemployment/Resources/happiness_unemployment_summary.csv) - file containing records that are in both the happiness and unemployment datasets; only contains &#39;Country&#39;, &#39;Avg. Happiness&#39;, and &#39;Avg. Unemployment Rate&#39; columns.
        - [happiness\_unemployment\_yearly.csv](https://github.com/reginesgit/project1/blob/main/Unemployment/Resources/happiness_unemployment_yearly.csv) - file containing records that are in both the happiness and unemployment datasets
        - [unemployment\_complete\_df.csv](https://github.com/reginesgit/project1/blob/main/Unemployment/Resources/unemployment_complete_df.csv) - cleaned version of the unemployment dataset

- [Happiness](https://github.com/reginesgit/project1/tree/main/Happiness) (Folder):

    - [Happiness\_Beginning](https://github.com/reginesgit/project1/blob/main/Happiness/Happiness_Beginning.ipynb): jupyter notebook used to clean and merge original datasets from Kaggle
    - [Happiness\_Visual\_Analysis](https://github.com/reginesgit/project1/blob/main/Happiness/Happiness_Visual_Analysis.ipynb): jupyter notebook used to visualize trends within the happiness data using the cleaned dataset
    - [Resources (Folder](https://github.com/reginesgit/project1/tree/main/Happiness/Resources)):

        - [2015.csv](https://github.com/reginesgit/project1/blob/main/Happiness/Resources/2015.csv) - Happiness rank and scores by country, 2015 (raw data)
        - [2016.csv](https://github.com/reginesgit/project1/blob/main/Happiness/Resources/2016.csv) - Happiness rank and scores by country, 2016 (raw data)
        - [2017.csv](https://github.com/reginesgit/project1/blob/main/Happiness/Resources/2017.csv) - Happiness rank and scores by country, 2017 (raw data)
        - [2018.csv](https://github.com/reginesgit/project1/blob/main/Happiness/Resources/2018.csv) - Happiness rank and scores by country, 2018 (raw data)
        - [2019.csv](https://github.com/reginesgit/project1/blob/main/Happiness/Resources/2019.csv) - Happiness rank and scores by country, 2019 (raw data)
        - [avg\_happiness.csv](https://github.com/reginesgit/project1/blob/main/Happiness/Resources/avg_happiness.csv) - cleaned and merged version of the happiness data, including an average happiness column; only includes happiness scores for every year
        - [happiness\_bottom10.csv](https://github.com/reginesgit/project1/blob/main/Happiness/Resources/happiness_bottom10.csv) - happiness data for the 10 countries with the lowest average happiness score
        - [happiness\_top10.csv](https://github.com/reginesgit/project1/blob/main/Happiness/Resources/happiness_top10.csv) - happiness data for the 10 countries with the highest average happiness score
        - [merged\_happiness\_data.csv](https://github.com/reginesgit/project1/blob/main/Happiness/Resources/merged_happiness_data.csv) - cleaned and merged version of the happiness data; includes all columns
        - [country\_region.csv](https://github.com/reginesgit/project1/blob/main/Happiness/Resources/country_region.csv) - country and region data
        
        
- [Healthcare( folder](https://github.com/reginesgit/project1/tree/main/Healthcare)):

    - [HealthcareStarter.ipynb](https://github.com/reginesgit/project1/blob/main/Healthcare/HealthcareStarter.ipynb) - notebook was    used to bring in raw data from World Health Organization Global Expenditure Database, clean columns, separate health and population, and create in csvs.
    - [Healthmergehappy.ipynb](https://github.com/reginesgit/project1/blob/main/Healthcare/healthmergehappy.ipynb) - notebook was used to bring happiness, health, and population csv&#39;s into one


- [Weather (folder)](https://github.com/reginesgit/project1/tree/main/Weather)

    - [Weather.ipynb](https://github.com/reginesgit/project1/blob/main/Weather/Weather.ipynb) - notebook used to prepare and merge data sources, perform API calls and export weather csv's.
    - [Weather_Report.ipynb](https://github.com/reginesgit/project1/blob/main/Weather/Weather_Report.ipynb) - notebook used for visualizations of weather and happiness data, also generated image files relating to weather.
    - [Countries_and_Capitals.csv](https://github.com/reginesgit/project1/blob/main/Weather/Countries_and_Capitals.csv) - Initial dataset used to perform weather requests.
    - [weather_data.csv](https://github.com/reginesgit/project1/blob/main/Weather/weather_data.csv) - export from weather.ipynb: weather data combined with country data.
    - [happiness_weather.csv](https://github.com/reginesgit/project1/blob/main/Weather/happiness_weather.csv) - export from weather.ipynb: weather data combined with avg. happiness data.
    - [happiness_weather_top10.csv](https://github.com/reginesgit/project1/blob/main/Weather/happiness_weather_top10.csv) - exported from weather.ipynb: top 10 "happiest" countries and their weather.
    

- [SocialSupport( folder](https://github.com/reginesgit/project1/tree/main/SocialSupport)):

     - [Social\_Support\_Final](https://github.com/reginesgit/project1/blob/main/SocialSupport/Social_Support_Final.ipynb) - Cleaning and Final Analysis : jupyter notebook used to analyze social support data 
    - [Resources (Folder](https://github.com/reginesgit/project1/tree/main/SocialSupport/Resources)):
        - [2015.csv](https://github.com/reginesgit/project1/blob/main/SocialSupport/Resources/2015.csv) - Happiness rank and scores by country, 2015 (raw data)
        - [2016.csv](https://github.com/reginesgit/project1/blob/main/SocialSupport/Resources/2016.csv) - Happiness rank and scores by country, 2016 (raw data)
        - [2017.csv](https://github.com/reginesgit/project1/blob/main/SocialSupport/Resources/2017.csv) - Happiness rank and scores by country, 2017 (raw data)
        - [2018.csv](https://github.com/reginesgit/project1/blob/main/SocialSupport/Resources/2018.csv) - Happiness rank and scores by country, 2018 (raw data)
        - [2019.csv](https://github.com/reginesgit/project1/blob/main/SocialSupport/Resources/2019.csv) - Happiness rank and scores by country, 2019 (raw data)
        - [avg\_FamilyHappiness.csv](https://github.com/reginesgit/project1/blob/main/SocialSupport/Resources/avg_FamilyHappiness.csv) - only average happiness and family data
        - [avg\_happiness.csv](https://github.com/reginesgit/project1/blob/main/SocialSupport/Resources/avg_happiness.csv)
        - [combined\_df.csv](https://github.com/reginesgit/project1/blob/main/SocialSupport/Resources/combined_df.csv)
        - [combined\_family\_15\_19\_df.csv](https://github.com/reginesgit/project1/blob/main/SocialSupport/Resources/combined_family_15_19.csv)
        - [merged\_happines\_data.csv](https://github.com/reginesgit/project1/blob/main/SocialSupport/Resources/merged_happiness_data.csv) - merged version of the five happiness csv



- [Images (Folder)](https://github.com/reginesgit/project1/tree/main/Images): this contains some of the images of chats and graphs as result of the analisys . Some images will be in the notebooks.

## Tasks

World Happiness Report (WHR) was base of the project. Using mean of the happiness score as the target Variable.

◦ Obtained additional external datasets to see what other factors would influence

happiness

◦ Based on question to answer, merged appropriate dataset with WHR on &#39;country

name&#39; (left join)

**Clean Up**

◦ Remove NaN&#39;s from datasets

◦ Rename duplicate column names for clarity

◦ Identify top (and bottom) countries based on happiness


## Analysis Process


Calculating numerical correlations → Scatter plots and linear regression


Understanding categorical correlations → Bar charts


Calculating relationship with more than 2 variables → Scatter plots with color label



## Data Sources

World Happiness Report

[https://www.kaggle.com/unsdsn/world-happiness](https://www.kaggle.com/unsdsn/world-happiness)

World Health Organization Global Expenditure Database

[https://apps.who.int/nha/database/Select/Indicators/en](https://apps.who.int/nha/database/Select/Indicators/en)

International Monetary Fund

[https://www.imf.org/en/Publications/SPROLLS/world-economic-outlook-databases#sort=%40imfdate%20descending](https://www.imf.org/en/Publications/SPROLLS/world-economic-outlook-databases#sort=%40imfdate%20descending)

World Bank Data Catalogue

[https://documents.worldbank.org/en/publication/documents-reports](https://documents.worldbank.org/en/publication/documents-reports)

Weather API

[https://openweathermap.org/ap](https://openweathermap.org/ap)





