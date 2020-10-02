<img src="https://raw.githubusercontent.com/codecaviar/digital_asset_management/master/assets/bingyune-and-company-logo-6400x3600.png" align="left" width="200" height="auto">

<br/><br/><br/><br/>

----------

# Housing Crisis: 4 Tactics to Detect and Remove Outliers

**Code Caviar Story**: https://www.bingyune.com/blog/housing-crisis-outliers    

## Project Overview

Outliers are extreme data values that are distant from other values in your dataset. Outliers can distort the conclusions you draw from descriptive statistics (like mean and standard deviation) and from data visuals (like histograms and scatter plots). Many machine learning algorithms and statistical models are also sensitive to the range and distribution of data values used in your training data. Some of the most common causes of outliers in a dataset include data entry errors (human errors), measurement errors (instrument errors), and data processing errors (data manipulation errors). Consequently, outliers can come from multiple sources and hide in a single feature or n-dimensional feature space. Aside from the specific task of investigating these extreme data values (for anomaly detection) or in the case of naturally occurring outliers (novelties), the goal is often to remove or ignore outliers in your analysis.

**The goal of this project is to provide a Quick Guide on 4 popular methods for outlier detection.** The project makes use of the Boston House Pricing Dataset from [Sckit-Learn](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_boston.html). This dataset contains 506 instances and 13 numeric/categorical attributes (with no missing values). This dataset is a copy of [UCI ML housing dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/housing/) and was taken from the StatLib library maintained at Carnegie Mellon University.

## Summary:

Outliers are a simple concept - values that are notably different from other data points, and they can cause problems in statistical procedures. A univariate outlier is a data point that consists of an extreme value on one variable, while a multivariate outlier is a combination of unusual scores on at least two variables. Both types of outliers can influence the outcome of statistical analyses and machine learning models. Unfortunately, there are no strict statistical rules for definitively identifying outliers. Finding outliers depends on subject-area knowledge and an understanding of the data collection process. While there is no solid mathematical definition, the guidelines and statistical tests described in this article can be used to successfully find outlier candidates.

Extreme Value Analysis
    * Visualizing data with scatter plots, histograms, box plots
    * Use z-scores and interquartile range calculations
Proximity Methods
    * K-means
    * Density-Based Spatial Clustering of Applications with Noise (DBSCAN)
Projection Methods
    * Principal component analysis (PCA)
Higher Dimensional Automatic Detection
    * Isolation Forest
    * Minimum Covariance Determinant
    * Local Outlier Factor
    * One-Class Support Vector Machine

In general, you can follow these simple steps for handling outliers: 1) identify the potential outlier candidates; 2) remove the potential outlier candidates from your training dataset; and 3) evaluate the model performance.

## Getting Started

Cloning the git repository and installing the provided packages will help you get a copy of the project up and running on your local machine. The analysis for this project was performed using Jupyter Notebook (.ipynb) and the packages were managed using the Anaconda platform.

```
git clone https://github.com/codecaviar/housing-crisis-outliers.git
conda env create -f environment.yml
```

File Description:
* environment.yml - packages used to perform this analysis
* notebook_housing_crisis_outliers.ipynb - Jupyter Notebook for this project including data wrangling and exploratory data analysis     

## Authors

- **BingYune Chen** - [LinkedIn](https://www.linkedin.com/in/bingyune-chen/)
- **BingYune & Co** - [GitHub](https://github.com/codecaviar)

## License

The project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

The project referenced the following resources:
* https://www.kdnuggets.com/2017/01/3-methods-deal-outliers.html
* https://towardsdatascience.com/ways-to-detect-and-remove-the-outliers-404d16608dba
* https://machinelearningmastery.com/clustering-algorithms-with-python/
* https://pca4ds.github.io/
* https://machinelearningmastery.com/how-to-identify-outliers-in-your-data/
* https://jakevdp.github.io/PythonDataScienceHandbook/05.09-principal-component-analysis.html

----------
The Code Caviar is a digital magazine about data science and analytics that dives deep into key topics, so you can experience the thrill of solving at scale.
