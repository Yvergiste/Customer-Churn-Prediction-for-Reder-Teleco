# Customer-Churn-Prediction-for-Reder-Telecom
# Title: Customer Churn Prediction for Reder Telecom
## Objective:
The primary objective of this project is to develop a machine learning model to predict customer churn for Reder Telecom. By identifying customers at risk of leaving, the company can take proactive measures to retain them and reduce churn rates.
## Dataset:
The dataset contains customer-related information, including demographics, subscription details, engagement metrics, service interactions, payment history, and marketing communication data. Key features include:
- Demographics: Age, Gender
- Subscription Details: SubscriptionPlan, SubscriptionDuration
- Engagement Metrics: WebsitePageViews, WebsiteTimeSpent, EngagementMetricsLogins, EngagementMetricsFrequency
- Service Interactions: ServiceInteractions_Call, ServiceInteractions_Email, ServiceInteractions_Chat
- Payment History: PaymentHistoryNoOfLatePayments
- Marketing Communication: MarketingCommunicationNoOfEmails, MarketingCommunicationOpenClickDiff, MarketingCommunicationSentOpenDiff
- Feedback: Net Promoter Score (NPS), FeedbackRating
- Clickstream Data: ClickstreamData_Click, ClickstreamData_Add to Cart, ClickstreamData_Search
- Purchase Details: PurchasedFrequency, PurchasedValue
## Methodology:
1.	Data Preprocessing: Cleaning the dataset, handling missing values, and encoding categorical variables.
- Gender encoding: Male = 0, Female = 1
- SubscriptionPlan and EngagementMetricsFrequency were encoded using unique value mappings.
2.	Feature Scaling: StandardScaler was used to normalize the feature values.
3.	Model Development: Two machine learning models were developed and compared:
  - Logistic Regression
- Decision Tree Classifier with max_depth = 5 to prevent overfitting.
4.	Model Evaluation: Models were evaluated using accuracy, precision, recall, and F1 scores on the train, validation, and test sets. Confusion matrices were used to interpret model performance on the test set.
Results:
- Logistic Regression Model:
•	Test Accuracy Score: 0.969
•	Test Precision Score: 0.964
•	Test Recall Score: 0.973
•	Test F1 Score: 0.969
- Decision Tree Model:
•	Test Accuracy Score: 0.973
•	Test Precision Score: 0.972
•	Test Recall Score: 0.974
•	Test F1 Score: 0.973
- Confusion Matrix for Logistic Regression:
•	Churn: Correctly predicted 841, incorrectly predicted 31
•	Not Churn: Correctly predicted 852, incorrectly predicted 32
- Confusion Matrix for Decision Tree:
•	Churn: Correctly predicted 848, incorrectly predicted 24
•	Not Churn: Correctly predicted 852, incorrectly predicted 23
## Key Features Influencing Churn:
1.	Number of service interactions (Call, Email, Chat)
2.	Number of late payments
3.	Time spent on the company’s website
4.	Net Promoter Score (NPS)
## Conclusion and Recommendation:
Both models performed exceptionally well, but the Decision Tree model is recommended for deployment due to its slightly superior performance metrics. The model will enable Reder Telecom to identify high-risk customers and implement targeted retention strategies, thereby reducing churn rates and enhancing customer satisfaction.
Continuous monitoring and evaluation of the model's performance are essential to ensure its effectiveness over time. Additionally, considering the dynamic nature of customer behavior, periodic retraining of the model with updated data is recommended to maintain its accuracy and relevance.


