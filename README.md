# credit-risk-classification
to train and evaluate a model based on loan risk. 

### Overview of the Analysis:
The purpose of the analysis was to develop and train machine learning models to assess credit risk and predict the creditworthiness of clients applying for loans. The analysis aimed to identify potential high-risk loans that are likely to default and distinguish them from healthy loans that are expected to be repaid. By accurately predicting credit risk, financial institutions can make informed decisions on loan approvals, minimizing the risk of financial losses and optimizing profitability. The analysis aimed to leverage historical lending data to build models that can effectively classify loan applicants and provide insights for risk assessment in the lending process.

#### Data:
The model utilized lending data, including loan size, interest rate, client income, total debt, debt-to-income ratio, number of accounts, and prior account flags. The loan status, indicating healthy (0) or high-risk (1), was used as the target variable.

#### Preprocessing:
After loading and reviewing the lending_data.csv, the data was divided into features (X) and labels (y). The label balance was checked using value_counts to determine the distribution of healthy loans and high-risk loans. The data was then split into training (X_train, y_train) and testing (X_test, y_test) sets using train_test_split.

#### Modeling and Evaluation:
A logistic regression model was trained using the original training data and used to predict labels for the test data (X_test). The model's performance was evaluated by calculating the balanced accuracy score, generating a confusion matrix, and printing a classification report to assess precision, recall, and F1 scores for both healthy loans and high-risk loans.

#### Results:
Machine Learning Model 1:

  - Balanced Accuracy Score: 99.24%
  - Precision for Healthy Loans: 100%
  - Precision for High-Risk Loans: 87%
  - Recall for Healthy Loans: 100%
  - Recall for High-Risk Loans: 89%
  - Machine Learning Model 2:

Balanced Accuracy Score: 99.52%
  - Precision for Healthy Loans: 100%
  - Precision for High-Risk Loans: 87%
  - Recall for Healthy Loans: 100%
  - Recall for High-Risk Loans: 100%

#### Summary:
Based on the results, both machine learning models performed well in predicting healthy loans, achieving a balanced accuracy score of over 99% and perfect precision and recall. However, the models showed some limitations in accurately identifying high-risk loans. Model 1 had a lower recall rate (89%) for high-risk loans, while Model 2 achieved a perfect recall rate (100%) for this category.

Considering the goal of the analysis and the risks involved, accurately identifying high-risk loans is crucial to minimize potential losses. Therefore, Model 2, which exhibited better recall for high-risk loans, is recommended for credit risk assessment. Although both models had the same precision score for high-risk loans, the improved recall of Model 2 ensures that no high-risk loans are left unidentified, reducing the risk of approving loans to clients likely to default.

In conclusion, Model 2 outperformed Model 1 in terms of recall for high-risk loans, making it the preferred choice for credit risk assessment. However, it is important to note that the selection of the model depends on the specific problem and priorities.
