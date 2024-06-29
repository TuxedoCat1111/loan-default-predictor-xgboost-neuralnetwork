## Loan Default Predictor

Data source: https://www.kaggle.com/datasets/laotse/credit-risk-dataset


**Overview**

This project involves the development of a predictive model to determine the likelihood of a loan applicant defaulting on their loan. The model is built using various machine learning classification algorithms, e.g XGBoost and a neural network, and is evaluated on multiple performance metrics such as precision, recall, specificity, and F1 score.



**Business Problem**

In the financial industry, particularly for banks and lending institutions, loan defaults represent a significant risk. The ability to accurately predict the likelihood of a borrower defaulting on a loan can help mitigate this risk. An effective loan default prediction model can assist in:

- Risk Management: Identifying high-risk applicants allows institutions to take proactive measures, such as adjusting interest rates, requesting additional collateral, or rejecting the application altogether.
- Customer Retention: By understanding the risk profile of borrowers, banks can offer tailored products that suit the customer's financial situation, improving customer satisfaction and loyalty.
- Operational Efficiency: Automating the risk assessment process reduces the manual effort required by loan officers, speeding up the loan approval process and reducing operational costs.
- Regulatory Compliance: Ensuring that the institution adheres to regulatory standards by maintaining a balanced and risk-aware lending portfolio.


**Real-World Applications**

The loan default predictor model can be applied in several real-world scenarios:

- Credit Scoring: Enhance traditional credit scoring methods by incorporating machine learning predictions to provide a more comprehensive risk assessment.
- Fraud Detection: Identify potential fraudulent applications by detecting anomalies and unusual patterns in the applicant's data.
- Portfolio Management: Maintain a balanced loan portfolio by continuously monitoring the risk levels and adjusting strategies accordingly.
- Personalized Lending: Offer personalized loan products based on the applicant's risk profile, improving both acceptance rates and customer satisfaction.


**Data Preprocessing**

The data preprocessing steps included:
- Handling missing values
- Encoding categorial variables
- Scaling (numerical features were normalized using MinMaxScalar
- Balancing the training and testing dataset to have a similar distribution of the target variable (to avoid bias).


**Model Development**

Multiple machine learning models were developed and evaluated, including:
- XGBoost: A powerful gradient boosting algorithm optimized using GridSearchCV to find the best hyperparameters.
- Neural Networks: Built using Keras and TensorFlow, with dropout layers and early stopping to prevent overfitting.
- Other Models: Logistic Regression, K-Nearest Neighbors (KNN), LightGBM, and CatBoost for comparison purposes.


**Evaluation Metrics**

The models were evaluated using several metrics:

Precision: The ability of the model to correctly identify non defaulting applicants.
Recall: The ability of the model to capture all non defaulting applicants.
Specificity: The ability of the model to correctly identify defaulting applicants.
F1 Score: The harmonic mean of precision and recall, providing a balance between the two.


**Results**

By focusing on maximizing recall, the best-performing model was the neural network which achieved recall of 99.23% and precision of 92%.
The XGBoost classifier, after tuning, also preformed very well and achieved recall of 98.98% and precision of 92.51%.


**Conclusion**

The loan default predictor model demonstrates strong predictive capabilities and can be a valuable tool for financial institutions to manage loan risk effectively. By integrating this model into their decision-making processes, lenders can reduce default rates, improve operational efficiency, and enhance customer satisfaction.


**Future Work**

Future improvements and extensions to this project could include:
- Feature Importance Analysis: identifying and analyzing the most significant features contributing to loan default predictions.
- Ensemble Methods: combining multiple models to improve overall performance.
- Real-Time Predictions
