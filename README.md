# Customer-Churn-Prediction
 predicting customer churn at a fictitious wireless telecom company and use insights from the model to develop an incentive plan for enticing would - be churners to remain with company.


### Objective
When a customer applies for a loan, banks and other credit providers use statistical models to determine whether or not to grant the loan based on the likelihood of
the loan being repaid. The factors involved in determining this ikelihood are complex, and extensive statistical analysis and modeling are required to predict the outcome for each individual case. Implement a model that predicts loan repayment or default based on the data provided.


### The dataset consists of the following fields:
    1   gender            
    2   SeniorCitizen     
    3   Partner          
    4   Dependents       
    5   tenure        
    6   PhoneService      
    7   MultipleLines     
    8   InternetService  
    9   OnlineSecurity   
    10  OnlineBackup      
    11  DeviceProtection  
    12  TechSupport       
    13  StreamingTV      
    14  StreamingMovies   
    15  Contract        
    16  PaperlessBilling 
    17  PaymentMethod    
    18  MonthlyCharges    
    19  TotalCharges     
    20  customerID 
    21  Churn

#### Machine Learning Steps followed to predictthe Loan status:
    1. Load the Dataset 
    2. Data Cleaning to fill missing values and remove unwanted values.
    3. Preprocesing the data of Categorical variables.
    4. Apply Standard Scaler to normalize the data
    5. Split Train and Test dataset
    6. Apply Different models in order to get the best model using SelectKBest to get best features:
        i.  Apply Logistic Regression 
            - accuracy score - 0.80
        ii. Apply Random Forest
            - accuracy score - 0.82
    5. Performance on Test Data
            - accuracy score - 0.81

### Final Conclusions
We selected the variables to be included in the model by using SelectKBest alogorithm and ran it on different K values for the features in order to extract the best number of features which would given the highest accuracy for the model.

#### Performance of the model (Random Forest Model):
     The calibration(train) accuracy of the model is 0.82
     The precision of the decision that the Customer would not be leaving is 0.85
     The precision of the decision that the Customer would be leaving is 0.62
     The validation(test) accuracy of the model is 0.81
     The precision of the decision that the Customer would not be leaving is 0.85
     The precision of the decision that the Customer would be leaving is 0.67

Hence, Our model is neither underfitting nor Overfitting.
##### The key factors that predict customer churn are as follows:
       - tenure
       - OnlineSecurity
       - OnlineBackup
       - TechSupport
       - Contract
       - PaperlessBilling
       - MonthlyCharges

#### Offers that should be made to encourage customers to retain them with the company should be as follows:
         1. Offer the customers to increase the tenure
         2. If Customer is having Internet services, they should be offered complementary Online security and online backup facilities
         3. Ensure the Tech Support to be provided on time and focus on cutomer needs and facilitate them timely
            People with longer Contract plan of their services tend to stay longer with the company, ensure to offer people longer contract plans with slightly low charges to               make them stay.
         4. If these actions are implemented, we can collect the latest Customer Churn data(post the implementation of these changes) and compare the same with historic data in             order to confirm that verify that the suggested changes has reduced the Customer Churn rate.      

