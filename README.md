
# Data Preprocessing, Model Building, and Prediction Analysis

## Dataset
The project utilizes the **Bank Marketing Dataset**, which records the outcomes of Portuguese bank marketing campaigns. It includes customer demographics, financial information, and campaign details. The target variable (`deposit`) indicates whether the client subscribed to a term deposit.

---

## Tasks Overview

### Step 01: Loading Important Libraries
Essential Python libraries like `pandas`, `numpy`, `matplotlib`, and machine learning utilities from `scikit-learn` are imported.

### Step 02: Loading Dataset
The dataset is loaded using `pandas.read_csv()`.

### Step 03: Exploring the Dataset
Key actions:
- Display first and last rows.
- Check dataset dimensions, columns, datatypes, and missing values.

### Step 04: Generating Summary Statistics
Statistical insights are generated to understand the numerical distribution.

### Step 05: Data Preprocessing
Includes:
1. Filling missing values using mode.
2. Encoding categorical variables with `LabelEncoder`.
3. Standardizing numerical columns using `StandardScaler`.

### Step 06: Feature Selection
Techniques used:
- Correlation heatmap to explore relationships.
- Mutual information to rank features.
- Selecting top 5 impactful features using `SelectKBest`.

### Step 07: Model Training
Models trained:
1. **Logistic Regression**
2. **Decision Tree**
3. **Random Forest**

Techniques:
- Train-test split.
- Cross-validation (5-fold) for performance evaluation.

### Step 08: Feature Importance Analysis
Identified top features impacting campaign success:
1. `Duration`
2. `Balance`
3. `Pdays`
4. `Previous`
5. `Poutcome`

### Step 09: Model Evaluation
Performance metrics include:
- Accuracy, Precision, Recall, F1-score.
- Models compared for predictive efficiency.

---

## How to Run the Code

1. **Install Dependencies**
   Install Python libraries using:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

2. **Place the Dataset**
   Ensure the dataset file (`bank_marketing_dataset.csv`) is in the same directory as the code.

3. **Run the Script**
   Execute the Python script in an IDE or terminal:
   ```bash
   python project_script.py
   ```

4. **Inspect Outputs**
   View:
   - Preprocessing logs in the console.
   - Visualizations (e.g., heatmaps).
   - Model evaluation results for Logistic Regression, Decision Tree and Random Forest.

---

## Conclusion
This project guides through preprocessing, feature selection, and model training for a real-world bank marketing dataset. Insights highlight the importance of targeted features like `duration` and `balance` in predicting campaign success.
