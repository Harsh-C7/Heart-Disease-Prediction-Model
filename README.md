## Heart Disease Prediction Model 

This project demonstrates a machine learning approach to predict the presence of heart disease using a dataset of patient health metrics. The code utilizes Python's [`pandas`](https://pandas.pydata.org/) for data manipulation, [`numpy`](https://numpy.org/) for numerical operations, and [`scikit-learn`](https://scikit-learn.org/stable/) for building and evaluating the machine learning model.

### Dataset
The dataset used is `heart_disease_data.csv`, which contains various health-related attributes of patients, including the target variable indicating the presence or absence of heart disease.

### Key Steps in the Code

1. **Data Loading and Exploration:**
   - The dataset is loaded using `pandas` and initial exploration is performed using `head()`, `shape`, and `describe()` methods to understand the structure and summary statistics of the data.
   - Missing values are checked using `isnull().sum()`.

2. **Data Preparation:**
   - Features (`x`) and target (`y`) variables are separated. The target variable is the "target" column, which indicates the presence of heart disease.
   - The dataset is split into training and testing sets using `train_test_split` with a stratified sampling approach to maintain the distribution of the target variable.

3. **Model Training:**
   - A `LogisticRegression` model is instantiated and trained on the training data (`x_train`, `y_train`) with a maximum iteration of 1000 to ensure convergence.

4. **Model Evaluation:**
   - The accuracy of the model is evaluated on both the training and testing datasets, providing insights into the model's performance and potential overfitting.

5. **Prediction:**
   - An example input data point is provided to demonstrate how the trained model can predict the presence of heart disease. The prediction is made using the `predict` method, and the result is interpreted to indicate whether the person has heart disease or not.

### Output
- The code outputs the accuracy of 85% on training dataset and 80% on testing dataset from the model.
- It also provides a prediction for a sample input, indicating whether the individual has heart disease.

This project serves as a basic example of using logistic regression for binary classification tasks in healthcare analytics.        
