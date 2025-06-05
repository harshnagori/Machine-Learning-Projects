# Diabetes Prediction

### 🔍 Problem Statement:
The objective of this project is to predict whether a person is diabetic or not based on health-related features using a **Support Vector Machine (SVM)** classifier with a linear kernel.

### 📊 Dataset:
- **Source**: PIMA Diabetes Dataset
- **Features**: Medical attributes like glucose level, BMI, insulin, pregnancies, age, etc.
- **Labels**: `0` (Non-Diabetic), `1` (Diabetic)

### 📁 Workflow:
1. **Data Loading**
   - Loaded the dataset into a Pandas DataFrame.

2. **Data Exploration**
   - Checked dataset structure using `.shape`, `.head()`, and `.describe()`.

3. **Data Preparation**
   - Separated the features and target labels.
   - Standardized the features using `StandardScaler` for better model performance.

4. **Train-Test Split**
   - Split the dataset into training and testing sets (80% training, 20% testing).

5. **Model Building**
   - Used **SVM Classifier** from `sklearn.svm` with a linear kernel:
     ```python
     svm.SVC(kernel='linear')
     ```

6. **Model Evaluation**
   - Evaluated the model using `accuracy_score` on both training and testing datasets.

7. **Predictive System**
   - Built a system to classify new data instances.
   - If the prediction is `1`, the output is: **"The person is diabetic."**
   - If the prediction is `0`, the output is: **"The person is not diabetic."**

### 📦 Libraries Used:
- Pandas
- NumPy
- Scikit-learn

### ✅ Outcome:
- Successfully developed a binary classification system for diabetes prediction.
- Achieved strong accuracy using a linear SVM.
- Demonstrated a complete ML pipeline: from data preprocessing to deployment of a simple predictive tool.
