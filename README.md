# Predicting House Prices with Machine Learning

Our goal is to predict sale prices for homes in Ames, Iowa using Advanced Supervised Regression Techniques.

## Tools and Libraries
- Tools :
#####         Python
#####         Jupyter
- Libraries :
#####        Pandas — For handling structured data
#####        Scikit Learn — For machine learning
#####        NumPy — For linear algebra and mathematics
#####        Seaborn — For data visualization

## Our Machine Learning Model Development Cycle

<p align="center">
  <img width="600" src="https://github.com/anuragd3118/Predicting-House-Prices-with-Machine-Learning/blob/main/Machine%20learning%20model%20development%20cycle.webp" alt="Machine Learning Model Development Cycle">
</p>

## Machine Learning Models Used

##### Decision Tree
- A tree algorithm used in machine learning to find patterns in data by learning decision rules.
##### Random Forest
- A type of bagging method that plays on ‘the wisdom of crowds’ effect. It uses multiple independent decision trees in parallel to learn from data and aggregates their predictions for an outcome.
##### Gradient Boosting Machines
- A type of boosting method that uses a combination of decision tree in series. Each tree is used to predict and correct the errors by the preceding tree additively.

## Evaluation through Error Calculation
Our performance metric will be the Negative Root Mean Squared Error (NRMSE). I’ve used this because it’s the closest I can get to Kaggle’s scoring metric in SciKit Learn.

##### Decision Tree
- Predictably this was our worst performing method. Our best decision tree score -0.205 NRMSE. Tuning the hyperparameters didn’t appear to make much of a difference to the model’s however it trained in under 2 seconds. There is definitely some scope to assess a wider range of hyperparameters.
##### Random Forest
- Our random forest model was a marked improvement on our decision tree with a NRMSE of -0.144. The model took around 75 seconds to train.
##### Gradient Boosting Machines
- This was our best performer by a significant amount with a NRMSE of -0.126. The hyperparameters significantly impact the results illustrating that we must be incredibly careful in how we tune these more complex models. The model took around 196 seconds to train.
