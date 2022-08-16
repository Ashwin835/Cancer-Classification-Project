# Classification-Model-Project

# Project Description
 This Dataset was obtained from the url: https://www.kaggle.com/datasets/shravan3273/breast-cancer-classifiction
 
 Given a bunch of features of a tumor, we want to find a model that gives the best predictions on if a tumor is benign
 or malignant. Finding the best fitting model has many factors to it, but for this project only the 
 cross val score is being looked at, along with any major overfitting/underfitting. Given the size of the data, 10 folds
for cross validation was chosen as there wasn't any over/underfitting as well. Some of the models tested are logistic
 regression, K neighbors classifier, naive bayes, support vector classification (linear and rbf), decision tree 
classification and random forest classification


# Project Results
                                          LOGISTIC REGRESSION
 Overall this model is really good for both the trained and test data, shwoing there was no over/underfitting. The test data
on cross validiation was very high accuracy with low standard deviation. The training data didn't differ much from the 
 test data
 
 
                                          K NEIGHBORS CLASSIFICATION
 This model was also very solid, but not better than the logistic regression. With n_neighbors being 20, you get both 
 training and testing data with very high accuracy above 95% with low standard deviation. A lower number of neighbors 
 below 10 would result in good accuracy but a bit higher standard deviation. above 35 will lead to lower accuracies and
 higher standard deviations. The accuracy for the test data was very solid, but the standard deviation was a bit higher
 compared to logisitc regression, so that is why logistic regression is better
 
                                                SVC (LINEAR) 
 This model was good for both test and training set. The test set wasn't as accurate as the logistic test set, but the 
standard deviation was lower, making it very slightly better than the logistic regression. The value of C doesn't 
affect the result of the accuracy and standard deviation drastically. 


                                                  SVC (RBF) 
 The accuracies and standard deviation for test data of this model were very similar compared to the test results of 
 the K Neighbors classifier. Both test and train data performed well on the model given their accuracies and standard
 deviation. As you increased the gamma parameter, the accuracies and standard deviation got worse. The C parameter
 didn't have much of an drastic effect on the percentages regardless of it's value
 
 
                                                  NAIVE BAYES
 This model is the least accurate in giving results on the test set. With only 88% accuracy and variance of 9%. However,
 there isin't a significant difference compared to others. We are also assuming that all of the independent variables
 are independent
 
 
                                         DECISION TREE CLASSIFICATION 
 This model has good accuracy and standard deviation percentages on both test and train data. Still is not the best choice
 compared to the other models, but not a bad model
 
 
                                         RANDOM FOREST CLASSIFICATION 
 Just like decision tree classification,Random Forest Classification has good results but is not the best choice still. 
 With the n_estmates parameter, trees lower than 10 gives worse accuracy with higher standard deviation. Trees higher
 than 10 are also good, but then the amount of data per tree decreases, and overfitting can be possible
 
 
                                            CONCLUSION/BEST MODEL
 Overall, no model was bad in terms of cross validation results. Both the training and test data had relatively close 
 accuracy and standard deviation, indicating that there was no over/underfitting. The best model to predict tumor states
given the datset is the linear SVC. It had a very high accuracy percentage. Although the logistic regression had a 
 slightly higher accuracy, Linear SVC had a lower standard deviation. Linear models worked the best for this dataset
showing that the datset was linearly seperable
