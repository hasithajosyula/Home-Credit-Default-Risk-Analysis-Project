# Home-Credit-Default-Risk-Analysis-Project

**Introduction:**

Many people struggle to get loans due to insufficient or non-existent credit histories. And, unfortunately, this population is often taken advantage of by untrustworthy lenders.

Home Credit strives to broaden financial inclusion for the unbanked population by providing a positive and safe borrowing experience. In order to make sure this underserved population has a positive loan experience, Home Credit makes use of a variety of alternative data--including telco and transactional information--to predict their clients' repayment abilities.

While Home Credit is currently using various statistical and machine learning methods to make these predictions, they're challenging Kagglers to help them unlock the full potential of their data. Doing so will ensure that clients capable of repayment are not rejected and that loans are given with a principal, maturity, and repayment calendar that will empower their clients to be successful.

**Business Problem**

Home Credit is a B2C company serving the unbanked sector of the populations by serving them loans. As these sectors has little to no credit history, Home Credit needs to assess repayment ability of the customer depending on other factors of the customers and provide them with trustful services. To improve this situation, Home Credit needs to assess the following factors for any customers to successfully give a loan:

1.	Principal
2.	Maturity of the loan
3.	Repayment calendar

Why is it important?

1. Individuals lacking credit history or facing inadequate financial resources struggle to secure loans.
2. Banks face challenges extending loans to the unbanked population due to the complexity of predicting their repayment capacity.
3. This strategy holds potential for adoption not only by Home Credit but also by other financial institutions aiming to enhance financial inclusivity.
4. Financial institutions can harness alternative data, such as telecommunications and transactional records, coupled with machine learning models, to facilitate these anticipations.
5. This methodology ensures that clients with the ability to repay are not declined loans, ensuring that loans are granted with a principal amount, maturity, and repayment schedule that empowers clients toward success.

**Project objective:**

The primary objective of this project revolves around utilizing historical loan application data to create predictive models determining an applicant's likelihood of loan repayment. These models are meticulously designed to empower lending institutions to render well-informed loan provision decisions, particularly to creditworthy clientele. By doing so, this initiative not only facilitates individuals with a commendable repayment history to access loans but also assists the company in circumventing instances of loan default.

Our project undertakes the construction of a Machine Learning model that exhibits the proficiency to forecast both potential loan defaulters and the creditworthiness of individuals seeking financial borrowing. Anchored in historical data, our efforts are dedicated to developing a robust and accurate model ideally suited to seamlessly integrate into existing operational processes. Through the amalgamation of data-driven insights, we aspire to enhance the precision and effectiveness of loan assessment procedures.

**Your group's solution to the business problem.**

The data is distributed across multiple tables, each representing a factor utilized by Home Credit to comprehend customer behavior. The primary challenge we encountered was identifying the pivotal features that hold the key to predicting customer default. To address this, we embarked on an initial step of conducting Exploratory Data Analysis (EDA) and formulated hypotheses based on both intuition and EDA findings.

Subsequently, we tackled the issue of missing values by employing data imputation strategies. Additionally, we undertook Feature Engineering to eliminate redundant or insignificant predictors while crafting new ones tailored to our specific requirements. Addressing the imbalance in the target variable, we executed a combination of undersampling and oversampling and employed the SMOTE technique on the data. Our approach involved employing diverse models to train and forecast the target variable, utilizing the Area Under the ROC Curve (AUC) as our evaluation metric. Comprehensive code and model comparisons are accessible in the repository.

Our objective was to construct a classification model that effectively predicts loan applicant default likelihood. The provided data encompassed a range of credit-related details for each application. Our data preprocessing involved outlier removal, mean-value imputation for missing entries, and conversion of categorical variables into dummy variables. Once the refined dataset was prepared for testing, it was divided into training and testing sets. Through K-fold cross-validation, models were trained, and a total of ten models were developed utilizing five classification methods. Moreover, we implemented three distinct sampling techniques to address the class imbalance within the data.

During the model assessment, we employed the area under the curve (AUC) as our performance metric, leading us to identify the top three models out of the ten. These included two XGboosted models and one Ridge Regression linear model. The AUC scores ranged between 0.6477 and 0.6843. To enhance performance, we created an ensemble model by integrating the top three models along with their specific sampling techniques. The final ensemble model yielded the highest score among the four models submitted to Kaggle, achieving a score of 0.71609. In light of these results, we recommend Home Credit to consider employing this combined methodology for future application reviews. This approach exhibited a 20% performance increase over the majority response classification. By integrating this model, Home Credit can enhance its ability to predict applicants unsuitable for loan approval based on their credit history.

**Your contribution to the project**

Throughout the project, I played a major role in both Exploratory Data Analysis (EDA) and Modeling. In close collaboration with the team, we engaged in weekly brainstorming sessions to unravel the intricacies of the dataset. An integral facet of my responsibilities was exploring the relationships between the target variable and predictor variables within the dataset, which is an important part of this project's framework. Furthermore, I was also involved in building predictive models and calculating essential metrics such as AUC, accuracy, and others. I also performed activities related to feature engineering and carefully assessed the importance of features. This deliberate approach aimed to improve the model by recognizing and changing important features.

**The business value of the solution**

The company is currently experiencing an 8% default rate among all its loans. Our model has been constructed with an accuracy of 68%. Considering this, if the company adopts our algorithm for loan approval decisions, it could prevent approximately 5.44% of loans from being extended to defaulters. As a result, the percentage of defaulters could decrease to 2.56%, leading to reduced losses. Moreover, by enhancing the quality of training, the model's accuracy has the potential to improve further. This, in turn, would contribute to minimizing losses even more effectively.

**Difficulties that your group encountered along the way**

Throughout the project, we encountered a series of challenges that tested our problem-solving abilities. Initially, we grappled with the dataset's vastness, which contained many variables. Comprehending the intricacies of the data demanded a considerable amount of time and effort. Another significant hurdle was the pronounced imbalance within the dataset. This imbalance had the potential to introduce bias into our predictions. We implemented techniques like undersampling, oversampling, and SMOTE to mitigate this. These measures were essential in tackling issues of overfitting or underfitting.

The process of constructing models presented its own set of obstacles. Determining the most suitable models for training proved to be a complex task. For instance, we had to exclude the SVC model due to extended execution times. However, we overcame these challenges and successfully developed models that effectively predicted the target variable.

Engaging in feature engineering and evaluating feature significance also came with their share of challenges, largely stemming from the notable variations detected within the fields. Furthermore, collaborating on the project posed challenges, as team members were concurrently juggling full-time jobs or internships. This restricted availability sometimes made coordination and meeting deadlines demanding. Despite these challenges, we persevered with determination and successfully produced a resilient credit risk prediction model for Home Credit.

**What you learned in the project**

Engaging in the Home Credit default risk analysis project provided me with immensely valuable experience. It taught me how to handle extensive datasets effectively, address outliers and missing values, and manage dataset imbalances. I acquired the skillset to employ techniques like undersampling, oversampling, and SMOTE to mitigate imbalance and potential bias in the data. Furthermore, I delved into Lasso and ridge regression models, expanding my data science knowledge beyond my prior understanding. This enriched my data science comprehension and facilitated the enhancement of my skillset.

Beyond the technical aspects, I gained invaluable experience in teamwork and effective communication within a group, especially under the constraints of tight project deadlines. These valuable lessons will illuminate our path in future undertakings, empowering us to skillfully apply predictive analytics to a wide spectrum of business challenges spanning different industries.



