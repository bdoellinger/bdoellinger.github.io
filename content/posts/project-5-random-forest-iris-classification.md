---
date: 2021-03-01T10:00:55-04:00
description: "A simple classification app that determines to which category an iris flower with specific parameters belongs to."
featured_image: "/images/project_5_Classificatoin_Iris_Versicolor_image.jpg"
title: "Project 5: Classic Iris Classification"
---

* libraries: streamlit, pandas, PIL, sklearn, pickle

A classic example for classification is the iris dataset. Given a iris flower with specific parameters:
sepal length, sepal width, petal length and petal width, we want to determine to which category this specific iris flower belongs (Setosa, Versicolor or Virginica?).
This problem can be approached by using the iris data set, containing data of already classified samples (columns: sepal length, sepal width, petal length, petal width, category).
Possible strategies for a model with reasonable accuracy are for example: Decision Tree, Random Forest, K-Means Clustering or K-Nearest Neighbors.

This project uses a random forest classifier (since this model receives a good accuracy) that has been prebuilt using sklearn and saved using pickle (and hence doesn't have to be rebuilt every time we use the application).
The user can specify the parameters of a iris flower in the streamlit UI, the random forest classifier is then loaded and used to make and display the most likely prediction for the given parameter.

{{< figure src="/images/project_5_classification_iris_screenshot.png" >}}

[Link to GitHub Repository](https://github.com/bdoellinger/)

[Run application directly with Heroku](https://dashboard.heroku.com/apps/bd-project-05-iris)
(if application isn't currently active on the server, starting might take a while)
