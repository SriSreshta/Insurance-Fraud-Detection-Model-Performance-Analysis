# Insurance Fraud Detection & Model Performance Analysis

## 📌 Project Overview
This project focuses on detecting fraudulent insurance claims using four distinct **machine learning models**. The core of the project is to not only train these models but to then visually compare their predictive performance in a clear and interactive **Tableau** visualization.

The workflow was divided into two main stages:

1.  **Model Training & Evaluation (Python)**
    - Preprocessed raw insurance claim data, handling categorical features and missing values.
    - Trained four classifier models: **Random Forest, AdaBoost, XGBoost, and CatBoost**.
    - Generated predictions from each model on a holdout test set.

2.  **Comparative Visualization (Tableau)**
    - Exported the actual outcomes and the predictions from all four models to a CSV file.
    - Created a comparative Tableau visualization to analyze the performance of each model side-by-side using **confusion matrix heatmaps**.

---

## ⚙️ Machine Learning Pipeline
### Data Preprocessing
- Handled missing values and encoded categorical variables using one-hot encoding.
- Dropped unique identifier columns (`policy_number`, etc.) to prevent data leakage during training.
- Split the dataset into **training (80%)** and **testing (20%)** sets to ensure a fair evaluation.

### Models Trained
- **Random Forest Classifier**
- **AdaBoost Classifier**
- **XGBoost Classifier**
- **CatBoost Classifier**

> ✅ The final predictions from all four models were exported to a single file for a direct head-to-head comparison in Tableau.

---

## 📊 Tableau Visualization
To make the model performance results **interpretable and easy to compare**, the predictions were visualized in Tableau. The dashboard focuses on one key component:

### Comparative Confusion Matrix Heatmap
A single, powerful visualization that places the confusion matrix for each of the four models side-by-side. This allows for an at-a-glance assessment of:

- **True Positives:** Which model was best at correctly identifying actual fraud?
- **False Positives:** Which model raised the fewest false alarms?
- **Overall Accuracy:** The balance between correctly identifying fraud and non-fraud cases.

### Interactivity
- **Tooltips:** Hovering over any cell in the heatmaps reveals the exact count and model name, allowing for detailed inspection of performance metrics.
- **Filtering:** The view can be easily filtered to isolate and analyze the performance of a single model.

