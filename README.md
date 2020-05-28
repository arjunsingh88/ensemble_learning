# Ensemble Learning
Ensemble learning is the process by which multiple models, such as classifiers or experts, are strategically generated and combined to solve a particular computational intelligence problem. Ensemble learning is primarily used to improve the (classification, prediction, function approximation, etc.) performance of a model, or reduce the likelihood of an unfortunate selection of a poor one. Other applications of ensemble learning include assigning a confidence to the decision made by the model, selecting optimal (or near optimal) features, data fusion, incremental learning, nonstationary learning and error-correcting. This article focuses on classification related applications of ensemble learning, however, all principle ideas described below can be easily generalized to function approximation or prediction type problems as well.

Use of ensemble learning algorithm to improve the accuracy of Decision tree model. Build a predictive model to understand key parameters affecting USA income. 

## Bagging
Bagging is an ensemble technique mainly used to reduce the variance of our predictions by combining the result of multiple classifiers modelled on different sub-samples of the same data set
###             Bagging = Bootstrapping + Aggregation
![Bagging](https://github.com/arjunsingh88/ensemble_learning/blob/master/Visualizations/bagging.jpg)

### Random Forest

Random Forest is an ensembling method and one of the most popular and powerful algorithm in Machine Learning. 
The random forest is a model made up of many decision trees. Rather than just simply averaging the prediction of trees (which we could call a “forest”), this model uses two key concepts that gives it the name random:
1. Random sampling of training data points when building trees
2. Random subsets of features considered when splitting nodes

![Random forest](https://user-images.githubusercontent.com/45566835/83131586-58bb2680-a0e0-11ea-8c00-2817fa00265a.png)

### Bagging with Random forest
* `Step 1.` Repeat For ntrees 10,200 by increment of 10
* `Step 2.` &nbsp;&nbsp; Repeat for mtrys 1:7 (no of features to try)
* `Step 3.` &nbsp;&nbsp;&nbsp;&nbsp; Repeat for different seeds "num" from 1:20
* `Step 4.` &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; set Seed (num)
* `Step 5.`	&nbsp;&nbsp;&nbsp;&nbsp; 	  compute mean(accuracies of different setseed)
* `Step 6.` &nbsp;&nbsp;  max(between all the 7 try’s
* `Step 7.` Result
