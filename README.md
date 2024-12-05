# Weather Prediction with Machine Learning

This repository contains a project for building and evaluating machine learning models to predict whether it will rain tomorrow based on historical weather data. The project uses a dataset for training and validation, and the results are submitted to a Kaggle competition.

---

## Project Structure

1. **Dataset Introduction**  
   - The dataset `train-val.csv` is loaded and explored for training and validation.
   - A separate test set is used for Kaggle submission.

2. **Exploratory Data Analysis (EDA)**  
   - Understanding the dataset structure, including:
     - Number of samples and features.
     - Data types of each feature.
     - Distribution of samples across categories.
     - Correlation analysis and other key insights.
   - The results of EDA guide preprocessing and model training.

3. **Dataset Preprocessing**  
   - Handled missing values.
   - Encoded categorical variables for compatibility with machine learning models.
   - Scaled features where necessary.
   - Used `ColumnTransformer` for streamlined preprocessing.

4. **Model Training**  
   - Trained seven classifiers using default hyperparameters:
     1. Naive Bayes
     2. KNeighborsClassifier
     3. Logistic Regression
     4. Multi-Layer Perceptron (MLP) with one hidden layer
     5. Support Vector Classifier (SVC)
     6. Decision Tree
     7. Random Forest
   - Evaluated models using F1 Score and selected the best-performing model.

5. **Model Optimization**  
   - Performed hyperparameter tuning using Grid Search with 5-fold cross-validation.
   - Compared models after tuning and re-evaluated their performance.

6. **Kaggle Submission**  
   - Predictions from the best model were saved in the required format:
     - A column for `id` from the test set.
     - A column for predicted values.

