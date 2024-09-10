# GDP-Analysis-of-countries-with-R

## Overview
This project is a collaborative effort by **Mallikarjuna Gowdra Basavarajappa**, **Mark Walter Alfred**, **Swathi Pydi**, and **Udit Jayant Dayani** for the ST661 course. It involves an analysis of the GDP and gender wage gap data across different countries and regions from 1950 to 2021. The project aims to identify trends, regional variations, and correlations between gender wage gaps and GDP using **R** for data wrangling, analysis, and visualization.

## Dataset
The project utilizes two datasets:
- **GDP Dataset**: Contains GDP per capita (in USD) for 130 countries from 1950 to 2021.
- **Gender Wage Gap Dataset**: Covers gender wage gap percentages for 38 countries from 1970 to 2015.

## Research Questions
1. Which countries exhibited the largest and smallest gender wage gaps, and how consistent were they over time?
    - Year-by-year analysis from 2000 to 2015.
    - Decade-by-decade analysis since 1980 for select countries.
2. Were there regional trends in gender wage gaps?
3. What correlations exist between gender wage gaps and a country’s GDP?

## Data Wrangling
The datasets were cleaned and merged as follows:
1. Removed years prior to 2000 to focus on the period between 2000-2015.
2. Missing data points were filled using the mean for that country/year.
3. Each country was assigned to a region to enable regional analysis.
4. The datasets were merged on the "Country" column, enabling joint analysis of gender wage gaps and GDP.

## Tools and Libraries Used
- **R**: Main programming language used for data manipulation, analysis, and visualization.
- **Shiny**: Interactive web application framework for building visualizations.
- **ggplot2**: For plotting graphs and visualizations.
- **dplyr**: For data wrangling and manipulation.
- **tidyr**: For transforming data into a tidy format.
- **readr**: For reading CSV files.

## Analysis and Key Insights
### Question 1a: Year-by-year Gender Wage Gaps (2000-2015)
- **Largest Gap**: South Korea exhibited the largest gender wage gap, averaging around 38.81%.
- **Smallest Gap**: Costa Rica had the smallest gap, averaging around 3.37%.
- Most countries showed a decrease in wage gaps from 2000 to 2010, but some gaps increased again after 2010.

### Question 1b: Decade-by-decade Gender Wage Gaps (1980 onwards)
- **Key Finding**: Countries like the UK, US, Finland, and Japan showed a consistent reduction in gender wage gaps across decades. In contrast, Australia and Sweden had more fluctuation in their wage gaps.

### Question 2: Regional Gender Wage Gap Trends
- **Western Europe**: Downward trend, with Ireland and Luxembourg showing the most significant decreases.
- **Southern Europe**: Fluctuating wage gaps, with GDP decreases during the financial crisis (2007-2013).
- **Northern Europe**: Stable gaps in Norway and Denmark, with Iceland showing volatility.
- **Central & Eastern Europe**: Estonia exhibited the highest and most consistent gender wage gap.

## Shiny App
A Shiny app was developed to allow users to interactively explore:
1. Gender wage gap and GDP trends by region.
2. Gender wage gap and GDP trends by country.

### To run the app:
1. Clone the repository.
2. Install required libraries:
   r
   install.packages(c("shiny", "ggplot2", "dplyr", "tidyr", "readr"))
   
3. Launch the Shiny app:
   r
   shiny::runApp("path_to_app_folder")
   

## How to Run the Analysis
1. Open the R script or RMarkdown file.
2. Ensure the datasets are loaded and wrangled as described.
3. Execute the analysis to generate visualizations and tables.
