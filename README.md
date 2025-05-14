# Heart Disease Predictor

## Project Overview
This project is aimed at predicting the presence of heart disease using the Cleveland Heart Disease dataset. The objective was to analyze the dataset and build a robust machine learning model for classification. The Random Forest algorithm was used as the primary model, achieving an impressive accuracy of 81%. The K-Nearest Neighbors (KNN) algorithm was also implemented for comparison purposes.

## Dataset
**Source:** Cleveland Heart Disease Dataset

The dataset contains several features related to patient health and medical diagnostics, including:
- **Age**
- **Gender**
- **Chest Pain Type (CP)**
- **Resting Blood Pressure (Trestbps)**
- **Serum Cholesterol (Chol)**
- **Fasting Blood Sugar (FBS)**
- **Resting Electrocardiographic Results (Restecg)**
- **Maximum Heart Rate Achieved (Thalach)**
- **Exercise-Induced Angina (Exang)**
- **ST Depression Induced by Exercise Relative to Rest (Oldpeak)**
- **Slope of the Peak Exercise ST Segment (Slope)**
- **Number of Major Vessels Colored by Fluoroscopy (Ca)**
- **Thalassemia (Thal)**

The target variable is a binary indicator of the presence or absence of heart disease.

## Tools and Technologies
**Programming Language:** Python

**Libraries Used:**
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Data Preprocessing
### Data Cleaning:
- Checked for missing values and handled them appropriately.
- Normalized continuous variables to bring them into a similar range.

### Feature Selection:
- Analyzed feature importance using correlation heatmaps.
- Retained features with significant predictive power.

### Data Splitting:
- The dataset was split into training and testing sets (80%-20% ratio).

## Random Forest Algorithm Implementation
### Model Selection:
- Random Forest was chosen for its robustness and ability to handle complex datasets with high dimensionality.

### Hyperparameter Tuning:
- Grid search and cross-validation were used to optimize hyperparameters such as the number of estimators, maximum depth, and minimum samples split.

### Model Training:
- Trained the Random Forest classifier on the training dataset.

### Feature Importance:
- The model provided insights into the importance of each feature, helping to understand their contribution to predictions.

### Performance Metrics:
- **Accuracy:** 81%
- Precision, Recall, and F1-score metrics were evaluated to ensure robustness.

## Key Results
- **Confusion Matrix:** A confusion matrix was plotted to visualize true positives, true negatives, false positives, and false negatives.
- **Receiver Operating Characteristic (ROC) Curve:** Demonstrated a high area under the curve (AUC), indicating excellent model performance.

## Comparison with KNN Algorithm
For benchmarking, the Random Forest model was compared with the KNN algorithm. While KNN achieved commendable accuracy, Random Forest outperformed it in terms of overall performance and feature interpretability.

## Visualizations
Several plots were generated for data analysis and model evaluation:
- Pairplots to identify relationships between features.
- Correlation heatmap to select relevant features.
- Feature importance bar chart to identify the most impactful variables.
- ROC curve to evaluate classifier performance.

## Conclusion
The project successfully built a predictive model for heart disease using the Cleveland dataset. The Random Forest algorithm proved to be the best-performing model for this classification task, achieving significant accuracy and offering valuable insights into feature importance.

## Future Scope
- Explore ensemble methods like Gradient Boosting or XGBoost to further improve accuracy.
- Extend the study to include more comprehensive datasets for better generalization.
- Deploy the model as a web application for real-time heart disease prediction.

## How to Run the Project
1. Clone this repository.
2. Install the required dependencies using:
   ```bash
   pip install -r requirements.txt
