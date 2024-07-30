# Churn_prediction
# PROJECT_NAME : Bank_Customer_churn_prediction
# DATASET : 175028 records , 34 columns
# DATA_PREPROCESSING :
              • Drops unnecessary columns (CustomerId)
              • Encodes categorical data (Surname and object_dat categories).
              • Rounds Age values and creates new derived features(Mem__no__Products, Cred_Bal_Sal,
              Bal_sal, Tenure_Age, Age_Tenure_product, IsSenior).
              • Scales numeric columns (Age, Tenure, CreditScore, Balance, EstimatedSalary, and their
              derived forms).
              EXPLORATORY_DATA_ANALYSIS(findings-insights):
              • HEAT_MAP: Credit score, age, tenure are inversely proportional to churn rate and age ,no: of
              products are directly proportional to churn rate. Survival analysis can help understand the
              duration until customers churn based on different variables. Here clearly shown that senior ,
              male , credit score are main reasons for active customers without churning.
              • BOX_PLOTS(numeric_data): Balance variable had strong corelation with churn rate than
              estimated salary.
              • BAR_GRAPHS(catergorical_data): Female had more churn rate than male. Germany had
              more churn rate than France, Spain
              • KNN_CLUSTERING: Clusters reveal distinct segments of customers, which can be used to for
              marketing strategies and services to prevent churning.
              • FEATURE_IMPORTANCE: Random forest and Decision tree model are used for finding feature
              importance. But permutation_random_forest given accurate feature importance like
              Balance, Age , No: of products for churn rate output.
# MODEL BUILDING(Methodologies): ROC Scores for Classification Models:
      # Individual Methods:
              Decision Tree: 0.7029
              Logistic Regression: 0.6134
              Random Forest: 0.8636
              K Nearest Neighbors: 0.5575
              Naive Bayes: 0.7716
      # Ensemble Techniques:
              HistGradientBoosting: 0.8932
              LightGBM: 0.8938
              CatBoost: 0.8938
              AdaBoost: 0.8798
              XGB: 0.8951
              Gradient Boosting: 0.8892
1. Among all models XGB model had more
score.
2. Ensemble models performed better than individual models.


# RESULTS : 
    To mitigate churn rate effectively, prioritize customer satisfaction by tailoring retention
strategies to factors such as seniority, credit score, gender, and geographic location. Implement
proactive measures like enhancing service quality, providing targeted incentives, and addressing key
variables identified through thorough analysis, such as balance, age, and product engagement.
