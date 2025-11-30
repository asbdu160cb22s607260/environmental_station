Environmental Station Data Analysis
Project Overview
     This project demonstrates the data cleaning, preprocessing, and analytics workflow on a dataset collected from various environmental monitoring stations. The analysis aims to identify climate patterns, sensor anomalies, and derive insights about regional environmental conditions using Python's pandas and visualization libraries.​

Dataset
     500 records, 12 columns capturing station metadata, sensor readings (temperature, humidity, wind speed, precipitation, air quality), event notes, and regional information.

Common data issues 
     Missing values, inconsistent formats ("Two Thousand" vs 2000), duplicated entries, and textual errors.

Data Cleaning Process
     Removed duplicate rows to ensure data quality.

     Handled missing values using:

       Mode/most-frequent value for categorical fields like "Location".

       KNN imputer for numerical columns like "Temperature".

       Mean imputation and string replacements for fields like "Humidity" ("eighty" ⇒ 80).

       Forward-fill technique for columns such as "Elevation".​

     Standardized inconsistent data formats and converted text-based numbers to integers.

     Ensured correct data types for each column.

Analysis & Visualizations
     Explored temperature and humidity variations using scatter plots, grouped by region.

     Computed and plotted average temperature by region to reveal geographic climate differences.

     Examined sensor statuses and missing data patterns.

     Saved cleaned dataset as EnvironmentalStationCleaned.csv for reproducible results.​

