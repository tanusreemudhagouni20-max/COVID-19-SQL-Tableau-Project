# COVID-19-SQL-Tableau-Project
# COVID-19 Data Exploration Project

## Project Overview
This project explores global COVID-19 data to analyze infection trends, mortality rates, and vaccination progress across countries. 
SQL was used to clean and analyze the dataset, while Tableau was used to build an interactive dashboard to visualize key insights.
The goal of this project is to transform raw pandemic data into meaningful insights that help understand how COVID-19 spread globally and how different countries were affected.

## Tools Used
* SQL Server Management Studio
* Tableau

## Project Objectives
Clean and prepare the dataset using SQL
 Explore key metrics such as total cases, total deaths, and infection rates
 Calculate important indicators such as death percentage and percentage of population infected
 Analyze vaccination progress using SQL joins and window functions
 Create structured datasets for visualization
 Build an interactive Tableau dashboard to communicate insights effectively

## Data Profile
Two datasets were used in this project.
### 1. Covid Deaths Table

Columns include:
* Location
* Continent
* Date
* Population
* Total Cases
* New Cases
* Total Deaths
* New Deaths

### 2. Covid Vaccinations Table
Contains vaccination data across countries.

Columns include:
* Date
* Location
* Vaccinations

## Data Cleaning
The dataset was cleaned and prepared using SQL before performing analysis.

Steps performed:
* Removed aggregated rows such as world or continent totals by filtering records where the 'continent column was NULL'
* Handled missing values in vaccination columns to avoid calculation errors
* Converted numeric columns such as deaths and vaccinations to appropriate data types
* Ensured the dataset contained only country-level records for reliable comparisons

## SQL Data Exploration
SQL queries were used to explore the spread and impact of COVID-19 across countries.

### Death Percentage Analysis
Calculated the percentage of deaths relative to confirmed cases to understand the severity of the disease in different countries.

### Infection Rate Analysis
Calculated the percentage of population infected in each country to identify regions with the highest infection rates.

### Global Trends Over Time
Analyzed case trends over time to understand how the pandemic evolved across different waves.

### Vaccination Progress Analysis
Vaccination data was analyzed by joining the deaths dataset with the vaccination dataset.
A 'window function' was used to calculate cumulative vaccinations for each country, showing the running total of vaccinations over time.

### Vaccination Percentage Using CTE
A 'Common Table Expression (CTE)' was used to calculate the percentage of population vaccinated, enabling comparisons between countries.

## Tableau Visualization
After completing the SQL analysis, the processed dataset was imported into Tableau to create an interactive dashboard.
The dashboard highlights infection rates, death counts, and global pandemic trends.

### Dashboard Visualizations
'Global Cases and Death Percentage' – Summary of total global cases, deaths, and death percentage
'Death Count by Continent' – Comparison of total deaths across continents
'Countries with Highest Infection Rate' – Percentage of population infected by country
'Global Infection Trends Over Time' – Time-series visualization showing pandemic waves

## Key Insights
* The global dataset shows 150,574,977 confirmed cases and 3,180,206 deaths, resulting in a global death rate of approximately 2.11%.
* The United States recorded the highest total death count, followed by Brazil and Mexico.
* Countries such as Andorra experienced very high infection rates, with approximately 17.12% of the population infected.
* North America recorded the highest death count among continents, followed by South America and Asia.
* Time-series analysis shows infection rates increasing steadily from late 2020 through mid-2021, indicating multiple waves of the pandemic.
* Countries including the United States, United Kingdom, and India experienced significant infection surges during early 2021.

## Conclusion
This project demonstrates how SQL and Tableau can be used together to analyze large datasets and generate meaningful insights.
SQL Server Management Studio was used for data cleaning, transformation, and analytical queries to calculate key pandemic metrics. The results were then visualized in Tableau through an interactive dashboard that highlights global case trends, mortality rates, and infection patterns.

## Repository Contents
1. COVID 19 Sql query.sql-  SQL queries used for data exploration 
2. Covid 19 Tableau.twbx-  Tableau dashboard file  
3. COVID 19 Sql,Tableau report.docx-  Detailed project report 
4. Tableau Dashboard.png-  Dashboard preview image


 















