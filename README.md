# Customer Segmentation Analysis With Unsupervised Learning

## Summary
In this project, we apply unsupervised machine learning techniques to identify segments of a population based on demographics data. We then examine the distribution of the population among the identified segments for a specific subset of the population to identify over- and under-represented demographic groups as compared with the entire population. The demographic groups over-represented in the population subset are deemed as of high target value for an advertisement campaign.

First dimensionality of the demographics data is reduced using Principal Component Analysis (1st PCA component in shown below):

![](resources/pca1.png?raw=true)

Next, we split population into clusters using K-Nearest Neighbors algorithm with elbow method of selecting optimal number of clusters and compare clustering of general and target populations:

![](resources/clusters.png?raw=true)

Finally, we examine principal components for the clusters with largest discrepancies between populations for insights about the groups:  

![](resources/top_pca_cluster2.png?raw=true)

## Results
Our analysis shows that population with high target value for an advertisement campaign consists from high income-earners, with lower mobility, living in neighborhoods with higher share of 1-2 family homes in dense metropolitan areas not far from city centers, with avantegarde and "green" conscientious views. The group of customers unlikely to repsond to an advertisement campaign were found to consist from younger, less traditional, low income-earners, with high mobility, living in neighborhoods with higher share of 6-10 family homes. It is interesting to note that the under-represented clusters contain both positive and negative values for PCA component #3, implying that this group is gender neutral (male and female), with less dominant males who are more likely to invest and more dominant females who are less likely to invest.

## Project Structure
```
|-- `Identify_Customer_Segments.ipynb`: main analysis Jupyter Notebook
|-- `Identify_Customer_Segments.html`: main analysis html version
```

## Data:
Note: datasets and data documentation are not publicly available.
### Data Summary
  - Udacity_AZDIAS_Subset.csv: Demographics data for the general population of Germany; 891211 persons (rows) x 85 features (columns).
  - Udacity_CUSTOMERS_Subset.csv: Demographics data for customers of a mail-order company; 191652 persons (rows) x 85 features (columns).
  - Data_Dictionary.md: Detailed information file about the features in the provided datasets.
  - AZDIAS_Feature_Summary.csv: Summary of feature attributes for demographics data; 85 features (rows) x 4 columns

## Requirements
Python 3.6 + with the following packages:
```
numpy
pandas
matplotlib
seaborn
sklearn
```

## Authors
- Alexander Manasson

## Acknowledgements
- Udacity for providing template notebook
- AZDIAS for providing data used in analysis
