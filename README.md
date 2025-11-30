🌿 Environmental Station Data Analysis
📌 Project Overview

     This project demonstrates a complete data cleaning, preprocessing, and analytics workflow on a dataset collected from multiple environmental monitoring stations. The goal is to identify climate patterns, detect sensor anomalies, and derive insights into regional environmental conditions using Python’s pandas and visualization libraries.

📁 Dataset

     The dataset contains 500 records and 12 columns, including:

       Station metadata

       Sensor readings (temperature, humidity, wind speed, precipitation, air quality)

       Event notes

       Regional information

⚠️ Common Data Issues

     The raw dataset included several real-world data problems such as:

       Missing values

       Inconsistent formats (e.g., "Two Thousand" vs 2000)

       Duplicated entries

       Textual spelling or formatting errors

🧹 Data Cleaning Process
🔁 Duplicate Handling

     Removed all duplicate rows to improve dataset reliability.

🧩 Missing Value Treatment

     Categorical fields (e.g., Location): Filled using mode.

     Numerical columns (e.g., Temperature): Filled using KNN Imputer.

     Humidity: Used mean imputation and converted entries like "eighty" → 80.

     Elevation: Filled using forward-fill (FFILL) to maintain logical sequence.

🛠 Standardization

     Converted text-based numbers into integers.

     Standardized inconsistent data formats.

     Ensured correct data types across all columns.

📊 Analysis & Visualizations

     Scatter plots to study temperature and humidity variations by region.

     Average temperature charts to reveal geographic climate differences.

     Sensor status analysis and missing data pattern evaluation.

     Saved cleaned dataset as EnvironmentalStationCleaned.csv for reproducibility.

🚀 Tools & Libraries

     Python 

     Pandas – data manipulation

     NumPy – numerical operations

     Matplotlib & Seaborn – visualizations

     Scikit-Learn – KNN imputation
