# Rock vs Mine Classification

### 🔍 Problem Statement:
The goal of this project is to classify sonar signals as either rocks or mines using a Logistic Regression model. Each data sample contains 60 numerical features representing sonar signal strength at different frequencies.

### 📊 Dataset:
- **Features**: 60 continuous values
- **Labels**: 'R' (Rock) or 'M' (Mine)

### 📁 Workflow:
1. **Data Loading**
   - Loaded the dataset into a Pandas DataFrame.

2. **Data Exploration**
   - Used `.shape` to check dimensions.
   - Used `.value_counts()` to examine the label distribution.
   - Found the dataset to be nearly balanced between 'R' and 'M'.

3. **Data Preparation**
   - Separated the features and the target label.
   - Did **not** use label encoding — used the labels as-is.

4. **Train-Test Split**
   - Split the data into training and testing sets (80% train, 20% test).

5. **Model Building**
   - Used **Logistic Regression** from `sklearn.linear_model` to train the model.

6. **Model Evaluation**
   - Calculated and printed the accuracy on both training and test data.

7. **Predictive System**
   - Built a simple system to classify new data inputs.
   - If the model predicts 'R', the output is: **"The object is a Rock."**
   - If the model predicts 'M', the output is: **"The object is a Mine."**

### 📦 Libraries Used:
- Pandas
- NumPy
- Scikit-learn

### ✅ Outcome:
- Successfully built a binary classification system.
- Achieved reliable accuracy due to a balanced dataset and a straightforward model.
- Demonstrated the end-to-end ML workflow from loading data to deploying a basic prediction system.
