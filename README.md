# machine_learning_project-unsupervised-learning

## Project Outcomes
- Unsupervised Learning: perform unsupervised learning techniques on a wholesale data dataset. The project involves four main parts: exploratory data analysis and pre-processing, KMeans clustering, hierarchical clustering, and PCA.

### Project Description:
In this project, we will apply unsupervised learning techniques to a real-world data set and use data visualization tools to communicate the insights gained from the analysis.

The data set for this project is the "Wholesale Data" dataset containing information about various products sold by a grocery store.
The project will involve the following tasks:

-	Exploratory data analysis and pre-processing: We will import and clean the data sets, analyze and visualize the relationships between the different variables, handle missing values and outliers, and perform feature engineering as needed.
-	Unsupervised learning: We will use the Wholesale Data dataset to perform k-means clustering, hierarchical clustering, and principal component analysis (PCA) to identify patterns and group similar data points together. We will determine the optimal number of clusters and communicate the insights gained through data visualization.

The ultimate goal of the project is to gain insights from the data sets and communicate these insights to stakeholders using appropriate visualizations and metrics to make informed decisions based on the business questions asked."

## Process

### EDA and Preprocessing

A lot of time was spent on the exploration and cleanin stage. Some of the decisions made in this portion of the project were to omit the categorical details(further explanation on that is within the notebook), the use of Box-Cox transformation over logarithmic transformation and to proceed with the project with a comparison between two versions of the data set, one with outliers and one without.

### Model Training

As expected, by having to do everything twice this part of the project took quite some time, but was interesting to me on a learning level to see the differences, and similarities between the data sets when utilizing the different models. The project entails the use of KMeans Clustering, Aglommerative Clustering and Principal Component Analysis for analysing the features.

### Conclusion

- There are some noteable positive correlations between some of the features and only a very slight difference between the numbers for our original data set and the data set where the outliers were removed: \
    -Grocery and Detergents_Paper    0.818    0.818\
    -Milk and Grocery                0.777    0.777\
    -Milk and Detergents_Paper       0.685    0.693
    
- All models looked better with 2 clusters across the board. The KMeans model appears to edge out the Aglommerative model just slightly as the groupings look a little cleaner.

- 93% of the variability could still be explained when we reduced our model to 4 components.

- When looking at the sihouette scores, there is a small interesting peak at 6 variables on the chart. Is this because there are 6 original categories?
