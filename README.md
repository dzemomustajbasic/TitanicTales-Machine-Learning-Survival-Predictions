# Description

This project aims to predict the survival of passengers on the Titanic using machine learning techniques. The dataset is obtained from the Kaggle Titanic competition, which contains information about passengers such as age, gender, class, and more. The goal is to build a predictive model that can determine whether a passenger survived or not based on these features.

I chose the Random Forest Classifier for this task because it is an ensemble model that aggregates multiple decision tree algorithms. I opted for this algorithm because it is well-suited for classification tasks, particularly in scenarios where the dataset may have complex relationships between features and the target variable (Survived in this case). Random forests are effective in handling data with categorical and numerical features, and they tend to generalize well while mitigating overfitting. 

# Features

 ## Data Preprocessing:

  Imputation: Handles missing values in the Age column by replacing them with the mean age.
  
  Encoding: Converts categorical features (Sex and Embarked) into numerical format using OneHotEncoder.
  
  Feature Dropping: Removes unnecessary features (Embarked, Name, Ticket, Cabin, Sex).
  
  Stratified Sampling: Ensures that the training and test sets have similar distributions of the target variable (Survived) and important categorical features (Pclass, Sex).

  Scaling: Standardizes the feature values to have a mean of 0 and a standard deviation of 1.

  After completing the data processing, a Pipeline was created to streamline and automate the preprocessing steps.

  ## Modeling:

  Uses a RandomForestClassifier for prediction.
  
  Utilizes GridSearchCV for hyperparameter optimization to find the best model parameters.
  
  Evaluates model performance on both training and test sets to ensure generalization.


  

