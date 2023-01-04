# Portfolio Allocation Optimization 

In this project, we built a model that takes in historical data of the instruments and forecasts the return by machine learning and time series methods for investors to perform portfolio rebalancing regularly. 

### Modelling Approach
Models used: CatBoost, LightGBM, KNN, Random Forest, Naïve Bayes Regression and Multinomial Regression 
* ROC AUC score was used to gauge the performance of the models fitted

| Model                 | ROC AUC score  | 
|:--------------------: |:-------------: | 
| Random Forest         | 0.7535364      |
| CatBoost              | 0.7529079      | 
| LightGBM              | 0.7484488      | 
| Naïve Bayes Regression| 0.6919283      |
| Multinomial Regression| 0.7202357      |
| KNN                   | 0.6385671      |

CatBoost, LightGBM and Random Forest were selected to be part of the final stacked model as they have the best performance.

Using the predicted ranking probabilities, we generated the investment decision by assigning investment weights to each ranking bucket and calculating the investment decision for each instrument accordingly. 

