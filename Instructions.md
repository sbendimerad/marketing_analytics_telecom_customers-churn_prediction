1. Examine the dataset to understand the churn phenomenon. Identify 3 reasons why analyzing customer churn is crucial for telecom companies.
2. Import the necessary libraries.
3. Load the dataset and conduct an exploratory data analysis (EDA).
   * Import the dataset using pandas.
   * Examine data shape, data types, percentage of missing values by columns.
   * Display basic statistics.
4. Execute specific data visualizations to gain insights into factors affecting churn. 
   * Plot the distribution of customer churn with count plot.
   * Compare the tenure of churned vs. retained customers with a box plot.
   * Explore the relationship between payment methods and churn with a count plot.
5. Prepare your dataset for predictive modeling. 
   * Use the helper_preprocessing_code.Py tp prepare the data.
   * Split the dataset into an 80% training set and a 20% testing set.
6. Train a logistic regression model to predict customer churn and evaluate its performance. 
  * Implement a logistic regression model using scikit-learn.
  * Calculate the model's accuracy, precision, recall, and F1-score. 
  * Interpret the confusion matrix to evaluate model effectiveness.
