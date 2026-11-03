# NUMBER OF DEATHS BY CAUSE- What Mortality rate looks like in 30 years 

## Introduction
This project analyses global mortality trends over a 30-year period, examining the number of deaths attributed to different causes across countries. The analysis focuses on identifying the leading causes of death, tracking changes in mortality patterns over time, and highlighting countries with the highest death counts. The goal is to generate insights that support better understanding of global health challenges and inform public health planning and decision-making.

## Problem Statement
Understanding the major causes of death and their distribution across countries is essential for effective public health planning. However, without a clear analysis of long-term mortality trends, it is difficult to identify leading causes of death, track changes over time, and determine which countries bear the greatest mortality burden. 

This project addresses this gap by analyzing 30 years of mortality data to uncover key patterns, identify the leading causes of death, and highlight countries with the highest death counts.

## Data Sourcing
The dataset is a public-made dataset available on Kaggle for practical purpose, containing 6061 records from a period of 1990 to 2019.

The key fields include;
 - Country
 - Year
 - Causes

## Data Cleaning and Transformation
 - A backup copy of the raw data was made
 - Separated real countries from aggregates (World bank, income groups, WHO regions, OECD, World) to avoid double-counting
 - The Cause fields were unpivoted into Cause and Number, to easy DAX writing

## Data Modelling (Power BI)
A Galaxy Schema was built in Power BI to connect the fact tables to the Dimension tables

Fact tables
 - Annual Country Deaths
 - World Deaths
 - WHO Regions
 - World Bank Regions
 - Income Groupings
 - G20 Countries
 - OECD Countries
   
Dimension tables
 - Dim Country
 - Dim Year

**_View Relationships_**
![](Data_Modelling.png)

##Analytics and Measures




