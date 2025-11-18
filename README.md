# traffic_accident_severity_prediction
## Big Data & Data Mining Project – UK Road Accident Dataset (2020)

This project applies data mining, machine learning, clustering, and predictive modelling to the 2020 Great Britain Road Accident dataset. The goal is to understand accident patterns, identify key risk factors, and build a model capable of predicting accident severity.
## Overview

Road traffic accidents present serious public health challenges. This project analyses the Great Britain 2020 road accident dataset to extract insights, discover hidden patterns, and build predictive models that estimate accident severity.

The workflow covers data cleansing, exploratory data analysis, association rule mining, clustering, outlier detection, and classification modelling.
## Project Objectives

Clean and preprocess accident, casualty, vehicle, and LSOA datasets

Explore accident patterns by age, time, location, motorcycle type, pedestrian involvement, and weather

Identify contributing factors using Apriori Association Rule Mining

Detect geographical hotspots using KMeans and DBSCAN clustering

Detect unusual accident events using Isolation Forest, LOF, and IQR

Build and evaluate ML models for predicting accident injury severity
### Key cleaning operations included:

Replacing invalid values (e.g., -1 → mean or category)

Handling missing coordinates

Removing irrelevant fields

One-hot encoding for association mining
## Exploratory Data Analysis (EDA)
### Demographics

Male casualties were significantly higher than female

Highest accident involvement: ages 25–55Timing Patterns

Peak accident hours: 3pm–5pm

Pedestrian accidents peak at 8am and 3pm

Friday recorded the highest accident frequency

### Motorcycle Findings

125cc and 500cc+ vehicles peak at similar evening hours

500cc motorcycles see highest accidents on Sundays

### Environmental Insights

Most accidents occurred on dry roads, not during adverse weather

Low wind speeds were associated with more accidents
## Association Rule Mining (Apriori)

Apriori was used to understand relationships between:

Speed limits

Light conditions

Junction type

Road surface conditions

Urban vs rural areas

Lift was used to identify the strongest associations influencing severity.
## Accident Hotspot Detection
Clustering Techniques Used

KMeans (k=5 using elbow method)

DBSCAN

### Hotspots emerged around:

Hull

Scunthorpe

Hessle

Bridlington

Other key Humber region cities
## Outlier Detection

Applied three techniques:

Isolation Forest

Local Outlier Factor (LOF)

IQR Method

Findings:

Outliers mostly concentrated near London

Highlight potential abnormal or unusual accident events
## Machine Learning – Severity Prediction

Models tested:

Random Forest

Decision Tree

XGBoost

Best Model: Random Forest

Accuracy: 61%

Precision: 60%

F1-Score: 63%

Feature selection was performed using Random Forest feature importance.
## Tools

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

MLxtend (Apriori)

DBSCAN, KMeans
## Recommendations

Strengthen traffic law enforcement during peak hours

Improve pedestrian crossing infrastructure

Implement motorcycle lane markings

Dualize congested single-lane roads in urban areas
## Future Work

Train deep learning models

Expand datasets across multiple years

Integrate real-time traffic/weather data

Improve feature engineering to boost model accuracy
