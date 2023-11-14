## Dataset Source
https://www.kaggle.com/datasets/akshaydattatraykhare/diabetes-dataset

## Objective
Use and evaluate different classification models to determine which best fit the given data.

## Notebook Contents
1. Part I - Data Cleaning and EDA
2. Part II - Handling Missing Values, Feature Selection and Scaling
3. Part III - Modeling
4. Conclusion and Findings
5. Functions

## Approach
1. Use different visualizations to explore the shape and distribution of data.
2. Audit the data to find missing and duplicate values.
3. Handle missing or zero values by using the mean best fit for the feature:
   a. Divide the dataset into two groups based on the outcome feature.
   b. Get the mean of each group of dataset.
   c. Replace the zero values with the mean of whatever group the instance belongs to.
   d. Make sure not to replace the zero values of the features where it is normal to have zero values. For instance, pregnancies.
4. Compare the mean of the two datasets and select the features with higher Outcome = 1 and Outcome = 0 ratio, which means that the features with higher Outcome = 1 and Outcome = 0 ratio are lkely correlated to the Outcome = 1.
5. Create two trials, one using all the feature with higher than 20% of Outcome = 1 and Outcome = 0 ratio and the other using all the feature with higher than 10% of Outcome = 1 and Outcome = 0 ratio.
6. Use different machine learning classification models and compare the metrics of each models.
7. Select the model which have the best recall score as recall is one of the key metrics used in medical diagnosis.
