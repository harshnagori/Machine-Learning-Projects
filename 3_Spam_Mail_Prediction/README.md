# 📧 Spam Mail Prediction

### 🔍 Problem Statement:
The goal of this project is to classify email messages as either **spam** or **ham** (not spam) using a Logistic Regression model. The input is raw email text which is processed and transformed into numerical vectors using TF-IDF for effective classification.

### 📊 Dataset:
- **Features**: Raw email text messages
- **Labels**: `0` for Spam, `1` for Ham

### 📁 Workflow:
1. **Data Loading**
   - Loaded the dataset using Pandas.

2. **Data Exploration**
   - Used `.shape`, `.head()` to explore and clean data.
   - Replaced null values with empty strings.

3. **Data Preparation**
   - Applied **label encoding**: `spam → 0`, `ham → 1`.
   - Separated features and target labels.
   - Split into training and testing sets (80% train, 20% test).

4. **Feature Extraction**
   - Used **TfidfVectorizer** with the following:
     - `min_df=1`
     - `stop_words='english'`
     - `lowercase=True`

5. **Model Building**
   - Trained a **Logistic Regression** classifier from `sklearn.linear_model`.

6. **Model Evaluation**
   - Calculated and printed accuracy for both training and test data.

7. **Predictive System**
   - Built a system to classify new email messages.
   - Output:
     - If `0`: **"This is a Spam mail."**
     - If `1`: **"This is a Ham mail."**

### 📦 Libraries Used:
- Pandas
- Scikit-learn
- Numpy

### ✅ Outcome:
- Successfully built a spam detection model using text vectorization and logistic regression.
- Achieved good performance and implemented a working predictive system.
