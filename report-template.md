# Report: Predict Bike Sharing Demand with AutoGluon Solution
#### Saher Pathan

## Initial Training
### What did you realize when you tried to submit your predictions? What changes were needed to the output of the predictor to submit your results?
The output of predictor didn't match that of the expected format for submission. Did necessary changes to the data frame column datatypes, utilized 'count' label while training. 

### What was the top-ranked model that performed?
The top-ranked model was the one with new additional features and no hyperparameter tuning.
|best model|score|
|--|--|
|WeightedEnsemble_L3|-30.290553|
   
## Exploratory data analysis and feature creation
### What did the exploratory analysis find and how did you add additional features?
EDA revealed insights into feature distribution and relationships. Additional features were created using hot encoding. 

### How much better did your model perform after adding additional features and why do you think that is?
The model improved significantly, as newly added features provided more relevant and precise information.

## Hyperparameter tuning
### How much better did your model perform after trying different hyperparameters?
Comparatively much better and more stable.
### If you were given more time with this dataset, where do you think you would spend more time?
I would further focus on feature engineering processes to extract more meaningful data.

### Create a table with the models you ran, the hyperparameters modified, and the kaggle score.
|model|hpo1|hpo2|hpo3|score|
|--|--|--|--|--|
|initial|default_vals|default_vals|default_vals| 1.85146|
|add_features|default_vals|default_vals|default_vals| 0.62155|
|hpo|GBM: num_leaves: lower=26, upper=66|GBM: num_boost_round: 100|NN: dropout_prob: 0.0, 0.5|	0.47832|

### Create a line plot showing the top model score for the three (or more) training runs during the project.


![model_train_score](https://github.com/Saherpathan/nd009t-c1-intro-to-ml-project-starter/assets/80739877/bf1f5103-19ed-40c2-a99e-5821503ece29)



### Create a line plot showing the top kaggle score for the three (or more) prediction submissions during the project.

![model_test_score](https://github.com/Saherpathan/nd009t-c1-intro-to-ml-project-starter/assets/80739877/64b7c0d6-d98c-412f-b8b2-764c0db87d34)


## Summary
Project is executed successfully
