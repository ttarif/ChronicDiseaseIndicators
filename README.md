# Chronic Disease Indicators Analysis

This project is a comprehensive analysis of the Chronic Disease Indicators dataset. It includes exploratory data analysis, temporal analysis of disease indicators, geographic comparison of disease indicators, demographic analysis of disease indicators, and a predictive model.

## Table of Contents

- Motivation
- Dataset Description
- Data Wrangling
- Installation
- Usage
  - Temporal Analysis of Disease Indicators
  - Geographic Comparison of Disease Indicators
  - Demographic Analysis of Disease Indicators
  - Word Cloud of Disease Reports
  - Predictive Modeling
- Results and Implications

## Motivation

The analysis of chronic disease indicators is crucial for understanding disease patterns, guiding health interventions, and resource allocation. This project aims to:

- **Understand Disease Patterns**: Analyze the progression and prevalence of chronic diseases over time.
- **Support Health Interventions**: Identify high-risk populations and inform preventive measures.
- **Resource Allocation**: Guide public health officials in prioritizing resources for the most prevalent or severe conditions.
- **Monitor and Evaluate Interventions**: Assess whether health interventions are effective and inform necessary adjustments.

## Dataset Description

- **Source**: U.S. Chronic Disease Indicators dataset from [Data.gov](https://catalog.data.gov/dataset/u-s-chronic-disease-indicators).
- **Time Span**: Data from 2001 to 2021.
- **Contents**: The dataset includes information on location, data source, topics, questions, responses, data values, confidence limits, and stratification categories such as gender and ethnicity.
- **Use Case**: The dataset allows for a detailed analysis of chronic disease indicators, including temporal trends, geographic disparities, and demographic differences.

## Data Wrangling

The data wrangling process involves:

- **Data Acquisition**: Downloading and loading the dataset into a pandas DataFrame.
- **Data Cleaning**:
  - Removing columns with no unique values.
  - Filtering out rows with missing values.
  - Converting value columns to numeric.
  - Filtering out rows where values are totaled.
  - Creating a combined text data column for textual analysis.
- **Data Transformation**:
  - One-Hot Encoding for categorical variables.
  - Standardizing data values.
  - Encoding topic labels.
  - Filtering data by decade for temporal analysis.

## Installation

The project is written in Python. You need to have Python installed to run this project. The required libraries are:

- pandas
- matplotlib
- seaborn
- plotly
- ipywidgets
- sklearn
- collections
- wordcloud
- imblearn
- xgboost

You can install these libraries using pip:

```python
pip install pandas matplotlib seaborn plotly ipywidgets sklearn collections wordcloud imblearn xgboost gdown
```

## Usage
The project includes the following tasks:

### Temporal Analysis of Disease Indicators
Analyze the progression of disease indicators over time to identify trends and patterns that can predict future disease prevalence. This is visualized through interactive line charts, allowing users to modify time periods and analyze trends by mean data values.

### Geographic Comparison of Disease Indicators
Compare disease indicators across different geographic regions to identify hotspots and disparities. This task uses choropleth maps to visualize disease prevalence across states.

### Demographic Analysis of Disease Indicators
Explore how disease indicators vary across different demographic groups such as gender, age, and race/ethnicity. Stacked bar charts are used to illustrate disparities, aiding healthcare providers in tailoring interventions.

### Word Cloud of Disease Reports
Generate a word cloud to understand the frequency of words used in disease reports. This provides qualitative insights into prevalent health issues and emerging trends.

### Predictive Modeling
Build and evaluate a predictive model to forecast disease indicators based on various features. The model's performance is assessed using metrics such as accuracy, confusion matrices, and classification reports.

## Results and Implications
The results from this analysis provide critical insights for public health officials, policymakers, and healthcare providers:

- Temporal Analysis: Helps in predicting future disease prevalence and planning preventive measures.
- Geographic Comparison: Enables resource allocation to regions with higher disease burdens.
- Demographic Analysis: Supports the tailoring of interventions to specific demographic groups.
- Word Cloud: Informs emerging trends based on textual data.
- Predictive Modeling: Provides a tool for anticipating disease indicators, aiding in effective resource allocation and preventive planning.
