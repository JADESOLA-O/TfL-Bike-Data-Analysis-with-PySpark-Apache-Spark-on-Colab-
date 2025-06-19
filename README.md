Transport for London 2014 Bike Hire Analysis Using PySpark
This project explores London’s 2014 bike hire data using PySpark on Google Colab. It focuses on understanding ride duration patterns and performing statistical analysis to test whether ride durations from Baylis Road, Waterloo station differ from other stations.

Project Summary
I did an end-to-end Big Data analytics project using PySpark on Google Colab to analyze Transport for London (TfL) 2014 bike hire data. The project involves data cleaning, feature engineering, and hypothesis testing. Using a two-sample T-test, it was found that rides starting from Baylis Road, Waterloo station were significantly shorter than those from other stations.

Objective
The objective is to determine whether the average ride duration from Baylis Road, Waterloo station is statistically shorter than rides from other stations across London.

Tools & Technologies
Python (PySpark)
Pyspark.sql.functions
Google Colab
Pandas, NumPy
Matplotlib / Seaborn (for visuals)
Statistical tests (Levene's Test, Two-Sample T-Test)

Workflow
1. Data Cleaning & Preprocessing
Handled null and duplicate values
Converted timestamps to datetime format
Filtered station-specific data

2. Feature Engineering
Created new columns like Month, Day of Week for temporal analysis
Grouped ride counts by station and date for pattern analysis

4. Visualization
Bar charts showing seasonal ride trends
Identified July as the month with the highest ride count

4. Statistical Analysis
Levene's Test used to check for equal variances
Two-sample T-test conducted to compare ride durations

📊 Hypothesis Testing
Hypothesis:
H₀: There is no significant difference in ride durations between Baylis Road, Waterloo and other stations
H₁: Rides from Baylis Road, Waterloo are shorter

Results:
T-statistic: -10.67

p-value: 1.57e-26 (significant at α = 0.05)

Avg. duration (Baylis Road): 1046.69 secs

Avg. duration (Other stations): 1470.59 secs

Conclusion: Based on this findings we reject the null hypothesis as Rides from Baylis Road, Waterloo are statistically shorter.

Key Insights
Strong seasonal trends: fewer rides in winter, peak in summer (July)
Shorter ride durations from Baylis Road likely influenced by nearby commuting routes or short-distance usage
Demonstrates how big data processing with PySpark enables scalable analysis of urban mobility data
