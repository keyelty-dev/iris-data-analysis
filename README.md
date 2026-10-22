# Iris Dataset Analysis and K-Means Clustering

## Project Overview

This project focuses on Exploratory Data Analysis (EDA) and unsupervised machine learning using the Iris dataset. The main objective is to investigate the relationships between flower features, detect outliers, analyze correlations, and identify natural clusters among the three Iris species.

## Dataset

The Iris dataset contains 150 samples from three species:

- Setosa
- Versicolor
- Virginica

Each sample includes four numerical features:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

## Project Objectives

- Detect and analyze outliers using the Interquartile Range (IQR) method.
- Evaluate the potential impact of outlier removal on statistical measures.
- Investigate feature distributions and overlap between species.
- Analyze relationships between features using scatter plots.
- Calculate correlation coefficients and visualize correlation matrices.
- Apply feature scaling and determine the number of clusters using the Elbow Method.
- Perform K-Means clustering with three clusters.
- Evaluate clustering quality using the Silhouette Score.
- Compare the resulting clusters with the actual species labels.

## Methodology

### 1. Outlier Detection

The IQR method was applied to identify potential outliers across the four numerical features. Box plots, scatter plots, and summary tables were used to examine the detected observations.

### 2. Outlier Impact Analysis

Selected observations were examined in greater detail, and statistical measures were compared before and after their removal. Since the changes in the examined statistics were relatively limited, the observations were not automatically removed based solely on their statistical outlier status.

### 3. Feature Distribution and Species Overlap

Scatter plots and heatmaps were used to investigate similarities and overlap between species across sepal and petal measurements.

### 4. Correlation Analysis

Correlation coefficients, scatter plots, and heatmaps were used to explore linear relationships between features within each species.

### 5. K-Means Clustering

The four features were scaled before applying K-Means with the following parameters:

- Number of clusters: 3
- Random state: 42
- Number of initializations: 10

The Elbow Method was used to help select the number of clusters.

### 6. Clustering Evaluation

The clustering results were evaluated using the Silhouette Score and by comparing cluster assignments with the actual species labels.

## Results

- The dataset was divided into three clusters containing 53, 50, and 47 samples, respectively.
- The Silhouette Score was approximately 0.4599, indicating moderate cluster separation.
- All 50 Setosa samples were assigned to the same cluster.
- Versicolor and Virginica samples were distributed across the other two clusters, indicating that separating these species was more challenging.
- Petal features provided clearer visual separation between groups than sepal features.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Conclusion

This project demonstrates how exploratory data analysis, statistical techniques, visualization, and unsupervised machine learning can be combined to investigate a dataset.

The results suggest that petal measurements are particularly useful for distinguishing Iris species. K-Means successfully grouped the Setosa samples, while some overlap remained between Versicolor and Virginica.

The project also highlights the importance of evaluating outliers carefully and interpreting clustering results alongside visualizations and quantitative metrics.

## Project File

The Jupyter Notebook contains the analysis, visualizations, statistical calculations, clustering implementation, and evaluation results.
