# 🏦 Loan Approval Prediction using Random Forest

This project builds a **classification model** to predict whether a loan application will be **approved** or **rejected**, based on applicant data. The model uses a **Random Forest Classifier** and evaluates its performance using **accuracy**, **classification report**, and **confusion matrix**.

---

## 📁 Dataset

- **File**: `train.csv`  
- The dataset includes features such as:
  - `Gender`, `Married`, `Dependents`, `Education`, `Self_Employed`
  - `ApplicantIncome`, `CoapplicantIncome`, `LoanAmount`, `Loan_Amount_Term`
  - `Credit_History`, `Property_Area`, `Loan_Status`

---

## 🧰 Libraries Used

- `pandas`, `numpy` — for data manipulation
- `matplotlib`, `seaborn` — for visualizations
- `sklearn` — for preprocessing, model building, and evaluation

---

## 🔍 Workflow

### 1. **Load Dataset**
- Read `train.csv` using `pandas`.

### 2. **Data Cleaning**
- Handle missing values using mode or median.
- Drop `Loan_ID` (not a predictive feature).

### 3. **Data Encoding**
- Label encode categorical variables like `Gender`, `Married`, `Education`, etc.
- Convert `Dependents` to integer, replacing `'3+'` with `3`.

### 4. **Train-Test Split**
- Split data into 80% training and 20% testing using `train_test_split`.

### 5. **Feature Scaling**
- Normalize features using `StandardScaler` for better model performance.

### 6. **Model Training**
- Use `RandomForestClassifier` with 100 estimators.

### 7. **Model Evaluation**
- Evaluate using:
  - **Accuracy score**
  - **Classification report** (precision, recall, F1-score)
  - **Confusion matrix heatmap**

### 8. **Prediction Display**
- Display predicted vs actual outcomes with prediction probabilities.

---

## ✅ Sample Output

- **Accuracy**: e.g., `~80%+`
- **Classification Report**: shows precision, recall, F1-score for approval/rejection.
- **Confusion Matrix**: visual overview of correct/incorrect predictions.
- **Prediction Table**
## 💻 How to Run

1. Install dependencies:
 pip install pandas numpy matplotlib seaborn scikit-learn
Place the train.csv file in your working directory.

Update the file path if necessary in the code:
df = pd.read_csv(r'C:\Path\To\Your\train.csv')
Run the full script in a Jupyter Notebook or Python IDE.


