# Credit_Risk_Evaluator

# Background
LendingClub is a peer-to-peer lending services company that allows individual investors to partially fund personal loans as well as buy and sell notes backing the loans on a secondary market. LendingClub offers their previous data through an API.

You will be using this data to create machine learning models to classify the risk level of given loans. Specifically, you will be comparing the Logistic Regression model and Random Forest Classifier.

# Scores
  Scaled data uses StandardScaler
  
Logistic Regression scores - 
Original data: 0.5087196937473416
Scaled data: 0.7598894087622289

Random Forest scores - 
Original data: 0.644193960017014
Scaled data: 0.6435559336452573

# Evaluation

After cleaning and pre-processing the data using standard cleaning tools as well as get_dummies, I ran the original data through both the Logistic Regression and Random Forest Classifer models. I also scaled the data to determine how that affected the scores. (Resulting scores above.)

The Logistic Regression scores showed the larger increase in accuracy when scaled although the result is still not very accurate. The Random Forest Classifier scores show that model was not very sensitive to scaling as the scores barely moved, and it was also not very accurate. 

The next steps I would take would be to try a different scaling method (Min/Max) to see if that makes a difference. I would also consider if scaling is appropriate for the data that I have. It may be that adjusting the weight of the categorical data is negatively affecting the outcomes. There are other options for how to evaluate this data for the purposes of making predictions. My conclusion is that the scaling and models used are not the most appropriate for the data I have.
