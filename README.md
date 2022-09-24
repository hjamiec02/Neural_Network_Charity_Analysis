# Neural_Network_Charity_Analysis

## Overview of the analysis: 

A business team at Alphabet Soup provided a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization. Using features provided in the dataset from past donors I helped create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results: Using bulleted lists and images to support your answers, address the following questions.

- The data was preprocessed with the following steps:
  - The EIN and NAME columns have been dropped .
  - The columns with more than 10 unique values have been grouped together.
  - The categorical variables have been encoded using one-hot encoding. 
  - The preprocessed data is split into features and target arrays.
  - The preprocessed data is split into training and testing datasets.
  - The numerical values have been standardized using the StandardScaler() module. 

- The target variable for the model is IS_SUCCESSFUL

- The variables are considered to be the features for the model are:
  - STATUS                        
  - ASK_AMT                                       
  - APPLICATION_TYPE_Other      
  - APPLICATION_TYPE_T10          
  - APPLICATION_TYPE_T19        
  - APPLICATION_TYPE_T3          
  - APPLICATION_TYPE_T4           
  - APPLICATION_TYPE_T5          
  - APPLICATION_TYPE_T6         
  - APPLICATION_TYPE_T7          
  - APPLICATION_TYPE_T8          
  - AFFILIATION_CompanySponsored  
  - AFFILIATION_Family/Parent     
  - AFFILIATION_Independent      
  - AFFILIATION_National         
  - AFFILIATION_Other            
  - AFFILIATION_Regional        
  - CLASSIFICATION_C1000         
  - CLASSIFICATION_C1200          
  - CLASSIFICATION_C2000         
  - CLASSIFICATION_C2100          
  - CLASSIFICATION_C3000          
  - CLASSIFICATION_Other          
  - USE_CASE_CommunityServ        
  - USE_CASE_Heathcare            
  - USE_CASE_Other                
  - USE_CASE_Preservation         
  - USE_CASE_ProductDev           
  - ORGANIZATION_Association      
  - ORGANIZATION_Co-operative     
  - ORGANIZATION_Corporation      
  - ORGANIZATION_Trust            
  - INCOME_AMT_0                  
  - INCOME_AMT_1-9999             
  - INCOME_AMT_10000-24999        
  - INCOME_AMT_100000-499999      
  - INCOME_AMT_10M-50M            
  - INCOME_AMT_1M-5M              
  - INCOME_AMT_25000-99999        
  - INCOME_AMT_50M+               
  - INCOME_AMT_5M-10M            
  - SPECIAL_CONSIDERATIONS_N     
  - SPECIAL_CONSIDERATIONS_Y      

- The The EIN and NAME columns have been dropped initally, as they are not features for the model.

### Compiling, Training, and Evaluating the Models

How many neurons, layers, and activation functions did you select for your neural network model, and why?



Were you able to achieve the target model performance?

What steps did you take to try and increase model performance?

## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
