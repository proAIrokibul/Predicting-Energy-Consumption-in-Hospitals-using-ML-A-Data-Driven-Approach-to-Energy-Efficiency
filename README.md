# Predicting-Energy-Consumption-in-Hospitals-using-ML-A-Data-Driven-Approach-to-Energy-Efficiency
## Project Overview
This project focuses on predicting the "AI Predicted Health Status" of individuals based on various environmental and physiological parameters. The dataset includes numerical features such as temperature, humidity, oxygen levels, heart rate, and power usage metrics, along with categorical features like energy source, HVAC mode, and season. 

## Business Impact
Accurate health status predictions can have significant implications in various industries, including healthcare, energy management, and smart building systems. Predictive insights from this model can help in:
- Enhancing proactive patient monitoring and reducing emergency incidents.
- Optimizing energy consumption in smart hospitals by aligning HVAC usage with patient health conditions.
- Improving resource allocation for better operational efficiency.

## Data Preprocessing & Feature Engineering
- Converted timestamp to datetime format and extracted hour and month features.
- Encoded categorical features appropriately.
- Handled missing values and performed outlier detection.
- Scaled numerical features using standardization techniques.

## Exploratory Data Analysis (EDA)
- Distribution plots of numerical features.
- Correlation heatmaps to identify relationships between features.
- Count plots for categorical features.
- Feature importance analysis after modeling.

## Machine Learning Models & Performance
### Initial Model Performance
#### Random Forest
- **Accuracy:** 0.5035
- **Precision/Recall/F1-score:**
  - Class 0: Precision: 0.51, Recall: 0.52, F1-score: 0.52
  - Class 1: Precision: 0.49, Recall: 0.49, F1-score: 0.49

#### XGBoost
- **Accuracy:** 0.511
- **Precision/Recall/F1-score:**
  - Class 0: Precision: 0.52, Recall: 0.50, F1-score: 0.51
  - Class 1: Precision: 0.50, Recall: 0.52, F1-score: 0.51

#### Neural Network
- **Accuracy:** 0.488
- **Precision/Recall/F1-score:**
  - Class 0: Precision: 0.49, Recall: 0.04, F1-score: 0.08
  - Class 1: Precision: 0.49, Recall: 0.96, F1-score: 0.65

## Model Tuning & Optimization
Hyperparameter tuning was performed using Optuna for XGBoost and Random Forest to improve accuracy and reduce overfitting.

### Final Model Performance After Hyperparameter Tuning
#### XGBoost
- **Train Accuracy:** 0.9066
- **Test Accuracy:** 0.8180

#### Random Forest
- **Train Accuracy:** 0.7256
- **Test Accuracy:** 0.6810

## Conclusion
- XGBoost outperformed other models after tuning, achieving an 81.8% accuracy on the test set.
- Random Forest showed a decent improvement post-tuning but still lagged behind XGBoost.
- Feature importance visualization highlighted key factors influencing predictions.
- The insights from this project can help in developing better AI-driven health monitoring systems and optimizing energy consumption in healthcare facilities.

