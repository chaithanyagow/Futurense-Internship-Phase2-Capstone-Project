# Sports Data Analysis and Data Warehousing Project

# Introduction

This repository contains a comprehensive project focused on the analysis, transformation, and warehousing of sports data. It includes various IPython notebook files (.ipynb), SQL scripts, and dataset files. The project addresses multiple problem statements, each targeting specific data processing and analytical tasks using Python, SQL, and various data visualization tools.

# Dataset Files
Sports dataset.csv, cleaned_sports_dataset.csv: The primary dataset used throughout the project, containing various features related to player performance, health, and training.
player_details.csv: Contains details about individual players such as their age, height, weight, and position.
player_performance.csv: Contains performance metrics of players like goals, assists, and cards received.
health.csv: Contains health-related metrics of players such as fatigue and injury history.
training.csv: Contains training-related metrics such as training hours and effective training.

Problem Statements
Problem Statement 1: Data Cleaning and Imputation
Description:
dentify and handle missing values using advanced imputation techniques.
Correct anomalies by identifying outliers using statistical methods and domain knowledge.
Standardize data formats and ensure consistency across the dataset.

Approach:
Used KNN Imputer for missing value imputation.
Applied z-score to identify and remove outliers.
Standardized and validated the dataset to ensure consistency.

Problem Statement 2: Player Position Analysis
Description:
Analyze player positions to identify the highest and lowest number of players.
Perform statistical analysis to determine if the distribution of players across positions is significantly different from a uniform distribution.

Approach:
Performed chi-square tests to validate the findings.
Created visualizations to display the distribution of players by position.

Problem Statement 3: Data Ingestion Pipeline
Description:
Design and implement a data ingestion pipeline that supports incremental data loading.
Optimize storage using data partitioning and indexing strategies.
Implement logging and monitoring to track performance and reliability.

Approach:
Incremental Loading: Implemented Python scripts to handle incremental data loading into a SQLite database. The pipeline ensures that only new or updated records are loaded, avoiding redundancy.
Optimization: Used partitioning and indexing to improve storage and query performance.
Logging and Monitoring: Added logging to track the data ingestion process, including error handling and performance metrics.

Problem Statement 4: Pass Completion Rate and Assists Analysis
Description:
Analyze the relationship between pass completion rate and assists.
Identify outliers using advanced outlier detection methods.
Perform regression analysis and evaluate the model.

Approach:
Used Isolation Forest for outlier detection.
Applied linear regression and cross-validation for model evaluation.

Problem Statement 5: Feature Engineering and Optimization
Description:
Perform complex transformations on the dataset, including feature engineering.
Implement data normalization and dimensionality reduction.
Use machine learning techniques for feature selection.

Approach:
Created new features such as GoalsPerGame, AssistsPerGame, and CardsPerGame.
Applied PCA for dimensionality reduction.
Normalized the data using MinMaxScaler.

Problem Statement 6: Data Warehouse Schema Design
Description:
Design and implement a data warehouse schema using advanced SQL features like window functions and CTEs.
Store the transformed data efficiently and ensure it supports complex analytical queries.
Implement data security and access control mechanisms.

Approach:
Schema Design: Created dimension and fact tables for storing detailed and aggregated data.
Advanced SQL Features: Used CTEs and window functions for complex queries.
Optimization: Implemented indexing, partitioning, and materialized views for performance optimization.

Problem Statement 7: Team and Player Performance Analysis
Description:
Identify the team with the highest number of goals.
Perform a time series analysis to understand trends in goal scoring over the season.
Analyze the top goal scorer's performance metrics over time.

Approach:
Created various visualizations including horizontal bar plots and stacked bar charts.
Conducted time series analysis to identify trends and patterns.

Problem Statement 8: Interactive Dashboard Creation
Description:
Create an interactive dashboard using Pygwalker to explore and visualize the dataset dynamically.

Approach:
Utilized Pygwalker to generate interactive visualizations and dashboards for comprehensive data exploration.
