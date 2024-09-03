# Data-Driven Analysis of Air Quality in Beijing

## Overview
This project analyzes historical and real-time air quality data in Beijing using various data preprocessing and visualization techniques. It incorporates interactive elements to explore and update the data dynamically, providing insights into pollution trends and their potential impacts.

## Table of Contents
- [Project Structure](#project-structure)
- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Seasonal and Temporal Patterns](#seasonal-and-temporal-patterns)
- [Correlation Analysis](#correlation-analysis)
- [Interactive API and Dashboard Features](#interactive-api-and-dashboard-features)
- [Outliers Analysis](#outliers-analysis)
- [Results](#results)
- [Future Improvements](#future-improvements)
- [Business Value](#business-value)

## Project Structure
The project consists of the following files:
- `Data_Visualization_Beijing_Air_Quality_Analysis.ipynb`: Notebook for data preprocessing, exploratory data analysis, visualization, and interactive API integration.
- `Project Presentation.pptx`: Presentation summarizing the key findings and visualizations.
- `README.md`: Project documentation.

## Problem Statement
The project analyzes historical and real-time air quality data for Beijing to identify trends, seasonal variations, and correlations among different pollutants. The insights aim to support environmental decision-making and public awareness.

### Objectives
- Analyze long-term trends and real-time data in Beijing's air quality.
- Identify key pollutants contributing to poor air quality.
- Explore seasonal, temporal, and real-time patterns of pollutant levels.

## Dataset
The dataset includes:
- **Air Quality Data**: Daily records of PM2.5, PM10, O3, NO2, SO2, and CO concentrations from January 2014 to December 2023.
- **API Data**: Real-time air quality data fetched using an API, allowing dynamic updates.

### Columns in the Dataset:
- `Date`: Date of the observation.
- `PM25`: Particulate matter 2.5 micrometers or smaller.
- `PM10`: Particulate matter 10 micrometers or smaller.
- `O3`: Ozone concentration.
- `NO2`: Nitrogen dioxide concentration.
- `SO2`: Sulfur dioxide concentration.
- `CO`: Carbon monoxide concentration.

## Data Preprocessing
- **Column Renaming**: Removed spaces and standardized column names.
- **Data Type Conversion**: Converted the `Date` column to datetime format and pollutant columns to numeric types.
- **Outlier Handling**: Detected and removed outliers using the Interquartile Range (IQR) method to ensure data quality.

## Exploratory Data Analysis
- **Descriptive Statistics**: Analyzed the mean, median, and distribution of pollutant levels.
- **Box Plots**: Visualized the spread and outliers for each pollutant.
- **Histograms and Violin Plots**: Explored the frequency distributions and density of pollutant levels.

## Seasonal and Temporal Patterns
- **Seasonal Trends**: Identified higher pollutant levels in winter and peak ozone levels in summer.
- **Weekday vs. Weekend Analysis**: Found lower pollutant levels on weekends due to reduced traffic and industrial activity.
- **Visualizations**: Line charts and bar plots showing monthly, yearly, and day-type differences in pollution levels.

## Correlation Analysis
- **Heatmap**: Visualized the correlations between different pollutants.
- **Key Findings**:
  - Strong correlation between PM2.5 and PM10, indicating shared sources or behaviors.
  - Negative correlation between O3 and NO2 due to photochemical reactions.

## Interactive API and Dashboard Features
- **Widget API**:
  - Fetched data from the air quality API using Python requests.
  - Displayed real-time AQI data with dynamic updates using IPython's display capabilities.
  - Included a refresh button to update the AQI values and display the latest information on pollutant impacts.
  
- **Map Tile API**:
  - Integrated `folium` to display a map centered on Beijing.
  - Added real-time air quality markers using AQI data, visually representing pollution levels on the map.
  
- **Interactive Pollutant Trends**:
  - Developed dropdown widgets using `ipywidgets` to select different pollutants.
  - Enabled users to interactively view time trends of each pollutant by year, providing a clear visualization of how pollutant levels have changed over time.

## Outliers Analysis
- **Identification of Outliers**: Using IQR, identified days with extremely high or low pollution levels.
- **Outliers per Pollutant**:
  - PM2.5 and PM10 showed frequent spikes related to combustion sources and industrial activities.
  - O3 outliers corresponded with high sunlight and stagnant air conditions.
  - SO2 and CO outliers indicated sporadic but significantly elevated levels, possibly from industrial emissions and inefficient combustion.

## Results
- Successfully visualized and analyzed both historical and real-time air quality trends in Beijing.
- Identified key pollutants, their seasonal patterns, and interactive methods to monitor real-time data.
- Highlighted periods of high pollution and potential contributing factors.

## Future Improvements
- Expand interactive features and refine the dashboard for better user experience.
- Integrate additional data sources, such as weather or traffic data, to further enhance the analysis.
- Implement predictive models to forecast future air quality trends based on historical and real-time data.

## Business Value
- **Policy Support**: Provides data-driven insights for environmental policy decisions.
- **Public Awareness**: Enhances public understanding of air quality issues.
- **Health Impact**: Identifies periods of high pollution that can inform public health advisories.

---

This version incorporates the specific interactive elements you've developed, including the Widget API, Map Tile API, and interactive pollutant trend analysis, aligning well with the requirements of data analysis and visualization roles. Let me know if further adjustments are needed!
