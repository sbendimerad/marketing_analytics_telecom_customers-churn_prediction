1. Reflect on how churn impacts revenue and customer acquisition costs.
  * How is retaining existing customers more cost-effective than acquiring new ones ? 
  * How can churn indicate dissatisfaction or competitive disadvantage ?

    
2. Open a jupyter notebook and import the necessary libraries using the heper_strating_code.py.

   
4. Explore the data : 
  * Use pandas  `read_csv`  function to import your dataset. 
  * Apply `info()`, `describe()`, and `isnull().sum()` to get a preliminary view of the dataset’s structure and underlying patterns.

    
5. For data visualization, leverage seaborn's plotting functions. 
  * Begin with `sns.countplot()` for churn distribution. 
    * Create a figure with plt.figure(figsize=(8, 5))
    * Use `sns.countplot()` with the Churn column.
    * Add labels for x and y using plt.xlabel(???) and plt.ylabel(???)
    * Add a title with plt.title(???)
    $ display the chart with plt.show()
  * Use `sns.boxplot()`, tenure and Churn columns to compare tenure vs churn status. 
    * Begin with plt.figure(figsize=(8, 5))
    * Use `sns.boxlot()` with the tenure and Churn columns
    * Add labels for x and y using plt.xlabel(???) and plt.ylabel(???)
    * Add a title with plt.title(???)
    * Display the chart with plt.show()
  * Employ `sns.countplot()` again to analyze churn by InternetService and PaymentMethod, adjusting label rotation for clarity.
    * Begin with plt.figure(figsize=(8, 5))
    * Use `sns.countplot(x=???, hue=???, data=???, palette='Set3')`
    * Add labels for x and y using `plt.xlabel(???) and plt.ylabel(???)`
    * Add a title with plt.title(???)
    * Adjust label rotation with  `plt.xticks(rotation=45)`
    * Display the chart with plt.show()
   
      
6. Preprocess the data : 
  * I have already created for you the code that preprocesses the data, you can copy it from helper_preprocessing_code.py and paste it on your notebook.
  * Create a X dataframe by dropping customerID and Churn columns.
  * Create a Y dataframe by keeping just the Churn column.
  * Finally, split your data with `train_test_split`, ensuring a test size of 20%. You should have : X_train, y_train, X_test, y_test.
  * Apply the preprocessing code using this snippet : 
    `X_train_transformed = preprocessor.fit_transform(X_train)
     X_test_transformed = preprocessor.transform(X_test)`
    
7. Train a churn predictive model : 
  * Instantiate a LogisticRegression model from `sklearn.linear_model`. 
  * Fit the model on X_train_transformed data with the `.fit method`.
  * Predict on the X_test_transformed data using the and save the predicted data in variable named predictions. 
  * Use `accuracy_score`, `precision_score`, `recall_score`, `f1_score` from `sklearn.metrics` to evaluate your model on y_test and predictions.
  * Plot the confusion matrix 

