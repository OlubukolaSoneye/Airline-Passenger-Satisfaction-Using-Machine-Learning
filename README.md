# Airline-Passenger-Satisfaction-Using-Machine-Learning
The project analyses the Satisfaction of airline passengers, by analysing a dataset of 10,000 passengers. The SEMMA framework was utilised in the process of SAS data mining, with Regression and Decision tree models utilised. 

<img src="Screenshot 2026-02-21 at 12.15.56.png" width="500"/>


##  📊 The Business
Airlines operate in a highly competitive industry where customer satisfaction directly impacts retention, revenue, and brand reputation. From a dataset of 10,000 passengers, 67.4% were classified as Neutral or Dissatisfied. This project aimed to identify the key drivers of dissatisfaction and provide data-driven recommendations to improve airline performance and customer experience. 

## 📌 Project Overview
Developed predictive machine learning models using SAS to analyse airline passenger satisfaction. Applied the SEMMA framework (Sample, Explore, Modify, Model, Assess) to:

1. Clean and prepare structured passenger data
2. Identify patterns driving dissatisfaction
3. Build and evaluate classification models
4. Deliver actionable business recommendations

## 📌 Data Exploration
Using the File Import Node, the data was imported into SAS. A total of 22 variables were categorised into three levels for this project. 15 variables are Ordinal, 4 variables are Interval and 3 variables are Binary.
<img src="Screenshot 2026-02-21 at 12.39.17.png"/> 

## 📌 Dataset Balance
From the Graph explore node, the data set balance is Imbalanced. This is due to the non-equal distribution between the two categories, which are Neutral or Dissatisfied at 67.4% and Satisfied at 32.6%.
<img src="Screenshot 2026-02-21 at 12.16.26.png"/> 

## 📌 Sampling Method (through the Data Partition Node)
The dataset was split into three: Train set: 50.0, Validation set: 30.0 , Test set: 20.0.

The Data Partition Node was chosen for Sampling to prevent overfitting and enhance the model performance. Missing Data Values - I observed missing data across 3 variables, to address the missing values, Mean Imputation was used via the Impute node for three variables.
<img src="Screenshot 2026-02-21 at 12.17.44.png"/> 


## 📌 Outliers
The Neutral or Dissatisfied group's departure delays, arrival delays and flight show a large variation, indicating that major delays and long flights have a detrimental effect on satisfaction.
<img src="Screenshot 2026-02-21 at 12.17.55.png"/> 

## 📌 Multicollonearity
The scatter plot reveals that the variables Departure_Delay and Arrival_Delay are highly correlated.
<img src="Screenshot 2026-02-21 at 12.18.06.png"/> 

Data Modelling was done using Logistic Regression models and Decision tree models, Here is the result of the best performing model

From the models created, the most optimal model from the project is the DT-Entropy-Multiway Split, with a ROC Index of 0.98, indicating how well it can distinguish between classes. The most likely positive instances are efficiently targeted by attaining a high Cumulative Lift 3. Its low false negative rate of 54 and somewhat low false positive rate of 167 make it reliable for use in decision-making.
<img src="Screenshot 2026-02-21 at 12.18.18.png"/> 

## 📌 % Response and Cumulative Lift of DT-Entropy-Multiway split]
<img src="Screenshot 2026-02-21 at 12.18.32.png"/> 

## 📌 Business Recommendation and Conclusion
From the analysis, there are inconsistent airline's schedules leading to Neutral/Dissatisfied passengers. The findings suggest that the airline should focus on operational improvements, such as adhering strictly to schedules and additional strategies for satisfaction such as clear communication and compensation for any extreme delay. Age variable is slightly right skewed indicating more younger passengers, with a mean age of 38.2 years. The airline should address specific age needs for this group, as an opportunity to generate more revenue. Additionally, targeting marketing campaigns and  incentives to attract their highest category of returning customers  (38.2years). Flight distance does not follow a normal distribution with outliers indicating passengers on long-haul flights report higher dissatisfaction, therefore the airline should explore improvements for long flights such as food, entertainment and comfort.

## 📬 Contact
Made by Bukola Soneye
LinkedIn:https://inkedin.com/in/bukola-soneye/
