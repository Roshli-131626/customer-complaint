# customer-complaint
In this project, we set out to predict the outcome of credit report complaints based on various features such as product type, sub-issue, company, state, response time, and more. The goal is to classify the complaints into categories based on the company’s response.

### Project Description

In this project, we set out to predict the outcome of credit report complaints based on various features such as product type, sub-issue, company, state, response time, and more. The goal is to classify the complaints into categories based on the company’s response (e.g., "Closed with explanation," "Closed with non-monetary relief," "In progress," etc.). This analysis is valuable for understanding patterns in complaint handling and potentially improving customer service processes.

### Project Workflow

1. **Data Collection and Preparation**:
    - **Data Loading**: The dataset provided consists of credit report complaints, including features such as product type, issue, sub-issue, company, state, and more.
    - **Data Cleaning**: This involves handling missing values, correcting data types, and potentially dealing with imbalanced classes.
    - **Text Preprocessing**: The textual data (such as issue descriptions) is cleaned, tokenized, and converted into numerical form using methods like TF-IDF.

2. **Exploratory Data Analysis (EDA)**:
    - **Visualization**: We explored the distribution of various features such as product type, company responses, and geographic distribution of complaints. 
    - **Correlation Analysis**: Identified relationships between features and the target variable.

3. **Feature Engineering**:
    - **Vectorization**: Textual data was converted into numerical format using TF-IDF.
    - **Categorical Encoding**: Features like "Product," "Sub-issue," and "Company" were encoded into numerical values.
    - **Dimensionality Reduction**: Techniques like PCA could be applied to reduce feature space and improve model efficiency.

4. **Model Selection and Training**:
    - **Models Used**: We trained and evaluated several models including:
        - Naive Bayes
        - Support Vector Machine (SVM)
        - Random Forest
        - Logistic Regression
        - K-Nearest Neighbors
        - Decision Tree
        - Gradient Boosting
        - AdaBoost
        - Ridge Classifier
        - MLP Classifier
        - Extra Trees
        - Bagging
        - Voting Classifier
        - SGD Classifier
    - **Evaluation**: Each model was evaluated using accuracy, precision, recall, F1-score, and ROC-AUC score.
    - **Model Comparison**: The models were compared to select the best-performing one.

5. **Model Explanation**:
    - **SHAP**: Used SHAP (SHapley Additive exPlanations) to interpret the best-performing model's predictions and understand feature importance.
    - **LIME**: Attempted to use LIME (Local Interpretable Model-agnostic Explanations) to further interpret the model predictions, though there were technical difficulties with visualization.

6. **Final Model Selection and Evaluation**:
    - **Best Model**: The best-performing model was selected based on the evaluation metrics. 
    - **Detailed Evaluation**: A final evaluation was conducted, including classification reports and confusion matrices to understand the model's performance on the test set.

### Achievements and Insights

- **Accurate Prediction**: The model was able to predict the outcome of credit report complaints with a high degree of accuracy, potentially helping companies to better manage their response strategies.
- **Feature Importance**: Through SHAP, we identified key features that influence the model’s predictions, providing insights into what factors are most critical in determining complaint outcomes.
- **Model Interpretability**: Although there were challenges with LIME, the use of SHAP allowed for an interpretable model, giving us confidence in the decisions made by the model.

### Visualizations and Insights

- **Data Distribution**: Bar charts, histograms, and box plots were used to visualize the distribution of complaints across different products and companies.
- **Model Performance**: ROC curves and confusion matrices provided insights into model performance.
- **Feature Importance**: SHAP plots highlighted the most important features driving model decisions.

### Challenges

- **Computational Resources**: The SHAP explainer was computationally expensive, causing delays in processing.
- **Visualization Issues**: LIME did not produce the expected visualizations, which limited our ability to interpret model predictions in a user-friendly manner.

This project highlights the practical application of machine learning and NLP techniques in real-world scenarios, demonstrating how predictive modeling can assist in better understanding and managing customer complaints in the financial industry.
