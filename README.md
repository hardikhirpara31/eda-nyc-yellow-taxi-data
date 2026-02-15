# eda-nyc-yellow-taxi-data
Exploratory Data Analysis On New York City Yellow Taxi Data

Objective:
Learning exploratory data analysis (EDA) with the help of a dataset on yellow taxi rides in New York City.
Understand why EDA is an important step in the process of DS & ML.


Problem Statement:
As an analyst at an upcoming taxi operation in NYC, you are asked to use the 2023 taxi trip data to uncover insights that could help optimise taxi operations. The goal is to analyse patterns in the data that can inform strategic decisions to improve service efficiency, maximise revenue, and enhance passenger experience.


Project workflow:
1. Data Loading
2. Data Cleaning
3. Exploratory Analysis: Bivariate and Multivariate
4. Creating Visualisations to Support the Analysis
5. Deriving Insights and Stating Conclusions


Data Understanding:
The yellow taxi trip records include fields capturing pick-up and drop-off dates/times, pick-up and drop-off locations, trip distances, itemized fares, rate types, payment types, and driver-reported passenger counts.
The data is stored in Parquet format (*.parquet*). The dataset is from 2009 to 2024. However, for this assignment, we will only be using the data from 2023.
The data for each month is present in a different parquet file. You will get twelve files for each of the months in 2023.
The data was collected and provided to the NYC Taxi and Limousine Commission (TLC) by technology providers like vendors and taxi hailing apps.
You can find the link to the TLC trip records page here: https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page


Data Description:
You can find the data description here: [Data Dictionary](https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf)


Taxi Zones:
Each of the trip records contains a field corresponding to the location of the pickup or drop-off of the trip, populated by numbers ranging from 1-263.
These numbers correspond to taxi zones, which may be downloaded as a table or map/shapefile and matched to the trip records using a join.
This is covered in more detail in later sections.


Directory Structure:
├── dataset/
│    ├── taxi_zones/
│    ├── trip_records [Download 1-12 months .parquet files from https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page]/
├── notebook
│    ├── EDA_NYC_Taxi_Analyis.ipynb
├── images
│    ├── data-dictionary.png
├── eda_report
│    ├── EDA_NYC_Taxi_Analysis.pdf
├── README.md


Libraries required:
os
numpy
pandas
matplotlib
seaborn
scikit-learn
pathlib
warnings
geopandas
