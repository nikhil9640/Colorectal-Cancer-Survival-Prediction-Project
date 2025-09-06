# Colorectal-Cancer-Survival-Prediction-Project
Colorectal cancer (CRC) is one of the leading causes of cancer-related deaths worldwide. Predicting survival outcomes based on patient demographics, medical history, lifestyle factors and treatment details can support clinicians in decision-making and help identify high-risk groups.

# Objective
Machine learning models offer the potential to uncover hidden patterns in patient data and improve prognostic accuracy compared to traditional statistical approaches.
The primary goal of this project is to predict the survival status of colorectal cancer patients using clinical, demographic, and lifestyle features.
Specifically, the project aims to:
1. Explore and preprocess patient data.
2. Identify key risk factors and predictors of survival.
3. Train classification models to predict survival status.
4. Evaluate model performance using accuracy and classification metrics.

# Methodology
1. Load dataset
2. Exploratory Data Analysis (basic prints + plots)
3. Data preprocessing (imputation, one-hot encoding, scaling)
4. Feature selection (Logistic coef + permutation importance)
5. Model training (Logistic Regression)
6. Evaluation (accuracy, classification report, confusion matrix)
7. Save artifacts (trained pipeline, feature importance CSVs, plots)

# Drawbacks/Limitations
The dataset may not be fully representative (regional or hospital bias).
Missing clinical details (tumor genetics, comorbidities) could reduce predictive power.
Logistic regression assumes linearity between predictors and outcome.
Survival was treated as a binary classification (alive vs deceased), while real survival is time-to-event, better suited for survival analysis methods (Cox regression, Kaplan-Meier, etc.).

# Models Used
**1. Logistic Regression**
Baseline interpretable model.
Provides coefficients to understand feature influence.
**2. (Optional Extension:** Random Forest / Gradient Boosting)
Can handle nonlinear interactions.
Often improves prediction accuracy but is less interpretable.

# Conclusion
This project demonstrates the feasibility of applying machine learning to predict colorectal cancer survival outcomes.
Logistic Regression provided an interpretable baseline, highlighting important predictors such as stage, treatment, and lifestyle factors.

**Future work could include:**
Using ensemble models (Random Forest, XGBoost) for improved accuracy.
Applying time-to-event survival models for more clinically relevant predictions.
Incorporating larger and more diverse patient datasets.
Ultimately, such predictive models can act as decision-support tools to guide clinicians and patients toward personalized cancer management strategies.
