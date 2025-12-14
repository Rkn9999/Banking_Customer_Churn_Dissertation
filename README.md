# Banking_Customer_Churn_Dissertation

# Project Title
Evaluating Machine Learning Models for Banking Customer Churn Prediction

# Project Overview
This project focuses on predicting customer churn in the banking sector using supervised machine learning techniques. Customer churn refers to customers who discontinue their relationship with a bank. Since customer retention is critical for profitability and long-term sustainability, this study evaluates multiple machine learning models to identify customers who are at high risk of leaving. The work is part of an MSc dissertation in Big Data Analytics submitted to Sheffield Hallam University.

# Dataset Description
The study uses a publicly available banking customer churn dataset sourced from Kaggle. The dataset contains 10,000 customer records with demographic, financial, and behavioural attributes such as age, credit score, account balance, tenure, number of products, activity status, and estimated salary. The target variable is Exited, which indicates whether a customer has churned or not. The dataset is moderately imbalanced, with fewer churned customers compared to retained customers, reflecting real-world banking scenarios.

# Data Preprocessing
Several preprocessing steps were applied to prepare the dataset for machine learning. Non-informative identifiers such as customer ID, row number, and surname were removed to avoid noise and data leakage. Categorical variables such as gender and geography were encoded into numerical format to make them suitable for machine learning algorithms. Feature scaling was applied using standardisation to ensure that numerical variables were on a comparable scale, which is especially important for distance-based and gradient-based models.

# Handling Class Imbalance
Customer churn datasets are typically imbalanced, which can bias models toward predicting non-churn customers. To address this issue, the Synthetic Minority Oversampling Technique was applied to the training data. SMOTE generates synthetic samples for the minority churn class, enabling models to learn churn patterns more effectively. This approach improves recall and F1-score for churn prediction without altering the test dataset.

# Machine Learning Models Used
The project evaluates five supervised machine learning models. Logistic Regression is used as a baseline due to its simplicity and interpretability. K-Nearest Neighbours is included as a distance-based model that classifies customers based on similarity. Random Forest is used as an ensemble model that improves robustness and reduces overfitting. Gradient Boosting is applied to capture complex non-linear relationships by sequentially improving weak learners. Extreme Gradient Boosting is included as an optimised boosting model with regularisation and efficient computation.

# Model Evaluation
Model performance is evaluated using multiple metrics to account for class imbalance. Accuracy is used to measure overall correctness. Precision and recall assess how well churn customers are identified. F1-score is used to balance precision and recall. Macro-averaged F1-score treats each class equally, while weighted F1-score accounts for class distribution. The Area Under the Receiver Operating Characteristic Curve is used to evaluate the model’s ability to distinguish between churned and non-churned customers.

# Key Findings
The experimental results show that ensemble-based models outperform traditional models in predicting banking customer churn. Gradient Boosting achieved the best overall performance, with high accuracy, balanced F1-scores, and strong AUC-ROC values. The findings confirm that advanced ensemble techniques are more effective in capturing complex behavioural and financial patterns associated with churn.

# Practical Implications
The results of this project can support banks in developing data-driven customer retention strategies. By identifying high-risk customers early, banks can design targeted interventions such as personalised offers, improved digital services, and proactive customer engagement. The study also highlights the importance of handling class imbalance and using appropriate evaluation metrics in real-world churn prediction systems.

# How to Use This Project
This project can be used as a reference for academic research, coursework, or applied analytics in customer churn prediction. The methodology and modelling framework can be extended to other financial or service-based industries with similar churn problems. The structure is suitable for replication and further experimentation with additional datasets or advanced explainable AI techniques.

# Ethical Considerations
The dataset used in this project is publicly available and contains no confidential or personally identifiable information. All analysis follows ethical data usage principles and aligns with responsible AI practices. The models are intended to support decision-making and not replace human judgement in customer management.

Author
Rama Krishna Nandamuri
MSc Big Data Analytics
Sheffield Hallam University
