# Capstone-Project-Credit-Card-Default-Prediction-
The purpose of this project is to conduct quantitative analysis on credit card default risk by using 6 machine learning models with accessible customer data, instead of credit score or credit history, with the goal of assisting and speeding up the human decision making process.

## Dataset Source<br>
This dataset contains information on default payments, demographic factors, credit limit, history of payments, and bill statements of credit card clients in Taiwan from April 2005 to September 2005.

## Project Overview<br>
Machine Learning Modeling. The detailed notebook of modeling can be found <a href="https://github.com/KK-Niraj/Credit-Card-Default-Prediction/blob/main/Credit_Card_Default_Prediction_Capstone_Project.ipynb">here</a>.

Machine Learning Models Used: 
1. Logistic Regression
2. Decision Tree
3. Random Forest
4. XGBoost
5. SVC
6. KNN


## Key Findings from EDA
1. Males have more delayed payment than females in this dataset. Keep in mind that this finding only applies to this dataset, it does not imply this is true for other datasets.
2. Customers with higher education have less default payments and higher credit limits.
3. Customers aged between 30-50 have the lowest delayed payment rate, while younger groups (20-30) and older groups (50-70) all have higher delayed payment rates. However, the delayed rate drops slightly again in customers older than 70.
4. There appears to be no correlation between default payment and marital status.
5. Customers being inactive doesn’t mean they have no default risk. We found 317 out of 870 inactive customers who had no consumption in 6 months then defaulted next month.

## Model Comparison
In these 6 models, Random Forest model has the highest precision but the lowest recall, if the business cares precision the most, then this model is the best candidate. If the balance of recall and precision is the most important metric, then SVC is the ideal model. Since KNN has slightly higher recall but much lower precision than SVC, I would recommend SVC. 
![WhatsApp Image 2022-10-09 at 10 10 08 PM](https://user-images.githubusercontent.com/87687977/195095589-8b7ce925-d611-48f7-92b3-b10f440ff934.jpeg)

## Recommendations Based on ROC_AUC Curve
![WhatsApp Image 2022-10-09 at 10 09 13 PM](https://user-images.githubusercontent.com/87687977/195095745-1c360541-de54-418a-9c14-a8fd2a191589.jpeg)

## Conclusion
▶ After performing the various model we the get the best accuracy form the SVC(Support Vector Classifier) and KNN.
▶ Decision Tree is the least accurate as compared to other models performed.
▶ SVC has the best precision and the recall balance.
▶ Higher recall can be achieved if low precision is acceptable.
▶ We can deploy the model and can be served as an aid to human decision.
▶ Model can be improved with more data and computational resources.

## Future Work
1. Models are not exhaustive. Other models could perform better.
2. Get more computational resources to tune models.
