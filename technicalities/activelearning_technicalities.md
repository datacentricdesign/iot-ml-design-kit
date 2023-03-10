---
layout: default
title: Active Learning Technicalities
nav_order: 1
parent: "Technicalities"
has_children: false
---

# Active Learning Technicalities

The technique used to train models is called active learning. The way it generally works is by selecting a couple of starting points you will label, then using an algorithm to find and label the least certain points. 

To select the starting points, a combination of functions is used. One function that randomly selects starting points, and another that uses an algorithm to find certain data points. This algorithm is called k-means clustering, and it works like this: in the first iteration, all points get assigned a certain label. All data points with the same label, belong to the same cluster. Based on information contained in each data point, the algorithm is able to compute an average over all the points in a specific cluster. 

An example to clarify: say you recorded 3 different activities, preprocessed the data, and fed it to a k-means algorithm. For the algorithm to assign labels, it will pick either one of the 3 activities you recorded. So we have labels 1, 2 or 3. To keep it simple, we’ll say we had a dataset of 30 points, 2 features, and a true distribution that’s 10-10-10. In the first iteration, imagine 3 points got assigned label 1. Each feature has a numeric value, so all we have to do is compute the average of feature 1 and feature 2 (3 points, so we sum them and divide by 3). This information makes for another data point, and it’s called a cluster center. The cluster centers get computed for cluster 1, 2 and 3. Because it has the same structure as the other points, we can compute the distance from its center for each point in all clusters. K-means will optimize its predictions by reassigning points so that the distances get smaller in each iteration. This is the final result that we observe. If a point lies exactly on its cluster center, we are the most certain that it belongs to that specific cluster. The further it lies from the center, the more chance that it could actually belong to another cluster (and k-means made a wrong prediction). To minimize iterations, the active learning pipeline should start with the most certain points. They get detected first, and combined with the other function each activity gets selected to be a part of the initial training data. After this, a model gets trained on this training data.

This model will make predictions for all those points you didn’t label. Points being assigned to a class, or activity, in this particular case, is a process called classification. Classification is basically predicting what class a data point belongs to. From classification we can obtain a score that tells us how certain the prediction is. You are asked to label the least certain point to add to the training data, and retrain the model from before using this added point. To keep it simple, we’ll spare you the details of how the least certain sample is actually computed. The result however, will show that the model will make increasingly better predictions with every iteration. 
