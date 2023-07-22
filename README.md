# Capstone Project (Classification)
##  Capstone Project on Health Insurance Cross Sell Prediction

### Problem Statement
Our client is an Insurance company that has provided Health Insurance to its customers now they need your help in building a model to predict whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.

An insurance policy is an arrangement by which a company undertakes to provide a guarantee of compensation for specified loss, damage, illness, or death in return for the payment of a specified premium. A premium is a sum of money that the customer needs to pay regularly to an insurance company for this guarantee.

For example, you may pay a premium of Rs. 5000 each year for a health insurance cover of Rs. 200,000/- so that if, God forbid, you fall ill and need to be hospitalised in that year, the insurance provider company will bear the cost of hospitalisation etc. for upto Rs. 200,000. Now if you are wondering how can company bear such high hospitalisation cost when it charges a premium of only Rs. 5000/-, that is where the concept of probabilities comes in picture. For example, like you, there may be 100 customers who would be paying a premium of Rs. 5000 every year, but only a few of them (say 2-3) would get hospitalised that year and not everyone. This way everyone shares the risk of everyone else.

Just like medical insurance, there is vehicle insurance where every year customer needs to pay a premium of certain amount to insurance provider company so that in case of unfortunate accident by the vehicle, the insurance provider company will provide a compensation (called ‘sum assured’) to the customer.

###  Objective 
Building a model to predict whether a customer would be interested in Vehicle Insurance is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

### Attributes Information
- id : Unique ID for the customer

- Gender : Gender of the customer

- Age : Age of the customer

- Driving_License : 0 - Customer does not have DL, 1 - Customer already has DL

- Region_Code : Unique code for the region of the customer

- Previously_Insured : 1 : Customer already has Vehicle Insurance, 0 : Customer doesn't have Vehicle Insurance

- Vehicle_Age : Age of the Vehicle

- Vehicle_Damage : 1 : Customer got his/her vehicle damaged in the past. 0 : Customer didn't get his/her vehicle damaged in the past.

- Annual_Premium : The amount customer needs to pay as premium in the year

- PolicySalesChannel : Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.

- Vintage : Number of Days, Customer has been associated with the company

- Response : 1 : Customer is interested, 0 : Customer is not interested


### Summary
The health insurance cross sell prediction dataset is a dataset that contains information about customers of an insurance company and whether they have purchased a particular insurance product. The goal is to build a predictive model that can accurately identify which customers are likely to purchase the product.

In this project, we analyzed the dataset and performed exploratory data analysis to understand the patterns and relationships in the data. We then preprocessed the data and trained four different classification models:

Logistic Regression, KNN, Random Forest, and XGBoost.

### Conclusion
- There are 206089 Male customers and 175020 Female customers

- There are 380297 people who own Driving License and 812 don't

- Its found that most of the people who own driving license owns a car

- It is observed that people who have previously not insured are intrested in the policy

- It is found that people who have not insured previously are more intrested in buying the ploicy, so it is better to tap the market who previously have not insured

- It is observed that most of the people with vehicle age is 1-2 years.

- Ratio wise people with vehicle age greater than 2 years are more intrested in buying policy

- Most of the customers have their vehicle age as 1-2 years

- As per the ratio it is better to tap the customers whose vehicle age is more than 2 years and we have a good scope in people who own vehicle of age 1-2 years as well.

- Its found that previously customers who got their vehicle damaged are more intrested in buying new policy

- Customers who are previously not damaged their car are not much intrested in buying the policy

- People who have damaged their car previously are more intrested in buying the policy.

- It is found that people who have damaged their vehicle and not damaged share almost equal proportion.

- Comparing the insights previously it is found that the people who damaged their vehicle are more intrested to buy ploicy, so since 50% of the people who are willing to buy the plociy, the market is big to capture

- Most of the premium falls under range 5000-100000

- There are some premiums that are above 100000

- There are no outliers in the age columns and most of the customers belong to age group 25-48

- Customes of age between 32-58 ar more mature and are intrested in buying the policy

- Tapping the customer of age between 32-58 would be more benificial

- Most of the customers belong to region code 28 followed by 8

- Most of our customers belong to region code 28, so it would be better if we run our marketing campagn such that in 28 to aquire more customers and in other regions to penetrate the market.

- Its found that most of the customer have vehicle age of around 1-2 year and there are less customers whose vehicle age is greater than 2 years

- Its found that most of the customers who do not own driving license are less and are least intreasted, so tapping the customers with license would be benificial

- It is found that policy sales channel and respons is negativly correlated.

- Most of the properties/features against eachother are very least correlated.

- Positive response of Vintage customers are positivly correlated with annual customers.

### Model Evaluation and Conclusion
It is evident from the evaluation matrix that Random Forest Algorithm outperforms rest of the algorithms with maximum accuracy of 90%. So we have considered Random Forest model to save and for futhur deployment to make predictions on unseen data.
