# Titanic Kaggle Challenge
http://www.kaggle.com/c/titanic-gettingStarted
 
>The sinking of the Titanic is one of the most infamous shipwrecks in history.

>On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1,502 out of 2,224 passengers and crew.

>While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

>In this challenge, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).

### Table of Contents:
1. Import and profile data
2. Transform categorical variables
3. Correlation Matrix
4. Feature Engineering, Impute, Bin Features
5. Add Interactions
6. Score Models
7. Tune Hyper Parameters - if necessary
8. Calculate Model Probabilities
9. Create Ensemble Models
10. Calculate Model Performance Metrics
11. Select Final Model
12. Submit to Kaggle
13. Compare Public Score with Leaderboard

The goal was to build a notebook that could provide a iterable workflow in order to explore different strategies to clean the data, 
perform feature engineering, evaluate models using K-fold cross validation. 

Additionally, the notebook can be published to Kaggle and scored.

### Baseline Model:
*   Categorical features performed better if they are one-hot encoded.
*   Continuous features like Fare, Age, and Family Size (SibSp + Parch) performed better as continuous instead of as bins.
*   A baseline model with just these two findings results in a strong public score of **0.79186**.

### Additions for Final Model:
*   Feature interactions.
*   Tuned hyper-parameters.
*   Ensemble models.
*   Much better definition of Family Size that distinguished between siblings and spouses and between parents and children. 
*   Final Model resulted in big improvement in cv metrics, but a lower score of **0.78468**.

### Kaggle Submission:
https://www.kaggle.com/code/cganxs/titanic-competition