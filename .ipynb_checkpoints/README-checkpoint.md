# Titanic Kaggle Challenge
 http://www.kaggle.com/c/titanic-gettingStarted
 
>The sinking of the Titanic is one of the most infamous shipwrecks in history.

>On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1,502 out of 2,224 passengers and crew.

>While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.

>In this challenge, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).


### Workflow:
The goal was to build a notebook that could provide a iterable workflow in order to explore different strategies to:

*   Clean the data
*   Perform feature engineering
*   Evaluate models using K-fold cross validation
*   Upload notebook to Kaggle to publish and score the model


### Findings:
*   Categorical features performed better if they are one-hot encoded.
*   Continuous features like Fare, Age, and Family Size performed better as continuous instead of as bins.
*   Doing this results in an above median-model with a Public Score of **0.79186**.
*   Adding feature interactions provided gains, but the impact was minimal.
*   No need to iterate over hyper-parameters for further gains. Run study and settle on best parameters.
*   Adding ensemble models resulted in big improvement in cv metrics, but a lower score of **0.78468**.







