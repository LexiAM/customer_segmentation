# Customer Segmentation With Unsupervised Learning

## Summary
In this project, we apply unsupervised machine learning techniques (PCA dimensionality reduction and K-Means clustering) to identify segments of a population based on demographics data. We then examine the distribution of the population among the identified segments for a specific subset of the population to identify over- and under-represented demographic groups as compared with the entire population.

This project is part of the Udacity Introduction to Machine Learning Nanodegree.

## Project Structure
Analysis Notebook:
- Identify_Customer_Segments.ipynb (also available in html)
- Data:
  - Udacity_AZDIAS_Subset.csv: Demographics data for the general population of Germany; 891211 persons (rows) x 85 features (columns).
  - Udacity_CUSTOMERS_Subset.csv: Demographics data for customers of a mail-order company; 191652 persons (rows) x 85 features (columns).
  - Data_Dictionary.md: Detailed information file about the features in the provided datasets.
  - AZDIAS_Feature_Summary.csv: Summary of feature attributes for demographics data; 85 features (rows) x 4 columns

Note: datasets and data documentation are not publicly available.

## Requirements
Python 3.6 + with the following packages:
- numpy
- pandas
- matplotlib
- seaborn
- sklearn

## Authors
- Alexander Manasson
- Udacity
