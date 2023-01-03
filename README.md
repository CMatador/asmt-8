# Visualizing the 2019 Annual Business Survey using Census API Data
## Overview
Our repo is organized as follows:
- Visualizations and the code used to create them are stored in the [viz.ipynb](https://github.com/CMatador/asmt-8/blob/master/viz.ipynb) file
- Our code for data extraction, transformation, and loading is stored in the [etl.ipynb](https://github.com/CMatador/asmt-8/blob/master/etl.ipynb) file
- Our extracted and cleaned data, which we use for the visualizations, are stored in CSV format in the [CSV](https://github.com/CMatador/asmt-8/tree/master/CSV) file

## Data Summary
From the ABS [Website](https://www.census.gov/data/developers/data-sets/abs.2019.html): 
> The Annual Business Survey (ABS) provides information on selected economic and demographic characteristics for businesses and business owners by sex, ethnicity, race, and veteran status. The ABS replaces the five-year Survey of Business Owners (SBO) for employer businesses, the Annual Survey of Entrepreneurs (ASE), the Business R&D and Innovation for Microbusinesses survey (BRDI-M), and the innovation section of the Business R&D and Innovation Survey (BRDI-S).
> Datasets include:
>- **Company Summary.** Provides data for employer businesses by sector, sex, ethnicity, race, veteran status, years in business, receipts size of firm, and employment size of firm for the U.S., states, and metro areas. Data for counties and economic places are available for 2018, and urban and rural classification of firms are available for 2021.
>- **Characteristics of Businesses.** Provides data for respondent employer firms by sector, sex, ethnicity, race, veteran status, years in business, receipts size of firm, and employment size of firm for the U.S., states, and metro areas, including detailed business characteristics. Data for counties and economic places are available for 2018, and urban and rural classification of firms are available for 2021.
>- **Characteristics of Business Owners.** Provides data for owners of respondent employer firms by sector, sex, ethnicity, race, and veteran status for the U.S., states, and metro areas, including detailed owner characteristics. Data for counties and economic places are available for 2018.
>- **Module Business Characteristics.** Newly introduced in 2021, provides data for respondent employer firms by sector, sex, ethnicity, race, veteran status, years in business, receipts size of firm, and employment size of firm for the U.S., states, and metro areas, including unique business characteristics such as types of technology used by the business, and the effect of the Coronavirus Pandemic on the business. Urban and rural classification of firms are available for 2021.

<!-- I think here we should add a link to the API variable descriptions as well as maybe the code from the ETL where we change variable names -->

## Problem Statement
Our goal was for our team to demonstrate our proficiency in API usage, data extraction, transformation, and cleaning (ETL), visualization, and analysis while answering the following questions:
- How do worker status, industry occupation, and owner race intersect to affect worker pay? 
- How are nulls distributed throughout this dataset?
- How are different technologies employed across states and industries, and how do they affect worker employment?
- How are owner demographics distributed? And how does the distribution of these demographics affect revenue?

## Data Processing
- We gathered our data from the 2019 Annual Business Survey through their API.
- Created functions to clean the API response texts and convert them into DataFrames.
- We then selected relevant columns and to export to csv files for analysis and visualization.
- Full process detailed here: [ETL](https://github.com/CMatador/asmt-8/blob/master/etl.ipynb)

## Results
There are 4 topics explored through data analysis and visualization:

  1. Business/Employee Characteristics
  2. Revenue
  3. Business Owner Demographics
  4. Technology Usage
  
A general overview of our results follow. Business owners are predominantly white males in older age groups. Companies owned by white individuals have much, much higher revenues than minority-owned businesses. Cloud services and specialized software are the most popular technologies adopted by companies. 

## Conclusions and Next Steps
