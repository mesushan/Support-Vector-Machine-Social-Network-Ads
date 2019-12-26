# Support-Vector-Machine-Social-Network-Ads
Using Support Vector Machine (SVM) with linear and non-linear kernel to make the prediction and compare the difference

## Problem

Suppose a company is going to launch a new campaign for their new brand of car and want to know which category of people are likely to buy their brand new car so they can have the ads that target those peoples. For this they contacted a social network advertising company which have the data from another similar successful campaign. Now, they want to make a model which helps achieve their goal.

## Dataset

The dataset contains 400 entries which contains the userId, gender, age, estimatedsalary and the purchased history. The matric of features taken into account are age and estimated salary which are going to predict if the user is going to buy new car or not(1=Yes, 0=No).

## Solution

First the pre-processing of data is done and then the prediction is done using Support Vector Machine (SVM) and kernel SVM. The confusion matrix and visualization clearly shows the prediction made by both models and the difference.. The dataset is split into 75/25 ratio (training set = 0.75 & test set = 0.25).

The confusion matrix with SVM (linear kernel) shows that our model predicts 90 correct and 10 wrong decisions which shows 90% accuracy.

![cm_svm](https://user-images.githubusercontent.com/14214659/71461542-dc32bd80-27b8-11ea-853e-8a09cb857ab3.png)

The confusion matrix with kernle SVM shows that our model predicts 93 correct and 7 wrong decisions which shows 93% accuracy.

![cm_kernel_svm](https://user-images.githubusercontent.com/14214659/71461571-ed7bca00-27b8-11ea-9e96-ad2e6e55c9ab.png)

The data visualization of the training set and test set is given below. As in the svm the kernel was selected as linear, the graph is linear with a straight line whereas kerel svm deals with non-linear data, the graph is non-linear (curve). The green dots shows the people buying the car whereas red dots shows the people not buying the car. The green dots on the green region shows the true positive  whereas the red dots on the red region shows the true negative. The wrongly classified are the green dots in the red region (false negative) and the red dots in the green region (false positive).

![SVM (Training set)](https://user-images.githubusercontent.com/14214659/71461589-06847b00-27b9-11ea-941c-6500f79b1875.png)

![SVM (Test set)](https://user-images.githubusercontent.com/14214659/71461612-18661e00-27b9-11ea-8165-a7838cd113e2.png)

![Kernel SVM (Training set)](https://user-images.githubusercontent.com/14214659/71461621-261ba380-27b9-11ea-81d2-17e55d8f5c50.png)

![Kernel SVM (Test set)](https://user-images.githubusercontent.com/14214659/71461640-35025600-27b9-11ea-8b21-24f4595307b8.png)


## Conclusion
Fromt the two models, it is clear that for this dataset, the non-linear kernel (default) is better than the linear kernel svm as it predicts more accurately and the graph shows that too.
