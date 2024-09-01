**SyriaTel Customer Churn Analysis**


**Business Understanding**


**Project Statement Overview**


SyriaTel, a telecommunications company, is dealing with a significant problem of customer churn, where a substantial number of customers are leaving their services for those of competitors. To tackle this challenge, the company seeks to build a predictive model for customer churn. By examining the dataset, SyriaTel aims to understand the factors contributing to customer attrition, with the ultimate objective of lowering the churn rate, enhancing customer retention, and boosting overall profitability.

**Specific Objectives**

* Identify the key factors contributing to customer churn.
* Create a model that can accurately predict which customers are at risk of leaving.
* Implement strategies to proactively retain customers who are identified as at risk of churn.

**Data Understanding**


We used customer churn dataset from the telecom industry sourced from Kaggle. The dataset contains information about customers, their usage patterns, and whether they have churned or not. The dataset contains 3,333 records and 21 columns. There were 4 to be categorical features and 17  numerical features.

**Data Preparation**


Dataset cleaning was done by checking missing data, duplicates, converting variables to appropriate data types and appropriate feature transformations was done and applied to modelling.

**Modeling**


We used SMOTE to fix the class imbalance of our target variable "churn"
The baseline model was logistic regression. I also explore decision tree and made model evaluation of the best performing mosel.

**Evaluation**


DecisionTreeClassifier has the highest recall score making it a better model as compared to Logistic regression.
The ROC curve analysis indicates that the DecisionTreeClassifier outperforms the LogisticRegression model. The DecisionTreeClassifier achieved the highest AUC score of 0.82, surpassing the LogisticRegression, which obtained an AUC score of 0.813. A higher AUC score signifies that the classifier is more effective at differentiating between positive and negative instances.


**Conclusion**


According to the visualizations, the following features are classified under important features hence they contribute more to customer churn;`international plan`,`total day minutes`, `customer service calls`and `total day charge`.The identification of these key features indicates areas where targeted interventions can significantly impact customer retention. By focusing on the international plan, daytime usage, customer service interactions, and total daytime charges, SyriaTel can implement strategies to address customer concerns and reduce churn rates.

**Recommendations**
* Adjust pricing strategies to offer better value for customers who incur high daytime charges. Introduce tiered pricing or loyalty discounts to mitigate churn.

* There is high churn rate in area code 415 and 510. SyriaTel can introduce promotional offers to customers these area code to enable them stay with the company.

* Improve customer service quality and reduce the number of customer service calls. This will lead to effective resolution to customers problems and lead to higher satisfaction hence reduced churn. 

* Consider revising the international plan to offer more competitive rates or additional benefits to retain customers who are heavy international users.