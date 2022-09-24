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

- The variables that are considered to be the features for the model are:
    
    - APPLICATION_TYPE—Alphabet Soup application type
    - AFFILIATION—Affiliated sector of industry
    - CLASSIFICATION—Government organization classification
    - USE_CASE—Use case for funding
    - ORGANIZATION—Organization type
    - STATUS—Active status
    - INCOME_AMT—Income classification
    - SPECIAL_CONSIDERATIONS—Special consideration for application
    - ASK_AMT—Funding amount requested


- The The EIN and NAME columns have been dropped initally, as they are not features for the first model.

### Compiling, Training, and Evaluating the Models

My inital model consisted of two layers, the first had 80 neurons, the second had 50, both with relu activations functions. The output layer was assigned a sigmoid activations funcation, as the out put would be grouped as either "IS_SUCCESSFUL" or not.  
The initial model output is pictured below:

<img width="631" alt="Screen Shot 2022-09-24 at 12 09 19 PM" src="https://user-images.githubusercontent.com/105119531/192108010-5bf62deb-0bbf-4101-a4c6-c13cb8fe973f.png">

I attempted three more models tyring to reach an accuracy of greater then 75%.  
- In the first additional attempt I also dropped “low information” columns “STATUS”, “SPECIAL_CONSIDERATIONS”,
 binned low occurrence value counts “APPLICATION_TYPE”, “CLASSIFICATION” and added a hidden layer, producing the results pictured below:

<img width="878" alt="D3 1 " src="https://user-images.githubusercontent.com/105119531/192108253-d35e16a7-54e6-4f4f-8838-631fb9221d3a.png">

- In my second attempt I Dropped “low information” columns “STATUS”, “SPECIAL_CONSIDERATIONS”, binned low occurrence value counts “APPLICATION_TYPE”, “CLASSIFICATION”, bucketed “NAME” into three categories “, and added a hidden layer and changed activation functions to sigmoid, producing the results pictured below:

<img width="995" alt="D3 2" src="https://user-images.githubusercontent.com/105119531/192108350-52484d3b-d726-4a45-9f67-2915abef70f2.png">

- In my third and final attempt, I dropped “low information” columns “STATUS”, “SPECIAL_CONSIDERATIONS”, binned low occurrence value counts “APPLICATION_TYPE”, “CLASSIFICATION”, binned “NAME” into an other category for all values less than or equal to five. I did not change the model from the initial settings. The results are pictured below:

<img width="830" alt="D3 3" src="https://user-images.githubusercontent.com/105119531/192108460-1eb507a3-a623-4349-9332-eb42a0897bc8.png">


## Summary: 
I was able to achieve a result above 75% with the adjustments made in the third model. Because neural networks are very complex, it would take a great deal more investigation to determine how to improve the model from here.  The results are sufficient for this assignment but could still be improved.


 
